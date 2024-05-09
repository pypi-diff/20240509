# Comparing `tmp/robotcode_runner-0.82.0.tar.gz` & `tmp/robotcode_runner-0.82.1.tar.gz`

## Comparing `robotcode_runner-0.82.0.tar` & `robotcode_runner-0.82.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0    29976 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/LICENSE.txt
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/README.md
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/pyproject.toml
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 robotcode_runner-0.82.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6306 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    29986 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/LICENSE.txt
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/README.md
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/pyproject.toml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 robotcode_runner-0.82.1/PKG-INFO
```

### Comparing `robotcode_runner-0.82.0/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.82.1/src/robotcode/runner/cli/libdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.0/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.82.1/src/robotcode/runner/cli/rebot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.0/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.82.1/src/robotcode/runner/cli/robot.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Any, List, Optional, Set, Tuple, Union, cast
 
 import click
 from robot.errors import DataError, Information
 from robot.run import USAGE, RobotFramework
 from robot.version import get_full_version
 
+import robotcode.modifiers
 from robotcode.plugin import Application, pass_application
 from robotcode.plugin.click_helper.aliases import AliasedCommand
 from robotcode.plugin.click_helper.types import add_options
 from robotcode.robot.config.loader import load_robot_config_from_path
 from robotcode.robot.config.model import RobotBaseProfile
 from robotcode.robot.config.utils import get_config_files
 
@@ -21,21 +22,25 @@
 class RobotFrameworkEx(RobotFramework):
     def __init__(
         self,
         app: Application,
         paths: List[str],
         dry: bool,
         root_folder: Optional[Path],
+        by_longname: Tuple[str, ...] = (),
+        exclude_by_longname: Tuple[str, ...] = (),
     ) -> None:
         super().__init__()
         self.app = app
         self.paths = paths
         self.dry = dry
         self.root_folder = root_folder
         self._orig_cwd = Path.cwd()
+        self.by_longname = by_longname
+        self.exclude_by_longname = exclude_by_longname
 
     def parse_arguments(self, cli_args: Any) -> Any:
         if self.root_folder is not None and Path.cwd() != self.root_folder:
             self.app.verbose(f"Changing working directory from {self._orig_cwd} to {self.root_folder}")
             os.chdir(self.root_folder)
 
         try:
@@ -57,14 +62,26 @@
             line_end = "\n"
             raise Information(
                 "Dry run, not executing any commands. "
                 f"Would execute robot with the following options and arguments:\n"
                 f'{line_end.join((*(f"{k} = {v!r}" for k, v in options.items()), *arguments))}'
             )
 
+        modifiers = []
+        root_name = options.get("name", None)
+
+        if self.by_longname:
+            modifiers.append(robotcode.modifiers.ByLongName(*self.by_longname, root_name=root_name))
+
+        if self.exclude_by_longname:
+            modifiers.append(robotcode.modifiers.ExcludedByLongName(*self.exclude_by_longname, root_name=root_name))
+
+        if modifiers:
+            options["prerunmodifier"] = options.get("prerunmodifier", []) + modifiers
+
         return options, arguments
 
 
 # mypy: disable-error-code="arg-type"
 
 ROBOT_OPTIONS: Set[click.Command] = {
     click.option(
@@ -86,18 +103,15 @@
         message=f"%(prog)s %(version)s\n{USAGE.splitlines()[0].split(' -- ')[0].strip()} {get_full_version()}",
     ),
     click.argument("robot_options_and_args", nargs=-1, type=click.Path()),
 }
 
 
 def handle_robot_options(
-    app: Application,
-    by_longname: Tuple[str, ...],
-    exclude_by_longname: Tuple[str, ...],
-    robot_options_and_args: Tuple[str, ...],
+    app: Application, robot_options_and_args: Tuple[str, ...]
 ) -> Tuple[Optional[Path], RobotBaseProfile, List[str]]:
     robot_arguments: Optional[List[Union[str, Path]]] = None
     old_sys_path = sys.path.copy()
     try:
         _, robot_arguments = RobotFramework().parse_arguments(robot_options_and_args)
     except (DataError, Information):
         pass
@@ -114,28 +128,14 @@
             .evaluated_with_env(verbose_callback=app.verbose, error_callback=app.error)
         )
     except (TypeError, ValueError) as e:
         raise click.ClickException(str(e)) from e
 
     cmd_options = profile.build_command_line()
 
-    if by_longname:
-        sep = ";" if any(True for l in by_longname if ":" in l) else ":"
-        cmd_options += (
-            "--prerunmodifier",
-            f"robotcode.modifiers.ByLongName{sep}{sep.join(by_longname)}",
-        )
-
-    if exclude_by_longname:
-        sep = ";" if any(True for l in exclude_by_longname if ":" in l) else ":"
-        cmd_options += (
-            "--prerunmodifier",
-            f"robotcode.modifiers.ExcludedByLongName{sep}{sep.join(exclude_by_longname)}",
-        )
-
     app.verbose(
         lambda: "Executing robot with following options:\n    "
         + " ".join(f'"{o}"' for o in (cmd_options + list(robot_options_and_args)))
     )
 
     return root_folder, profile, cmd_options
 
@@ -166,26 +166,26 @@
     robotcode robot
     robotcode robot tests
     robotcode robot -i regression -e wip tests
     robotcode --profile ci robot -i regression -e wip tests
     ```
     """
 
-    root_folder, profile, cmd_options = handle_robot_options(
-        app, by_longname, exclude_by_longname, robot_options_and_args
-    )
+    root_folder, profile, cmd_options = handle_robot_options(app, robot_options_and_args)
 
     app.exit(
         cast(
             int,
             RobotFrameworkEx(
                 app,
                 (
                     [*(app.config.default_paths if app.config.default_paths else ())]
                     if profile.paths is None
                     else profile.paths if isinstance(profile.paths, list) else [profile.paths]
                 ),
                 app.config.dry,
                 root_folder,
+                by_longname,
+                exclude_by_longname,
             ).execute_cli((*cmd_options, *robot_options_and_args), exit=False),
         )
     )
```

### Comparing `robotcode_runner-0.82.0/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.82.1/src/robotcode/runner/cli/testdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.0/src/robotcode/runner/cli/discover/discover.py` & `robotcode_runner-0.82.1/src/robotcode/runner/cli/discover/discover.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,31 +458,31 @@
 
 def handle_options(
     app: Application,
     by_longname: Tuple[str, ...],
     exclude_by_longname: Tuple[str, ...],
     robot_options_and_args: Tuple[str, ...],
 ) -> Tuple[TestSuite, Collector, Optional[Dict[str, List[Diagnostic]]]]:
-    root_folder, profile, cmd_options = handle_robot_options(
-        app, by_longname, exclude_by_longname, robot_options_and_args
-    )
+    root_folder, profile, cmd_options = handle_robot_options(app, robot_options_and_args)
 
     diagnostics_logger = DiagnosticsLogger()
     try:
         _patch()
 
         options, arguments = RobotFrameworkEx(
             app,
             (
                 [*(app.config.default_paths if app.config.default_paths else ())]
                 if profile.paths is None
                 else profile.paths if isinstance(profile.paths, list) else [profile.paths]
             ),
             app.config.dry,
             root_folder,
+            by_longname,
+            exclude_by_longname,
         ).parse_arguments((*cmd_options, "--runemptysuite", *robot_options_and_args))
 
         settings = RobotSettings(options)
 
         if app.show_diagnostics:
             LOGGER.register_console_logger(**settings.console_output_config)
         else:
```

### Comparing `robotcode_runner-0.82.0/.gitignore` & `robotcode_runner-0.82.1/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.0/LICENSE.txt` & `robotcode_runner-0.82.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.0/README.md` & `robotcode_runner-0.82.1/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.82.0/pyproject.toml` & `robotcode_runner-0.82.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,18 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.82.0",
-  "robotcode-modifiers==0.82.0",
-  "robotcode-plugin==0.82.0",
-  "robotcode==0.82.0",
+  "robotcode-robot==0.82.1",
+  "robotcode-modifiers==0.82.1",
+  "robotcode-plugin==0.82.1",
+  "robotcode==0.82.1",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.82.0/PKG-INFO` & `robotcode_runner-0.82.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: robotcode-runner
-Version: 0.82.0
+Version: 0.82.1
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://opencollective.com/robotcode
 Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
 Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
 Project-URL: Source, https://github.com/robotcodedev/robotcode
@@ -21,18 +21,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.82.0
-Requires-Dist: robotcode-plugin==0.82.0
-Requires-Dist: robotcode-robot==0.82.0
-Requires-Dist: robotcode==0.82.0
+Requires-Dist: robotcode-modifiers==0.82.1
+Requires-Dist: robotcode-plugin==0.82.1
+Requires-Dist: robotcode-robot==0.82.1
+Requires-Dist: robotcode==0.82.1
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

