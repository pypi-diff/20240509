# Comparing `tmp/adatoolbox-0.0.8.tar.gz` & `tmp/adatoolbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adatoolbox-0.0.8.tar", last modified: Tue Apr 25 15:38:50 2023, max compression
+gzip compressed data, was "adatoolbox-0.0.9.tar", last modified: Mon Sep 25 16:15:37 2023, max compression
```

## Comparing `adatoolbox-0.0.8.tar` & `adatoolbox-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:50.666183 adatoolbox-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-03-27 19:16:17.000000 adatoolbox-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      504 2023-04-25 15:38:50.633689 adatoolbox-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      750 2023-04-25 15:38:35.000000 adatoolbox-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-25 15:38:50.734754 adatoolbox-0.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:44.828911 adatoolbox-0.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:45.849779 adatoolbox-0.0.8/src/adatoolbox/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.8/src/adatoolbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:46.934891 adatoolbox-0.0.8/src/adatoolbox/database/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.8/src/adatoolbox/database/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1007 2023-03-27 19:16:17.000000 adatoolbox-0.0.8/src/adatoolbox/database/base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:45.101646 adatoolbox-0.0.8/src/adatoolbox/domain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:48.367325 adatoolbox-0.0.8/src/adatoolbox/domain/auth/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:54:11.000000 adatoolbox-0.0.8/src/adatoolbox/domain/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1343 2023-03-31 18:34:42.000000 adatoolbox-0.0.8/src/adatoolbox/domain/auth/base_authentication.py
--rw-r--r--   0 root         (0) root         (0)      236 2023-03-31 20:21:16.000000 adatoolbox-0.0.8/src/adatoolbox/domain/auth/base_permission.py
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-11 08:17:51.000000 adatoolbox-0.0.8/src/adatoolbox/domain/auth/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:48.625417 adatoolbox-0.0.8/src/adatoolbox/domain/event/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:28:16.000000 adatoolbox-0.0.8/src/adatoolbox/domain/event/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:49.348686 adatoolbox-0.0.8/src/adatoolbox/domain/event/adapters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:40:22.000000 adatoolbox-0.0.8/src/adatoolbox/domain/event/adapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      547 2023-04-25 15:37:42.000000 adatoolbox-0.0.8/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-04-25 15:34:52.000000 adatoolbox-0.0.8/src/adatoolbox/domain/event/adapters/pika_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:50.150501 adatoolbox-0.0.8/src/adatoolbox/domain/secret/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 11:56:09.000000 adatoolbox-0.0.8/src/adatoolbox/domain/secret/__init__.py
--rw-r--r--   0 root         (0) root         (0)      730 2023-03-31 12:07:26.000000 adatoolbox-0.0.8/src/adatoolbox/domain/secret/doppler.py
--rw-r--r--   0 root         (0) root         (0)       55 2023-03-31 12:06:28.000000 adatoolbox-0.0.8/src/adatoolbox/domain/secret/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:50.540109 adatoolbox-0.0.8/src/adatoolbox/utils/
--rw-r--r--   0 root         (0) root         (0)      293 2023-03-29 14:22:01.000000 adatoolbox-0.0.8/src/adatoolbox/utils/enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 15:38:46.669119 adatoolbox-0.0.8/src/adatoolbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)      504 2023-04-25 15:38:44.000000 adatoolbox-0.0.8/src/adatoolbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      813 2023-04-25 15:38:44.000000 adatoolbox-0.0.8/src/adatoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 15:38:44.000000 adatoolbox-0.0.8/src/adatoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-25 15:38:44.000000 adatoolbox-0.0.8/src/adatoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:37.252527 adatoolbox-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-03-27 19:16:17.000000 adatoolbox-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      504 2023-09-25 16:15:36.762041 adatoolbox-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      750 2023-09-25 16:13:26.000000 adatoolbox-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-09-25 16:15:37.277015 adatoolbox-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:34.856873 adatoolbox-0.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:35.093908 adatoolbox-0.0.9/src/adatoolbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.9/src/adatoolbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:35.351022 adatoolbox-0.0.9/src/adatoolbox/database/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.9/src/adatoolbox/database/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-06-02 19:11:58.000000 adatoolbox-0.0.9/src/adatoolbox/database/base_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:34.944774 adatoolbox-0.0.9/src/adatoolbox/domain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:35.542028 adatoolbox-0.0.9/src/adatoolbox/domain/auth/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:54:11.000000 adatoolbox-0.0.9/src/adatoolbox/domain/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-09-25 15:56:28.000000 adatoolbox-0.0.9/src/adatoolbox/domain/auth/base_authentication.py
+-rw-r--r--   0 root         (0) root         (0)      236 2023-03-31 20:21:16.000000 adatoolbox-0.0.9/src/adatoolbox/domain/auth/base_permission.py
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-11 08:17:51.000000 adatoolbox-0.0.9/src/adatoolbox/domain/auth/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:35.566501 adatoolbox-0.0.9/src/adatoolbox/domain/event/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:28:16.000000 adatoolbox-0.0.9/src/adatoolbox/domain/event/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:35.863101 adatoolbox-0.0.9/src/adatoolbox/domain/event/adapters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:40:22.000000 adatoolbox-0.0.9/src/adatoolbox/domain/event/adapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      547 2023-04-25 15:37:42.000000 adatoolbox-0.0.9/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-04-25 15:34:52.000000 adatoolbox-0.0.9/src/adatoolbox/domain/event/adapters/pika_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:36.190101 adatoolbox-0.0.9/src/adatoolbox/domain/secret/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 11:56:09.000000 adatoolbox-0.0.9/src/adatoolbox/domain/secret/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      730 2023-03-31 12:07:26.000000 adatoolbox-0.0.9/src/adatoolbox/domain/secret/doppler.py
+-rw-r--r--   0 root         (0) root         (0)       55 2023-03-31 12:06:28.000000 adatoolbox-0.0.9/src/adatoolbox/domain/secret/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:36.646765 adatoolbox-0.0.9/src/adatoolbox/utils/
+-rw-r--r--   0 root         (0) root         (0)      293 2023-03-29 14:22:01.000000 adatoolbox-0.0.9/src/adatoolbox/utils/enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:35.265161 adatoolbox-0.0.9/src/adatoolbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-09-25 16:15:34.000000 adatoolbox-0.0.9/src/adatoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      813 2023-09-25 16:15:34.000000 adatoolbox-0.0.9/src/adatoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-25 16:15:34.000000 adatoolbox-0.0.9/src/adatoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-09-25 16:15:34.000000 adatoolbox-0.0.9/src/adatoolbox.egg-info/top_level.txt
```

### Comparing `adatoolbox-0.0.8/LICENSE` & `adatoolbox-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.0.8/pyproject.toml` & `adatoolbox-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 authors = ["Isaias Santana <isaiassantana@alojasengecon.com.br>"]
 description = "Biblioteca Lojas Engecon."
 name = "adatoolbox"
-version = "0.0.8"
+version = "0.0.9"
 
 [project]
 authors = [
   {name = "Lojas Engecon", email = "tecnologia@lojasengecon.com.br"},
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 description = "adatoolbox"
 name = "adatoolbox"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.0.8"
+version = "0.0.9"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/lojas-engecon/toolbox/issues"
 "Homepage" = "https://github.com/lojas-engecon/toolbox"
 
 [tool.poetry.dependencies]
 build = "*"
```

### Comparing `adatoolbox-0.0.8/src/adatoolbox/database/base_model.py` & `adatoolbox-0.0.9/src/adatoolbox/database/base_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from django.db import models
+from simple_history.models import HistoricalRecords
 
 
 class BaseModel(models.Model):
     cd_estabelecimento = models.CharField(
         "Estabelecimento",
         max_length=20,
         null=True,
@@ -35,15 +36,16 @@
         auto_now=True
     )
     dt_deletado = models.DateTimeField(
         "Deletado em",
         null=True,
         blank=True
     )
+    history = HistoricalRecords()
 
-    def delete(self):
-        self.dt_deletado = True
-        self.save()
+    # def delete(self):
+    #     self.dt_deletado = True
+    #     self.save()
 
     class Meta:
         abstract = True
```

### Comparing `adatoolbox-0.0.8/src/adatoolbox/domain/auth/base_authentication.py` & `adatoolbox-0.0.9/src/adatoolbox/domain/auth/base_authentication.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,13 +19,11 @@
         try:
             headers = {"Authorization": f"{token} "}
             url = f"{API_AD_URL}/api-ad/api/usuarios/userdata/"
             response = requests.get(url, headers=headers, timeout=10)
             response.raise_for_status()
             return response.json(), token
         except HTTPError as error:
-            logger.debug(f"JWT Token {token[:3]}**** is Invalid. Permission Denied.")
-            raise exceptions.PermissionDenied(_("Not authorized")) from error
+            logger.debug(f"JWT Token {token[:3]}**** is Invalid. Not authenticated.")
+            raise exceptions.NotAuthenticated(_("Not authenticated")) from error
         except (ConnectionError, Timeout) as error:
-            # sentry_sdk.capture_exception(error)
-            # raise GatewayTimeout(_("Request timeout for Auth-Api server")) from error
             pass
```

### Comparing `adatoolbox-0.0.8/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py` & `adatoolbox-0.0.9/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.0.8/src/adatoolbox/domain/event/adapters/pika_adapter.py` & `adatoolbox-0.0.9/src/adatoolbox/domain/event/adapters/pika_adapter.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.0.8/src/adatoolbox/domain/secret/doppler.py` & `adatoolbox-0.0.9/src/adatoolbox/domain/secret/doppler.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.0.8/src/adatoolbox.egg-info/SOURCES.txt` & `adatoolbox-0.0.9/src/adatoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

