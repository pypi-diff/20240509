# Comparing `tmp/FoccoERPy-0.3.0.tar.gz` & `tmp/foccoerpy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FoccoERPy-0.3.0.tar", last modified: Fri Apr 12 14:00:46 2024, max compression
+gzip compressed data, was "foccoerpy-0.3.1.tar", last modified: Thu May  9 17:47:19 2024, max compression
```

## Comparing `FoccoERPy-0.3.0.tar` & `foccoerpy-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy/Focco/
--rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/FoccoERPy/Focco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy/FoccoSession/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/FoccoERPy/FoccoSession/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/FoccoERPy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/FoccoERPy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/FoccoERPy/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/FoccoERPy/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/FoccoERPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-12 14:00:45.000000 FoccoERPy-0.3.0/FoccoERPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-12 14:00:45.000000 FoccoERPy-0.3.0/FoccoERPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 14:00:45.000000 FoccoERPy-0.3.0/FoccoERPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 14:00:45.000000 FoccoERPy-0.3.0/FoccoERPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 14:00:45.000000 FoccoERPy-0.3.0/FoccoERPy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-12 14:00:41.000000 FoccoERPy-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 14:00:45.998744 FoccoERPy-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:47:19.627676 foccoerpy-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:47:19.623676 foccoerpy-0.3.1/FoccoERPy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:47:19.627676 foccoerpy-0.3.1/FoccoERPy/Focco/
+-rw-r--r--   0 runner    (1001) docker     (127)     7640 2024-05-09 17:47:14.000000 foccoerpy-0.3.1/FoccoERPy/Focco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:47:19.627676 foccoerpy-0.3.1/FoccoERPy/FoccoSession/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-09 17:47:14.000000 foccoerpy-0.3.1/FoccoERPy/FoccoSession/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 17:47:14.000000 foccoerpy-0.3.1/FoccoERPy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:47:19.627676 foccoerpy-0.3.1/FoccoERPy/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-09 17:47:14.000000 foccoerpy-0.3.1/FoccoERPy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:47:19.627676 foccoerpy-0.3.1/FoccoERPy/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-09 17:47:14.000000 foccoerpy-0.3.1/FoccoERPy/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:47:19.627676 foccoerpy-0.3.1/FoccoERPy/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-09 17:47:14.000000 foccoerpy-0.3.1/FoccoERPy/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 17:47:19.627676 foccoerpy-0.3.1/FoccoERPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 17:47:19.000000 foccoerpy-0.3.1/FoccoERPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-09 17:47:19.000000 foccoerpy-0.3.1/FoccoERPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 17:47:19.000000 foccoerpy-0.3.1/FoccoERPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 17:47:19.000000 foccoerpy-0.3.1/FoccoERPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 17:47:19.000000 foccoerpy-0.3.1/FoccoERPy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-09 17:47:14.000000 foccoerpy-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 17:47:19.627676 foccoerpy-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-09 17:47:14.000000 foccoerpy-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-09 17:47:14.000000 foccoerpy-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 17:47:19.627676 foccoerpy-0.3.1/setup.cfg
```

### Comparing `FoccoERPy-0.3.0/FoccoERPy/Focco/__init__.py` & `foccoerpy-0.3.1/FoccoERPy/Focco/__init__.py`

 * *Files identical despite different names*

### Comparing `FoccoERPy-0.3.0/FoccoERPy/FoccoSession/__init__.py` & `foccoerpy-0.3.1/FoccoERPy/FoccoSession/__init__.py`

 * *Files identical despite different names*

### Comparing `FoccoERPy-0.3.0/FoccoERPy/core/__init__.py` & `foccoerpy-0.3.1/FoccoERPy/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,28 +49,31 @@
 
     return resposta_focco
 
 def apontamento_tempo_padrao(
         session: FoccoSession,
         id_ordem_roteiro: int,
         quantidade: float,
-        data: datetime = datetime.now(),
+        data: Optional[datetime] = None,
         finalizar: bool = False,
         id_tipo_apontamento: str = 'TP',
         origem_apontamento: str = 'API',
         usuario: str = 'Apontamento API GTRP',
         id_funcionario: Optional[int] = None,
         id_recurso: Optional[int] = None,
     ):
     """
         Apontamento por tempo padrão
     """
 
     PATH = 'api/Entities/Manufatura.Producao.Apontamento.ApontamentoProducao'
 
+    if data is None:
+        data = datetime.now()
+
     BODY = {
         'OrdemRoteiro': {
             'ID': id_ordem_roteiro
         },
         'Quantidade': quantidade,
         'DataApontamento': data.isoformat(),
         'TipoApontamento': {
```

### Comparing `FoccoERPy-0.3.0/FoccoERPy/exceptions/__init__.py` & `foccoerpy-0.3.1/FoccoERPy/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `FoccoERPy-0.3.0/FoccoERPy/handlers/__init__.py` & `foccoerpy-0.3.1/FoccoERPy/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `FoccoERPy-0.3.0/FoccoERPy.egg-info/PKG-INFO` & `foccoerpy-0.3.1/FoccoERPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FoccoERPy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Biblioteca de funções que permitem se conectar à API do FoccoERP 
 Author-email: Gabriel Niziolek <ganiziolek@gmail.com>
 Project-URL: Homepage, https://github.com/GaNiziolek/FoccoERPy
 Project-URL: Bug Tracker, https://github.com/GaNiziolek/FoccoERPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FoccoERPy-0.3.0/LICENSE` & `foccoerpy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FoccoERPy-0.3.0/PKG-INFO` & `foccoerpy-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FoccoERPy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Biblioteca de funções que permitem se conectar à API do FoccoERP 
 Author-email: Gabriel Niziolek <ganiziolek@gmail.com>
 Project-URL: Homepage, https://github.com/GaNiziolek/FoccoERPy
 Project-URL: Bug Tracker, https://github.com/GaNiziolek/FoccoERPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `FoccoERPy-0.3.0/pyproject.toml` & `foccoerpy-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FoccoERPy"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="Gabriel Niziolek", email="ganiziolek@gmail.com" },
 ]
 description = "Biblioteca de funções que permitem se conectar à API do FoccoERP "
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

