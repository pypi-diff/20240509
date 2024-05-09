# Comparing `tmp/django-usefathom-1.2.2.tar.gz` & `tmp/django_usefathom-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-usefathom-1.2.2.tar", last modified: Fri Feb  3 20:38:11 2023, max compression
+gzip compressed data, was "django_usefathom-2.0.0.tar", max compression
```

## Comparing `django-usefathom-1.2.2.tar` & `django_usefathom-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 20:38:11.428299 django-usefathom-1.2.2/
--rw-r--r--   0 root         (0) root         (0)     1077 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      116 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3062 2023-02-03 20:38:11.428557 django-usefathom-1.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2100 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 20:38:11.403649 django-usefathom-1.2.2/django_usefathom.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3062 2023-02-03 20:38:11.000000 django-usefathom-1.2.2/django_usefathom.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2023-02-03 20:38:11.000000 django-usefathom-1.2.2/django_usefathom.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-03 20:38:11.000000 django-usefathom-1.2.2/django_usefathom.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-03 20:38:11.000000 django-usefathom-1.2.2/django_usefathom.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-02-03 20:38:11.000000 django-usefathom-1.2.2/django_usefathom.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      103 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      977 2023-02-03 20:38:11.429408 django-usefathom-1.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       37 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 20:38:11.416596 django-usefathom-1.2.2/usefathom/
--rw-r--r--   0 root         (0) root         (0)       78 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/usefathom/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1152 2023-02-03 20:28:33.000000 django-usefathom-1.2.2/usefathom/api.py
--rw-r--r--   0 root         (0) root         (0)      147 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/usefathom/apps.py
--rw-r--r--   0 root         (0) root         (0)      335 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/usefathom/context_processors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 20:38:11.386871 django-usefathom-1.2.2/usefathom/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 20:38:11.425209 django-usefathom-1.2.2/usefathom/templates/usefathom/
--rw-r--r--   0 root         (0) root         (0)       54 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/usefathom/templates/usefathom/click.html
--rw-r--r--   0 root         (0) root         (0)       55 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/usefathom/templates/usefathom/submit.html
--rw-r--r--   0 root         (0) root         (0)      423 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/usefathom/templates/usefathom/usefathom.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-03 20:38:11.426570 django-usefathom-1.2.2/usefathom/templatetags/
--rw-r--r--   0 root         (0) root         (0)      506 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/usefathom/templatetags/fathom.py
--rw-r--r--   0 root         (0) root         (0)       60 2022-12-10 08:20:04.000000 django-usefathom-1.2.2/usefathom/tests.py
+-rw-r--r--   0        0        0     1077 2022-12-10 08:20:04.474860 django_usefathom-2.0.0/LICENSE
+-rw-r--r--   0        0        0     1816 2024-05-07 04:18:01.714122 django_usefathom-2.0.0/README.md
+-rw-r--r--   0        0        0      534 2024-05-08 02:28:02.491224 django_usefathom-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2022-12-10 08:20:04.475683 django_usefathom-2.0.0/usefathom/__init__.py
+-rw-r--r--   0        0        0      942 2024-05-07 03:58:16.406711 django_usefathom-2.0.0/usefathom/api.py
+-rw-r--r--   0        0        0      147 2022-12-10 08:20:04.475887 django_usefathom-2.0.0/usefathom/apps.py
+-rw-r--r--   0        0        0      194 2024-05-07 04:18:26.919739 django_usefathom-2.0.0/usefathom/context_processors.py
+-rw-r--r--   0        0        0      104 2024-05-07 04:11:00.402889 django_usefathom-2.0.0/usefathom/templates/usefathom/click.html
+-rw-r--r--   0        0        0      105 2024-05-07 04:11:15.241497 django_usefathom-2.0.0/usefathom/templates/usefathom/submit.html
+-rw-r--r--   0        0        0      482 2024-05-07 04:18:39.450681 django_usefathom-2.0.0/usefathom/templates/usefathom/usefathom.html
+-rw-r--r--   0        0        0      543 2024-05-07 04:10:45.604051 django_usefathom-2.0.0/usefathom/templatetags/fathom.py
+-rw-r--r--   0        0        0       60 2022-12-10 08:20:04.476703 django_usefathom-2.0.0/usefathom/tests.py
+-rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 django_usefathom-2.0.0/PKG-INFO
```

### Comparing `django-usefathom-1.2.2/LICENSE` & `django_usefathom-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-usefathom-1.2.2/PKG-INFO` & `django_usefathom-2.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 Metadata-Version: 2.1
 Name: django-usefathom
-Version: 1.2.2
+Version: 2.0.0
 Summary: A Django app to integrate Fathom Analytics into your project
-Home-page: https://github.com/paulchubatyy/django-usefathom/
-Author: Paul Chubatyy
-Author-email: code@citylance.biz
+Home-page: https://github.com/paulchubatyy/django-usefathom
 License: MIT
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
+Author: Paul Chubatyy
+Author-email: xobb@citylance.biz
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Project-URL: Repository, https://github.com/paulchubatyy/django-usefathom
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # django-usefathom
 
 Fathom Analytics integration with Django projects. Provides ability to integrate
 page view tracking and goal reporting.
 
+> If you want to track goals instead of events, please use the 1.x.x version of the library.
+
 ## Installation
 
 Install the package:
 
 ```
 pip install django-usefathom
 ```
@@ -73,53 +68,36 @@
 
 ```jinja2
 {% include "usefathom/usefathom.html" %}
 ```
 
 From this point your site visits will be tracked.
 
-## Custom domain for Fathom Analytics script
-
-If you want to use the custom domain for Fathom Analytics add to your `settings.py`:
-
-```python
-FATHOM_SCRIPT_URL=https://cname.yourdomain.com/script.js
-```
-
-## Goal Tracking
+## Event Tracking
 
 ### Python
 
-Optionally, add your goals dictionary to your `settings.py` file:
-
-```python
-FATHOM_GOALS = {
-    "registration": "XXXO9X",
-    "add_to_card": "YYYO9X,
-    # ....
-}
-```
-
-Now if you want to report a goal from your backend service to Fathom analytics:
+Now if you want to report a event from your backend service to Fathom analytics:
 
 ```python
-from usefathom.api import track
+import usefathom
 
 def some_view(request, *args, **kwargs):
     # anywhere you have request object, most likely views are a good place for this
-    track(request, "add_to_card", "2999")  # Third parameter is optional, attaches the monetary value to the goal. 29.99 in example
+    usefathom.track(request, "add_to_card", 100)  # Third parameter is optional integer, attaches the monetary value to the event in cents
 ```
 
 And the goal will be reported to Fathom analytics on the next page load.
 
 ### HTML+JS
 
 You can use template tags to track the goals from the html. It's useful when tracking external link clicks, etc.
 
 ```jinja2
 {% load fathom }
 ......with link
-<a href="https://go-somewhere.com/link" {% click_goal "somewhere_link_clicked" 100 %}>Go somewhere?</a>
+<a href="https://go-somewhere.com/link" {% click_event "somewhere_link_clicked" 100 %}>Go somewhere?</a>
 ......with form
-<form method="POST" {% submit_goal "registration_submit" %}>
+<form method="POST" {% submit_event "registration_submit" %}>
 ```
 
+
```

### Comparing `django-usefathom-1.2.2/README.md` & `django_usefathom-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # django-usefathom
 
 Fathom Analytics integration with Django projects. Provides ability to integrate
 page view tracking and goal reporting.
 
+> If you want to track goals instead of events, please use the 1.x.x version of the library.
+
 ## Installation
 
 Install the package:
 
 ```
 pip install django-usefathom
 ```
@@ -48,53 +50,35 @@
 
 ```jinja2
 {% include "usefathom/usefathom.html" %}
 ```
 
 From this point your site visits will be tracked.
 
-## Custom domain for Fathom Analytics script
-
-If you want to use the custom domain for Fathom Analytics add to your `settings.py`:
-
-```python
-FATHOM_SCRIPT_URL=https://cname.yourdomain.com/script.js
-```
-
-## Goal Tracking
+## Event Tracking
 
 ### Python
 
-Optionally, add your goals dictionary to your `settings.py` file:
-
-```python
-FATHOM_GOALS = {
-    "registration": "XXXO9X",
-    "add_to_card": "YYYO9X,
-    # ....
-}
-```
-
-Now if you want to report a goal from your backend service to Fathom analytics:
+Now if you want to report a event from your backend service to Fathom analytics:
 
 ```python
-from usefathom.api import track
+import usefathom
 
 def some_view(request, *args, **kwargs):
     # anywhere you have request object, most likely views are a good place for this
-    track(request, "add_to_card", "2999")  # Third parameter is optional, attaches the monetary value to the goal. 29.99 in example
+    usefathom.track(request, "add_to_card", 100)  # Third parameter is optional integer, attaches the monetary value to the event in cents
 ```
 
 And the goal will be reported to Fathom analytics on the next page load.
 
 ### HTML+JS
 
 You can use template tags to track the goals from the html. It's useful when tracking external link clicks, etc.
 
 ```jinja2
 {% load fathom }
 ......with link
-<a href="https://go-somewhere.com/link" {% click_goal "somewhere_link_clicked" 100 %}>Go somewhere?</a>
+<a href="https://go-somewhere.com/link" {% click_event "somewhere_link_clicked" 100 %}>Go somewhere?</a>
 ......with form
-<form method="POST" {% submit_goal "registration_submit" %}>
+<form method="POST" {% submit_event "registration_submit" %}>
 ```
```

