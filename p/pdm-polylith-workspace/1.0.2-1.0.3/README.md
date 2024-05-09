# Comparing `tmp/pdm_polylith_workspace-1.0.2.tar.gz` & `tmp/pdm_polylith_workspace-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_polylith_workspace-1.0.2.tar", max compression
+gzip compressed data, was "pdm_polylith_workspace-1.0.3.tar", max compression
```

## Comparing `pdm_polylith_workspace-1.0.2.tar` & `pdm_polylith_workspace-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1008 2024-02-09 08:50:51.458954 pdm_polylith_workspace-1.0.2/README.md
--rw-r--r--   0        0        0      568 2024-05-01 07:13:05.626149 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/configuration/__init__.py
--rw-r--r--   0        0        0     2194 2024-05-01 07:13:05.627768 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/configuration/core.py
--rw-r--r--   0        0        0      255 2024-05-01 07:13:05.630437 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/parsing/__init__.py
--rw-r--r--   0        0        0      751 2024-02-09 08:50:51.444767 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/parsing/core.py
--rw-r--r--   0        0        0     2156 2024-02-09 08:50:51.445237 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/parsing/rewrite.py
--rw-r--r--   0        0        0        0 2024-02-09 08:50:51.445339 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/__init__.py
--rw-r--r--   0        0        0     1154 2024-05-01 07:13:05.633175 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/core.py
--rw-r--r--   0        0        0        0 2024-02-09 08:50:51.445849 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/hooks/__init__.py
--rw-r--r--   0        0        0      643 2024-05-01 07:13:05.633555 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py
--rw-r--r--   0        0        0     1022 2024-05-01 07:13:05.634363 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py
--rw-r--r--   0        0        0        0 2024-02-09 08:50:51.428428 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm_workspace_hooks/__init__.py
--rw-r--r--   0        0        0      465 2024-05-01 07:13:05.630250 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm_workspace_hooks/core.py
--rw-r--r--   0        0        0      545 2024-05-01 07:13:05.631513 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/repo/__init__.py
--rw-r--r--   0        0        0      862 2024-05-01 07:13:05.632494 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-09 08:50:51.451835 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/repo/repo.py
--rw-r--r--   0        0        0      467 2024-05-01 07:13:05.628052 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/toml/__init__.py
--rw-r--r--   0        0        0     3254 2024-05-01 07:13:05.629877 pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/toml/core.py
--rw-r--r--   0        0        0      641 2024-05-01 07:13:05.625646 pdm_polylith_workspace-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1694 1970-01-01 00:00:00.000000 pdm_polylith_workspace-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1008 2024-02-09 08:50:51.458954 pdm_polylith_workspace-1.0.3/README.md
+-rw-r--r--   0        0        0      568 2024-05-09 09:58:56.791975 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/configuration/__init__.py
+-rw-r--r--   0        0        0     2194 2024-05-09 09:58:56.793096 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/configuration/core.py
+-rw-r--r--   0        0        0      255 2024-05-09 09:58:56.795970 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/parsing/__init__.py
+-rw-r--r--   0        0        0      751 2024-02-09 08:50:51.444767 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/parsing/core.py
+-rw-r--r--   0        0        0     2156 2024-02-09 08:50:51.445237 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/parsing/rewrite.py
+-rw-r--r--   0        0        0        0 2024-02-09 08:50:51.445339 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/pdm/__init__.py
+-rw-r--r--   0        0        0     1154 2024-05-09 09:58:56.798573 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/pdm/core.py
+-rw-r--r--   0        0        0        0 2024-02-09 08:50:51.445849 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/pdm/hooks/__init__.py
+-rw-r--r--   0        0        0      723 2024-05-09 09:58:56.799333 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py
+-rw-r--r--   0        0        0     1022 2024-05-09 09:58:56.800419 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py
+-rw-r--r--   0        0        0        0 2024-02-09 08:50:51.428428 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/pdm_workspace_hooks/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-09 09:58:56.795574 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/pdm_workspace_hooks/core.py
+-rw-r--r--   0        0        0      545 2024-05-09 09:58:56.796979 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      862 2024-05-09 09:58:56.797916 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-09 08:50:51.451835 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/repo/repo.py
+-rw-r--r--   0        0        0      467 2024-05-09 09:58:56.793569 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     3254 2024-05-09 09:58:56.795219 pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/toml/core.py
+-rw-r--r--   0        0        0      641 2024-05-09 09:58:56.791448 pdm_polylith_workspace-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1694 1970-01-01 00:00:00.000000 pdm_polylith_workspace-1.0.3/PKG-INFO
```

### Comparing `pdm_polylith_workspace-1.0.2/README.md` & `pdm_polylith_workspace-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/configuration/__init__.py` & `pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/configuration/core.py` & `pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/configuration/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/parsing/core.py` & `pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/parsing/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/parsing/rewrite.py` & `pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/parsing/rewrite.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/core.py` & `pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py` & `pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/pdm/hooks/bricks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 from pdm_polylith_workspace.polylith import toml
 from pdm_polylith_workspace.polylith.pdm import core
 
-def build_initialize(config_data: dict, build_dir: Path) -> None:
+def build_initialize(root: Path, config_data: dict, build_dir: Path) -> None:
     bricks = toml.get_project_packages_from_polylith_section(config_data)
+    found_bricks = {k: v for (k, v) in bricks.items() if Path(root / k).exists()}
+    if not bricks or not found_bricks:
+        return
     top_ns = toml.get_custom_top_namespace_from_polylith_section(config_data)
     work_dir = core.get_work_dir(config_data)
-    if not bricks:
-        print('No bricks found.')
-        return
     if not top_ns:
         core.copy_bricks_as_is(bricks, build_dir)
     else:
         core.copy_and_rewrite_bricks(bricks, top_ns, work_dir, build_dir)
         core.cleanup(work_dir)
```

### Comparing `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py` & `pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/pdm/hooks/workspace.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/repo/__init__.py` & `pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/repo/get.py` & `pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/repo/repo.py` & `pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.2/pdm_polylith_workspace/polylith/toml/core.py` & `pdm_polylith_workspace-1.0.3/pdm_polylith_workspace/polylith/toml/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_workspace-1.0.2/pyproject.toml` & `pdm_polylith_workspace-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdm-polylith-workspace"
-version = "1.0.2"
+version = "1.0.3"
 description = "a PDM build hook for a Polylith workspace"
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 authors = ["David Vujic"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `pdm_polylith_workspace-1.0.2/PKG-INFO` & `pdm_polylith_workspace-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-polylith-workspace
-Version: 1.0.2
+Version: 1.0.3
 Summary: a PDM build hook for a Polylith workspace
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 License: MIT
 Author: David Vujic
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

