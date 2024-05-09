# Comparing `tmp/adatoolbox-0.1.16.tar.gz` & `tmp/adatoolbox-0.2.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adatoolbox-0.1.16.tar", last modified: Thu May  9 12:15:43 2024, max compression
+gzip compressed data, was "adatoolbox-0.2.16.tar", last modified: Thu May  9 12:23:13 2024, max compression
```

## Comparing `adatoolbox-0.1.16.tar` & `adatoolbox-0.2.16.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:43.287801 adatoolbox-0.1.16/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-03-27 19:16:17.000000 adatoolbox-0.1.16/LICENSE
--rw-r--r--   0 root         (0) root         (0)      508 2024-05-09 12:15:43.247780 adatoolbox-0.1.16/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.1.16/README.md
--rw-r--r--   0 root         (0) root         (0)      755 2024-05-09 12:15:10.000000 adatoolbox-0.1.16/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 12:15:43.290594 adatoolbox-0.1.16/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:41.462299 adatoolbox-0.1.16/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:41.919125 adatoolbox-0.1.16/src/adatoolbox/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.1.16/src/adatoolbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:41.668100 adatoolbox-0.1.16/src/adatoolbox/domain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:42.462154 adatoolbox-0.1.16/src/adatoolbox/domain/auth/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:54:11.000000 adatoolbox-0.1.16/src/adatoolbox/domain/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1485 2024-05-09 12:11:20.000000 adatoolbox-0.1.16/src/adatoolbox/domain/auth/base_authentication.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-12-07 17:39:39.000000 adatoolbox-0.1.16/src/adatoolbox/domain/auth/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:42.589860 adatoolbox-0.1.16/src/adatoolbox/domain/database/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-29 20:02:08.000000 adatoolbox-0.1.16/src/adatoolbox/domain/database/__init__.py
--rw-r--r--   0 root         (0) root         (0)      840 2023-12-07 14:44:37.000000 adatoolbox-0.1.16/src/adatoolbox/domain/database/base_model.py
--rw-r--r--   0 root         (0) root         (0)       10 2023-12-07 17:41:05.000000 adatoolbox-0.1.16/src/adatoolbox/domain/database/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:42.640415 adatoolbox-0.1.16/src/adatoolbox/domain/event/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:28:16.000000 adatoolbox-0.1.16/src/adatoolbox/domain/event/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:42.838300 adatoolbox-0.1.16/src/adatoolbox/domain/event/adapters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:40:22.000000 adatoolbox-0.1.16/src/adatoolbox/domain/event/adapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      547 2023-04-25 15:37:42.000000 adatoolbox-0.1.16/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-04-25 15:34:52.000000 adatoolbox-0.1.16/src/adatoolbox/domain/event/adapters/pika_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:42.942004 adatoolbox-0.1.16/src/adatoolbox/domain/memory/
--rw-r--r--   0 root         (0) root         (0)        0 2023-12-08 23:14:52.000000 adatoolbox-0.1.16/src/adatoolbox/domain/memory/__init__.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-12-11 14:17:34.000000 adatoolbox-0.1.16/src/adatoolbox/domain/memory/memory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:43.099208 adatoolbox-0.1.16/src/adatoolbox/domain/secret/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 11:56:09.000000 adatoolbox-0.1.16/src/adatoolbox/domain/secret/__init__.py
--rw-r--r--   0 root         (0) root         (0)      730 2023-03-31 12:07:26.000000 adatoolbox-0.1.16/src/adatoolbox/domain/secret/doppler.py
--rw-r--r--   0 root         (0) root         (0)       55 2023-03-31 12:06:28.000000 adatoolbox-0.1.16/src/adatoolbox/domain/secret/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:43.146156 adatoolbox-0.1.16/src/adatoolbox/utils/
--rw-r--r--   0 root         (0) root         (0)      293 2023-03-29 14:22:01.000000 adatoolbox-0.1.16/src/adatoolbox/utils/enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:43.196063 adatoolbox-0.1.16/src/adatoolbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)      508 2024-05-09 12:15:41.000000 adatoolbox-0.1.16/src/adatoolbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      904 2024-05-09 12:15:41.000000 adatoolbox-0.1.16/src/adatoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 12:15:41.000000 adatoolbox-0.1.16/src/adatoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-09 12:15:41.000000 adatoolbox-0.1.16/src/adatoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:23:12.905165 adatoolbox-0.2.16/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-03-27 19:16:17.000000 adatoolbox-0.2.16/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      508 2024-05-09 12:23:12.860497 adatoolbox-0.2.16/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.2.16/README.md
+-rw-r--r--   0 root         (0) root         (0)      755 2024-05-09 12:22:54.000000 adatoolbox-0.2.16/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 12:23:12.993635 adatoolbox-0.2.16/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:23:10.104975 adatoolbox-0.2.16/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:23:10.421236 adatoolbox-0.2.16/src/adatoolbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.2.16/src/adatoolbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:23:10.229337 adatoolbox-0.2.16/src/adatoolbox/domain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:23:11.349900 adatoolbox-0.2.16/src/adatoolbox/domain/auth/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:54:11.000000 adatoolbox-0.2.16/src/adatoolbox/domain/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-05-09 12:22:29.000000 adatoolbox-0.2.16/src/adatoolbox/domain/auth/base_authentication.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-12-07 17:39:39.000000 adatoolbox-0.2.16/src/adatoolbox/domain/auth/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:23:11.642961 adatoolbox-0.2.16/src/adatoolbox/domain/database/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-11-29 20:02:08.000000 adatoolbox-0.2.16/src/adatoolbox/domain/database/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      840 2023-12-07 14:44:37.000000 adatoolbox-0.2.16/src/adatoolbox/domain/database/base_model.py
+-rw-r--r--   0 root         (0) root         (0)       10 2023-12-07 17:41:05.000000 adatoolbox-0.2.16/src/adatoolbox/domain/database/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:23:11.702792 adatoolbox-0.2.16/src/adatoolbox/domain/event/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:28:16.000000 adatoolbox-0.2.16/src/adatoolbox/domain/event/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:23:12.141090 adatoolbox-0.2.16/src/adatoolbox/domain/event/adapters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:40:22.000000 adatoolbox-0.2.16/src/adatoolbox/domain/event/adapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      547 2023-04-25 15:37:42.000000 adatoolbox-0.2.16/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-04-25 15:34:52.000000 adatoolbox-0.2.16/src/adatoolbox/domain/event/adapters/pika_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:23:12.466051 adatoolbox-0.2.16/src/adatoolbox/domain/memory/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-08 23:14:52.000000 adatoolbox-0.2.16/src/adatoolbox/domain/memory/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-12-11 14:17:34.000000 adatoolbox-0.2.16/src/adatoolbox/domain/memory/memory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:23:12.683311 adatoolbox-0.2.16/src/adatoolbox/domain/secret/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 11:56:09.000000 adatoolbox-0.2.16/src/adatoolbox/domain/secret/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      730 2023-03-31 12:07:26.000000 adatoolbox-0.2.16/src/adatoolbox/domain/secret/doppler.py
+-rw-r--r--   0 root         (0) root         (0)       55 2023-03-31 12:06:28.000000 adatoolbox-0.2.16/src/adatoolbox/domain/secret/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:23:12.745514 adatoolbox-0.2.16/src/adatoolbox/utils/
+-rw-r--r--   0 root         (0) root         (0)      293 2023-03-29 14:22:01.000000 adatoolbox-0.2.16/src/adatoolbox/utils/enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:23:12.820581 adatoolbox-0.2.16/src/adatoolbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      508 2024-05-09 12:23:09.000000 adatoolbox-0.2.16/src/adatoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      904 2024-05-09 12:23:09.000000 adatoolbox-0.2.16/src/adatoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 12:23:09.000000 adatoolbox-0.2.16/src/adatoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-09 12:23:09.000000 adatoolbox-0.2.16/src/adatoolbox.egg-info/top_level.txt
```

### Comparing `adatoolbox-0.1.16/LICENSE` & `adatoolbox-0.2.16/LICENSE`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.1.16/pyproject.toml` & `adatoolbox-0.2.16/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 authors = ["Isaias Santana <isaiassantana@alojasengecon.com.br>"]
 description = "Biblioteca Lojas Engecon."
 name = "adatoolbox"
-version = "0.1.16"
+version = "0.2.16"
 
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
-version = "0.1.16"
+version = "0.2.16"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/pievotecnologia/adatoolbox"
 "Homepage" = "https://github.com/pievotecnologia/adatoolbox"
 
 [tool.poetry.dependencies]
 build = "*"
```

### Comparing `adatoolbox-0.1.16/src/adatoolbox/domain/auth/base_authentication.py` & `adatoolbox-0.2.16/src/adatoolbox/domain/auth/base_authentication.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         try:
             token = jwt.decode(
                 http_authorizaton.split(' ')[1],
                 settings.AUTHENTICATION_API_SECRET_KEY,
                 algorithms=["HS256"])
         except Exception as error:
             logger.error(error)
-            raise exceptions.NotAuthenticated({"detail": "Invalid Token."})
+            raise exceptions.NotAuthenticated({"detail": "Invalid Token"})
         
         try:
             user = Memory.get('user_{}'.format(token.get('user_id')))
         except Exception as error:
             logger.error(error)
             raise exceptions.ValidationError(
                 {"detail": "We are having an authentication problem. Please try again later."})
```

### Comparing `adatoolbox-0.1.16/src/adatoolbox/domain/database/base_model.py` & `adatoolbox-0.2.16/src/adatoolbox/domain/database/base_model.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.1.16/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py` & `adatoolbox-0.2.16/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.1.16/src/adatoolbox/domain/event/adapters/pika_adapter.py` & `adatoolbox-0.2.16/src/adatoolbox/domain/event/adapters/pika_adapter.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.1.16/src/adatoolbox/domain/memory/memory.py` & `adatoolbox-0.2.16/src/adatoolbox/domain/memory/memory.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.1.16/src/adatoolbox/domain/secret/doppler.py` & `adatoolbox-0.2.16/src/adatoolbox/domain/secret/doppler.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.1.16/src/adatoolbox.egg-info/SOURCES.txt` & `adatoolbox-0.2.16/src/adatoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

