# Comparing `tmp/t_object-0.1.7.tar.gz` & `tmp/t_object-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-pnkefpib/t_object-0.1.7.tar", last modified: Sat Apr  6 12:57:50 2024, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-anhyfj6r/t_object-0.1.8.tar", last modified: Thu May  9 21:43:03 2024, max compression
```

## Comparing `t_object-0.1.7.tar` & `t_object-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-06 12:57:50.858070 t_object-0.1.7/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-06 12:57:28.000000 t_object-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4324 2024-04-06 12:57:50.858070 t_object-0.1.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3871 2024-04-06 12:57:28.000000 t_object-0.1.7/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-04-06 12:57:28.000000 t_object-0.1.7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-06 12:57:28.000000 t_object-0.1.7/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-06 12:57:50.862070 t_object-0.1.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-06 12:57:28.000000 t_object-0.1.7/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-06 12:57:50.858070 t_object-0.1.7/t_object/
--rw-rw-rw-   0 root         (0) root         (0)      449 2024-04-06 12:57:28.000000 t_object-0.1.7/t_object/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8338 2024-04-06 12:57:28.000000 t_object-0.1.7/t_object/base_object.py
--rw-rw-rw-   0 root         (0) root         (0)     8633 2024-04-06 12:57:28.000000 t_object-0.1.7/t_object/builder.py
--rw-rw-rw-   0 root         (0) root         (0)      672 2024-04-06 12:57:28.000000 t_object-0.1.7/t_object/config_enums.py
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-06 12:57:28.000000 t_object-0.1.7/t_object/t_object.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-06 12:57:50.858070 t_object-0.1.7/t_object.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4324 2024-04-06 12:57:50.000000 t_object-0.1.7/t_object.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      397 2024-04-06 12:57:50.000000 t_object-0.1.7/t_object.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-06 12:57:50.000000 t_object-0.1.7/t_object.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-06 12:57:50.000000 t_object-0.1.7/t_object.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-06 12:57:50.000000 t_object-0.1.7/t_object.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-06 12:57:50.000000 t_object-0.1.7/t_object.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-06 12:57:50.858070 t_object-0.1.7/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2734 2024-04-06 12:57:28.000000 t_object-0.1.7/tests/test_t_object.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:43:03.937655 t_object-0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-09 21:42:38.000000 t_object-0.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4324 2024-05-09 21:43:03.937655 t_object-0.1.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3871 2024-05-09 21:42:38.000000 t_object-0.1.8/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-09 21:42:38.000000 t_object-0.1.8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-05-09 21:42:38.000000 t_object-0.1.8/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-09 21:43:03.937655 t_object-0.1.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-09 21:42:38.000000 t_object-0.1.8/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:43:03.937655 t_object-0.1.8/t_object/
+-rw-rw-rw-   0 root         (0) root         (0)      449 2024-05-09 21:42:38.000000 t_object-0.1.8/t_object/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7264 2024-05-09 21:42:38.000000 t_object-0.1.8/t_object/base_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     8633 2024-05-09 21:42:38.000000 t_object-0.1.8/t_object/builder.py
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-05-09 21:42:38.000000 t_object-0.1.8/t_object/config_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-05-09 21:42:38.000000 t_object-0.1.8/t_object/t_object.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:43:03.937655 t_object-0.1.8/t_object.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4324 2024-05-09 21:43:03.000000 t_object-0.1.8/t_object.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      397 2024-05-09 21:43:03.000000 t_object-0.1.8/t_object.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-09 21:43:03.000000 t_object-0.1.8/t_object.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-09 21:43:03.000000 t_object-0.1.8/t_object.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-09 21:43:03.000000 t_object-0.1.8/t_object.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-05-09 21:43:03.000000 t_object-0.1.8/t_object.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:43:03.937655 t_object-0.1.8/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2963 2024-05-09 21:42:38.000000 t_object-0.1.8/tests/test_t_object.py
```

### Comparing `t_object-0.1.7/PKG-INFO` & `t_object-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_object
-Version: 0.1.7
+Version: 0.1.8
 Summary: t_object
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_object
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_object-0.1.7/README.rst` & `t_object-0.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `t_object-0.1.7/setup.py` & `t_object-0.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,11 +22,11 @@
     description="t_object",
     long_description=readme,
     keywords="t_object",
     name="t_object",
     packages=find_packages(include=["t_object", "t_object.*"]),
     test_suite="tests",
     url="https://www.thoughtful.ai/",
-    version="0.1.7",
+    version="0.1.8",
     zip_safe=False,
     install_requires=install_requirements,
 )
```

### Comparing `t_object-0.1.7/t_object/base_object.py` & `t_object-0.1.8/t_object/base_object.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,48 @@
 """This module contains the Base Thoughtful Object."""
 
 import json
 import os
 import pickle
 
-from deprecated.classic import deprecated
-from pydantic import BaseModel, TypeAdapter, ValidationError
+from pydantic import BaseModel, TypeAdapter
 
 
 class _BaseThoughtfulObject(BaseModel):
     """This class is the base class for all Thoughtful objects."""
 
-    @deprecated(reason="This method renamed, please use 'to_json_str' method instead.")
-    def convert_to_json_string(self) -> str:
+    def to_json_str(self, include_fields: list[str] = None) -> str:
         """Convert an episode to a json string."""
-        return self.to_json_str()
-
-    def to_json_str(self) -> str:
-        """Convert an episode to a json string."""
-        return self.model_dump_json(indent=4)
-
-    @deprecated(reason="This method renamed, please use 'to_dict' method instead.")
-    def convert_to_dict(self) -> dict:
-        """Convert an object to a dictionary."""
-        return self.to_dict()
+        return self.model_dump_json(indent=4, include=include_fields)
 
     def to_dict(self) -> dict:
         """Convert an object to a dictionary."""
         return self.model_dump()
 
-    def save_to_json_file(self, file_path: str = "") -> str:
+    def save_to_json_file(self, file_path: str = "", include_fields: list[str] = None) -> str:
         """Save an episode to a json file.
 
         Args:
             file_path (str): The path to the file.
+            include_fields (list[str], optional): The fields to include in the json file.
         """
         folder_path = os.path.join(os.getcwd(), "output")
         if not os.path.exists(folder_path):
             folder_path = os.getcwd()
         self._custom_model_config["json_file_path"] = os.path.join(folder_path, f"{self.__class__.__name__}-%s.json")
 
         file_path = file_path or self._get_json_default_file_path()
         if not file_path:
             raise ValueError("File path must be provided or set in the model config.")
         _, extension = os.path.splitext(file_path)
         if extension != ".json":
             raise ValueError(f"File extension must be .json, not {extension}")
 
         with open(file_path, "w") as file:
-            file.write(self.convert_to_json_string())
+            file.write(self.to_json_str(include_fields))
         return file_path
 
     def save_to_pickle_file(self, file_path: str) -> str:
         """Save an object to a pickle file.
 
         Args:
             file_path (str): The path to the file.
@@ -62,35 +52,32 @@
             raise ValueError("File path must be provided or set in the model config.")
         with open(file_path, "wb") as file:
             pickle.dump(self, file)
         return file_path
 
     def pretty_string(self) -> str:
         """Convert an object to a string."""
-        try:
-            text = f"\n==={self.__class__.__name__}===\n"
-            for key, value in self.__dict__.items():
-                value_type = f"<{value.__class__.__name__}>"
-                if isinstance(value, list):
-                    text += f"{key}: LIST[{len(value)}] \n"
-                    for number, item in enumerate(value):
-                        text += f" [{number}] <{item.__class__.__name__}> {self._add_space(item)} \n"
-                elif isinstance(value, tuple):
-                    text += f"{key}: TUPLE[{len(value)}] \n"
-                    for number, item in enumerate(value):
-                        text += f" [{number}] <{item.__class__.__name__}> {self._add_space(item)} \n"
-                elif isinstance(value, dict):
-                    text += f"{key}: DICT[{len(value.keys())}] \n"
-                    for k, v in value.items():
-                        text += f" [{k}] <{v.__class__.__name__}> {self._add_space(v)} \n"
-                else:
-                    text += f"{key}: {value_type} {self._add_space(value)} \n"
-            return text[:-1]
-        except Exception as e:
-            raise ValueError(f"Unable to convert object to string. {e}")
+        text = f"\n==={self.__class__.__name__}===\n"
+        for key, value in self.__dict__.items():
+            value_type = f"<{value.__class__.__name__}>"
+            if isinstance(value, list):
+                text += f"{key}: LIST[{len(value)}] \n"
+                for number, item in enumerate(value):
+                    text += f" [{number}] <{item.__class__.__name__}> {self._add_space(item)} \n"
+            elif isinstance(value, tuple):
+                text += f"{key}: TUPLE[{len(value)}] \n"
+                for number, item in enumerate(value):
+                    text += f" [{number}] <{item.__class__.__name__}> {self._add_space(item)} \n"
+            elif isinstance(value, dict):
+                text += f"{key}: DICT[{len(value.keys())}] \n"
+                for k, v in value.items():
+                    text += f" [{k}] <{v.__class__.__name__}> {self._add_space(v)} \n"
+            else:
+                text += f"{key}: {value_type} {self._add_space(value)} \n"
+        return text[:-1]
 
     def _add_space(self, text: object):
         text = text.pretty_string() if isinstance(text, _BaseThoughtfulObject) else str(text)
         spaces = 4
         return text.replace("\n", "\n" + spaces * " ")
 
     @classmethod
@@ -104,36 +91,30 @@
             object: The objects.
         """
         try:
             with open(file_path, "rb") as file:
                 return pickle.load(file)
         except FileNotFoundError:
             raise FileNotFoundError(f"Unable to load file {file_path}. File not Found.")
-        except Exception as e:
-            raise Exception(f"Unable to load file {file_path}. {e}")
 
     @classmethod
     def load_from_json_file(cls, file_path: str) -> "_BaseThoughtfulObject":
         """Load an object from a json file and returns the object.
 
         Args:
             file_path (str): The path to the file.
 
         Returns:
             object: The objects.
         """
         try:
             with open(file_path, "r") as file:
                 return cls.model_validate_json(file.read())
-        except ValidationError as e:
-            raise ValidationError(f"Unable to load file {file_path}. Some fields are missing . \n {e}")
         except FileNotFoundError:
             raise FileNotFoundError(f"Unable to load file {file_path}. File not Found.")
-        except Exception as e:
-            raise Exception(f"Unable to load file {file_path}. {e}")
 
     def get_json_schema(self, file_path):
         """Return the json schema for the object."""
         _, extension = os.path.splitext(file_path)
         if extension != ".json":
             raise ValueError(f"File extension must be .json, not {extension}")
 
@@ -195,13 +176,9 @@
 
         """
         ta = TypeAdapter(list[cls])
         try:
             with open(file_path, "r") as file:
                 data = file.read()
                 return ta.validate_json(data)
-        except ValidationError as e:
-            raise ValidationError(f"Unable to load file {file_path}. Some fields are missing . \n {e}") from e
         except FileNotFoundError:
             raise FileNotFoundError(f"Unable to load file {file_path}. File not Found.")
-        except Exception as e:
-            raise Exception(f"Unable to load file {file_path}. {e}")
```

### Comparing `t_object-0.1.7/t_object/builder.py` & `t_object-0.1.8/t_object/builder.py`

 * *Files identical despite different names*

### Comparing `t_object-0.1.7/t_object/config_enums.py` & `t_object-0.1.8/t_object/config_enums.py`

 * *Files identical despite different names*

### Comparing `t_object-0.1.7/t_object/t_object.py` & `t_object-0.1.8/t_object/t_object.py`

 * *Files identical despite different names*

### Comparing `t_object-0.1.7/t_object.egg-info/PKG-INFO` & `t_object-0.1.8/t_object.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t_object
-Version: 0.1.7
+Version: 0.1.8
 Summary: t_object
 Home-page: https://www.thoughtful.ai/
 Author: Thoughtful
 Author-email: support@thoughtful.ai
 Keywords: t_object
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `t_object-0.1.7/tests/test_t_object.py` & `t_object-0.1.8/tests/test_t_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,19 @@
         """Test the export of the object."""
         self.patient.save_to_json_file(),
         self.car.save_to_json_file()
         self.car.save_to_json_file()
         self.car.save_to_json_file()
         self.car.save_to_json_file()
 
+    def test_export_some_fields(self):
+        """Test the export of the object with some fields."""
+        file = self.patient.save_to_json_file(include_fields=["name", "age"])
+        print(Patient.load_from_json_file(file))
+
     def test_import(self):
         """Test the import of the object."""
         self.patient.save_to_json_file(os.path.join(self.output_dir, "patient.json")),
         self.car.save_to_json_file(os.path.join(self.output_dir, "car.json"))
         patient = Patient.load_from_json_file(os.path.join(self.output_dir, "patient.json"))
         car = Car.load_from_json_file(os.path.join(self.output_dir, "car.json"))
         self.assertEqual(self.patient, patient)
```

