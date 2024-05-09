# Comparing `tmp/shareyourcloning_linkml-0.1.5.1a0.tar.gz` & `tmp/shareyourcloning_linkml-0.1.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareyourcloning_linkml-0.1.5.1a0.tar", max compression
+gzip compressed data, was "shareyourcloning_linkml-0.1.5a0.tar", max compression
```

## Comparing `shareyourcloning_linkml-0.1.5.1a0.tar` & `shareyourcloning_linkml-0.1.5a0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1087 2024-05-09 08:24:53.212984 shareyourcloning_linkml-0.1.5.1a0/LICENSE
--rw-r--r--   0        0        0      923 2024-05-09 08:24:53.212984 shareyourcloning_linkml-0.1.5.1a0/README.md
--rw-r--r--   0        0        0    17584 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/project/excel/shareyourcloning_linkml.xlsx
--rw-r--r--   0        0        0     4170 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/project/graphql/shareyourcloning_linkml.graphql
--rw-r--r--   0        0        0     6881 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/project/jsonld/shareyourcloning_linkml.context.jsonld
--rw-r--r--   0        0        0    82662 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/project/jsonld/shareyourcloning_linkml.jsonld
--rw-r--r--   0        0        0    42020 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/project/jsonschema/shareyourcloning_linkml.schema.json
--rw-r--r--   0        0        0    54517 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/project/owl/shareyourcloning_linkml.owl.ttl
--rw-r--r--   0        0        0      400 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/project/prefixmap/shareyourcloning_linkml.yaml
--rw-r--r--   0        0        0     6097 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/project/protobuf/shareyourcloning_linkml.proto
--rw-r--r--   0        0        0    64643 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/project/python/shareyourcloning_linkml.py
--rw-r--r--   0        0        0    44003 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/project/shacl/shareyourcloning_linkml.shacl.ttl
--rw-r--r--   0        0        0     9599 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/project/shex/shareyourcloning_linkml.shex
--rw-r--r--   0        0        0    30242 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/project/sqlschema/shareyourcloning_linkml.sql
--rw-r--r--   0        0        0     1501 2024-05-09 08:25:06.436983 shareyourcloning_linkml-0.1.5.1a0/pyproject.toml
--rw-r--r--   0        0        0      186 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/src/shareyourcloning_linkml/_version.py
--rw-r--r--   0        0        0       41 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/src/shareyourcloning_linkml/datamodel/__init__.py
--rw-r--r--   0        0        0    25928 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/src/shareyourcloning_linkml/datamodel/_models.py
--rw-r--r--   0        0        0       42 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/src/shareyourcloning_linkml/datamodel/models.py
--rw-r--r--   0        0        0    15636 2024-05-09 08:24:53.216984 shareyourcloning_linkml-0.1.5.1a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml
--rw-r--r--   0        0        0     1879 1970-01-01 00:00:00.000000 shareyourcloning_linkml-0.1.5.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-08 16:47:39.665000 shareyourcloning_linkml-0.1.5a0/LICENSE
+-rw-r--r--   0        0        0      923 2024-05-08 16:47:39.665000 shareyourcloning_linkml-0.1.5a0/README.md
+-rw-r--r--   0        0        0    17584 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/excel/shareyourcloning_linkml.xlsx
+-rw-r--r--   0        0        0     4170 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/graphql/shareyourcloning_linkml.graphql
+-rw-r--r--   0        0        0     6881 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/jsonld/shareyourcloning_linkml.context.jsonld
+-rw-r--r--   0        0        0    82662 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/jsonld/shareyourcloning_linkml.jsonld
+-rw-r--r--   0        0        0    42020 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/jsonschema/shareyourcloning_linkml.schema.json
+-rw-r--r--   0        0        0    54517 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/owl/shareyourcloning_linkml.owl.ttl
+-rw-r--r--   0        0        0      400 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/prefixmap/shareyourcloning_linkml.yaml
+-rw-r--r--   0        0        0     6097 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/protobuf/shareyourcloning_linkml.proto
+-rw-r--r--   0        0        0    64643 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/python/shareyourcloning_linkml.py
+-rw-r--r--   0        0        0    44003 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/shacl/shareyourcloning_linkml.shacl.ttl
+-rw-r--r--   0        0        0     9599 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/shex/shareyourcloning_linkml.shex
+-rw-r--r--   0        0        0    30242 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/project/sqlschema/shareyourcloning_linkml.sql
+-rw-r--r--   0        0        0     1499 2024-05-08 16:47:52.165159 shareyourcloning_linkml-0.1.5a0/pyproject.toml
+-rw-r--r--   0        0        0      186 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/_version.py
+-rw-r--r--   0        0        0       41 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/datamodel/__init__.py
+-rw-r--r--   0        0        0    25928 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/datamodel/_models.py
+-rw-r--r--   0        0        0       42 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/datamodel/models.py
+-rw-r--r--   0        0        0    15636 2024-05-08 16:47:39.669000 shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml
+-rw-r--r--   0        0        0     1877 1970-01-01 00:00:00.000000 shareyourcloning_linkml-0.1.5a0/PKG-INFO
```

### Comparing `shareyourcloning_linkml-0.1.5.1a0/LICENSE` & `shareyourcloning_linkml-0.1.5a0/LICENSE`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/README.md` & `shareyourcloning_linkml-0.1.5a0/README.md`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/project/excel/shareyourcloning_linkml.xlsx` & `shareyourcloning_linkml-0.1.5a0/project/excel/shareyourcloning_linkml.xlsx`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/project/graphql/shareyourcloning_linkml.graphql` & `shareyourcloning_linkml-0.1.5a0/project/graphql/shareyourcloning_linkml.graphql`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/project/jsonld/shareyourcloning_linkml.context.jsonld` & `shareyourcloning_linkml-0.1.5a0/project/jsonld/shareyourcloning_linkml.context.jsonld`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/project/jsonld/shareyourcloning_linkml.jsonld` & `shareyourcloning_linkml-0.1.5a0/project/jsonld/shareyourcloning_linkml.jsonld`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/project/jsonschema/shareyourcloning_linkml.schema.json` & `shareyourcloning_linkml-0.1.5a0/project/jsonschema/shareyourcloning_linkml.schema.json`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/project/owl/shareyourcloning_linkml.owl.ttl` & `shareyourcloning_linkml-0.1.5a0/project/owl/shareyourcloning_linkml.owl.ttl`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/project/protobuf/shareyourcloning_linkml.proto` & `shareyourcloning_linkml-0.1.5a0/project/protobuf/shareyourcloning_linkml.proto`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/project/python/shareyourcloning_linkml.py` & `shareyourcloning_linkml-0.1.5a0/project/python/shareyourcloning_linkml.py`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/project/shacl/shareyourcloning_linkml.shacl.ttl` & `shareyourcloning_linkml-0.1.5a0/project/shacl/shareyourcloning_linkml.shacl.ttl`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/project/shex/shareyourcloning_linkml.shex` & `shareyourcloning_linkml-0.1.5a0/project/shex/shareyourcloning_linkml.shex`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/project/sqlschema/shareyourcloning_linkml.sql` & `shareyourcloning_linkml-0.1.5a0/project/sqlschema/shareyourcloning_linkml.sql`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/pyproject.toml` & `shareyourcloning_linkml-0.1.5a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Manuel Lera-Ramirez <manuel.lera-ramirez@ucl.ac.uk>"]
 description = "A LinkML data model for ShareYourCloning"
 include = ["README.md", "src/shareyourcloning_linkml/schema", "project"]
 license = "MIT"
 name = "shareyourcloning-linkml"
 readme = "README.md"
-version = "0.1.5.1a0"
+version = "0.1.5a0"
 
 homepage = "https://github.com/genestorian/ShareYourCloning_LinkML"
 repository = "https://github.com/genestorian/ShareYourCloning_LinkML"
 documentation = "https://genestorian.github.io/ShareYourCloning_LinkML"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `shareyourcloning_linkml-0.1.5.1a0/src/shareyourcloning_linkml/datamodel/_models.py` & `shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/datamodel/_models.py`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml` & `shareyourcloning_linkml-0.1.5a0/src/shareyourcloning_linkml/schema/shareyourcloning_linkml.yaml`

 * *Files identical despite different names*

### Comparing `shareyourcloning_linkml-0.1.5.1a0/PKG-INFO` & `shareyourcloning_linkml-0.1.5a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareyourcloning-linkml
-Version: 0.1.5.1a0
+Version: 0.1.5a0
 Summary: A LinkML data model for ShareYourCloning
 Home-page: https://github.com/genestorian/ShareYourCloning_LinkML
 License: MIT
 Author: Manuel Lera-Ramirez
 Author-email: manuel.lera-ramirez@ucl.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

