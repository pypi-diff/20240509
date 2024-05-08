# Comparing `tmp/ploomber-cloud-0.2.6.tar.gz` & `tmp/ploomber-cloud-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomber-cloud-0.2.6.tar", last modified: Fri May  3 16:11:24 2024, max compression
+gzip compressed data, was "ploomber-cloud-0.2.7.tar", last modified: Wed May  8 23:02:09 2024, max compression
```

## Comparing `ploomber-cloud-0.2.6.tar` & `ploomber-cloud-0.2.7.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:11:24.520578 ploomber-cloud-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 16:11:24.520578 ploomber-cloud-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-03 16:11:24.520578 ploomber-cloud-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:11:24.516578 ploomber-cloud-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:11:24.520578 ploomber-cloud-0.2.6/src/ploomber_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:11:24.520578 ploomber-cloud-0.2.6/src/ploomber_cloud/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:11:24.520578 ploomber-cloud-0.2.6/src/ploomber_cloud/assets/vllm/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/assets/vllm/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/assets/vllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/assets/vllm/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/assets/vllm/test-vllm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6851 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:11:24.520578 ploomber-cloud-0.2.6/src/ploomber_cloud/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/configurations/community.json
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/configurations/premium.json
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8269 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-03 16:11:08.000000 ploomber-cloud-0.2.6/src/ploomber_cloud/zip_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:11:24.520578 ploomber-cloud-0.2.6/src/ploomber_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-03 16:11:24.000000 ploomber-cloud-0.2.6/src/ploomber_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-03 16:11:24.000000 ploomber-cloud-0.2.6/src/ploomber_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:11:24.000000 ploomber-cloud-0.2.6/src/ploomber_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-03 16:11:24.000000 ploomber-cloud-0.2.6/src/ploomber_cloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-03 16:11:24.000000 ploomber-cloud-0.2.6/src/ploomber_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-03 16:11:24.000000 ploomber-cloud-0.2.6/src/ploomber_cloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     5291 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.142724 ploomber-cloud-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.146724 ploomber-cloud-0.2.7/src/ploomber_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6483 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/test-vllm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/src/ploomber_cloud/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/configurations/community.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/configurations/premium.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12131 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8884 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3975 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-05-08 23:01:55.000000 ploomber-cloud-0.2.7/src/ploomber_cloud/zip_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:02:09.150724 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-08 23:02:08.000000 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-08 23:02:08.000000 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 23:02:08.000000 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-08 23:02:08.000000 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-08 23:02:08.000000 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 23:02:08.000000 ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/top_level.txt
```

### Comparing `ploomber-cloud-0.2.6/CHANGELOG.md` & `ploomber-cloud-0.2.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # CHANGELOG
 
+## 0.2.7 (2024-05-08)
+
+- [Feature] Add `--clear-cache` option to `ploomber-cloud examples`.
+
 ## 0.2.6 (2024-05-03)
 
 - [Feature] Allow switching the config file to use via `--config/-c` in `init`, `deploy`, `templates`, `resources`, and `labels` subcommands
 
 ## 0.2.5 (2024-05-02)
 
 - [Feature] Add `--watch-incremental` option to `ploomber-cloud deploy`.
```

### Comparing `ploomber-cloud-0.2.6/pyproject.toml` & `ploomber-cloud-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/setup.py` & `ploomber-cloud-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/api.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/api.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/api_key.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/api_key.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/assets/vllm/requirements.txt` & `ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/requirements.txt`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/assets/vllm/test-vllm.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/assets/vllm/test-vllm.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/cli.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,18 +101,23 @@
 def github():
     """Configure workflow file for triggering
     GitHub actions"""
     github_.github()
 
 
 @cli.command()
+@click.option(
+    "--clear-cache",
+    is_flag=True,
+    help="Invalidate the examples metadata cache",
+)
 @click.argument("name", type=str, required=False)
-def examples(name):
+def examples(name, clear_cache):
     """Download an example from the doc repository"""
-    examples_.examples(name)
+    examples_.examples(name, clear_cache)
 
 
 @cli.command()
 @click.option("--project-id", "project_id", help="Project ID to delete", required=False)
 @click.option(
     "--all",
     "-a",
```

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/config.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import json
 from pathlib import Path
+import json
 from contextlib import contextmanager
 
 
+from dotenv import dotenv_values
+
 from ploomber_cloud.util import pretty_print, raise_error_on_duplicate_keys
 from ploomber_cloud.constants import VALID_PROJECT_TYPES, FORCE_INIT_MESSAGE
 from ploomber_cloud.exceptions import InvalidPloomberConfigException
+from ploomber_cloud.abc import PersistedMapping
 
 
 @contextmanager
 def path_to_config(path_new):
     """
     Context manager to temporarily change the path that PloomberCloudConfig uses to
     read/write the config file.
@@ -21,35 +24,19 @@
 
     try:
         yield
     finally:
         PloomberCloudConfig.PATH_TO_CONFIG = CURRENT_PATH
 
 
-class PloomberCloudConfig:
+class PloomberCloudConfig(PersistedMapping):
     """Manages the ploomber-cloud.json file"""
 
     PATH_TO_CONFIG = "ploomber-cloud.json"
 
-    def __init__(self) -> None:
-        self._path = Path(self.PATH_TO_CONFIG)
-        self._data = None
-
-    @property
-    def data(self):
-        """Return the data stored in the config file"""
-        if self._data is None:
-            raise RuntimeError("Data has not been loaded")
-
-        return self._data
-
-    def exists(self):
-        """Return True if the config file exists, False otherwise"""
-        return self._path.exists()
-
     def _validate_labels(self):
         if "labels" not in self._data.keys():
             return None
         for label in self._data["labels"]:
             if not isinstance(label, str):
                 return (
                     f"'labels' must be a list of strings. "
@@ -152,46 +139,53 @@
 
         if error:
             raise InvalidPloomberConfigException(
                 f"There are some issues with the ploomber-cloud.json file:\n{error}\n"
                 f"{FORCE_INIT_MESSAGE}\n"
             )
 
-    def load(self):
-        """
-        Load the config file. Accessing data will raise an error if this
-        method hasn't been executed
-        """
+    def _load(self):
         if not self.exists():
             raise InvalidPloomberConfigException(
                 "Project not initialized. "
                 "Run 'ploomber-cloud init' to initialize your project."
             )
 
         try:
-            self._data = json.loads(
+            return json.loads(
                 self._path.read_text(), object_pairs_hook=raise_error_on_duplicate_keys
             )
         except ValueError as e:
             error_message = "Please add a valid ploomber-cloud.json file."
             if "Duplicate keys" in str(e):
                 error_message = f"{error_message} {str(e)}"
             raise InvalidPloomberConfigException(
                 f"{error_message}\n{FORCE_INIT_MESSAGE}"
             ) from e
-        self._validate_config()
 
-    def dump(self, data_new):
+    def _dump(self, data_new):
         """Dump data to the config file"""
-        self._data = data_new
-        self._path.write_text(json.dumps(data_new, indent=4))
+        return json.dumps(data_new, indent=4)
+
+    def _validate_path(self, path_to_config):
+        if Path(path_to_config).suffix != ".json":
+            raise InvalidPloomberConfigException(
+                f"Invalid config file name: {path_to_config}. "
+                "Must have .json extension"
+            )
+
+
+class ProjectEnv(PersistedMapping):
+    PATH_TO_CONFIG = ".env"
+
+    def _validate_config(self):
+        pass
+
+    def _load(self):
+        return dotenv_values(self._path)
+
+    def _dump(self, data_new):
+        lines = [f"{key}={value}" for key, value in data_new.items()]
+        return "\n".join(lines)
 
-    def __setitem__(self, key, value):
-        self._data[key] = value
-        self._validate_config()
-        self.dump(self._data)
-
-    def __delitem__(self, key):
-        if key not in self._data:
-            raise InvalidPloomberConfigException(f"Key does not exist: {key}")
-        del self._data[key]
-        self.dump(self._data)
+    def _validate_path(self, path_to_config):
+        pass
```

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/configurations/community.json` & `ploomber-cloud-0.2.7/src/ploomber_cloud/configurations/community.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/configurations/premium.json` & `ploomber-cloud-0.2.7/src/ploomber_cloud/configurations/premium.json`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/constants.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/constants.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/delete.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/delete.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/deploy.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/deploy.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/examples.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/examples.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 HOME_PATH = Path("~", ".ploomber").expanduser()
 CLONED_REPO_PATH = HOME_PATH / "doc-repo"
 METADATA_PATH = HOME_PATH / ".ploomber-cloud-metadata"
 MISSING_API_KEY_MSG = """To deploy, you need an API key. Get one here:
 https://docs.cloud.ploomber.io/en/latest/quickstart/apikey.html \n
 Then run:\n$ ploomber-cloud key YOUR-KEY"""
 INVALID_CHOICE_ERROR_MSG = (
-    "Invalid example choice. "
+    "Invalid example choice. {reason}"
     "Command should be in the format:\n\n \
 $ ploomber-cloud examples framework/example-name\n\n \
 or to select from a menu of examples:\n\n \
-$ ploomber-cloud examples\n"
+$ ploomber-cloud examples\n\nTo clear the cache:\n\n \
+$ ploomber-cloud examples --clear-cache"
 )
 
 
 def _get_docs_repo():
     """Download zip archive of ploomber/doc and extract it"""
     url = "https://api.github.com/repos/ploomber/doc/zipball/main"
     headers = {
@@ -208,49 +209,63 @@
         click.echo(MISSING_API_KEY_MSG)
 
     click.echo(f"$ cd {location}")
     click.echo("$ ploomber-cloud init")
     click.echo("$ ploomber-cloud deploy\n")
 
 
-def examples(name=None):
+def examples(name=None, clear_cache=False):
     """Download an example app from the ploomber/docs/examples repo"""
     # Check if metadata exists and is current
-    current = _validate_metadata()
-    if not current:
+    metadata_updated = _validate_metadata() if not clear_cache else False
+    if not metadata_updated:
         # Download GH doc repo
         subpath = _get_docs_repo()
         # Parse into metadata file
         examples_data = _parse_directory_tree(
             f"{CLONED_REPO_PATH}/{subpath}/examples", 0
         )
         _save_metadata(examples_data)
+        click.echo("Downloaded latest examples...\n")
 
     examples = _load_metadata()["examples"]
     _save_metadata(examples)
 
     path_to_example, example_title = None, None
 
     # Prompt user for example choice
     if name:
         # Validate
-        try:
-            framework, name = name.split("/", 1)
-            if framework == "docker" and name not in examples[framework]:
-                raise PloomberCloudRuntimeException(
-                    f"{framework}/{name} does not exist. "
-                    f"Please enter a valid project."
-                )
-
-            path_to_example = examples[framework][name]["path"]
-            example_title = examples[framework][name]["title"]
-        except KeyError as e:
-            raise PloomberCloudRuntimeException(INVALID_CHOICE_ERROR_MSG) from e
-        except ValueError as e:
-            raise PloomberCloudRuntimeException(INVALID_CHOICE_ERROR_MSG) from e
+        if "/" not in name:
+            error_msg = INVALID_CHOICE_ERROR_MSG.format(
+                reason="Either the framework or the project is missing.\n"
+            )
+            raise PloomberCloudRuntimeException(error_msg)
+
+        framework, name = name.split("/", 1)
+
+        if framework == "docker" and name not in examples[framework]:
+            raise PloomberCloudRuntimeException(
+                f"{framework}/{name} does not exist. " f"Please enter a valid project."
+            )
+
+        if framework not in examples:
+            error_msg = INVALID_CHOICE_ERROR_MSG.format(
+                reason=f"Couldn't find framework: {framework}.\n"
+            )
+            raise PloomberCloudRuntimeException(error_msg)
+
+        if name not in examples[framework]:
+            error_msg = INVALID_CHOICE_ERROR_MSG.format(
+                reason=f"Couldn't find project: {name}.\n"
+            )
+            raise PloomberCloudRuntimeException(error_msg)
+
+        path_to_example = examples[framework][name]["path"]
+        example_title = examples[framework][name]["title"]
 
     if not path_to_example or not example_title:
         path_to_example, example_title = _prompt_user_for_example_choice(examples)
 
     # Prompt user for location
     location = _prompt_user_for_location()
```

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/exceptions.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/functions.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/functions.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/github.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/github.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/init.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/init.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/io.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/io.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/labels.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/labels.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/resources.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/resources.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/templates.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/templates.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/util.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/util.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud/zip_.py` & `ploomber-cloud-0.2.7/src/ploomber_cloud/zip_.py`

 * *Files identical despite different names*

### Comparing `ploomber-cloud-0.2.6/src/ploomber_cloud.egg-info/SOURCES.txt` & `ploomber-cloud-0.2.7/src/ploomber_cloud.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/ploomber_cloud/__init__.py
 src/ploomber_cloud/_telemetry.py
+src/ploomber_cloud/abc.py
 src/ploomber_cloud/api.py
 src/ploomber_cloud/api_key.py
 src/ploomber_cloud/cli.py
 src/ploomber_cloud/client.py
 src/ploomber_cloud/config.py
 src/ploomber_cloud/constants.py
 src/ploomber_cloud/delete.py
```

