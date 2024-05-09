# Comparing `tmp/django_notifications_views-0.1.6.tar.gz` & `tmp/django_notifications_views-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_notifications_views-0.1.6.tar", last modified: Thu May  9 17:01:07 2024, max compression
+gzip compressed data, was "django_notifications_views-0.1.7.tar", last modified: Thu May  9 17:07:14 2024, max compression
```

## Comparing `django_notifications_views-0.1.6.tar` & `django_notifications_views-0.1.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 17:01:07.777105 django_notifications_views-0.1.6/
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)       73 2024-04-25 19:24:06.000000 django_notifications_views-0.1.6/AUTHORS
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1116 2024-04-25 19:12:10.000000 django_notifications_views-0.1.6/LICENSE
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 17:01:07.776730 django_notifications_views-0.1.6/PKG-INFO
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1329 2024-05-09 15:39:24.000000 django_notifications_views-0.1.6/README.md
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 17:01:07.771520 django_notifications_views-0.1.6/django_notifications_views/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.6/django_notifications_views/__init__.py
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)      480 2024-05-09 17:01:05.000000 django_notifications_views-0.1.6/django_notifications_views/__version__.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       63 2024-04-25 19:11:13.000000 django_notifications_views-0.1.6/django_notifications_views/admin.py
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)      903 2024-04-25 19:19:22.000000 django_notifications_views-0.1.6/django_notifications_views/app_settings.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      175 2024-04-25 19:45:35.000000 django_notifications_views-0.1.6/django_notifications_views/apps.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1430 2024-05-09 15:48:08.000000 django_notifications_views-0.1.6/django_notifications_views/expo_utils.py
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 17:01:07.776037 django_notifications_views-0.1.6/django_notifications_views/migrations/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.6/django_notifications_views/migrations/__init__.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      749 2024-05-09 15:48:14.000000 django_notifications_views-0.1.6/django_notifications_views/models.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1008 2024-04-25 19:11:13.000000 django_notifications_views-0.1.6/django_notifications_views/serializers.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       60 2024-04-25 19:11:13.000000 django_notifications_views-0.1.6/django_notifications_views/tests.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      501 2024-05-09 16:40:14.000000 django_notifications_views-0.1.6/django_notifications_views/urls.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     3108 2024-05-09 17:00:58.000000 django_notifications_views-0.1.6/django_notifications_views/views.py
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 17:01:07.776250 django_notifications_views-0.1.6/django_notifications_views.egg-info/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 17:01:07.000000 django_notifications_views-0.1.6/django_notifications_views.egg-info/PKG-INFO
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      804 2024-05-09 17:01:07.000000 django_notifications_views-0.1.6/django_notifications_views.egg-info/SOURCES.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-09 17:01:07.000000 django_notifications_views-0.1.6/django_notifications_views.egg-info/dependency_links.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-08 18:36:11.000000 django_notifications_views-0.1.6/django_notifications_views.egg-info/not-zip-safe
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      101 2024-05-09 17:01:07.000000 django_notifications_views-0.1.6/django_notifications_views.egg-info/requires.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       27 2024-05-09 17:01:07.000000 django_notifications_views-0.1.6/django_notifications_views.egg-info/top_level.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       38 2024-05-09 17:01:07.777176 django_notifications_views-0.1.6/setup.cfg
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1314 2024-05-08 18:36:08.000000 django_notifications_views-0.1.6/setup.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 17:07:14.912439 django_notifications_views-0.1.7/
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)       73 2024-04-25 19:24:06.000000 django_notifications_views-0.1.7/AUTHORS
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1116 2024-04-25 19:12:10.000000 django_notifications_views-0.1.7/LICENSE
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 17:07:14.911887 django_notifications_views-0.1.7/PKG-INFO
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1329 2024-05-09 15:39:24.000000 django_notifications_views-0.1.7/README.md
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 17:07:14.909630 django_notifications_views-0.1.7/django_notifications_views/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.7/django_notifications_views/__init__.py
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)      480 2024-05-09 17:07:10.000000 django_notifications_views-0.1.7/django_notifications_views/__version__.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       63 2024-04-25 19:11:13.000000 django_notifications_views-0.1.7/django_notifications_views/admin.py
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)      903 2024-04-25 19:19:22.000000 django_notifications_views-0.1.7/django_notifications_views/app_settings.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      175 2024-04-25 19:45:35.000000 django_notifications_views-0.1.7/django_notifications_views/apps.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     1430 2024-05-09 15:48:08.000000 django_notifications_views-0.1.7/django_notifications_views/expo_utils.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 17:07:14.911177 django_notifications_views-0.1.7/django_notifications_views/migrations/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.7/django_notifications_views/migrations/__init__.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      749 2024-05-09 15:48:14.000000 django_notifications_views-0.1.7/django_notifications_views/models.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     1008 2024-04-25 19:11:13.000000 django_notifications_views-0.1.7/django_notifications_views/serializers.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       60 2024-04-25 19:11:13.000000 django_notifications_views-0.1.7/django_notifications_views/tests.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      501 2024-05-09 16:40:14.000000 django_notifications_views-0.1.7/django_notifications_views/urls.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     3112 2024-05-09 17:06:58.000000 django_notifications_views-0.1.7/django_notifications_views/views.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 17:07:14.911403 django_notifications_views-0.1.7/django_notifications_views.egg-info/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 17:07:14.000000 django_notifications_views-0.1.7/django_notifications_views.egg-info/PKG-INFO
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      804 2024-05-09 17:07:14.000000 django_notifications_views-0.1.7/django_notifications_views.egg-info/SOURCES.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-09 17:07:14.000000 django_notifications_views-0.1.7/django_notifications_views.egg-info/dependency_links.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-08 18:36:11.000000 django_notifications_views-0.1.7/django_notifications_views.egg-info/not-zip-safe
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      101 2024-05-09 17:07:14.000000 django_notifications_views-0.1.7/django_notifications_views.egg-info/requires.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       27 2024-05-09 17:07:14.000000 django_notifications_views-0.1.7/django_notifications_views.egg-info/top_level.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       38 2024-05-09 17:07:14.912537 django_notifications_views-0.1.7/setup.cfg
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1314 2024-05-08 18:36:08.000000 django_notifications_views-0.1.7/setup.py
```

### Comparing `django_notifications_views-0.1.6/LICENSE` & `django_notifications_views-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.6/PKG-INFO` & `django_notifications_views-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_notifications_views
-Version: 0.1.6
+Version: 0.1.7
 Summary: Django-notifications-views is an extension for Django-notifications-hq that provides a viewset for the notifications.
 Home-page: https://github.com/nachoborrelli/Django-notifications-views
 Author: nachoborrelli
 Author-email: nacho2911@hotmail.com
 License: MIT
 Keywords: django notifications hq views
 Classifier: Framework :: Django
```

### Comparing `django_notifications_views-0.1.6/README.md` & `django_notifications_views-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.6/django_notifications_views/app_settings.py` & `django_notifications_views-0.1.7/django_notifications_views/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.6/django_notifications_views/expo_utils.py` & `django_notifications_views-0.1.7/django_notifications_views/expo_utils.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.6/django_notifications_views/models.py` & `django_notifications_views-0.1.7/django_notifications_views/models.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.6/django_notifications_views/serializers.py` & `django_notifications_views-0.1.7/django_notifications_views/serializers.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.6/django_notifications_views/views.py` & `django_notifications_views-0.1.7/django_notifications_views/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.exceptions import ValidationError
 
 from django_filters import rest_framework as filters
 
 from django_notifications_views.serializers import NotificationSerializer
 from django_notifications_views.app_settings import api_settings as settings
-from django_notifications_views.models import ExpoToken
 
 
 class NotificationsViewSet(GenericViewSet, ListModelMixin, RetrieveModelMixin):
     filter_backends = (
         filters.DjangoFilterBackend,
         rest_filters.SearchFilter,
         rest_filters.OrderingFilter,
@@ -49,14 +48,15 @@
         for notification in self.get_queryset():
             notification.unread = False
             notification.save()
         return Response(status=status.HTTP_204_NO_CONTENT)
     
 
 if settings.get_user_setting('USE_EXPO_NOTIFICATIONS'):
+    from django_notifications_views.models import ExpoToken
     class ManageDeviceExpo(GenericViewSet):
         permission_classes = [IsAuthenticated]
 
         @action(detail=False, url_path="register-device", methods=["POST"])
         def register_device(self, request, *args, **kwargs):
             user = request.user
```

### Comparing `django_notifications_views-0.1.6/django_notifications_views.egg-info/PKG-INFO` & `django_notifications_views-0.1.7/django_notifications_views.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_notifications_views
-Version: 0.1.6
+Version: 0.1.7
 Summary: Django-notifications-views is an extension for Django-notifications-hq that provides a viewset for the notifications.
 Home-page: https://github.com/nachoborrelli/Django-notifications-views
 Author: nachoborrelli
 Author-email: nacho2911@hotmail.com
 License: MIT
 Keywords: django notifications hq views
 Classifier: Framework :: Django
```

### Comparing `django_notifications_views-0.1.6/django_notifications_views.egg-info/SOURCES.txt` & `django_notifications_views-0.1.7/django_notifications_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.6/setup.py` & `django_notifications_views-0.1.7/setup.py`

 * *Files identical despite different names*

