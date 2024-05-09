# Comparing `tmp/mkdocs_drawio-1.6.1.tar.gz` & `tmp/mkdocs_drawio-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_drawio-1.6.1.tar", max compression
+gzip compressed data, was "mkdocs_drawio-1.6.2.tar", max compression
```

## Comparing `mkdocs_drawio-1.6.1.tar` & `mkdocs_drawio-1.6.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1052 2024-05-07 23:30:18.113949 mkdocs_drawio-1.6.1/LICENSE
--rw-r--r--   0        0        0     2313 2024-05-07 23:30:18.113949 mkdocs_drawio-1.6.1/README.md
--rw-r--r--   0        0        0     3789 2024-05-07 23:30:18.117949 mkdocs_drawio-1.6.1/mkdocs_drawio/plugin.py
--rw-r--r--   0        0        0      840 2024-05-07 23:30:18.117949 mkdocs_drawio-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 mkdocs_drawio-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1052 2024-05-09 13:12:13.673411 mkdocs_drawio-1.6.2/LICENSE
+-rw-r--r--   0        0        0     2313 2024-05-09 13:12:13.673411 mkdocs_drawio-1.6.2/README.md
+-rw-r--r--   0        0        0     3789 2024-05-09 13:12:13.673411 mkdocs_drawio-1.6.2/mkdocs_drawio/plugin.py
+-rw-r--r--   0        0        0      832 2024-05-09 13:12:13.673411 mkdocs_drawio-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3278 1970-01-01 00:00:00.000000 mkdocs_drawio-1.6.2/PKG-INFO
```

### Comparing `mkdocs_drawio-1.6.1/LICENSE` & `mkdocs_drawio-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_drawio-1.6.1/README.md` & `mkdocs_drawio-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_drawio-1.6.1/mkdocs_drawio/plugin.py` & `mkdocs_drawio-1.6.2/mkdocs_drawio/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_drawio-1.6.1/pyproject.toml` & `mkdocs_drawio-1.6.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-drawio"
-version = "1.6.1"
+version = "1.6.2"
 description = "MkDocs plugin for embedding Drawio files"
 authors = [
     "Sergey Lukin <onixpro@gmail.com>",
     "Jan Larwig <jan@larwig.com>"
 ]
 license = "MIT"
 readme = "README.md"
@@ -15,22 +15,22 @@
 ]
 packages = [
     { include = "mkdocs_drawio/plugin.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7.0"
-requests = "^2.31.0"
-Jinja2 = "^3.1.0"
-beautifulsoup4 = "^4.12.0"
-lxml = "^5.0.0"
-mkdocs = "^1.5.0"
+requests = ">=2.0"
+Jinja2 = ">=3.0"
+beautifulsoup4 = ">=4.0"
+lxml = ">=4.0"
+mkdocs = ">=1.3"
 
 [tool.poetry.dev-dependencies]
-black = "^24.4.0"
+black = ">=24.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."mkdocs.plugins"]
 drawio = 'mkdocs_drawio.plugin:DrawioPlugin'
```

### Comparing `mkdocs_drawio-1.6.1/PKG-INFO` & `mkdocs_drawio-1.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-drawio
-Version: 1.6.1
+Version: 1.6.2
 Summary: MkDocs plugin for embedding Drawio files
 Home-page: https://github.com/tuunit/mkdocs-drawio/
 License: MIT
 Keywords: mkdocs,plugin,markdown,drawio
 Author: Sergey Lukin
 Author-email: onixpro@gmail.com
 Requires-Python: >=3.7.0,<4.0.0
@@ -12,19 +12,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: Jinja2 (>=3.1.0,<4.0.0)
-Requires-Dist: beautifulsoup4 (>=4.12.0,<5.0.0)
-Requires-Dist: lxml (>=5.0.0,<6.0.0)
-Requires-Dist: mkdocs (>=1.5.0,<2.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: Jinja2 (>=3.0)
+Requires-Dist: beautifulsoup4 (>=4.0)
+Requires-Dist: lxml (>=4.0)
+Requires-Dist: mkdocs (>=1.3)
+Requires-Dist: requests (>=2.0)
 Project-URL: Repository, https://github.com/tuunit/mkdocs-drawio/
 Description-Content-Type: text/markdown
 
 # MkDocs Plugin for embedding Drawio files
 [![Publish Badge](https://github.com/tuunit/mkdocs-drawio/workflows/Publish/badge.svg)](https://github.com/tuunit/mkdocs-drawio/actions)
 [![PyPI](https://img.shields.io/pypi/v/mkdocs-drawio)](https://pypi.org/project/mkdocs-drawio/)
```

