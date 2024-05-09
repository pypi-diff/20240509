# Comparing `tmp/proxyvars-0.9.1.tar.gz` & `tmp/proxyvars-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxyvars-0.9.1.tar", max compression
+gzip compressed data, was "proxyvars-0.9.2.tar", max compression
```

## Comparing `proxyvars-0.9.1.tar` & `proxyvars-0.9.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2023-12-22 05:54:59.803830 proxyvars-0.9.1/LICENSE
--rw-r--r--   0        0        0     3882 2023-12-22 05:54:59.803830 proxyvars-0.9.1/README.md
--rw-r--r--   0        0        0    25068 2023-12-22 05:54:59.803830 proxyvars-0.9.1/proxyvars/__init__.py
--rw-r--r--   0        0        0        0 2023-12-22 05:54:59.803830 proxyvars-0.9.1/proxyvars/py.typed
--rw-r--r--   0        0        0     5485 2023-12-22 05:54:59.803830 proxyvars-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4859 1970-01-01 00:00:00.000000 proxyvars-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-02-16 17:29:57.356500 proxyvars-0.9.2/LICENSE
+-rw-r--r--   0        0        0     4033 2024-02-16 17:29:57.356500 proxyvars-0.9.2/README.md
+-rw-r--r--   0        0        0    24981 2024-02-16 17:29:57.360499 proxyvars-0.9.2/proxyvars/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-16 17:29:57.360499 proxyvars-0.9.2/proxyvars/py.typed
+-rw-r--r--   0        0        0     5483 2024-02-16 17:29:57.360499 proxyvars-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 proxyvars-0.9.2/PKG-INFO
```

### Comparing `proxyvars-0.9.1/LICENSE` & `proxyvars-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proxyvars-0.9.1/README.md` & `proxyvars-0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 
-# proxyvars [![skeleton](https://img.shields.io/badge/61eeffb-skeleton?label=%F0%9F%92%80%20bswck/skeleton&labelColor=black&color=grey&link=https%3A//github.com/bswck/skeleton)](https://github.com/bswck/skeleton/tree/61eeffb)
+# proxyvars [![skeleton](https://img.shields.io/badge/7935235-skeleton?label=%F0%9F%92%80%20bswck/skeleton&labelColor=black&color=grey&link=https%3A//github.com/bswck/skeleton)](https://github.com/bswck/skeleton/tree/7935235)
 [![Package version](https://img.shields.io/pypi/v/proxyvars?label=PyPI)](https://pypi.org/project/proxyvars/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/proxyvars.svg?logo=python&label=Python)](https://pypi.org/project/proxyvars/)
 
 [![Tests](https://github.com/bswck/proxyvars/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/proxyvars/actions/workflows/test.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/proxyvars.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/proxyvars)
+[![Documentation Status](https://readthedocs.org/projects/proxyvars/badge/?version=latest)](https://proxyvars.readthedocs.io/en/latest/?badge=latest)
+[![License](https://img.shields.io/github/license/bswck/proxyvars.svg?label=License)](https://github.com/bswck/proxyvars/blob/HEAD/LICENSE)
+
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![License](https://img.shields.io/github/license/bswck/proxyvars.svg?label=License)](https://github.com/bswck/proxyvars/blob/HEAD/LICENSE)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 A simple and straight-forward Python module for creating context-dependent proxy objects.
 
 As for now, the documentation is mostly in the codebase (check relevant docstrings of `proxy()`, `const_proxy()`, `lookup_proxy()`, `proxy_field_accessor()`, `proxy_item_accessor()` and `proxy_attribute_accessor()` for more information).
 
 # Installation
@@ -29,17 +31,17 @@
 ```shell
 poetry add proxyvars
 ```
 
 ## For contributors
 
 <!--
-This section was generated from bswck/skeleton@61eeffb.
+This section was generated from bswck/skeleton@7935235.
 Instead of changing this particular file, you might want to alter the template:
-https://github.com/bswck/skeleton/tree/61eeffb/project/README.md.jinja
+https://github.com/bswck/skeleton/tree/7935235/project/README.md.jinja
 -->
 
 > [!Note]
 > If you use Windows, it is highly recommended to complete the installation in the way presented below through [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).
```

### Comparing `proxyvars-0.9.1/proxyvars/__init__.py` & `proxyvars-0.9.2/proxyvars/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,18 +170,16 @@
     proxy_metaclass
         The metaclass of the proxy object (default: `type`).
         This is useful if you want add custom descriptors to the result proxy object.
     namespace_overwrites
         A mapping of attribute names to values that the namespace
         of the Proxy class will be updated with before the class's creation.
     """
-    # pylint: disable=too-many-statements
     descriptor = partial(proxy_descriptor, get_state, overwrite_state)
 
-    # pylint: disable=too-few-public-methods
     class Proxy(
         proxy_base_cls,  # type: ignore[misc,valid-type]
         metaclass=lambda name, bases, namespace: proxy_metaclass(  # type: ignore[misc]
             name,
             bases,
             {**namespace, **(namespace_overwrites or {})},
         ),
```

### Comparing `proxyvars-0.9.1/pyproject.toml` & `proxyvars-0.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-# This file was generated from bswck/skeleton@61eeffb.
+# This file was generated from bswck/skeleton@7935235.
 # Instead of changing this particular file, you might want to alter the template:
-# https://github.com/bswck/skeleton/tree/61eeffb/project/pyproject.toml.jinja
+# https://github.com/bswck/skeleton/tree/7935235/project/pyproject.toml.jinja
 
 [tool.poetry]
 name = "proxyvars"
-version = "0.9.1"
+version = "0.9.2"
 description = "A simple and straight-forward Python module for creating context-dependent proxy objects."
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "proxyvars/" }]
 homepage = "https://github.com/bswck/proxyvars"
 
 [tool.poetry.urls]
 Documentation = "https://proxyvars.readthedocs.io/en/latest/"
 Issues = "https://github.com/bswck/proxyvars/issues"
 Distribution = "https://pypi.org/project/proxyvars/"
 Coverage = "https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/proxyvars"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<=3.12"
+python = ">=3.8,<3.13"
 
 [tool.poetry.group.dev.dependencies]
+pytest-lazy-fixture = "^0.6.3"
 
 [tool.poetry.group.dev-skeleton.dependencies]
-# This dependency group was generated from bswck/skeleton@61eeffb.
+# This dependency group was generated from bswck/skeleton@7935235.
 # Instead of changing this particular file, you might want to alter the template:
-# https://github.com/bswck/skeleton/tree/61eeffb/project/pyproject.toml.jinja
+# https://github.com/bswck/skeleton/tree/7935235/project/pyproject.toml.jinja
 mypy = "^1.7.0"
 ruff = "^0.1.2"
 towncrier = "^23.11.0"
 pytest = "^7.4.3"
 coverage = "^7.3.2"
 poethepoet = "^0.24.3"
 pre-commit = "^3.5.0"
 smokeshow = "^0.4.0"
-pytest-lazy-fixture = "^0.6.3"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 markdown-exec = ">=1.3.0"
 mkdocs-material = ">=8.2,<10.0.0"
 mkdocstrings = { version = ">=0.19.0", extras = ["python"] }
 
 [tool.poe.tasks]
 test = "pytest -v"
 lint = "ruff check ."
-skeleton = "scripts/skeleton.sh"
+skeleton = "scripts/7935235.sh"
 check = [
     { ref="test" },
     { ref="lint" },
 ]
 release.script = "scripts.release:main"
 
 [tool.poe.tasks.added]
```

### Comparing `proxyvars-0.9.1/PKG-INFO` & `proxyvars-0.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: proxyvars
-Version: 0.9.1
+Version: 0.9.2
 Summary: A simple and straight-forward Python module for creating context-dependent proxy objects.
 Home-page: https://github.com/bswck/proxyvars
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
-Requires-Python: >=3.8,<=3.12
+Requires-Python: >=3.8,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Coverage, https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/proxyvars
 Project-URL: Documentation, https://proxyvars.readthedocs.io/en/latest/
 Project-URL: Distribution, https://pypi.org/project/proxyvars/
 Project-URL: Issues, https://github.com/bswck/proxyvars/issues
 Description-Content-Type: text/markdown
 
 
-# proxyvars [![skeleton](https://img.shields.io/badge/61eeffb-skeleton?label=%F0%9F%92%80%20bswck/skeleton&labelColor=black&color=grey&link=https%3A//github.com/bswck/skeleton)](https://github.com/bswck/skeleton/tree/61eeffb)
+# proxyvars [![skeleton](https://img.shields.io/badge/7935235-skeleton?label=%F0%9F%92%80%20bswck/skeleton&labelColor=black&color=grey&link=https%3A//github.com/bswck/skeleton)](https://github.com/bswck/skeleton/tree/7935235)
 [![Package version](https://img.shields.io/pypi/v/proxyvars?label=PyPI)](https://pypi.org/project/proxyvars/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/proxyvars.svg?logo=python&label=Python)](https://pypi.org/project/proxyvars/)
 
 [![Tests](https://github.com/bswck/proxyvars/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/proxyvars/actions/workflows/test.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/proxyvars.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/proxyvars)
+[![Documentation Status](https://readthedocs.org/projects/proxyvars/badge/?version=latest)](https://proxyvars.readthedocs.io/en/latest/?badge=latest)
+[![License](https://img.shields.io/github/license/bswck/proxyvars.svg?label=License)](https://github.com/bswck/proxyvars/blob/HEAD/LICENSE)
+
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-[![License](https://img.shields.io/github/license/bswck/proxyvars.svg?label=License)](https://github.com/bswck/proxyvars/blob/HEAD/LICENSE)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 
 A simple and straight-forward Python module for creating context-dependent proxy objects.
 
 As for now, the documentation is mostly in the codebase (check relevant docstrings of `proxy()`, `const_proxy()`, `lookup_proxy()`, `proxy_field_accessor()`, `proxy_item_accessor()` and `proxy_attribute_accessor()` for more information).
 
 # Installation
@@ -51,17 +53,17 @@
 ```shell
 poetry add proxyvars
 ```
 
 ## For contributors
 
 <!--
-This section was generated from bswck/skeleton@61eeffb.
+This section was generated from bswck/skeleton@7935235.
 Instead of changing this particular file, you might want to alter the template:
-https://github.com/bswck/skeleton/tree/61eeffb/project/README.md.jinja
+https://github.com/bswck/skeleton/tree/7935235/project/README.md.jinja
 -->
 
 > [!Note]
 > If you use Windows, it is highly recommended to complete the installation in the way presented below through [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).
```

