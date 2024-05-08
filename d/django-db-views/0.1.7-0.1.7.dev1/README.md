# Comparing `tmp/django-db-views-0.1.7.tar.gz` & `tmp/django_db_views-0.1.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-db-views-0.1.7.tar", last modified: Mon May  6 20:58:58 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `django-db-views-0.1.7.tar` & `django_db_views-0.1.7.dev1.tar`

### file list

```diff
@@ -1,40 +1,15 @@
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.520457 django-db-views-0.1.7/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1074 2023-07-13 18:00:46.000000 django-db-views-0.1.7/LICENSE
--rw-r--r--   0 bartlomiej  (1000) bartlomiej  (1000)     5976 2024-05-06 20:58:58.520457 django-db-views-0.1.7/PKG-INFO
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     4926 2023-12-02 21:56:45.000000 django-db-views-0.1.7/README.md
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.516457 django-db-views-0.1.7/django_db_views/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       32 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/__init__.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)    15199 2024-05-06 20:58:07.000000 django-db-views-0.1.7/django_db_views/autodetector.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      416 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/context_manager.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1408 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/db_view.py
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.520457 django-db-views-0.1.7/django_db_views/management/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/management/__init__.py
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.520457 django-db-views-0.1.7/django_db_views/management/commands/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/management/commands/__init__.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     4797 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/management/commands/makeviewmigrations.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     2935 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/migration_functions.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     2596 2023-07-13 18:00:46.000000 django-db-views-0.1.7/django_db_views/operations.py
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.520457 django-db-views-0.1.7/django_db_views.egg-info/
--rw-r--r--   0 bartlomiej  (1000) bartlomiej  (1000)     5976 2024-05-06 20:58:58.000000 django-db-views-0.1.7/django_db_views.egg-info/PKG-INFO
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      901 2024-05-06 20:58:58.000000 django-db-views-0.1.7/django_db_views.egg-info/SOURCES.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        1 2024-05-06 20:58:58.000000 django-db-views-0.1.7/django_db_views.egg-info/dependency_links.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       11 2024-05-06 20:58:58.000000 django-db-views-0.1.7/django_db_views.egg-info/requires.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       22 2024-05-06 20:58:58.000000 django-db-views-0.1.7/django_db_views.egg-info/top_level.txt
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)       38 2024-05-06 20:58:58.520457 django-db-views-0.1.7/setup.cfg
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1582 2024-05-06 20:58:07.000000 django-db-views-0.1.7/setup.py
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.520457 django-db-views-0.1.7/tests/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/__init__.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      529 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/asserts_utils.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1541 2024-05-06 20:58:07.000000 django-db-views-0.1.7/tests/conftest.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      380 2023-12-27 10:36:42.000000 django-db-views-0.1.7/tests/decorators.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     2444 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/dynamic_models_fixtures.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1493 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/fixturies.py
-drwxrwxr-x   0 bartlomiej  (1000) bartlomiej  (1000)        0 2024-05-06 20:58:58.520457 django-db-views-0.1.7/tests/test_app/
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/test_app/__init__.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     4370 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/test_app/models.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/test_autodetector.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     1018 2024-05-05 22:09:17.000000 django-db-views-0.1.7/tests/test_backward_compatibility.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)        0 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/test_db_functions.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)    14171 2024-05-06 20:58:07.000000 django-db-views-0.1.7/tests/test_db_views.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)     3025 2023-07-13 18:00:46.000000 django-db-views-0.1.7/tests/test_materialized_views.py
--rw-rw-r--   0 bartlomiej  (1000) bartlomiej  (1000)      143 2024-05-06 20:58:07.000000 django-db-views-0.1.7/tests/utils.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/CHANGELOG.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/__init__.py
+-rw-r--r--   0        0        0    15199 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/autodetector.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/context_manager.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/db_view.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/migration_functions.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/operations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/management/commands/__init__.py
+-rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/django_db_views/management/commands/makeviewmigrations.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/LICENSE
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/README.md
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/pyproject.toml
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 django_db_views-0.1.7.dev1/PKG-INFO
```

### Comparing `django-db-views-0.1.7/LICENSE` & `django_db_views-0.1.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.7/PKG-INFO` & `django_db_views-0.1.7.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: django-db-views
-Version: 0.1.7
-Summary: Handle database views. Allow to create migrations for database views. View migrations using django code. They can be reversed. Changes in model view definition are detected automatically. Support almost all options as regular makemigrations command
-Home-page: https://github.com/BezBartek/django-db-views
-Author: Bartłomiej Nowak and Mariusz Okulanis
-Author-email: n.bartek3762@gmail.com
-License: MIT
-Keywords: views,database views,django,database perspective,view migrations,database table function,django materialized views
+Version: 0.1.7.dev1
+Summary:     Handle database views.     Allow to create migrations for database views.     View migrations using django code.     They can be reversed.     Changes in model view definition are detected automatically.     Support almost all options as regular makemigrations command
+Project-URL: Homepage, https://github.com/BezBartek/django-db-views
+Project-URL: Documentation, https://github.com/BezBartek/django-db-views/blob/master/README.md
+Project-URL: Repository, https://github.com/BezBartek/django-db-views
+Project-URL: Issues, https://github.com/BezBartek/django-db-views/issues
+Project-URL: Changelog, https://github.com/BezBartek/django-db-views/blob/master/CHANGELOG.md
+Author: Mariusz Okulanis
+Author-email: Bartłomiej Nowak <n.bartek3762@gmail.com>
+Maintainer-email: Bartłomiej Nowak <n.bartek3762@gmail.com>
+License: MIT License
+License-File: LICENSE
+Keywords: database perspective,database table function,database views,django,django materialized views,view migrations,views
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: django
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Django
-Requires-Dist: six
 
 # django-db-views
 
 
 [![License](https://img.shields.io/:license-mit-blue.svg)](http://doge.mit-license.org)  
 [![PyPi](https://badge.fury.io/py/django-db-views.svg)](https://pypi.org/project/django-db-views/)  
 **Django Versions** 2.2 to 4.2+
```

### Comparing `django-db-views-0.1.7/README.md` & `django_db_views-0.1.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.7/django_db_views/autodetector.py` & `django_db_views-0.1.7.dev1/django_db_views/autodetector.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.7/django_db_views/db_view.py` & `django_db_views-0.1.7.dev1/django_db_views/db_view.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.7/django_db_views/management/commands/makeviewmigrations.py` & `django_db_views-0.1.7.dev1/django_db_views/management/commands/makeviewmigrations.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.7/django_db_views/migration_functions.py` & `django_db_views-0.1.7.dev1/django_db_views/migration_functions.py`

 * *Files identical despite different names*

### Comparing `django-db-views-0.1.7/django_db_views/operations.py` & `django_db_views-0.1.7.dev1/django_db_views/operations.py`

 * *Files identical despite different names*

