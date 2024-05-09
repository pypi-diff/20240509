# Comparing `tmp/slalom_tapdance-1.0.1.dev68.tar.gz` & `tmp/slalom_tapdance-1.0.1.dev69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-1.0.1.dev68.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.1.dev69.tar", max compression
```

## Comparing `slalom_tapdance-1.0.1.dev68.tar` & `slalom_tapdance-1.0.1.dev69.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-08 20:45:18.333261 slalom_tapdance-1.0.1.dev68/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-08 20:45:33.809463 slalom_tapdance-1.0.1.dev68/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-08 20:45:18.337261 slalom_tapdance-1.0.1.dev68/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-08 20:45:18.337261 slalom_tapdance-1.0.1.dev68/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-08 20:45:18.337261 slalom_tapdance-1.0.1.dev68/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-08 20:45:18.337261 slalom_tapdance-1.0.1.dev68/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-08 20:45:18.337261 slalom_tapdance-1.0.1.dev68/tapdance/install_helper.py
--rw-r--r--   0        0        0    38026 2024-05-08 20:45:18.341261 slalom_tapdance-1.0.1.dev68/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-08 20:45:18.341261 slalom_tapdance-1.0.1.dev68/tapdance/states.py
--rw-r--r--   0        0        0    12102 2024-05-08 20:45:18.341261 slalom_tapdance-1.0.1.dev68/tapdance/syncs.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev68/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-09 16:04:11.222231 slalom_tapdance-1.0.1.dev69/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-09 16:04:27.345911 slalom_tapdance-1.0.1.dev69/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/install_helper.py
+-rw-r--r--   0        0        0    38026 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/states.py
+-rw-r--r--   0        0        0    12043 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/syncs.py
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev69/PKG-INFO
```

### Comparing `slalom_tapdance-1.0.1.dev68/LICENSE` & `slalom_tapdance-1.0.1.dev69/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev68/pyproject.toml` & `slalom_tapdance-1.0.1.dev69/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "1.0.1-dev.68"
+version = "1.0.1-dev.69"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-1.0.1.dev68/tapdance/cli.py` & `slalom_tapdance-1.0.1.dev69/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev68/tapdance/config.py` & `slalom_tapdance-1.0.1.dev69/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev68/tapdance/docker.py` & `slalom_tapdance-1.0.1.dev69/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev68/tapdance/install_helper.py` & `slalom_tapdance-1.0.1.dev69/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev68/tapdance/plans.py` & `slalom_tapdance-1.0.1.dev69/tapdance/plans.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev68/tapdance/states.py` & `slalom_tapdance-1.0.1.dev69/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev68/tapdance/syncs.py` & `slalom_tapdance-1.0.1.dev69/tapdance/syncs.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,15 @@
     replication_strategy = replication_strategy or tap_settings.get(
         "REPLICATION_STRATEGY", "INCREMENTAL"
     )
 
     is_parent_child_tap = tap_settings.get("IS_PARENT_CHILD_TAP", False)
 
     config.validate_replication_strategy(replication_strategy)
-
-    #could use something here to identify a parent child table
+    
     table_name = table_name or tap_settings.get("TABLE_NAME", None)
     exclude_tables = exclude_tables or tap_settings.get("EXCLUDE_TABLES", None)
     rules_file = config.get_rules_file(taps_dir, tap_name)
 
     # TODO: Resolve bug in Windows STDERR inclusion when emitting catalog json from
     #       docker run
     # if dockerized is None:
```

### Comparing `slalom_tapdance-1.0.1.dev68/PKG-INFO` & `slalom_tapdance-1.0.1.dev69/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 1.0.1.dev68
+Version: 1.0.1.dev69
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

