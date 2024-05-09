# Comparing `tmp/arktika-icebreaker-0.5.0.tar.gz` & `tmp/arktika_icebreaker-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arktika-icebreaker-0.5.0.tar", last modified: Sun Mar 24 10:36:12 2024, max compression
+gzip compressed data, was "arktika_icebreaker-0.6.0.tar", last modified: Thu May  9 08:00:31 2024, max compression
```

## Comparing `arktika-icebreaker-0.5.0.tar` & `arktika_icebreaker-0.6.0.tar`

### file list

```diff
@@ -1,36 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:36:12.506350 arktika-icebreaker-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-24 10:36:12.506350 arktika-icebreaker-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 10:36:12.506350 arktika-icebreaker-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:36:12.498350 arktika-icebreaker-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:36:12.506350 arktika-icebreaker-0.5.0/src/arktika_icebreaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-24 10:36:12.000000 arktika-icebreaker-0.5.0/src/arktika_icebreaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-24 10:36:12.000000 arktika-icebreaker-0.5.0/src/arktika_icebreaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 10:36:12.000000 arktika-icebreaker-0.5.0/src/arktika_icebreaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-24 10:36:12.000000 arktika-icebreaker-0.5.0/src/arktika_icebreaker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-24 10:36:12.000000 arktika-icebreaker-0.5.0/src/arktika_icebreaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-24 10:36:12.000000 arktika-icebreaker-0.5.0/src/arktika_icebreaker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:36:12.502350 arktika-icebreaker-0.5.0/src/icebreaker/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:36:12.502350 arktika-icebreaker-0.5.0/src/icebreaker/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/_cli/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:36:12.502350 arktika-icebreaker-0.5.0/src/icebreaker/_cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/_cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/_cli/commands/fmt.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/_cli/commands/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:36:12.502350 arktika-icebreaker-0.5.0/src/icebreaker/_cli/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/_cli/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/_cli/interfaces/_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/_cli/interfaces/_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/_cli/interfaces/_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 10:36:10.000000 arktika-icebreaker-0.5.0/src/icebreaker/version
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 10:36:12.506350 arktika-icebreaker-0.5.0/src/icebreaker/versioning/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/src/icebreaker/versioning/_version_file_based.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-24 10:35:53.000000 arktika-icebreaker-0.5.0/version
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:31.519396 arktika_icebreaker-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-09 08:00:31.519396 arktika_icebreaker-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:00:31.519396 arktika_icebreaker-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:31.511396 arktika_icebreaker-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:31.515396 arktika_icebreaker-0.6.0/src/arktika_icebreaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-09 08:00:31.000000 arktika_icebreaker-0.6.0/src/arktika_icebreaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-09 08:00:31.000000 arktika_icebreaker-0.6.0/src/arktika_icebreaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:00:31.000000 arktika_icebreaker-0.6.0/src/arktika_icebreaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 08:00:31.000000 arktika_icebreaker-0.6.0/src/arktika_icebreaker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-09 08:00:31.000000 arktika_icebreaker-0.6.0/src/arktika_icebreaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 08:00:31.000000 arktika_icebreaker-0.6.0/src/arktika_icebreaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:31.511396 arktika_icebreaker-0.6.0/src/icebreaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:31.511396 arktika_icebreaker-0.6.0/src/icebreaker/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_cli/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:31.515396 arktika_icebreaker-0.6.0/src/icebreaker/_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_cli/commands/fmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_cli/commands/fmt_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_cli/commands/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:31.515396 arktika_icebreaker-0.6.0/src/icebreaker/_cli/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_cli/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_cli/interfaces/_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_cli/interfaces/_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_cli/interfaces/_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:31.515396 arktika_icebreaker-0.6.0/src/icebreaker/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:31.515396 arktika_icebreaker-0.6.0/src/icebreaker/_internal/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_internal/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_internal/formatting/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_internal/formatting/_ruff_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:31.515396 arktika_icebreaker-0.6.0/src/icebreaker/_internal/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_internal/typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_internal/typing/_mypy_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/_internal/typing/_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:31.515396 arktika_icebreaker-0.6.0/src/icebreaker/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/testing/_test_code_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/testing/_test_code_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 08:00:29.000000 arktika_icebreaker-0.6.0/src/icebreaker/version
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:00:31.515396 arktika_icebreaker-0.6.0/src/icebreaker/versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/src/icebreaker/versioning/_version_file_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 08:00:09.000000 arktika_icebreaker-0.6.0/version
```

### Comparing `arktika-icebreaker-0.5.0/LICENSE` & `arktika_icebreaker-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arktika-icebreaker-0.5.0/PKG-INFO` & `arktika_icebreaker-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arktika-icebreaker
-Version: 0.5.0
+Version: 0.6.0
 Summary: Software Dev Kit
 Author-email: Arktika <oss@arktika.io>
 License: MIT License
         
         Copyright (c) Arktika
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,14 +37,17 @@
 Requires-Dist: build==1.*; extra == "dev"
 Requires-Dist: twine==4.*; extra == "dev"
 Requires-Dist: hypothesis==6.*; extra == "dev"
 Requires-Dist: pytest==7.*; extra == "dev"
 Requires-Dist: pytest-asyncio==0.*; extra == "dev"
 Provides-Extra: cli
 Requires-Dist: ruff==0.*; extra == "cli"
+Provides-Extra: testing
+Requires-Dist: ruff==0.*; extra == "testing"
+Requires-Dist: mypy==1.*; extra == "testing"
 
 # icebreaker
 
 Icebreaker is a software development kit (currently Python only), otherwise known as a service chassis, which provides tools to handle cross-cutting concerns in your software projects.
 
 ## Table of Contents
 * [CLI](docs/icebreaker/cli/index.md)
```

### Comparing `arktika-icebreaker-0.5.0/pyproject.toml` & `arktika_icebreaker-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,19 @@
     "pytest-asyncio==0.*",
 ]
 
 cli = [
     "ruff==0.*"
 ]
 
+testing = [
+    "ruff==0.*",
+    "mypy==1.*"
+]
+
 [project.scripts]
 icebreaker = "icebreaker.__main__:main"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [tool.setuptools.packages.find]
```

### Comparing `arktika-icebreaker-0.5.0/src/arktika_icebreaker.egg-info/PKG-INFO` & `arktika_icebreaker-0.6.0/src/arktika_icebreaker.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arktika-icebreaker
-Version: 0.5.0
+Version: 0.6.0
 Summary: Software Dev Kit
 Author-email: Arktika <oss@arktika.io>
 License: MIT License
         
         Copyright (c) Arktika
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -37,14 +37,17 @@
 Requires-Dist: build==1.*; extra == "dev"
 Requires-Dist: twine==4.*; extra == "dev"
 Requires-Dist: hypothesis==6.*; extra == "dev"
 Requires-Dist: pytest==7.*; extra == "dev"
 Requires-Dist: pytest-asyncio==0.*; extra == "dev"
 Provides-Extra: cli
 Requires-Dist: ruff==0.*; extra == "cli"
+Provides-Extra: testing
+Requires-Dist: ruff==0.*; extra == "testing"
+Requires-Dist: mypy==1.*; extra == "testing"
 
 # icebreaker
 
 Icebreaker is a software development kit (currently Python only), otherwise known as a service chassis, which provides tools to handle cross-cutting concerns in your software projects.
 
 ## Table of Contents
 * [CLI](docs/icebreaker/cli/index.md)
```

### Comparing `arktika-icebreaker-0.5.0/src/icebreaker/_cli/_cli.py` & `arktika_icebreaker-0.6.0/src/icebreaker/_cli/_cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,77 +5,101 @@
 from pathlib import Path
 import traceback
 from typing import Any
 from typing import Self
 from typing import TypeAlias
 
 from icebreaker._cli.commands.fmt import Fmt
+from icebreaker._cli.commands.fmt_check import FmtCheck
 from icebreaker._cli.commands.version import Version
 from icebreaker._cli.interfaces import ExitCode
 from icebreaker._cli.interfaces import Printer
 from icebreaker._cli.interfaces import Reader
+from icebreaker._internal.formatting import Formatter
 
 Command: TypeAlias = str
+Subcommand: TypeAlias = str | None
 Arguments: TypeAlias = dict[str, Any]
-Handler: TypeAlias = Callable[[], None]
+Handler: TypeAlias = Callable[[], ExitCode]
 
 
 class CLI:
     printer: Printer
     error_printer: Printer
     reader: Reader
+    formatter: Formatter
 
     def __init__(
         self: Self,
         printer: Printer,
         error_printer: Printer,
         reader: Reader,
+        formatter: Formatter,
     ) -> None:
         self.printer = printer
         self.error_printer = error_printer
         self.reader = reader
+        self.formatter = formatter
 
     def __call__(self: Self) -> ExitCode:
-        command_and_arguments: tuple[Command, Arguments] = self._get_called_command_and_arguments()
-        command: Command = command_and_arguments[0]
-        arguments: Arguments = command_and_arguments[1]
-        handler: Handler | None = self._get_handler(command=command, arguments=arguments)
+        command, subcommand, arguments = self._get_called_command_and_arguments()
+        handler: Handler | None = self._get_handler(command=command, subcommand=subcommand, arguments=arguments)
 
         if handler is None:
             self.error_printer(f"Unknown command: {command}\n")
             return ExitCode(1)
 
         try:
-            handler()
-            exit_code = ExitCode(0)
+            exit_code = handler()
         except BaseException:
             self.error_printer(traceback.format_exc())
             exit_code = ExitCode(1)
 
         return exit_code
 
-    def _get_called_command_and_arguments(self: Self) -> tuple[Command, Arguments]:
-        argument_parser: ArgumentParser = ArgumentParser(
-            prog="icebreaker", description="Icebreaker CLI.", exit_on_error=False
+    def _get_called_command_and_arguments(self: Self) -> tuple[Command, Subcommand, Arguments]:
+        root_argument_parser: ArgumentParser = ArgumentParser(
+            prog="icebreaker",
+            description="Icebreaker CLI.",
+            exit_on_error=False,
         )
-        subparsers: Any = argument_parser.add_subparsers(title="Commands", dest="command")
+        root_subparsers: Any = root_argument_parser.add_subparsers(title="Commands", dest="command")
 
         # Add "fmt" command
-        fmt_parser: ArgumentParser = subparsers.add_parser(name="fmt", description="Format the codebase.")
-        fmt_parser.add_argument("--check", action="store_true", default=False)
-        fmt_parser.add_argument("target", metavar="TARGET", nargs="?", default=".", type=Path)
+        fmt_parser: ArgumentParser = root_subparsers.add_parser(
+            name="fmt",
+            description="Format the codebase.",
+        )
+        fmt_parser.add_argument("--target", metavar="TARGET", default=".", type=Path)
+
+        fmt_subparsers: Any = fmt_parser.add_subparsers(title="subcommands", dest="subcommand")
+
+        # Add "fmt check" command
+        fmt_check_parser: ArgumentParser = fmt_subparsers.add_parser(
+            name="check", description="Check the formatting of the codebase."
+        )
+        fmt_check_parser.add_argument("--target", metavar="TARGET", default=".", type=Path)
 
         # Add "version" command
-        subparsers.add_parser(name="version", description="Show version number and quit.")
+        root_subparsers.add_parser(name="version", description="Show version number and quit.")
 
-        parsed_arguments: Namespace = argument_parser.parse_args()
+        parsed_arguments: Namespace = root_argument_parser.parse_args()
         arguments: Arguments = vars(parsed_arguments)
         command: Command = arguments.pop("command")
-        return command, arguments
+        subcommand: Subcommand = arguments.pop("subcommand") if "subcommand" in arguments else None
+        return command, subcommand, arguments
 
-    def _get_handler(self: Self, command: Command, arguments: Arguments) -> Handler | None:
+    def _get_handler(self: Self, command: Command, subcommand: Subcommand, arguments: Arguments) -> Handler | None:
         handler: Handler | None = None
         if command == "version":
             handler = functools.partial(Version(printer=self.printer).__call__, **arguments)
         elif command == "fmt":
-            handler = functools.partial(Fmt(printer=self.printer, error_printer=self.error_printer), **arguments)
+            if subcommand == "check":
+                handler = functools.partial(
+                    FmtCheck(printer=self.printer, error_printer=self.error_printer, formatter=self.formatter),
+                    **arguments,
+                )
+            else:
+                handler = functools.partial(
+                    Fmt(printer=self.printer, error_printer=self.error_printer, formatter=self.formatter), **arguments
+                )
         return handler
```

### Comparing `arktika-icebreaker-0.5.0/src/icebreaker/versioning/_version_file_based.py` & `arktika_icebreaker-0.6.0/src/icebreaker/versioning/_version_file_based.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from inspect import FrameInfo
 import json
 import logging
 import os
 from pathlib import Path
 from types import ModuleType
 from typing import Self
+from types import FrameType
 
 
 class VersionFileBased:
     """
     Version file based versioning.
     Allows your project to be versioned by a file.
     """
@@ -61,13 +62,13 @@
 
     def _get_calling_module(self: Self) -> Path:
         stack: list[FrameInfo] = inspect.stack()
         # 0th position in inspect.stack() will be this LOC
         # 1st position will be self.resolve_version calling this function
         # 2nd position will be the function calling us
         calling_module_frame: FrameInfo = stack[2]
-        calling_module_name: str = calling_module_frame[0]
+        calling_module_name: FrameType = calling_module_frame[0]
         calling_module: ModuleType | None = inspect.getmodule(calling_module_name)
         if not calling_module or not calling_module.__file__:
             raise ModuleNotFoundError("Could not discover calling module.")
         calling_module_path: Path = Path(calling_module.__file__)
         return calling_module_path
```

