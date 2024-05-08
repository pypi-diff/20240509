# Comparing `tmp/confhub-0.0.4a0.tar.gz` & `tmp/confhub-0.0.5a0.tar.gz`

## Comparing `confhub-0.0.4a0.tar` & `confhub-0.0.5a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 confhub-0.0.4a0/CHANGELOG.md
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 confhub-0.0.4a0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/__init__.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/__main__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/__meta__.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/commands.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/enums.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/exceptions.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/models.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/reader.py
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/setup_logger.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 confhub-0.0.4a0/confhub/templates.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 confhub-0.0.4a0/tests/.secrets.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 confhub-0.0.4a0/tests/example__secrets.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 confhub-0.0.4a0/tests/settings.yml
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 confhub-0.0.4a0/tests/test_confhub.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 confhub-0.0.4a0/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 confhub-0.0.4a0/LICENSE
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 confhub-0.0.4a0/README.md
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 confhub-0.0.4a0/pyproject.toml
--rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 confhub-0.0.4a0/PKG-INFO
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 confhub-0.0.5a0/CHANGELOG.md
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 confhub-0.0.5a0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 confhub-0.0.5a0/confhub/__init__.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 confhub-0.0.5a0/confhub/__main__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 confhub-0.0.5a0/confhub/__meta__.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 confhub-0.0.5a0/confhub/commands.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 confhub-0.0.5a0/confhub/enums.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 confhub-0.0.5a0/confhub/exceptions.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 confhub-0.0.5a0/confhub/models.py
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 confhub-0.0.5a0/confhub/reader.py
+-rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 confhub-0.0.5a0/confhub/setup_logger.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 confhub-0.0.5a0/confhub/templates.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 confhub-0.0.5a0/tests/.secrets.yml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 confhub-0.0.5a0/tests/example__secrets.yml
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 confhub-0.0.5a0/tests/settings.yml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 confhub-0.0.5a0/tests/test_confhub.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 confhub-0.0.5a0/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 confhub-0.0.5a0/LICENSE
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 confhub-0.0.5a0/README.md
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 confhub-0.0.5a0/pyproject.toml
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 confhub-0.0.5a0/PKG-INFO
```

### Comparing `confhub-0.0.4a0/CHANGELOG.md` & `confhub-0.0.5a0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `confhub-0.0.4a0/confhub/__main__.py` & `confhub-0.0.5a0/confhub/__main__.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.4a0/confhub/commands.py` & `confhub-0.0.5a0/confhub/commands.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.4a0/confhub/enums.py` & `confhub-0.0.5a0/confhub/enums.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.4a0/confhub/exceptions.py` & `confhub-0.0.5a0/confhub/exceptions.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.4a0/confhub/models.py` & `confhub-0.0.5a0/confhub/models.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.4a0/confhub/reader.py` & `confhub-0.0.5a0/confhub/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from dynaconf.utils.boxing import DynaBox
 
 from confhub.enums import Service
 from confhub.exceptions import PathError, ModuleException
 from confhub.setup_logger import SetupLogger, LoggerReg
 
 logger: structlog.BoundLogger = structlog.get_logger("confhub")
+load_dotenv()
 
 
 class ReaderConf:
     """
 
     Class for reading configuration files.
     Supported configuration formats:
@@ -32,51 +33,54 @@
     data_export(): Returns collected data in dictionary format.
     create_service_urls(): Finds services in the configuration and creates URLs for them.
 
     """
     def __init__(
             self,
             *paths: str | Path,
-            env: str | Path = '.env',
             dev: bool = False,
             logger_registrations: Optional[list[LoggerReg]] = None,
     ) -> None:
         """
         :param paths: str | Path - Configuration path
-        :param env: str| Path - Path to the project environment variable file
         :param dev: Local priority for configuration determination,
         :param logger_registrations: Logger configuration, default: LoggerReg(name="", level=LoggerReg.Level.DEBUG)
         """
         if logger_registrations is None:
             logger_registrations = [LoggerReg(name="", level=LoggerReg.Level.DEBUG)]
 
         SetupLogger(name_registration=logger_registrations, default_development=dev)
 
         self.dev = dev
         PathError.checking_paths(*paths)
         settings_files = [*paths]
 
         try:
-            PathError.checking_paths(env)
-            load_dotenv(env)
+            PathError.checking_paths('.env')
         except PathError as _:
-            logger.warning('The `.env` file was not found and will not be loaded!', env_path=env)
+            logger.warning('The `.env` file was not found and will not be loaded!')
 
         __data: LazySettings = Dynaconf(settings_files=settings_files)
 
+        try:
+            self.is_dev = bool(__data.dev)
+        except ValueError:
+            logger.warning('Development clarification point is not set or is not of type `bool`', default_value=self.dev)
+            self.is_dev = False
+
         self.data = self.data_export(data=__data)
 
     def data_export(self, data: LazySettings) -> dict:
         """
         Returns collected data in dictionary format
 
         :param data: LazySettings - LazySettings object
         :return: dict - collected data in dictionary format depending on development conditions
         """
-        if os.getenv('DEV', False) or self.dev:
+        if self.is_dev or self.dev:
             __data: DynaBox = data.get('development')
         else:
             __data: DynaBox = data.get('release')
 
         if __data is None:
             raise ModuleException('The configuration is empty! Please check your configuration data.')
```

### Comparing `confhub-0.0.4a0/confhub/setup_logger.py` & `confhub-0.0.5a0/confhub/setup_logger.py`

 * *Files identical despite different names*

### Comparing `confhub-0.0.4a0/tests/test_confhub.py` & `confhub-0.0.5a0/tests/test_confhub.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,12 +9,12 @@
     )
 
     assert url_config.scheme == 'http'
     assert url_config.port == 8080
 
 
 def test_reader() -> None:
-    reader = ReaderConf('tests/settings.yml', 'tests/.secrets.yml', env='tests/.env', dev=True, )
+    reader = ReaderConf('tests/settings.yml', 'tests/.secrets.yml', dev=True, )
     reader.create_service_urls()
     configuration = reader.data
 
     assert configuration.get('postgresql_url') == 'postgresql+asyncpg://ghost:qwerty@127.0.0.1:5432/database'
```

### Comparing `confhub-0.0.4a0/.gitignore` & `confhub-0.0.5a0/.gitignore`

 * *Files identical despite different names*

### Comparing `confhub-0.0.4a0/LICENSE` & `confhub-0.0.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `confhub-0.0.4a0/README.md` & `confhub-0.0.5a0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 ```
 
 Далее вы можете использовать конфигурацию в вашем коде:
 
 ```python
 from confhub.reader import ReaderConf
 
-reader = ReaderConf('config/settings.yml', 'config/.secrets.yml', env='config/.env', dev=True)
+reader = ReaderConf('config/settings.yml', 'config/.secrets.yml', dev=True)
 reader.create_service_urls()
 configuration = reader.data
 
 assert configuration.get('postgresql_url') == 'postgresql+asyncpg://ghost:qwerty@127.0.0.1:5432/database'
 # True
 ```
 
@@ -85,15 +85,15 @@
         WARNING: str = "WARNING"
         ERROR: str = "ERROR"
         CRITICAL: str = "CRITICAL"
         NONE: str = None
 """
 
 reader = ReaderConf(
-    'config/settings.yml', 'config/.secrets.yml', env='config/.env', dev=True,
+    'config/settings.yml', 'config/.secrets.yml', dev=True,
     logger_registrations = [
         LoggerReg(name="название вашего логера", level=LoggerReg.Level.INFO),
         LoggerReg(name="название вашего следующего логера", level=LoggerReg.Level.ERROR),
         # и так далее
     ]
 )
 ```
```

### Comparing `confhub-0.0.4a0/pyproject.toml` & `confhub-0.0.5a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `confhub-0.0.4a0/PKG-INFO` & `confhub-0.0.5a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: confhub
-Version: 0.0.4a0
+Version: 0.0.5a0
 Summary: Configuration add-on to Dynaconf
 Project-URL: Repository, https://github.com/morington/confhub/
 Author-email: Adam Morington <morington.mail@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: cfg,confhub,config,configuration,dynaconf,setting,settings
 Classifier: Development Status :: 3 - Alpha
@@ -77,15 +77,15 @@
 ```
 
 Далее вы можете использовать конфигурацию в вашем коде:
 
 ```python
 from confhub.reader import ReaderConf
 
-reader = ReaderConf('config/settings.yml', 'config/.secrets.yml', env='config/.env', dev=True)
+reader = ReaderConf('config/settings.yml', 'config/.secrets.yml', dev=True)
 reader.create_service_urls()
 configuration = reader.data
 
 assert configuration.get('postgresql_url') == 'postgresql+asyncpg://ghost:qwerty@127.0.0.1:5432/database'
 # True
 ```
 
@@ -111,15 +111,15 @@
         WARNING: str = "WARNING"
         ERROR: str = "ERROR"
         CRITICAL: str = "CRITICAL"
         NONE: str = None
 """
 
 reader = ReaderConf(
-    'config/settings.yml', 'config/.secrets.yml', env='config/.env', dev=True,
+    'config/settings.yml', 'config/.secrets.yml', dev=True,
     logger_registrations = [
         LoggerReg(name="название вашего логера", level=LoggerReg.Level.INFO),
         LoggerReg(name="название вашего следующего логера", level=LoggerReg.Level.ERROR),
         # и так далее
     ]
 )
 ```
```

