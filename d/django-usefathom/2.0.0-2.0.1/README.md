# Comparing `tmp/django_usefathom-2.0.0.tar.gz` & `tmp/django_usefathom-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_usefathom-2.0.0.tar", max compression
+gzip compressed data, was "django_usefathom-2.0.1.tar", max compression
```

## Comparing `django_usefathom-2.0.0.tar` & `django_usefathom-2.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2022-12-10 08:20:04.474860 django_usefathom-2.0.0/LICENSE
--rw-r--r--   0        0        0     1816 2024-05-07 04:18:01.714122 django_usefathom-2.0.0/README.md
--rw-r--r--   0        0        0      534 2024-05-08 02:28:02.491224 django_usefathom-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       78 2022-12-10 08:20:04.475683 django_usefathom-2.0.0/usefathom/__init__.py
--rw-r--r--   0        0        0      942 2024-05-07 03:58:16.406711 django_usefathom-2.0.0/usefathom/api.py
--rw-r--r--   0        0        0      147 2022-12-10 08:20:04.475887 django_usefathom-2.0.0/usefathom/apps.py
--rw-r--r--   0        0        0      194 2024-05-07 04:18:26.919739 django_usefathom-2.0.0/usefathom/context_processors.py
--rw-r--r--   0        0        0      104 2024-05-07 04:11:00.402889 django_usefathom-2.0.0/usefathom/templates/usefathom/click.html
--rw-r--r--   0        0        0      105 2024-05-07 04:11:15.241497 django_usefathom-2.0.0/usefathom/templates/usefathom/submit.html
--rw-r--r--   0        0        0      482 2024-05-07 04:18:39.450681 django_usefathom-2.0.0/usefathom/templates/usefathom/usefathom.html
--rw-r--r--   0        0        0      543 2024-05-07 04:10:45.604051 django_usefathom-2.0.0/usefathom/templatetags/fathom.py
--rw-r--r--   0        0        0       60 2022-12-10 08:20:04.476703 django_usefathom-2.0.0/usefathom/tests.py
--rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 django_usefathom-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-12-10 08:20:04.474860 django_usefathom-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1816 2024-05-07 04:18:01.714122 django_usefathom-2.0.1/README.md
+-rw-r--r--   0        0        0      518 2024-05-09 05:20:12.782440 django_usefathom-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-05-09 05:17:48.170058 django_usefathom-2.0.1/usefathom/__init__.py
+-rw-r--r--   0        0        0      942 2024-05-07 03:58:16.406711 django_usefathom-2.0.1/usefathom/api.py
+-rw-r--r--   0        0        0      147 2022-12-10 08:20:04.475887 django_usefathom-2.0.1/usefathom/apps.py
+-rw-r--r--   0        0        0      194 2024-05-07 04:18:26.919739 django_usefathom-2.0.1/usefathom/context_processors.py
+-rw-r--r--   0        0        0      104 2024-05-07 04:11:00.402889 django_usefathom-2.0.1/usefathom/templates/usefathom/click.html
+-rw-r--r--   0        0        0      105 2024-05-07 04:11:15.241497 django_usefathom-2.0.1/usefathom/templates/usefathom/submit.html
+-rw-r--r--   0        0        0      482 2024-05-07 04:18:39.450681 django_usefathom-2.0.1/usefathom/templates/usefathom/usefathom.html
+-rw-r--r--   0        0        0      543 2024-05-07 04:10:45.604051 django_usefathom-2.0.1/usefathom/templatetags/fathom.py
+-rw-r--r--   0        0        0       60 2022-12-10 08:20:04.476703 django_usefathom-2.0.1/usefathom/tests.py
+-rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 django_usefathom-2.0.1/PKG-INFO
```

### Comparing `django_usefathom-2.0.0/LICENSE` & `django_usefathom-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_usefathom-2.0.0/README.md` & `django_usefathom-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django_usefathom-2.0.0/pyproject.toml` & `django_usefathom-2.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "django-usefathom"
-version = "2.0.0"
+version = "2.0.1"
 description = "A Django app to integrate Fathom Analytics into your project"
 authors = ["Paul Chubatyy <xobb@citylance.biz>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/paulchubatyy/django-usefathom"
 packages = [
     { include = "usefathom" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
-twine = "4.0.2"
 docutils = "0.21.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_usefathom-2.0.0/usefathom/api.py` & `django_usefathom-2.0.1/usefathom/api.py`

 * *Files identical despite different names*

### Comparing `django_usefathom-2.0.0/usefathom/templatetags/fathom.py` & `django_usefathom-2.0.1/usefathom/templatetags/fathom.py`

 * *Files identical despite different names*

### Comparing `django_usefathom-2.0.0/PKG-INFO` & `django_usefathom-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-usefathom
-Version: 2.0.0
+Version: 2.0.1
 Summary: A Django app to integrate Fathom Analytics into your project
 Home-page: https://github.com/paulchubatyy/django-usefathom
 License: MIT
 Author: Paul Chubatyy
 Author-email: xobb@citylance.biz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

