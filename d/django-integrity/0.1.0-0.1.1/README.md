# Comparing `tmp/django_integrity-0.1.0.tar.gz` & `tmp/django_integrity-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_integrity-0.1.0.tar", last modified: Tue May  7 21:07:44 2024, max compression
+gzip compressed data, was "django_integrity-0.1.1.tar", last modified: Thu May  9 09:43:43 2024, max compression
```

## Comparing `django_integrity-0.1.0.tar` & `django_integrity-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:07:44.910139 django_integrity-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-07 21:07:41.000000 django_integrity-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-07 21:07:44.910139 django_integrity-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-07 21:07:41.000000 django_integrity-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-07 21:07:41.000000 django_integrity-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 21:07:44.910139 django_integrity-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:07:44.906139 django_integrity-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:07:44.906139 django_integrity-0.1.0/src/django_integrity/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-07 21:07:41.000000 django_integrity-0.1.0/src/django_integrity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-05-07 21:07:41.000000 django_integrity-0.1.0/src/django_integrity/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-07 21:07:41.000000 django_integrity-0.1.0/src/django_integrity/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 21:07:41.000000 django_integrity-0.1.0/src/django_integrity/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 21:07:44.910139 django_integrity-0.1.0/src/django_integrity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-07 21:07:44.000000 django_integrity-0.1.0/src/django_integrity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-07 21:07:44.000000 django_integrity-0.1.0/src/django_integrity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 21:07:44.000000 django_integrity-0.1.0/src/django_integrity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-07 21:07:44.000000 django_integrity-0.1.0/src/django_integrity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 21:07:44.000000 django_integrity-0.1.0/src/django_integrity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:43:43.701741 django_integrity-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-09 09:43:40.000000 django_integrity-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-09 09:43:43.701741 django_integrity-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-09 09:43:40.000000 django_integrity-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-09 09:43:40.000000 django_integrity-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:43:43.701741 django_integrity-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:43:43.697741 django_integrity-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:43:43.697741 django_integrity-0.1.1/src/django_integrity/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 09:43:40.000000 django_integrity-0.1.1/src/django_integrity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-09 09:43:40.000000 django_integrity-0.1.1/src/django_integrity/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5296 2024-05-09 09:43:40.000000 django_integrity-0.1.1/src/django_integrity/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:43:40.000000 django_integrity-0.1.1/src/django_integrity/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:43:43.701741 django_integrity-0.1.1/src/django_integrity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-09 09:43:43.000000 django_integrity-0.1.1/src/django_integrity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-09 09:43:43.000000 django_integrity-0.1.1/src/django_integrity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:43:43.000000 django_integrity-0.1.1/src/django_integrity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-09 09:43:43.000000 django_integrity-0.1.1/src/django_integrity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 09:43:43.000000 django_integrity-0.1.1/src/django_integrity.egg-info/top_level.txt
```

### Comparing `django_integrity-0.1.0/LICENSE` & `django_integrity-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_integrity-0.1.0/PKG-INFO` & `django_integrity-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_integrity
-Version: 0.1.0
+Version: 0.1.1
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Kraken Technologies Limited
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `django_integrity-0.1.0/README.md` & `django_integrity-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_integrity-0.1.0/pyproject.toml` & `django_integrity-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 where = ["src"]
 
 # Project
 # -------
 
 [project]
 name = "django_integrity"
-version = "0.1.0"
+version = "0.1.1"
 license.file = "LICENSE"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     # We cannot decide for users if they want to use psycopg2, psycopg2-binary, or
     # psycopg (i.e. psycopg3) with or without the [binary] extra. It should be part of
     # their own project dependencies anyway.
```

### Comparing `django_integrity-0.1.0/src/django_integrity/constraints.py` & `django_integrity-0.1.1/src/django_integrity/constraints.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import contextlib
 from collections.abc import Iterator, Sequence
 
 from django import db as django_db
 
+
 try:
     from psycopg import sql
 except ImportError:
     from psycopg2 import sql
 
 
 # Note [Deferrable constraints]
@@ -155,15 +156,15 @@
     because the change of state would only last for the remainder of the transaction.
 
     See https://www.postgresql.org/docs/current/sql-set-constraints.html
     """
 
 
 def foreign_key_constraint_name(
-    model: django_db.models.Model, field_name: str, *, using: str
+    model: type[django_db.models.Model], field_name: str, *, using: str
 ) -> str:
     """
     Calculate FK constraint name for a model's field.
 
     Django's constraint names are based on the names of the tables and columns involved.
 
     Because there is a 63-character limit on constraint names in PostgreSQL,
```

### Comparing `django_integrity-0.1.0/src/django_integrity/conversion.py` & `django_integrity-0.1.1/src/django_integrity/conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import contextlib
 import dataclasses
 import re
 from collections.abc import Iterator, Mapping
 
 from django import db as django_db
 
+
 try:
     import psycopg
 except ImportError:
     import psycopg2 as psycopg
 
 
 @contextlib.contextmanager
@@ -69,15 +70,15 @@
 
 @dataclasses.dataclass(frozen=True)
 class Unique(_Rule):
     """
     A unique constraint defined by a model and a set of fields.
     """
 
-    model: django_db.models.Model
+    model: type[django_db.models.Model]
     fields: tuple[str]
 
     _pattern = re.compile(r"Key \((?P<fields>.+)\)=\(.*\) already exists.")
 
     def is_match(self, error: django_db.IntegrityError) -> bool:
         if not isinstance(error.__cause__, psycopg.errors.UniqueViolation):
             return False
@@ -97,15 +98,15 @@
     """
     A unique constraint on the primary key of a model.
 
     If the model has no primary key, a PrimaryKeyDoesNotExist error is raised when
     trying to create a PrimaryKey rule.
     """
 
-    model: django_db.models.Model
+    model: type[django_db.models.Model]
 
     _pattern = re.compile(r"Key \((?P<fields>.+)\)=\(.*\) already exists.")
 
     def __post_init__(self):
         """
         Ensure the model has a primary key.
 
@@ -144,15 +145,15 @@
 
 @dataclasses.dataclass(frozen=True)
 class NotNull(_Rule):
     """
     A not-null constraint on a Model's field.
     """
 
-    model: django_db.models.Model
+    model: type[django_db.models.Model]
     field: str
 
     def is_match(self, error: django_db.IntegrityError) -> bool:
         if not isinstance(error.__cause__, psycopg.errors.NotNullViolation):
             return False
 
         return (
@@ -163,15 +164,15 @@
 
 @dataclasses.dataclass(frozen=True)
 class ForeignKey(_Rule):
     """
     A foreign key constraint on a Model's field.
     """
 
-    model: django_db.models.Model
+    model: type[django_db.models.Model]
     field: str
 
     _detail_pattern = re.compile(
         r"Key \((?P<field>.+)\)=\((?P<value>.+)\) is not present in table"
     )
 
     def is_match(self, error: django_db.IntegrityError) -> bool:
```

### Comparing `django_integrity-0.1.0/src/django_integrity.egg-info/PKG-INFO` & `django_integrity-0.1.1/src/django_integrity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_integrity
-Version: 0.1.0
+Version: 0.1.1
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Kraken Technologies Limited
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

