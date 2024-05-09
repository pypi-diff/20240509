# Comparing `tmp/cae_cli-0.2.2.tar.gz` & `tmp/cae_cli-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.2.2.tar", last modified: Thu May  9 00:05:08 2024, max compression
+gzip compressed data, was "cae_cli-0.2.3.tar", last modified: Thu May  9 01:12:38 2024, max compression
```

## Comparing `cae_cli-0.2.2.tar` & `cae_cli-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 00:05:08.551187 cae_cli-0.2.2/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      415 2024-05-09 00:05:08.549915 cae_cli-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 00:05:08.511855 cae_cli-0.2.2/cae/
--rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.2.2/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.2/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.2/cae/__init__.py
--rw-rw-rw-   0        0        0     8965 2024-05-09 00:05:06.000000 cae_cli-0.2.2/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-09 00:05:08.536404 cae_cli-0.2.2/cae/templates/
--rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.2.2/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.2/cae/templates/dependency_wrapper.txt
--rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.2/cae/templates/entity.txt
--rw-rw-rw-   0        0        0      584 2024-05-07 21:04:05.000000 cae_cli-0.2.2/cae/templates/entityFactory.txt
--rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.2/cae/templates/entityImplementation.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.2/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      463 2024-05-08 23:15:42.000000 cae_cli-0.2.2/cae/templates/implementation_ruc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.2/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.2/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.2/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.2.2/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.2/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.2.2/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.2/cae/templates/use_case_factory.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.2/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.2/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.2/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      353 2024-05-08 23:10:54.000000 cae_cli-0.2.2/cae/templates/use_case_ruc.txt
--rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.2.2/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 00:05:08.548917 cae_cli-0.2.2/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      415 2024-05-09 00:05:08.000000 cae_cli-0.2.2/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      869 2024-05-09 00:05:08.000000 cae_cli-0.2.2/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 00:05:08.000000 cae_cli-0.2.2/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-09 00:05:08.000000 cae_cli-0.2.2/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-09 00:05:08.000000 cae_cli-0.2.2/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 00:05:08.551187 cae_cli-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      610 2024-05-09 00:05:06.000000 cae_cli-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 01:12:38.136301 cae_cli-0.2.3/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      415 2024-05-09 01:12:38.135303 cae_cli-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 01:12:38.098231 cae_cli-0.2.3/cae/
+-rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.2.3/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.3/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.3/cae/__init__.py
+-rw-rw-rw-   0        0        0     8485 2024-05-09 01:09:21.000000 cae_cli-0.2.3/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-09 01:12:38.120258 cae_cli-0.2.3/cae/templates/
+-rw-rw-rw-   0        0        0      613 2024-05-09 01:12:33.000000 cae_cli-0.2.3/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.3/cae/templates/dependency_wrapper.txt
+-rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.3/cae/templates/entity.txt
+-rw-rw-rw-   0        0        0      584 2024-05-07 21:04:05.000000 cae_cli-0.2.3/cae/templates/entityFactory.txt
+-rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.3/cae/templates/entityImplementation.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.3/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      463 2024-05-08 23:15:42.000000 cae_cli-0.2.3/cae/templates/implementation_ruc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.3/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.3/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.3/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.2.3/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.3/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.2.3/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.3/cae/templates/use_case_factory.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.3/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.3/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.3/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      353 2024-05-08 23:10:54.000000 cae_cli-0.2.3/cae/templates/use_case_ruc.txt
+-rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.2.3/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 01:12:38.134299 cae_cli-0.2.3/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-05-09 01:12:38.000000 cae_cli-0.2.3/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      869 2024-05-09 01:12:38.000000 cae_cli-0.2.3/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 01:12:38.000000 cae_cli-0.2.3/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-09 01:12:38.000000 cae_cli-0.2.3/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-09 01:12:38.000000 cae_cli-0.2.3/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 01:12:38.136301 cae_cli-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      610 2024-05-09 01:12:33.000000 cae_cli-0.2.3/setup.py
```

### Comparing `cae_cli-0.2.2/LICENSE` & `cae_cli-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/README.md` & `cae_cli-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/cae/ArchFlowJavaWeb.py` & `cae_cli-0.2.3/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/cae/db.json` & `cae_cli-0.2.3/cae/db.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954545454545454%*

 * *Differences: {"'functions'": "{'function_core_layer': {'steps': {delete: [4, 3]}}, 'core_basic_dir': {'steps': "*

 * *                '{delete: [1, 0]}}}'}*

```diff
@@ -65,24 +65,14 @@
                 }
             ]
         },
         "core_basic_dir": {
             "steps": [
                 {
                     "create_folder": [
-                        "factories"
-                    ]
-                },
-                {
-                    "create_folder": [
-                        "factories/dependency_wrapper"
-                    ]
-                },
-                {
-                    "create_folder": [
                         "implementations"
                     ]
                 },
                 {
                     "create_folder": [
                         "implementations/dependencies/ports"
                     ]
@@ -148,34 +138,14 @@
                 {
                     "core_basic_dir": "None"
                 },
                 {
                     "create_folder": [
                         "implementations/dependencies/mappers"
                     ]
-                },
-                {
-                    "create_file_based_in_template": [
-                        "factories/",
-                        "<pc>args[1] use case factory</pc>.java",
-                        "use_case_factory.txt",
-                        [
-                            "args[1]"
-                        ]
-                    ]
-                },
-                {
-                    "create_file_based_in_template": [
-                        "factories/dependency_wrapper/",
-                        "<pc>args[1] use case dependency wrapper</pc>.java",
-                        "dependency_wrapper.txt",
-                        [
-                            "args[1]"
-                        ]
-                    ]
                 }
             ]
         },
         "install": {
             "steps": [
                 {
                     "install_layer": [
```

### Comparing `cae_cli-0.2.2/cae/templates/assembler.txt` & `cae_cli-0.2.3/cae/templates/assembler.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 package <pk><group_id></group_id>.<artifact_id_sem_core></artifact_id_sem_core></pk>.assemblers.use_cases.<sc>args[0]</sc>;
 
-
+import com.cae.use_cases.assemblers.UseCaseAssembler;
 import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.<pc>args[0]</pc>UseCase;
-import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.factories.<pc>args[0]</pc>UseCaseFactory;
-import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.factories.dependency_wrapper.<pc>args[0]</pc>UseCaseDependencyWrapper;
 import lombok.AccessLevel;
 import lombok.NoArgsConstructor;
 
 @NoArgsConstructor(access = AccessLevel.PRIVATE)
-public class <pc>args[0]</pc>UseCaseAssembler {
+public class <pc>args[0]</pc>UseCaseAssembler implements UseCaseAssembler<<pc>args[0]</pc>UseCase>{
 
     public static final <pc>args[0]</pc>UseCase ASSEMBLED_INSTANCE;
 
     static {
-        var useCaseDependencies = <pc>args[0]</pc>UseCaseDependencyWrapper.builder()
-                .build();
-        ASSEMBLED_INSTANCE = <pc>args[0]</pc>UseCaseFactory.createSingletonInstanceUsing(useCaseDependencies);
     }
 
 }
```

### Comparing `cae_cli-0.2.2/cae/templates/entityFactory.txt` & `cae_cli-0.2.3/cae/templates/entityFactory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/cae/templates/implementation_cuc.txt` & `cae_cli-0.2.3/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/cae/templates/implementation_suc.txt` & `cae_cli-0.2.3/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/cae/templates/pom-adapters.txt` & `cae_cli-0.2.3/cae/templates/pom-adapters.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/cae/templates/pom-assemblers.txt` & `cae_cli-0.2.3/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/cae/templates/pom-core.txt` & `cae_cli-0.2.3/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/cae/templates/use_case.txt` & `cae_cli-0.2.3/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/cae/templates/use_case_factory.txt` & `cae_cli-0.2.3/cae/templates/use_case_factory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/cae/templates/use_case_implementation.txt` & `cae_cli-0.2.3/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.2.3/cae_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.2/setup.py` & `cae_cli-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.2.2',
+    version='0.2.3',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
```

