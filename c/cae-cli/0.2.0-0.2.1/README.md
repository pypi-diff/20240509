# Comparing `tmp/cae_cli-0.2.0.tar.gz` & `tmp/cae_cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.2.0.tar", last modified: Wed May  8 23:39:03 2024, max compression
+gzip compressed data, was "cae_cli-0.2.1.tar", last modified: Wed May  8 23:51:43 2024, max compression
```

## Comparing `cae_cli-0.2.0.tar` & `cae_cli-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 23:39:03.650454 cae_cli-0.2.0/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      415 2024-05-08 23:39:03.649444 cae_cli-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 23:39:03.613651 cae_cli-0.2.0/cae/
--rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.2.0/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.0/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.0/cae/__init__.py
--rw-rw-rw-   0        0        0     8952 2024-05-08 23:38:55.000000 cae_cli-0.2.0/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-08 23:39:03.635424 cae_cli-0.2.0/cae/templates/
--rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.2.0/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.0/cae/templates/dependency_wrapper.txt
--rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.0/cae/templates/entity.txt
--rw-rw-rw-   0        0        0      584 2024-05-07 21:04:05.000000 cae_cli-0.2.0/cae/templates/entityFactory.txt
--rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.0/cae/templates/entityImplementation.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.0/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.0/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.0/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.0/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.2.0/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.0/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.2.0/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.0/cae/templates/use_case_factory.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.0/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.0/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.0/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.2.0/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 23:39:03.647936 cae_cli-0.2.0/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      415 2024-05-08 23:39:03.000000 cae_cli-0.2.0/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      801 2024-05-08 23:39:03.000000 cae_cli-0.2.0/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 23:39:03.000000 cae_cli-0.2.0/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-08 23:39:03.000000 cae_cli-0.2.0/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-08 23:39:03.000000 cae_cli-0.2.0/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 23:39:03.650454 cae_cli-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      610 2024-05-08 23:38:55.000000 cae_cli-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 23:51:43.457706 cae_cli-0.2.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      415 2024-05-08 23:51:43.456706 cae_cli-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 23:51:43.415653 cae_cli-0.2.1/cae/
+-rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.2.1/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.1/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.1/cae/__init__.py
+-rw-rw-rw-   0        0        0     8952 2024-05-08 23:38:55.000000 cae_cli-0.2.1/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-08 23:51:43.437677 cae_cli-0.2.1/cae/templates/
+-rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.2.1/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.1/cae/templates/dependency_wrapper.txt
+-rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.1/cae/templates/entity.txt
+-rw-rw-rw-   0        0        0      584 2024-05-07 21:04:05.000000 cae_cli-0.2.1/cae/templates/entityFactory.txt
+-rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.1/cae/templates/entityImplementation.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.1/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      463 2024-05-08 23:15:42.000000 cae_cli-0.2.1/cae/templates/implementation_ruc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.1/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.1/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.1/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.2.1/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.1/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.2.1/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.1/cae/templates/use_case_factory.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.1/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.1/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.1/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      353 2024-05-08 23:10:54.000000 cae_cli-0.2.1/cae/templates/use_case_ruc.txt
+-rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.2.1/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 23:51:43.455706 cae_cli-0.2.1/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-05-08 23:51:43.000000 cae_cli-0.2.1/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      869 2024-05-08 23:51:43.000000 cae_cli-0.2.1/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 23:51:43.000000 cae_cli-0.2.1/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-08 23:51:43.000000 cae_cli-0.2.1/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-08 23:51:43.000000 cae_cli-0.2.1/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 23:51:43.457706 cae_cli-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      610 2024-05-08 23:50:44.000000 cae_cli-0.2.1/setup.py
```

### Comparing `cae_cli-0.2.0/LICENSE` & `cae_cli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/README.md` & `cae_cli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae/ArchFlowJavaWeb.py` & `cae_cli-0.2.1/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae/db.json` & `cae_cli-0.2.1/cae/db.json`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae/templates/assembler.txt` & `cae_cli-0.2.1/cae/templates/assembler.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae/templates/entityFactory.txt` & `cae_cli-0.2.1/cae/templates/entityFactory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae/templates/implementation_cuc.txt` & `cae_cli-0.2.1/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae/templates/implementation_suc.txt` & `cae_cli-0.2.1/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae/templates/pom-adapters.txt` & `cae_cli-0.2.1/cae/templates/pom-adapters.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae/templates/pom-assemblers.txt` & `cae_cli-0.2.1/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae/templates/pom-core.txt` & `cae_cli-0.2.1/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae/templates/use_case.txt` & `cae_cli-0.2.1/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae/templates/use_case_factory.txt` & `cae_cli-0.2.1/cae/templates/use_case_factory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae/templates/use_case_implementation.txt` & `cae_cli-0.2.1/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.0/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.2.1/cae_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,25 @@
 cae/db.json
 cae/templates/assembler.txt
 cae/templates/dependency_wrapper.txt
 cae/templates/entity.txt
 cae/templates/entityFactory.txt
 cae/templates/entityImplementation.txt
 cae/templates/implementation_cuc.txt
+cae/templates/implementation_ruc.txt
 cae/templates/implementation_suc.txt
 cae/templates/pom-adapters.txt
 cae/templates/pom-assemblers.txt
 cae/templates/pom-core.txt
 cae/templates/use_case.txt
 cae/templates/use_case_cuc.txt
 cae/templates/use_case_factory.txt
 cae/templates/use_case_implementation.txt
 cae/templates/use_case_input.txt
 cae/templates/use_case_output.txt
+cae/templates/use_case_ruc.txt
 cae/templates/use_case_suc.txt
 cae_cli.egg-info/PKG-INFO
 cae_cli.egg-info/SOURCES.txt
 cae_cli.egg-info/dependency_links.txt
 cae_cli.egg-info/requires.txt
 cae_cli.egg-info/top_level.txt
```

### Comparing `cae_cli-0.2.0/setup.py` & `cae_cli-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.2.0',
+    version='0.2.1',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
```

