# Comparing `tmp/flask_project_creator-0.1.tar.gz` & `tmp/flask_project_creator-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_project_creator-0.1.tar", last modified: Thu May  9 06:09:17 2024, max compression
+gzip compressed data, was "flask_project_creator-0.2.tar", last modified: Thu May  9 08:17:04 2024, max compression
```

## Comparing `flask_project_creator-0.1.tar` & `flask_project_creator-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 06:09:17.725315 flask_project_creator-0.1/
--rw-rw-rw-   0        0        0       88 2024-05-09 06:09:17.722314 flask_project_creator-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 06:09:17.657356 flask_project_creator-0.1/flask_project_creator/
--rw-rw-rw-   0        0        0     3154 2024-05-08 18:06:12.000000 flask_project_creator-0.1/flask_project_creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 06:09:17.721315 flask_project_creator-0.1/flask_project_creator.egg-info/
--rw-rw-rw-   0        0        0       88 2024-05-09 06:09:16.000000 flask_project_creator-0.1/flask_project_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2024-05-09 06:09:16.000000 flask_project_creator-0.1/flask_project_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 06:09:16.000000 flask_project_creator-0.1/flask_project_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2024-05-09 06:09:16.000000 flask_project_creator-0.1/flask_project_creator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2024-05-09 06:09:16.000000 flask_project_creator-0.1/flask_project_creator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-09 06:09:16.000000 flask_project_creator-0.1/flask_project_creator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 06:09:17.726319 flask_project_creator-0.1/setup.cfg
--rw-rw-rw-   0        0        0      347 2024-05-08 18:06:40.000000 flask_project_creator-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:17:04.051812 flask_project_creator-0.2/
+-rw-rw-rw-   0        0        0     1141 2024-05-09 08:17:04.049457 flask_project_creator-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 08:17:03.915838 flask_project_creator-0.2/flask_project_creator/
+-rw-rw-rw-   0        0        0     3154 2024-05-08 18:06:12.000000 flask_project_creator-0.2/flask_project_creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:17:04.047441 flask_project_creator-0.2/flask_project_creator.egg-info/
+-rw-rw-rw-   0        0        0     1141 2024-05-09 08:17:03.000000 flask_project_creator-0.2/flask_project_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2024-05-09 08:17:03.000000 flask_project_creator-0.2/flask_project_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 08:17:03.000000 flask_project_creator-0.2/flask_project_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2024-05-09 08:17:03.000000 flask_project_creator-0.2/flask_project_creator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        6 2024-05-09 08:17:03.000000 flask_project_creator-0.2/flask_project_creator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-09 08:17:03.000000 flask_project_creator-0.2/flask_project_creator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 08:17:04.051812 flask_project_creator-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1444 2024-05-09 08:16:24.000000 flask_project_creator-0.2/setup.py
```

### Comparing `flask_project_creator-0.1/flask_project_creator/__init__.py` & `flask_project_creator-0.2/flask_project_creator/__init__.py`

 * *Files identical despite different names*

