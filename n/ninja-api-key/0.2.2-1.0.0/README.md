# Comparing `tmp/ninja_api_key-0.2.2.tar.gz` & `tmp/ninja_api_key-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninja_api_key-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ninja_api_key-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ninja_api_key-0.2.2.tar` & `ninja_api_key-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     2508 2024-05-08 14:39:33.267017 ninja_api_key-0.2.2/README.md
--rw-r--r--   0        0        0       96 2024-05-08 14:39:33.267017 ninja_api_key-0.2.2/ninja_apikey/__init__.py
--rw-r--r--   0        0        0     1429 2024-05-08 14:39:33.267017 ninja_api_key-0.2.2/ninja_apikey/admin.py
--rw-r--r--   0        0        0      185 2024-05-08 14:39:33.271017 ninja_api_key-0.2.2/ninja_apikey/apps.py
--rw-r--r--   0        0        0     1364 2024-05-08 14:39:33.271017 ninja_api_key-0.2.2/ninja_apikey/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-08 14:39:33.271017 ninja_api_key-0.2.2/ninja_apikey/migrations/__init__.py
--rw-r--r--   0        0        0      968 2024-05-08 14:39:33.271017 ninja_api_key-0.2.2/ninja_apikey/models.py
--rw-r--r--   0        0        0     1676 2024-05-08 14:39:33.271017 ninja_api_key-0.2.2/ninja_apikey/security.py
--rw-r--r--   0        0        0     3078 2024-05-08 14:39:33.271017 ninja_api_key-0.2.2/ninja_apikey/tests.py
--rw-r--r--   0        0        0     1826 2024-05-08 14:39:33.271017 ninja_api_key-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4550 1970-01-01 00:00:00.000000 ninja_api_key-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1690 2024-05-09 20:14:39.346975 ninja_api_key-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 20:14:39.346975 ninja_api_key-1.0.0/ninja_apikey/__init__.py
+-rw-r--r--   0        0        0     1291 2024-05-09 20:14:39.346975 ninja_api_key-1.0.0/ninja_apikey/admin.py
+-rw-r--r--   0        0        0      185 2024-05-09 20:14:39.346975 ninja_api_key-1.0.0/ninja_apikey/apps.py
+-rw-r--r--   0        0        0     1588 2024-05-09 20:14:39.346975 ninja_api_key-1.0.0/ninja_apikey/hashers.py
+-rw-r--r--   0        0        0     1364 2024-05-09 20:14:39.346975 ninja_api_key-1.0.0/ninja_apikey/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-09 20:14:39.346975 ninja_api_key-1.0.0/ninja_apikey/migrations/__init__.py
+-rw-r--r--   0        0        0      953 2024-05-09 20:14:39.346975 ninja_api_key-1.0.0/ninja_apikey/models.py
+-rw-r--r--   0        0        0     1660 2024-05-09 20:14:39.346975 ninja_api_key-1.0.0/ninja_apikey/security.py
+-rw-r--r--   0        0        0     1856 2024-05-09 20:14:39.346975 ninja_api_key-1.0.0/ninja_apikey/tests/test_hashers_sha256.py
+-rw-r--r--   0        0        0     3099 2024-05-09 20:14:39.346975 ninja_api_key-1.0.0/ninja_apikey/tests/test_security.py
+-rw-r--r--   0        0        0     1836 2024-05-09 20:14:39.346975 ninja_api_key-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 ninja_api_key-1.0.0/PKG-INFO
```

### Comparing `ninja_api_key-0.2.2/ninja_apikey/admin.py` & `ninja_api_key-1.0.0/ninja_apikey/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from django.contrib import admin, messages
 
 from .models import APIKey
 from .security import generate_key
 
 
-@admin.action(description="Revoke selected API keys")  # type: ignore
+@admin.action(description="Revoke selected API keys")
 def revoke_key(modeladmin, request, queryset):
-    queryset.update(revoked=True)  # pragma: no cover
+    queryset.update(revoked=True)
 
 
 @admin.register(APIKey)
 class APIKeyAdmin(admin.ModelAdmin):
     list_display = [
         "prefix",
         "user",
@@ -20,28 +20,28 @@
         "revoked",
         "is_active",
     ]
     readonly_fields = ["prefix", "hashed_key", "created_at"]
     actions = [revoke_key]
     list_filter = ["revoked"]
 
-    @admin.display  # type: ignore
+    @admin.display
     def is_active(self, obj: APIKey):
-        return obj.is_valid  # pragma: no cover
+        return obj.is_valid
 
-    is_active.boolean = True  # Display property as boolean
+    is_active.boolean = True
 
     def save_model(self, request, obj: APIKey, form, change):
-        if not obj.prefix:  # New API key
+        if not obj.prefix:
             key = generate_key()
             obj.prefix = key.prefix
             obj.hashed_key = key.hashed_key
 
             if request:
-                messages.add_message(  # pragma: no cover
+                messages.add_message(
                     request,
                     messages.WARNING,
                     f"The API key for {obj} is '{key.prefix}.{key.key}'."
                     "You should store it somewhere safe: "
                     "you will not be able to see the key again.",
                 )
```

### Comparing `ninja_api_key-0.2.2/ninja_apikey/migrations/0001_initial.py` & `ninja_api_key-1.0.0/ninja_apikey/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ninja_api_key-0.2.2/ninja_apikey/models.py` & `ninja_api_key-1.0.0/ninja_apikey/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# type: ignore
 from django.contrib.auth import get_user_model
 from django.db import models
 from django.utils import timezone
 
 
 class APIKey(models.Model):
     prefix = models.CharField(max_length=8, primary_key=True)
```

### Comparing `ninja_api_key-0.2.2/ninja_apikey/security.py` & `ninja_api_key-1.0.0/ninja_apikey/security.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Optional
 
 from django.contrib.auth.hashers import check_password, make_password
 from django.http import HttpRequest
 from django.utils.crypto import get_random_string
 from ninja.security import APIKeyHeader
 
-from .models import APIKey  # type: ignore
+from .models import APIKey
 
 KeyData = namedtuple("KeyData", "prefix key hashed_key")
 
 
 def generate_key() -> KeyData:
     prefix = get_random_string(8)
     key = get_random_string(56)
```

### Comparing `ninja_api_key-0.2.2/ninja_apikey/tests.py` & `ninja_api_key-1.0.0/ninja_apikey/tests/test_security.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-# flake8: noqa
 from datetime import timedelta
 
 import pytest
 from django.contrib.admin.sites import AdminSite
 from django.contrib.auth.hashers import (
     PBKDF2PasswordHasher,
     check_password,
     make_password,
 )
 from django.contrib.auth.models import User
 from django.utils import timezone
 from django.utils.crypto import get_random_string
 
-from .admin import APIKeyAdmin
-from .models import APIKey
-from .security import check_apikey, generate_key
+from ninja_apikey.admin import APIKeyAdmin
+from ninja_apikey.models import APIKey
+from ninja_apikey.security import check_apikey, generate_key
 
 
 def test_apikey_validation():
     key = APIKey()
     assert key
     assert key.is_valid
     key.revoked = True
```

### Comparing `ninja_api_key-0.2.2/pyproject.toml` & `ninja_api_key-1.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
+
+
 [project]
 name = "ninja-api-key"
+description = "Django Ninja API Key Authentication"
+version = "1.0.0"
 authors = [
   {name = "Lucas Rangel Cezimbra", email="lucas@cezimbra.tec.br"},
   {name = "Maximilian Wassink", email="wassink.maximilian@protonmail.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.6.2"
 classifiers = [
@@ -31,33 +35,35 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Security",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-dynamic = ["version", "description"]
 keywords = ["django", "rest", "ninja", "auth", "apikey"]
 dependencies = [
     "django",
     "django-ninja"
 ]
 
 [project.urls]
 Source = "https://github.com/lucasrcezimbra/ninja-api-key"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "pytest-cov",
     "pytest-django",
-    "black",
-    "isort",
-    "flake8",
-    "flake8-bugbear",
-    "flake8-bandit",
-    "mypy",
-    "django-stubs",
-    ]
+]
+
+
 
 [tool.flit.module]
 name = "ninja_apikey"
+
+
+[tool.ruff]
+line-length = 88
+
+[tool.ruff.lint]
+select = ["E", "F", "I"]
+ignore = ["E501"]
```

### Comparing `ninja_api_key-0.2.2/PKG-INFO` & `ninja_api_key-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ninja-api-key
-Version: 0.2.2
-Summary: Easy to use API key authentication for Django Ninja REST Framework
+Version: 1.0.0
+Summary: Django Ninja API Key Authentication
 Keywords: django,rest,ninja,auth,apikey
 Author-email: Lucas Rangel Cezimbra <lucas@cezimbra.tec.br>, Maximilian Wassink <wassink.maximilian@protonmail.com>
 Requires-Python: >=3.6.2
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
@@ -30,109 +30,106 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django
 Requires-Dist: django-ninja
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-django ; extra == "test"
-Requires-Dist: black ; extra == "test"
-Requires-Dist: isort ; extra == "test"
-Requires-Dist: flake8 ; extra == "test"
-Requires-Dist: flake8-bugbear ; extra == "test"
-Requires-Dist: flake8-bandit ; extra == "test"
-Requires-Dist: mypy ; extra == "test"
-Requires-Dist: django-stubs ; extra == "test"
 Project-URL: Source, https://github.com/lucasrcezimbra/ninja-api-key
 Provides-Extra: test
 
-<div align="center">
-    <h3>Django Ninja APIKey</h3>
-    <em>Easy to use API key authentication for Django Ninja REST Framework</em>
-</div>
-<br>
-<div align="center">
-    <p>
-        <a href="https://github.com/mawassk/django-ninja-apikey/actions/workflows/build.yml?query=branch%3Amain++" target="_blank">
-            <img src="https://github.com/mawassk/django-ninja-apikey/workflows/build/badge.svg?branch=main" alt="build">
-        </a>
-        <a href="https://codecov.io/gh/mawassk/django-ninja-apikey" target="_blank">
-            <img src="https://img.shields.io/codecov/c/github/mawassk/django-ninja-apikey?color=%2334D058" alt="coverage">
-        </a>
-        <a href="https://pypi.org/project/django-ninja-apikey/">
-            <img src="https://img.shields.io/pypi/v/django-ninja-apikey?color=%2334D058&label=pypi%20package" alt="pypi">
-        </a>
-        <a href="https://github.com/psf/black" target="_blank">
-            <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="black">
-        </a>
-    </p>
-</div>
-
----
-
-This is an unofficial [Django](https://github.com/django/django) app which makes it **easy** to manage API keys for the [Django Ninja REST Framework](https://github.com/vitalik/django-ninja).
-
-**Key Features:**
-- **Easy** integration in your projects
-- Well integrated in the **admin interface**
-- **Secure** API keys due to hashing
-- Works with the **standard** user model
+# Ninja API Key
+
+
+[![PyPI](https://img.shields.io/pypi/v/ninja-api-key.svg)](https://pypi.python.org/pypi/ninja-api-key)
+
+[![codecov](https://codecov.io/gh/lucasrcezimbra/ninja-api-key/graph/badge.svg)](https://codecov.io/gh/lucasrcezimbra/ninja-api-key)
+
+
+API Key authentication for [Django Ninja](https://django-ninja.dev/).
+
+This is a fork from [django-ninja-apikey](https://github.com/mawassk/django-ninja-apikey).
+
+Key Features:
+- Easy integration into your projects
+- Well integrated with the Admin interface
+- Secure API keys due to hashing
+- Works with the standard user model
+
 
 ## Installation
 
+```bash
+pip install ninja-api-key
 ```
-pip install django-ninja-apikey
-```
 
-## Usage
-Add `ninja_apikey` to your installed apps in your django project:
+
+## How to use
+1. Add `ninja_apikey` to your installed apps in your Django project:
 ```Python
 # settings.py
 
 INSTALLED_APPS = [
     # ...
     "ninja_apikey",
 ]
 ```
-Run the included migrations:
-```
+
+2. Apply migrations
+```shell
 python manage.py migrate
 ```
-Secure an api endpoint with the API keys:
+
+3. Secure
+
+a. the whole API
 ```Python
 # api.py
 
 from ninja import NinjaAPI
 from ninja_apikey.security import APIKeyAuth
 
 #  ...
 
-auth = APIKeyAuth()
-api = NinjaAPI()
+api = NinjaAPI(auth=APIKeyAuth())
 
 # ...
 
-@api.get("/secure_endpoint", auth=auth)
+@api.get("/secure_endpoint")
 def secure_endpoint(request):
     return f"Hello, {request.user}!"
 ```
-Or secure your whole api (or a specific [router](https://django-ninja.rest-framework.com/tutorial/routers/)) with the API keys:
+
+b. an specific endpoint
 ```Python
 # api.py
 
 from ninja import NinjaAPI
 from ninja_apikey.security import APIKeyAuth
 
 #  ...
 
-api = NinjaAPI(auth=APIKeyAuth())
+auth = APIKeyAuth()
+api = NinjaAPI()
 
 # ...
 
-@api.get("/secure_endpoint")
+@api.get("/secure_endpoint", auth=auth)
 def secure_endpoint(request):
     return f"Hello, {request.user}!"
 ```
-You can create now API keys from django's admin interface.
 
-## License
-This project is licensed under the terms of the MIT license.
+
+## Contributing
+
+Contributions are welcome, feel free to open an Issue or Pull Request.
+
+```
+git clone https://github.com/lucasrcezimbra/ninja-api-key
+cd ninja-api-key
+python -m venv .venv
+source .venv/bin/activate
+pip install .[test]
+pre-commit install
+make test
+```
```

