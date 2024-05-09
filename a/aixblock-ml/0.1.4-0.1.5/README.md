# Comparing `tmp/aixblock_ml-0.1.4.tar.gz` & `tmp/aixblock_ml-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aixblock_ml-0.1.4.tar", max compression
+gzip compressed data, was "aixblock_ml-0.1.5.tar", max compression
```

## Comparing `aixblock_ml-0.1.4.tar` & `aixblock_ml-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      331 2024-05-04 00:02:04.849352 aixblock_ml-0.1.4/README.md
--rw-r--r--   0        0        0       84 2024-05-04 01:42:25.778657 aixblock_ml-0.1.4/aixblock_ml/__init__.py
--rw-r--r--   0        0        0    10484 2024-04-15 02:31:16.790340 aixblock_ml-0.1.4/aixblock_ml/api.py
--rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.1.4/aixblock_ml/default_configs/Dockerfile
--rw-r--r--   0        0        0     2686 2024-04-15 02:26:57.535131 aixblock_ml-0.1.4/aixblock_ml/default_configs/README.md
--rw-r--r--   0        0        0     3854 2024-05-03 23:57:13.318089 aixblock_ml-0.1.4/aixblock_ml/default_configs/_wsgi.py
--rw-r--r--   0        0        0     3854 2024-04-04 03:08:16.489309 aixblock_ml-0.1.4/aixblock_ml/default_configs/_wsgi.py.tmpl
--rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.1.4/aixblock_ml/default_configs/docker-compose.yml
--rw-r--r--   0        0        0     1141 2024-05-04 00:29:14.036344 aixblock_ml-0.1.4/aixblock_ml/default_configs/model.py
--rw-r--r--   0        0        0      346 2024-05-04 01:19:58.591957 aixblock_ml-0.1.4/aixblock_ml/default_configs/requirements.txt
--rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.1.4/aixblock_ml/exceptions.py
--rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.1.4/aixblock_ml/helpers.py
--rw-r--r--   0        0        0    35738 2024-04-24 07:46:56.510948 aixblock_ml-0.1.4/aixblock_ml/model.py
--rw-r--r--   0        0        0     8777 2024-05-04 01:46:09.131725 aixblock_ml-0.1.4/aixblock_ml/server.py
--rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.1.4/aixblock_ml/templates/preview.html
--rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.1.4/aixblock_ml/utils.py
--rw-r--r--   0        0        0      325 2024-05-04 01:46:24.217738 aixblock_ml-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 aixblock_ml-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      331 2024-05-04 00:02:04.849352 aixblock_ml-0.1.5/README.md
+-rw-r--r--   0        0        0       84 2024-05-09 06:12:20.455945 aixblock_ml-0.1.5/aixblock_ml/__init__.py
+-rw-r--r--   0        0        0    10484 2024-04-15 02:31:16.790340 aixblock_ml-0.1.5/aixblock_ml/api.py
+-rw-r--r--   0        0        0      267 2024-04-01 06:20:49.118665 aixblock_ml-0.1.5/aixblock_ml/default_configs/Dockerfile
+-rw-r--r--   0        0        0     2686 2024-04-15 02:26:57.535131 aixblock_ml-0.1.5/aixblock_ml/default_configs/README.md
+-rw-r--r--   0        0        0     3353 2024-05-09 06:11:49.858213 aixblock_ml-0.1.5/aixblock_ml/default_configs/_wsgi.py
+-rw-r--r--   0        0        0     3351 2024-05-09 06:12:03.001107 aixblock_ml-0.1.5/aixblock_ml/default_configs/_wsgi.py.tmpl
+-rw-r--r--   0        0        0      559 2024-04-03 08:23:03.374688 aixblock_ml-0.1.5/aixblock_ml/default_configs/docker-compose.yml
+-rw-r--r--   0        0        0     1141 2024-05-04 00:29:14.036344 aixblock_ml-0.1.5/aixblock_ml/default_configs/model.py
+-rw-r--r--   0        0        0      350 2024-05-09 06:11:32.930550 aixblock_ml-0.1.5/aixblock_ml/default_configs/requirements.txt
+-rw-r--r--   0        0        0     1899 2024-04-01 06:20:49.123299 aixblock_ml-0.1.5/aixblock_ml/exceptions.py
+-rw-r--r--   0        0        0     2357 2024-04-01 06:43:06.660882 aixblock_ml-0.1.5/aixblock_ml/helpers.py
+-rw-r--r--   0        0        0    35738 2024-04-24 07:46:56.510948 aixblock_ml-0.1.5/aixblock_ml/model.py
+-rw-r--r--   0        0        0     8777 2024-05-04 01:46:09.131725 aixblock_ml-0.1.5/aixblock_ml/server.py
+-rw-r--r--   0        0        0        6 2024-04-01 06:20:49.127187 aixblock_ml-0.1.5/aixblock_ml/templates/preview.html
+-rw-r--r--   0        0        0     1987 2024-04-03 08:23:03.033057 aixblock_ml-0.1.5/aixblock_ml/utils.py
+-rw-r--r--   0        0        0      325 2024-05-09 06:12:14.402126 aixblock_ml-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 aixblock_ml-0.1.5/PKG-INFO
```

### Comparing `aixblock_ml-0.1.4/aixblock_ml/api.py` & `aixblock_ml-0.1.5/aixblock_ml/api.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.4/aixblock_ml/default_configs/README.md` & `aixblock_ml-0.1.5/aixblock_ml/default_configs/README.md`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.4/aixblock_ml/default_configs/_wsgi.py` & `aixblock_ml-0.1.5/aixblock_ml/default_configs/_wsgi.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,12 @@
 import os
 import argparse
 import logging
 import logging.config
 
-logging.config.dictConfig({{
-  "version": 1,
-  "formatters": {{
-    "standard": {{
-      "format": "[%(asctime)s] [%(levelname)s] [%(name)s::%(funcName)s::%(lineno)d] %(message)s"
-    }}
-  }},
-  "handlers": {{
-    "console": {{
-      "class": "logging.StreamHandler",
-      "level": "DEBUG",
-      "stream": "ext://sys.stdout",
-      "formatter": "standard"
-    }}
-  }},
-  "root": {{
-    "level": "ERROR",
-    "handlers": [
-      "console"
-    ],
-    "propagate": True
-  }}
-}})
 
 from aixblock_ml.api import init_app
 from {script} import {model_class}
 
 
 _DEFAULT_CONFIG_PATH = os.path.join(os.path.dirname(__file__), 'config.json')
```

### Comparing `aixblock_ml-0.1.4/aixblock_ml/default_configs/_wsgi.py.tmpl` & `aixblock_ml-0.1.5/aixblock_ml/default_configs/_wsgi.py.tmpl`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,12 @@
 import os
 import argparse
 import logging
 import logging.config
 
-logging.config.dictConfig({{
-  "version": 1,
-  "formatters": {{
-    "standard": {{
-      "format": "[%(asctime)s] [%(levelname)s] [%(name)s::%(funcName)s::%(lineno)d] %(message)s"
-    }}
-  }},
-  "handlers": {{
-    "console": {{
-      "class": "logging.StreamHandler",
-      "level": "DEBUG",
-      "stream": "ext://sys.stdout",
-      "formatter": "standard"
-    }}
-  }},
-  "root": {{
-    "level": "ERROR",
-    "handlers": [
-      "console"
-    ],
-    "propagate": True
-  }}
-}})
-
 from aixblock_ml.api import init_app
 from {script} import {model_class}
 
 
 _DEFAULT_CONFIG_PATH = os.path.join(os.path.dirname(__file__), 'config.json')
```

### Comparing `aixblock_ml-0.1.4/aixblock_ml/default_configs/docker-compose.yml` & `aixblock_ml-0.1.5/aixblock_ml/default_configs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.4/aixblock_ml/default_configs/model.py` & `aixblock_ml-0.1.5/aixblock_ml/default_configs/model.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.4/aixblock_ml/exceptions.py` & `aixblock_ml-0.1.5/aixblock_ml/exceptions.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.4/aixblock_ml/helpers.py` & `aixblock_ml-0.1.5/aixblock_ml/helpers.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.4/aixblock_ml/model.py` & `aixblock_ml-0.1.5/aixblock_ml/model.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.4/aixblock_ml/server.py` & `aixblock_ml-0.1.5/aixblock_ml/server.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.4/aixblock_ml/utils.py` & `aixblock_ml-0.1.5/aixblock_ml/utils.py`

 * *Files identical despite different names*

### Comparing `aixblock_ml-0.1.4/PKG-INFO` & `aixblock_ml-0.1.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aixblock_ml
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: TonyShark
 Author-email: quoi@wow-ai.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

