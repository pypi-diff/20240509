# Comparing `tmp/py_gadzooks-0.2.8.tar.gz` & `tmp/py_gadzooks-0.2.9.tar.gz`

## Comparing `py_gadzooks-0.2.8.tar` & `py_gadzooks-0.2.9.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/gadzooks/__init__.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/gadzooks/build_docs.py
--rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/gadzooks/check_version.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/gadzooks/loc_summarize.py
--rwxr-xr-x   0        0        0     1385 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/gadzooks/main.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/LICENSE
--rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/README.md
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 py_gadzooks-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 py_gadzooks-0.2.9/gadzooks/__init__.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 py_gadzooks-0.2.9/gadzooks/build_docs.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 py_gadzooks-0.2.9/gadzooks/check_format.py
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 py_gadzooks-0.2.9/gadzooks/check_version.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 py_gadzooks-0.2.9/gadzooks/loc_summarize.py
+-rwxr-xr-x   0        0        0     1464 2020-02-02 00:00:00.000000 py_gadzooks-0.2.9/gadzooks/main.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 py_gadzooks-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 py_gadzooks-0.2.9/LICENSE
+-rw-r--r--   0        0        0     6756 2020-02-02 00:00:00.000000 py_gadzooks-0.2.9/README.md
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 py_gadzooks-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 py_gadzooks-0.2.9/PKG-INFO
```

### Comparing `py_gadzooks-0.2.8/gadzooks/__init__.py` & `py_gadzooks-0.2.9/gadzooks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from argparse import ArgumentParser, Namespace
 import sys
 from typing import ClassVar, Optional
 
 
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 
 
 def error(msg: str) -> None:
     """Prints an error message and exits the program with return code 1."""
     print(f'ERROR: {msg}', file=sys.stderr)
     sys.exit(1)
```

### Comparing `py_gadzooks-0.2.8/gadzooks/build_docs.py` & `py_gadzooks-0.2.9/gadzooks/build_docs.py`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.8/gadzooks/check_version.py` & `py_gadzooks-0.2.9/gadzooks/check_version.py`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.8/gadzooks/loc_summarize.py` & `py_gadzooks-0.2.9/gadzooks/loc_summarize.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,13 +23,13 @@
         cmd = ['radon', 'raw'] + list(paths) + ['-s']
         lines = subprocess.check_output(cmd, text=True).splitlines()
         num_files = sum(not line.startswith(' ') for line in lines) - 1
         assert lines[-12] == '** Total **'
         print(f'Checked {num_files} source file(s)\n')
         print('LINE STATS')
         print('----------')
-        pairs = [line.strip().split(": ", maxsplit=1) for line in lines[-11:-4]]  # type: ignore[misc]
+        pairs = [line.strip().split(': ', maxsplit=1) for line in lines[-11:-4]]  # type: ignore[misc]
         width = len(pairs[0][1])
         for (key, val) in pairs:
             key = (key + ':').ljust(16)
             val = val.rjust(width)
             print(f'{key} {val}')
```

### Comparing `py_gadzooks-0.2.8/gadzooks/main.py` & `py_gadzooks-0.2.9/gadzooks/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python3
 
 import argparse
 from typing import cast
 
 from gadzooks import Subcommand, __version__
 from gadzooks.build_docs import BuildDocs
+from gadzooks.check_format import CheckFormat
 from gadzooks.check_version import CheckVersion
 from gadzooks.loc_summarize import LinesOfCodeSummarize
 
 
 SUBCOMMANDS: dict[str, type[Subcommand]] = {
     'build-docs': BuildDocs,
+    'check-format': CheckFormat,
     'check-version': CheckVersion,
     'loc-summarize': LinesOfCodeSummarize,
 }
 
 def main() -> None:
     """Main entry point for gadzooks executable."""
     parser = argparse.ArgumentParser()
```

### Comparing `py_gadzooks-0.2.8/LICENSE` & `py_gadzooks-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py_gadzooks-0.2.8/README.md` & `py_gadzooks-0.2.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
     - [Lines of code summary](#loc-summarize)
     - [Check version consistency](#check-version)
+    - [Check code formatting](#check-format)
     - [Build documentation](#build-docs)
 
 ## Installation
 
 ```text
 pip install py-gadzooks
 ```
@@ -30,14 +31,15 @@
 Once installed, `gadzooks` will be available as a command-line executable.
 
 Different tools can be called as subcommands, which are as follows:
 
 | Subcommand | Description |
 | ---------- | ----------- |
 | `build-docs` | Build project documentation |
+| `check-format` | Check code formatting |
 | `check-version` | Check version consistency |
 | `loc-summarize` | Summarize lines of code |
 
 To view the help and options for a particular subcommand, do:
 
 ```text
 gadzooks <SUBCOMMAND> --help
@@ -94,14 +96,40 @@
 | `--version-path VERSION_PATH` | Path to file where package version is defined | `<PKG_NAME>/__init__.py` |
 | `--check-tag` | Check that latest tag is valid | |
 | `--check-dist` | Check version of latest built wheel | |
 | `--dist-dir DIST_DIR` | Directory where wheels are built | `dist` |
 | `--changelog CHANGELOG` | Changelog file | |
 | `--changelog-version-regex` | Pattern to match to find version in changelog file (`{version}` within the pattern marks the target version) | `{version}` |
 
+### `check-format`
+
+Runs an installed code formatter on source files. Currently supported formatters (for Python code only) are:
+
+- [Black](https://black.readthedocs.io/en/stable/)
+- [Ruff](https://docs.astral.sh/ruff/formatter)
+- [Yapf](https://github.com/google/yapf)
+
+Example usage:
+
+```text
+gadzooks check-format . --formatter black --ignore-patterns "\s*" -- --line-length 120 --skip-string-normalization
+```
+
+If `--` is present, the arguments that come before it are `gadzooks`' arguments; those that come after it are passed to the formatter program.
+
+`check-format` does not (by default) edit the code in place, but rather prints out a stream of _diffs_ indicating what formatting changes would be made. The user may choose to apply the changes or not.
+
+The program exits with return code 1 if there are any changes, and 0 otherwise.
+
+| Option | Description | Default |
+| ------ | ----------- | ------- |
+| (positional) | Files or directories to check | (required) |
+| `--formatter` | Formatter program (`black`, `ruff`, or `yapf`) | `black` |
+| `--ignore-patterns` | One or more regular expressions that will be ignored in the diffs (e.g. `"\s*"` ignores changes where whitespace lines are added or removed) | |
+
 ### `build-docs`
 
 Runs a command to build docs within your project.
 
 A typical pattern is to build documentation from template files such as Markdown, then save them out as HTML. Often this is done external to source control via some CI process which builds and deploys docs to a website. However, in some cases you may want to commit the built documentation to your Git repo. This is an easy step to forget, so `gadzooks` let you make the action into a `pre-commit` hook.
 
 Example usage:
```

### Comparing `py_gadzooks-0.2.8/PKG-INFO` & `py_gadzooks-0.2.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: py-gadzooks
-Version: 0.2.8
+Version: 0.2.9
 Summary: A collection of code maintenance tools for Python projects, intended to be used within git hooks.
 Project-URL: Documentation, https://github.com/jeremander/gadzooks#readme
 Project-URL: Issues, https://github.com/jeremander/gadzooks/issues
 Project-URL: Source, https://github.com/jeremander/gadzooks
 Author-email: Jeremy Silver <jeremys@nessiness.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -26,14 +26,15 @@
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
     - [Lines of code summary](#loc-summarize)
     - [Check version consistency](#check-version)
+    - [Check code formatting](#check-format)
     - [Build documentation](#build-docs)
 
 ## Installation
 
 ```text
 pip install py-gadzooks
 ```
@@ -45,14 +46,15 @@
 Once installed, `gadzooks` will be available as a command-line executable.
 
 Different tools can be called as subcommands, which are as follows:
 
 | Subcommand | Description |
 | ---------- | ----------- |
 | `build-docs` | Build project documentation |
+| `check-format` | Check code formatting |
 | `check-version` | Check version consistency |
 | `loc-summarize` | Summarize lines of code |
 
 To view the help and options for a particular subcommand, do:
 
 ```text
 gadzooks <SUBCOMMAND> --help
@@ -109,14 +111,40 @@
 | `--version-path VERSION_PATH` | Path to file where package version is defined | `<PKG_NAME>/__init__.py` |
 | `--check-tag` | Check that latest tag is valid | |
 | `--check-dist` | Check version of latest built wheel | |
 | `--dist-dir DIST_DIR` | Directory where wheels are built | `dist` |
 | `--changelog CHANGELOG` | Changelog file | |
 | `--changelog-version-regex` | Pattern to match to find version in changelog file (`{version}` within the pattern marks the target version) | `{version}` |
 
+### `check-format`
+
+Runs an installed code formatter on source files. Currently supported formatters (for Python code only) are:
+
+- [Black](https://black.readthedocs.io/en/stable/)
+- [Ruff](https://docs.astral.sh/ruff/formatter)
+- [Yapf](https://github.com/google/yapf)
+
+Example usage:
+
+```text
+gadzooks check-format . --formatter black --ignore-patterns "\s*" -- --line-length 120 --skip-string-normalization
+```
+
+If `--` is present, the arguments that come before it are `gadzooks`' arguments; those that come after it are passed to the formatter program.
+
+`check-format` does not (by default) edit the code in place, but rather prints out a stream of _diffs_ indicating what formatting changes would be made. The user may choose to apply the changes or not.
+
+The program exits with return code 1 if there are any changes, and 0 otherwise.
+
+| Option | Description | Default |
+| ------ | ----------- | ------- |
+| (positional) | Files or directories to check | (required) |
+| `--formatter` | Formatter program (`black`, `ruff`, or `yapf`) | `black` |
+| `--ignore-patterns` | One or more regular expressions that will be ignored in the diffs (e.g. `"\s*"` ignores changes where whitespace lines are added or removed) | |
+
 ### `build-docs`
 
 Runs a command to build docs within your project.
 
 A typical pattern is to build documentation from template files such as Markdown, then save them out as HTML. Often this is done external to source control via some CI process which builds and deploys docs to a website. However, in some cases you may want to commit the built documentation to your Git repo. This is an easy step to forget, so `gadzooks` let you make the action into a `pre-commit` hook.
 
 Example usage:
```

