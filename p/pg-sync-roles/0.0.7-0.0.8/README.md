# Comparing `tmp/pg_sync_roles-0.0.7.tar.gz` & `tmp/pg_sync_roles-0.0.8.tar.gz`

## Comparing `pg_sync_roles-0.0.7.tar` & `pg_sync_roles-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.7/pg_sync_roles.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.7/.gitignore
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.7/LICENSE
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.7/README.md
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.8/pg_sync_roles.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.8/README.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5443 2020-02-02 00:00:00.000000 pg_sync_roles-0.0.8/PKG-INFO
```

### Comparing `pg_sync_roles-0.0.7/pg_sync_roles.py` & `pg_sync_roles-0.0.8/pg_sync_roles.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         )).fetchall()[0][0]
 
     def get_database_connect_roles(database_names):
         if database_names:
             existing_database_connect_roles_rows = execute_sql(sql.SQL("""
                 SELECT datname, grantee::regrole
                 FROM pg_database, aclexplode(datacl)
-                WHERE grantee::regrole::text LIKE 'database\\_connect\\_%'
+                WHERE grantee::regrole::text LIKE '\\_pgsr\\_database\\_connect\\_%'
                 AND privilege_type = 'CONNECT'
                 AND datname IN ({database_names})
             """).format(database_names=sql.SQL(',').join(sql.Literal(database_name) for database_name in database_names))).fetchall()
         else:
             existing_database_connect_roles_rows = []
 
         existing_database_connect_roles_dict = {
@@ -74,15 +74,15 @@
         return tuple(membership for membership, in membership_rows)
 
     def create_role(role_name):
         execute_sql(sql.SQL('CREATE ROLE {role_name};').format(role_name=sql.Identifier(role_name)))
 
     def get_available_database_connect_role():
         for _ in range(0, 10):
-            database_connect_role = 'database_connect_' + uuid4().hex[:8]
+            database_connect_role = '_pgsr_database_connect_' + uuid4().hex[:8]
             if not get_role_exists(database_connect_role):
                 return database_connect_role
 
         raise Exception('Unable to find available role name')
 
     def grant_connect(database_name, role_name):
         execute_sql(sql.SQL('GRANT CONNECT ON DATABASE {database_name} TO {role_name}').format(
```

### Comparing `pg_sync_roles-0.0.7/.gitignore` & `pg_sync_roles-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.7/LICENSE` & `pg_sync_roles-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_sync_roles-0.0.7/README.md` & `pg_sync_roles-0.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 > [!WARNING]  
 > Work in progress. This README serves as a rough design spec.
 
 ## Features
 
 - Transparently handles high numbers of permissions - avoiding "row is too big" errors.
-- Locks where necessary - working around "tuple concurrently updated" or "tuple concurrently deleted" errors" that can happen when permission changes are performed concurrently.
-- Optionally removes permissions from roles
+- Locks where necessary - working around "tuple concurrently updated" or "tuple concurrently deleted" errors that can happen when permission changes are performed concurrently.
+- Optionally removes permissions from roles.
 - Handles database connect, schema usage, table select permissions, and role memberships - typically useful when using PostgreSQL as a data warehouse with a high number of users that need granular permissions.
 
 
 ## Installation
 
 pg-sync-roles can be installed from PyPI using pip. psycopg2 or psycopg (Psycopg 3) must also be explicitly installed.
 
@@ -23,27 +23,28 @@
 
 
 ## Usage
 
 To give a user CONNECT privileges on a database, as well as membership of role:
 
 ```python
-from pg_sync_roles import DatabaseConnect, RoleMembership, sync_roles
+from pg_sync_roles import Login, DatabaseConnect, RoleMembership, sync_roles
 
 # For example purposes, PostgreSQL can be run locally using this...
 # docker run --rm -it -e POSTGRES_HOST_AUTH_METHOD=trust -p 5432:5432 postgres
 
 # ... which should work with this engine
 engine = sa.create_engine('postgresql+psycopg://postgres@127.0.0.1:5432/')
 
 with engine.begin() as conn:
     sync_roles(
         conn,
         'my_user_name',
         grants=(
+            Login(password='...', valid_until='...'),
             DatabaseConnect('my_database_name'),
             RoleMembership('my_role_name'),
         ),
     )
 ```
 
 A more complex example, where permissions and memberships are granted, but also any existing permissions not passed are revoked:
@@ -76,14 +77,21 @@
             SchemaUsage,
             RoleMembership,
         ),
     )
 ```
 
 
+## Under the hood
+
+pg-sync-roles maintains a role per database perimission, a role per schema pemission, and and per table permission, and rather than roles being granted permissions directly on objects, membership is granted to these roles that indirectly grant permissions on objects. This means that from the object's point of view, only 1 role has any given permission. This works around the de-facto limit on the number of roles that can have permission to any object.
+
+The names of the roles maintained by pg-sync-roles begin with the prefix `_pgsr_`. Each name ends with a randomly generated unique identifier.
+
+
 ## Compatibility
 
 pg-sync-roles aims to be compatible with a wide range of Python and other dependencies:
 
 - Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
 - psycopg2 >= 2.9.2 and Psycopg 3 >= 3.1.4
 - SQLAlchemy >= 1.4.24 (tested on 1.4.24 and 2.0.0)
```

### Comparing `pg_sync_roles-0.0.7/pyproject.toml` & `pg_sync_roles-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-sync-roles"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Department for Business and Trade", email="sre@digital.trade.gov.uk" },
 ]
 description = "Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pg_sync_roles-0.0.7/PKG-INFO` & `pg_sync_roles-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pg-sync-roles
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python utility function to ensure that a PostgreSQL role has certain permissions or role memberships
 Project-URL: Source, https://github.com/uktrade/pg-sync-roles
 Author-email: Department for Business and Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -32,16 +32,16 @@
 
 > [!WARNING]  
 > Work in progress. This README serves as a rough design spec.
 
 ## Features
 
 - Transparently handles high numbers of permissions - avoiding "row is too big" errors.
-- Locks where necessary - working around "tuple concurrently updated" or "tuple concurrently deleted" errors" that can happen when permission changes are performed concurrently.
-- Optionally removes permissions from roles
+- Locks where necessary - working around "tuple concurrently updated" or "tuple concurrently deleted" errors that can happen when permission changes are performed concurrently.
+- Optionally removes permissions from roles.
 - Handles database connect, schema usage, table select permissions, and role memberships - typically useful when using PostgreSQL as a data warehouse with a high number of users that need granular permissions.
 
 
 ## Installation
 
 pg-sync-roles can be installed from PyPI using pip. psycopg2 or psycopg (Psycopg 3) must also be explicitly installed.
 
@@ -51,27 +51,28 @@
 
 
 ## Usage
 
 To give a user CONNECT privileges on a database, as well as membership of role:
 
 ```python
-from pg_sync_roles import DatabaseConnect, RoleMembership, sync_roles
+from pg_sync_roles import Login, DatabaseConnect, RoleMembership, sync_roles
 
 # For example purposes, PostgreSQL can be run locally using this...
 # docker run --rm -it -e POSTGRES_HOST_AUTH_METHOD=trust -p 5432:5432 postgres
 
 # ... which should work with this engine
 engine = sa.create_engine('postgresql+psycopg://postgres@127.0.0.1:5432/')
 
 with engine.begin() as conn:
     sync_roles(
         conn,
         'my_user_name',
         grants=(
+            Login(password='...', valid_until='...'),
             DatabaseConnect('my_database_name'),
             RoleMembership('my_role_name'),
         ),
     )
 ```
 
 A more complex example, where permissions and memberships are granted, but also any existing permissions not passed are revoked:
@@ -104,14 +105,21 @@
             SchemaUsage,
             RoleMembership,
         ),
     )
 ```
 
 
+## Under the hood
+
+pg-sync-roles maintains a role per database perimission, a role per schema pemission, and and per table permission, and rather than roles being granted permissions directly on objects, membership is granted to these roles that indirectly grant permissions on objects. This means that from the object's point of view, only 1 role has any given permission. This works around the de-facto limit on the number of roles that can have permission to any object.
+
+The names of the roles maintained by pg-sync-roles begin with the prefix `_pgsr_`. Each name ends with a randomly generated unique identifier.
+
+
 ## Compatibility
 
 pg-sync-roles aims to be compatible with a wide range of Python and other dependencies:
 
 - Python >= 3.7.1 (tested on 3.7.1, 3.8.0, 3.9.0, 3.10.0, and 3.11.0)
 - psycopg2 >= 2.9.2 and Psycopg 3 >= 3.1.4
 - SQLAlchemy >= 1.4.24 (tested on 1.4.24 and 2.0.0)
```

