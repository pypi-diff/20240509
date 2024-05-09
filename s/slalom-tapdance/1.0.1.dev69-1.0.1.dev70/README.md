# Comparing `tmp/slalom_tapdance-1.0.1.dev69.tar.gz` & `tmp/slalom_tapdance-1.0.1.dev70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-1.0.1.dev69.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.1.dev70.tar", max compression
```

## Comparing `slalom_tapdance-1.0.1.dev69.tar` & `slalom_tapdance-1.0.1.dev70.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-09 16:04:11.222231 slalom_tapdance-1.0.1.dev69/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-09 16:04:27.345911 slalom_tapdance-1.0.1.dev69/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/install_helper.py
--rw-r--r--   0        0        0    38026 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/states.py
--rw-r--r--   0        0        0    12043 2024-05-09 16:04:11.226231 slalom_tapdance-1.0.1.dev69/tapdance/syncs.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev69/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-09 18:31:46.174534 slalom_tapdance-1.0.1.dev70/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-09 18:32:02.534739 slalom_tapdance-1.0.1.dev70/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/install_helper.py
+-rw-r--r--   0        0        0    38026 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/states.py
+-rw-r--r--   0        0        0    11998 2024-05-09 18:31:46.178535 slalom_tapdance-1.0.1.dev70/tapdance/syncs.py
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.1.dev70/PKG-INFO
```

### Comparing `slalom_tapdance-1.0.1.dev69/LICENSE` & `slalom_tapdance-1.0.1.dev70/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev69/pyproject.toml` & `slalom_tapdance-1.0.1.dev70/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "1.0.1-dev.69"
+version = "1.0.1-dev.70"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-1.0.1.dev69/tapdance/cli.py` & `slalom_tapdance-1.0.1.dev70/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev69/tapdance/config.py` & `slalom_tapdance-1.0.1.dev70/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev69/tapdance/docker.py` & `slalom_tapdance-1.0.1.dev70/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev69/tapdance/install_helper.py` & `slalom_tapdance-1.0.1.dev70/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev69/tapdance/plans.py` & `slalom_tapdance-1.0.1.dev70/tapdance/plans.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev69/tapdance/states.py` & `slalom_tapdance-1.0.1.dev70/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.1.dev69/tapdance/syncs.py` & `slalom_tapdance-1.0.1.dev70/tapdance/syncs.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,14 @@
     pipeline_version_num = config.get_pipeline_version_number()
     table_state_file = config.replace_placeholders(
         {"table_state_file": table_state_file},
         tap_name,
         table_name,
         pipeline_version_num,
     )["table_state_file"]
-    logging.warning(f'{table_catalog_file}')
     tap_args = f"--config {config_file} --catalog {table_catalog_file} "
     if s3_file_exists(table_state_file):
         local_state_file_in = os.path.join(
             config.get_tap_output_dir(tap_name, taps_dir),
             f"{tap_name}-{table_name}-state.json",
         )
         if not uio.get_text_file_contents(table_state_file):
```

### Comparing `slalom_tapdance-1.0.1.dev69/PKG-INFO` & `slalom_tapdance-1.0.1.dev70/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 1.0.1.dev69
+Version: 1.0.1.dev70
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

