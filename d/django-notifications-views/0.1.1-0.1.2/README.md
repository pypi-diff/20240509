# Comparing `tmp/django_notifications_views-0.1.1.tar.gz` & `tmp/django_notifications_views-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_notifications_views-0.1.1.tar", last modified: Thu May  9 15:08:08 2024, max compression
+gzip compressed data, was "django_notifications_views-0.1.2.tar", last modified: Thu May  9 15:41:22 2024, max compression
```

## Comparing `django_notifications_views-0.1.1.tar` & `django_notifications_views-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:08:08.805695 django_notifications_views-0.1.1/
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)       73 2024-04-25 19:24:06.000000 django_notifications_views-0.1.1/AUTHORS
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1116 2024-04-25 19:12:10.000000 django_notifications_views-0.1.1/LICENSE
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1965 2024-05-09 15:08:08.805383 django_notifications_views-0.1.1/PKG-INFO
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1082 2024-05-09 12:09:40.000000 django_notifications_views-0.1.1/README.md
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:08:08.803131 django_notifications_views-0.1.1/django_notifications_views/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.1/django_notifications_views/__init__.py
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)      472 2024-05-09 12:52:11.000000 django_notifications_views-0.1.1/django_notifications_views/__version__.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       63 2024-04-25 19:11:13.000000 django_notifications_views-0.1.1/django_notifications_views/admin.py
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)      903 2024-04-25 19:19:22.000000 django_notifications_views-0.1.1/django_notifications_views/app_settings.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      175 2024-04-25 19:45:35.000000 django_notifications_views-0.1.1/django_notifications_views/apps.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1366 2024-04-25 19:45:29.000000 django_notifications_views-0.1.1/django_notifications_views/expo_utils.py
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:08:08.804794 django_notifications_views-0.1.1/django_notifications_views/migrations/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.1/django_notifications_views/migrations/__init__.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      685 2024-04-25 19:45:29.000000 django_notifications_views-0.1.1/django_notifications_views/models.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1008 2024-04-25 19:11:13.000000 django_notifications_views-0.1.1/django_notifications_views/serializers.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       60 2024-04-25 19:11:13.000000 django_notifications_views-0.1.1/django_notifications_views/tests.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      356 2024-05-09 12:36:39.000000 django_notifications_views-0.1.1/django_notifications_views/urls.py
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     3038 2024-05-09 12:35:39.000000 django_notifications_views-0.1.1/django_notifications_views/views.py
-drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:08:08.805019 django_notifications_views-0.1.1/django_notifications_views.egg-info/
--rw-r--r--   0 nachoborrelli   (501) staff       (20)     1965 2024-05-09 15:08:08.000000 django_notifications_views-0.1.1/django_notifications_views.egg-info/PKG-INFO
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      804 2024-05-09 15:08:08.000000 django_notifications_views-0.1.1/django_notifications_views.egg-info/SOURCES.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-09 15:08:08.000000 django_notifications_views-0.1.1/django_notifications_views.egg-info/dependency_links.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-08 18:36:11.000000 django_notifications_views-0.1.1/django_notifications_views.egg-info/not-zip-safe
--rw-r--r--   0 nachoborrelli   (501) staff       (20)      101 2024-05-09 15:08:08.000000 django_notifications_views-0.1.1/django_notifications_views.egg-info/requires.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       27 2024-05-09 15:08:08.000000 django_notifications_views-0.1.1/django_notifications_views.egg-info/top_level.txt
--rw-r--r--   0 nachoborrelli   (501) staff       (20)       38 2024-05-09 15:08:08.805783 django_notifications_views-0.1.1/setup.cfg
--rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1314 2024-05-08 18:36:08.000000 django_notifications_views-0.1.1/setup.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:41:22.415669 django_notifications_views-0.1.2/
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)       73 2024-04-25 19:24:06.000000 django_notifications_views-0.1.2/AUTHORS
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1116 2024-04-25 19:12:10.000000 django_notifications_views-0.1.2/LICENSE
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 15:41:22.415371 django_notifications_views-0.1.2/PKG-INFO
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1329 2024-05-09 15:39:24.000000 django_notifications_views-0.1.2/README.md
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:41:22.413480 django_notifications_views-0.1.2/django_notifications_views/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.2/django_notifications_views/__init__.py
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)      480 2024-05-09 15:41:14.000000 django_notifications_views-0.1.2/django_notifications_views/__version__.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       63 2024-04-25 19:11:13.000000 django_notifications_views-0.1.2/django_notifications_views/admin.py
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)      903 2024-04-25 19:19:22.000000 django_notifications_views-0.1.2/django_notifications_views/app_settings.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      175 2024-04-25 19:45:35.000000 django_notifications_views-0.1.2/django_notifications_views/apps.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     1386 2024-05-09 15:40:37.000000 django_notifications_views-0.1.2/django_notifications_views/expo_utils.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:41:22.414815 django_notifications_views-0.1.2/django_notifications_views/migrations/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        0 2024-04-25 19:11:13.000000 django_notifications_views-0.1.2/django_notifications_views/migrations/__init__.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      705 2024-05-09 15:40:45.000000 django_notifications_views-0.1.2/django_notifications_views/models.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     1008 2024-04-25 19:11:13.000000 django_notifications_views-0.1.2/django_notifications_views/serializers.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       60 2024-04-25 19:11:13.000000 django_notifications_views-0.1.2/django_notifications_views/tests.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      356 2024-05-09 12:36:39.000000 django_notifications_views-0.1.2/django_notifications_views/urls.py
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     3058 2024-05-09 15:40:13.000000 django_notifications_views-0.1.2/django_notifications_views/views.py
+drwxr-xr-x   0 nachoborrelli   (501) staff       (20)        0 2024-05-09 15:41:22.415013 django_notifications_views-0.1.2/django_notifications_views.egg-info/
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)     2212 2024-05-09 15:41:22.000000 django_notifications_views-0.1.2/django_notifications_views.egg-info/PKG-INFO
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      804 2024-05-09 15:41:22.000000 django_notifications_views-0.1.2/django_notifications_views.egg-info/SOURCES.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-09 15:41:22.000000 django_notifications_views-0.1.2/django_notifications_views.egg-info/dependency_links.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)        1 2024-05-08 18:36:11.000000 django_notifications_views-0.1.2/django_notifications_views.egg-info/not-zip-safe
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)      101 2024-05-09 15:41:22.000000 django_notifications_views-0.1.2/django_notifications_views.egg-info/requires.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       27 2024-05-09 15:41:22.000000 django_notifications_views-0.1.2/django_notifications_views.egg-info/top_level.txt
+-rw-r--r--   0 nachoborrelli   (501) staff       (20)       38 2024-05-09 15:41:22.415732 django_notifications_views-0.1.2/setup.cfg
+-rw-rw-r--   0 nachoborrelli   (501) staff       (20)     1314 2024-05-08 18:36:08.000000 django_notifications_views-0.1.2/setup.py
```

### Comparing `django_notifications_views-0.1.1/LICENSE` & `django_notifications_views-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.1/PKG-INFO` & `django_notifications_views-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_notifications_views
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django-notifications-views is an extension for Django-notifications-hq that provides a viewset for the notifications.
 Home-page: https://github.com/nachoborrelli/Django-notifications-views
 Author: nachoborrelli
 Author-email: nacho2911@hotmail.com
 License: MIT
 Keywords: django notifications hq views
 Classifier: Framework :: Django
@@ -55,16 +55,23 @@
     
 Include viewset routes
 
 ```python
 from django_notifications_views.urls import router as django_notifications_views_router
 your_router.registry.extend(django_notifications_views_router.registry)
 ```
-    
 
+Add the following to your settings.py if you want to enable Expo Go notifications:
+
+```python
+DJANGO_NOTIFICATIONS_VIEWS = {
+    'USE_EXPO_NOTIFICATIONS': True, # Set to True to enable expo notifications
+    'EXPO_APP_ID': '<your-expo-app-id>', 
+}
+```
 ## Contributing
 
 -   [Juan Ignacio Borrelli](https://www.linkedin.com/in/juan-ignacio-borrelli/)
     
 
 Maintained and developed by [Linkchar Software Development](https://linkchar.com/).
```

### Comparing `django_notifications_views-0.1.1/README.md` & `django_notifications_views-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -31,16 +31,23 @@
     
 Include viewset routes
 
 ```python
 from django_notifications_views.urls import router as django_notifications_views_router
 your_router.registry.extend(django_notifications_views_router.registry)
 ```
-    
 
+Add the following to your settings.py if you want to enable Expo Go notifications:
+
+```python
+DJANGO_NOTIFICATIONS_VIEWS = {
+    'USE_EXPO_NOTIFICATIONS': True, # Set to True to enable expo notifications
+    'EXPO_APP_ID': '<your-expo-app-id>', 
+}
+```
 ## Contributing
 
 -   [Juan Ignacio Borrelli](https://www.linkedin.com/in/juan-ignacio-borrelli/)
     
 
 Maintained and developed by [Linkchar Software Development](https://linkchar.com/).
```

### Comparing `django_notifications_views-0.1.1/django_notifications_views/app_settings.py` & `django_notifications_views-0.1.2/django_notifications_views/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.1/django_notifications_views/expo_utils.py` & `django_notifications_views-0.1.2/django_notifications_views/expo_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     DeviceNotRegisteredError,
     PushClient,
     PushMessage,
     PushTicketError,
 )
 from django.conf import settings
 
-if settings.USE_EXPO_NOTIFICATIONS:
+if settings.get_user_setting('USE_EXPO_NOTIFICATIONS'):
     def send_push_message(token, message, data=None):
         """
         Send push notification to expo token associated with user.
         if token is not valid, delete it from db
         :param token: string
         :param message: string
         :param data:optional: dict
```

### Comparing `django_notifications_views-0.1.1/django_notifications_views/models.py` & `django_notifications_views-0.1.2/django_notifications_views/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.db import models
 from notifications.signals import notify
 from django.conf import settings
 
 
-if settings.USE_EXPO_NOTIFICATIONS:
+if settings.get_user_setting('USE_EXPO_NOTIFICATIONS'):
     from django_notifications_views.expo_utils import expo_push_notification_handler
     class ExpoToken(models.Model):
         token = models.CharField(max_length=200)
         user = models.ForeignKey(
             "users.User", on_delete=models.CASCADE, related_name="expo_tokens"
         )
         created_at = models.DateTimeField(auto_now_add=True)
```

### Comparing `django_notifications_views-0.1.1/django_notifications_views/serializers.py` & `django_notifications_views-0.1.2/django_notifications_views/serializers.py`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.1/django_notifications_views/views.py` & `django_notifications_views-0.1.2/django_notifications_views/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def mark_all_as_read(self, request):
         for notification in self.get_queryset():
             notification.unread = False
             notification.save()
         return Response(status=status.HTTP_204_NO_CONTENT)
     
 
-if settings.USE_EXPO_NOTIFICATIONS:
+if settings.get_user_setting('USE_EXPO_NOTIFICATIONS'):
     class ManageDeviceExpo(GenericViewSet):
         permission_classes = [IsAuthenticated]
 
         @action(detail=False, url_path="register-device", methods=["POST"])
         def register_device(self, request, *args, **kwargs):
             user = request.user
```

### Comparing `django_notifications_views-0.1.1/django_notifications_views.egg-info/PKG-INFO` & `django_notifications_views-0.1.2/django_notifications_views.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_notifications_views
-Version: 0.1.1
+Version: 0.1.2
 Summary: Django-notifications-views is an extension for Django-notifications-hq that provides a viewset for the notifications.
 Home-page: https://github.com/nachoborrelli/Django-notifications-views
 Author: nachoborrelli
 Author-email: nacho2911@hotmail.com
 License: MIT
 Keywords: django notifications hq views
 Classifier: Framework :: Django
@@ -55,16 +55,23 @@
     
 Include viewset routes
 
 ```python
 from django_notifications_views.urls import router as django_notifications_views_router
 your_router.registry.extend(django_notifications_views_router.registry)
 ```
-    
 
+Add the following to your settings.py if you want to enable Expo Go notifications:
+
+```python
+DJANGO_NOTIFICATIONS_VIEWS = {
+    'USE_EXPO_NOTIFICATIONS': True, # Set to True to enable expo notifications
+    'EXPO_APP_ID': '<your-expo-app-id>', 
+}
+```
 ## Contributing
 
 -   [Juan Ignacio Borrelli](https://www.linkedin.com/in/juan-ignacio-borrelli/)
     
 
 Maintained and developed by [Linkchar Software Development](https://linkchar.com/).
```

### Comparing `django_notifications_views-0.1.1/django_notifications_views.egg-info/SOURCES.txt` & `django_notifications_views-0.1.2/django_notifications_views.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_notifications_views-0.1.1/setup.py` & `django_notifications_views-0.1.2/setup.py`

 * *Files identical despite different names*

