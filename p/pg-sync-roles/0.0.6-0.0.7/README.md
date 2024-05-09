# Comparing `tmp/pg_sync_roles-0.0.6.tar.gz` & `tmp/pg_sync_roles-0.0.7.tar.gz`

## Comparing `pg_sync_roles-0.0.6.tar` & `pg_sync_roles-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.6/pg_sync_roles.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.6/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.6/LICENSE
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.6/README.md
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.7/pg_sync_roles.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.7/README.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.7/PKG-INFO
```

### Comparing `pg_sync_roles-0.0.6/.gitignore` & `pg_sync_roles-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.6/LICENSE` & `pg_sync_roles-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.6/README.md` & `pg_sync_roles-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.6/pyproject.toml` & `pg_sync_roles-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-sync-roles"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Department for Business and Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pg_sync_roles-0.0.6/PKG-INFO` & `pg_sync_roles-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pg-sync-roles
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships
 Project-URL: Source, https://github.com/uktrade/pg-sync-roles
 Author-email: Department for Business and Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

