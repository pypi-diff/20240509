# Comparing `tmp/slalom_tapdance-1.0.1.dev67.tar.gz` & `tmp/slalom_tapdance-1.0.1.dev68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-1.0.1.dev67.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.1.dev68.tar", max compression
```

## Comparing `slalom_tapdance-1.0.1.dev67.tar` & `slalom_tapdance-1.0.1.dev68.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-08 20:38:58.029229 slalom_tapdance-1.0.1.dev67/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-08 20:39:23.293231 slalom_tapdance-1.0.1.dev67/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/install_helper.py
--rw-r--r--   0        0        0    38121 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/states.py
--rw-r--r--   0        0        0    12133 2024-05-08 20:38:58.033229 slalom_tapdance-1.0.1.dev67/tapdance/syncs.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev67/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-08 20:45:18.333261 slalom_tapdance-1.0.1.dev68/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-08 20:45:33.809463 slalom_tapdance-1.0.1.dev68/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-08 20:45:18.337261 slalom_tapdance-1.0.1.dev68/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-08 20:45:18.337261 slalom_tapdance-1.0.1.dev68/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-08 20:45:18.337261 slalom_tapdance-1.0.1.dev68/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-08 20:45:18.337261 slalom_tapdance-1.0.1.dev68/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-08 20:45:18.337261 slalom_tapdance-1.0.1.dev68/tapdance/install_helper.py
+-rw-r--r--   0        0        0    38026 2024-05-08 20:45:18.341261 slalom_tapdance-1.0.1.dev68/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-08 20:45:18.341261 slalom_tapdance-1.0.1.dev68/tapdance/states.py
+-rw-r--r--   0        0        0    12102 2024-05-08 20:45:18.341261 slalom_tapdance-1.0.1.dev68/tapdance/syncs.py
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev68/PKG-INFO
```

### Comparing `slalom_tapdance-1.0.1.dev67/LICENSE` & `slalom_tapdance-1.0.1.dev68/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev67/pyproject.toml` & `slalom_tapdance-1.0.1.dev68/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "1.0.1-dev.67"
+version = "1.0.1-dev.68"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-1.0.1.dev67/tapdance/cli.py` & `slalom_tapdance-1.0.1.dev68/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev67/tapdance/config.py` & `slalom_tapdance-1.0.1.dev68/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev67/tapdance/docker.py` & `slalom_tapdance-1.0.1.dev68/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev67/tapdance/install_helper.py` & `slalom_tapdance-1.0.1.dev68/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev67/tapdance/plans.py` & `slalom_tapdance-1.0.1.dev68/tapdance/plans.py`

 * *Files 1% similar despite different names*

```diff
@@ -632,15 +632,15 @@
     matches: Dict[str, Dict[str, bool]],
     primary_keys: Dict[str, List[str]],
     replication_keys: Dict[str, List[str]],
     table_stream_ids: Dict[str, str],
     excluded_table_stream_ids: Dict[str, List[str]],
 ) -> str:
     """
-    Creates the test for the plan file that will be written to the file.
+    Creates the text for the plan file
     """
     sorted_tables = sorted(matches.keys())
     file_text = ""
     file_text += "selected_tables:\n"
     for table in sorted_tables:
         stream_id = table_stream_ids[table]
         primary_key_cols: List[str] = primary_keys[table]
@@ -843,33 +843,32 @@
 
 
 @logged(
     "selecting '{table_name}' catalog metadata "
     "from '{tap_name}' source catalog file: {full_catalog_file}"
 )
 def _create_table_catalog(
-    #could alter the catalog here
     tap_name: str,
     table_name: str,
     full_catalog_file: str = None,
     output_file: str = None,
     all_table_catalog: bool = False
 ) -> None:
     """
-    Create an individual catalog for a stream
+    Create an individual catalog for each stream. 
     """
     taps_dir = config.get_taps_dir()
     catalog_dir = config.get_tap_output_dir(tap_name, taps_dir)
     source_catalog_path = full_catalog_file or os.path.join(
         catalog_dir, "catalog-selected.json"
     )
     output_file = output_file or os.path.join(catalog_dir, f"{table_name}-catalog.json")
     included_table_objects = []
     catalog_full = json.loads(Path(source_catalog_path).read_text())
-    # Loop through all the tables in the catalog until we find the current table
+    # Loop through all the tables in the catalog
     for tbl in catalog_full["streams"]:
         stream_name = _get_stream_name(tbl)
         # Always add the current table to it's catalog
         if stream_name in table_name:
             _get_stream_metadata_object(tbl)["selected"] = True
             logging.info(f'Adding current table:{table_name} to catalog.')
             included_table_objects.append(tbl)
```

### Comparing `slalom_tapdance-1.0.1.dev67/tapdance/states.py` & `slalom_tapdance-1.0.1.dev68/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev67/tapdance/syncs.py` & `slalom_tapdance-1.0.1.dev68/tapdance/syncs.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,14 @@
 
     config.print_plugin_version(tap_exe,target_exe)
 
     replication_strategy = replication_strategy or tap_settings.get(
         "REPLICATION_STRATEGY", "INCREMENTAL"
     )
 
-    logging.info(tap_settings)
     is_parent_child_tap = tap_settings.get("IS_PARENT_CHILD_TAP", False)
 
     config.validate_replication_strategy(replication_strategy)
 
     #could use something here to identify a parent child table
     table_name = table_name or tap_settings.get("TABLE_NAME", None)
     exclude_tables = exclude_tables or tap_settings.get("EXCLUDE_TABLES", None)
```

### Comparing `slalom_tapdance-1.0.1.dev67/PKG-INFO` & `slalom_tapdance-1.0.1.dev68/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 1.0.1.dev67
+Version: 1.0.1.dev68
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

