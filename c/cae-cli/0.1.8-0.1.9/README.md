# Comparing `tmp/cae_cli-0.1.8.tar.gz` & `tmp/cae_cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cae_cli-0.1.8.tar", last modified: Tue May  7 21:16:19 2024, max compression
+gzip compressed data, was "cae_cli-0.1.9.tar", last modified: Wed May  8 23:32:52 2024, max compression
```

## Comparing `cae_cli-0.1.8.tar` & `cae_cli-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 21:16:19.919302 cae_cli-0.1.8/
--rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      415 2024-05-07 21:16:19.918302 cae_cli-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 21:16:19.887359 cae_cli-0.1.8/cae/
--rw-rw-rw-   0        0        0     7644 2024-05-07 20:56:41.000000 cae_cli-0.1.8/cae/ArchFlowJavaWeb.py
--rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.1.8/cae/Run.py
--rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.1.8/cae/__init__.py
--rw-rw-rw-   0        0        0     8078 2024-05-07 02:25:43.000000 cae_cli-0.1.8/cae/db.json
-drwxrwxrwx   0        0        0        0 2024-05-07 21:16:19.904775 cae_cli-0.1.8/cae/templates/
--rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.1.8/cae/templates/assembler.txt
--rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.1.8/cae/templates/dependency_wrapper.txt
--rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.1.8/cae/templates/entity.txt
--rw-rw-rw-   0        0        0      584 2024-05-07 21:04:05.000000 cae_cli-0.1.8/cae/templates/entityFactory.txt
--rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.1.8/cae/templates/entityImplementation.txt
--rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.1.8/cae/templates/implementation_cuc.txt
--rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.1.8/cae/templates/implementation_suc.txt
--rw-rw-rw-   0        0        0     1691 2024-05-07 21:09:29.000000 cae_cli-0.1.8/cae/templates/pom-adapters.txt
--rw-rw-rw-   0        0        0     1565 2024-05-07 21:16:17.000000 cae_cli-0.1.8/cae/templates/pom-assemblers.txt
--rw-rw-rw-   0        0        0     1918 2024-05-07 21:09:29.000000 cae_cli-0.1.8/cae/templates/pom-core.txt
--rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.1.8/cae/templates/use_case.txt
--rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.1.8/cae/templates/use_case_cuc.txt
--rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.1.8/cae/templates/use_case_factory.txt
--rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.1.8/cae/templates/use_case_implementation.txt
--rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.1.8/cae/templates/use_case_input.txt
--rw-rw-rw-   0        0        0      397 2024-05-04 04:16:15.000000 cae_cli-0.1.8/cae/templates/use_case_output.txt
--rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.1.8/cae/templates/use_case_suc.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 21:16:19.917306 cae_cli-0.1.8/cae_cli.egg-info/
--rw-rw-rw-   0        0        0      415 2024-05-07 21:16:19.000000 cae_cli-0.1.8/cae_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      801 2024-05-07 21:16:19.000000 cae_cli-0.1.8/cae_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 21:16:19.000000 cae_cli-0.1.8/cae_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-07 21:16:19.000000 cae_cli-0.1.8/cae_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-07 21:16:19.000000 cae_cli-0.1.8/cae_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 21:16:19.919302 cae_cli-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      610 2024-05-07 21:16:17.000000 cae_cli-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 23:32:52.652111 cae_cli-0.1.9/
+-rw-rw-rw-   0        0        0    11558 2024-04-27 03:32:12.000000 cae_cli-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      415 2024-05-08 23:32:52.651111 cae_cli-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-04-27 03:32:12.000000 cae_cli-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 23:32:52.615451 cae_cli-0.1.9/cae/
+-rw-rw-rw-   0        0        0     7787 2024-05-08 20:05:59.000000 cae_cli-0.1.9/cae/ArchFlowJavaWeb.py
+-rw-rw-rw-   0        0        0      345 2024-05-05 20:22:02.000000 cae_cli-0.1.9/cae/Run.py
+-rw-rw-rw-   0        0        0       22 2024-05-05 19:42:37.000000 cae_cli-0.1.9/cae/__init__.py
+-rw-rw-rw-   0        0        0     8906 2024-05-08 23:26:36.000000 cae_cli-0.1.9/cae/db.json
+drwxrwxrwx   0        0        0        0 2024-05-08 23:32:52.635485 cae_cli-0.1.9/cae/templates/
+-rw-rw-rw-   0        0        0     1034 2024-05-05 03:41:55.000000 cae_cli-0.1.9/cae/templates/assembler.txt
+-rw-rw-rw-   0        0        0      328 2024-05-04 04:28:51.000000 cae_cli-0.1.9/cae/templates/dependency_wrapper.txt
+-rw-rw-rw-   0        0        0      247 2024-05-07 20:48:33.000000 cae_cli-0.1.9/cae/templates/entity.txt
+-rw-rw-rw-   0        0        0      584 2024-05-07 21:04:05.000000 cae_cli-0.1.9/cae/templates/entityFactory.txt
+-rw-rw-rw-   0        0        0      271 2024-05-07 20:51:51.000000 cae_cli-0.1.9/cae/templates/entityImplementation.txt
+-rw-rw-rw-   0        0        0      773 2024-05-05 03:55:59.000000 cae_cli-0.1.9/cae/templates/implementation_cuc.txt
+-rw-rw-rw-   0        0        0      889 2024-05-05 03:57:58.000000 cae_cli-0.1.9/cae/templates/implementation_suc.txt
+-rw-rw-rw-   0        0        0     1736 2024-05-08 20:11:20.000000 cae_cli-0.1.9/cae/templates/pom-adapters.txt
+-rw-rw-rw-   0        0        0     1594 2024-05-08 20:35:57.000000 cae_cli-0.1.9/cae/templates/pom-assemblers.txt
+-rw-rw-rw-   0        0        0     1945 2024-05-08 20:11:20.000000 cae_cli-0.1.9/cae/templates/pom-core.txt
+-rw-rw-rw-   0        0        0      570 2024-05-04 04:12:40.000000 cae_cli-0.1.9/cae/templates/use_case.txt
+-rw-rw-rw-   0        0        0      401 2024-05-05 04:01:36.000000 cae_cli-0.1.9/cae/templates/use_case_cuc.txt
+-rw-rw-rw-   0        0        0     1128 2024-05-05 03:07:00.000000 cae_cli-0.1.9/cae/templates/use_case_factory.txt
+-rw-rw-rw-   0        0        0     1058 2024-05-05 03:02:51.000000 cae_cli-0.1.9/cae/templates/use_case_implementation.txt
+-rw-rw-rw-   0        0        0      387 2024-05-04 04:15:05.000000 cae_cli-0.1.9/cae/templates/use_case_input.txt
+-rw-rw-rw-   0        0        0      307 2024-05-08 20:39:09.000000 cae_cli-0.1.9/cae/templates/use_case_output.txt
+-rw-rw-rw-   0        0        0      410 2024-05-05 04:03:32.000000 cae_cli-0.1.9/cae/templates/use_case_suc.txt
+drwxrwxrwx   0        0        0        0 2024-05-08 23:32:52.650110 cae_cli-0.1.9/cae_cli.egg-info/
+-rw-rw-rw-   0        0        0      415 2024-05-08 23:32:52.000000 cae_cli-0.1.9/cae_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      801 2024-05-08 23:32:52.000000 cae_cli-0.1.9/cae_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 23:32:52.000000 cae_cli-0.1.9/cae_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-08 23:32:52.000000 cae_cli-0.1.9/cae_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-08 23:32:52.000000 cae_cli-0.1.9/cae_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 23:32:52.652111 cae_cli-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      610 2024-05-08 23:32:50.000000 cae_cli-0.1.9/setup.py
```

### Comparing `cae_cli-0.1.8/LICENSE` & `cae_cli-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.8/README.md` & `cae_cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.8/cae/ArchFlowJavaWeb.py` & `cae_cli-0.1.9/cae/ArchFlowJavaWeb.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
     def __init__(self):
         super().__init__()
         self.StringManipulator.tag_functions_user = {"artifact_id": self.get_artifact_id,
                                                      "group_id": self.get_group_id,
                                                      "artifact_id_sem_core": self.artifact_id_remove_core}
 
     def create_project(self, group_id, artifact_id, version, package_name):
+        group_id = self.StringManipulator.to_packeage_case(group_id)
+        artifact_id = self.StringManipulator.to_kebab_case(artifact_id)
         maven_command = [
             "mvn",
             "archetype:generate",  # Corrected the typo here
             "-DgroupId=" + group_id,
             "-DartifactId=" + artifact_id,
             "-Dversion=" + version,
             "-Dpackage=" + package_name,
```

### Comparing `cae_cli-0.1.8/cae/db.json` & `cae_cli-0.1.9/cae/db.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768939393939394%*

 * *Differences: {"'functions'": "{'new_layer': {'steps': {1: {'create_file_based_in_template': {insert: [(0, "*

 * *                "'<kc>args[1]args[3]</kc>/')], delete: [0]}}}}, 'new_ruc': OrderedDict([('steps', "*

 * *                "[OrderedDict([('walk_to_use_case_layer', ['core'])]), "*

 * *                "OrderedDict([('create_folder', ['<sc>args[1]</sc>'])]), "*

 * *                "OrderedDict([('create_file_based_in_template', ['<sc>args[1]</sc>/', '<pc>args[1] "*

 * *                "use case</pc>.java', 'use_case_ruc.txt', ['args[1]' […]*

```diff
@@ -431,15 +431,15 @@
                         "args[1]args[3]",
                         "1.0",
                         "args[4]"
                     ]
                 },
                 {
                     "create_file_based_in_template": [
-                        "args[1]args[3]/",
+                        "<kc>args[1]args[3]</kc>/",
                         "pom.xml",
                         "pomargs[3].txt",
                         [
                             "args[0]",
                             "args[1]",
                             "args[2]",
                             "args[3]"
@@ -478,14 +478,73 @@
                         "montadores",
                         "-assemblers",
                         "args[1].args[2].assemblers.use_cases"
                     ]
                 }
             ]
         },
+        "new_ruc": {
+            "steps": [
+                {
+                    "walk_to_use_case_layer": [
+                        "core"
+                    ]
+                },
+                {
+                    "create_folder": [
+                        "<sc>args[1]</sc>"
+                    ]
+                },
+                {
+                    "create_file_based_in_template": [
+                        "<sc>args[1]</sc>/",
+                        "<pc>args[1] use case</pc>.java",
+                        "use_case_ruc.txt",
+                        [
+                            "args[1]"
+                        ]
+                    ]
+                },
+                {
+                    "create_folder": [
+                        "<sc>args[1]</sc>/implementations"
+                    ]
+                },
+                {
+                    "create_folder": [
+                        "<sc>args[1]</sc>/implementations/ports"
+                    ]
+                },
+                {
+                    "create_file_based_in_template": [
+                        "<sc>args[1]</sc>/implementations/",
+                        "<pc>args[1] use case implementation</pc>.java",
+                        "implementation_ruc.txt",
+                        [
+                            "args[1]"
+                        ]
+                    ]
+                },
+                {
+                    "return_root_path": "None"
+                },
+                {
+                    "function_adapters_layer": [
+                        "",
+                        "args[1]"
+                    ]
+                },
+                {
+                    "function_assembler_layer": [
+                        "",
+                        "args[1]"
+                    ]
+                }
+            ]
+        },
         "new_suc": {
             "steps": [
                 {
                     "walk_to_use_case_layer": [
                         "core"
                     ]
                 },
```

### Comparing `cae_cli-0.1.8/cae/templates/assembler.txt` & `cae_cli-0.1.9/cae/templates/assembler.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.8/cae/templates/entityFactory.txt` & `cae_cli-0.1.9/cae/templates/entityFactory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.8/cae/templates/implementation_cuc.txt` & `cae_cli-0.1.9/cae/templates/implementation_cuc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.8/cae/templates/implementation_suc.txt` & `cae_cli-0.1.9/cae/templates/implementation_suc.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.8/cae/templates/pom-adapters.txt` & `cae_cli-0.1.9/cae/templates/pom-core.txt`

 * *Files 9% similar despite different names*

#### Comparing `cae_cli-0.1.8/cae/templates/pom-adapters.txt` & `cae_cli-0.1.9/cae/templates/pom-core.txt`

```diff
@@ -1,15 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/maven-v4_0_0.xsd">
   <modelVersion>4.0.0</modelVersion>
-  <groupId>args[0]</groupId>
-  <artifactId>args[1]args[3]</artifactId>
+  <groupId>
+    <pk>args[0]</pk>
+  </groupId>
+  <artifactId>
+    <kc>args[1]args[3]</kc>
+  </artifactId>
   <packaging>jar</packaging>
   <version>1.0-SNAPSHOT</version>
-  <name>args[1]args[3]</name>
+  <name>
+    <kc>args[1]args[3]</kc>
+  </name>
+  <url>http://maven.apache.org</url>
   <properties>
     <maven.compiler.source>11</maven.compiler.source>
     <maven.compiler.target>11</maven.compiler.target>
     <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
   </properties>
   <dependencies>
     <dependency>
@@ -27,18 +34,23 @@
     <dependency>
       <groupId>org.mockito</groupId>
       <artifactId>mockito-junit-jupiter</artifactId>
       <version>4.8.0</version>
       <scope>test</scope>
     </dependency>
     <dependency>
-      <groupId>args[0]</groupId>
-      <artifactId>args[1]-core</artifactId>
-      <version>1.0-SNAPSHOT</version>
+      <groupId>com.nimbusds</groupId>
+      <artifactId>nimbus-jose-jwt</artifactId>
+      <version>9.30.2</version>
     </dependency>
     <dependency>
-      <groupId>ch.qos.logback</groupId>
-      <artifactId>logback-classic</artifactId>
-      <version>1.4.7</version>
+      <groupId>org.projectlombok</groupId>
+      <artifactId>lombok</artifactId>
+      <version>1.18.26</version>
+    </dependency>
+    <dependency>
+      <groupId>com.clean-arch-enablers</groupId>
+      <artifactId>cae-framework</artifactId>
+      <version>0.7.0</version>
     </dependency>
   </dependencies>
 </project>
```

### Comparing `cae_cli-0.1.8/cae/templates/pom-assemblers.txt` & `cae_cli-0.1.9/cae/templates/pom-assemblers.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,90 +9,92 @@
 00000080: 7267 2f50 4f4d 2f34 2e30 2e30 2068 7474  rg/POM/4.0.0 htt
 00000090: 703a 2f2f 6d61 7665 6e2e 6170 6163 6865  p://maven.apache
 000000a0: 2e6f 7267 2f6d 6176 656e 2d76 345f 305f  .org/maven-v4_0_
 000000b0: 302e 7873 6422 3e0d 0a20 2020 203c 6d6f  0.xsd">..    <mo
 000000c0: 6465 6c56 6572 7369 6f6e 3e34 2e30 2e30  delVersion>4.0.0
 000000d0: 3c2f 6d6f 6465 6c56 6572 7369 6f6e 3e0d  </modelVersion>.
 000000e0: 0a0d 0a20 2020 203c 6772 6f75 7049 643e  ...    <groupId>
-000000f0: 6172 6773 5b30 5d3c 2f67 726f 7570 4964  args[0]</groupId
-00000100: 3e0d 0a20 2020 203c 6172 7469 6661 6374  >..    <artifact
-00000110: 4964 3e3c 7363 3e61 7267 735b 315d 6172  Id><sc>args[1]ar
-00000120: 6773 5b33 5d3c 7363 3e3c 2f61 7274 6966  gs[3]<sc></artif
-00000130: 6163 7449 643e 0d0a 2020 2020 3c70 6163  actId>..    <pac
-00000140: 6b61 6769 6e67 3e6a 6172 3c2f 7061 636b  kaging>jar</pack
-00000150: 6167 696e 673e 0d0a 2020 2020 3c76 6572  aging>..    <ver
-00000160: 7369 6f6e 3e31 2e30 2d53 4e41 5053 484f  sion>1.0-SNAPSHO
-00000170: 543c 2f76 6572 7369 6f6e 3e0d 0a20 2020  T</version>..   
-00000180: 203c 6e61 6d65 3e3c 7363 3e61 7267 735b   <name><sc>args[
-00000190: 315d 6172 6773 5b33 5d3c 7363 3e3c 2f6e  1]args[3]<sc></n
-000001a0: 616d 653e 0d0a 0d0a 2020 2020 3c75 726c  ame>....    <url
-000001b0: 3e68 7474 703a 2f2f 6d61 7665 6e2e 6170  >http://maven.ap
-000001c0: 6163 6865 2e6f 7267 3c2f 7572 6c3e 0d0a  ache.org</url>..
-000001d0: 0d0a 2020 2020 3c70 726f 7065 7274 6965  ..    <propertie
-000001e0: 733e 0d0a 2020 2020 2020 2020 3c6d 6176  s>..        <mav
-000001f0: 656e 2e63 6f6d 7069 6c65 722e 736f 7572  en.compiler.sour
-00000200: 6365 3e31 313c 2f6d 6176 656e 2e63 6f6d  ce>11</maven.com
-00000210: 7069 6c65 722e 736f 7572 6365 3e0d 0a20  piler.source>.. 
-00000220: 2020 2020 2020 203c 6d61 7665 6e2e 636f         <maven.co
-00000230: 6d70 696c 6572 2e74 6172 6765 743e 3131  mpiler.target>11
-00000240: 3c2f 6d61 7665 6e2e 636f 6d70 696c 6572  </maven.compiler
-00000250: 2e74 6172 6765 743e 0d0a 2020 2020 2020  .target>..      
-00000260: 2020 3c70 726f 6a65 6374 2e62 7569 6c64    <project.build
-00000270: 2e73 6f75 7263 6545 6e63 6f64 696e 673e  .sourceEncoding>
-00000280: 5554 462d 383c 2f70 726f 6a65 6374 2e62  UTF-8</project.b
-00000290: 7569 6c64 2e73 6f75 7263 6545 6e63 6f64  uild.sourceEncod
-000002a0: 696e 673e 0d0a 2020 2020 3c2f 7072 6f70  ing>..    </prop
-000002b0: 6572 7469 6573 3e0d 0a0d 0a20 2020 203c  erties>....    <
-000002c0: 6465 7065 6e64 656e 6369 6573 3e0d 0a20  dependencies>.. 
-000002d0: 2020 2020 2020 203c 6465 7065 6e64 656e         <dependen
-000002e0: 6379 3e0d 0a20 2020 2020 2020 2020 2020  cy>..           
-000002f0: 203c 6772 6f75 7049 643e 6a75 6e69 743c   <groupId>junit<
-00000300: 2f67 726f 7570 4964 3e0d 0a20 2020 2020  /groupId>..     
-00000310: 2020 2020 2020 203c 6172 7469 6661 6374         <artifact
-00000320: 4964 3e6a 756e 6974 3c2f 6172 7469 6661  Id>junit</artifa
-00000330: 6374 4964 3e0d 0a20 2020 2020 2020 2020  ctId>..         
-00000340: 2020 203c 7665 7273 696f 6e3e 342e 3133     <version>4.13
-00000350: 2e32 3c2f 7665 7273 696f 6e3e 0d0a 2020  .2</version>..  
-00000360: 2020 2020 2020 2020 2020 3c73 636f 7065            <scope
-00000370: 3e74 6573 743c 2f73 636f 7065 3e0d 0a20  >test</scope>.. 
-00000380: 2020 2020 2020 203c 2f64 6570 656e 6465         </depende
-00000390: 6e63 793e 0d0a 2020 2020 2020 2020 3c64  ncy>..        <d
-000003a0: 6570 656e 6465 6e63 793e 0d0a 2020 2020  ependency>..    
-000003b0: 2020 2020 2020 2020 3c67 726f 7570 4964          <groupId
-000003c0: 3e6f 7267 2e6d 6f63 6b69 746f 3c2f 6772  >org.mockito</gr
-000003d0: 6f75 7049 643e 0d0a 2020 2020 2020 2020  oupId>..        
-000003e0: 2020 2020 3c61 7274 6966 6163 7449 643e      <artifactId>
-000003f0: 6d6f 636b 6974 6f2d 636f 7265 3c2f 6172  mockito-core</ar
-00000400: 7469 6661 6374 4964 3e0d 0a20 2020 2020  tifactId>..     
-00000410: 2020 2020 2020 203c 7665 7273 696f 6e3e         <version>
-00000420: 342e 382e 303c 2f76 6572 7369 6f6e 3e0d  4.8.0</version>.
-00000430: 0a20 2020 2020 2020 2020 2020 203c 7363  .            <sc
-00000440: 6f70 653e 7465 7374 3c2f 7363 6f70 653e  ope>test</scope>
-00000450: 0d0a 2020 2020 2020 2020 3c2f 6465 7065  ..        </depe
-00000460: 6e64 656e 6379 3e0d 0a20 2020 2020 2020  ndency>..       
-00000470: 203c 6465 7065 6e64 656e 6379 3e0d 0a20   <dependency>.. 
-00000480: 2020 2020 2020 2020 2020 203c 6772 6f75             <grou
-00000490: 7049 643e 6f72 672e 6d6f 636b 6974 6f3c  pId>org.mockito<
-000004a0: 2f67 726f 7570 4964 3e0d 0a20 2020 2020  /groupId>..     
-000004b0: 2020 2020 2020 203c 6172 7469 6661 6374         <artifact
-000004c0: 4964 3e6d 6f63 6b69 746f 2d6a 756e 6974  Id>mockito-junit
-000004d0: 2d6a 7570 6974 6572 3c2f 6172 7469 6661  -jupiter</artifa
-000004e0: 6374 4964 3e0d 0a20 2020 2020 2020 2020  ctId>..         
-000004f0: 2020 203c 7665 7273 696f 6e3e 342e 382e     <version>4.8.
-00000500: 303c 2f76 6572 7369 6f6e 3e0d 0a20 2020  0</version>..   
-00000510: 2020 2020 2020 2020 203c 7363 6f70 653e           <scope>
-00000520: 7465 7374 3c2f 7363 6f70 653e 0d0a 2020  test</scope>..  
-00000530: 2020 2020 2020 3c2f 6465 7065 6e64 656e        </dependen
-00000540: 6379 3e0d 0a20 2020 2020 2020 203c 6465  cy>..        <de
-00000550: 7065 6e64 656e 6379 3e0d 0a20 2020 2020  pendency>..     
-00000560: 2020 2020 2020 203c 6772 6f75 7049 643e         <groupId>
-00000570: 6172 6773 5b30 5d3c 2f67 726f 7570 4964  args[0]</groupId
-00000580: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
-00000590: 6172 7469 6661 6374 4964 3e61 7267 735b  artifactId>args[
-000005a0: 315d 2d61 6461 7074 6572 733c 2f61 7274  1]-adapters</art
-000005b0: 6966 6163 7449 643e 0d0a 2020 2020 2020  ifactId>..      
-000005c0: 2020 2020 2020 3c76 6572 7369 6f6e 3e31        <version>1
-000005d0: 2e30 2d53 4e41 5053 484f 543c 2f76 6572  .0-SNAPSHOT</ver
-000005e0: 7369 6f6e 3e0d 0a20 2020 2020 2020 203c  sion>..        <
-000005f0: 2f64 6570 656e 6465 6e63 793e 0d0a 2020  /dependency>..  
-00000600: 2020 3c2f 6465 7065 6e64 656e 6369 6573    </dependencies
-00000610: 3e0d 0a3c 2f70 726f 6a65 6374 3e         >..</project>
+000000f0: 3c70 6b3e 6172 6773 5b30 5d3c 2f70 6b3e  <pk>args[0]</pk>
+00000100: 3c2f 6772 6f75 7049 643e 0d0a 2020 2020  </groupId>..    
+00000110: 3c61 7274 6966 6163 7449 643e 3c6b 633e  <artifactId><kc>
+00000120: 6172 6773 5b31 5d61 7267 735b 335d 3c2f  args[1]args[3]</
+00000130: 6b63 3e3c 2f61 7274 6966 6163 7449 643e  kc></artifactId>
+00000140: 0d0a 2020 2020 3c70 6163 6b61 6769 6e67  ..    <packaging
+00000150: 3e6a 6172 3c2f 7061 636b 6167 696e 673e  >jar</packaging>
+00000160: 0d0a 2020 2020 3c76 6572 7369 6f6e 3e31  ..    <version>1
+00000170: 2e30 2d53 4e41 5053 484f 543c 2f76 6572  .0-SNAPSHOT</ver
+00000180: 7369 6f6e 3e0d 0a20 2020 203c 6e61 6d65  sion>..    <name
+00000190: 3e3c 6b63 3e61 7267 735b 315d 6172 6773  ><kc>args[1]args
+000001a0: 5b33 5d3c 2f6b 633e 3c2f 6e61 6d65 3e0d  [3]</kc></name>.
+000001b0: 0a0d 0a20 2020 203c 7572 6c3e 6874 7470  ...    <url>http
+000001c0: 3a2f 2f6d 6176 656e 2e61 7061 6368 652e  ://maven.apache.
+000001d0: 6f72 673c 2f75 726c 3e0d 0a0d 0a20 2020  org</url>....   
+000001e0: 203c 7072 6f70 6572 7469 6573 3e0d 0a20   <properties>.. 
+000001f0: 2020 2020 2020 203c 6d61 7665 6e2e 636f         <maven.co
+00000200: 6d70 696c 6572 2e73 6f75 7263 653e 3131  mpiler.source>11
+00000210: 3c2f 6d61 7665 6e2e 636f 6d70 696c 6572  </maven.compiler
+00000220: 2e73 6f75 7263 653e 0d0a 2020 2020 2020  .source>..      
+00000230: 2020 3c6d 6176 656e 2e63 6f6d 7069 6c65    <maven.compile
+00000240: 722e 7461 7267 6574 3e31 313c 2f6d 6176  r.target>11</mav
+00000250: 656e 2e63 6f6d 7069 6c65 722e 7461 7267  en.compiler.targ
+00000260: 6574 3e0d 0a20 2020 2020 2020 203c 7072  et>..        <pr
+00000270: 6f6a 6563 742e 6275 696c 642e 736f 7572  oject.build.sour
+00000280: 6365 456e 636f 6469 6e67 3e55 5446 2d38  ceEncoding>UTF-8
+00000290: 3c2f 7072 6f6a 6563 742e 6275 696c 642e  </project.build.
+000002a0: 736f 7572 6365 456e 636f 6469 6e67 3e0d  sourceEncoding>.
+000002b0: 0a20 2020 203c 2f70 726f 7065 7274 6965  .    </propertie
+000002c0: 733e 0d0a 0d0a 2020 2020 3c64 6570 656e  s>....    <depen
+000002d0: 6465 6e63 6965 733e 0d0a 2020 2020 2020  dencies>..      
+000002e0: 2020 3c64 6570 656e 6465 6e63 793e 0d0a    <dependency>..
+000002f0: 2020 2020 2020 2020 2020 2020 3c67 726f              <gro
+00000300: 7570 4964 3e6a 756e 6974 3c2f 6772 6f75  upId>junit</grou
+00000310: 7049 643e 0d0a 2020 2020 2020 2020 2020  pId>..          
+00000320: 2020 3c61 7274 6966 6163 7449 643e 6a75    <artifactId>ju
+00000330: 6e69 743c 2f61 7274 6966 6163 7449 643e  nit</artifactId>
+00000340: 0d0a 2020 2020 2020 2020 2020 2020 3c76  ..            <v
+00000350: 6572 7369 6f6e 3e34 2e31 332e 323c 2f76  ersion>4.13.2</v
+00000360: 6572 7369 6f6e 3e0d 0a20 2020 2020 2020  ersion>..       
+00000370: 2020 2020 203c 7363 6f70 653e 7465 7374       <scope>test
+00000380: 3c2f 7363 6f70 653e 0d0a 2020 2020 2020  </scope>..      
+00000390: 2020 3c2f 6465 7065 6e64 656e 6379 3e0d    </dependency>.
+000003a0: 0a20 2020 2020 2020 203c 6465 7065 6e64  .        <depend
+000003b0: 656e 6379 3e0d 0a20 2020 2020 2020 2020  ency>..         
+000003c0: 2020 203c 6772 6f75 7049 643e 6f72 672e     <groupId>org.
+000003d0: 6d6f 636b 6974 6f3c 2f67 726f 7570 4964  mockito</groupId
+000003e0: 3e0d 0a20 2020 2020 2020 2020 2020 203c  >..            <
+000003f0: 6172 7469 6661 6374 4964 3e6d 6f63 6b69  artifactId>mocki
+00000400: 746f 2d63 6f72 653c 2f61 7274 6966 6163  to-core</artifac
+00000410: 7449 643e 0d0a 2020 2020 2020 2020 2020  tId>..          
+00000420: 2020 3c76 6572 7369 6f6e 3e34 2e38 2e30    <version>4.8.0
+00000430: 3c2f 7665 7273 696f 6e3e 0d0a 2020 2020  </version>..    
+00000440: 2020 2020 2020 2020 3c73 636f 7065 3e74          <scope>t
+00000450: 6573 743c 2f73 636f 7065 3e0d 0a20 2020  est</scope>..   
+00000460: 2020 2020 203c 2f64 6570 656e 6465 6e63       </dependenc
+00000470: 793e 0d0a 2020 2020 2020 2020 3c64 6570  y>..        <dep
+00000480: 656e 6465 6e63 793e 0d0a 2020 2020 2020  endency>..      
+00000490: 2020 2020 2020 3c67 726f 7570 4964 3e6f        <groupId>o
+000004a0: 7267 2e6d 6f63 6b69 746f 3c2f 6772 6f75  rg.mockito</grou
+000004b0: 7049 643e 0d0a 2020 2020 2020 2020 2020  pId>..          
+000004c0: 2020 3c61 7274 6966 6163 7449 643e 6d6f    <artifactId>mo
+000004d0: 636b 6974 6f2d 6a75 6e69 742d 6a75 7069  ckito-junit-jupi
+000004e0: 7465 723c 2f61 7274 6966 6163 7449 643e  ter</artifactId>
+000004f0: 0d0a 2020 2020 2020 2020 2020 2020 3c76  ..            <v
+00000500: 6572 7369 6f6e 3e34 2e38 2e30 3c2f 7665  ersion>4.8.0</ve
+00000510: 7273 696f 6e3e 0d0a 2020 2020 2020 2020  rsion>..        
+00000520: 2020 2020 3c73 636f 7065 3e74 6573 743c      <scope>test<
+00000530: 2f73 636f 7065 3e0d 0a20 2020 2020 2020  /scope>..       
+00000540: 203c 2f64 6570 656e 6465 6e63 793e 0d0a   </dependency>..
+00000550: 2020 2020 2020 2020 3c64 6570 656e 6465          <depende
+00000560: 6e63 793e 0d0a 2020 2020 2020 2020 2020  ncy>..          
+00000570: 2020 3c67 726f 7570 4964 3e3c 706b 3e61    <groupId><pk>a
+00000580: 7267 735b 305d 3c2f 706b 3e3c 2f67 726f  rgs[0]</pk></gro
+00000590: 7570 4964 3e0d 0a20 2020 2020 2020 2020  upId>..         
+000005a0: 2020 203c 6172 7469 6661 6374 4964 3e3c     <artifactId><
+000005b0: 6b63 3e61 7267 735b 315d 2d61 6461 7074  kc>args[1]-adapt
+000005c0: 6572 733c 2f6b 633e 3c2f 6172 7469 6661  ers</kc></artifa
+000005d0: 6374 4964 3e0d 0a20 2020 2020 2020 2020  ctId>..         
+000005e0: 2020 203c 7665 7273 696f 6e3e 312e 302d     <version>1.0-
+000005f0: 534e 4150 5348 4f54 3c2f 7665 7273 696f  SNAPSHOT</versio
+00000600: 6e3e 0d0a 2020 2020 2020 2020 3c2f 6465  n>..        </de
+00000610: 7065 6e64 656e 6379 3e0d 0a20 2020 203c  pendency>..    <
+00000620: 2f64 6570 656e 6465 6e63 6965 733e 0d0a  /dependencies>..
+00000630: 3c2f 7072 6f6a 6563 743e                 </project>
```

### Comparing `cae_cli-0.1.8/cae/templates/use_case.txt` & `cae_cli-0.1.9/cae/templates/use_case.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.8/cae/templates/use_case_factory.txt` & `cae_cli-0.1.9/cae/templates/use_case_factory.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.8/cae/templates/use_case_implementation.txt` & `cae_cli-0.1.9/cae/templates/use_case_implementation.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.8/cae_cli.egg-info/SOURCES.txt` & `cae_cli-0.1.9/cae_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cae_cli-0.1.8/setup.py` & `cae_cli-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='cae-cli',
-    version='0.1.8',
+    version='0.1.9',
     license='Apache License',
     author='Carlos Vinicius Da Silva',
     long_description="teste da aplicação ainda",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='cae-cli',
     description=u'o cae tem como objetivo facilitar a utilização de projeto com arquitetura limpa',
```

