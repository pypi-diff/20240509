# Comparing `tmp/django_notifications_views-0.1.0.tar.gz` & `tmp/django_notifications_views-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_notifications_views-0.1.0.tar", last modified: Wed May  8 18:36:11 2024, max compression
+gzip compressed data, was "django_notifications_views-0.1.1.tar", last modified: Thu May  9 15:08:08 2024, max compression
```

## Comparing `django_notifications_views-0.1.0.tar` & `django_notifications_views-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-08 18:36:11.484115 django_notifications_views-0.1.0/
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)       73 2024-04-25 19:24:06.000000 django_notifications_views-0.1.0/AUTHORS
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1116 2024-04-25 19:12:10.000000 django_notifications_views-0.1.0/LICENSE
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1980 2024-05-08 18:36:11.483789 django_notifications_views-0.1.0/PKG-INFO
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1097 2024-04-25 19:57:27.000000 django_notifications_views-0.1.0/README.md
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-08 18:36:11.481054 django_notifications_views-0.1.0/django_notifications_views/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.0/django_notifications_views/__init__.py
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)      476 2024-04-25 19:23:54.000000 django_notifications_views-0.1.0/django_notifications_views/__version__.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       63 2024-04-25 19:11:13.000000 django_notifications_views-0.1.0/django_notifications_views/admin.py
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)      903 2024-04-25 19:19:22.000000 django_notifications_views-0.1.0/django_notifications_views/app_settings.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      175 2024-04-25 19:45:35.000000 django_notifications_views-0.1.0/django_notifications_views/apps.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1366 2024-04-25 19:45:29.000000 django_notifications_views-0.1.0/django_notifications_views/expo_utils.py
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-08 18:36:11.482977 django_notifications_views-0.1.0/django_notifications_views/migrations/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.0/django_notifications_views/migrations/__init__.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      685 2024-04-25 19:45:29.000000 django_notifications_views-0.1.0/django_notifications_views/models.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1008 2024-04-25 19:11:13.000000 django_notifications_views-0.1.0/django_notifications_views/serializers.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       60 2024-04-25 19:11:13.000000 django_notifications_views-0.1.0/django_notifications_views/tests.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      270 2024-04-25 19:45:29.000000 django_notifications_views-0.1.0/django_notifications_views/urls.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1540 2024-04-25 19:45:29.000000 django_notifications_views-0.1.0/django_notifications_views/views.py
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-08 18:36:11.483353 django_notifications_views-0.1.0/django_notifications_views.egg-info/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1980 2024-05-08 18:36:11.000000 django_notifications_views-0.1.0/django_notifications_views.egg-info/PKG-INFO
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      804 2024-05-08 18:36:11.000000 django_notifications_views-0.1.0/django_notifications_views.egg-info/SOURCES.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-08 18:36:11.000000 django_notifications_views-0.1.0/django_notifications_views.egg-info/dependency_links.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-08 18:36:11.000000 django_notifications_views-0.1.0/django_notifications_views.egg-info/not-zip-safe
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      101 2024-05-08 18:36:11.000000 django_notifications_views-0.1.0/django_notifications_views.egg-info/requires.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       27 2024-05-08 18:36:11.000000 django_notifications_views-0.1.0/django_notifications_views.egg-info/top_level.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       38 2024-05-08 18:36:11.484190 django_notifications_views-0.1.0/setup.cfg
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1314 2024-05-08 18:36:08.000000 django_notifications_views-0.1.0/setup.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:08:08.805695 django_notifications_views-0.1.1/
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)       73 2024-04-25 19:24:06.000000 django_notifications_views-0.1.1/AUTHORS
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1116 2024-04-25 19:12:10.000000 django_notifications_views-0.1.1/LICENSE
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     1965 2024-05-09 15:08:08.805383 django_notifications_views-0.1.1/PKG-INFO
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1082 2024-05-09 12:09:40.000000 django_notifications_views-0.1.1/README.md
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:08:08.803131 django_notifications_views-0.1.1/django_notifications_views/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.1/django_notifications_views/__init__.py
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)      472 2024-05-09 12:52:11.000000 django_notifications_views-0.1.1/django_notifications_views/__version__.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       63 2024-04-25 19:11:13.000000 django_notifications_views-0.1.1/django_notifications_views/admin.py
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)      903 2024-04-25 19:19:22.000000 django_notifications_views-0.1.1/django_notifications_views/app_settings.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      175 2024-04-25 19:45:35.000000 django_notifications_views-0.1.1/django_notifications_views/apps.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     1366 2024-04-25 19:45:29.000000 django_notifications_views-0.1.1/django_notifications_views/expo_utils.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:08:08.804794 django_notifications_views-0.1.1/django_notifications_views/migrations/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.1/django_notifications_views/migrations/__init__.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      685 2024-04-25 19:45:29.000000 django_notifications_views-0.1.1/django_notifications_views/models.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     1008 2024-04-25 19:11:13.000000 django_notifications_views-0.1.1/django_notifications_views/serializers.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       60 2024-04-25 19:11:13.000000 django_notifications_views-0.1.1/django_notifications_views/tests.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      356 2024-05-09 12:36:39.000000 django_notifications_views-0.1.1/django_notifications_views/urls.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     3038 2024-05-09 12:35:39.000000 django_notifications_views-0.1.1/django_notifications_views/views.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:08:08.805019 django_notifications_views-0.1.1/django_notifications_views.egg-info/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     1965 2024-05-09 15:08:08.000000 django_notifications_views-0.1.1/django_notifications_views.egg-info/PKG-INFO
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      804 2024-05-09 15:08:08.000000 django_notifications_views-0.1.1/django_notifications_views.egg-info/SOURCES.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-09 15:08:08.000000 django_notifications_views-0.1.1/django_notifications_views.egg-info/dependency_links.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-08 18:36:11.000000 django_notifications_views-0.1.1/django_notifications_views.egg-info/not-zip-safe
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      101 2024-05-09 15:08:08.000000 django_notifications_views-0.1.1/django_notifications_views.egg-info/requires.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       27 2024-05-09 15:08:08.000000 django_notifications_views-0.1.1/django_notifications_views.egg-info/top_level.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       38 2024-05-09 15:08:08.805783 django_notifications_views-0.1.1/setup.cfg
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1314 2024-05-08 18:36:08.000000 django_notifications_views-0.1.1/setup.py
```

### Comparing `django_notifications_views-0.1.0/LICENSE` & `django_notifications_views-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.0/PKG-INFO` & `django_notifications_views-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_notifications_views
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django-notifications-views is an extension for Django-notifications-hq that provides a viewset for the notifications.
 Home-page: https://github.com/nachoborrelli/Django-notifications-views
 Author: nachoborrelli
 Author-email: nacho2911@hotmail.com
 License: MIT
 Keywords: django notifications hq views
 Classifier: Framework :: Django
@@ -42,32 +42,29 @@
     
 Add `django_notifications_views` app to INSTALLED_APPS in your django settings.py:
 
 ```python
 INSTALLED_APPS = (
     ...,
     "django.contrib.staticfiles",
-	"rest_framework",  # required only if using the provided REST endpoints
+    "rest_framework",  # required only if using the provided REST endpoints
     'notifications',
     'django_notifications_views',
      ...,
 )
 ```
     
 Include viewset routes
 
 ```python
 from django_notifications_views.urls import router as django_notifications_views_router
 your_router.registry.extend(django_notifications_views_router.registry)
 ```
     
 
-### Explanation
-
-
 ## Contributing
 
 -   [Juan Ignacio Borrelli](https://www.linkedin.com/in/juan-ignacio-borrelli/)
     
 
 Maintained and developed by [Linkchar Software Development](https://linkchar.com/).
```

### Comparing `django_notifications_views-0.1.0/README.md` & `django_notifications_views-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,32 +18,29 @@
     
 Add `django_notifications_views` app to INSTALLED_APPS in your django settings.py:
 
 ```python
 INSTALLED_APPS = (
     ...,
     "django.contrib.staticfiles",
-	"rest_framework",  # required only if using the provided REST endpoints
+    "rest_framework",  # required only if using the provided REST endpoints
     'notifications',
     'django_notifications_views',
      ...,
 )
 ```
     
 Include viewset routes
 
 ```python
 from django_notifications_views.urls import router as django_notifications_views_router
 your_router.registry.extend(django_notifications_views_router.registry)
 ```
     
 
-### Explanation
-
-
 ## Contributing
 
 -   [Juan Ignacio Borrelli](https://www.linkedin.com/in/juan-ignacio-borrelli/)
     
 
 Maintained and developed by [Linkchar Software Development](https://linkchar.com/).
```

### Comparing `django_notifications_views-0.1.0/django_notifications_views/app_settings.py` & `django_notifications_views-0.1.1/django_notifications_views/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.0/django_notifications_views/expo_utils.py` & `django_notifications_views-0.1.1/django_notifications_views/expo_utils.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.0/django_notifications_views/models.py` & `django_notifications_views-0.1.1/django_notifications_views/models.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.0/django_notifications_views/serializers.py` & `django_notifications_views-0.1.1/django_notifications_views/serializers.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.0/django_notifications_views.egg-info/PKG-INFO` & `django_notifications_views-0.1.1/django_notifications_views.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_notifications_views
-Version: 0.1.0
+Version: 0.1.1
 Summary: Django-notifications-views is an extension for Django-notifications-hq that provides a viewset for the notifications.
 Home-page: https://github.com/nachoborrelli/Django-notifications-views
 Author: nachoborrelli
 Author-email: nacho2911@hotmail.com
 License: MIT
 Keywords: django notifications hq views
 Classifier: Framework :: Django
@@ -42,32 +42,29 @@
     
 Add `django_notifications_views` app to INSTALLED_APPS in your django settings.py:
 
 ```python
 INSTALLED_APPS = (
     ...,
     "django.contrib.staticfiles",
-	"rest_framework",  # required only if using the provided REST endpoints
+    "rest_framework",  # required only if using the provided REST endpoints
     'notifications',
     'django_notifications_views',
      ...,
 )
 ```
     
 Include viewset routes
 
 ```python
 from django_notifications_views.urls import router as django_notifications_views_router
 your_router.registry.extend(django_notifications_views_router.registry)
 ```
     
 
-### Explanation
-
-
 ## Contributing
 
 -   [Juan Ignacio Borrelli](https://www.linkedin.com/in/juan-ignacio-borrelli/)
     
 
 Maintained and developed by [Linkchar Software Development](https://linkchar.com/).
```

### Comparing `django_notifications_views-0.1.0/django_notifications_views.egg-info/SOURCES.txt` & `django_notifications_views-0.1.1/django_notifications_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.0/setup.py` & `django_notifications_views-0.1.1/setup.py`

 * *Files identical despite different names*

