# Comparing `tmp/slalom_tapdance-1.0.1.dev71.tar.gz` & `tmp/slalom_tapdance-1.0.1.dev72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-1.0.1.dev71.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.1.dev72.tar", max compression
```

## Comparing `slalom_tapdance-1.0.1.dev71.tar` & `slalom_tapdance-1.0.1.dev72.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-09 18:34:32.896958 slalom_tapdance-1.0.1.dev71/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-09 18:34:50.136812 slalom_tapdance-1.0.1.dev71/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/install_helper.py
--rw-r--r--   0        0        0    38026 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/states.py
--rw-r--r--   0        0        0    11998 2024-05-09 18:34:32.900958 slalom_tapdance-1.0.1.dev71/tapdance/syncs.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev71/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-09 18:41:45.249899 slalom_tapdance-1.0.1.dev72/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-09 18:41:59.001820 slalom_tapdance-1.0.1.dev72/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-09 18:41:45.253899 slalom_tapdance-1.0.1.dev72/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-09 18:41:45.253899 slalom_tapdance-1.0.1.dev72/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-09 18:41:45.253899 slalom_tapdance-1.0.1.dev72/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-09 18:41:45.253899 slalom_tapdance-1.0.1.dev72/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-09 18:41:45.253899 slalom_tapdance-1.0.1.dev72/tapdance/install_helper.py
+-rw-r--r--   0        0        0    38838 2024-05-09 18:41:45.253899 slalom_tapdance-1.0.1.dev72/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-09 18:41:45.253899 slalom_tapdance-1.0.1.dev72/tapdance/states.py
+-rw-r--r--   0        0        0    11998 2024-05-09 18:41:45.253899 slalom_tapdance-1.0.1.dev72/tapdance/syncs.py
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev72/PKG-INFO
```

### Comparing `slalom_tapdance-1.0.1.dev71/LICENSE` & `slalom_tapdance-1.0.1.dev72/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev71/pyproject.toml` & `slalom_tapdance-1.0.1.dev72/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "1.0.1-dev.71"
+version = "1.0.1-dev.72"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-1.0.1.dev71/tapdance/cli.py` & `slalom_tapdance-1.0.1.dev72/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev71/tapdance/config.py` & `slalom_tapdance-1.0.1.dev72/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev71/tapdance/docker.py` & `slalom_tapdance-1.0.1.dev72/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev71/tapdance/install_helper.py` & `slalom_tapdance-1.0.1.dev72/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev71/tapdance/plans.py` & `slalom_tapdance-1.0.1.dev72/tapdance/plans.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,51 +380,65 @@
         )
     return result
 
 
 def _get_rules_file_keys(
     key_type: str, matches: Dict[str, Dict[str, bool]], rules_file: str,
 ) -> Dict[str, List[str]]:
+    """Return a Dictionary of table names and columns that contain an 
+       override in the Rules file that match the provided key type. 
+    
+    """
     result: Dict[str, List[str]] = {}
     if key_type not in ["primary-key", "replication-key"]:
         raise ValueError(
             f"Unexpected key type '{key_type}'. "
             "Expected: 'replication-key' or 'primary-key'"
         )
     # Check rules_file to fill `matches`
     plan_file_lines = uio.get_text_file_contents(rules_file).splitlines()
-    #Key Overrides
+    # Loop through the contents of the rules file and check if each line contains an override
     key_overrides = [
         line.split("->")[0].rstrip()
         for line in plan_file_lines
         if "->" in line and line.split("->")[1].lstrip().rstrip() == key_type
     ]
     for key_spec in key_overrides:
+        # Check to see if the override is formatted correctly
         if len(key_spec.split(".")) != 2 or "*" in key_spec:
             raise ValueError(
                 f"Expected '{key_type}' indicator with exact two-part key, separated "
                 f"by '.'.  Found '{key_spec}'"
             )
         table_name, key_col_name = key_spec.split(".")
+        # Check that the column is on the table
         if table_name not in matches:
             raise ValueError(f"Could not locate table '{table_name}' in selected list.")
         if key_col_name not in matches[table_name]:
             raise ValueError(f"Key column '{key_spec}' is not in column list.")
         elif not matches[table_name][key_col_name]:
             raise ValueError(f"Key column '{key_spec}' is not a selected column.")
-        result[table_name] = [key_col_name]
+        # Add the column to the table key in the dictionary
+        # If the table is already in the result dictionary, append the new column to the list. 
+        if table_name in result:
+            result[table_name].append(key_col_name)
+        else:
+            result[table_name] = [key_col_name]
     return result
 
 
 def _get_table_keys(
     matches: Dict[str, Dict[str, bool]],
     matched_stream_ids: Dict[str, str],
     catalog_file: str,
     rules_file: str,
 ) -> Tuple[Dict[str, List[str]], Dict[str, List[str]]]:
+    """
+    
+    """
     primary_keys: Dict[str, List[str]] = {}
     replication_keys: Dict[str, List[str]] = {}
     stream_name_lookup = {v: k for k, v in matched_stream_ids.items()}
     for key_type, collection in [
         ("primary-key", primary_keys),
         ("replication-key", replication_keys),
     ]:
@@ -432,17 +446,20 @@
             _get_catalog_file_keys(
                 key_type,
                 matches=matches,
                 matched_stream_ids=matched_stream_ids,
                 catalog_file=catalog_file,
             )
         )
+        # Get a dictionary of table names with their overrides from the rules file
         key_overrides = _get_rules_file_keys(
             key_type, matches=matches, rules_file=rules_file
         )
+        # Loop through the Key override dict and replace the Keys that we got 
+        # from the catalog file
         for table, override in key_overrides.items():
             if table.startswith('"'):
                 table = stream_name_lookup[table.lstrip('"').rstrip('"')]
             collection[table] = override
     return primary_keys, replication_keys
```

### Comparing `slalom_tapdance-1.0.1.dev71/tapdance/states.py` & `slalom_tapdance-1.0.1.dev72/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev71/tapdance/syncs.py` & `slalom_tapdance-1.0.1.dev72/tapdance/syncs.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev71/PKG-INFO` & `slalom_tapdance-1.0.1.dev72/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 1.0.1.dev71
+Version: 1.0.1.dev72
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

