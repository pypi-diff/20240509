# Comparing `tmp/leafdb-1.0.1.tar.gz` & `tmp/leafdb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leafdb-1.0.1.tar", last modified: Sun Sep 17 14:31:05 2023, max compression
+gzip compressed data, was "leafdb-1.0.2.tar", last modified: Thu May  9 10:36:18 2024, max compression
```

## Comparing `leafdb-1.0.1.tar` & `leafdb-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 yhq        (501) staff       (20)        0 2023-09-17 14:31:05.553733 leafdb-1.0.1/
--rw-r--r--   0 yhq        (501) staff       (20)      284 2023-09-17 14:31:05.553637 leafdb-1.0.1/PKG-INFO
-drwxr-xr-x   0 yhq        (501) staff       (20)        0 2023-09-17 14:31:05.553510 leafdb-1.0.1/leafdb.egg-info/
--rw-r--r--   0 yhq        (501) staff       (20)      284 2023-09-17 14:31:05.000000 leafdb-1.0.1/leafdb.egg-info/PKG-INFO
--rw-r--r--   0 yhq        (501) staff       (20)      167 2023-09-17 14:31:05.000000 leafdb-1.0.1/leafdb.egg-info/SOURCES.txt
--rw-r--r--   0 yhq        (501) staff       (20)        1 2023-09-17 14:31:05.000000 leafdb-1.0.1/leafdb.egg-info/dependency_links.txt
--rw-r--r--   0 yhq        (501) staff       (20)       11 2023-09-17 14:31:05.000000 leafdb-1.0.1/leafdb.egg-info/requires.txt
--rw-r--r--   0 yhq        (501) staff       (20)        7 2023-09-17 14:31:05.000000 leafdb-1.0.1/leafdb.egg-info/top_level.txt
--rwx------   0 yhq        (501) staff       (20)    29448 2023-09-17 14:30:23.000000 leafdb-1.0.1/leafdb.py
--rw-r--r--   0 yhq        (501) staff       (20)       38 2023-09-17 14:31:05.553773 leafdb-1.0.1/setup.cfg
--rwx------   0 yhq        (501) staff       (20)      502 2023-09-17 14:30:35.000000 leafdb-1.0.1/setup.py
+drwxr-xr-x   0 yhq        (501) staff       (20)        0 2024-05-09 10:36:18.236874 leafdb-1.0.2/
+-rw-r--r--   0 yhq        (501) staff       (20)      308 2024-05-09 10:36:18.236683 leafdb-1.0.2/PKG-INFO
+drwxr-xr-x   0 yhq        (501) staff       (20)        0 2024-05-09 10:36:18.236439 leafdb-1.0.2/leafdb.egg-info/
+-rw-r--r--   0 yhq        (501) staff       (20)      308 2024-05-09 10:36:18.000000 leafdb-1.0.2/leafdb.egg-info/PKG-INFO
+-rw-r--r--   0 yhq        (501) staff       (20)      167 2024-05-09 10:36:18.000000 leafdb-1.0.2/leafdb.egg-info/SOURCES.txt
+-rw-r--r--   0 yhq        (501) staff       (20)        1 2024-05-09 10:36:18.000000 leafdb-1.0.2/leafdb.egg-info/dependency_links.txt
+-rw-r--r--   0 yhq        (501) staff       (20)       11 2024-05-09 10:36:18.000000 leafdb-1.0.2/leafdb.egg-info/requires.txt
+-rw-r--r--   0 yhq        (501) staff       (20)        7 2024-05-09 10:36:18.000000 leafdb-1.0.2/leafdb.egg-info/top_level.txt
+-rw-r--r--   0 yhq        (501) staff       (20)    29790 2024-05-09 10:32:35.000000 leafdb-1.0.2/leafdb.py
+-rw-r--r--   0 yhq        (501) staff       (20)       38 2024-05-09 10:36:18.236919 leafdb-1.0.2/setup.cfg
+-rwx------   0 yhq        (501) staff       (20)      501 2024-05-09 10:35:19.000000 leafdb-1.0.2/setup.py
```

### Comparing `leafdb-1.0.1/leafdb.py` & `leafdb-1.0.2/leafdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
 
 __all__ = ["DbDialect", "database", "SQLConn", "SQLRow", "SQLRowCollection", "SQLParser", "Connection", "BaseDbs",
            "MultipleBaseDbs"]
 
 import os
 import re
 from collections import OrderedDict
@@ -296,34 +296,41 @@
                 _key = "%s%d" % (SQLParser.params_mark, i)
                 params.update({_key: argv})
             kwargs.update(params)
         return " ".join(sqls), kwargs
 
 
 class Connection(object):
-    def __init__(self, connection):
+    def __init__(self, connection, close_with_result=False):
         self._conn = connection
         self._dbtype = (connection.engine.name or "").lower().strip()
         self.open = not connection.closed
+        self._close_with_result = close_with_result
 
     def close(self):
-        self._conn.close()
+        if not self._close_with_result:
+            self._conn.close()
         self.open = False
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc, val, traceback):
         self.close()
 
     def __repr__(self):
         return '<Connection open={}>'.format(self.open)
 
     def query(self, query, fetchall=False, **params):
-        cursor = self._conn.execute(text(query), **params)
+        # Execute the given query.
+        # cursor = self._conn.execute(text(query), **params)
+        cursor = self._conn.execute(
+            text(query).bindparams(**params)
+        )  # TODO: PARAMS GO HERE
+
         if not cursor.keys():  # Skip insert,update has none return values error
         	return None
         row_gen = (SQLRow(cursor.keys(), row) for row in cursor)
         results = SQLRowCollection(row_gen)
         if fetchall:
             results.list()
         return results
@@ -513,21 +520,22 @@
 
     def get_version(self):
         if not self.version:
             _fetchall = True if self._engine.name.lower() == "mssql" else False
             self.version = self.query("select @@version", fetchall=_fetchall).first()[0]
         return self.version
 
-    def get_connection(self):
+    def get_connection(self, close_with_result=False):
         if not self.open:
             raise exc.ResourceClosedError('BaseDbs closed.')
-        return Connection(self._engine.connect())
+
+        return Connection(self._engine.connect(), close_with_result=close_with_result)
 
     def query(self, query, fetchall=False, **params):
-        with self.get_connection() as conn:
+        with self.get_connection(True) as conn:
             return conn.query(query, fetchall, **params)
 
     def bulk_query(self, query, *multiparams):
         with self.get_connection() as conn:
             conn.bulk_query(query, *multiparams)
 
     def query_file(self, path, fetchall=False, **params):
```

