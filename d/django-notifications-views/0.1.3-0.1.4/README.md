# Comparing `tmp/django_notifications_views-0.1.3.tar.gz` & `tmp/django_notifications_views-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_notifications_views-0.1.3.tar", last modified: Thu May  9 15:48:53 2024, max compression
+gzip compressed data, was "django_notifications_views-0.1.4.tar", last modified: Thu May  9 15:58:18 2024, max compression
```

## Comparing `django_notifications_views-0.1.3.tar` & `django_notifications_views-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:48:53.208866 django_notifications_views-0.1.3/
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)       73 2024-04-25 19:24:06.000000 django_notifications_views-0.1.3/AUTHORS
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1116 2024-04-25 19:12:10.000000 django_notifications_views-0.1.3/LICENSE
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 15:48:53.208561 django_notifications_views-0.1.3/PKG-INFO
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1329 2024-05-09 15:39:24.000000 django_notifications_views-0.1.3/README.md
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:48:53.206667 django_notifications_views-0.1.3/django_notifications_views/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.3/django_notifications_views/__init__.py
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)      480 2024-05-09 15:48:52.000000 django_notifications_views-0.1.3/django_notifications_views/__version__.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       63 2024-04-25 19:11:13.000000 django_notifications_views-0.1.3/django_notifications_views/admin.py
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)      903 2024-04-25 19:19:22.000000 django_notifications_views-0.1.3/django_notifications_views/app_settings.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      175 2024-04-25 19:45:35.000000 django_notifications_views-0.1.3/django_notifications_views/apps.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1430 2024-05-09 15:48:08.000000 django_notifications_views-0.1.3/django_notifications_views/expo_utils.py
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:48:53.208023 django_notifications_views-0.1.3/django_notifications_views/migrations/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.3/django_notifications_views/migrations/__init__.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      749 2024-05-09 15:48:14.000000 django_notifications_views-0.1.3/django_notifications_views/models.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1008 2024-04-25 19:11:13.000000 django_notifications_views-0.1.3/django_notifications_views/serializers.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       60 2024-04-25 19:11:13.000000 django_notifications_views-0.1.3/django_notifications_views/tests.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      356 2024-05-09 12:36:39.000000 django_notifications_views-0.1.3/django_notifications_views/urls.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     3086 2024-05-09 15:48:18.000000 django_notifications_views-0.1.3/django_notifications_views/views.py
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:48:53.208220 django_notifications_views-0.1.3/django_notifications_views.egg-info/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 15:48:53.000000 django_notifications_views-0.1.3/django_notifications_views.egg-info/PKG-INFO
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      804 2024-05-09 15:48:53.000000 django_notifications_views-0.1.3/django_notifications_views.egg-info/SOURCES.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-09 15:48:53.000000 django_notifications_views-0.1.3/django_notifications_views.egg-info/dependency_links.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-08 18:36:11.000000 django_notifications_views-0.1.3/django_notifications_views.egg-info/not-zip-safe
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      101 2024-05-09 15:48:53.000000 django_notifications_views-0.1.3/django_notifications_views.egg-info/requires.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       27 2024-05-09 15:48:53.000000 django_notifications_views-0.1.3/django_notifications_views.egg-info/top_level.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       38 2024-05-09 15:48:53.208930 django_notifications_views-0.1.3/setup.cfg
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1314 2024-05-08 18:36:08.000000 django_notifications_views-0.1.3/setup.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:58:18.550166 django_notifications_views-0.1.4/
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)       73 2024-04-25 19:24:06.000000 django_notifications_views-0.1.4/AUTHORS
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1116 2024-04-25 19:12:10.000000 django_notifications_views-0.1.4/LICENSE
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 15:58:18.549895 django_notifications_views-0.1.4/PKG-INFO
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1329 2024-05-09 15:39:24.000000 django_notifications_views-0.1.4/README.md
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:58:18.548290 django_notifications_views-0.1.4/django_notifications_views/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.4/django_notifications_views/__init__.py
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)      480 2024-05-09 15:58:18.000000 django_notifications_views-0.1.4/django_notifications_views/__version__.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       63 2024-04-25 19:11:13.000000 django_notifications_views-0.1.4/django_notifications_views/admin.py
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)      903 2024-04-25 19:19:22.000000 django_notifications_views-0.1.4/django_notifications_views/app_settings.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      175 2024-04-25 19:45:35.000000 django_notifications_views-0.1.4/django_notifications_views/apps.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     1430 2024-05-09 15:48:08.000000 django_notifications_views-0.1.4/django_notifications_views/expo_utils.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:58:18.549409 django_notifications_views-0.1.4/django_notifications_views/migrations/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.4/django_notifications_views/migrations/__init__.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      749 2024-05-09 15:48:14.000000 django_notifications_views-0.1.4/django_notifications_views/models.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     1008 2024-04-25 19:11:13.000000 django_notifications_views-0.1.4/django_notifications_views/serializers.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       60 2024-04-25 19:11:13.000000 django_notifications_views-0.1.4/django_notifications_views/tests.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      494 2024-05-09 15:58:08.000000 django_notifications_views-0.1.4/django_notifications_views/urls.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     3086 2024-05-09 15:48:18.000000 django_notifications_views-0.1.4/django_notifications_views/views.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:58:18.549596 django_notifications_views-0.1.4/django_notifications_views.egg-info/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 15:58:18.000000 django_notifications_views-0.1.4/django_notifications_views.egg-info/PKG-INFO
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      804 2024-05-09 15:58:18.000000 django_notifications_views-0.1.4/django_notifications_views.egg-info/SOURCES.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-09 15:58:18.000000 django_notifications_views-0.1.4/django_notifications_views.egg-info/dependency_links.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-08 18:36:11.000000 django_notifications_views-0.1.4/django_notifications_views.egg-info/not-zip-safe
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      101 2024-05-09 15:58:18.000000 django_notifications_views-0.1.4/django_notifications_views.egg-info/requires.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       27 2024-05-09 15:58:18.000000 django_notifications_views-0.1.4/django_notifications_views.egg-info/top_level.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       38 2024-05-09 15:58:18.550220 django_notifications_views-0.1.4/setup.cfg
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1314 2024-05-08 18:36:08.000000 django_notifications_views-0.1.4/setup.py
```

### Comparing `django_notifications_views-0.1.3/LICENSE` & `django_notifications_views-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.3/PKG-INFO` & `django_notifications_views-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_notifications_views
-Version: 0.1.3
+Version: 0.1.4
 Summary: Django-notifications-views is an extension for Django-notifications-hq that provides a viewset for the notifications.
 Home-page: https://github.com/nachoborrelli/Django-notifications-views
 Author: nachoborrelli
 Author-email: nacho2911@hotmail.com
 License: MIT
 Keywords: django notifications hq views
 Classifier: Framework :: Django
```

### Comparing `django_notifications_views-0.1.3/README.md` & `django_notifications_views-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.3/django_notifications_views/app_settings.py` & `django_notifications_views-0.1.4/django_notifications_views/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.3/django_notifications_views/expo_utils.py` & `django_notifications_views-0.1.4/django_notifications_views/expo_utils.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.3/django_notifications_views/models.py` & `django_notifications_views-0.1.4/django_notifications_views/models.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.3/django_notifications_views/serializers.py` & `django_notifications_views-0.1.4/django_notifications_views/serializers.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.3/django_notifications_views/views.py` & `django_notifications_views-0.1.4/django_notifications_views/views.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.3/django_notifications_views.egg-info/PKG-INFO` & `django_notifications_views-0.1.4/django_notifications_views.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_notifications_views
-Version: 0.1.3
+Version: 0.1.4
 Summary: Django-notifications-views is an extension for Django-notifications-hq that provides a viewset for the notifications.
 Home-page: https://github.com/nachoborrelli/Django-notifications-views
 Author: nachoborrelli
 Author-email: nacho2911@hotmail.com
 License: MIT
 Keywords: django notifications hq views
 Classifier: Framework :: Django
```

### Comparing `django_notifications_views-0.1.3/django_notifications_views.egg-info/SOURCES.txt` & `django_notifications_views-0.1.4/django_notifications_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.3/setup.py` & `django_notifications_views-0.1.4/setup.py`

 * *Files identical despite different names*

