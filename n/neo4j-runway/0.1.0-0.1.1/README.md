# Comparing `tmp/neo4j_runway-0.1.0.tar.gz` & `tmp/neo4j_runway-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4j_runway-0.1.0.tar", max compression
+gzip compressed data, was "neo4j_runway-0.1.1.tar", max compression
```

## Comparing `neo4j_runway-0.1.0.tar` & `neo4j_runway-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11354 2024-05-01 12:35:47.639470 neo4j_runway-0.1.0/LICENSE
--rw-r--r--   0        0        0     4725 2024-05-01 18:05:02.618828 neo4j_runway-0.1.0/README.md
--rw-r--r--   0        0        0      205 2024-05-01 12:25:23.214243 neo4j_runway-0.1.0/neo4j_runway/__init__.py
--rw-r--r--   0        0        0       33 2024-04-29 23:04:42.985466 neo4j_runway-0.1.0/neo4j_runway/discovery/__init__.py
--rw-r--r--   0        0        0     3211 2024-05-02 13:25:34.948014 neo4j_runway-0.1.0/neo4j_runway/discovery/discovery.py
--rw-r--r--   0        0        0       79 2024-04-29 23:04:42.986387 neo4j_runway-0.1.0/neo4j_runway/ingestion/__init__.py
--rw-r--r--   0        0        0    10822 2024-05-02 11:43:53.432510 neo4j_runway-0.1.0/neo4j_runway/ingestion/generate_ingest.py
--rwxr-xr-x   0        0        0     3503 2024-05-01 12:25:23.215248 neo4j_runway-0.1.0/neo4j_runway/ingestion/pyingest.py
--rw-r--r--   0        0        0       21 2024-04-29 23:04:42.987658 neo4j_runway-0.1.0/neo4j_runway/llm/__init__.py
--rw-r--r--   0        0        0     4543 2024-05-01 12:25:23.215746 neo4j_runway-0.1.0/neo4j_runway/llm/llm.py
--rw-r--r--   0        0        0       38 2024-04-29 23:04:42.988650 neo4j_runway-0.1.0/neo4j_runway/modeler/__init__.py
--rw-r--r--   0        0        0     7948 2024-05-02 13:25:34.960509 neo4j_runway-0.1.0/neo4j_runway/modeler/modeler.py
--rw-r--r--   0        0        0      229 2024-05-02 11:43:53.434393 neo4j_runway-0.1.0/neo4j_runway/objects/__init__.py
--rw-r--r--   0        0        0     5681 2024-05-02 11:43:53.434996 neo4j_runway-0.1.0/neo4j_runway/objects/arrows.py
--rw-r--r--   0        0        0    11004 2024-05-02 11:43:53.435687 neo4j_runway-0.1.0/neo4j_runway/objects/data_model.py
--rw-r--r--   0        0        0     4403 2024-05-01 14:55:46.065975 neo4j_runway-0.1.0/neo4j_runway/objects/node.py
--rw-r--r--   0        0        0     1693 2024-05-02 13:25:34.944947 neo4j_runway-0.1.0/neo4j_runway/objects/property.py
--rw-r--r--   0        0        0     4422 2024-05-02 11:43:53.436385 neo4j_runway-0.1.0/neo4j_runway/objects/relationship.py
--rw-r--r--   0        0        0      904 2024-05-02 11:43:53.436909 neo4j_runway-0.1.0/neo4j_runway/objects/user_input.py
--rw-r--r--   0        0        0     2205 2024-04-29 23:04:42.992114 neo4j_runway-0.1.0/neo4j_runway/resources/prompts/prompts.py
--rw-r--r--   0        0        0      138 2024-04-29 23:04:43.003742 neo4j_runway-0.1.0/neo4j_runway/utils/__init__.py
--rw-r--r--   0        0        0     3429 2024-04-29 23:04:43.003938 neo4j_runway-0.1.0/neo4j_runway/utils/naming_conventions.py
--rw-r--r--   0        0        0      917 2024-05-01 12:25:23.223161 neo4j_runway-0.1.0/neo4j_runway/utils/test_connection.py
--rw-r--r--   0        0        0     1116 2024-05-06 15:16:50.346236 neo4j_runway-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6015 1970-01-01 00:00:00.000000 neo4j_runway-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-05-01 12:35:47.639470 neo4j_runway-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4725 2024-05-01 18:05:02.618828 neo4j_runway-0.1.1/README.md
+-rw-r--r--   0        0        0      205 2024-05-01 12:25:23.214243 neo4j_runway-0.1.1/neo4j_runway/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-29 23:04:42.985466 neo4j_runway-0.1.1/neo4j_runway/discovery/__init__.py
+-rw-r--r--   0        0        0     3211 2024-05-02 13:25:34.948014 neo4j_runway-0.1.1/neo4j_runway/discovery/discovery.py
+-rw-r--r--   0        0        0       79 2024-04-29 23:04:42.986387 neo4j_runway-0.1.1/neo4j_runway/ingestion/__init__.py
+-rw-r--r--   0        0        0    11693 2024-05-09 14:23:16.900284 neo4j_runway-0.1.1/neo4j_runway/ingestion/generate_ingest.py
+-rwxr-xr-x   0        0        0     3503 2024-05-01 12:25:23.215248 neo4j_runway-0.1.1/neo4j_runway/ingestion/pyingest.py
+-rw-r--r--   0        0        0       21 2024-04-29 23:04:42.987658 neo4j_runway-0.1.1/neo4j_runway/llm/__init__.py
+-rw-r--r--   0        0        0     4543 2024-05-01 12:25:23.215746 neo4j_runway-0.1.1/neo4j_runway/llm/llm.py
+-rw-r--r--   0        0        0       38 2024-04-29 23:04:42.988650 neo4j_runway-0.1.1/neo4j_runway/modeler/__init__.py
+-rw-r--r--   0        0        0     7948 2024-05-02 13:25:34.960509 neo4j_runway-0.1.1/neo4j_runway/modeler/modeler.py
+-rw-r--r--   0        0        0      229 2024-05-02 11:43:53.434393 neo4j_runway-0.1.1/neo4j_runway/objects/__init__.py
+-rw-r--r--   0        0        0     5681 2024-05-09 15:42:41.632781 neo4j_runway-0.1.1/neo4j_runway/objects/arrows.py
+-rw-r--r--   0        0        0    11004 2024-05-09 15:42:40.024287 neo4j_runway-0.1.1/neo4j_runway/objects/data_model.py
+-rw-r--r--   0        0        0     3320 2024-05-09 16:05:18.875638 neo4j_runway-0.1.1/neo4j_runway/objects/node.py
+-rw-r--r--   0        0        0     2851 2024-05-09 16:05:18.876065 neo4j_runway-0.1.1/neo4j_runway/objects/property.py
+-rw-r--r--   0        0        0     3587 2024-05-09 16:05:18.876546 neo4j_runway-0.1.1/neo4j_runway/objects/relationship.py
+-rw-r--r--   0        0        0      904 2024-05-02 11:43:53.436909 neo4j_runway-0.1.1/neo4j_runway/objects/user_input.py
+-rw-r--r--   0        0        0     2205 2024-04-29 23:04:42.992114 neo4j_runway-0.1.1/neo4j_runway/resources/prompts/prompts.py
+-rw-r--r--   0        0        0      138 2024-04-29 23:04:43.003742 neo4j_runway-0.1.1/neo4j_runway/utils/__init__.py
+-rw-r--r--   0        0        0     3429 2024-04-29 23:04:43.003938 neo4j_runway-0.1.1/neo4j_runway/utils/naming_conventions.py
+-rw-r--r--   0        0        0      917 2024-05-01 12:25:23.223161 neo4j_runway-0.1.1/neo4j_runway/utils/test_connection.py
+-rw-r--r--   0        0        0     1116 2024-05-09 16:05:34.918238 neo4j_runway-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6015 1970-01-01 00:00:00.000000 neo4j_runway-0.1.1/PKG-INFO
```

### Comparing `neo4j_runway-0.1.0/LICENSE` & `neo4j_runway-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.0/README.md` & `neo4j_runway-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.0/neo4j_runway/discovery/discovery.py` & `neo4j_runway-0.1.1/neo4j_runway/discovery/discovery.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.0/neo4j_runway/ingestion/generate_ingest.py` & `neo4j_runway-0.1.1/neo4j_runway/ingestion/generate_ingest.py`

 * *Files 8% similar despite different names*

```diff
@@ -59,17 +59,16 @@
         self.database: Union[str, None] = database
         self.csv_name: str = csv_name
         self.csv_dir: str = csv_dir
         self.file_output_dir: str = file_output_dir
         self._config_files_list: Union[List[Dict[str, Any]], None] = []
         self._constraints: Dict[str, str] = {}
         self._cypher_map: Dict[str, Dict[str, Any]] = {}
-        self._generate_base_information()
 
-    def _generate_base_information(self):
+    def _generate_base_information(self, method: str = "api", batch_size: int = 100):
         for node in self.data_model.nodes:
             if len(node.unique_properties_column_mapping) > 0:
                 for unique_property in node.unique_properties:
                     self._constraints[
                         generate_constraints_key(
                             label_or_type=node.label, unique_property=unique_property
                         )
@@ -80,15 +79,18 @@
             # add to cypher map
             self._cypher_map[lowercase_first_letter(node.label)] = {
                 "cypher": literal_unicode(
                     generate_merge_node_clause_standard(node=node)
                 ),
                 "cypher_loadcsv": literal_unicode(
                     generate_merge_node_load_csv_clause(
-                        node=node, csv_name=self.csv_name
+                        node=node,
+                        csv_name=self.csv_name,
+                        method=method,
+                        batch_size=batch_size,
                     )
                 ),
                 "csv": f"$BASE/{self.csv_dir}{self.csv_name}",
             }
 
         ## get relationships
         for rel in self.data_model.relationships:
@@ -112,44 +114,50 @@
                 ),
                 "cypher_loadcsv": literal_unicode(
                     generate_merge_relationship_load_csv_clause(
                         relationship=rel,
                         source_node=source,
                         target_node=target,
                         csv_name=self.csv_name,
+                        method=method,
+                        batch_size=batch_size,
                     )
                 ),
                 "csv": f"$BASE/{self.csv_dir}{self.csv_name}",
             }
 
         self._config_files_list = []
         for item in self._cypher_map:
             file_dict = {}
             if self._cypher_map[item]["csv"]:
                 file_dict["url"] = self._cypher_map[item]["csv"]
                 file_dict["cql"] = self._cypher_map[item]["cypher"]
-                file_dict["chunk_size"] = 100
+                file_dict["chunk_size"] = batch_size
                 self._config_files_list.append(file_dict)
 
-    def generate_pyingest_yaml_file(self, file_name: str = "pyingest_config") -> None:
+    def generate_pyingest_yaml_file(
+        self, file_name: str = "pyingest_config", batch_size: int = 100
+    ) -> None:
         """
         Generate the PyIngest yaml file.
         """
 
         if self.file_output_dir != "":
             os.makedirs(self.file_output_dir, exist_ok=True)
 
         with open(f"./{self.file_output_dir}{file_name}.yml", "w") as config_yaml:
-            config_yaml.write(self.generate_pyingest_yaml_string())
+            config_yaml.write(self.generate_pyingest_yaml_string(batch_size=batch_size))
 
-    def generate_pyingest_yaml_string(self) -> str:
+    def generate_pyingest_yaml_string(self, batch_size: int = 100) -> str:
         """
         Generate the PyIngest yaml in string format.
         """
 
+        self._generate_base_information(batch_size=batch_size)
+
         final_yaml = {}
         final_yaml["files"] = self._config_files_list
         config_dump = yaml.dump(final_yaml)
 
         to_return = (
             f"server_uri: {self.uri}\n"
             + f"admin_user: {self.username}\n"
@@ -177,36 +185,49 @@
         ) as constraints_cypher:
             constraints_cypher.write(self.generate_constraints_cypher_string())
 
     def generate_constraints_cypher_string(self) -> str:
         """
         Generate the Constraints cypher file in string format.
         """
+
+        if not self._constraints:
+            self._generate_base_information()
+
         to_return = ""
 
         for constraint in self._constraints:
             to_return = to_return + self._constraints[constraint]
 
         return to_return
 
-    def generate_load_csv_file(self, file_name: str = "load_csv") -> None:
+    def generate_load_csv_file(
+        self, file_name: str = "load_csv", batch_size: int = 100, method: str = "api"
+    ) -> None:
         """
         Generate the load_csv cypher file.
         """
 
         if self.file_output_dir != "":
             os.makedirs(self.file_output_dir, exist_ok=True)
 
         with open(f"./{self.file_output_dir}{file_name}.cypher", "w") as load_csv_file:
-            load_csv_file.write(self.generate_load_csv_string())
-
-    def generate_load_csv_string(self) -> str:
+            load_csv_file.write(
+                self.generate_load_csv_string(batch_size=batch_size, method=method)
+            )
+
+    def generate_load_csv_string(
+        self, batch_size: int = 100, method: str = "api"
+    ) -> str:
         """
         Generate the load_csv cypher in string format.
         """
+
+        self._generate_base_information(batch_size=batch_size, method=method)
+
         to_return = ""
 
         for constraint in self._constraints:
             to_return = to_return + self._constraints[constraint]
 
         for item in self._cypher_map:
             to_return = to_return + self._cypher_map[item]["cypher_loadcsv"]
@@ -287,21 +308,23 @@
 MERGE (n:{node.label} {{{generate_set_unique_property(node.unique_properties_column_mapping)}}})
 {generate_set_property(node.nonunique_properties_column_mapping)}"""
 
 
 def generate_merge_node_load_csv_clause(
     node: Node,
     csv_name: str,
+    method: str = "api",
     batch_size: int = 10000,
 ) -> str:
     """
     Generate a MERGE node clause for the LOAD CSV method.
     """
 
-    return f"""LOAD CSV WITH HEADERS FROM 'file:///{csv_name}' as row
+    command = ":auto " if method == "browser" else ""
+    return f"""{command}LOAD CSV WITH HEADERS FROM 'file:///{csv_name}' as row
 CALL {{
     WITH row
     MERGE (n:{node.label} {{{generate_set_unique_property(node.unique_properties_column_mapping)}}})
     {generate_set_property(node.nonunique_properties_column_mapping)}
 }} IN TRANSACTIONS OF {str(batch_size)} ROWS;
 """
 
@@ -322,21 +345,23 @@
 
 
 def generate_merge_relationship_load_csv_clause(
     relationship: Relationship,
     source_node: Node,
     target_node: Node,
     csv_name: str,
+    method: str = "api",
     batch_size: int = 10000,
 ) -> str:
     """
     Generate a MERGE relationship clause for the LOAD CSV method.
     """
 
-    return f"""LOAD CSV WITH HEADERS FROM 'file:///{csv_name}' as row
+    command = ":auto " if method == "browser" else ""
+    return f"""{command}LOAD CSV WITH HEADERS FROM 'file:///{csv_name}' as row
 CALL {{
     WITH row
     {generate_match_node_clause(source_node).replace('(n:', '(source:')}
     {generate_match_node_clause(target_node).replace('(n:', '(target:')}
     MERGE (source)-[n:{relationship.type}]->(target)
     {generate_set_property(relationship.nonunique_properties_column_mapping)}
 }} IN TRANSACTIONS OF {str(batch_size)} ROWS;
```

### Comparing `neo4j_runway-0.1.0/neo4j_runway/ingestion/pyingest.py` & `neo4j_runway-0.1.1/neo4j_runway/ingestion/pyingest.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.0/neo4j_runway/llm/llm.py` & `neo4j_runway-0.1.1/neo4j_runway/llm/llm.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.0/neo4j_runway/modeler/modeler.py` & `neo4j_runway-0.1.1/neo4j_runway/modeler/modeler.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.0/neo4j_runway/objects/arrows.py` & `neo4j_runway-0.1.1/neo4j_runway/objects/arrows.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.0/neo4j_runway/objects/data_model.py` & `neo4j_runway-0.1.1/neo4j_runway/objects/data_model.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.0/neo4j_runway/objects/node.py` & `neo4j_runway-0.1.1/neo4j_runway/objects/node.py`

 * *Files 24% similar despite different names*

```diff
@@ -99,43 +99,12 @@
     @classmethod
     def from_arrows(cls, arrows_node: ArrowsNode):
         """
         Initialize a Node from an arrows node.
         """
 
         props = [
-            cls._parse_arrows_property(
-                arrows_property={k: v}, arrows_node_caption=arrows_node.caption
-            )
+            Property.from_arrows(arrows_property={k: v}, caption=arrows_node.caption)
             for k, v in arrows_node.properties.items()
         ]
         # support only single labels for now, take first label
-        return cls(label=arrows_node.labels[0], properties=props)
-
-    @staticmethod
-    def _parse_arrows_property(
-        arrows_property: Dict[str, str], arrows_node_caption: str
-    ) -> Property:
-        """
-        Parse the arrows property representation into a standard Property model.
-        Unique property names are stored in the nodes caption as a comma-separated list: List<str>.
-        Arrow property values are formatted as <csv_mapping> | <python_type>.
-        """
-
-        if "|" in list(arrows_property.values())[0]:
-            csv_mapping, python_type = [
-                x.strip() for x in list(arrows_property.values())[0].split("|")
-            ]
-        else:
-            csv_mapping = list(arrows_property.values())[0]
-            python_type = "unknown"
-
-        is_unique = list(arrows_property.keys())[0] in [
-            x.strip() for x in arrows_node_caption.split(",")
-        ]
-
-        return Property(
-            name=list(arrows_property.keys())[0],
-            csv_mapping=csv_mapping,
-            type=python_type,
-            is_unique=is_unique,
-        )
+        return cls(label=arrows_node.labels[0], properties=props)
```

### Comparing `neo4j_runway-0.1.0/neo4j_runway/objects/user_input.py` & `neo4j_runway-0.1.1/neo4j_runway/objects/user_input.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.0/neo4j_runway/resources/prompts/prompts.py` & `neo4j_runway-0.1.1/neo4j_runway/resources/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.0/neo4j_runway/utils/naming_conventions.py` & `neo4j_runway-0.1.1/neo4j_runway/utils/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.0/neo4j_runway/utils/test_connection.py` & `neo4j_runway-0.1.1/neo4j_runway/utils/test_connection.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.1.0/pyproject.toml` & `neo4j_runway-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neo4j-runway"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Python library that contains tools for data discovery, data model generation and ingestion for the Neo4j graph database."
 authors = ["Alex Gilmore", "Jason Booth", "Dan Bukowski"]
 license = "MIT"
 readme = "README.md"
 keywords = ["graph", "neo4j", "data model"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `neo4j_runway-0.1.0/PKG-INFO` & `neo4j_runway-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4j-runway
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library that contains tools for data discovery, data model generation and ingestion for the Neo4j graph database.
 License: MIT
 Keywords: graph,neo4j,data model
 Author: Alex Gilmore
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

