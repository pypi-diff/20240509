# Comparing `tmp/cae_cli-0.2.1.tar.gz` & `tmp/cae_cli-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.2.1.tar", last modified: Wed May  8 23:51:43 2024, max compression
+gzip compressed data, was "cae_cli-0.2.2.tar", last modified: Thu May  9 00:05:08 2024, max compression
```

## Comparing `cae_cli-0.2.1.tar` & `cae_cli-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 23:51:43.457706 cae_cli-0.2.1/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      415 2024-05-08 23:51:43.456706 cae_cli-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 23:51:43.415653 cae_cli-0.2.1/cae/
--rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.2.1/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.1/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.1/cae/__init__.py
--rw-rw-rw-   0        0        0     8952 2024-05-08 23:38:55.000000 cae_cli-0.2.1/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-08 23:51:43.437677 cae_cli-0.2.1/cae/templates/
--rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.2.1/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.1/cae/templates/dependency_wrapper.txt
--rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.1/cae/templates/entity.txt
--rw-rw-rw-   0        0        0      584 2024-05-07 21:04:05.000000 cae_cli-0.2.1/cae/templates/entityFactory.txt
--rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.1/cae/templates/entityImplementation.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.1/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      463 2024-05-08 23:15:42.000000 cae_cli-0.2.1/cae/templates/implementation_ruc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.1/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.1/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.1/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.2.1/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.1/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.2.1/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.1/cae/templates/use_case_factory.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.1/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.1/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.1/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      353 2024-05-08 23:10:54.000000 cae_cli-0.2.1/cae/templates/use_case_ruc.txt
--rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.2.1/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 23:51:43.455706 cae_cli-0.2.1/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      415 2024-05-08 23:51:43.000000 cae_cli-0.2.1/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      869 2024-05-08 23:51:43.000000 cae_cli-0.2.1/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 23:51:43.000000 cae_cli-0.2.1/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-08 23:51:43.000000 cae_cli-0.2.1/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-08 23:51:43.000000 cae_cli-0.2.1/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 23:51:43.457706 cae_cli-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      610 2024-05-08 23:50:44.000000 cae_cli-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 00:05:08.551187 cae_cli-0.2.2/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      415 2024-05-09 00:05:08.549915 cae_cli-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 00:05:08.511855 cae_cli-0.2.2/cae/
+-rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.2.2/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.2/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.2/cae/__init__.py
+-rw-rw-rw-   0        0        0     8965 2024-05-09 00:05:06.000000 cae_cli-0.2.2/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-09 00:05:08.536404 cae_cli-0.2.2/cae/templates/
+-rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.2.2/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.2/cae/templates/dependency_wrapper.txt
+-rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.2/cae/templates/entity.txt
+-rw-rw-rw-   0        0        0      584 2024-05-07 21:04:05.000000 cae_cli-0.2.2/cae/templates/entityFactory.txt
+-rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.2/cae/templates/entityImplementation.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.2/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      463 2024-05-08 23:15:42.000000 cae_cli-0.2.2/cae/templates/implementation_ruc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.2/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.2/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.2/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.2.2/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.2/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.2.2/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.2/cae/templates/use_case_factory.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.2/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.2/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.2/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      353 2024-05-08 23:10:54.000000 cae_cli-0.2.2/cae/templates/use_case_ruc.txt
+-rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.2.2/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 00:05:08.548917 cae_cli-0.2.2/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-05-09 00:05:08.000000 cae_cli-0.2.2/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      869 2024-05-09 00:05:08.000000 cae_cli-0.2.2/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 00:05:08.000000 cae_cli-0.2.2/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-09 00:05:08.000000 cae_cli-0.2.2/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-09 00:05:08.000000 cae_cli-0.2.2/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 00:05:08.551187 cae_cli-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      610 2024-05-09 00:05:06.000000 cae_cli-0.2.2/setup.py
```

### Comparing `cae_cli-0.2.1/LICENSE` & `cae_cli-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/README.md` & `cae_cli-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/cae/ArchFlowJavaWeb.py` & `cae_cli-0.2.2/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/cae/db.json` & `cae_cli-0.2.2/cae/db.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990530303030303%*

 * *Differences: {"'functions'": "{'new_project': {'steps': {0: {'new_layer': {insert: [(4, "*

 * *                "'<pk>args[1].args[2].core</pk>.use_cases')], delete: [4]}}, 1: {'new_layer': "*

 * *                "{insert: [(4, '<pk>args[1].args[2].adapters</pk>.use_cases')], delete: [4]}}, 2: "*

 * *                "{'new_layer': {insert: [(4, '<pk>args[1].args[2].assemblers</pk>.use_cases')], "*

 * *                'delete: [4]}}}}}'}*

```diff
@@ -460,33 +460,33 @@
             "steps": [
                 {
                     "new_layer": [
                         "args[1]",
                         "args[2]",
                         "core",
                         "-core",
-                        "args[1].args[2].core.use_cases"
+                        "<pk>args[1].args[2].core</pk>.use_cases"
                     ]
                 },
                 {
                     "new_layer": [
                         "args[1]",
                         "args[2]",
                         "adaptadores",
                         "-adapters",
-                        "args[1].args[2].adapters.use_cases"
+                        "<pk>args[1].args[2].adapters</pk>.use_cases"
                     ]
                 },
                 {
                     "new_layer": [
                         "args[1]",
                         "args[2]",
                         "montadores",
                         "-assemblers",
-                        "args[1].args[2].assemblers.use_cases"
+                        "<pk>args[1].args[2].assemblers</pk>.use_cases"
                     ]
                 }
             ]
         },
         "new_ruc": {
             "steps": [
                 {
```

### Comparing `cae_cli-0.2.1/cae/templates/assembler.txt` & `cae_cli-0.2.2/cae/templates/assembler.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/cae/templates/entityFactory.txt` & `cae_cli-0.2.2/cae/templates/entityFactory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/cae/templates/implementation_cuc.txt` & `cae_cli-0.2.2/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/cae/templates/implementation_suc.txt` & `cae_cli-0.2.2/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/cae/templates/pom-adapters.txt` & `cae_cli-0.2.2/cae/templates/pom-adapters.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/cae/templates/pom-assemblers.txt` & `cae_cli-0.2.2/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/cae/templates/pom-core.txt` & `cae_cli-0.2.2/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/cae/templates/use_case.txt` & `cae_cli-0.2.2/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/cae/templates/use_case_factory.txt` & `cae_cli-0.2.2/cae/templates/use_case_factory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/cae/templates/use_case_implementation.txt` & `cae_cli-0.2.2/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.2.2/cae_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.1/setup.py` & `cae_cli-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.2.1',
+    version='0.2.2',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
```

