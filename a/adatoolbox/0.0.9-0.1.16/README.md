# Comparing `tmp/adatoolbox-0.0.9.tar.gz` & `tmp/adatoolbox-0.1.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adatoolbox-0.0.9.tar", last modified: Mon Sep 25 16:15:37 2023, max compression
+gzip compressed data, was "adatoolbox-0.1.16.tar", last modified: Thu May  9 12:15:43 2024, max compression
```

## Comparing `adatoolbox-0.0.9.tar` & `adatoolbox-0.1.16.tar`

### file list

```diff
@@ -1,35 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:37.252527 adatoolbox-0.0.9/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-03-27 19:16:17.000000 adatoolbox-0.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)      504 2023-09-25 16:15:36.762041 adatoolbox-0.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.9/README.md
--rw-r--r--   0 root         (0) root         (0)      750 2023-09-25 16:13:26.000000 adatoolbox-0.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-09-25 16:15:37.277015 adatoolbox-0.0.9/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:34.856873 adatoolbox-0.0.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:35.093908 adatoolbox-0.0.9/src/adatoolbox/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.9/src/adatoolbox/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:35.351022 adatoolbox-0.0.9/src/adatoolbox/database/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.0.9/src/adatoolbox/database/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1099 2023-06-02 19:11:58.000000 adatoolbox-0.0.9/src/adatoolbox/database/base_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:34.944774 adatoolbox-0.0.9/src/adatoolbox/domain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:35.542028 adatoolbox-0.0.9/src/adatoolbox/domain/auth/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:54:11.000000 adatoolbox-0.0.9/src/adatoolbox/domain/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-09-25 15:56:28.000000 adatoolbox-0.0.9/src/adatoolbox/domain/auth/base_authentication.py
--rw-r--r--   0 root         (0) root         (0)      236 2023-03-31 20:21:16.000000 adatoolbox-0.0.9/src/adatoolbox/domain/auth/base_permission.py
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-11 08:17:51.000000 adatoolbox-0.0.9/src/adatoolbox/domain/auth/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:35.566501 adatoolbox-0.0.9/src/adatoolbox/domain/event/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:28:16.000000 adatoolbox-0.0.9/src/adatoolbox/domain/event/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:35.863101 adatoolbox-0.0.9/src/adatoolbox/domain/event/adapters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:40:22.000000 adatoolbox-0.0.9/src/adatoolbox/domain/event/adapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)      547 2023-04-25 15:37:42.000000 adatoolbox-0.0.9/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-04-25 15:34:52.000000 adatoolbox-0.0.9/src/adatoolbox/domain/event/adapters/pika_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:36.190101 adatoolbox-0.0.9/src/adatoolbox/domain/secret/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 11:56:09.000000 adatoolbox-0.0.9/src/adatoolbox/domain/secret/__init__.py
--rw-r--r--   0 root         (0) root         (0)      730 2023-03-31 12:07:26.000000 adatoolbox-0.0.9/src/adatoolbox/domain/secret/doppler.py
--rw-r--r--   0 root         (0) root         (0)       55 2023-03-31 12:06:28.000000 adatoolbox-0.0.9/src/adatoolbox/domain/secret/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:36.646765 adatoolbox-0.0.9/src/adatoolbox/utils/
--rw-r--r--   0 root         (0) root         (0)      293 2023-03-29 14:22:01.000000 adatoolbox-0.0.9/src/adatoolbox/utils/enum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-25 16:15:35.265161 adatoolbox-0.0.9/src/adatoolbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)      504 2023-09-25 16:15:34.000000 adatoolbox-0.0.9/src/adatoolbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      813 2023-09-25 16:15:34.000000 adatoolbox-0.0.9/src/adatoolbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-25 16:15:34.000000 adatoolbox-0.0.9/src/adatoolbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-09-25 16:15:34.000000 adatoolbox-0.0.9/src/adatoolbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:43.287801 adatoolbox-0.1.16/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-03-27 19:16:17.000000 adatoolbox-0.1.16/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      508 2024-05-09 12:15:43.247780 adatoolbox-0.1.16/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.1.16/README.md
+-rw-r--r--   0 root         (0) root         (0)      755 2024-05-09 12:15:10.000000 adatoolbox-0.1.16/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 12:15:43.290594 adatoolbox-0.1.16/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:41.462299 adatoolbox-0.1.16/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:41.919125 adatoolbox-0.1.16/src/adatoolbox/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-27 19:16:17.000000 adatoolbox-0.1.16/src/adatoolbox/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:41.668100 adatoolbox-0.1.16/src/adatoolbox/domain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:42.462154 adatoolbox-0.1.16/src/adatoolbox/domain/auth/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 12:54:11.000000 adatoolbox-0.1.16/src/adatoolbox/domain/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2024-05-09 12:11:20.000000 adatoolbox-0.1.16/src/adatoolbox/domain/auth/base_authentication.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-12-07 17:39:39.000000 adatoolbox-0.1.16/src/adatoolbox/domain/auth/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:42.589860 adatoolbox-0.1.16/src/adatoolbox/domain/database/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-11-29 20:02:08.000000 adatoolbox-0.1.16/src/adatoolbox/domain/database/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      840 2023-12-07 14:44:37.000000 adatoolbox-0.1.16/src/adatoolbox/domain/database/base_model.py
+-rw-r--r--   0 root         (0) root         (0)       10 2023-12-07 17:41:05.000000 adatoolbox-0.1.16/src/adatoolbox/domain/database/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:42.640415 adatoolbox-0.1.16/src/adatoolbox/domain/event/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:28:16.000000 adatoolbox-0.1.16/src/adatoolbox/domain/event/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:42.838300 adatoolbox-0.1.16/src/adatoolbox/domain/event/adapters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 14:40:22.000000 adatoolbox-0.1.16/src/adatoolbox/domain/event/adapters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      547 2023-04-25 15:37:42.000000 adatoolbox-0.1.16/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-04-25 15:34:52.000000 adatoolbox-0.1.16/src/adatoolbox/domain/event/adapters/pika_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:42.942004 adatoolbox-0.1.16/src/adatoolbox/domain/memory/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-08 23:14:52.000000 adatoolbox-0.1.16/src/adatoolbox/domain/memory/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-12-11 14:17:34.000000 adatoolbox-0.1.16/src/adatoolbox/domain/memory/memory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:43.099208 adatoolbox-0.1.16/src/adatoolbox/domain/secret/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-31 11:56:09.000000 adatoolbox-0.1.16/src/adatoolbox/domain/secret/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      730 2023-03-31 12:07:26.000000 adatoolbox-0.1.16/src/adatoolbox/domain/secret/doppler.py
+-rw-r--r--   0 root         (0) root         (0)       55 2023-03-31 12:06:28.000000 adatoolbox-0.1.16/src/adatoolbox/domain/secret/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:43.146156 adatoolbox-0.1.16/src/adatoolbox/utils/
+-rw-r--r--   0 root         (0) root         (0)      293 2023-03-29 14:22:01.000000 adatoolbox-0.1.16/src/adatoolbox/utils/enum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 12:15:43.196063 adatoolbox-0.1.16/src/adatoolbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      508 2024-05-09 12:15:41.000000 adatoolbox-0.1.16/src/adatoolbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      904 2024-05-09 12:15:41.000000 adatoolbox-0.1.16/src/adatoolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 12:15:41.000000 adatoolbox-0.1.16/src/adatoolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-09 12:15:41.000000 adatoolbox-0.1.16/src/adatoolbox.egg-info/top_level.txt
```

### Comparing `adatoolbox-0.0.9/LICENSE` & `adatoolbox-0.1.16/LICENSE`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.0.9/pyproject.toml` & `adatoolbox-0.1.16/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 authors = ["Isaias Santana <isaiassantana@alojasengecon.com.br>"]
 description = "Biblioteca Lojas Engecon."
 name = "adatoolbox"
-version = "0.0.9"
+version = "0.1.16"
 
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
-version = "0.0.9"
+version = "0.1.16"
 
 [project.urls]
-"Bug Tracker" = "https://github.com/lojas-engecon/toolbox/issues"
-"Homepage" = "https://github.com/lojas-engecon/toolbox"
+"Bug Tracker" = "https://github.com/pievotecnologia/adatoolbox"
+"Homepage" = "https://github.com/pievotecnologia/adatoolbox"
 
 [tool.poetry.dependencies]
 build = "*"
 loguru = "^0.7.0"
 pika = "^1.3.1"
 python = "^3.9"
 twine = "*"
```

### Comparing `adatoolbox-0.0.9/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py` & `adatoolbox-0.1.16/src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.0.9/src/adatoolbox/domain/event/adapters/pika_adapter.py` & `adatoolbox-0.1.16/src/adatoolbox/domain/event/adapters/pika_adapter.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.0.9/src/adatoolbox/domain/secret/doppler.py` & `adatoolbox-0.1.16/src/adatoolbox/domain/secret/doppler.py`

 * *Files identical despite different names*

### Comparing `adatoolbox-0.0.9/src/adatoolbox.egg-info/SOURCES.txt` & `adatoolbox-0.1.16/src/adatoolbox.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,23 @@
 README.md
 pyproject.toml
 src/adatoolbox/__init__.py
 src/adatoolbox.egg-info/PKG-INFO
 src/adatoolbox.egg-info/SOURCES.txt
 src/adatoolbox.egg-info/dependency_links.txt
 src/adatoolbox.egg-info/top_level.txt
-src/adatoolbox/database/__init__.py
-src/adatoolbox/database/base_model.py
 src/adatoolbox/domain/auth/__init__.py
 src/adatoolbox/domain/auth/base_authentication.py
-src/adatoolbox/domain/auth/base_permission.py
 src/adatoolbox/domain/auth/settings.py
+src/adatoolbox/domain/database/__init__.py
+src/adatoolbox/domain/database/base_model.py
+src/adatoolbox/domain/database/settings.py
 src/adatoolbox/domain/event/__init__.py
 src/adatoolbox/domain/event/adapters/__init__.py
 src/adatoolbox/domain/event/adapters/mq_publisher_adapter.py
 src/adatoolbox/domain/event/adapters/pika_adapter.py
+src/adatoolbox/domain/memory/__init__.py
+src/adatoolbox/domain/memory/memory.py
 src/adatoolbox/domain/secret/__init__.py
 src/adatoolbox/domain/secret/doppler.py
 src/adatoolbox/domain/secret/settings.py
 src/adatoolbox/utils/enum.py
```

