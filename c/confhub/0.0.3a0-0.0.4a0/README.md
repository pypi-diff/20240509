# Comparing `tmp/confhub-0.0.3a0.tar.gz` & `tmp/confhub-0.0.4a0.tar.gz`

## Comparing `confhub-0.0.3a0.tar` & `confhub-0.0.4a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 confhub-0.0.3a0/CHANGELOG.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 confhub-0.0.3a0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/__init__.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/__main__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/__meta__.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/commands.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/enums.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/exceptions.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/models.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/reader.py
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/setup_logger.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 confhub-0.0.3a0/confhub/templates.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 confhub-0.0.3a0/tests/.secrets.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 confhub-0.0.3a0/tests/example__secrets.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 confhub-0.0.3a0/tests/settings.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 confhub-0.0.3a0/tests/test_confhub.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 confhub-0.0.3a0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 confhub-0.0.3a0/LICENSE
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 confhub-0.0.3a0/README.md
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 confhub-0.0.3a0/pyproject.toml
--rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 confhub-0.0.3a0/PKG-INFO
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 confhub-0.0.4a0/CHANGELOG.md
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 confhub-0.0.4a0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/__main__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/__meta__.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/commands.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/enums.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/exceptions.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/models.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/reader.py
+-rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/setup_logger.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/templates.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 confhub-0.0.4a0/tests/.secrets.yml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 confhub-0.0.4a0/tests/example__secrets.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 confhub-0.0.4a0/tests/settings.yml
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 confhub-0.0.4a0/tests/test_confhub.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 confhub-0.0.4a0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 confhub-0.0.4a0/LICENSE
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 confhub-0.0.4a0/README.md
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 confhub-0.0.4a0/pyproject.toml
+-rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 confhub-0.0.4a0/PKG-INFO
```

### Comparing `confhub-0.0.3a0/confhub/__main__.py` & `confhub-0.0.4a0/confhub/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,10 +36,14 @@
         self.parser.add_argument(
             '-c', '--create',
             metavar="folder", type=str,
             help='Generating configuration files'
         )
 
 
-if __name__ == '__main__':
+def main() -> None:
     config = Config()
     config.parsing()
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `confhub-0.0.3a0/confhub/commands.py` & `confhub-0.0.4a0/confhub/commands.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3a0/confhub/enums.py` & `confhub-0.0.4a0/confhub/enums.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,15 +26,18 @@
     rabbitmq = "rabbitmq"
     influxdb = "influxdb"
 
     def get_scheme(self) -> str:
         return Schemes[self.value].value
 
     def create_url(self, data: dict[str, str | int]) -> str:
-        __config = URLConfig(scheme=self.get_scheme(), **data)
+        __config = URLConfig(
+            scheme=data.get('scheme', self.get_scheme()),
+            **{key: value for key, value in data.items() if key != 'scheme'}
+        )
         url: str = __config.get_human_url()
 
         __hidden_config = __config
         
         if __hidden_config.user:
             __hidden_config.user = f"{__hidden_config.user[0]}{'*' * len(__hidden_config.user)}{__hidden_config.user[-1]}"
```

### Comparing `confhub-0.0.3a0/confhub/exceptions.py` & `confhub-0.0.4a0/confhub/exceptions.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3a0/confhub/models.py` & `confhub-0.0.4a0/confhub/models.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3a0/confhub/reader.py` & `confhub-0.0.4a0/confhub/reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from pathlib import Path
 from typing import Optional, Any
 
 import structlog
+from dotenv import load_dotenv
 from dynaconf import Dynaconf, LazySettings
 from dynaconf.utils.boxing import DynaBox
 
 from confhub.enums import Service
 from confhub.exceptions import PathError, ModuleException
 from confhub.setup_logger import SetupLogger, LoggerReg
 
@@ -52,22 +53,19 @@
 
         self.dev = dev
         PathError.checking_paths(*paths)
         settings_files = [*paths]
 
         try:
             PathError.checking_paths(env)
-            settings_files.append(env)
+            load_dotenv(env)
         except PathError as _:
             logger.warning('The `.env` file was not found and will not be loaded!', env_path=env)
 
-        __data: LazySettings = Dynaconf(
-            load_dotenv=True,
-            settings_files=settings_files
-        )
+        __data: LazySettings = Dynaconf(settings_files=settings_files)
 
         self.data = self.data_export(data=__data)
 
     def data_export(self, data: LazySettings) -> dict:
         """
         Returns collected data in dictionary format
```

### Comparing `confhub-0.0.3a0/confhub/setup_logger.py` & `confhub-0.0.4a0/confhub/setup_logger.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3a0/confhub/templates.py` & `confhub-0.0.4a0/confhub/templates.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3a0/tests/test_confhub.py` & `confhub-0.0.4a0/tests/test_confhub.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3a0/.gitignore` & `confhub-0.0.4a0/.gitignore`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3a0/LICENSE` & `confhub-0.0.4a0/LICENSE`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3a0/README.md` & `confhub-0.0.4a0/README.md`

 * *Files identical despite different names*

### Comparing `confhub-0.0.3a0/pyproject.toml` & `confhub-0.0.4a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -40,8 +40,11 @@
 ]
 dynamic = ["version"]
 
 [tool.hatch.version]
 path = "confhub/__meta__.py"
 
 [project.urls]
-Repository = "https://github.com/morington/confhub/"
+Repository = "https://github.com/morington/confhub/"
+
+[project.scripts]
+confhub = "confhub.__main__:main"
```

### Comparing `confhub-0.0.3a0/PKG-INFO` & `confhub-0.0.4a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: confhub
-Version: 0.0.3a0
+Version: 0.0.4a0
 Summary: Configuration add-on to Dynaconf
 Project-URL: Repository, https://github.com/morington/confhub/
 Author-email: Adam Morington <morington.mail@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: cfg,confhub,config,configuration,dynaconf,setting,settings
 Classifier: Development Status :: 3 - Alpha
```

