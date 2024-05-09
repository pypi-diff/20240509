# Comparing `tmp/debby-1.1.0.tar.gz` & `tmp/debby-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debby-1.1.0.tar", max compression
+gzip compressed data, was "debby-1.1.1.tar", max compression
```

## Comparing `debby-1.1.0.tar` & `debby-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    35149 2024-05-09 09:23:41.666567 debby-1.1.0/LICENSE
--rw-r--r--   0        0        0     4859 2024-05-09 09:23:41.666567 debby-1.1.0/README.md
--rw-r--r--   0        0        0      301 2024-05-09 09:23:41.666567 debby-1.1.0/debby/__init__.py
--rw-r--r--   0        0        0      739 2024-05-09 09:23:41.666567 debby-1.1.0/debby/__main__.py
--rw-r--r--   0        0        0     7792 2024-05-09 09:23:41.666567 debby-1.1.0/debby/args.py
--rw-r--r--   0        0        0     2263 2024-05-09 09:23:41.666567 debby-1.1.0/debby/control_file.py
--rw-r--r--   0        0        0      383 2024-05-09 09:23:41.666567 debby-1.1.0/debby/exceptions.py
--rw-r--r--   0        0        0     2449 2024-05-09 09:23:41.666567 debby-1.1.0/debby/files.py
--rw-r--r--   0        0        0      165 2024-05-09 09:23:41.666567 debby-1.1.0/debby/meta/__init__.py
--rw-r--r--   0        0        0     1210 2024-05-09 09:23:41.666567 debby-1.1.0/debby/meta/meta.py
--rw-r--r--   0        0        0     2543 2024-05-09 09:23:41.666567 debby-1.1.0/debby/meta/meta_loader.py
--rw-r--r--   0        0        0      702 2024-05-09 09:23:41.666567 debby-1.1.0/debby/meta/meta_loader_factory.py
--rw-r--r--   0        0        0      883 2024-05-09 09:23:41.666567 debby-1.1.0/debby/meta/poetry_meta_loader.py
--rw-r--r--   0        0        0     1992 2024-05-09 09:23:41.666567 debby-1.1.0/debby/meta/pyproject_meta_loader.py
--rw-r--r--   0        0        0      986 2024-05-09 09:23:41.666567 debby-1.1.0/debby/package.py
--rw-r--r--   0        0        0        1 2024-05-09 09:23:41.666567 debby-1.1.0/debby/py.typed
--rw-r--r--   0        0        0      784 2024-05-09 09:23:50.546504 debby-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5753 1970-01-01 00:00:00.000000 debby-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-09 10:47:46.572876 debby-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4859 2024-05-09 10:47:46.572876 debby-1.1.1/README.md
+-rw-r--r--   0        0        0      301 2024-05-09 10:47:46.572876 debby-1.1.1/debby/__init__.py
+-rw-r--r--   0        0        0      739 2024-05-09 10:47:46.572876 debby-1.1.1/debby/__main__.py
+-rw-r--r--   0        0        0     7798 2024-05-09 10:47:46.576876 debby-1.1.1/debby/args.py
+-rw-r--r--   0        0        0     2263 2024-05-09 10:47:46.576876 debby-1.1.1/debby/control_file.py
+-rw-r--r--   0        0        0      383 2024-05-09 10:47:46.576876 debby-1.1.1/debby/exceptions.py
+-rw-r--r--   0        0        0     2449 2024-05-09 10:47:46.576876 debby-1.1.1/debby/files.py
+-rw-r--r--   0        0        0      165 2024-05-09 10:47:46.576876 debby-1.1.1/debby/meta/__init__.py
+-rw-r--r--   0        0        0     1210 2024-05-09 10:47:46.576876 debby-1.1.1/debby/meta/meta.py
+-rw-r--r--   0        0        0     2543 2024-05-09 10:47:46.576876 debby-1.1.1/debby/meta/meta_loader.py
+-rw-r--r--   0        0        0      702 2024-05-09 10:47:46.576876 debby-1.1.1/debby/meta/meta_loader_factory.py
+-rw-r--r--   0        0        0      883 2024-05-09 10:47:46.576876 debby-1.1.1/debby/meta/poetry_meta_loader.py
+-rw-r--r--   0        0        0     1992 2024-05-09 10:47:46.576876 debby-1.1.1/debby/meta/pyproject_meta_loader.py
+-rw-r--r--   0        0        0      986 2024-05-09 10:47:46.576876 debby-1.1.1/debby/package.py
+-rw-r--r--   0        0        0        1 2024-05-09 10:47:46.576876 debby-1.1.1/debby/py.typed
+-rw-r--r--   0        0        0      784 2024-05-09 10:47:54.256880 debby-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5753 1970-01-01 00:00:00.000000 debby-1.1.1/PKG-INFO
```

### Comparing `debby-1.1.0/LICENSE` & `debby-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `debby-1.1.0/README.md` & `debby-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `debby-1.1.0/debby/__main__.py` & `debby-1.1.1/debby/__main__.py`

 * *Files identical despite different names*

### Comparing `debby-1.1.0/debby/args.py` & `debby-1.1.1/debby/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,17 @@
             "--template",
             help="Path to a control file template to use instead of generating one from scratch. This file may contain placeholders such as {meta.name} and {meta.version}. See the documentation for more information. https://abrahammurciano.github.io/debby",
             type=Path,
         )
         parser.add_argument(
             "-o",
             "--out-dir",
-            help="Path to the output directory. Defaults to debian/build.",
+            help="Path to the output directory. Defaults to the current working directory.",
             type=Path,
-            default=Path("debian/build"),
+            default=Path("."),
         )
         parser.add_argument(
             "--no-size",
             help="Do not include the total size of the package in the control file.",
             action="store_true",
         )
         cls._add_meta_source_group(parser)
```

### Comparing `debby-1.1.0/debby/control_file.py` & `debby-1.1.1/debby/control_file.py`

 * *Files identical despite different names*

### Comparing `debby-1.1.0/debby/files.py` & `debby-1.1.1/debby/files.py`

 * *Files identical despite different names*

### Comparing `debby-1.1.0/debby/meta/meta.py` & `debby-1.1.1/debby/meta/meta.py`

 * *Files identical despite different names*

### Comparing `debby-1.1.0/debby/meta/meta_loader.py` & `debby-1.1.1/debby/meta/meta_loader.py`

 * *Files identical despite different names*

### Comparing `debby-1.1.0/debby/meta/meta_loader_factory.py` & `debby-1.1.1/debby/meta/meta_loader_factory.py`

 * *Files identical despite different names*

### Comparing `debby-1.1.0/debby/meta/poetry_meta_loader.py` & `debby-1.1.1/debby/meta/poetry_meta_loader.py`

 * *Files identical despite different names*

### Comparing `debby-1.1.0/debby/meta/pyproject_meta_loader.py` & `debby-1.1.1/debby/meta/pyproject_meta_loader.py`

 * *Files identical despite different names*

### Comparing `debby-1.1.0/debby/package.py` & `debby-1.1.1/debby/package.py`

 * *Files identical despite different names*

### Comparing `debby-1.1.0/pyproject.toml` & `debby-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "debby"
 # Version is overwritten at build time by CI based on git tag
-version = "1.1.0"
+version = "1.1.1"
 description = "Create .deb files easily using python package metadata"
 authors = ["Abraham Murciano <abrahammurciano@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/abrahammurciano/debby"
 documentation = "https://abrahammurciano.github.io/debby/debby"
 keywords = []
```

### Comparing `debby-1.1.0/PKG-INFO` & `debby-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debby
-Version: 1.1.0
+Version: 1.1.1
 Summary: Create .deb files easily using python package metadata
 Home-page: https://github.com/abrahammurciano/debby
 License: GPLv3
 Author: Abraham Murciano
 Author-email: abrahammurciano@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

