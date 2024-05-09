# Comparing `tmp/hatch_polylith_bricks-1.2.2.tar.gz` & `tmp/hatch_polylith_bricks-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatch_polylith_bricks-1.2.2.tar", max compression
+gzip compressed data, was "hatch_polylith_bricks-1.2.3.tar", max compression
```

## Comparing `hatch_polylith_bricks-1.2.2.tar` & `hatch_polylith_bricks-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3140 2024-02-09 08:50:51.457205 hatch_polylith_bricks-1.2.2/README.md
--rw-r--r--   0        0        0       74 2024-05-01 07:11:19.859275 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch/__init__.py
--rw-r--r--   0        0        0      419 2024-05-01 07:11:19.859554 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch/core.py
--rw-r--r--   0        0        0        0 2024-01-22 14:07:16.218717 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch/hooks/__init__.py
--rw-r--r--   0        0        0     1602 2024-05-01 07:11:19.860335 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py
--rw-r--r--   0        0        0        0 2024-01-22 14:07:16.215883 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch_hooks/__init__.py
--rw-r--r--   0        0        0      192 2024-05-01 07:11:19.859086 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch_hooks/hooks.py
--rw-r--r--   0        0        0      253 2024-05-01 07:11:19.860532 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/parsing/__init__.py
--rw-r--r--   0        0        0      751 2024-02-09 08:50:51.444767 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/parsing/core.py
--rw-r--r--   0        0        0     2156 2024-02-09 08:50:51.445237 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/parsing/rewrite.py
--rw-r--r--   0        0        0      543 2024-05-01 07:11:19.861539 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/repo/__init__.py
--rw-r--r--   0        0        0      861 2024-05-01 07:11:19.862462 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/repo/get.py
--rw-r--r--   0        0        0     1964 2024-02-09 08:50:51.451835 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/repo/repo.py
--rw-r--r--   0        0        0      466 2024-05-01 07:11:19.857016 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/toml/__init__.py
--rw-r--r--   0        0        0     3253 2024-05-01 07:11:19.858850 hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/toml/core.py
--rw-r--r--   0        0        0      676 2024-05-01 07:11:19.856553 hatch_polylith_bricks-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 hatch_polylith_bricks-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3140 2024-02-09 08:50:51.457205 hatch_polylith_bricks-1.2.3/README.md
+-rw-r--r--   0        0        0       74 2024-05-09 10:00:34.236346 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/hatch/__init__.py
+-rw-r--r--   0        0        0      419 2024-05-09 10:00:34.236616 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/hatch/core.py
+-rw-r--r--   0        0        0        0 2024-01-22 14:07:16.218717 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/hatch/hooks/__init__.py
+-rw-r--r--   0        0        0     1647 2024-05-09 10:00:34.237450 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py
+-rw-r--r--   0        0        0        0 2024-01-22 14:07:16.215883 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/hatch_hooks/__init__.py
+-rw-r--r--   0        0        0      192 2024-05-09 10:00:34.236159 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/hatch_hooks/hooks.py
+-rw-r--r--   0        0        0      253 2024-05-09 10:00:34.237644 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/parsing/__init__.py
+-rw-r--r--   0        0        0      751 2024-02-09 08:50:51.444767 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/parsing/core.py
+-rw-r--r--   0        0        0     2156 2024-02-09 08:50:51.445237 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/parsing/rewrite.py
+-rw-r--r--   0        0        0      543 2024-05-09 10:00:34.238638 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/repo/__init__.py
+-rw-r--r--   0        0        0      861 2024-05-09 10:00:34.239558 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/repo/get.py
+-rw-r--r--   0        0        0     1964 2024-02-09 08:50:51.451835 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/repo/repo.py
+-rw-r--r--   0        0        0      466 2024-05-09 10:00:34.234119 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/toml/__init__.py
+-rw-r--r--   0        0        0     3253 2024-05-09 10:00:34.235919 hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/toml/core.py
+-rw-r--r--   0        0        0      676 2024-05-09 10:00:34.233653 hatch_polylith_bricks-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 hatch_polylith_bricks-1.2.3/PKG-INFO
```

### Comparing `hatch_polylith_bricks-1.2.2/README.md` & `hatch_polylith_bricks-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py` & `hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/hatch/hooks/bricks.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from hatch_polylith_bricks.polylith import parsing, repo, toml
 from hatch_polylith_bricks.polylith.hatch import core
 
 class PolylithBricksHook(BuildHookInterface):
     PLUGIN_NAME = 'polylith-bricks'
 
     def initialize(self, _version: str, build_data: Dict[str, Any]) -> None:
-        pyproject = Path(f'{self.root}/{repo.default_toml}')
-        print(f'Using {pyproject.as_posix()}.')
+        root = self.root
+        pyproject = Path(f'{root}/{repo.default_toml}')
         data = toml.read_toml_document(pyproject)
         bricks = toml.get_project_packages_from_polylith_section(data)
+        found_bricks = {k: v for (k, v) in bricks.items() if Path(f'{root}/{k}').exists()}
+        if not bricks or not found_bricks:
+            return
         top_ns = core.get_top_namespace(data, self.config)
         work_dir = core.get_work_dir(self.config)
-        if not bricks:
-            print('No bricks found.')
-            return
         if not top_ns:
             build_data['force_include'] = bricks
             return
         ns = parsing.parse_brick_namespace_from_path(bricks)
         for (source, brick) in bricks.items():
             path = parsing.copy_brick(source, brick, work_dir)
             rewritten_bricks = parsing.rewrite_modules(path, ns, top_ns)
```

### Comparing `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/parsing/core.py` & `hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/parsing/core.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/parsing/rewrite.py` & `hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/parsing/rewrite.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/repo/__init__.py` & `hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/repo/get.py` & `hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/repo/get.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/repo/repo.py` & `hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/repo/repo.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.2/hatch_polylith_bricks/polylith/toml/core.py` & `hatch_polylith_bricks-1.2.3/hatch_polylith_bricks/polylith/toml/core.py`

 * *Files identical despite different names*

### Comparing `hatch_polylith_bricks-1.2.2/pyproject.toml` & `hatch_polylith_bricks-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hatch-polylith-bricks"
-version = "1.2.2"
+version = "1.2.3"
 description = "Hatch build hook plugin for Polylith"
 authors = ['David Vujic']
 homepage = "https://davidvujic.github.io/python-polylith-docs/"
 repository = "https://github.com/davidvujic/python-polylith"
 license = "MIT"
 readme = "README.md"
```

### Comparing `hatch_polylith_bricks-1.2.2/PKG-INFO` & `hatch_polylith_bricks-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-polylith-bricks
-Version: 1.2.2
+Version: 1.2.3
 Summary: Hatch build hook plugin for Polylith
 Home-page: https://davidvujic.github.io/python-polylith-docs/
 License: MIT
 Author: David Vujic
 Requires-Python: >=3.9,<4.0
 Classifier: Framework :: Hatch
 Classifier: License :: OSI Approved :: MIT License
```

