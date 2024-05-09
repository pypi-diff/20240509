# Comparing `tmp/pdm_polylith_bricks-1.0.2.tar.gz` & `tmp/pdm_polylith_bricks-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_polylith_bricks-1.0.2.tar", max compression
+gzip compressed data, was "pdm_polylith_bricks-1.0.3.tar", max compression
```

## Comparing `pdm_polylith_bricks-1.0.2.tar` & `pdm_polylith_bricks-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     2825 2024-02-09 08:50:51.458099 pdm_polylith_bricks-1.0.2/README.md
--rw-r--r--   0        0        0      565 2024-05-01 07:12:19.056201 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/configuration/__init__.py
--rw-r--r--   0        0        0     2191 2024-05-01 07:12:19.057713 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/configuration/core.py
--rw-r--r--   0        0        0      249 2024-05-01 07:12:19.060190 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/parsing/__init__.py
--rw-r--r--   0        0        0      751 2024-02-09 08:50:51.444767 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/parsing/core.py
--rw-r--r--   0        0        0     2156 2024-02-09 08:50:51.445237 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/parsing/rewrite.py
--rw-r--r--   0        0        0        0 2024-02-09 08:50:51.445339 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/pdm/__init__.py
--rw-r--r--   0        0        0     1151 2024-05-01 07:12:19.062948 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/pdm/core.py
--rw-r--r--   0        0        0        0 2024-02-09 08:50:51.445849 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/pdm/hooks/__init__.py
--rw-r--r--   0        0        0      637 2024-05-01 07:12:19.063321 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/pdm/hooks/bricks.py
--rw-r--r--   0        0        0     1019 2024-05-01 07:12:19.064682 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/pdm/hooks/workspace.py
--rw-r--r--   0        0        0        0 2024-02-09 08:50:51.427795 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/pdm_project_hooks/__init__.py
--rw-r--r--   0        0        0      259 2024-05-01 07:12:19.060016 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/pdm_project_hooks/core.py
--rw-r--r--   0        0        0      539 2024-05-01 07:12:19.061256 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/repo/__init__.py
--rw-r--r--   0        0        0      859 2024-05-01 07:12:19.062263 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-09 08:50:51.451835 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/repo/repo.py
--rw-r--r--   0        0        0      464 2024-05-01 07:12:19.057941 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/toml/__init__.py
--rw-r--r--   0        0        0     3251 2024-05-01 07:12:19.059723 pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/toml/core.py
--rw-r--r--   0        0        0      614 2024-05-01 07:12:19.055711 pdm_polylith_bricks-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 pdm_polylith_bricks-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2825 2024-02-09 08:50:51.458099 pdm_polylith_bricks-1.0.3/README.md
+-rw-r--r--   0        0        0      565 2024-05-09 09:59:56.767008 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/configuration/__init__.py
+-rw-r--r--   0        0        0     2191 2024-05-09 09:59:56.768132 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/configuration/core.py
+-rw-r--r--   0        0        0      249 2024-05-09 09:59:56.770529 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/parsing/__init__.py
+-rw-r--r--   0        0        0      751 2024-02-09 08:50:51.444767 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/parsing/core.py
+-rw-r--r--   0        0        0     2156 2024-02-09 08:50:51.445237 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/parsing/rewrite.py
+-rw-r--r--   0        0        0        0 2024-02-09 08:50:51.445339 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/pdm/__init__.py
+-rw-r--r--   0        0        0     1151 2024-05-09 09:59:56.773151 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/pdm/core.py
+-rw-r--r--   0        0        0        0 2024-02-09 08:50:51.445849 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/pdm/hooks/__init__.py
+-rw-r--r--   0        0        0      717 2024-05-09 09:59:56.773599 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/pdm/hooks/bricks.py
+-rw-r--r--   0        0        0     1019 2024-05-09 09:59:56.774361 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/pdm/hooks/workspace.py
+-rw-r--r--   0        0        0        0 2024-02-09 08:50:51.427795 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/pdm_project_hooks/__init__.py
+-rw-r--r--   0        0        0      280 2024-05-09 09:59:56.770341 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/pdm_project_hooks/core.py
+-rw-r--r--   0        0        0      539 2024-05-09 09:59:56.771529 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      859 2024-05-09 09:59:56.772496 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-09 08:50:51.451835 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/repo/repo.py
+-rw-r--r--   0        0        0      464 2024-05-09 09:59:56.768368 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     3251 2024-05-09 09:59:56.770022 pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/toml/core.py
+-rw-r--r--   0        0        0      614 2024-05-09 09:59:56.766522 pdm_polylith_bricks-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 pdm_polylith_bricks-1.0.3/PKG-INFO
```

### Comparing `pdm_polylith_bricks-1.0.2/README.md` & `pdm_polylith_bricks-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/configuration/__init__.py` & `pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/configuration/core.py` & `pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/configuration/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/parsing/core.py` & `pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/parsing/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/parsing/rewrite.py` & `pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/parsing/rewrite.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/pdm/core.py` & `pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/pdm/hooks/bricks.py` & `pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/pdm/hooks/bricks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 from pdm_polylith_bricks.polylith import toml
 from pdm_polylith_bricks.polylith.pdm import core
 
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

### Comparing `pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/pdm/hooks/workspace.py` & `pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/pdm/hooks/workspace.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/repo/__init__.py` & `pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/repo/get.py` & `pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/repo/repo.py` & `pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.2/pdm_polylith_bricks/polylith/toml/core.py` & `pdm_polylith_bricks-1.0.3/pdm_polylith_bricks/polylith/toml/core.py`

 * *Files identical despite different names*

### Comparing `pdm_polylith_bricks-1.0.2/pyproject.toml` & `pdm_polylith_bricks-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdm-polylith-bricks"
-version = "1.0.2"
+version = "1.0.3"
 description = "a PDM build hook for Polylith"
 authors = ["David Vujic"]
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 license = "MIT"
 readme = "README.md"
```

### Comparing `pdm_polylith_bricks-1.0.2/PKG-INFO` & `pdm_polylith_bricks-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-polylith-bricks
-Version: 1.0.2
+Version: 1.0.3
 Summary: a PDM build hook for Polylith
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 License: MIT
 Author: David Vujic
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

