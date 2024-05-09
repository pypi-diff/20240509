# Comparing `tmp/rubrical-1.0.1.tar.gz` & `tmp/rubrical-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubrical-1.0.1.tar", max compression
+gzip compressed data, was "rubrical-1.0.2.tar", max compression
```

## Comparing `rubrical-1.0.1.tar` & `rubrical-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    15976 2024-02-16 12:01:51.397360 rubrical-1.0.1/LICENSE
--rw-r--r--   0        0        0     1774 2024-02-16 12:01:51.397360 rubrical-1.0.1/README.md
--rw-r--r--   0        0        0     1936 2024-02-16 12:02:09.013282 rubrical-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/__init__.py
--rw-r--r--   0        0        0      784 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/comparisons/__init__.py
--rw-r--r--   0        0        0     2694 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/comparisons/semversion.py
--rw-r--r--   0        0        0      767 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/comparisons/string.py
--rw-r--r--   0        0        0      554 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/comparisons/utils.py
--rw-r--r--   0        0        0      568 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/enum.py
--rw-r--r--   0        0        0     2863 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/main.py
--rw-r--r--   0        0        0        0 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/package_managers/__init__.py
--rw-r--r--   0        0        0     2765 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/package_managers/base_package_manager.py
--rw-r--r--   0        0        0     1448 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/package_managers/go.py
--rw-r--r--   0        0        0     1781 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/package_managers/jsonnet.py
--rw-r--r--   0        0        0     5273 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/package_managers/nodejs.py
--rw-r--r--   0        0        0     2707 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/package_managers/python.py
--rw-r--r--   0        0        0      271 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/package_managers/utilities/git.py
--rw-r--r--   0        0        0     2537 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/reporters/gh.py
--rw-r--r--   0        0        0     1508 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/reporters/terminal.py
--rw-r--r--   0        0        0     4286 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/rubrical.py
--rw-r--r--   0        0        0        0 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/schemas/__init__.py
--rw-r--r--   0        0        0      578 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/schemas/configuration.py
--rw-r--r--   0        0        0      312 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/schemas/package.py
--rw-r--r--   0        0        0      235 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/schemas/results.py
--rw-r--r--   0        0        0        0 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/subcommands/__init__.py
--rw-r--r--   0        0        0     1103 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/subcommands/configs.py
--rw-r--r--   0        0        0      633 2024-02-16 12:01:51.397360 rubrical-1.0.1/rubrical/utilities/console.py
--rw-r--r--   0        0        0     2833 1970-01-01 00:00:00.000000 rubrical-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    15976 2024-05-09 10:01:39.226434 rubrical-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1774 2024-05-09 10:01:39.226434 rubrical-1.0.2/README.md
+-rw-r--r--   0        0        0     1958 2024-05-09 10:01:52.026500 rubrical-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/__init__.py
+-rw-r--r--   0        0        0      784 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/comparisons/__init__.py
+-rw-r--r--   0        0        0     2694 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/comparisons/semversion.py
+-rw-r--r--   0        0        0      767 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/comparisons/string.py
+-rw-r--r--   0        0        0      554 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/comparisons/utils.py
+-rw-r--r--   0        0        0      568 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/enum.py
+-rw-r--r--   0        0        0     2863 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/main.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/package_managers/__init__.py
+-rw-r--r--   0        0        0     2765 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/package_managers/base_package_manager.py
+-rw-r--r--   0        0        0     1448 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/package_managers/go.py
+-rw-r--r--   0        0        0     1781 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/package_managers/jsonnet.py
+-rw-r--r--   0        0        0     5273 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/package_managers/nodejs.py
+-rw-r--r--   0        0        0     2707 2024-05-09 10:01:39.226434 rubrical-1.0.2/rubrical/package_managers/python.py
+-rw-r--r--   0        0        0      271 2024-05-09 10:01:39.230434 rubrical-1.0.2/rubrical/package_managers/utilities/git.py
+-rw-r--r--   0        0        0     2560 2024-05-09 10:01:39.230434 rubrical-1.0.2/rubrical/reporters/gh.py
+-rw-r--r--   0        0        0     1508 2024-05-09 10:01:39.230434 rubrical-1.0.2/rubrical/reporters/terminal.py
+-rw-r--r--   0        0        0     4286 2024-05-09 10:01:39.230434 rubrical-1.0.2/rubrical/rubrical.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:01:39.230434 rubrical-1.0.2/rubrical/schemas/__init__.py
+-rw-r--r--   0        0        0      578 2024-05-09 10:01:39.230434 rubrical-1.0.2/rubrical/schemas/configuration.py
+-rw-r--r--   0        0        0      312 2024-05-09 10:01:39.230434 rubrical-1.0.2/rubrical/schemas/package.py
+-rw-r--r--   0        0        0      235 2024-05-09 10:01:39.230434 rubrical-1.0.2/rubrical/schemas/results.py
+-rw-r--r--   0        0        0        0 2024-05-09 10:01:39.230434 rubrical-1.0.2/rubrical/subcommands/__init__.py
+-rw-r--r--   0        0        0     1103 2024-05-09 10:01:39.230434 rubrical-1.0.2/rubrical/subcommands/configs.py
+-rw-r--r--   0        0        0      633 2024-05-09 10:01:39.230434 rubrical-1.0.2/rubrical/utilities/console.py
+-rw-r--r--   0        0        0     2877 1970-01-01 00:00:00.000000 rubrical-1.0.2/PKG-INFO
```

### Comparing `rubrical-1.0.1/LICENSE` & `rubrical-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/README.md` & `rubrical-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/pyproject.toml` & `rubrical-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 [tool.isort]
 profile = "black"
 
 [tool.setuptools_scm]
 
 [tool.poetry]
 name = "rubrical"
-version = "1.0.1"
+version = "1.0.2"
 description = "A CLI to encourage (😅) people to update their dependencies!"
 authors = ["Ivan Lee <ivanklee86@gmail.com>"]
 license = "MPL-2.0"
 homepage = "https://github.com/ivanklee86/rubrical"
 repository = "https://github.com/ivanklee86/rubrical"
 readme = "README.md"
 classifiers=[
@@ -45,38 +45,39 @@
 ]
 
 [tool.poetry.scripts]
 rubrical = "rubrical.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.12"
-typer = {extras = ["all"], version = "^0.9.0"}
+typer = {extras = ["all"], version = "^0.12.0"}
 pydantic = "^2.5.2"
 semver = "^3.0.2"
 pygithub = "^2.0.0"
 python-benedict = {extras = ["all"], version = "^0.33.0"}
 pyyaml = "^6.0"
-requirements-parser = "^0.5.0"
-pyproject-parser = "^0.9.1"
+requirements-parser = "^0.9.0"
+pyproject-parser = "^0.11.0"
 setuptools = "^69.0.0"
+dom-toml = "^2.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.0.0"
 mypy = "^1.7.1"
 pytest = "^8.0.0"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 pytest-flake8 = "^1.1.1"
 pytest-html = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.0.2"
 setuptools-scm = "^8.0.0"
 twine = "^5.0.0"
 pre-commit = "^3.4.0"
 isort = "^5.13.1"
-ruff = "^0.2.0"
+ruff = "^0.4.0"
 python-dotenv = "^1.0.0"
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.4"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
```

### Comparing `rubrical-1.0.1/rubrical/comparisons/__init__.py` & `rubrical-1.0.2/rubrical/comparisons/__init__.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/comparisons/semversion.py` & `rubrical-1.0.2/rubrical/comparisons/semversion.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/comparisons/string.py` & `rubrical-1.0.2/rubrical/comparisons/string.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/comparisons/utils.py` & `rubrical-1.0.2/rubrical/comparisons/utils.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/enum.py` & `rubrical-1.0.2/rubrical/enum.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/main.py` & `rubrical-1.0.2/rubrical/main.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/package_managers/base_package_manager.py` & `rubrical-1.0.2/rubrical/package_managers/base_package_manager.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/package_managers/go.py` & `rubrical-1.0.2/rubrical/package_managers/go.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/package_managers/jsonnet.py` & `rubrical-1.0.2/rubrical/package_managers/jsonnet.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/package_managers/nodejs.py` & `rubrical-1.0.2/rubrical/package_managers/nodejs.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/package_managers/python.py` & `rubrical-1.0.2/rubrical/package_managers/python.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/reporters/gh.py` & `rubrical-1.0.2/rubrical/reporters/gh.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,40 +4,41 @@
 
 from rubrical.enum import PackageCheck
 from rubrical.schemas.results import PackageCheckResult
 from rubrical.utilities import console
 
 
 def _generate_report(reporting_data: Dict[str, List[PackageCheckResult]]):
-    test = """
+    rep = """
 ## [Rubrical](https://github.com/ivanklee86/rubrical) Report
 
 """
-
     for package_manager in reporting_data.keys():
-        test += f"### {package_manager}\n\n"
+        rep += f"### {package_manager}\n\n"
 
         not_ok_results = [
             x
             for x in reporting_data[package_manager]
             if x.check in [PackageCheck.BLOCK, PackageCheck.WARN]
         ]
         if not_ok_results:
-            test += "| File | Dependency | Result |\n"
-            test += "|------|------------|--------|\n"
+            rep += "| File | Dependency | Result |\n"
+            rep += "|------|------------|--------|\n"
 
             for result in not_ok_results:
                 if result.check == PackageCheck.BLOCK:
-                    test += f"| {result.file} | {result.name} | ❌ {result.version_package} < {result.version_block}, update to >= {result.version_warn} |\n"
+                    rep += f"| {result.file} | {result.name} | ❌ {result.version_package} < {result.version_block}, update to >= {result.version_warn} |\n"
                 elif result.check == PackageCheck.WARN:
-                    test += f"| {result.file} | {result.name} | ⚠️ {result.version_package} < {result.version_warn}, update to >= {result.version_warn} |\n"
+                    rep += f"| {result.file} | {result.name} | ⚠️ {result.version_package} < {result.version_warn}, update to >= {result.version_warn} |\n"
         else:
-            test += "🟢 All dependencies up to date!"
+            rep += "🟢 All dependencies up to date!\n"
+
+        rep += "\n"
 
-    return test
+    return rep.rstrip()
 
 
 def report_github(
     access_token: str,
     custom_url: str,
     repository_name: str,
     pr_id: int,
```

### Comparing `rubrical-1.0.1/rubrical/reporters/terminal.py` & `rubrical-1.0.2/rubrical/reporters/terminal.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/rubrical.py` & `rubrical-1.0.2/rubrical/rubrical.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/schemas/configuration.py` & `rubrical-1.0.2/rubrical/schemas/configuration.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/subcommands/configs.py` & `rubrical-1.0.2/rubrical/subcommands/configs.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/rubrical/utilities/console.py` & `rubrical-1.0.2/rubrical/utilities/console.py`

 * *Files identical despite different names*

### Comparing `rubrical-1.0.1/PKG-INFO` & `rubrical-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: rubrical
-Version: 1.0.1
+Version: 1.0.2
 Summary: A CLI to encourage (😅) people to update their dependencies!
 Home-page: https://github.com/ivanklee86/rubrical
 License: MPL-2.0
 Author: Ivan Lee
 Author-email: ivanklee86@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
+Requires-Dist: dom-toml (>=2.0.0,<3.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: pygithub (>=2.0.0,<3.0.0)
-Requires-Dist: pyproject-parser (>=0.9.1,<0.10.0)
+Requires-Dist: pyproject-parser (>=0.11.0,<0.12.0)
 Requires-Dist: python-benedict[all] (>=0.33.0,<0.34.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requirements-parser (>=0.5.0,<0.6.0)
+Requires-Dist: requirements-parser (>=0.9.0,<0.10.0)
 Requires-Dist: semver (>=3.0.2,<4.0.0)
 Requires-Dist: setuptools (>=69.0.0,<70.0.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: typer[all] (>=0.12.0,<0.13.0)
 Project-URL: Repository, https://github.com/ivanklee86/rubrical
 Description-Content-Type: text/markdown
 
 # rubrical
 
 [![CI](https://github.com/ivanklee86/rubrical/actions/workflows/ci.yaml/badge.svg)](https://github.com/ivanklee86/rubrical/actions/workflows/ci.yaml) [![codecov](https://codecov.io/gh/ivanklee86/rubrical/branch/main/graph/badge.svg?token=9WJM4LBDEX)](https://codecov.io/gh/ivanklee86/rubrical) [![PyPI version](https://badge.fury.io/py/rubrical.svg)](https://badge.fury.io/py/rubrical)
```

