# Comparing `tmp/gradema-0.0.6.tar.gz` & `tmp/gradema-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gradema-0.0.6.tar", max compression
+gzip compressed data, was "gradema-0.1.0.tar", max compression
```

## Comparing `gradema-0.0.6.tar` & `gradema-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1056 2024-03-21 22:01:48.859372 gradema-0.0.6/LICENSE
--rw-r--r--   0        0        0     1919 2024-05-05 19:22:46.166690 gradema-0.0.6/README.md
--rw-r--r--   0        0        0       76 2024-04-29 15:19:53.229011 gradema-0.0.6/gradema/__init__.py
--rw-r--r--   0        0        0      216 2024-04-29 15:40:40.187785 gradema-0.0.6/gradema/grader/__init__.py
--rw-r--r--   0        0        0     3572 2024-04-29 15:40:40.179785 gradema-0.0.6/gradema/grader/_grader.py
--rw-r--r--   0        0        0      952 2024-04-23 03:17:43.476074 gradema-0.0.6/gradema/grader/_reporter.py
--rw-r--r--   0        0        0      138 2024-04-28 23:22:30.124159 gradema-0.0.6/gradema/grader/console/__init__.py
--rw-r--r--   0        0        0    11776 2024-05-05 19:55:39.691038 gradema-0.0.6/gradema/grader/console/_console.py
--rw-r--r--   0        0        0     1207 2024-04-23 03:17:09.439666 gradema-0.0.6/gradema/grader/console/_indent.py
--rw-r--r--   0        0        0     3074 2024-05-05 19:21:42.369911 gradema-0.0.6/gradema/grader/console/_runner.py
--rw-r--r--   0        0        0      752 2024-04-27 03:22:41.296861 gradema-0.0.6/gradema/grader/console/_util.py
--rw-r--r--   0        0        0       81 2024-04-18 04:40:01.722764 gradema-0.0.6/gradema/section/__init__.py
--rw-r--r--   0        0        0     1806 2024-04-18 04:09:33.425423 gradema-0.0.6/gradema/section/_section.py
--rw-r--r--   0        0        0     1053 2024-05-04 18:58:24.811647 gradema-0.0.6/gradema/test/__init__.py
--rw-r--r--   0        0        0     1302 2024-05-07 18:27:21.191922 gradema-0.0.6/gradema/test/_command.py
--rw-r--r--   0        0        0      339 2024-04-29 15:39:17.702812 gradema-0.0.6/gradema/test/_dummy.py
--rw-r--r--   0        0        0     1610 2024-05-07 18:37:25.131177 gradema-0.0.6/gradema/test/_exists.py
--rw-r--r--   0        0        0     4159 2024-05-05 23:17:52.897199 gradema-0.0.6/gradema/test/_python.py
--rw-r--r--   0        0        0     7214 2024-05-05 20:01:17.638954 gradema-0.0.6/gradema/test/_reporter.py
--rw-r--r--   0        0        0     2197 2024-05-04 04:51:27.181724 gradema-0.0.6/gradema/test/_rust.py
--rw-r--r--   0        0        0     3949 2024-05-07 18:30:33.234225 gradema-0.0.6/gradema/test/_stdio.py
--rw-r--r--   0        0        0      511 2024-04-29 15:38:21.742151 gradema-0.0.6/gradema/test/_test.py
--rw-r--r--   0        0        0      256 2024-05-04 02:11:16.307576 gradema-0.0.6/gradema/test/argument.py
--rw-r--r--   0        0        0      621 2024-05-07 18:37:34.759292 gradema-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2766 1970-01-01 00:00:00.000000 gradema-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-03-21 22:01:48.859372 gradema-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5522 2024-05-08 23:45:23.741198 gradema-0.1.0/README.md
+-rw-r--r--   0        0        0       76 2024-04-29 15:19:53.229011 gradema-0.1.0/gradema/__init__.py
+-rw-r--r--   0        0        0      216 2024-04-29 15:40:40.187785 gradema-0.1.0/gradema/grader/__init__.py
+-rw-r--r--   0        0        0     3572 2024-05-08 22:51:43.094360 gradema-0.1.0/gradema/grader/_grader.py
+-rw-r--r--   0        0        0      952 2024-05-08 22:51:43.070359 gradema-0.1.0/gradema/grader/_reporter.py
+-rw-r--r--   0        0        0      138 2024-04-28 23:22:30.124159 gradema-0.1.0/gradema/grader/console/__init__.py
+-rw-r--r--   0        0        0    12810 2024-05-09 00:06:43.720607 gradema-0.1.0/gradema/grader/console/_console.py
+-rw-r--r--   0        0        0     1207 2024-04-23 03:17:09.439666 gradema-0.1.0/gradema/grader/console/_indent.py
+-rw-r--r--   0        0        0     3992 2024-05-08 22:51:43.090360 gradema-0.1.0/gradema/grader/console/_runner.py
+-rw-r--r--   0        0        0      752 2024-04-27 03:22:41.296861 gradema-0.1.0/gradema/grader/console/_util.py
+-rw-r--r--   0        0        0       81 2024-04-18 04:40:01.722764 gradema-0.1.0/gradema/section/__init__.py
+-rw-r--r--   0        0        0     1806 2024-04-18 04:09:33.425423 gradema-0.1.0/gradema/section/_section.py
+-rw-r--r--   0        0        0     1105 2024-05-09 00:38:37.039471 gradema-0.1.0/gradema/test/__init__.py
+-rw-r--r--   0        0        0     1302 2024-05-08 22:51:43.078359 gradema-0.1.0/gradema/test/_command.py
+-rw-r--r--   0        0        0      339 2024-04-29 15:39:17.702812 gradema-0.1.0/gradema/test/_dummy.py
+-rw-r--r--   0        0        0     2281 2024-05-08 22:51:43.078359 gradema-0.1.0/gradema/test/_exists.py
+-rw-r--r--   0        0        0     4265 2024-05-09 00:38:37.047471 gradema-0.1.0/gradema/test/_python.py
+-rw-r--r--   0        0        0     7214 2024-05-08 22:51:57.750534 gradema-0.1.0/gradema/test/_reporter.py
+-rw-r--r--   0        0        0     2197 2024-05-08 22:51:57.750534 gradema-0.1.0/gradema/test/_rust.py
+-rw-r--r--   0        0        0     3949 2024-05-08 22:51:57.750534 gradema-0.1.0/gradema/test/_stdio.py
+-rw-r--r--   0        0        0      511 2024-04-29 15:38:21.742151 gradema-0.1.0/gradema/test/_test.py
+-rw-r--r--   0        0        0      256 2024-05-04 02:11:16.307576 gradema-0.1.0/gradema/test/argument.py
+-rw-r--r--   0        0        0      903 2024-05-09 00:39:48.188321 gradema-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6276 1970-01-01 00:00:00.000000 gradema-0.1.0/PKG-INFO
```

### Comparing `gradema-0.0.6/LICENSE` & `gradema-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gradema-0.0.6/gradema/grader/_grader.py` & `gradema-0.1.0/gradema/grader/_grader.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.6/gradema/grader/_reporter.py` & `gradema-0.1.0/gradema/grader/_reporter.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.6/gradema/grader/console/_console.py` & `gradema-0.1.0/gradema/grader/console/_console.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import dataclasses
 import difflib
 import io
 import shlex
 import shutil
 import subprocess
 import traceback
+import webbrowser
 from pathlib import Path
 from typing import TextIO, Optional, Sequence, Mapping
 
 from rich import markup
 from rich.console import Console
 from rich.prompt import Prompt
 
@@ -85,15 +86,16 @@
 
 
 @dataclasses.dataclass
 class ConsoleTestReporter(TestReporter):
     reporter: "ConsoleGraderReporter"
 
     def log(self, message: str) -> None:
-        self.reporter.console.print(markup.escape(message))
+        indent = indentation(self.reporter.depth)
+        self.reporter.console.print(indent + markup.escape(message))
 
     def log_unexpected_exception(self, exception: BaseException) -> None:
         indent = indentation(self.reporter.depth)
         buffer = io.StringIO()
         traceback.print_exception(exception, file=buffer)
         indented_text = indent_text(self.reporter.depth, buffer.getvalue())
         # make end="" because the exception text should have a trailing newline
@@ -123,21 +125,24 @@
         self.reporter.console.print(f"{indent}Running command: [magenta]{markup.escape(shlex.join(command))}[/magenta]")
         return CommandData(self.reporter.stdout, self.reporter.stderr)
 
     def report_stdio_command(self, command: Sequence[str], test_identifier: str, input_file: Optional[Path], stdout_as_output: bool) -> StdioCommandData:
         indent = indentation(self.reporter.depth)
         indent_plus = indentation(self.reporter.depth + 1)
         output_file = self.__get_output_file(test_identifier)
-        self.reporter.console.print(f"{indent}Command to be run: [magenta]{markup.escape(shlex.join(command))}[/magenta]")
+        # NOTE: On Windows shlex.join will almost always result in quoting the entire argument.
+        #   Because of this, we need to turn off automatic highlighting, or it won't be magenta, and won't be easily visible on PowerShell
+        self.reporter.console.print(f"{indent}Command to be run: [magenta]{markup.escape(shlex.join(command))}[/magenta]", highlight=False)
         if input_file is not None or stdout_as_output:
             self.reporter.console.print(f"{indent}Command to be run including I/O redirection:")
             self.reporter.console.print(
                 f"{indent}[magenta]{markup.escape(shlex.join(command))}[/magenta]"
                 + (f" \\\n{indent_plus}[magenta]< {markup.escape(shlex.quote(str(input_file)))}[/magenta]" if input_file is not None else "")
-                + (f" \\\n{indent_plus}[magenta]> {markup.escape(shlex.quote(str(output_file)))}[/magenta]" if stdout_as_output else "")
+                + (f" \\\n{indent_plus}[magenta]> {markup.escape(shlex.quote(str(output_file)))}[/magenta]" if stdout_as_output else ""),
+                highlight=False,
             )
 
         return StdioCommandData(output_file, self.reporter.stdout, self.reporter.stderr)
 
     def maybe_launch_debugger(self, command: Sequence[str]) -> None:
         indent = indentation(self.reporter.depth)
         if self.reporter.debug_mode:
@@ -155,21 +160,35 @@
                     launch_debugger = False
                     break
             if launch_debugger:
                 subprocess.run(command)
 
     def report_diff_result(self, test_identifier: str, goal_file: Path, output_file: Path, similarity: float, fuzzy: bool) -> None:
         indent = indentation(self.reporter.depth)
-        self.reporter.console.print(f"{indent}Diff between [yellow]{markup.escape(str(goal_file))}[/yellow] and [yellow]{markup.escape(str(output_file))}[/yellow]")
+        self.reporter.console.print(
+            f"{indent}Diff between [yellow]{markup.escape(shlex.quote(str(goal_file)))}[/yellow] and [yellow]{markup.escape(shlex.quote(str(output_file)))}[/yellow]"
+        )
         # TODO Customize stdio directory here
         directory = TEST_DIRECTORY / "stdio/diffs"
         directory.mkdir(parents=True, exist_ok=True)
         html_output = directory / f"{test_identifier}.html"
         html_diff(goal_file, output_file, html_output)
-        self.reporter.console.print(f"{indent}Diff available to view at file://{html_output.resolve().absolute()}")
+        # NOTE: file:// will not be highlighted on Windows in PowerShell, Command Prompt, or Git Bash
+        url = f"file://{html_output.resolve().absolute()}"
+        self.reporter.console.print(f"{indent}Diff available to view at {url}")
+        if self.reporter.debug_mode and similarity < 1.0:
+            while True:
+                response = Prompt.ask(
+                    prompt=f"{indent}Press [cyan]Enter[/cyan] to continue, or type 'o' and then [cyan]Enter[/cyan] to open this diff view in the web browser",
+                    console=self.reporter.console,
+                )
+                if response == "":
+                    break
+                if response[0].lower() == "o":
+                    webbrowser.open(url)
 
     def report_file_exists_test(self, file: Path, expected: str) -> None:
         indent = indentation(self.reporter.depth)
         self.reporter.console.print(f"{indent}Checking for the existence of '{file}' and its containing type of data: {expected}")
 
     def report_file_exists_test_result(self, file: Path, expected: str, is_correct: bool, actual: Optional[str]) -> None:
         indent_plus = indentation(self.reporter.depth + 1)
```

### Comparing `gradema-0.0.6/gradema/grader/console/_indent.py` & `gradema-0.1.0/gradema/grader/console/_indent.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.6/gradema/grader/console/_runner.py` & `gradema-0.1.0/gradema/grader/console/_runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import argparse
 import sys
 from pathlib import Path
 
 from rich.console import Console
 from rich.text import Text
 
 from ._console import ConsoleGraderReporter
@@ -34,36 +35,56 @@
     console.print(f"[blue]{'=' * console.width}[/blue]")
 
 
 def run_grader(args: list[str], section: Section) -> int:
     if not section.is_pointed:
         raise ValueError("The root section must be pointed!")
     assert section.points is not None
+    parser = argparse.ArgumentParser(
+        prog="Gradema Autograder",
+        epilog="Gradema - created by Lavender Shannon for Dr. Taylor",
+    )
+    parser.add_argument("-g", "--grade", action="store_true")
+    parser.add_argument("-d", "--debug", action="store_true")
+    try:
+        parsed_args = parser.parse_args(args)
+    except SystemExit as e:
+        code = e.code
+        assert isinstance(code, int)
+        return code
+
     # Useful documentation here: https://rich.readthedocs.io/en/latest/markup.html
     console = Console(soft_wrap=True)
     welcome(console)
 
     interactive = True
     debug_mode = True
-    try:
-        console.print("Press [cyan]Enter[/cyan] now to continue")
-        input()
-    except EOFError:
-        interactive = False
-        debug_mode = False
-
-    if interactive:
-        console.print(
-            """Which of the following modes do you want to run in?
-    1) debug+grade mode (d)
-    2) grade only mode (g)
-Type 'd' or 'g', then hit [cyan]Enter[/cyan]."""
-        )
-        mode_input = input()
-        debug_mode = mode_input == "" or mode_input[0].lower() != "g"
+    if not parsed_args.debug:
+        if parsed_args.grade:
+            debug_mode = False
+            # TODO determine if we are in an interactive terminal and set interactive accordingly
+            # set interactive to False for now
+            interactive = False
+        else:
+            try:
+                console.print("Press [cyan]Enter[/cyan] now to continue")
+                input()
+            except EOFError:
+                interactive = False
+                debug_mode = False
+
+        if interactive and debug_mode:  # if debug mode was set to False, then the --grade option must have been specified
+            console.print(
+                """Which of the following modes do you want to run in?
+        1) debug+grade mode (d)
+        2) grade only mode (g)
+    Type 'd' or 'g', then hit [cyan]Enter[/cyan]."""
+            )
+            mode_input = input()
+            debug_mode = mode_input == "" or mode_input[0].lower() != "g"
 
     reporter = ConsoleGraderReporter(
         section,
         console,
         sys.stdout,
         sys.stderr,
         interactive=interactive,
```

### Comparing `gradema-0.0.6/gradema/grader/console/_util.py` & `gradema-0.1.0/gradema/grader/console/_util.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.6/gradema/section/_section.py` & `gradema-0.1.0/gradema/section/_section.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.6/gradema/test/__init__.py` & `gradema-0.1.0/gradema/test/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ._test import Test, FractionalTestResult, PercentTestResult, TestResult
 from ._python import (
     create_python_test,
     create_python_pytest,
     create_python_format_check,
     create_python_format_check_from_path,
     create_python_type_check,
+    create_mypy_command,
     create_python_stdio_test,
     create_python_traditional_stdio_test,
     create_python_traditional_arg_test,
 )
 from ._dummy import dummy_test
 from ._exists import create_file_exists_test
 from ._rust import RustProgram
@@ -25,12 +26,13 @@
     "create_python_test",
     "create_python_pytest",
     "create_python_stdio_test",
     "create_python_traditional_stdio_test",
     "create_python_format_check",
     "create_python_format_check_from_path",
     "create_python_type_check",
+    "create_mypy_command",
     "dummy_test",
     "create_file_exists_test",
     "RustProgram",
     "create_python_traditional_arg_test",
 ]
```

### Comparing `gradema-0.0.6/gradema/test/_command.py` & `gradema-0.1.0/gradema/test/_command.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.6/gradema/test/_python.py` & `gradema-0.1.0/gradema/test/_python.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     return CommandTest(["python", "-m", module_name], ["pudb", "-m", module_name])
 
 
 def create_python_pytest(file_argument: str) -> Test:
     """
     Creates a pytest test.
 
-    Currently, does not have a debugging option. See source code if this function for detailed comment.
+    Currently, does not have a debugging option. See source code of this function for detailed comment.
 
     :param file_argument: The argument to pass to pytest that is the file and optionally has a ``::test_function_name`` tacked on at the end
     :return: A pytest test
     """
     # TODO add a debug command to pytest
     """
     So... I (Lavender Shannon) spent a couple of hours trying to figure out how to use pudb and pytest together.
@@ -87,7 +87,11 @@
 
 def create_python_format_check() -> Test:
     return create_python_format_check_from_path(".")
 
 
 def create_python_type_check() -> Test:
     return CommandTest(["mypy", "--strict", "--disallow-any-explicit", "."])
+
+
+def create_mypy_command(arguments: Sequence[str]) -> Test:
+    return CommandTest(["mypy", *arguments])
```

### Comparing `gradema-0.0.6/gradema/test/_reporter.py` & `gradema-0.1.0/gradema/test/_reporter.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.6/gradema/test/_rust.py` & `gradema-0.1.0/gradema/test/_rust.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.6/gradema/test/_stdio.py` & `gradema-0.1.0/gradema/test/_stdio.py`

 * *Files identical despite different names*

### Comparing `gradema-0.0.6/pyproject.toml` & `gradema-0.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,32 @@
 [tool.poetry]
 name = "gradema"
-version = "0.0.6"
+version = "0.1.0"
 description = "The utility you need to easily configure auto-grading"
-authors = ["Lavender Shannon <jdsfz4@mst.edu>"]
+authors = ["Lavender Shannon <retrodaredevil@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://gradema.readthedocs.io"
-repository = "https://git.mst.edu/gradema/gradema"
+repository = "https://gitlab.com/classroomcode/gradema/gradema"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 rich = "13.7.1"
-pudb = "^2024.1"
-mypy = "^1.10.0"
 editorconfig = "^0.12.4"
 python-magic = "^0.4.27"
-py2cfg = "^0.7.3"
+# We choose to not include mypy, pudb, pytest, or black here
+#   because those should be explicitly dependeded on in the assignment repository
 
 [tool.poetry.group.dev.dependencies]
+mypy = "^1.10.0"
+pudb = "^2024.1"
 pytest = "8.1.1"
 black = "^24.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+# https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-format
+line-length = 180
```

