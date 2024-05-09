# Comparing `tmp/pypomes_core-0.9.7.tar.gz` & `tmp/pypomes_core-0.9.8.tar.gz`

## Comparing `pypomes_core-0.9.7.tar` & `pypomes_core-0.9.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    28318 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2887 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    24281 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-0.9.8/PKG-INFO
```

### Comparing `pypomes_core-0.9.7/src/pypomes_core/.ruff.toml` & `pypomes_core-0.9.8/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/src/pypomes_core/__init__.py` & `pypomes_core-0.9.8/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.9.8/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.9.8/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/src/pypomes_core/email_pomes.py` & `pypomes_core-0.9.8/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.9.8/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/src/pypomes_core/env_pomes.py` & `pypomes_core-0.9.8/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.9.8/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/src/pypomes_core/file_pomes.py` & `pypomes_core-0.9.8/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/src/pypomes_core/json_pomes.py` & `pypomes_core-0.9.8/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/src/pypomes_core/list_pomes.py` & `pypomes_core-0.9.8/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/src/pypomes_core/str_pomes.py` & `pypomes_core-0.9.8/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/src/pypomes_core/validation_msgs.py` & `pypomes_core-0.9.8/src/pypomes_core/validation_msgs.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         "en": "Authentication token required",
         "pt": "Token de autenticação deve ser fornecido",
     },
     109: {
         "en": "Invalid authentication token",
         "pt": "Token de autenticação inválido",
     },
+    110: {
+        "en": "{} {} {} {}",
+        "pt": "{} {} {} {}",
+    },
     111: {
         "en": "Unknown attribute",
         "pt": "Atributo desconhecido",
     },
     112: {
         "en": "Required attribute",
         "pt": "Atributo obrigatório",
```

### Comparing `pypomes_core-0.9.7/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.9.8/src/pypomes_core/validation_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,15 +520,15 @@
         case "pt":
             from .validation_msgs import _ERR_MSGS_PT
             err_msgs = _ERR_MSGS_PT
         case _:
             err_msgs = {}
 
     # initialize the return variable
-    result: str = VALIDATE_MSG_PREFIX + str(error_id) + ": " + err_msgs.get(error_id)
+    result: str = VALIDATE_MSG_PREFIX + str(error_id) + ": " + (err_msgs.get(error_id) or "")
 
     # apply the provided arguments
     for arg in args:
         if arg is None:
             result = result.replace(" {}", "", 1)
         elif isinstance(arg, str) and arg.startswith("@"):
             result += " " + arg
```

### Comparing `pypomes_core-0.9.7/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.9.8/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/LICENSE` & `pypomes_core-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.9.7/pyproject.toml` & `pypomes_core-0.9.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.9.7"
+version = "0.9.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-0.9.7/PKG-INFO` & `pypomes_core-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 0.9.7
+Version: 0.9.8
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```
