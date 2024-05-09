# Comparing `tmp/typedmongo-1.4.0.tar.gz` & `tmp/typedmongo-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedmongo-1.4.0.tar", last modified: Tue May  7 09:28:45 2024, max compression
+gzip compressed data, was "typedmongo-1.5.0.tar", last modified: Wed May  8 03:20:53 2024, max compression
```

## Comparing `typedmongo-1.4.0.tar` & `typedmongo-1.5.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-05-07 09:28:32.689580 typedmongo-1.4.0/LICENSE
--rw-r--r--   0        0        0     3808 2024-05-07 09:28:32.689580 typedmongo-1.4.0/README.md
--rw-r--r--   0        0        0     1441 2024-05-07 09:28:45.517577 typedmongo-1.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/asyncio/__init__.py
--rw-r--r--   0        0        0     5575 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/asyncio/test_client.py
--rw-r--r--   0        0        0     4229 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/asyncio/test_table.py
--rw-r--r--   0        0        0     1218 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/sync.py
--rw-r--r--   0        0        0     5335 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/test_client.py
--rw-r--r--   0        0        0     3031 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/test_expressions.py
--rw-r--r--   0        0        0      582 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/test_marshamallow.py
--rw-r--r--   0        0        0     4221 2024-05-07 09:28:32.689580 typedmongo-1.4.0/tests/test_table.py
--rw-r--r--   0        0        0      811 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/__init__.py
--rw-r--r--   0        0        0      811 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/asyncio/__init__.py
--rw-r--r--   0        0        0    10328 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/asyncio/client.py
--rw-r--r--   0        0        0     9999 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/asyncio/fields.py
--rw-r--r--   0        0        0     8494 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/asyncio/table.py
--rw-r--r--   0        0        0    10122 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/client.py
--rw-r--r--   0        0        0      163 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/exceptions.py
--rw-r--r--   0        0        0     5468 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/expressions.py
--rw-r--r--   0        0        0     9999 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/fields.py
--rw-r--r--   0        0        0      849 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/marshamallow.py
--rw-r--r--   0        0        0     1325 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/sync.py
--rw-r--r--   0        0        0     8494 2024-05-07 09:28:32.689580 typedmongo-1.4.0/typedmongo/table.py
--rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 typedmongo-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-08 03:20:40.907615 typedmongo-1.5.0/LICENSE
+-rw-r--r--   0        0        0     3808 2024-05-08 03:20:40.907615 typedmongo-1.5.0/README.md
+-rw-r--r--   0        0        0     1441 2024-05-08 03:20:53.779699 typedmongo-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-08 03:20:40.907615 typedmongo-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 03:20:40.907615 typedmongo-1.5.0/tests/asyncio/__init__.py
+-rw-r--r--   0        0        0     6050 2024-05-08 03:20:40.907615 typedmongo-1.5.0/tests/asyncio/test_client.py
+-rw-r--r--   0        0        0     4229 2024-05-08 03:20:40.907615 typedmongo-1.5.0/tests/asyncio/test_table.py
+-rw-r--r--   0        0        0     1218 2024-05-08 03:20:40.907615 typedmongo-1.5.0/tests/sync.py
+-rw-r--r--   0        0        0     5798 2024-05-08 03:20:40.907615 typedmongo-1.5.0/tests/test_client.py
+-rw-r--r--   0        0        0     3031 2024-05-08 03:20:40.907615 typedmongo-1.5.0/tests/test_expressions.py
+-rw-r--r--   0        0        0      582 2024-05-08 03:20:40.907615 typedmongo-1.5.0/tests/test_marshamallow.py
+-rw-r--r--   0        0        0     4221 2024-05-08 03:20:40.907615 typedmongo-1.5.0/tests/test_table.py
+-rw-r--r--   0        0        0      926 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/__init__.py
+-rw-r--r--   0        0        0      926 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/asyncio/__init__.py
+-rw-r--r--   0        0        0    10328 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/asyncio/client.py
+-rw-r--r--   0        0        0     9999 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/asyncio/fields.py
+-rw-r--r--   0        0        0     8494 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/asyncio/table.py
+-rw-r--r--   0        0        0    10122 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/client.py
+-rw-r--r--   0        0        0      163 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/exceptions.py
+-rw-r--r--   0        0        0     5468 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/expressions.py
+-rw-r--r--   0        0        0     9999 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/fields.py
+-rw-r--r--   0        0        0      849 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/marshamallow.py
+-rw-r--r--   0        0        0     1384 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/shortcuts.py
+-rw-r--r--   0        0        0     1325 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/sync.py
+-rw-r--r--   0        0        0     8494 2024-05-08 03:20:40.907615 typedmongo-1.5.0/typedmongo/table.py
+-rw-r--r--   0        0        0     4181 1970-01-01 00:00:00.000000 typedmongo-1.5.0/PKG-INFO
```

### Comparing `typedmongo-1.4.0/LICENSE` & `typedmongo-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/README.md` & `typedmongo-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/pyproject.toml` & `typedmongo-1.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typedmongo"
-version = "1.4.0"
+version = "1.5.0"
 description = "A production-ready modern Python MongoDB ODM"
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "pymongo>=4.6.3",
     "motor>=3.4.0",
```

### Comparing `typedmongo-1.4.0/tests/asyncio/test_client.py` & `typedmongo-1.5.0/tests/asyncio/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -187,7 +187,24 @@
         [User.name],
         {User.name: True, User._id: False},
     ],
 )
 async def test_projection(documents_id, projection):
     user = await User.objects.find_one(User.age == 18, projection=projection)
     assert user is not None
+
+
+@pytest.mark.parametrize(
+    "shortcut",
+    [
+        mongo.Contains("be"),
+        mongo.Contains("bE", case_sensitive=False),
+        mongo.StartsWith("A"),
+        mongo.StartsWith("a", case_sensitive=False),
+        mongo.EndsWith("r"),
+        mongo.EndsWith("R", case_sensitive=False),
+    ],
+)
+async def test_shortcut(documents_id, shortcut):
+    user = await User.objects.find_one(User.name == shortcut)
+    assert user is not None
+    assert user.name == "Aber"
```

### Comparing `typedmongo-1.4.0/tests/asyncio/test_table.py` & `typedmongo-1.5.0/tests/asyncio/test_table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/tests/sync.py` & `typedmongo-1.5.0/tests/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/tests/test_client.py` & `typedmongo-1.5.0/tests/test_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -187,7 +187,24 @@
         [User.name],
         {User.name: True, User._id: False},
     ],
 )
 def test_projection(documents_id, projection):
     user = User.objects.find_one(User.age == 18, projection=projection)
     assert user is not None
+
+
+@pytest.mark.parametrize(
+    "shortcut",
+    [
+        mongo.Contains("be"),
+        mongo.Contains("bE", case_sensitive=False),
+        mongo.StartsWith("A"),
+        mongo.StartsWith("a", case_sensitive=False),
+        mongo.EndsWith("r"),
+        mongo.EndsWith("R", case_sensitive=False),
+    ],
+)
+def test_shortcut(documents_id, shortcut):
+    user = User.objects.find_one(User.name == shortcut)
+    assert user is not None
+    assert user.name == "Aber"
```

### Comparing `typedmongo-1.4.0/tests/test_expressions.py` & `typedmongo-1.5.0/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/tests/test_marshamallow.py` & `typedmongo-1.5.0/tests/test_marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/tests/test_table.py` & `typedmongo-1.5.0/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/typedmongo/__init__.py` & `typedmongo-1.5.0/typedmongo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typedmongo.shortcuts import Contains, EndsWith, StartsWith
+
 from .client import (
     DeleteMany,
     DeleteOne,
     InsertOne,
     ReplaceOne,
     UpdateMany,
     UpdateOne,
@@ -19,14 +21,17 @@
     ListField,
     ObjectIdField,
     StringField,
 )
 from .table import Index, MongoTable, Table
 
 __all__ = [
+    "Contains",
+    "StartsWith",
+    "EndsWith",
     "DeleteMany",
     "DeleteOne",
     "InsertOne",
     "ReplaceOne",
     "UpdateMany",
     "UpdateOne",
     "initial_collections",
```

### Comparing `typedmongo-1.4.0/typedmongo/asyncio/__init__.py` & `typedmongo-1.5.0/typedmongo/asyncio/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typedmongo.shortcuts import Contains, EndsWith, StartsWith
+
 from .client import (
     DeleteMany,
     DeleteOne,
     InsertOne,
     ReplaceOne,
     UpdateMany,
     UpdateOne,
@@ -19,14 +21,17 @@
     ListField,
     ObjectIdField,
     StringField,
 )
 from .table import Index, MongoTable, Table
 
 __all__ = [
+    "Contains",
+    "StartsWith",
+    "EndsWith",
     "DeleteMany",
     "DeleteOne",
     "InsertOne",
     "ReplaceOne",
     "UpdateMany",
     "UpdateOne",
     "initial_collections",
```

### Comparing `typedmongo-1.4.0/typedmongo/asyncio/client.py` & `typedmongo-1.5.0/typedmongo/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/typedmongo/asyncio/fields.py` & `typedmongo-1.5.0/typedmongo/asyncio/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/typedmongo/asyncio/table.py` & `typedmongo-1.5.0/typedmongo/asyncio/table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/typedmongo/client.py` & `typedmongo-1.5.0/typedmongo/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/typedmongo/expressions.py` & `typedmongo-1.5.0/typedmongo/expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/typedmongo/fields.py` & `typedmongo-1.5.0/typedmongo/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/typedmongo/marshamallow.py` & `typedmongo-1.5.0/typedmongo/marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/typedmongo/sync.py` & `typedmongo-1.5.0/typedmongo/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/typedmongo/table.py` & `typedmongo-1.5.0/typedmongo/table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.4.0/PKG-INFO` & `typedmongo-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typedmongo
-Version: 1.4.0
+Version: 1.5.0
 Summary: A production-ready modern Python MongoDB ODM
 Author-Email: abersheeran <me@abersheeran.com>
 License: Apache2.0
 Requires-Python: >=3.10
 Requires-Dist: pymongo>=4.6.3
 Requires-Dist: motor>=3.4.0
 Requires-Dist: marshmallow>=3.21.1
```

