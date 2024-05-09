# Comparing `tmp/ymlstash-1.0.2.tar.gz` & `tmp/ymlstash-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ymlstash-1.0.2.tar", max compression
+gzip compressed data, was "ymlstash-1.1.0.tar", max compression
```

## Comparing `ymlstash-1.0.2.tar` & `ymlstash-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-05-07 18:56:12.873162 ymlstash-1.0.2/LICENSE
--rw-r--r--   0        0        0     1266 2024-05-07 19:30:45.260589 ymlstash-1.0.2/README.md
--rw-r--r--   0        0        0      572 2024-05-07 20:18:05.720009 ymlstash-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       50 2024-05-07 13:34:28.333474 ymlstash-1.0.2/ymlstash/__init__.py
--rw-r--r--   0        0        0     1691 2024-05-07 19:16:15.727816 ymlstash-1.0.2/ymlstash/stash.py
--rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 ymlstash-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-07 18:56:12.873162 ymlstash-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1457 2024-05-09 09:50:41.964518 ymlstash-1.1.0/README.md
+-rw-r--r--   0        0        0      572 2024-05-09 09:50:57.731089 ymlstash-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       50 2024-05-07 13:34:28.333474 ymlstash-1.1.0/ymlstash/__init__.py
+-rw-r--r--   0        0        0     1948 2024-05-09 09:47:57.228842 ymlstash-1.1.0/ymlstash/stash.py
+-rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 ymlstash-1.1.0/PKG-INFO
```

### Comparing `ymlstash-1.0.2/LICENSE` & `ymlstash-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ymlstash-1.0.2/README.md` & `ymlstash-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -61,10 +61,28 @@
 
 List all keys existing in stash:
 
 ```python
 keys = stash.list_keys()
 ```
 
+Delete a key:
+
+```python
+stash.delete("foo")
+```
+
+Check for key existance:
+
+```python
+stash.exists("foo")
+```
+
+Drop all files (careful, this deletes everything):
+
+```python
+stash.drop()
+```
+
 ## License
 
 [MIT](LICENSE)
```

### Comparing `ymlstash-1.0.2/pyproject.toml` & `ymlstash-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ymlstash"
-version = "1.0.2"
+version = "1.1.0"
 description = "A simple ORM-like utility for operating on local YAML files via Python dataclasses"
 authors = ["Yuval Adam <_@yuv.al>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/yuvadm/ymlstash"
 repository = "https://github.com/yuvadm/ymlstash"
```

### Comparing `ymlstash-1.0.2/ymlstash/stash.py` & `ymlstash-1.1.0/ymlstash/stash.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,50 +2,60 @@
 import os
 
 from dataclasses import asdict, fields
 from pathlib import Path
 
 
 class YmlStash:
-    def __init__(self, clazz, path, file_suffix="yml", unsafe=False):
-        self.clazz = clazz
+    def __init__(self, model, path, file_suffix="yml", unsafe=False):
+        self.model = model
         self.path = Path(path)
         self.file_suffix = f".{file_suffix}"
         self.yaml_loader = yaml.SafeLoader
         self._validate()
 
     def _validate(self):
         if not self.path.exists():
             raise Exception(f"Path {self.path} does not exist and cannot be used")
 
-        key_field = getattr(self.clazz, "key", None)
-        field_names = [f.name for f in fields(self.clazz)]
+        key_field = getattr(self.model, "key", None)
+        field_names = [f.name for f in fields(self.model)]
         if key_field and key_field not in field_names:
-            raise Exception(f"Dataclass {self.clazz} has no key field '{key_field}'")
+            raise Exception(f"Dataclass {self.model} has no key field '{key_field}'")
 
     def _get_path(self, key):
         return self.path / f"{key}{self.file_suffix}"
 
     def load(self, key):
         with open(self._get_path(key)) as f:
             y = yaml.load(f.read(), Loader=self.yaml_loader)
-        return self.clazz(**y)
+        return self.model(**y)
 
     def save(self, obj, key=None):
         if not key:
-            key_field = self.clazz.key
+            key_field = self.model.key
             if not key_field:
                 raise Exception("Cannot save object without a key or key field")
             key = getattr(obj, key_field)
         with open(self._get_path(key), "w") as f:
             f.write(yaml.dump(asdict(obj)))
 
+    def delete(self, key):
+        try:
+            os.remove(self._get_path(key))
+        except FileNotFoundError:
+            raise Exception(
+                f"Attempting to delete key '{key}' which was not found in stash"
+            )
+
+    def exists(self, key):
+        return self._get_path(key).exists()
+
     def _list_files(self):
         return [f for f in os.listdir(self.path) if f.endswith(self.file_suffix)]
 
     def list_keys(self):
         return [f.replace(self.file_suffix, "") for f in self._list_files()]
 
     def drop(self):
-        for f in self._list_files():
-            if f.endswith(self.file_suffix):
-                os.remove(self.path / f)
+        for key in self.list_keys():
+            self.delete(key)
```

### Comparing `ymlstash-1.0.2/PKG-INFO` & `ymlstash-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ymlstash
-Version: 1.0.2
+Version: 1.1.0
 Summary: A simple ORM-like utility for operating on local YAML files via Python dataclasses
 Home-page: https://github.com/yuvadm/ymlstash
 License: MIT
 Author: Yuval Adam
 Author-email: _@yuv.al
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -81,11 +81,29 @@
 
 List all keys existing in stash:
 
 ```python
 keys = stash.list_keys()
 ```
 
+Delete a key:
+
+```python
+stash.delete("foo")
+```
+
+Check for key existance:
+
+```python
+stash.exists("foo")
+```
+
+Drop all files (careful, this deletes everything):
+
+```python
+stash.drop()
+```
+
 ## License
 
 [MIT](LICENSE)
```

