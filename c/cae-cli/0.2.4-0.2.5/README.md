# Comparing `tmp/cae_cli-0.2.4.tar.gz` & `tmp/cae_cli-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.2.4.tar", last modified: Thu May  9 02:16:29 2024, max compression
+gzip compressed data, was "cae_cli-0.2.5.tar", last modified: Thu May  9 02:19:51 2024, max compression
```

## Comparing `cae_cli-0.2.4.tar` & `cae_cli-0.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 02:16:29.323389 cae_cli-0.2.4/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.4/LICENSE
--rw-rw-rw-   0        0        0      415 2024-05-09 02:16:29.323389 cae_cli-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 02:16:29.284330 cae_cli-0.2.4/cae/
--rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.2.4/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.4/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.4/cae/__init__.py
--rw-rw-rw-   0        0        0     8485 2024-05-09 01:09:21.000000 cae_cli-0.2.4/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-09 02:16:29.304147 cae_cli-0.2.4/cae/templates/
--rw-rw-rw-   0        0        0     1021 2024-05-09 02:10:39.000000 cae_cli-0.2.4/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.4/cae/templates/entity.txt
--rw-rw-rw-   0        0        0      730 2024-05-09 02:13:43.000000 cae_cli-0.2.4/cae/templates/entityFactory.txt
--rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.4/cae/templates/entityImplementation.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.4/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.4/cae/templates/implementation_ruc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.4/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.4/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.4/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.2.4/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.4/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.2.4/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.4/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.4/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.4/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      308 2024-05-09 01:56:52.000000 cae_cli-0.2.4/cae/templates/use_case_ruc.txt
--rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.2.4/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 02:16:29.322382 cae_cli-0.2.4/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      415 2024-05-09 02:16:29.000000 cae_cli-0.2.4/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      797 2024-05-09 02:16:29.000000 cae_cli-0.2.4/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 02:16:29.000000 cae_cli-0.2.4/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-09 02:16:29.000000 cae_cli-0.2.4/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-09 02:16:29.000000 cae_cli-0.2.4/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 02:16:29.324387 cae_cli-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      610 2024-05-09 02:16:27.000000 cae_cli-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:19:51.021281 cae_cli-0.2.5/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      415 2024-05-09 02:19:51.018765 cae_cli-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 02:19:50.957539 cae_cli-0.2.5/cae/
+-rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.2.5/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.5/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.5/cae/__init__.py
+-rw-rw-rw-   0        0        0     8459 2024-05-09 02:19:46.000000 cae_cli-0.2.5/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-09 02:19:51.002185 cae_cli-0.2.5/cae/templates/
+-rw-rw-rw-   0        0        0     1021 2024-05-09 02:10:39.000000 cae_cli-0.2.5/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.5/cae/templates/entity.txt
+-rw-rw-rw-   0        0        0      730 2024-05-09 02:13:43.000000 cae_cli-0.2.5/cae/templates/entityFactory.txt
+-rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.5/cae/templates/entityImplementation.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.5/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.5/cae/templates/implementation_ruc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.5/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.5/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.5/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.2.5/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.5/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.2.5/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.5/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.5/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.5/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      308 2024-05-09 01:56:52.000000 cae_cli-0.2.5/cae/templates/use_case_ruc.txt
+-rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.2.5/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 02:19:51.018765 cae_cli-0.2.5/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-05-09 02:19:50.000000 cae_cli-0.2.5/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2024-05-09 02:19:50.000000 cae_cli-0.2.5/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 02:19:50.000000 cae_cli-0.2.5/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-09 02:19:50.000000 cae_cli-0.2.5/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-09 02:19:50.000000 cae_cli-0.2.5/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 02:19:51.021281 cae_cli-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      610 2024-05-09 02:19:46.000000 cae_cli-0.2.5/setup.py
```

### Comparing `cae_cli-0.2.4/LICENSE` & `cae_cli-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/README.md` & `cae_cli-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/cae/ArchFlowJavaWeb.py` & `cae_cli-0.2.5/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/cae/db.json` & `cae_cli-0.2.5/cae/db.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981060606060606%*

 * *Differences: {"'functions'": "{'function_core_layer': {'steps': {2: {'create_folder': "*

 * *                "['implementations/mappers']}}}, 'core_basic_dir': {'steps': {1: {'create_folder': "*

 * *                "['implementations/ports']}}}}"}*

```diff
@@ -70,15 +70,15 @@
                 {
                     "create_folder": [
                         "implementations"
                     ]
                 },
                 {
                     "create_folder": [
-                        "implementations/dependencies/ports"
+                        "implementations/ports"
                     ]
                 },
                 {
                     "create_folder": [
                         "io"
                     ]
                 }
@@ -136,15 +136,15 @@
                     ]
                 },
                 {
                     "core_basic_dir": "None"
                 },
                 {
                     "create_folder": [
-                        "implementations/dependencies/mappers"
+                        "implementations/mappers"
                     ]
                 }
             ]
         },
         "install": {
             "steps": [
                 {
```

### Comparing `cae_cli-0.2.4/cae/templates/assembler.txt` & `cae_cli-0.2.5/cae/templates/assembler.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/cae/templates/entityFactory.txt` & `cae_cli-0.2.5/cae/templates/entityFactory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/cae/templates/implementation_cuc.txt` & `cae_cli-0.2.5/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/cae/templates/implementation_ruc.txt` & `cae_cli-0.2.5/cae/templates/implementation_ruc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/cae/templates/implementation_suc.txt` & `cae_cli-0.2.5/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/cae/templates/pom-adapters.txt` & `cae_cli-0.2.5/cae/templates/pom-adapters.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/cae/templates/pom-assemblers.txt` & `cae_cli-0.2.5/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/cae/templates/pom-core.txt` & `cae_cli-0.2.5/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/cae/templates/use_case.txt` & `cae_cli-0.2.5/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/cae/templates/use_case_implementation.txt` & `cae_cli-0.2.5/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.2.5/cae_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.4/setup.py` & `cae_cli-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.2.4',
+    version='0.2.5',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
```

