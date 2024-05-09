# Comparing `tmp/cae_cli-0.2.3.tar.gz` & `tmp/cae_cli-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.2.3.tar", last modified: Thu May  9 01:12:38 2024, max compression
+gzip compressed data, was "cae_cli-0.2.4.tar", last modified: Thu May  9 02:16:29 2024, max compression
```

## Comparing `cae_cli-0.2.3.tar` & `cae_cli-0.2.4.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 01:12:38.136301 cae_cli-0.2.3/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      415 2024-05-09 01:12:38.135303 cae_cli-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 01:12:38.098231 cae_cli-0.2.3/cae/
--rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.2.3/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.3/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.3/cae/__init__.py
--rw-rw-rw-   0        0        0     8485 2024-05-09 01:09:21.000000 cae_cli-0.2.3/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-09 01:12:38.120258 cae_cli-0.2.3/cae/templates/
--rw-rw-rw-   0        0        0      613 2024-05-09 01:12:33.000000 cae_cli-0.2.3/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.2.3/cae/templates/dependency_wrapper.txt
--rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.3/cae/templates/entity.txt
--rw-rw-rw-   0        0        0      584 2024-05-07 21:04:05.000000 cae_cli-0.2.3/cae/templates/entityFactory.txt
--rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.3/cae/templates/entityImplementation.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.3/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      463 2024-05-08 23:15:42.000000 cae_cli-0.2.3/cae/templates/implementation_ruc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.3/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.3/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.3/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.2.3/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.3/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.2.3/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.2.3/cae/templates/use_case_factory.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.3/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.3/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.3/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      353 2024-05-08 23:10:54.000000 cae_cli-0.2.3/cae/templates/use_case_ruc.txt
--rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.2.3/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 01:12:38.134299 cae_cli-0.2.3/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      415 2024-05-09 01:12:38.000000 cae_cli-0.2.3/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      869 2024-05-09 01:12:38.000000 cae_cli-0.2.3/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 01:12:38.000000 cae_cli-0.2.3/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-09 01:12:38.000000 cae_cli-0.2.3/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-09 01:12:38.000000 cae_cli-0.2.3/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 01:12:38.136301 cae_cli-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      610 2024-05-09 01:12:33.000000 cae_cli-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:16:29.323389 cae_cli-0.2.4/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0      415 2024-05-09 02:16:29.323389 cae_cli-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 02:16:29.284330 cae_cli-0.2.4/cae/
+-rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.2.4/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.2.4/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.2.4/cae/__init__.py
+-rw-rw-rw-   0        0        0     8485 2024-05-09 01:09:21.000000 cae_cli-0.2.4/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-09 02:16:29.304147 cae_cli-0.2.4/cae/templates/
+-rw-rw-rw-   0        0        0     1021 2024-05-09 02:10:39.000000 cae_cli-0.2.4/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.2.4/cae/templates/entity.txt
+-rw-rw-rw-   0        0        0      730 2024-05-09 02:13:43.000000 cae_cli-0.2.4/cae/templates/entityFactory.txt
+-rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.2.4/cae/templates/entityImplementation.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.2.4/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      794 2024-05-09 02:03:37.000000 cae_cli-0.2.4/cae/templates/implementation_ruc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.2.4/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.2.4/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.2.4/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.2.4/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.2.4/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.2.4/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.2.4/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.2.4/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.2.4/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      308 2024-05-09 01:56:52.000000 cae_cli-0.2.4/cae/templates/use_case_ruc.txt
+-rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.2.4/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 02:16:29.322382 cae_cli-0.2.4/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-05-09 02:16:29.000000 cae_cli-0.2.4/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2024-05-09 02:16:29.000000 cae_cli-0.2.4/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 02:16:29.000000 cae_cli-0.2.4/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-09 02:16:29.000000 cae_cli-0.2.4/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-09 02:16:29.000000 cae_cli-0.2.4/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 02:16:29.324387 cae_cli-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      610 2024-05-09 02:16:27.000000 cae_cli-0.2.4/setup.py
```

### Comparing `cae_cli-0.2.3/LICENSE` & `cae_cli-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.3/README.md` & `cae_cli-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.3/cae/ArchFlowJavaWeb.py` & `cae_cli-0.2.4/cae/ArchFlowJavaWeb.py`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.3/cae/db.json` & `cae_cli-0.2.4/cae/db.json`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.3/cae/templates/assembler.txt` & `cae_cli-0.2.4/cae/templates/assembler.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,13 +4,24 @@
 import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.<pc>args[0]</pc>UseCase;
 import lombok.AccessLevel;
 import lombok.NoArgsConstructor;
 
 @NoArgsConstructor(access = AccessLevel.PRIVATE)
 public class <pc>args[0]</pc>UseCaseAssembler implements UseCaseAssembler<<pc>args[0]</pc>UseCase>{
 
-    public static final <pc>args[0]</pc>UseCase ASSEMBLED_INSTANCE;
+    public static final <pc>args[0]</pc>UseCaseAssembler SINGLETON_ASSEMBLER = new <pc>args[0]</pc>UseCaseAssembler();
+
+    public static final <pc>args[0]</pc>UseCase V1;
 
     static {
+        V1 = <pc>args[0]</pc>UseCaseAssembler.initializeV1();
+    }
+
+    private static <pc>args[0]</pc>UseCase initializeV1(){
+        return new <pc>args[0]</pc>UseCaseImplementation();
     }
 
+    @Override
+    public <pc>args[0]</pc>UseCase getDefaultAssembledInstance(){
+        return V1;
+    }
 }
```

### Comparing `cae_cli-0.2.3/cae/templates/entityFactory.txt` & `cae_cli-0.2.4/cae/templates/use_case.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,8 @@
-package <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.entities.factories;
+package <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>;
 
-import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.entities.<pc>args[0]</pc>;
-import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.entities.implementations.<pc>args[0]</pc>Implementation;
-import lombok.AccessLevel;
-import lombok.NoArgsConstructor;
-
-@NoArgsConstructor(access = AccessLevel.PRIVATE)
-public class <pc>args[0]</pc>Factory {
-
-    public static <pc>args[0]</pc> getNewInstance(){
-        return new <pc>args[0]</pc>Implementation();
-    }
+import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.io.inputs.<pc>args[0]</pc>UseCaseInput;
+import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.io.outputs.<pc>args[0]</pc>UseCaseOutput;
+import com.cae.use_cases.specifics.functions.FunctionUseCase;
 
+public abstract class <pc>args[0]</pc>UseCase extends FunctionUseCase<<pc>args[0]</pc>UseCaseInput, <pc>args[0]</pc>UseCaseOutput> {
 }
```

### Comparing `cae_cli-0.2.3/cae/templates/implementation_cuc.txt` & `cae_cli-0.2.4/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.3/cae/templates/implementation_suc.txt` & `cae_cli-0.2.4/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.3/cae/templates/pom-adapters.txt` & `cae_cli-0.2.4/cae/templates/pom-adapters.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.3/cae/templates/pom-assemblers.txt` & `cae_cli-0.2.4/cae/templates/pom-assemblers.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.3/cae/templates/pom-core.txt` & `cae_cli-0.2.4/cae/templates/pom-core.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.2.3/cae/templates/use_case_factory.txt` & `cae_cli-0.2.4/cae/templates/use_case_implementation.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-package <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.factories;
+package <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.implementations;
 
+import com.cae.use_cases.correlations.UseCaseExecutionCorrelation;
 import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.<pc>args[0]</pc>UseCase;
-import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.factories.dependency_wrapper.<pc>args[0]</pc>UseCaseDependencyWrapper;
-import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.implementations.<pc>args[0]</pc>UseCaseImplementation;
-import lombok.AccessLevel;
-import lombok.NoArgsConstructor;
+import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.io.inputs.<pc>args[0]</pc>UseCaseInput;
+import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.io.outputs.<pc>args[0]</pc>UseCaseOutput;
 
-import java.util.Optional;
+public class <pc>args[0]</pc>UseCaseImplementation extends <pc>args[0]</pc>UseCase{
 
-@NoArgsConstructor(access = AccessLevel.PRIVATE)
-public class <pc>args[0]</pc>UseCaseFactory {
+    //declare here the ports and other dependencies you might need within this use case implementation
 
-    private static <pc>args[0]</pc>UseCase singleton = null;
-
-    public static <pc>args[0]</pc>UseCase createSingletonInstanceUsing(<pc>args[0]</pc>UseCaseDependencyWrapper dependencyWrapper){
-        return Optional.ofNullable(singleton).orElseGet(() -> {
-            singleton = new <pc>args[0]</pc>UseCaseImplementation(
- 	    );
-            return singleton;
-        });
+    @Override
+    protected <pc>args[0]</pc>UseCaseOutput applyInternalLogic(<pc>args[0]</pc>UseCaseInput input, UseCaseExecutionCorrelation correlation) {
+ 	 	//implement the logic of the use case here. to make contact with dependencies from here, create ports.
+ 	 	return null;
     }
-
 }
```

### Comparing `cae_cli-0.2.3/cae/templates/use_case_implementation.txt` & `cae_cli-0.2.4/cae/templates/implementation_ruc.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 package <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.implementations;
 
 import com.cae.use_cases.correlations.UseCaseExecutionCorrelation;
+import lombok.RequiredArgsConstructor;
 import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.<pc>args[0]</pc>UseCase;
-import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.io.inputs.<pc>args[0]</pc>UseCaseInput;
-import <pk><group_id></group_id>.<artifact_id></artifact_id></pk>.use_cases.<sc>args[0]</sc>.io.outputs.<pc>args[0]</pc>UseCaseOutput;
 
-public class <pc>args[0]</pc>UseCaseImplementation extends <pc>args[0]</pc>UseCase{
+
+@RequiredArgsConstructor
+public class <pc>args[0]</pc>UseCaseImplementation extends <pc>args[0]</pc>UseCase {
 
     //declare here the ports and other dependencies you might need within this use case implementation
 
     @Override
-    protected <pc>args[0]</pc>UseCaseOutput applyInternalLogic(<pc>args[0]</pc>UseCaseInput input, UseCaseExecutionCorrelation correlation) {
- 	 	//implement the logic of the use case here. to make contact with dependencies from here, create ports.
- 	 	return null;
+    protected void applyInternalLogic(UseCaseExecutionCorrelation useCaseExecutionCorrelation) {
+    //implement the logic of the use case here. to make contact with dependencies from here, create ports.
     }
 }
```

### Comparing `cae_cli-0.2.3/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.2.4/cae_cli.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 README.md
 setup.py
 cae/ArchFlowJavaWeb.py
 cae/Run.py
 cae/__init__.py
 cae/db.json
 cae/templates/assembler.txt
-cae/templates/dependency_wrapper.txt
 cae/templates/entity.txt
 cae/templates/entityFactory.txt
 cae/templates/entityImplementation.txt
 cae/templates/implementation_cuc.txt
 cae/templates/implementation_ruc.txt
 cae/templates/implementation_suc.txt
 cae/templates/pom-adapters.txt
 cae/templates/pom-assemblers.txt
 cae/templates/pom-core.txt
 cae/templates/use_case.txt
 cae/templates/use_case_cuc.txt
-cae/templates/use_case_factory.txt
 cae/templates/use_case_implementation.txt
 cae/templates/use_case_input.txt
 cae/templates/use_case_output.txt
 cae/templates/use_case_ruc.txt
 cae/templates/use_case_suc.txt
 cae_cli.egg-info/PKG-INFO
 cae_cli.egg-info/SOURCES.txt
```

### Comparing `cae_cli-0.2.3/setup.py` & `cae_cli-0.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.2.3',
+    version='0.2.4',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
```

