# Comparing `tmp/cuckoo_hasura-0.1.8.tar.gz` & `tmp/cuckoo_hasura-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuckoo_hasura-0.1.8.tar", last modified: Wed Apr 17 19:21:55 2024, max compression
+gzip compressed data, was "cuckoo_hasura-0.2.0.tar", last modified: Thu May  9 14:34:39 2024, max compression
```

## Comparing `cuckoo_hasura-0.1.8.tar` & `cuckoo_hasura-0.2.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:55.056230 cuckoo_hasura-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    29653 2024-04-17 19:21:55.056230 cuckoo_hasura-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27567 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:55.052230 cuckoo_hasura-0.1.8/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/codegen/default_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/codegen/example_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/codegen/graphql_2_python.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/codegen/model_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:55.052230 cuckoo_hasura-0.1.8/cuckoo/
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10610 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/binary_tree_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/finalizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/include.py
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/insert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:55.052230 cuckoo_hasura-0.1.8/cuckoo/models/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/models/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/models/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/models/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16454 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/root_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/cuckoo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:55.056230 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29653 2024-04-17 19:21:55.000000 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-17 19:21:55.000000 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 19:21:55.000000 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-17 19:21:55.000000 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-17 19:21:55.000000 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 19:21:55.000000 cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 19:21:55.056230 cuckoo_hasura-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 19:21:55.056230 cuckoo_hasura-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_include.py
--rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_insert.py
--rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)    35318 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_root_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-17 19:21:49.000000 cuckoo_hasura-0.1.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:34:39.678678 cuckoo_hasura-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    30978 2024-05-09 14:34:39.678678 cuckoo_hasura-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    28892 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:34:39.674678 cuckoo_hasura-0.2.0/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/codegen/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/codegen/example_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7218 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/codegen/graphql_2_python.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/codegen/model_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:34:39.674678 cuckoo_hasura-0.2.0/cuckoo/
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10610 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/binary_tree_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/cuckoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/finalizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/insert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:34:39.678678 cuckoo_hasura-0.2.0/cuckoo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/models/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/models/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16454 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9394 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/root_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/cuckoo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:34:39.678678 cuckoo_hasura-0.2.0/cuckoo_hasura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    30978 2024-05-09 14:34:39.000000 cuckoo_hasura-0.2.0/cuckoo_hasura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-09 14:34:39.000000 cuckoo_hasura-0.2.0/cuckoo_hasura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:34:39.000000 cuckoo_hasura-0.2.0/cuckoo_hasura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-09 14:34:39.000000 cuckoo_hasura-0.2.0/cuckoo_hasura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 14:34:39.000000 cuckoo_hasura-0.2.0/cuckoo_hasura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 14:34:39.000000 cuckoo_hasura-0.2.0/cuckoo_hasura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:34:39.678678 cuckoo_hasura-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:34:39.678678 cuckoo_hasura-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10331 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/tests/test_cuckoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/tests/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/tests/test_include.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11763 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/tests/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/tests/test_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35335 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/tests/test_root_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13633 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-05-09 14:34:33.000000 cuckoo_hasura-0.2.0/tests/test_utils.py
```

### Comparing `cuckoo_hasura-0.1.8/LICENSE` & `cuckoo_hasura-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/PKG-INFO` & `cuckoo_hasura-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuckoo-hasura
-Version: 0.1.8
+Version: 0.2.0
 Summary: An easy to use GraphQL query builder, optimized for Hasura.
 Author-email: Kenta Fried <kenta.fried@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kenta Fried
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -124,23 +124,73 @@
     2.1 Let the code generator query your Hasura schema API to generate the models you need. See the `codegen/README` for more info.
 
     2.2 Implement models manually by extending `HasuraTableModel` and save them in a schema-based folder structure. See the `tests/fixture/sample_models/public` folder for examples.
 
 ## Usage
 
 ### 1. Configuration
+Cuckoo requires:
+- an `httpx.Client` and/or `httpx.AsyncClient` for making synchronous/asynchronous requests
+- connection details to reach the Hasura server
 
-The first step for using Cuckoo is making sure we can connect to your Hasura instance. The easiest way to provide connection settings to Cuckoo is by simply defining 3 environment variables:
+## 1.1 Create an HTTPX Client cuckoo can use to make the request
+For anything but prototyping, it is best to register a client instance that Cuckoo will use for all queries and mutations. Please note that the client needs to be managed (AKA closed) inside the app where Cuckoo is used:
+```py
+from cuckoo import Cuckoo
+from httpx import Client
+
+if __name__ == "__main__":
+    client = Client()
+    Cuckoo.configure(session=client)
+
+    # using Cuckoo anywhere in the code base will now use the default client provided
+
+    client.close()
+```
+
+It is also possible to provide a client for a specific query:
+```py
+from cuckoo import Query
+from httpx import Client
+
+client = Client()
+authors = Query(Authors, session=client).many(..).returning()
+```
+
+## 1.1 Provide connection settings to your Hasura instance
+The easiest way to provide connection settings to Cuckoo is by simply defining 3 environment variables:
 ```sh
 HASURA_URL=http://hasura:8080/v1/graphql
 HASURA_ROLE=admin
 HASURA_ADMIN_SECRET=hasura
 ```
 
-Alternatively, you can provide the connection settings when instantiating your query or mutation. This comes in handy, if you need to connect to different Hasura instances within the same project:
+If you prefer, you can also set these details programatically:
+```py
+from cuckoo import Cuckoo
+
+if __name__ == "__main__":
+    client = Client()
+    Cuckoo.configure(
+        session=client,
+        config={
+            "url": "http://hasura:8080/v1/graphql"
+            "headers": {
+                "X-Hasura-Admin-Secret": "admin",
+                "X-Hasura-Role": "hasura",
+            }
+        }
+    )
+
+    # Cuckoo is ready!
+
+    client.close()
+```
+
+Finally, you can provide the connection settings when instantiating your query or mutation. This comes in handy, if you need to connect to different Hasura instances within the same project:
 ```py
 Query(Author, config={
     "url": "http://hasura:8080/v1/graphql"
     "headers": {
         "X-Hasura-Admin-Secret": "admin",
         "X-Hasura-Role": "hasura",
     }
```

### Comparing `cuckoo_hasura-0.1.8/README.md` & `cuckoo_hasura-0.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,23 +80,73 @@
     2.1 Let the code generator query your Hasura schema API to generate the models you need. See the `codegen/README` for more info.
 
     2.2 Implement models manually by extending `HasuraTableModel` and save them in a schema-based folder structure. See the `tests/fixture/sample_models/public` folder for examples.
 
 ## Usage
 
 ### 1. Configuration
+Cuckoo requires:
+- an `httpx.Client` and/or `httpx.AsyncClient` for making synchronous/asynchronous requests
+- connection details to reach the Hasura server
 
-The first step for using Cuckoo is making sure we can connect to your Hasura instance. The easiest way to provide connection settings to Cuckoo is by simply defining 3 environment variables:
+## 1.1 Create an HTTPX Client cuckoo can use to make the request
+For anything but prototyping, it is best to register a client instance that Cuckoo will use for all queries and mutations. Please note that the client needs to be managed (AKA closed) inside the app where Cuckoo is used:
+```py
+from cuckoo import Cuckoo
+from httpx import Client
+
+if __name__ == "__main__":
+    client = Client()
+    Cuckoo.configure(session=client)
+
+    # using Cuckoo anywhere in the code base will now use the default client provided
+
+    client.close()
+```
+
+It is also possible to provide a client for a specific query:
+```py
+from cuckoo import Query
+from httpx import Client
+
+client = Client()
+authors = Query(Authors, session=client).many(..).returning()
+```
+
+## 1.1 Provide connection settings to your Hasura instance
+The easiest way to provide connection settings to Cuckoo is by simply defining 3 environment variables:
 ```sh
 HASURA_URL=http://hasura:8080/v1/graphql
 HASURA_ROLE=admin
 HASURA_ADMIN_SECRET=hasura
 ```
 
-Alternatively, you can provide the connection settings when instantiating your query or mutation. This comes in handy, if you need to connect to different Hasura instances within the same project:
+If you prefer, you can also set these details programatically:
+```py
+from cuckoo import Cuckoo
+
+if __name__ == "__main__":
+    client = Client()
+    Cuckoo.configure(
+        session=client,
+        config={
+            "url": "http://hasura:8080/v1/graphql"
+            "headers": {
+                "X-Hasura-Admin-Secret": "admin",
+                "X-Hasura-Role": "hasura",
+            }
+        }
+    )
+
+    # Cuckoo is ready!
+
+    client.close()
+```
+
+Finally, you can provide the connection settings when instantiating your query or mutation. This comes in handy, if you need to connect to different Hasura instances within the same project:
 ```py
 Query(Author, config={
     "url": "http://hasura:8080/v1/graphql"
     "headers": {
         "X-Hasura-Admin-Secret": "admin",
         "X-Hasura-Role": "hasura",
     }
```

### Comparing `cuckoo_hasura-0.1.8/codegen/default_config.py` & `cuckoo_hasura-0.2.0/codegen/default_config.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/codegen/example_config.py` & `cuckoo_hasura-0.2.0/codegen/example_config.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/codegen/graphql_2_python.py` & `cuckoo_hasura-0.2.0/codegen/graphql_2_python.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/codegen/model_module.py` & `cuckoo_hasura-0.2.0/codegen/model_module.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/binary_tree_node.py` & `cuckoo_hasura-0.2.0/cuckoo/binary_tree_node.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/constants.py` & `cuckoo_hasura-0.2.0/cuckoo/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,41 +2,56 @@
 
 import os
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Literal,
+    Optional,
     Type,
     TypedDict,
     Union,
 )
 
-from tenacity import stop_after_attempt, wait_random_exponential
+from httpx import AsyncClient, Client
+from tenacity import (
+    retry_if_not_exception_type,
+    stop_after_attempt,
+    wait_random_exponential,
+)
 from typing_extensions import NotRequired, TypeAlias
 
+from cuckoo.errors import HasuraServerError
+
 if TYPE_CHECKING:
     from tenacity import RetryCallState, RetryError
     from tenacity.retry import RetryBaseT
     from tenacity.stop import StopBaseT
     from tenacity.wait import WaitBaseT
 
 HASURA_PORT = int(os.environ.get("HASURA_PORT", "8080"))
 HASURA_HEALTH_URL = os.environ.get("HASURA_HEALTH_URL", "")
-HASURA_URL = os.environ["HASURA_URL"]
-HASURA_ADMIN_SECRET = os.environ["HASURA_ADMIN_SECRET"]
-HASURA_ROLE = os.environ["HASURA_ROLE"]
+HASURA_URL = os.environ.get("HASURA_URL")
+HASURA_ADMIN_SECRET = os.environ.get("HASURA_ADMIN_SECRET")
+HASURA_ROLE = os.environ.get("HASURA_ROLE")
 
 DEFAULT_COLUMNS = ["uuid"]
 DEFAULT_COLUMNS_INVERTED = []
 
 
-class HasuraConfig(TypedDict):
-    url: str
-    headers: dict[str, str]
+class GlobalCuckooConfig(TypedDict):
+    cuckoo_config: CuckooConfig
+    session: Optional[Client]
+    session_async: Optional[AsyncClient]
+
+
+class CuckooConfig(TypedDict):
+    url: NotRequired[str]
+    headers: NotRequired[dict[str, str]]
+    retry: NotRequired[RetryConfig]
 
 
 class RetryConfig(TypedDict):
     sleep: NotRequired[Callable[[Union[int, float]], None]]
     stop: NotRequired[StopBaseT]
     wait: NotRequired[WaitBaseT]
     retry: NotRequired[RetryBaseT]
@@ -44,31 +59,27 @@
     after: NotRequired[Callable[[RetryCallState], None]]
     before_sleep: NotRequired[Callable[[RetryCallState], None]]
     reraise: NotRequired[bool]
     retry_error_cls: NotRequired[Type[RetryError]]
     retry_error_callback: NotRequired[Callable[[RetryCallState], Any]]
 
 
-class CuckooConfig(HasuraConfig):
-    retry: RetryConfig
-
-
 HASURA_HEADERS = {
     "X-Hasura-Admin-Secret": HASURA_ADMIN_SECRET,
     "X-Hasura-Role": HASURA_ROLE,
 }
-
-HASURA_DEFAULT_CONFIG: HasuraConfig = {
-    "url": HASURA_URL,
-    "headers": HASURA_HEADERS,
-}
-
 RETRY_DEFAULT_CONFIG: RetryConfig = {
     "wait": wait_random_exponential(multiplier=1, max=60),
     "stop": stop_after_attempt(5),
+    "retry": retry_if_not_exception_type(HasuraServerError),
+}
+HASURA_DEFAULT_CONFIG: CuckooConfig = {
+    "url": HASURA_URL,
+    "headers": HASURA_HEADERS,
+    "retry": RETRY_DEFAULT_CONFIG,
 }
 
 WHERE: TypeAlias = dict[str, Any]
 ORDER_DIRECTION: TypeAlias = Union[Literal["asc"], Literal["desc"]]
 ORDER_BY: TypeAlias = dict[str, Union[ORDER_DIRECTION, "ORDER_BY"]]
```

### Comparing `cuckoo_hasura-0.1.8/cuckoo/delete.py` & `cuckoo_hasura-0.2.0/cuckoo/delete.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/encoders.py` & `cuckoo_hasura-0.2.0/cuckoo/encoders.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/finalizers.py` & `cuckoo_hasura-0.2.0/cuckoo/finalizers.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/include.py` & `cuckoo_hasura-0.2.0/cuckoo/include.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/insert.py` & `cuckoo_hasura-0.2.0/cuckoo/insert.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/models/__init__.py` & `cuckoo_hasura-0.2.0/cuckoo/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/models/builtins.py` & `cuckoo_hasura-0.2.0/cuckoo/models/builtins.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/models/common.py` & `cuckoo_hasura-0.2.0/cuckoo/models/common.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/models/providers.py` & `cuckoo_hasura-0.2.0/cuckoo/models/providers.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/mutation.py` & `cuckoo_hasura-0.2.0/cuckoo/mutation.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/query.py` & `cuckoo_hasura-0.2.0/cuckoo/query.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/root_node.py` & `cuckoo_hasura-0.2.0/cuckoo/root_node.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,71 +10,96 @@
     Optional,
     Union,
 )
 
 import orjson
 from httpx import AsyncClient, Client, Response
 from pydantic import BaseModel
-from tenacity import AsyncRetrying, RetryError, Retrying
+from tenacity import AsyncRetrying, Retrying
 
-from cuckoo.binary_tree_node import BinaryTreeNode
-from cuckoo.constants import HASURA_DEFAULT_CONFIG, RETRY_DEFAULT_CONFIG, CuckooConfig
-from cuckoo.encoders import jsonable_encoder
-from cuckoo.errors import HasuraClientError, HasuraServerError
-from cuckoo.models import TMODEL
-from cuckoo.utils import in_brackets, to_compact_str, to_truncated_str
+from .binary_tree_node import BinaryTreeNode
+from .constants import CuckooConfig
+from .cuckoo import Cuckoo
+from .encoders import jsonable_encoder
+from .errors import HasuraClientError, HasuraServerError
+from .models import TMODEL
+from .utils import in_brackets, to_compact_str, to_truncated_str
 
 
 class RootNode(BinaryTreeNode[TMODEL]):
     VAR_NAME_BASE = "var"
 
     def __init__(
         self,
         config: Optional[CuckooConfig] = None,
         session: Optional[Client] = None,
         session_async: Optional[AsyncClient] = None,
         logger: Optional[Logger] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
-        self._config: CuckooConfig = {
-            **HASURA_DEFAULT_CONFIG,  # type: ignore
-            "retry": RETRY_DEFAULT_CONFIG,
-            **(config if config else {}),
-        }
+
+        self._config = Cuckoo.cuckoo_config(*([config] if config is not None else []))
+        self._session_override = session
+        self._session_override_async = session_async
         self._logger = logger
         self._var_name_counter: int = 0
         self._response: Optional[Response] = None
         self._response_data: Optional[dict[str, Any]] = None
         self._is_batch = False
 
-        self._close_session = False
-        if session is None:
-            self._close_session = True
-            self._session = Client(timeout=None)
-        else:
-            self._session = session
-
-        self._close_session_async = False
-        if session_async is None:
-            self._close_session_async = True
-            self._session_async = AsyncClient(timeout=None)
-        else:
-            self._session_async = session_async
-
     def __str__(self):
         outer_args = self._get_all_outer_args()
         return f"""
             {self._fragments.query_name}{
                 in_brackets(', '.join(outer_args), condition=bool(outer_args))
             } {{
                 {" ".join(str(child) for child in self._children)}
             }}
         """
 
+    @property
+    def session(self):
+        try:
+            return next(
+                effective_session
+                for effective_session in [
+                    self._session_override,  # prefer override
+                    Cuckoo.session(),  # default to global
+                ]
+                if effective_session is not None
+            )
+        except StopIteration:
+            raise HasuraClientError(
+                "No session provided. Use `Cuckoo.configure(session=my_session)` for "
+                "setting up a global session that all cuckoo calls will use by "
+                "default. Use the `session=my_session` argument in the Query/Mutation "
+                "constructor to override default."
+            )
+
+    @property
+    def session_async(self):
+        try:
+            return next(
+                effective_session
+                for effective_session in [
+                    self._session_override_async,  # prefer override
+                    Cuckoo.session_async(),  # default to global
+                ]
+                if effective_session is not None
+            )
+        except StopIteration:
+            raise HasuraClientError(
+                "No async session provided. Use "
+                "`Cuckoo.configure(session_async=my_session)` for setting up a global "
+                "session that all cuckoo calls will use by default. Use the "
+                "`session_async=my_session` argument in the Query/Mutation "
+                "constructor to override default."
+            )
+
     def _get_response(
         self,
         query_alias: str,
         key: Optional[str] = None,
     ) -> Union[dict, list, int]:
         if self._response_data is None:
             raise HasuraClientError(
@@ -122,70 +147,67 @@
             self._response_data = response_json["data"]
         else:
             raise NotImplementedError(
                 "Response did not contain any errors nor data. "
                 f"Response={self._response.text}."
             )
 
-    def _build_request(self):
+    def _build_request(self, session: Union[Client, AsyncClient]):
+        url = self._config["url"]
+        if url is None:
+            raise HasuraClientError(
+                "Missing Hasura server URL. Choices: "
+                "\n - Set the `HASURA_URL` environment variable"
+                '\n - Globally configure cuckoo:`Cuckoo.configure({"url": "http://.."})`'
+                '\n - Configure a query/mutation:`Query(config={"url": "http://.."})`'
+            )
+
         query = to_compact_str(str(self))
         variables = self._get_all_variables()
         json = {"query": query}
         if variables:
             json["variables"] = RootNode._jsonify_variables(variables)
 
         if self._logger:
             self._logger.debug(
                 f"Request created. {query=}, variables={to_truncated_str(variables)}."
             )
 
-        return self._session.build_request(
+        return session.build_request(
             method="POST",
-            url=self._config["url"],
+            url=url,
             headers=self._config["headers"],
             json=json,
         )
 
     def _execute(self, stream=False):
-        request = self._build_request()
+        request = self._build_request(self.session)
         if self._logger:
             if stream:
                 self._logger.debug("Dispatching http streaming request.")
             else:
                 self._logger.debug("Dispatching http request.")
 
-        try:
-            for attempt in Retrying(**self._config["retry"]):
-                with attempt:
-                    self._response = self._session.send(request=request, stream=stream)
-                    self._response.raise_for_status()
-                    if not stream:
-                        self._process_response()
-        except RetryError as err:
-            raise HasuraServerError(repr(err))
-        finally:
-            if self._close_session and self._session is not None:
-                self._session.close()
+        for attempt in Retrying(**self._config["retry"]):
+            with attempt:
+                self._response = self.session.send(request=request, stream=stream)
+                self._response.raise_for_status()
+                if not stream:
+                    self._process_response()
 
     async def _execute_async(self):
-        request = self._build_request()
+        request = self._build_request(self.session_async)
         if self._logger:
             self._logger.debug("Dispatching asynchronous http request.")
 
-        try:
-            async for attempt in AsyncRetrying(**self._config["retry"]):
-                with attempt:
-                    self._response = await self._session_async.send(request=request)
-                    self._response.raise_for_status()
-                    self._process_response()
-        except RetryError as err:
-            raise HasuraServerError(repr(err))
-        finally:
-            if self._close_session_async and self._session_async is not None:
-                await self._session_async.aclose()
+        async for attempt in AsyncRetrying(**self._config["retry"]):
+            with attempt:
+                self._response = await self.session_async.send(request=request)
+                self._response.raise_for_status()
+                self._process_response()
 
     @staticmethod
     def _jsonify_variables(variables):
         return orjson.loads(orjson.dumps(variables, default=RootNode._orjson_default))
 
     def _get_all_variables(self):
         return {
```

### Comparing `cuckoo_hasura-0.1.8/cuckoo/update.py` & `cuckoo_hasura-0.2.0/cuckoo/update.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo/utils.py` & `cuckoo_hasura-0.2.0/cuckoo/utils.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/PKG-INFO` & `cuckoo_hasura-0.2.0/cuckoo_hasura.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cuckoo-hasura
-Version: 0.1.8
+Version: 0.2.0
 Summary: An easy to use GraphQL query builder, optimized for Hasura.
 Author-email: Kenta Fried <kenta.fried@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Kenta Fried
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -124,23 +124,73 @@
     2.1 Let the code generator query your Hasura schema API to generate the models you need. See the `codegen/README` for more info.
 
     2.2 Implement models manually by extending `HasuraTableModel` and save them in a schema-based folder structure. See the `tests/fixture/sample_models/public` folder for examples.
 
 ## Usage
 
 ### 1. Configuration
+Cuckoo requires:
+- an `httpx.Client` and/or `httpx.AsyncClient` for making synchronous/asynchronous requests
+- connection details to reach the Hasura server
 
-The first step for using Cuckoo is making sure we can connect to your Hasura instance. The easiest way to provide connection settings to Cuckoo is by simply defining 3 environment variables:
+## 1.1 Create an HTTPX Client cuckoo can use to make the request
+For anything but prototyping, it is best to register a client instance that Cuckoo will use for all queries and mutations. Please note that the client needs to be managed (AKA closed) inside the app where Cuckoo is used:
+```py
+from cuckoo import Cuckoo
+from httpx import Client
+
+if __name__ == "__main__":
+    client = Client()
+    Cuckoo.configure(session=client)
+
+    # using Cuckoo anywhere in the code base will now use the default client provided
+
+    client.close()
+```
+
+It is also possible to provide a client for a specific query:
+```py
+from cuckoo import Query
+from httpx import Client
+
+client = Client()
+authors = Query(Authors, session=client).many(..).returning()
+```
+
+## 1.1 Provide connection settings to your Hasura instance
+The easiest way to provide connection settings to Cuckoo is by simply defining 3 environment variables:
 ```sh
 HASURA_URL=http://hasura:8080/v1/graphql
 HASURA_ROLE=admin
 HASURA_ADMIN_SECRET=hasura
 ```
 
-Alternatively, you can provide the connection settings when instantiating your query or mutation. This comes in handy, if you need to connect to different Hasura instances within the same project:
+If you prefer, you can also set these details programatically:
+```py
+from cuckoo import Cuckoo
+
+if __name__ == "__main__":
+    client = Client()
+    Cuckoo.configure(
+        session=client,
+        config={
+            "url": "http://hasura:8080/v1/graphql"
+            "headers": {
+                "X-Hasura-Admin-Secret": "admin",
+                "X-Hasura-Role": "hasura",
+            }
+        }
+    )
+
+    # Cuckoo is ready!
+
+    client.close()
+```
+
+Finally, you can provide the connection settings when instantiating your query or mutation. This comes in handy, if you need to connect to different Hasura instances within the same project:
 ```py
 Query(Author, config={
     "url": "http://hasura:8080/v1/graphql"
     "headers": {
         "X-Hasura-Admin-Secret": "admin",
         "X-Hasura-Role": "hasura",
     }
```

### Comparing `cuckoo_hasura-0.1.8/cuckoo_hasura.egg-info/SOURCES.txt` & `cuckoo_hasura-0.2.0/cuckoo_hasura.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 codegen/default_config.py
 codegen/example_config.py
 codegen/graphql_2_python.py
 codegen/model_module.py
 cuckoo/__init__.py
 cuckoo/binary_tree_node.py
 cuckoo/constants.py
+cuckoo/cuckoo.py
 cuckoo/delete.py
 cuckoo/encoders.py
 cuckoo/errors.py
 cuckoo/finalizers.py
 cuckoo/include.py
 cuckoo/insert.py
 cuckoo/mutation.py
@@ -26,14 +27,15 @@
 cuckoo/models/providers.py
 cuckoo_hasura.egg-info/PKG-INFO
 cuckoo_hasura.egg-info/SOURCES.txt
 cuckoo_hasura.egg-info/dependency_links.txt
 cuckoo_hasura.egg-info/entry_points.txt
 cuckoo_hasura.egg-info/requires.txt
 cuckoo_hasura.egg-info/top_level.txt
+tests/test_cuckoo.py
 tests/test_delete.py
 tests/test_include.py
 tests/test_insert.py
 tests/test_mutation.py
 tests/test_query.py
 tests/test_root_node.py
 tests/test_update.py
```

### Comparing `cuckoo_hasura-0.1.8/pyproject.toml` & `cuckoo_hasura-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cuckoo-hasura"
-version = "0.1.8"
+version = "0.2.0"
 description = "An easy to use GraphQL query builder, optimized for Hasura."
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 authors = [{ name = "Kenta Fried", email = "kenta.fried@gmail.com" }]
 keywords = []
 classifiers = [
```

### Comparing `cuckoo_hasura-0.1.8/tests/test_delete.py` & `cuckoo_hasura-0.2.0/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/tests/test_include.py` & `cuckoo_hasura-0.2.0/tests/test_include.py`

 * *Files 4% similar despite different names*

```diff
@@ -292,19 +292,24 @@
         actual = get_actual(author.articles_aggregate.aggregate)
 
         assert actual == expected
 
 
 def test_raises_error_if_instance_is_used_more_than_once(
     persisted_author: Author,
+    session: Client,
 ):
     columns = [Include(Article).many().returning()]
-    Query(Author).one_by_pk(uuid=persisted_author.uuid).returning(columns)
+    Query(Author, session=session).one_by_pk(uuid=persisted_author.uuid).returning(
+        columns
+    )
     with raises(ValueError) as error:
-        Query(Author).one_by_pk(uuid=persisted_author.uuid).returning(columns)
+        Query(Author, session=session).one_by_pk(uuid=persisted_author.uuid).returning(
+            columns
+        )
     assert (
         "Found an instance `Include(Article)` that was already used in an executed query"
     ) in str(error)
 
 
 @fixture(scope="module")
 def persisted_author(user_uuid: UUID, session: Client):
```

### Comparing `cuckoo_hasura-0.1.8/tests/test_insert.py` & `cuckoo_hasura-0.2.0/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/tests/test_mutation.py` & `cuckoo_hasura-0.2.0/tests/test_mutation.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/tests/test_query.py` & `cuckoo_hasura-0.2.0/tests/test_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
                     * CONCURRENCY
                 )
             )
 
         print("START ", datetime.now().isoformat())
         count = 0
         # for author in await Query(Author).many(where={}).returning_async():
-        for author in Query(Author).many(where={}).yielding():
+        for author in Query(Author, session=session).many(where={}).yielding():
             # assert isinstance(author.uuid, UUID)
             count += 1
         print("END ", count, datetime.now().isoformat())
 
 
 @mark.asyncio(scope="session")
 class TestAggregate:
```

### Comparing `cuckoo_hasura-0.1.8/tests/test_root_node.py` & `cuckoo_hasura-0.2.0/tests/test_root_node.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 from statistics import mean
 from typing import Any, Callable, Type
 from unittest.mock import MagicMock, patch
 from uuid import uuid4
 
 from httpx import AsyncClient, Client
 from pytest import fixture, mark, raises
-from tenacity import stop_after_attempt
+from tenacity import RetryError, stop_after_attempt
 
-from cuckoo import Query, root_node
-from cuckoo.errors import HasuraServerError
+from cuckoo import Query
 from cuckoo.include import Include
 from tests.fixture.base_fixture import VARIABLE_SEQUENCES, VARIABLE_TYPES
 from tests.fixture.common_utils import generate_author_data
 from tests.fixture.sample_models.public import Article, Author
 
 
 class TestJsonifyVariables:
@@ -97,114 +96,80 @@
             Query._jsonify_variables(author_data)
             seconds_elapsed.append(time.time() - start_time)
 
         assert limit_seconds > mean(seconds_elapsed)
 
 
 class TestIsRoot:
-    def test_simple_query_is_root_node(self):
-        query = Query(Author)
+    def test_simple_query_is_root_node(self, session: Client):
+        query = Query(Author, session=session)
 
         query.many(where={}).returning()
 
         assert query._is_root is True
         assert query._root == query
         assert query._parent == query
 
-    def test_included_subquery_is_not_root_node(self):
-        query = Query(Author)
+    def test_included_subquery_is_not_root_node(self, session: Client):
+        query = Query(Author, session=session)
         include = Include(Article)
 
         query.many(where={}).returning(columns=[include.many().returning()])
 
         assert include._is_root is False
         assert include._root != include
         assert include._parent != include
 
-    def test_batch_creates_root_node(self):
-        with Query.batch() as BatchQuery:
+    def test_batch_creates_root_node(self, session: Client):
+        with Query.batch(session=session) as BatchQuery:
             batch_query = BatchQuery(Author)
             batch_query.many(where={}).yielding()
         root = batch_query._parent
 
         assert root._is_root is True
         assert root._root == root
         assert root._parent == root
 
-    def test_batch_query_is_not_root_node(self):
-        with Query.batch() as BatchQuery:
+    def test_batch_query_is_not_root_node(self, session: Client):
+        with Query.batch(session=session) as BatchQuery:
             batch_query = BatchQuery(Author)
             batch_query.many(where={}).yielding()
 
         assert batch_query._is_root is False
         assert batch_query._root != batch_query
         assert batch_query._parent != batch_query
 
 
 class TestExecute:
     def test_default_config_stops_retrying_after_5_attempts(
         self,
         failing_session: MagicMock,
     ):
-        with raises(HasuraServerError):
+        with raises(RetryError):
             Query(Author, session=failing_session).many(where={}).returning()
 
         assert failing_session.send.call_count == 5
 
     def test_retry_config_can_be_changed(
         self,
         failing_session: MagicMock,
     ):
-        with raises(HasuraServerError):
+        with raises(RetryError):
             Query(
                 Author,
                 session=failing_session,
                 config={
                     "retry": {
                         "stop": stop_after_attempt(3),
                     }
                 },
             ).many(where={}).returning()
 
         assert failing_session.send.call_count == 3
 
-    def test_default_session_gets_closed_for_successful_query(
-        self,
-        default_session_close: MagicMock,
-    ):
-        Query(Author).many(where={}).returning()
-
-        assert default_session_close.call_count == 1
-
-    def test_default_session_gets_closed_for_unsuccessful_query(
-        self,
-        failing_default_session: MagicMock,
-    ):
-        with raises(HasuraServerError):
-            Query(Author).many(where={}).returning()
-
-        failing_default_session.close.assert_called_once()
-
-    def test_non_default_session_does_not_get_closed_for_successful_query(
-        self,
-        session: Client,
-    ):
-        Query(Author, session=session).many(where={}).returning()
-
-        assert not session.is_closed
-
-    def test_non_default_session_does_not_get_closed_for_unsuccessful_query(
-        self,
-        failing_session: MagicMock,
-    ):
-        with raises(HasuraServerError):
-            Query(Author, session=failing_session).many(where={}).returning()
-
-        failing_session.close.assert_not_called()
-
     @fixture
     def failing_session(self):
         mock = MagicMock(spec=Client)
         mock.send.side_effect = [
             Exception("1"),
             Exception("2"),
             Exception("3"),
@@ -215,44 +180,35 @@
 
     @fixture
     def failing_default_session(self, failing_session: MagicMock):
         with patch("cuckoo.root_node.Client", spec=Type[Client]) as mock:
             mock.return_value = failing_session
             yield failing_session
 
-    @fixture
-    def default_session_close(self):
-        with patch.object(
-            root_node.Client,
-            "close",
-            wraps=root_node.Client().close,
-        ) as spy:
-            yield spy
-
 
 @mark.asyncio(scope="session")
 class TestExecuteAsync:
     async def test_default_config_stops_retrying_after_5_attempts(
         self,
         failing_session: MagicMock,
     ):
-        with raises(HasuraServerError):
+        with raises(RetryError):
             await (
                 Query(Author, session_async=failing_session)
                 .many(where={})
                 .returning_async()
             )
 
         assert failing_session.send.call_count == 5
 
     async def test_retry_config_can_be_changed(
         self,
         failing_session: MagicMock,
     ):
-        with raises(HasuraServerError):
+        with raises(RetryError):
             await (
                 Query(
                     Author,
                     session_async=failing_session,
                     config={
                         "retry": {
                             "stop": stop_after_attempt(3),
@@ -261,54 +217,14 @@
                 )
                 .many(where={})
                 .returning_async()
             )
 
         assert failing_session.send.call_count == 3
 
-    async def test_default_session_gets_closed_for_successful_query(
-        self,
-        default_session_close: MagicMock,
-    ):
-        await Query(Author).many(where={}).returning_async()
-
-        assert default_session_close.call_count == 1
-
-    async def test_default_session_gets_closed_for_unsuccessful_query(
-        self,
-        failing_default_session: MagicMock,
-    ):
-        with raises(HasuraServerError):
-            await Query(Author).many(where={}).returning_async()
-
-        failing_default_session.aclose.assert_called_once()
-
-    async def test_non_default_session_does_not_get_closed_for_successful_query(
-        self,
-        session_async: AsyncClient,
-    ):
-        await (
-            Query(Author, session_async=session_async).many(where={}).returning_async()
-        )
-
-        assert not session_async.is_closed
-
-    async def test_non_default_session_does_not_get_closed_for_unsuccessful_query(
-        self,
-        failing_session: MagicMock,
-    ):
-        with raises(HasuraServerError):
-            await (
-                Query(Author, session_async=failing_session)
-                .many(where={})
-                .returning_async()
-            )
-
-        failing_session.aclose.assert_not_called()
-
     @fixture
     def failing_session(self):
         mock = MagicMock(spec=AsyncClient)
         mock.send.side_effect = [
             Exception("1"),
             Exception("2"),
             Exception("3"),
@@ -318,16 +234,7 @@
         return mock
 
     @fixture
     def failing_default_session(self, failing_session: MagicMock):
         with patch("cuckoo.root_node.AsyncClient", spec=Type[AsyncClient]) as mock:
             mock.return_value = failing_session
             yield failing_session
-
-    @fixture
-    def default_session_close(self):
-        with patch.object(
-            root_node.AsyncClient,
-            "aclose",
-            wraps=root_node.AsyncClient().aclose,
-        ) as spy:
-            yield spy
```

### Comparing `cuckoo_hasura-0.1.8/tests/test_update.py` & `cuckoo_hasura-0.2.0/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `cuckoo_hasura-0.1.8/tests/test_utils.py` & `cuckoo_hasura-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

