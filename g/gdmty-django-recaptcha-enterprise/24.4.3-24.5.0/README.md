# Comparing `tmp/gdmty-django-recaptcha-enterprise-24.4.3.tar.gz` & `tmp/gdmty_django_recaptcha_enterprise-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmty-django-recaptcha-enterprise-24.4.3.tar", last modified: Fri Mar 15 04:20:08 2024, max compression
+gzip compressed data, was "gdmty_django_recaptcha_enterprise-24.5.0.tar", last modified: Thu May  9 15:00:33 2024, max compression
```

## Comparing `gdmty-django-recaptcha-enterprise-24.4.3.tar` & `gdmty_django_recaptcha_enterprise-24.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 04:20:08.896491 gdmty-django-recaptcha-enterprise-24.4.3/
--rw-rw-rw-   0        0        0    11656 2024-03-15 03:59:12.000000 gdmty-django-recaptcha-enterprise-24.4.3/LICENSE
--rw-rw-rw-   0        0        0       53 2024-03-15 03:59:12.000000 gdmty-django-recaptcha-enterprise-24.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0    17515 2024-03-15 04:20:08.896491 gdmty-django-recaptcha-enterprise-24.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     2969 2024-03-15 03:59:12.000000 gdmty-django-recaptcha-enterprise-24.4.3/README.md
--rw-rw-rw-   0        0        0     1690 2024-03-15 04:19:47.000000 gdmty-django-recaptcha-enterprise-24.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-15 04:20:08.896491 gdmty-django-recaptcha-enterprise-24.4.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-15 04:20:08.878007 gdmty-django-recaptcha-enterprise-24.4.3/src/
-drwxrwxrwx   0        0        0        0 2024-03-15 04:20:08.887565 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/
--rw-rw-rw-   0        0        0      801 2024-03-15 04:19:47.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/__init__.py
--rw-rw-rw-   0        0        0       66 2024-03-15 03:59:12.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/admin.py
--rw-rw-rw-   0        0        0      201 2024-03-15 03:59:12.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/apps.py
--rw-rw-rw-   0        0        0      979 2024-03-15 03:59:12.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/decorators.py
-drwxrwxrwx   0        0        0        0 2024-03-15 04:20:08.893945 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/migrations/
--rw-rw-rw-   0        0        0        0 2024-03-15 03:59:12.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2024-03-15 03:59:12.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/models.py
--rw-rw-rw-   0        0        0     4238 2024-03-15 03:59:12.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/recaptcha.py
--rw-rw-rw-   0        0        0       63 2024-03-15 03:59:12.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/tests.py
--rw-rw-rw-   0        0        0       66 2024-03-15 03:59:12.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/views.py
-drwxrwxrwx   0        0        0        0 2024-03-15 04:20:08.893945 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise.egg-info/
--rw-rw-rw-   0        0        0    17515 2024-03-15 04:20:08.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      797 2024-03-15 04:20:08.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 04:20:08.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2024-03-15 04:20:08.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise.egg-info/requires.txt
--rw-rw-rw-   0        0        0       34 2024-03-15 04:20:08.000000 gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 15:00:33.703138 gdmty_django_recaptcha_enterprise-24.5.0/
+-rw-rw-rw-   0        0        0    11656 2024-03-15 03:59:12.000000 gdmty_django_recaptcha_enterprise-24.5.0/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-03-15 03:59:12.000000 gdmty_django_recaptcha_enterprise-24.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    17817 2024-05-09 15:00:33.703138 gdmty_django_recaptcha_enterprise-24.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3271 2024-05-09 14:59:36.000000 gdmty_django_recaptcha_enterprise-24.5.0/README.md
+-rw-rw-rw-   0        0        0     1690 2024-05-09 15:00:07.000000 gdmty_django_recaptcha_enterprise-24.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 15:00:33.703138 gdmty_django_recaptcha_enterprise-24.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 15:00:33.685226 gdmty_django_recaptcha_enterprise-24.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 15:00:33.695551 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/
+-rw-rw-rw-   0        0        0      801 2024-05-09 15:00:07.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-03-15 03:59:12.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/admin.py
+-rw-rw-rw-   0        0        0      201 2024-03-15 03:59:12.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/apps.py
+-rw-rw-rw-   0        0        0      977 2024-05-09 14:48:31.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/decorators.py
+drwxrwxrwx   0        0        0        0 2024-05-09 15:00:33.700150 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/migrations/
+-rw-rw-rw-   0        0        0        0 2024-03-15 03:59:12.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2024-03-15 03:59:12.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/models.py
+-rw-rw-rw-   0        0        0     4238 2024-03-15 03:59:12.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/recaptcha.py
+-rw-rw-rw-   0        0        0       63 2024-03-15 03:59:12.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/tests.py
+-rw-rw-rw-   0        0        0       66 2024-03-15 03:59:12.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/views.py
+drwxrwxrwx   0        0        0        0 2024-05-09 15:00:33.701607 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise.egg-info/
+-rw-rw-rw-   0        0        0    17817 2024-05-09 15:00:33.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2024-05-09 15:00:33.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 15:00:33.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2024-05-09 15:00:33.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2024-05-09 15:00:33.000000 gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise.egg-info/top_level.txt
```

### Comparing `gdmty-django-recaptcha-enterprise-24.4.3/LICENSE` & `gdmty_django_recaptcha_enterprise-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdmty-django-recaptcha-enterprise-24.4.3/PKG-INFO` & `gdmty_django_recaptcha_enterprise-24.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-django-recaptcha-enterprise
-Version: 24.4.3
+Version: 24.5.0
 Summary: Library for Django that implements Google's reCaptcha Enterprise
 Author-email: César Benjamín <mathereall@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -252,23 +252,25 @@
 INSTALLED_APPS = [
     ...,
     'gdmty_django_recaptcha_enterprise',
     ...
 ]
 
 # Set the following variables 
-RECAPTCHA_CREDENTIALS_SERVICE_ACCOUNT_FILE = os.path.join(BASE_DIR, "_gcp_sa", "recaptcha_enterprise_service_account_key.json")
-credentials = service_account.Credentials.from_service_account_file(RECAPTCHA_CREDENTIALS_SERVICE_ACCOUNT_FILE)
 RECAPTCHA_ENTERPRISE_PROJECT_ID = 'your-project-id'
-RECAPTCHA_ENTERPRISE_SERVICE_ACCOUNT_CREDENTIALS = credentials
+
 RECAPTCHA_ENTERPRISE_SITE_KEY_VERIFY = 'your-site-key' # This one is the site key for usage with seamless verification with the reCaptcha Enterprise API withouth user interaction
 RECAPTCHA_ENTERPRISE_SITE_KEY_CHALLENGE = 'your-site-key' # This one is the site key for usage with challenge verification with the reCaptcha Enterprise API with user interaction
 RECAPTCHA_ENTERPRISE_BYPASS_TOKEN = 'your-bypass-token' # Optional, only for debug and development usage. For production must be False. When DEBUG=False this must be False too or will not pass assesments never.
 
+RECAPTCHA_CREDENTIALS_SERVICE_ACCOUNT = your-service-account
+credentials = service_account.Credentials.from_service_account_info(RECAPTCHA_CREDENTIALS_SERVICE_ACCOUNT)
+RECAPTCHA_ENTERPRISE_SERVICE_ACCOUNT_CREDENTIALS = credentials
 
+# from_service_account_info() is a method from Credentials class that creates a Credentials object from a service account from a dictionary. You can use a json file with the service account info and load it with json.load to get the dictionary. or use from_service_account_file() method from Credentials class to load the json file and get the Credentials object directly.
 ```
 
 In your code:
 
 ```python
 # import assess_token from gdmty_django_recaptcha_enterprise.recaptcha, then you can use it to assess tokens where you need it. In this excample we show a hypothetical view that receives a token from a POST request.
 # You can use the decorator requires_recaptcha to verify the token before the view is executed.
@@ -287,9 +289,8 @@
 # When the decorator is used, the decorator handles de request to get the token from the request and assess it, if the token is valid the view is executed, if not, the view is not executed and a 403 response is returned.
 # 
 @requires_recaptcha(action='action-to-verify')
 def my_view(request):
     ...
     pass
     ...
-
 ```
```

### Comparing `gdmty-django-recaptcha-enterprise-24.4.3/README.md` & `gdmty_django_recaptcha_enterprise-24.5.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -22,23 +22,25 @@
 INSTALLED_APPS = [
     ...,
     'gdmty_django_recaptcha_enterprise',
     ...
 ]
 
 # Set the following variables 
-RECAPTCHA_CREDENTIALS_SERVICE_ACCOUNT_FILE = os.path.join(BASE_DIR, "_gcp_sa", "recaptcha_enterprise_service_account_key.json")
-credentials = service_account.Credentials.from_service_account_file(RECAPTCHA_CREDENTIALS_SERVICE_ACCOUNT_FILE)
 RECAPTCHA_ENTERPRISE_PROJECT_ID = 'your-project-id'
-RECAPTCHA_ENTERPRISE_SERVICE_ACCOUNT_CREDENTIALS = credentials
+
 RECAPTCHA_ENTERPRISE_SITE_KEY_VERIFY = 'your-site-key' # This one is the site key for usage with seamless verification with the reCaptcha Enterprise API withouth user interaction
 RECAPTCHA_ENTERPRISE_SITE_KEY_CHALLENGE = 'your-site-key' # This one is the site key for usage with challenge verification with the reCaptcha Enterprise API with user interaction
 RECAPTCHA_ENTERPRISE_BYPASS_TOKEN = 'your-bypass-token' # Optional, only for debug and development usage. For production must be False. When DEBUG=False this must be False too or will not pass assesments never.
 
+RECAPTCHA_CREDENTIALS_SERVICE_ACCOUNT = your-service-account
+credentials = service_account.Credentials.from_service_account_info(RECAPTCHA_CREDENTIALS_SERVICE_ACCOUNT)
+RECAPTCHA_ENTERPRISE_SERVICE_ACCOUNT_CREDENTIALS = credentials
 
+# from_service_account_info() is a method from Credentials class that creates a Credentials object from a service account from a dictionary. You can use a json file with the service account info and load it with json.load to get the dictionary. or use from_service_account_file() method from Credentials class to load the json file and get the Credentials object directly.
 ```
 
 In your code:
 
 ```python
 # import assess_token from gdmty_django_recaptcha_enterprise.recaptcha, then you can use it to assess tokens where you need it. In this excample we show a hypothetical view that receives a token from a POST request.
 # You can use the decorator requires_recaptcha to verify the token before the view is executed.
@@ -57,9 +59,8 @@
 # When the decorator is used, the decorator handles de request to get the token from the request and assess it, if the token is valid the view is executed, if not, the view is not executed and a 403 response is returned.
 # 
 @requires_recaptcha(action='action-to-verify')
 def my_view(request):
     ...
     pass
     ...
-
 ```
```

### Comparing `gdmty-django-recaptcha-enterprise-24.4.3/pyproject.toml` & `gdmty_django_recaptcha_enterprise-24.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gdmty-django-recaptcha-enterprise"
-version = "24.4.3"
+version = "24.5.0"
 description = "Library for Django that implements Google's reCaptcha Enterprise"
 readme = "README.md"
 authors = [{ name = "César Benjamín", email = "mathereall@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
@@ -32,15 +32,15 @@
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 "Homepage" = "https://github.com/gobiernodigitalmonterrey/gdmty-django-recaptcha-enterprise"
 "Bug Tracker" = "https://github.com/gobiernodigitalmonterrey/gdmty-django-recaptcha-enterprise/issues"
 
 [tool.bumpver]
-current_version = "24.4.3"
+current_version = "24.5.0"
 version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/__init__.py` & `gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     if assess_token(token, action):
         # do something
         ...
 
 """
 
 __title__ = "gdmty_django_recaptcha_enterprise"
-__version__ = "24.4.3"
+__version__ = "24.5.0"
 __description__ = "reCAPTCHA Enterprise's Django module for verifying reCAPTCHA tokens"
 __url__ = "https://github.com/SIGAMty/gdmty-django-recaptcha-enterprise"
 __author__ = "César Benjamín"
 __author_email__ = "mathereall@gmail.com"
 __license__ = "Apache 2.0"
 __keywords__ = ["django", "recaptcha", "enterprise", "google"]
 VERSION = __version__
```

### Comparing `gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/decorators.py` & `gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,7 @@
                 return HttpResponseForbidden("Petición inválida")
 
             return view_func(request, *args, **kwargs)
 
         return _wrapped_view
 
     return decorator
-
```

### Comparing `gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise/recaptcha.py` & `gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise/recaptcha.py`

 * *Files identical despite different names*

### Comparing `gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise.egg-info/PKG-INFO` & `gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdmty-django-recaptcha-enterprise
-Version: 24.4.3
+Version: 24.5.0
 Summary: Library for Django that implements Google's reCaptcha Enterprise
 Author-email: César Benjamín <mathereall@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -252,23 +252,25 @@
 INSTALLED_APPS = [
     ...,
     'gdmty_django_recaptcha_enterprise',
     ...
 ]
 
 # Set the following variables 
-RECAPTCHA_CREDENTIALS_SERVICE_ACCOUNT_FILE = os.path.join(BASE_DIR, "_gcp_sa", "recaptcha_enterprise_service_account_key.json")
-credentials = service_account.Credentials.from_service_account_file(RECAPTCHA_CREDENTIALS_SERVICE_ACCOUNT_FILE)
 RECAPTCHA_ENTERPRISE_PROJECT_ID = 'your-project-id'
-RECAPTCHA_ENTERPRISE_SERVICE_ACCOUNT_CREDENTIALS = credentials
+
 RECAPTCHA_ENTERPRISE_SITE_KEY_VERIFY = 'your-site-key' # This one is the site key for usage with seamless verification with the reCaptcha Enterprise API withouth user interaction
 RECAPTCHA_ENTERPRISE_SITE_KEY_CHALLENGE = 'your-site-key' # This one is the site key for usage with challenge verification with the reCaptcha Enterprise API with user interaction
 RECAPTCHA_ENTERPRISE_BYPASS_TOKEN = 'your-bypass-token' # Optional, only for debug and development usage. For production must be False. When DEBUG=False this must be False too or will not pass assesments never.
 
+RECAPTCHA_CREDENTIALS_SERVICE_ACCOUNT = your-service-account
+credentials = service_account.Credentials.from_service_account_info(RECAPTCHA_CREDENTIALS_SERVICE_ACCOUNT)
+RECAPTCHA_ENTERPRISE_SERVICE_ACCOUNT_CREDENTIALS = credentials
 
+# from_service_account_info() is a method from Credentials class that creates a Credentials object from a service account from a dictionary. You can use a json file with the service account info and load it with json.load to get the dictionary. or use from_service_account_file() method from Credentials class to load the json file and get the Credentials object directly.
 ```
 
 In your code:
 
 ```python
 # import assess_token from gdmty_django_recaptcha_enterprise.recaptcha, then you can use it to assess tokens where you need it. In this excample we show a hypothetical view that receives a token from a POST request.
 # You can use the decorator requires_recaptcha to verify the token before the view is executed.
@@ -287,9 +289,8 @@
 # When the decorator is used, the decorator handles de request to get the token from the request and assess it, if the token is valid the view is executed, if not, the view is not executed and a 403 response is returned.
 # 
 @requires_recaptcha(action='action-to-verify')
 def my_view(request):
     ...
     pass
     ...
-
 ```
```

### Comparing `gdmty-django-recaptcha-enterprise-24.4.3/src/gdmty_django_recaptcha_enterprise.egg-info/SOURCES.txt` & `gdmty_django_recaptcha_enterprise-24.5.0/src/gdmty_django_recaptcha_enterprise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

