# Comparing `tmp/libgal-1.0.2.tar.gz` & `tmp/libgal-1.0.3.tar.gz`

## Comparing `libgal-1.0.2.tar` & `libgal-1.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/FSUtils.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/HTMLParser.md
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/Installation.md
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/LoadEnv.md
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/Logger.md
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/SQLAlchemy.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/SQLMemory.md
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/Selenium.md
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/SimpleTeradata.md
--rw-r--r--   0        0        0    13840 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/Teradata.md
--rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/Utils.md
--rw-r--r--   0        0        0    15306 2020-02-02 00:00:00.000000 libgal-1.0.2/docs/by_example/TeradataExamples.md
--rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/__init__.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/DatabaseAPI.py
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/FSUtils.py
--rw-r--r--   0        0        0     4881 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/Logger.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/MLS.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/ODBCTools.py
--rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/SQLAlchemy.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/SQLMemory.py
--rw-r--r--   0        0        0    10366 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/Sqlite.py
--rw-r--r--   0        0        0    21087 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/Teradata.py
--rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/Utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libgal-1.0.2/libgal/modules/__init__.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/CSVFileLoggerTests.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/FileLoggerTests.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/JSONFileLoggerTests.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/LoggerTests.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/SQLAlchemyTests.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/SQliteTests.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/TeradataBasicTest.py
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/TeradataMLTests.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/TestEvaluateKsAndRocAuc.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 libgal-1.0.2/tests/TestNumNormTransformer.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 libgal-1.0.2/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libgal-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 libgal-1.0.2/README.md
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 libgal-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     9122 2020-02-02 00:00:00.000000 libgal-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 libgal-1.0.3/docs/FSUtils.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 libgal-1.0.3/docs/HTMLParser.md
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 libgal-1.0.3/docs/Installation.md
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 libgal-1.0.3/docs/LoadEnv.md
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 libgal-1.0.3/docs/Logger.md
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 libgal-1.0.3/docs/SQLAlchemy.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 libgal-1.0.3/docs/SQLMemory.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 libgal-1.0.3/docs/Selenium.md
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 libgal-1.0.3/docs/SimpleTeradata.md
+-rw-r--r--   0        0        0    13840 2020-02-02 00:00:00.000000 libgal-1.0.3/docs/Teradata.md
+-rw-r--r--   0        0        0    13437 2020-02-02 00:00:00.000000 libgal-1.0.3/docs/Utils.md
+-rw-r--r--   0        0        0    15306 2020-02-02 00:00:00.000000 libgal-1.0.3/docs/by_example/TeradataExamples.md
+-rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 libgal-1.0.3/libgal/__init__.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 libgal-1.0.3/libgal/modules/DatabaseAPI.py
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 libgal-1.0.3/libgal/modules/FSUtils.py
+-rw-r--r--   0        0        0     4945 2020-02-02 00:00:00.000000 libgal-1.0.3/libgal/modules/Logger.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 libgal-1.0.3/libgal/modules/MLS.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 libgal-1.0.3/libgal/modules/ODBCTools.py
+-rw-r--r--   0        0        0     5393 2020-02-02 00:00:00.000000 libgal-1.0.3/libgal/modules/SQLAlchemy.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 libgal-1.0.3/libgal/modules/SQLMemory.py
+-rw-r--r--   0        0        0    10366 2020-02-02 00:00:00.000000 libgal-1.0.3/libgal/modules/Sqlite.py
+-rw-r--r--   0        0        0    21087 2020-02-02 00:00:00.000000 libgal-1.0.3/libgal/modules/Teradata.py
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 libgal-1.0.3/libgal/modules/Utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 libgal-1.0.3/libgal/modules/__init__.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 libgal-1.0.3/tests/CSVFileLoggerTests.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 libgal-1.0.3/tests/FileLoggerTests.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 libgal-1.0.3/tests/JSONFileLoggerTests.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 libgal-1.0.3/tests/LoggerTests.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 libgal-1.0.3/tests/SQLAlchemyTests.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 libgal-1.0.3/tests/SQliteTests.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 libgal-1.0.3/tests/TeradataBasicTest.py
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 libgal-1.0.3/tests/TeradataMLTests.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 libgal-1.0.3/tests/TestEvaluateKsAndRocAuc.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 libgal-1.0.3/tests/TestNumNormTransformer.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 libgal-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 libgal-1.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 libgal-1.0.3/README.md
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 libgal-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 libgal-1.0.3/PKG-INFO
```

### Comparing `libgal-1.0.2/docs/FSUtils.md` & `libgal-1.0.3/docs/FSUtils.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/docs/HTMLParser.md` & `libgal-1.0.3/docs/HTMLParser.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/docs/Installation.md` & `libgal-1.0.3/docs/Installation.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/docs/LoadEnv.md` & `libgal-1.0.3/docs/LoadEnv.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/docs/Logger.md` & `libgal-1.0.3/docs/Logger.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/docs/SQLAlchemy.md` & `libgal-1.0.3/docs/SQLAlchemy.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/docs/SQLMemory.md` & `libgal-1.0.3/docs/SQLMemory.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/docs/Selenium.md` & `libgal-1.0.3/docs/Selenium.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/docs/SimpleTeradata.md` & `libgal-1.0.3/docs/SimpleTeradata.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/docs/Teradata.md` & `libgal-1.0.3/docs/Teradata.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/docs/Utils.md` & `libgal-1.0.3/docs/Utils.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/docs/by_example/TeradataExamples.md` & `libgal-1.0.3/docs/by_example/TeradataExamples.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/libgal/__init__.py` & `libgal-1.0.3/libgal/__init__.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/libgal/modules/DatabaseAPI.py` & `libgal-1.0.3/libgal/modules/DatabaseAPI.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/libgal/modules/FSUtils.py` & `libgal-1.0.3/libgal/modules/FSUtils.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/libgal/modules/Logger.py` & `libgal-1.0.3/libgal/modules/Logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import logging
 import os
 import datetime
 from typing import Optional
+import unidecode
 
 DEFAULT_FILE_BUFFER_SIZE = 1024 * 1024  # 1 MB
 
 
 class SingletonType(type):
     _instances = {}
 
@@ -129,15 +130,15 @@
             now = datetime.datetime.now()
             for handler in self._logger.handlers:
                 if isinstance(handler, BufferingHandler):
                     handler.close()
                     self._logger.removeHandler(handler)
 
             file_handler = BufferingHandler(
-                dirname + f"/{self._app_name}_{os.getpid()}_" + now.strftime("%Y-%m-%d") + ".log", encoding='utf-8')
+                dirname + f"/{unidecode.unidecode(self._app_name).replace(' ','_').lower()}_{os.getpid()}_" + now.strftime("%Y-%m-%d") + ".log", encoding='utf-8')
             file_handler.setFormatter(formatter)
             self._logger.addHandler(file_handler)
         else:
             self._logger.warning("No se ha especificado un directorio de salida para los logs")
 
 
 # a simple usecase
```

### Comparing `libgal-1.0.2/libgal/modules/MLS.py` & `libgal-1.0.3/libgal/modules/MLS.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/libgal/modules/ODBCTools.py` & `libgal-1.0.3/libgal/modules/ODBCTools.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/libgal/modules/SQLAlchemy.py` & `libgal-1.0.3/libgal/modules/SQLAlchemy.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/libgal/modules/SQLMemory.py` & `libgal-1.0.3/libgal/modules/SQLMemory.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/libgal/modules/Sqlite.py` & `libgal-1.0.3/libgal/modules/Sqlite.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/libgal/modules/Teradata.py` & `libgal-1.0.3/libgal/modules/Teradata.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/libgal/modules/Utils.py` & `libgal-1.0.3/libgal/modules/Utils.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/tests/FileLoggerTests.py` & `libgal-1.0.3/tests/FileLoggerTests.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/tests/LoggerTests.py` & `libgal-1.0.3/tests/LoggerTests.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/tests/SQLAlchemyTests.py` & `libgal-1.0.3/tests/SQLAlchemyTests.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/tests/SQliteTests.py` & `libgal-1.0.3/tests/SQliteTests.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/tests/TeradataBasicTest.py` & `libgal-1.0.3/tests/TeradataBasicTest.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/tests/TeradataMLTests.py` & `libgal-1.0.3/tests/TeradataMLTests.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/tests/TestEvaluateKsAndRocAuc.py` & `libgal-1.0.3/tests/TestEvaluateKsAndRocAuc.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/tests/TestNumNormTransformer.py` & `libgal-1.0.3/tests/TestNumNormTransformer.py`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/LICENSE.txt` & `libgal-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/README.md` & `libgal-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `libgal-1.0.2/pyproject.toml` & `libgal-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel.force-include]
 "libgal/modules" = "libgal/modules"
 
 [project]
 name = "libgal"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Jean Manuel González Mejía", email="ebrainding@gmail.com" },
   { name="Julián Leandro Giraldez", email="juliangiraldez@outlook.com"},
   { name="Sebastian Wilwerth", email="sebastian.wilwerth@gmail.com" }
 ]
 
 license = { file = "LICENSE.txt" }
@@ -30,13 +30,14 @@
 	"Brotli",
     "python-dotenv>=0.10.2",
 	"bs4",
     "pandas==2.0.0",
     "numpy>=1.26.1",
     "teradataml>=17.20.0.6",
     "scikit-learn",
-    "pyodbc"
+    "pyodbc",
+    "unidecode"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jeanmgonzalez/libgal"
 "Bug Tracker" = "https://github.com/jeanmgonzalez/libgal/issues"
```

### Comparing `libgal-1.0.2/PKG-INFO` & `libgal-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: libgal
-Version: 1.0.2
+Version: 1.0.3
 Summary: Librería para la simplificación del código en diversos proyectos de Python
 Project-URL: Homepage, https://github.com/jeanmgonzalez/libgal
 Project-URL: Bug Tracker, https://github.com/jeanmgonzalez/libgal/issues
 Author-email: Jean Manuel González Mejía <ebrainding@gmail.com>, Julián Leandro Giraldez <juliangiraldez@outlook.com>, Sebastian Wilwerth <sebastian.wilwerth@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 JEAN MANUEL GONZÁLEZ MEJÍA
@@ -36,14 +36,15 @@
 Requires-Dist: numpy>=1.26.1
 Requires-Dist: pandas==2.0.0
 Requires-Dist: pyodbc
 Requires-Dist: python-dotenv>=0.10.2
 Requires-Dist: scikit-learn
 Requires-Dist: selenium>=4.0.0
 Requires-Dist: teradataml>=17.20.0.6
+Requires-Dist: unidecode
 Description-Content-Type: text/markdown
 
 # LibGal
 
 Librería para agilizar el desarrollo de productos de datos en Python.
 
 [Home](https://github.com/jeanmgonzalez/libgal)
```

