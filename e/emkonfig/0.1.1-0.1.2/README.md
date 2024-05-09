# Comparing `tmp/emkonfig-0.1.1.tar.gz` & `tmp/emkonfig-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emkonfig-0.1.1.tar", max compression
+gzip compressed data, was "emkonfig-0.1.2.tar", max compression
```

## Comparing `emkonfig-0.1.1.tar` & `emkonfig-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       11 2024-02-29 13:39:01.443391 emkonfig-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-20 15:33:07.236309 emkonfig-0.1.1/emkonfig/__init__.py
--rw-r--r--   0        0        0     1589 2024-04-23 12:32:00.439509 emkonfig-0.1.1/emkonfig/config.py
--rw-r--r--   0        0        0     4684 2024-04-23 10:42:07.825422 emkonfig-0.1.1/emkonfig/parsers.py
--rw-r--r--   0        0        0     1052 2024-03-21 15:44:31.173249 emkonfig-0.1.1/emkonfig/registry.py
--rw-r--r--   0        0        0      168 2024-03-15 15:24:03.373331 emkonfig-0.1.1/emkonfig/utils.py
--rw-r--r--   0        0        0     3104 2024-04-23 14:45:57.897258 emkonfig-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 emkonfig-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-02-29 13:39:01.443391 emkonfig-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-20 15:33:07.236309 emkonfig-0.1.2/emkonfig/__init__.py
+-rw-r--r--   0        0        0     1589 2024-04-23 12:32:00.439509 emkonfig-0.1.2/emkonfig/config.py
+-rw-r--r--   0        0        0     4828 2024-05-09 13:32:22.917539 emkonfig-0.1.2/emkonfig/parsers.py
+-rw-r--r--   0        0        0     1052 2024-03-21 15:44:31.173249 emkonfig-0.1.2/emkonfig/registry.py
+-rw-r--r--   0        0        0      168 2024-03-15 15:24:03.373331 emkonfig-0.1.2/emkonfig/utils.py
+-rw-r--r--   0        0        0     3104 2024-05-06 14:24:16.527696 emkonfig-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 emkonfig-0.1.2/PKG-INFO
```

### Comparing `emkonfig-0.1.1/emkonfig/config.py` & `emkonfig-0.1.2/emkonfig/config.py`

 * *Files identical despite different names*

### Comparing `emkonfig-0.1.1/emkonfig/parsers.py` & `emkonfig-0.1.2/emkonfig/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,22 +51,25 @@
                     value = {}
                 assert isinstance(value, dict), f"Invalid value for class slug key parser: {value}"
                 class_slug, new_key = self.parse_class_slug_key(key)
                 cls = _EMKONFIG_REGISTRY[class_slug]
                 cls_location = cls.__module__ + "." + cls.__name__
                 parameters = _EMKONFIG_DEFAULTS_REGISTRY[class_slug]
                 parameters.update(value)
-                new_content[new_key] = {"_target_": cls_location, **parameters}
+                if new_key == "_":
+                    new_content.update({"_target_": cls_location, **parameters})
+                else:
+                    new_content[new_key] = {"_target_": cls_location, **parameters}
                 del new_content[key]
 
         return new_content
 
     @staticmethod
     def parse_class_slug_key(key: str) -> tuple[str, str]:
-        if "as" in key:
+        if " as " in key:
             class_slug, new_key = key[2:-1].split(" as ")
         else:
             class_slug = key[2:-1]
             new_key = key[2:-1]
         return class_slug, new_key
```

### Comparing `emkonfig-0.1.1/emkonfig/registry.py` & `emkonfig-0.1.2/emkonfig/registry.py`

 * *Files identical despite different names*

### Comparing `emkonfig-0.1.1/pyproject.toml` & `emkonfig-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emkonfig"
-version = "0.1.1"
+version = "0.1.2"
 description = "YAML template based configuration management tool"
 authors = ["Kıvanç Yüksel <kivanc.yuksel@emkademy.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers= [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `emkonfig-0.1.1/PKG-INFO` & `emkonfig-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emkonfig
-Version: 0.1.1
+Version: 0.1.2
 Summary: YAML template based configuration management tool
 License: MIT
 Author: Kıvanç Yüksel
 Author-email: kivanc.yuksel@emkademy.com
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

