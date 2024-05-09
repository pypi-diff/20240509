# Comparing `tmp/wrapica-1.0.3.tar.gz` & `tmp/wrapica-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrapica-1.0.3.tar", last modified: Wed Mar 13 20:34:37 2024, max compression
+gzip compressed data, was "wrapica-1.0.4.tar", last modified: Thu May  9 08:45:29 2024, max compression
```

## Comparing `wrapica-1.0.3.tar` & `wrapica-1.0.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.748617 wrapica-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-13 20:34:19.000000 wrapica-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-13 20:34:37.744617 wrapica-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-03-13 20:34:19.000000 wrapica-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-13 20:34:19.000000 wrapica-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 20:34:37.748617 wrapica-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/wrapica/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/wrapica/enums/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/enums/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/wrapica/job/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/job/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/wrapica/job/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/job/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/job/functions/job_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/wrapica/libica_exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/libica_exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/wrapica/libica_models/
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/libica_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/wrapica/project/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/wrapica/project/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project/functions/project_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/wrapica/project_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/wrapica/project_analysis/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_analysis/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16255 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_analysis/functions/project_analyses_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/wrapica/project_data/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.740617 wrapica-1.0.3/src/wrapica/project_data/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_data/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62189 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_data/functions/project_data_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.744617 wrapica-1.0.3/src/wrapica/project_pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.744617 wrapica-1.0.3/src/wrapica/project_pipelines/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_pipelines/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20996 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_pipelines/classes/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_pipelines/classes/cwl_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    14742 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_pipelines/classes/nextflow_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.744617 wrapica-1.0.3/src/wrapica/project_pipelines/functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_pipelines/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40298 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/project_pipelines/functions/project_pipelines_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.744617 wrapica-1.0.3/src/wrapica/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/utils/miscell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/utils/subprocess_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/utils/user_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/utils/websocket_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-13 20:34:19.000000 wrapica-1.0.3/src/wrapica/utils/websocket_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 20:34:37.744617 wrapica-1.0.3/src/wrapica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-13 20:34:37.000000 wrapica-1.0.3/src/wrapica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-13 20:34:37.000000 wrapica-1.0.3/src/wrapica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 20:34:37.000000 wrapica-1.0.3/src/wrapica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-13 20:34:37.000000 wrapica-1.0.3/src/wrapica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-13 20:34:37.000000 wrapica-1.0.3/src/wrapica.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.942399 wrapica-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 08:45:14.000000 wrapica-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-09 08:45:29.942399 wrapica-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-09 08:45:14.000000 wrapica-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-09 08:45:14.000000 wrapica-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:45:29.942399 wrapica-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/wrapica/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/wrapica/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/enums/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/wrapica/job/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/job/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/wrapica/job/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/job/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/job/functions/job_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/wrapica/libica_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/libica_exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.934399 wrapica-1.0.4/src/wrapica/libica_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/libica_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project/functions/project_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_analysis/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_analysis/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16255 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_analysis/functions/project_analyses_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_data/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_data/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62189 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_data/functions/project_data_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_pipelines/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22147 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/classes/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/classes/cwl_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/classes/nextflow_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.938399 wrapica-1.0.4/src/wrapica/project_pipelines/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40164 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/project_pipelines/functions/project_pipelines_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.942399 wrapica-1.0.4/src/wrapica/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/miscell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/subprocess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/user_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/websocket_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-09 08:45:14.000000 wrapica-1.0.4/src/wrapica/utils/websocket_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:45:29.942399 wrapica-1.0.4/src/wrapica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-09 08:45:29.000000 wrapica-1.0.4/src/wrapica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-05-09 08:45:29.000000 wrapica-1.0.4/src/wrapica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:45:29.000000 wrapica-1.0.4/src/wrapica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-09 08:45:29.000000 wrapica-1.0.4/src/wrapica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 08:45:29.000000 wrapica-1.0.4/src/wrapica.egg-info/top_level.txt
```

### Comparing `wrapica-1.0.3/LICENSE` & `wrapica-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/PKG-INFO` & `wrapica-1.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapica
-Version: 1.0.3
+Version: 1.0.4
 Summary: Secondary level functions for ICAv2 based off libica
 Author-email: Alexis Lucattini <alexis.lucattini@umccr.org>
 Project-URL: Homepage, https://github.com/umccr/wrapica
 Project-URL: Bug Tracker, https://github.com/umccr/wrapica/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wrapica-1.0.3/README.md` & `wrapica-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/pyproject.toml` & `wrapica-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wrapica"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
     { name = "Alexis Lucattini", email = "alexis.lucattini@umccr.org" },
 ]
 description = "Secondary level functions for ICAv2 based off libica"
 readme = "Readme.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `wrapica-1.0.3/src/wrapica/enums/__init__.py` & `wrapica-1.0.4/src/wrapica/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/job/functions/job_functions.py` & `wrapica-1.0.4/src/wrapica/job/functions/job_functions.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/libica_models/__init__.py` & `wrapica-1.0.4/src/wrapica/libica_models/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/project/functions/project_functions.py` & `wrapica-1.0.4/src/wrapica/project/functions/project_functions.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/project_analysis/__init__.py` & `wrapica-1.0.4/src/wrapica/project_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/project_analysis/functions/project_analyses_functions.py` & `wrapica-1.0.4/src/wrapica/project_analysis/functions/project_analyses_functions.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/project_data/__init__.py` & `wrapica-1.0.4/src/wrapica/project_data/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/project_data/functions/project_data_functions.py` & `wrapica-1.0.4/src/wrapica/project_data/functions/project_data_functions.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/project_pipelines/__init__.py` & `wrapica-1.0.4/src/wrapica/project_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/project_pipelines/classes/analysis.py` & `wrapica-1.0.4/src/wrapica/project_pipelines/classes/analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -433,14 +433,15 @@
         analysis_storage_id: Optional[str] = None,
         analysis_storage_size: Optional[AnalysisStorageSize] = None,
         activation_id: Optional[str] = None,
         # Output parameters
         output_parent_folder_id: Optional[str] = None,
         output_parent_folder_path: Optional[str] = None,
         analysis_output_uri: Optional[str] = None,
+        ica_logs_uri: Optional[str] = None,
         # Meta parameters
         tags: Optional[ICAv2PipelineAnalysisTags] = None
     ):
         """
         Initialise parent analysis class with the following attributes
 
         * name / user-reference  # The analysis name - Required
@@ -459,28 +460,34 @@
         self.user_reference = user_reference
         self.project_id = project_id
         self.pipeline_id = pipeline_id
         self.activation_id = activation_id
         self.output_parent_folder_id = output_parent_folder_id
         self.output_parent_folder_path = output_parent_folder_path
         self.analysis_output_uri = analysis_output_uri
+        self.ica_logs_uri = ica_logs_uri
 
         # Meta parameters
         self.tags = tags
         self.analysis_storage_id = analysis_storage_id
         self.analysis_storage_size = analysis_storage_size
         self.analysis_input = analysis_input
 
         self.engine_parameters: Optional[ICAv2EngineParameters] = None
 
         if self.analysis_output_uri is not None:
             self.analysis_output: List[AnalysisOutputMapping] = [self.get_analysis_output_mapping_from_uri()]
         else:
             self.analysis_output = None
 
+        if self.ica_logs_uri is not None:
+            self.ica_logs: List[AnalysisOutputMapping] = [self.get_ica_logs_mapping_from_uri()]
+        else:
+            self.ica_logs = None
+
         self.set_engine_parameters()
 
         # Set the analysis
         self.analysis: Optional[Union[CreateCwlAnalysis, CreateNextflowAnalysis]] = None
 
     def __call__(self) -> Analysis:
         """
@@ -513,14 +520,32 @@
         return AnalysisOutputMapping(
             source_path="out/",  # Hardcoded, all workflow outputs should be placed in the out folder,
             type=DataType.FOLDER.value,  # Hardcoded, out directory is a folder
             target_project_id=analysis_output_obj.project_id,
             target_path=analysis_output_obj.data.details.path
         )
 
+    def get_ica_logs_mapping_from_uri(self) -> AnalysisOutputMapping:
+        from ...project_data import convert_icav2_uri_to_data_obj
+        # Ensure that the path attribute of analysis_output_uri ends with /
+        if not urlparse(self.ica_logs_uri).path.endswith("/"):
+            raise ValueError("The analysis output uri must end with a /")
+
+        ica_logs_project_data_obj: ProjectData = convert_icav2_uri_to_data_obj(
+            self.ica_logs_uri,
+            create_data_if_not_found=True
+        )
+
+        return AnalysisOutputMapping(
+            source_path="ica_logs/",  # Hardcoded, all logs should be placed in the ica_logs folder,
+            type=DataType.FOLDER.value,  # Hardcoded, out directory is a folder
+            target_project_id=ica_logs_project_data_obj.project_id,
+            target_path=ica_logs_project_data_obj.data.details.path
+        )
+
     def set_engine_parameters(self):
         """
         Implemented in subclass
         :return:
         """
         raise NotImplementedError
```

### Comparing `wrapica-1.0.3/src/wrapica/project_pipelines/classes/cwl_analysis.py` & `wrapica-1.0.4/src/wrapica/project_pipelines/classes/cwl_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,15 @@
         analysis_storage_id: Optional[str] = None,
         analysis_storage_size: Optional[AnalysisStorageSize] = None,
         activation_id: Optional[str] = None,
         # Output parameters
         output_parent_folder_id: Optional[str] = None,
         output_parent_folder_path: Optional[str] = None,
         analysis_output_uri: Optional[str] = None,
+        ica_logs_uri: Optional[str] = None,
         # Meta parameters
         tags: Optional[ICAv2PipelineAnalysisTags] = None,
         # CWL Specific parameters
         cwltool_overrides: Optional[Dict] = None
     ):
         """
         Initialise input
@@ -231,14 +232,15 @@
         :param analysis_input
         :param analysis_storage_id
         :param analysis_storage_size
         :param activation_id
         :param output_parent_folder_id
         :param output_parent_folder_path
         :param analysis_output_uri
+        :param ica_logs_uri
         :param tags
         :param cwltool_overrides
         """
         # Initialise any cwl specific parameters first before calling the parent class
         # Set cwl specific inputs
         self.cwltool_overrides: Optional[Dict] = cwltool_overrides
         # Set under parent init script through set_engine_parameters
@@ -252,14 +254,15 @@
             analysis_input=analysis_input,
             analysis_storage_id=analysis_storage_id,
             analysis_storage_size=analysis_storage_size,
             activation_id=activation_id,
             output_parent_folder_id=output_parent_folder_id,
             output_parent_folder_path=output_parent_folder_path,
             analysis_output_uri=analysis_output_uri,
+            ica_logs_uri=ica_logs_uri,
             tags=tags
         )
 
     def set_engine_parameters(self):
         self.engine_parameters = ICAv2CWLEngineParameters(
             project_id=self.project_id,
             pipeline_id=self.pipeline_id,
```

### Comparing `wrapica-1.0.3/src/wrapica/project_pipelines/classes/nextflow_analysis.py` & `wrapica-1.0.4/src/wrapica/project_pipelines/classes/nextflow_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,15 @@
         analysis_storage_id: Optional[str] = None,
         analysis_storage_size: Optional[AnalysisStorageSize] = None,
         activation_id: Optional[str] = None,
         # Output parameters
         output_parent_folder_id: Optional[str] = None,
         output_parent_folder_path: Optional[str] = None,
         analysis_output_uri: Optional[str] = None,
+        ica_logs_uri: Optional[str] = None,
         # Meta parameters
         tags: Optional[ICAv2PipelineAnalysisTags] = None,
         # CWL Specific parameters
         cwltool_overrides: Optional[Dict] = None
     ):
         """
         Initialise input
@@ -317,14 +318,15 @@
         :param analysis_input
         :param analysis_storage_id
         :param analysis_storage_size
         :param activation_id
         :param output_parent_folder_id
         :param output_parent_folder_path
         :param analysis_output_uri
+        :param ica_logs_uri
         :param tags
         :param cwltool_overrides
         """
         # Initialise any cwl specific parameters first before calling the parent class
         # Set cwl specific inputs
         self.cwltool_overrides: Optional[Dict] = cwltool_overrides
         # Set under parent init script through set_engine_parameters
@@ -338,14 +340,15 @@
             analysis_input=analysis_input,
             analysis_storage_id=analysis_storage_id,
             analysis_storage_size=analysis_storage_size,
             activation_id=activation_id,
             output_parent_folder_id=output_parent_folder_id,
             output_parent_folder_path=output_parent_folder_path,
             analysis_output_uri=analysis_output_uri,
+            ica_logs_uri=ica_logs_uri,
             tags=tags
         )
 
     def set_engine_parameters(self):
         self.engine_parameters = ICAv2NextflowEngineParameters(
             project_id=self.project_id,
             pipeline_id=self.pipeline_id,
```

### Comparing `wrapica-1.0.3/src/wrapica/project_pipelines/functions/project_pipelines_functions.py` & `wrapica-1.0.4/src/wrapica/project_pipelines/functions/project_pipelines_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -579,31 +579,30 @@
 
         # Save the analysis
         cwl_analysis.save_analysis(Path("/path/to/analysis.json"))
 
     """
     # Enter a context with an instance of the API client
     with ApiClient(get_icav2_configuration()) as api_client:
-        # Force default headers to v3
-        # FIXME https://github.com/umccr-illumina/ica_v2/issues/173
+        # Force default headers to v4
         api_client.set_default_header(
             header_name="Content-Type",
-            header_value="application/vnd.illumina.v3+json"
+            header_value="application/vnd.illumina.v4+json"
         )
         api_client.set_default_header(
             header_name="Accept",
-            header_value="application/vnd.illumina.v3+json"
+            header_value="application/vnd.illumina.v4+json"
         )
 
         # Create an instance of the API class
         api_instance = ProjectAnalysisApi(api_client)
 
-        # override endpoint settings response type to the version we want i.e. AnalysisV3 or Analysis
+        # override endpoint settings response type to the version we want i.e. AnalysisV3 or AnalysisV4
         endpoint_settings = api_instance.create_cwl_analysis_endpoint.settings
-        endpoint_settings['response_type'] = (AnalysisV3,)
+        endpoint_settings['response_type'] = (AnalysisV4,)
 
     # example passing only required values which don't have defaults set
     try:
         # Create and start an analysis for a CWL pipeline.
         api_response: Analysis = api_instance.create_cwl_analysis(
             project_id,
             cwl_analysis
@@ -665,36 +664,35 @@
 
         # Save the analysis
         nextflow_analysis.save_analysis(Path("/path/to/analysis.json"))
 
     """
     # Enter a context with an instance of the API client
     with ApiClient(get_icav2_configuration()) as api_client:
-        # Force default headers to v3
-        # FIXME https://github.com/umccr-illumina/ica_v2/issues/173
+        # Force default headers to v4
         api_client.set_default_header(
             header_name="Content-Type",
-            header_value="application/vnd.illumina.v3+json"
+            header_value="application/vnd.illumina.v4+json"
         )
         api_client.set_default_header(
             header_name="Accept",
-            header_value="application/vnd.illumina.v3+json"
+            header_value="application/vnd.illumina.v4+json"
         )
 
         # Create an instance of the API class
         api_instance = ProjectAnalysisApi(api_client)
 
         # override endpoint settings response type to the version we want i.e. AnalysisV3 or Analysis
         endpoint_settings = api_instance.create_nextflow_analysis_endpoint.settings
-        endpoint_settings['response_type'] = (AnalysisV3,)
+        endpoint_settings['response_type'] = (AnalysisV4,)
 
     # example passing only required values which don't have defaults set
     try:
         # Create and start an analysis for a CWL pipeline.
-        api_response: AnalysisV3 = api_instance.create_nextflow_analysis(
+        api_response: AnalysisV4 = api_instance.create_nextflow_analysis(
             project_id,
             nextflow_analysis
         )
     except ApiException as e:
         logger.error("Exception when calling ProjectAnalysisApi->create_nextflow_analysis: %s\n" % e)
         raise ApiException
```

### Comparing `wrapica-1.0.3/src/wrapica/utils/__init__.py` & `wrapica-1.0.4/src/wrapica/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/utils/configuration.py` & `wrapica-1.0.4/src/wrapica/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/utils/globals.py` & `wrapica-1.0.4/src/wrapica/utils/globals.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/utils/logger.py` & `wrapica-1.0.4/src/wrapica/utils/logger.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/utils/miscell.py` & `wrapica-1.0.4/src/wrapica/utils/miscell.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/utils/subprocess_handler.py` & `wrapica-1.0.4/src/wrapica/utils/subprocess_handler.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica/utils/websocket_helpers.py` & `wrapica-1.0.4/src/wrapica/utils/websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `wrapica-1.0.3/src/wrapica.egg-info/PKG-INFO` & `wrapica-1.0.4/src/wrapica.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wrapica
-Version: 1.0.3
+Version: 1.0.4
 Summary: Secondary level functions for ICAv2 based off libica
 Author-email: Alexis Lucattini <alexis.lucattini@umccr.org>
 Project-URL: Homepage, https://github.com/umccr/wrapica
 Project-URL: Bug Tracker, https://github.com/umccr/wrapica/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wrapica-1.0.3/src/wrapica.egg-info/SOURCES.txt` & `wrapica-1.0.4/src/wrapica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

