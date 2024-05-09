# Comparing `tmp/django_notifications_views-0.1.2.tar.gz` & `tmp/django_notifications_views-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_notifications_views-0.1.2.tar", last modified: Thu May  9 15:41:22 2024, max compression
+gzip compressed data, was "django_notifications_views-0.1.3.tar", last modified: Thu May  9 15:48:53 2024, max compression
```

## Comparing `django_notifications_views-0.1.2.tar` & `django_notifications_views-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:41:22.415669 django_notifications_views-0.1.2/
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)       73 2024-04-25 19:24:06.000000 django_notifications_views-0.1.2/AUTHORS
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1116 2024-04-25 19:12:10.000000 django_notifications_views-0.1.2/LICENSE
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 15:41:22.415371 django_notifications_views-0.1.2/PKG-INFO
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1329 2024-05-09 15:39:24.000000 django_notifications_views-0.1.2/README.md
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:41:22.413480 django_notifications_views-0.1.2/django_notifications_views/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.2/django_notifications_views/__init__.py
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)      480 2024-05-09 15:41:14.000000 django_notifications_views-0.1.2/django_notifications_views/__version__.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       63 2024-04-25 19:11:13.000000 django_notifications_views-0.1.2/django_notifications_views/admin.py
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)      903 2024-04-25 19:19:22.000000 django_notifications_views-0.1.2/django_notifications_views/app_settings.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      175 2024-04-25 19:45:35.000000 django_notifications_views-0.1.2/django_notifications_views/apps.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1386 2024-05-09 15:40:37.000000 django_notifications_views-0.1.2/django_notifications_views/expo_utils.py
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:41:22.414815 django_notifications_views-0.1.2/django_notifications_views/migrations/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.2/django_notifications_views/migrations/__init__.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      705 2024-05-09 15:40:45.000000 django_notifications_views-0.1.2/django_notifications_views/models.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1008 2024-04-25 19:11:13.000000 django_notifications_views-0.1.2/django_notifications_views/serializers.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       60 2024-04-25 19:11:13.000000 django_notifications_views-0.1.2/django_notifications_views/tests.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      356 2024-05-09 12:36:39.000000 django_notifications_views-0.1.2/django_notifications_views/urls.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     3058 2024-05-09 15:40:13.000000 django_notifications_views-0.1.2/django_notifications_views/views.py
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:41:22.415013 django_notifications_views-0.1.2/django_notifications_views.egg-info/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 15:41:22.000000 django_notifications_views-0.1.2/django_notifications_views.egg-info/PKG-INFO
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      804 2024-05-09 15:41:22.000000 django_notifications_views-0.1.2/django_notifications_views.egg-info/SOURCES.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-09 15:41:22.000000 django_notifications_views-0.1.2/django_notifications_views.egg-info/dependency_links.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-08 18:36:11.000000 django_notifications_views-0.1.2/django_notifications_views.egg-info/not-zip-safe
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      101 2024-05-09 15:41:22.000000 django_notifications_views-0.1.2/django_notifications_views.egg-info/requires.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       27 2024-05-09 15:41:22.000000 django_notifications_views-0.1.2/django_notifications_views.egg-info/top_level.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       38 2024-05-09 15:41:22.415732 django_notifications_views-0.1.2/setup.cfg
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1314 2024-05-08 18:36:08.000000 django_notifications_views-0.1.2/setup.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:48:53.208866 django_notifications_views-0.1.3/
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)       73 2024-04-25 19:24:06.000000 django_notifications_views-0.1.3/AUTHORS
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1116 2024-04-25 19:12:10.000000 django_notifications_views-0.1.3/LICENSE
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 15:48:53.208561 django_notifications_views-0.1.3/PKG-INFO
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1329 2024-05-09 15:39:24.000000 django_notifications_views-0.1.3/README.md
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:48:53.206667 django_notifications_views-0.1.3/django_notifications_views/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.3/django_notifications_views/__init__.py
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)      480 2024-05-09 15:48:52.000000 django_notifications_views-0.1.3/django_notifications_views/__version__.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       63 2024-04-25 19:11:13.000000 django_notifications_views-0.1.3/django_notifications_views/admin.py
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)      903 2024-04-25 19:19:22.000000 django_notifications_views-0.1.3/django_notifications_views/app_settings.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      175 2024-04-25 19:45:35.000000 django_notifications_views-0.1.3/django_notifications_views/apps.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     1430 2024-05-09 15:48:08.000000 django_notifications_views-0.1.3/django_notifications_views/expo_utils.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:48:53.208023 django_notifications_views-0.1.3/django_notifications_views/migrations/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.3/django_notifications_views/migrations/__init__.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      749 2024-05-09 15:48:14.000000 django_notifications_views-0.1.3/django_notifications_views/models.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     1008 2024-04-25 19:11:13.000000 django_notifications_views-0.1.3/django_notifications_views/serializers.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       60 2024-04-25 19:11:13.000000 django_notifications_views-0.1.3/django_notifications_views/tests.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      356 2024-05-09 12:36:39.000000 django_notifications_views-0.1.3/django_notifications_views/urls.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     3086 2024-05-09 15:48:18.000000 django_notifications_views-0.1.3/django_notifications_views/views.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:48:53.208220 django_notifications_views-0.1.3/django_notifications_views.egg-info/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 15:48:53.000000 django_notifications_views-0.1.3/django_notifications_views.egg-info/PKG-INFO
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      804 2024-05-09 15:48:53.000000 django_notifications_views-0.1.3/django_notifications_views.egg-info/SOURCES.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-09 15:48:53.000000 django_notifications_views-0.1.3/django_notifications_views.egg-info/dependency_links.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-08 18:36:11.000000 django_notifications_views-0.1.3/django_notifications_views.egg-info/not-zip-safe
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      101 2024-05-09 15:48:53.000000 django_notifications_views-0.1.3/django_notifications_views.egg-info/requires.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       27 2024-05-09 15:48:53.000000 django_notifications_views-0.1.3/django_notifications_views.egg-info/top_level.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       38 2024-05-09 15:48:53.208930 django_notifications_views-0.1.3/setup.cfg
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1314 2024-05-08 18:36:08.000000 django_notifications_views-0.1.3/setup.py
```

### Comparing `django_notifications_views-0.1.2/LICENSE` & `django_notifications_views-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.2/PKG-INFO` & `django_notifications_views-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_notifications_views
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django-notifications-views is an extension for Django-notifications-hq that provides a viewset for the notifications.
 Home-page: https://github.com/nachoborrelli/Django-notifications-views
 Author: nachoborrelli
 Author-email: nacho2911@hotmail.com
 License: MIT
 Keywords: django notifications hq views
 Classifier: Framework :: Django
```

### Comparing `django_notifications_views-0.1.2/README.md` & `django_notifications_views-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.2/django_notifications_views/app_settings.py` & `django_notifications_views-0.1.3/django_notifications_views/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.2/django_notifications_views/expo_utils.py` & `django_notifications_views-0.1.3/django_notifications_views/expo_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from exponent_server_sdk import (
     DeviceNotRegisteredError,
     PushClient,
     PushMessage,
     PushTicketError,
 )
-from django.conf import settings
+from django_notifications_views.app_settings import api_settings as settings
 
 if settings.get_user_setting('USE_EXPO_NOTIFICATIONS'):
     def send_push_message(token, message, data=None):
         """
         Send push notification to expo token associated with user.
         if token is not valid, delete it from db
         :param token: string
```

### Comparing `django_notifications_views-0.1.2/django_notifications_views/models.py` & `django_notifications_views-0.1.3/django_notifications_views/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.db import models
 from notifications.signals import notify
-from django.conf import settings
+from django_notifications_views.app_settings import api_settings as settings
 
 
 if settings.get_user_setting('USE_EXPO_NOTIFICATIONS'):
     from django_notifications_views.expo_utils import expo_push_notification_handler
     class ExpoToken(models.Model):
         token = models.CharField(max_length=200)
         user = models.ForeignKey(
```

### Comparing `django_notifications_views-0.1.2/django_notifications_views/serializers.py` & `django_notifications_views-0.1.3/django_notifications_views/serializers.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.2/django_notifications_views/views.py` & `django_notifications_views-0.1.3/django_notifications_views/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 
 from django_filters import rest_framework as filters
 
 from django.conf import settings
 
 from django_notifications_views.serializers import NotificationSerializer
 
-from user_notifications.models import ExpoToken
-
+from django_notifications_views.app_settings import api_settings as settings
 
 class NotificationsViewSet(GenericViewSet, ListModelMixin, RetrieveModelMixin):
     filter_backends = (
         filters.DjangoFilterBackend,
         rest_filters.SearchFilter,
         rest_filters.OrderingFilter,
     )
```

### Comparing `django_notifications_views-0.1.2/django_notifications_views.egg-info/PKG-INFO` & `django_notifications_views-0.1.3/django_notifications_views.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_notifications_views
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django-notifications-views is an extension for Django-notifications-hq that provides a viewset for the notifications.
 Home-page: https://github.com/nachoborrelli/Django-notifications-views
 Author: nachoborrelli
 Author-email: nacho2911@hotmail.com
 License: MIT
 Keywords: django notifications hq views
 Classifier: Framework :: Django
```

### Comparing `django_notifications_views-0.1.2/django_notifications_views.egg-info/SOURCES.txt` & `django_notifications_views-0.1.3/django_notifications_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.2/setup.py` & `django_notifications_views-0.1.3/setup.py`

 * *Files identical despite different names*

