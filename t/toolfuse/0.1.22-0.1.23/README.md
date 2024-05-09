# Comparing `tmp/toolfuse-0.1.22.tar.gz` & `tmp/toolfuse-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolfuse-0.1.22.tar", max compression
+gzip compressed data, was "toolfuse-0.1.23.tar", max compression
```

## Comparing `toolfuse-0.1.22.tar` & `toolfuse-0.1.23.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.22/LICENSE
--rw-r--r--   0        0        0     4594 2024-05-05 16:31:27.833089 toolfuse-0.1.22/README.md
--rw-r--r--   0        0        0      803 2024-05-05 17:31:35.898085 toolfuse-0.1.22/pyproject.toml
--rw-r--r--   0        0        0      435 2024-05-05 03:00:01.092317 toolfuse-0.1.22/toolfuse/__init__.py
--rw-r--r--   0        0        0    30482 2024-05-05 17:31:31.075720 toolfuse-0.1.22/toolfuse/base.py
--rw-r--r--   0        0        0      197 2024-04-27 21:02:03.126589 toolfuse-0.1.22/toolfuse/models.py
--rw-r--r--   0        0        0      996 2024-05-05 02:09:19.322511 toolfuse-0.1.22/toolfuse/multi.py
--rw-r--r--   0        0        0      543 2024-05-05 03:06:09.263475 toolfuse-0.1.22/toolfuse/util.py
--rw-r--r--   0        0        0     5239 1970-01-01 00:00:00.000000 toolfuse-0.1.22/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.23/LICENSE
+-rw-r--r--   0        0        0     4594 2024-05-05 16:31:27.833089 toolfuse-0.1.23/README.md
+-rw-r--r--   0        0        0      803 2024-05-09 18:37:40.377543 toolfuse-0.1.23/pyproject.toml
+-rw-r--r--   0        0        0      435 2024-05-05 03:00:01.092317 toolfuse-0.1.23/toolfuse/__init__.py
+-rw-r--r--   0        0        0    30555 2024-05-09 18:37:31.926716 toolfuse-0.1.23/toolfuse/base.py
+-rw-r--r--   0        0        0      231 2024-05-09 18:34:01.339814 toolfuse-0.1.23/toolfuse/models.py
+-rw-r--r--   0        0        0      996 2024-05-05 02:09:19.322511 toolfuse-0.1.23/toolfuse/multi.py
+-rw-r--r--   0        0        0      543 2024-05-05 03:06:09.263475 toolfuse-0.1.23/toolfuse/util.py
+-rw-r--r--   0        0        0     5239 1970-01-01 00:00:00.000000 toolfuse-0.1.23/PKG-INFO
```

### Comparing `toolfuse-0.1.22/LICENSE` & `toolfuse-0.1.23/LICENSE`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.22/README.md` & `toolfuse-0.1.23/README.md`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.22/pyproject.toml` & `toolfuse-0.1.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toolfuse"
-version = "0.1.22"
+version = "0.1.23"
 description = "Tools for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "toolfuse"}]
 
 [tool.poetry.dependencies]
```

### Comparing `toolfuse-0.1.22/toolfuse/base.py` & `toolfuse-0.1.23/toolfuse/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,19 @@
 
     def ref(self) -> V1ToolRef:
         """Tool reference"""
         module = getmodule(self)
         if not module:
             raise ValueError("Tool not associated with a module")
         mod_parts = module.__name__.split(".")
-        version = pkgversion(mod_parts[0])
+        version = None
+        try:
+            version = pkgversion(mod_parts[0])
+        except:
+            pass
         return V1ToolRef(module=module.__name__, name=self.name(), version=version)
 
     def add_action(self, method: Callable) -> None:
         """
         Adds a new action to the tool using only the method provided. Name, schema,
         and description are derived automatically.
```

### Comparing `toolfuse-0.1.22/toolfuse/multi.py` & `toolfuse-0.1.23/toolfuse/multi.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.22/toolfuse/util.py` & `toolfuse-0.1.23/toolfuse/util.py`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.22/PKG-INFO` & `toolfuse-0.1.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolfuse
-Version: 0.1.22
+Version: 0.1.23
 Summary: Tools for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

