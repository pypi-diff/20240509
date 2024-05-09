# Comparing `tmp/cae_cli-0.2.5.tar.gz` & `tmp/cae_cli-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.2.5.tar", last modified: Thu May  9 02:19:51 2024, max compression
+gzip compressed data, was "cae_cli-0.2.6.tar", last modified: Thu May  9 02:35:21 2024, max compression
```

## Comparing `cae_cli-0.2.5.tar` & `cae_cli-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 02:19:51.021281 cae_cli-0.2.5/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      415 2024-05-09 02:19:51.018765 cae_cli-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 02:19:50.957539 cae_cli-0.2.5/cae/
--rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.2.5/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.5/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.5/cae/__init__.py
--rw-rw-rw-   0        0        0     8459 2024-05-09 02:19:46.000000 cae_cli-0.2.5/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-09 02:19:51.002185 cae_cli-0.2.5/cae/templates/
--rw-rw-rw-   0        0        0     1021 2024-05-09 02:10:39.000000 cae_cli-0.2.5/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.5/cae/templates/entity.txt
--rw-rw-rw-   0        0        0      730 2024-05-09 02:13:43.000000 cae_cli-0.2.5/cae/templates/entityFactory.txt
--rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.5/cae/templates/entityImplementation.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.5/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.5/cae/templates/implementation_ruc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.5/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.5/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.5/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.2.5/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.5/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.2.5/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.5/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.5/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.5/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      308 2024-05-09 01:56:52.000000 cae_cli-0.2.5/cae/templates/use_case_ruc.txt
--rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.2.5/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 02:19:51.018765 cae_cli-0.2.5/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      415 2024-05-09 02:19:50.000000 cae_cli-0.2.5/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      797 2024-05-09 02:19:50.000000 cae_cli-0.2.5/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 02:19:50.000000 cae_cli-0.2.5/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-09 02:19:50.000000 cae_cli-0.2.5/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-09 02:19:50.000000 cae_cli-0.2.5/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 02:19:51.021281 cae_cli-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0      610 2024-05-09 02:19:46.000000 cae_cli-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:35:21.436765 cae_cli-0.2.6/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      415 2024-05-09 02:35:21.435760 cae_cli-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 02:35:21.397226 cae_cli-0.2.6/cae/
+-rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.2.6/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.6/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.6/cae/__init__.py
+-rw-rw-rw-   0        0        0     8459 2024-05-09 02:22:16.000000 cae_cli-0.2.6/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-09 02:35:21.417067 cae_cli-0.2.6/cae/templates/
+-rw-rw-rw-   0        0        0     1174 2024-05-09 02:34:53.000000 cae_cli-0.2.6/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.6/cae/templates/entity.txt
+-rw-rw-rw-   0        0        0      770 2024-05-09 02:30:03.000000 cae_cli-0.2.6/cae/templates/entityFactory.txt
+-rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.6/cae/templates/entityImplementation.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.6/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.6/cae/templates/implementation_ruc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.6/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.6/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.6/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.2.6/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.6/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-09 02:30:03.000000 cae_cli-0.2.6/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.6/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.6/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.6/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      236 2024-05-09 02:34:53.000000 cae_cli-0.2.6/cae/templates/use_case_ruc.txt
+-rw-rw-rw-   0        0        0      408 2024-05-09 02:34:53.000000 cae_cli-0.2.6/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 02:35:21.434758 cae_cli-0.2.6/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-05-09 02:35:21.000000 cae_cli-0.2.6/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2024-05-09 02:35:21.000000 cae_cli-0.2.6/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 02:35:21.000000 cae_cli-0.2.6/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-09 02:35:21.000000 cae_cli-0.2.6/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-09 02:35:21.000000 cae_cli-0.2.6/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 02:35:21.436765 cae_cli-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      610 2024-05-09 02:34:53.000000 cae_cli-0.2.6/setup.py
```

### Comparing `cae_cli-0.2.5/LICENSE` & `cae_cli-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.5/README.md` & `cae_cli-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.5/cae/ArchFlowJavaWeb.py` & `cae_cli-0.2.6/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.5/cae/db.json` & `cae_cli-0.2.6/cae/db.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9565217391304348%*

 * *Differences: {"'functions'": "{'clean': OrderedDict([('steps', [OrderedDict([('clear_layer', ['core'])]), "*

 * *                "OrderedDict([('clear_layer', ['adapters'])]), OrderedDict([('clear_layer', "*

 * *                "['assemblers'])])])]), delete: ['clear']}"}*

```diff
@@ -20,15 +20,15 @@
                     "clear_all": "None"
                 },
                 {
                     "install_all": "None"
                 }
             ]
         },
-        "clear": {
+        "clean": {
             "steps": [
                 {
                     "clear_layer": [
                         "core"
                     ]
                 },
                 {
```

### Comparing `cae_cli-0.2.5/cae/templates/assembler.txt` & `cae_cli-0.2.6/cae/templates/assembler.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 package <pk><group_id></group_id>.<artifact_id_sem_core></artifact_id_sem_core></pk>.assemblers.use_cases.<sc>args[0]</sc>;
 
 import com.cae.use_cases.assemblers.UseCaseAssembler;
 import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.<pc>args[0]</pc>UseCase;
+import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.implementations.<pc>args[0]</pc>UseCaseCaseImplementation;
 import lombok.AccessLevel;
 import lombok.NoArgsConstructor;
 
 @NoArgsConstructor(access = AccessLevel.PRIVATE)
 public class <pc>args[0]</pc>UseCaseAssembler implements UseCaseAssembler<<pc>args[0]</pc>UseCase>{
 
     public static final <pc>args[0]</pc>UseCaseAssembler SINGLETON_ASSEMBLER = new <pc>args[0]</pc>UseCaseAssembler();
```

### Comparing `cae_cli-0.2.5/cae/templates/entityFactory.txt` & `cae_cli-0.2.6/cae/templates/entityFactory.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 package <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.entities.factories;
 
 import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.entities.<pc>args[0]</pc>;
 import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.entities.implementations.<pc>args[0]</pc>Implementation;
 import lombok.AccessLevel;
+import com.cae.entities.EntityFactory;
 import lombok.NoArgsConstructor;
 
 @NoArgsConstructor(access = AccessLevel.PRIVATE)
 public class <pc>args[0]</pc>Factory implements EntityFactory<<pc>args[0]</pc>> {
 
     public static final <pc>args[0]</pc>Factory SINGLETON = new <pc>args[0]</pc>Factory();
```

### Comparing `cae_cli-0.2.5/cae/templates/implementation_cuc.txt` & `cae_cli-0.2.6/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.5/cae/templates/implementation_ruc.txt` & `cae_cli-0.2.6/cae/templates/implementation_ruc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.5/cae/templates/implementation_suc.txt` & `cae_cli-0.2.6/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.5/cae/templates/pom-adapters.txt` & `cae_cli-0.2.6/cae/templates/pom-adapters.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.5/cae/templates/pom-assemblers.txt` & `cae_cli-0.2.6/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.5/cae/templates/pom-core.txt` & `cae_cli-0.2.6/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.5/cae/templates/use_case.txt` & `cae_cli-0.2.6/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.5/cae/templates/use_case_implementation.txt` & `cae_cli-0.2.6/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.5/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.2.6/cae_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.5/setup.py` & `cae_cli-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.2.5',
+    version='0.2.6',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
```

