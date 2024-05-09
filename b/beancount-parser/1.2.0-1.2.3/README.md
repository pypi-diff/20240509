# Comparing `tmp/beancount_parser-1.2.0.tar.gz` & `tmp/beancount_parser-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beancount_parser-1.2.0.tar", max compression
+gzip compressed data, was "beancount_parser-1.2.3.tar", max compression
```

## Comparing `beancount_parser-1.2.0.tar` & `beancount_parser-1.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1076 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/LICENSE
--rw-r--r--   0        0        0     2434 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/__init__.py
--rw-r--r--   0        0        0     1397 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/data_types.py
--rw-r--r--   0        0        0      335 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/grammar/account.lark
--rw-r--r--   0        0        0     3467 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/grammar/beancount.lark
--rw-r--r--   0        0        0       26 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/grammar/boolean.lark
--rw-r--r--   0        0        0       22 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/grammar/comment.lark
--rw-r--r--   0        0        0      162 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/grammar/currency.lark
--rw-r--r--   0        0        0      404 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/grammar/date.lark
--rw-r--r--   0        0        0      397 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/grammar/escaped_string.lark
--rw-r--r--   0        0        0      208 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/grammar/flag.lark
--rw-r--r--   0        0        0      223 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/grammar/link.lark
--rw-r--r--   0        0        0      162 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/grammar/numbers.lark
--rw-r--r--   0        0        0       29 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/grammar/section_header.lark
--rw-r--r--   0        0        0      289 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/grammar/tag.lark
--rw-r--r--   0        0        0     2858 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/helpers.py
--rw-r--r--   0        0        0     2337 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/beancount_parser/parser.py
--rw-r--r--   0        0        0      529 2024-05-06 00:41:08.592103 beancount_parser-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3168 1970-01-01 00:00:00.000000 beancount_parser-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/LICENSE
+-rw-r--r--   0        0        0     2434 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/__init__.py
+-rw-r--r--   0        0        0     1397 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/data_types.py
+-rw-r--r--   0        0        0      335 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/grammar/account.lark
+-rw-r--r--   0        0        0     3467 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/grammar/beancount.lark
+-rw-r--r--   0        0        0       26 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/grammar/boolean.lark
+-rw-r--r--   0        0        0       22 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/grammar/comment.lark
+-rw-r--r--   0        0        0      162 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/grammar/currency.lark
+-rw-r--r--   0        0        0      404 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/grammar/date.lark
+-rw-r--r--   0        0        0      397 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/grammar/escaped_string.lark
+-rw-r--r--   0        0        0      208 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/grammar/flag.lark
+-rw-r--r--   0        0        0      223 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/grammar/link.lark
+-rw-r--r--   0        0        0      162 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/grammar/numbers.lark
+-rw-r--r--   0        0        0       29 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/grammar/section_header.lark
+-rw-r--r--   0        0        0      289 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/grammar/tag.lark
+-rw-r--r--   0        0        0     2858 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/helpers.py
+-rw-r--r--   0        0        0     2865 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/beancount_parser/parser.py
+-rw-r--r--   0        0        0      529 2024-05-09 18:38:12.495792 beancount_parser-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3168 1970-01-01 00:00:00.000000 beancount_parser-1.2.3/PKG-INFO
```

### Comparing `beancount_parser-1.2.0/LICENSE` & `beancount_parser-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `beancount_parser-1.2.0/README.md` & `beancount_parser-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `beancount_parser-1.2.0/beancount_parser/data_types.py` & `beancount_parser-1.2.3/beancount_parser/data_types.py`

 * *Files identical despite different names*

### Comparing `beancount_parser-1.2.0/beancount_parser/grammar/beancount.lark` & `beancount_parser-1.2.3/beancount_parser/grammar/beancount.lark`

 * *Files identical despite different names*

### Comparing `beancount_parser-1.2.0/beancount_parser/helpers.py` & `beancount_parser-1.2.3/beancount_parser/helpers.py`

 * *Files identical despite different names*

### Comparing `beancount_parser-1.2.0/beancount_parser/parser.py` & `beancount_parser-1.2.3/beancount_parser/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import glob
 import json
+import logging
 import pathlib
 import typing
 
 from lark import Lark
 from lark import Tree
 
 GRAMMAR_FOLDER = pathlib.Path(__file__).parent / "grammar"
@@ -12,15 +13,15 @@
 
 def make_parser(**options: typing.Any) -> Lark:
     default_options = dict(propagate_positions=True, parser="lalr")
     with open(BEANCOUNT_GRAMMAR_FILE, "rt") as fo:
         return Lark(grammar=fo, **(default_options | options))
 
 
-def extract_includes(tree: Tree):
+def extract_includes(tree: Tree) -> typing.Generator[tuple[str, int], None, None]:
     """Extract include statements from the root tree"""
     if tree.data != "start":
         raise ValueError("Expected start")
     for child in tree.children:
         if child is None:
             continue
         if child.data != "statement":
@@ -29,36 +30,48 @@
         if not isinstance(first_child, Tree):
             continue
         if first_child.data != "simple_directive":
             continue
         include = first_child.children[0]
         if include.data != "include":
             continue
-        yield json.loads(include.children[0].value)
+        yield json.loads(include.children[0].value), first_child.meta.line
 
 
 def traverse(
     parser: Lark, bean_file: pathlib.Path, root_dir: pathlib.Path | None = None
 ) -> typing.Generator[tuple[pathlib.Path, Tree], None, None]:
     """Traverse a given bean file and follow all its includes, yield (path, parsed_tree) tuples"""
+    logger = logging.getLogger(__name__)
     visited_bean_files: set[pathlib.Path] = set()
 
     if root_dir is None:
         root_dir = bean_file.parent.absolute()
     pending_files = [bean_file.absolute()]
 
     while pending_files:
         current_file = pending_files.pop(0)
         visited_bean_files.add(current_file)
         tree = parser.parse(current_file.read_text())
         yield current_file, tree
         includes = extract_includes(tree)
-        for include in includes:
+        for include, lineno in includes:
+            logger.info(
+                "Process include at %s:%s with path value %s",
+                current_file,
+                lineno,
+                include,
+            )
             target_file = current_file.parent / include
             for matched_file in glob.glob(str(target_file)):
                 matched_file = pathlib.Path(matched_file).resolve().absolute()
                 if root_dir not in matched_file.parents:
+                    logger.warning(
+                        "Matched file %s is not a sub-path of root %s, ignored",
+                        matched_file,
+                        root_dir,
+                    )
                     # ensure include cannot go above the root folder, to avoid any potential security risk
                     continue
                 if matched_file in visited_bean_files:
                     continue
                 pending_files.append(matched_file)
```

### Comparing `beancount_parser-1.2.0/pyproject.toml` & `beancount_parser-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beancount-parser"
-version = "1.2.0"
+version = "1.2.3"
 description = "Standalone Lark based Beancount syntax parser (not relying on Beancount library), MIT license"
 authors = ["Fang-Pen Lin <fangpen@launchplatform.com>"]
 license = "MIT"
 repository = "https://github.com/LaunchPlatform/beancount-parser"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `beancount_parser-1.2.0/PKG-INFO` & `beancount_parser-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-parser
-Version: 1.2.0
+Version: 1.2.3
 Summary: Standalone Lark based Beancount syntax parser (not relying on Beancount library), MIT license
 Home-page: https://github.com/LaunchPlatform/beancount-parser
 License: MIT
 Author: Fang-Pen Lin
 Author-email: fangpen@launchplatform.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: beancount-parser Version: 1.2.0 Summary: Standalone
+Metadata-Version: 2.1 Name: beancount-parser Version: 1.2.3 Summary: Standalone
 Lark based Beancount syntax parser (not relying on Beancount library), MIT
 license Home-page: https://github.com/LaunchPlatform/beancount-parser License:
 MIT Author: Fang-Pen Lin Author-email: fangpen@launchplatform.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: lark
```

