# Comparing `tmp/subprocess_shell-0.1.0.tar.gz` & `tmp/subprocess_shell-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subprocess_shell-0.1.0.tar", last modified: Sun Mar  3 21:04:21 2024, max compression
+gzip compressed data, was "subprocess_shell-1.0.0.tar", last modified: Thu May  9 08:39:06 2024, max compression
```

## Comparing `subprocess_shell-0.1.0.tar` & `subprocess_shell-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-03-03 21:04:21.000000 subprocess_shell-0.1.0/
--rw-r--r--   0 arappold  (1000) arappold  (1000)     1072 2023-10-10 12:57:53.000000 subprocess_shell-0.1.0/LICENSE
--rw-r--r--   0 arappold  (1000) arappold  (1000)    20091 2024-03-03 21:04:21.000000 subprocess_shell-0.1.0/PKG-INFO
--rw-r--r--   0 arappold  (1000) arappold  (1000)    18211 2024-03-03 20:52:15.000000 subprocess_shell-0.1.0/README.md
--rw-r--r--   0 arappold  (1000) arappold  (1000)      583 2024-03-03 20:58:47.000000 subprocess_shell-0.1.0/pyproject.toml
--rw-r--r--   0 arappold  (1000) arappold  (1000)       38 2024-03-03 21:04:21.000000 subprocess_shell-0.1.0/setup.cfg
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-03-03 21:04:21.000000 subprocess_shell-0.1.0/src/
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-03-03 21:04:21.000000 subprocess_shell-0.1.0/src/subprocess_shell/
--rw-r--r--   0 arappold  (1000) arappold  (1000)    34410 2024-03-03 21:04:05.000000 subprocess_shell-0.1.0/src/subprocess_shell/__init__.py
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-03-03 21:04:21.000000 subprocess_shell-0.1.0/src/subprocess_shell.egg-info/
--rw-r--r--   0 arappold  (1000) arappold  (1000)    20091 2024-03-03 21:04:21.000000 subprocess_shell-0.1.0/src/subprocess_shell.egg-info/PKG-INFO
--rw-r--r--   0 arappold  (1000) arappold  (1000)      315 2024-03-03 21:04:21.000000 subprocess_shell-0.1.0/src/subprocess_shell.egg-info/SOURCES.txt
--rw-r--r--   0 arappold  (1000) arappold  (1000)        1 2024-03-03 21:04:21.000000 subprocess_shell-0.1.0/src/subprocess_shell.egg-info/dependency_links.txt
--rw-r--r--   0 arappold  (1000) arappold  (1000)       62 2024-03-03 21:04:21.000000 subprocess_shell-0.1.0/src/subprocess_shell.egg-info/requires.txt
--rw-r--r--   0 arappold  (1000) arappold  (1000)       17 2024-03-03 21:04:21.000000 subprocess_shell-0.1.0/src/subprocess_shell.egg-info/top_level.txt
-drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-03-03 21:04:21.000000 subprocess_shell-0.1.0/tests/
--rw-r--r--   0 arappold  (1000) arappold  (1000)    14509 2024-03-03 21:04:05.000000 subprocess_shell-0.1.0/tests/test_subprocess_shell.py
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/
+-rw-r--r--   0 arappold  (1000) arappold  (1000)     1072 2023-10-10 12:57:53.000000 subprocess_shell-1.0.0/LICENSE
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    20496 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/PKG-INFO
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    18616 2024-05-09 08:30:58.000000 subprocess_shell-1.0.0/README.md
+-rw-r--r--   0 arappold  (1000) arappold  (1000)      583 2024-05-09 07:46:38.000000 subprocess_shell-1.0.0/pyproject.toml
+-rw-r--r--   0 arappold  (1000) arappold  (1000)       38 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/setup.cfg
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell/
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    35431 2024-05-09 08:07:02.000000 subprocess_shell-1.0.0/src/subprocess_shell/__init__.py
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell.egg-info/
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    20496 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell.egg-info/PKG-INFO
+-rw-r--r--   0 arappold  (1000) arappold  (1000)      315 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 arappold  (1000) arappold  (1000)        1 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 arappold  (1000) arappold  (1000)       62 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell.egg-info/requires.txt
+-rw-r--r--   0 arappold  (1000) arappold  (1000)       17 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/src/subprocess_shell.egg-info/top_level.txt
+drwxr-xr-x   0 arappold  (1000) arappold  (1000)        0 2024-05-09 08:39:06.000000 subprocess_shell-1.0.0/tests/
+-rw-r--r--   0 arappold  (1000) arappold  (1000)    14509 2024-03-03 21:04:05.000000 subprocess_shell-1.0.0/tests/test_subprocess_shell.py
```

### Comparing `subprocess_shell-0.1.0/LICENSE` & `subprocess_shell-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `subprocess_shell-0.1.0/PKG-INFO` & `subprocess_shell-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subprocess_shell
-Version: 0.1.0
+Version: 1.0.0
 Summary: A shell for subprocess
 Author-email: Andreas Rappold <not_evil@rappold1.at>
 License: MIT License
         
         Copyright (c) 2023 Andreas Rappold
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,15 +42,15 @@
 
 is a Python package providing an alternative interface to sub processes. The aim is simplicity comparable to shell scripting and transparency for more complex use cases.
 
 [[_TOC_]]
 
 ![`videos/aperitif.mp4`](videos/aperitif.mp4)
 
-**Update:** the showcase presents an earlier version which didn't provide `run`
+**Update:** the showcase presents an earlier version which didn't provide `run()` and `wait(logs=...)`
 
 ## Features
 
 - Simple
     - e.g. 5 functions (`start`, `write`, `wait`, `read`, `run`) and 3 operators (`>>`, `+`, `-`)
 - Transparent
     - usability layer for [*subprocess*](https://docs.python.org/3/library/subprocess.html) except streams
@@ -423,15 +423,15 @@
 process = arguments >> start(
     stdin=subprocess.PIPE,
     stdout=subprocess.PIPE,
     pass_stdout=False,
     stderr=subprocess.PIPE,
     pass_stderr=False,
     queue_size=0,
-    logs=False,
+    logs=None,
     return_codes=(0,),
     force_color=True,
     async_=False,
     **{},
 )
 ```
 
@@ -658,33 +658,29 @@
       <td>
 
 `logs`
 
 </td>
       <td>
 
-`False`
+`None`
 
 </td>
       <td>
 
-if in a chain: analog of `wait(logs=False)`
+if in a chain: analog of `wait(logs=None)`
 
 </td>
     </tr>
     <tr>
       <td></td>
+      <td>boolean</td>
       <td>
 
-`True`
-
-</td>
-      <td>
-
-if in a chain: analog of `wait(logs=True)`
+if in a chain: analog of `wait(logs=False)` or `wait(logs=True)`
 
 </td>
     </tr>
     <tr>
       <td>
 
 `return_codes`
@@ -693,41 +689,28 @@
       <td>
 
 `(0,)`
 
 </td>
       <td>
 
-if in a chain: analog of `wait(return_code=(0,))`
+if in a chain: analog of `wait(return_codes=(0,))`
 
 </td>
     </tr>
     <tr>
       <td></td>
       <td>
 
-collection `object`
+collection `object` or `None`
 
 </td>
       <td>
 
-if in a chain: analog of `wait(return_code=object)`
-
-</td>
-    </tr>
-    <tr>
-      <td></td>
-      <td>
-
-`None`
-
-</td>
-      <td>
-
-if in a chain: analog of `wait(return_code=None)`
+if in a chain: analog of `wait(return_codes=object)` or `wait(return_codes=None)`
 
 </td>
     </tr>
     <tr>
       <td>
 
 `force_color`
@@ -857,20 +840,20 @@
 
 ### Wait for process
 
 ```python
 return_code = process >> wait(
     stdout=True,
     stderr=True,
-    logs=False,
+    logs=None,
     return_codes=(0,),
     rich=True,
-    stdout_color="green",
-    stderr_color="red",
-    log_color="dark_orange3",
+    stdout_style="green",
+    log_style="dark_orange3",
+    error_style="red",
     ascii=False,
 )
 ```
 
 <table>
   <tbody>
     <tr>
@@ -955,45 +938,74 @@
       <td>
 
 `logs`
 
 </td>
       <td>
 
+`None`
+
+</td>
+      <td>
+
+write stdout first and use `log_style` for stderr if the return code assert succeeds or `error_style` otherwise
+
+</td>
+    </tr>
+    <tr>
+      <td></td>
+      <td>
+
 `False`
 
 </td>
-      <td>write stdout first</td>
+      <td>
+
+write stdout first and use `error_style` for stderr
+
+</td>
     </tr>
     <tr>
       <td></td>
       <td>
 
 `True`
 
 </td>
-      <td>write stderr first</td>
+      <td>
+
+write stderr first and use `log_style`
+
+</td>
     </tr>
     <tr>
       <td>
 
 `return_codes`
 
 </td>
       <td>
 
 `(0,)`
 
 </td>
-      <td>assert the return code is 0</td>
+      <td>assert that the return code is 0</td>
     </tr>
     <tr>
       <td></td>
-      <td>collection</td>
-      <td>assert the return code is in the collection</td>
+      <td>
+
+collection `object`
+
+</td>
+      <td>
+
+assert that the return code is in `object`
+
+</td>
     </tr>
     <tr>
       <td></td>
       <td>
 
 `None`
 
@@ -1029,74 +1041,82 @@
 don't use *Rich*
 
 </td>
     </tr>
     <tr>
       <td>
 
-`stdout_color`
+`stdout_style`
 
 </td>
       <td>
 
 `"green"`
 
 </td>
-      <td>use green for stdout frame</td>
+      <td>use color "green" for stdout frame</td>
     </tr>
     <tr>
       <td></td>
-      <td>else</td>
+      <td>style object or string</td>
       <td>
 
-see [Standard Colors](https://rich.readthedocs.io/en/stable/appendix/colors.html)
+use style for stdout frame, see [Styles](https://rich.readthedocs.io/en/stable/style.html)
 
 </td>
     </tr>
     <tr>
       <td>
 
-`stderr_color`
+`log_style`
 
 </td>
       <td>
 
-`"red"`
+`"dark_orange3"`
+
+</td>
+      <td>
+
+use color "dark_orange3" for stderr frame, see argument `logs`
 
 </td>
-      <td>use red for stderr frame</td>
     </tr>
     <tr>
       <td></td>
-      <td>else</td>
+      <td>style object or string</td>
       <td>
 
-see [Standard Colors](https://rich.readthedocs.io/en/stable/appendix/colors.html)
+use style for stderr frame, see argument `logs` and [Styles](https://rich.readthedocs.io/en/stable/style.html)
 
 </td>
     </tr>
     <tr>
       <td>
 
-`log_color`
+`error_style`
 
 </td>
       <td>
 
-`"dark_orange3"`
+`"red"`
+
+</td>
+      <td>
+
+use color "red" for stderr frame, see argument `logs`
 
 </td>
-      <td>if logs: use "dark_orange3" for stderr frame</td>
     </tr>
     <tr>
       <td></td>
-      <td>else</td>
+      <td>style object or string</td>
       <td>
 
-see [Standard Colors](https://rich.readthedocs.io/en/stable/appendix/colors.html)
+use style for stderr frame, see argument `logs` and [Styles](https://rich.readthedocs.io/en/stable/style.html)
 
 </td>
     </tr>
     <tr>
       <td>
 
 `ascii`
```

### Comparing `subprocess_shell-0.1.0/README.md` & `subprocess_shell-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 is a Python package providing an alternative interface to sub processes. The aim is simplicity comparable to shell scripting and transparency for more complex use cases.
 
 [[_TOC_]]
 
 ![`videos/aperitif.mp4`](videos/aperitif.mp4)
 
-**Update:** the showcase presents an earlier version which didn't provide `run`
+**Update:** the showcase presents an earlier version which didn't provide `run()` and `wait(logs=...)`
 
 ## Features
 
 - Simple
     - e.g. 5 functions (`start`, `write`, `wait`, `read`, `run`) and 3 operators (`>>`, `+`, `-`)
 - Transparent
     - usability layer for [*subprocess*](https://docs.python.org/3/library/subprocess.html) except streams
@@ -383,15 +383,15 @@
 process = arguments >> start(
     stdin=subprocess.PIPE,
     stdout=subprocess.PIPE,
     pass_stdout=False,
     stderr=subprocess.PIPE,
     pass_stderr=False,
     queue_size=0,
-    logs=False,
+    logs=None,
     return_codes=(0,),
     force_color=True,
     async_=False,
     **{},
 )
 ```
 
@@ -618,33 +618,29 @@
       <td>
 
 `logs`
 
 </td>
       <td>
 
-`False`
+`None`
 
 </td>
       <td>
 
-if in a chain: analog of `wait(logs=False)`
+if in a chain: analog of `wait(logs=None)`
 
 </td>
     </tr>
     <tr>
       <td></td>
+      <td>boolean</td>
       <td>
 
-`True`
-
-</td>
-      <td>
-
-if in a chain: analog of `wait(logs=True)`
+if in a chain: analog of `wait(logs=False)` or `wait(logs=True)`
 
 </td>
     </tr>
     <tr>
       <td>
 
 `return_codes`
@@ -653,41 +649,28 @@
       <td>
 
 `(0,)`
 
 </td>
       <td>
 
-if in a chain: analog of `wait(return_code=(0,))`
+if in a chain: analog of `wait(return_codes=(0,))`
 
 </td>
     </tr>
     <tr>
       <td></td>
       <td>
 
-collection `object`
+collection `object` or `None`
 
 </td>
       <td>
 
-if in a chain: analog of `wait(return_code=object)`
-
-</td>
-    </tr>
-    <tr>
-      <td></td>
-      <td>
-
-`None`
-
-</td>
-      <td>
-
-if in a chain: analog of `wait(return_code=None)`
+if in a chain: analog of `wait(return_codes=object)` or `wait(return_codes=None)`
 
 </td>
     </tr>
     <tr>
       <td>
 
 `force_color`
@@ -817,20 +800,20 @@
 
 ### Wait for process
 
 ```python
 return_code = process >> wait(
     stdout=True,
     stderr=True,
-    logs=False,
+    logs=None,
     return_codes=(0,),
     rich=True,
-    stdout_color="green",
-    stderr_color="red",
-    log_color="dark_orange3",
+    stdout_style="green",
+    log_style="dark_orange3",
+    error_style="red",
     ascii=False,
 )
 ```
 
 <table>
   <tbody>
     <tr>
@@ -915,45 +898,74 @@
       <td>
 
 `logs`
 
 </td>
       <td>
 
+`None`
+
+</td>
+      <td>
+
+write stdout first and use `log_style` for stderr if the return code assert succeeds or `error_style` otherwise
+
+</td>
+    </tr>
+    <tr>
+      <td></td>
+      <td>
+
 `False`
 
 </td>
-      <td>write stdout first</td>
+      <td>
+
+write stdout first and use `error_style` for stderr
+
+</td>
     </tr>
     <tr>
       <td></td>
       <td>
 
 `True`
 
 </td>
-      <td>write stderr first</td>
+      <td>
+
+write stderr first and use `log_style`
+
+</td>
     </tr>
     <tr>
       <td>
 
 `return_codes`
 
 </td>
       <td>
 
 `(0,)`
 
 </td>
-      <td>assert the return code is 0</td>
+      <td>assert that the return code is 0</td>
     </tr>
     <tr>
       <td></td>
-      <td>collection</td>
-      <td>assert the return code is in the collection</td>
+      <td>
+
+collection `object`
+
+</td>
+      <td>
+
+assert that the return code is in `object`
+
+</td>
     </tr>
     <tr>
       <td></td>
       <td>
 
 `None`
 
@@ -989,74 +1001,82 @@
 don't use *Rich*
 
 </td>
     </tr>
     <tr>
       <td>
 
-`stdout_color`
+`stdout_style`
 
 </td>
       <td>
 
 `"green"`
 
 </td>
-      <td>use green for stdout frame</td>
+      <td>use color "green" for stdout frame</td>
     </tr>
     <tr>
       <td></td>
-      <td>else</td>
+      <td>style object or string</td>
       <td>
 
-see [Standard Colors](https://rich.readthedocs.io/en/stable/appendix/colors.html)
+use style for stdout frame, see [Styles](https://rich.readthedocs.io/en/stable/style.html)
 
 </td>
     </tr>
     <tr>
       <td>
 
-`stderr_color`
+`log_style`
 
 </td>
       <td>
 
-`"red"`
+`"dark_orange3"`
+
+</td>
+      <td>
+
+use color "dark_orange3" for stderr frame, see argument `logs`
 
 </td>
-      <td>use red for stderr frame</td>
     </tr>
     <tr>
       <td></td>
-      <td>else</td>
+      <td>style object or string</td>
       <td>
 
-see [Standard Colors](https://rich.readthedocs.io/en/stable/appendix/colors.html)
+use style for stderr frame, see argument `logs` and [Styles](https://rich.readthedocs.io/en/stable/style.html)
 
 </td>
     </tr>
     <tr>
       <td>
 
-`log_color`
+`error_style`
 
 </td>
       <td>
 
-`"dark_orange3"`
+`"red"`
+
+</td>
+      <td>
+
+use color "red" for stderr frame, see argument `logs`
 
 </td>
-      <td>if logs: use "dark_orange3" for stderr frame</td>
     </tr>
     <tr>
       <td></td>
-      <td>else</td>
+      <td>style object or string</td>
       <td>
 
-see [Standard Colors](https://rich.readthedocs.io/en/stable/appendix/colors.html)
+use style for stderr frame, see argument `logs` and [Styles](https://rich.readthedocs.io/en/stable/style.html)
 
 </td>
     </tr>
     <tr>
       <td>
 
 `ascii`
```

### Comparing `subprocess_shell-0.1.0/src/subprocess_shell/__init__.py` & `subprocess_shell-1.0.0/src/subprocess_shell/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,21 @@
 import selectors
 import subprocess
 import sys
 import threading
 import types
 import typing
 
+if typing.TYPE_CHECKING:
+    try:
+        import rich.style
+
+    except ImportError:
+        pass
+
 
 __all__ = ("start", "write", "wait", "read", "run")
 
 
 def _or(first_dictionary, second_dictionary):
     dictionary = dict(first_dictionary)
     dictionary.update(second_dictionary)
@@ -83,15 +90,15 @@
             typing.IO,
             str,
             pathlib.Path,
             typing.Callable[[typing.AnyStr], typing.Any],
         ] = subprocess.PIPE,
         pass_stderr: bool = False,
         queue_size: int = 0,
-        logs: bool = False,
+        logs: typing.Union[bool, None] = None,
         return_codes: typing.Union[typing.Container[int], None] = (0,),
         force_color: bool = True,
         async_: bool = False,
         **kwargs,
     ):
         """
         `{arguments} >> start(...)` starts a sub process similar to `subprocess.Popen({arguments}, ...)` and returns a process object
@@ -121,16 +128,16 @@
                 called in a different thread
                 **!! must not raise exceptions !!**
         pass_stderr : bool
             Don't touch stderr
         queue_size : int
             Limit size of queues
             *! may lead to deadlocks !*
-        logs : bool
-            Write stderr first if in a chain
+        logs : bool | None
+            Analog of `write(logs=logs)` if in a chain
         return_codes : container[int] | None
             Used to validate the return code if in a chain
         force_color : bool
             Set environment variable FORCE_COLOR to 1 if not set
         async_ : bool
             Use `asyncio` instead of `selectors`
         **kwargs
@@ -570,16 +577,15 @@
     def __str__(self):
         if not self._async:
             self._process.poll()
 
         _v_ = self._process.returncode is None
         code_string = "running" if _v_ else f"returned {self._process.returncode}"
 
-        _v_ = subprocess.list2cmdline(typing.cast(typing.Iterable, self._arguments))
-        return f"{self._start_datetime} `{_v_}` {code_string}"
+        return f"{self._start_datetime} `{subprocess.list2cmdline(typing.cast(typing.Iterable, self._arguments))}` {code_string}"
 
 
 class _Pass:
     def __init__(self, process, stderr, arguments):
         super().__init__()
 
         self.process = process
@@ -702,53 +708,61 @@
 
 
 class _Wait:
     def __init__(
         self,
         stdout: typing.Union[bool, typing.TextIO] = True,
         stderr: typing.Union[bool, typing.TextIO] = True,
-        logs: bool = False,
+        logs: typing.Union[bool, None] = None,
         return_codes: typing.Union[typing.Container[int], None] = (0,),
         rich: bool = True,
-        stdout_color: str = "green",
-        stderr_color: str = "red",
-        log_color: str = "dark_orange3",
+        stdout_style: typing.Union["rich.style.Style", str] = "green",
+        log_style: typing.Union["rich.style.Style", str] = "dark_orange3",
+        error_style: typing.Union["rich.style.Style", str] = "red",
         ascii: bool = False,
     ):
         """
         `{process} >> wait(...)` "waits for" the source process, writes stdout and stderr as separate frames and validates and returns the return code
 
         Parameters
         ----------
         stdout : bool | TextIO
             if   bool : optionally write stdout to `sys.stdout`
             if TextIO : write stdout to writable object
         stderr : bool | TextIO
             if   bool : optionally write stderr to `sys.stderr`
             if TextIO : write stderr to writable object
-        logs : bool
-            Write stderr first
+        logs : bool | None
+            if False : write stdout first and use `error_style` for stderr
+                True : write stderr first and use `log_style`
+                None : write stdout first and use `log_style` for stderr if return code assert succeeds or `error_style` otherwise
         return_codes : container[int]
             Used to validate the return code
         rich : bool
             Use *Rich* if available
+        stdout_style : rich.style.Style | str
+            Used for stdout frame
+        log_style : rich.style.Style | str
+            Used for stderr frame, see `logs`
+        error_style : rich.style.Style | str
+            Used for stderr frame, see `logs`
         ascii : bool
             Use ASCII instead of Unicode
         """
 
         super().__init__()
 
         self.stdout = stdout
         self.stderr = stderr
         self.logs = logs
         self.return_codes = return_codes
         self.rich = rich
-        self.stdout_color = stdout_color
-        self.stderr_color = stderr_color
-        self.log_color = log_color
+        self.stdout_style = stdout_style
+        self.log_style = log_style
+        self.error_style = error_style
         self.ascii = ascii
 
         self._r_console = None
         self._r_highlighter = None
         self._r_theme = None
         if rich:
             try:
@@ -781,44 +795,52 @@
 
         process._close_stdin()
 
         def _print_stdout():
             _v_ = process._stdout_queue is None or process.start.pass_stdout
             if not (_v_ or self.stdout is False):
                 _v_ = sys.stdout if self.stdout is True else self.stdout
-                self._print_stream(process.get_stdout_strings(), _v_, False, process)
+                self._print_stream(
+                    process.get_stdout_strings(), _v_, False, False, process
+                )
 
-        def _print_stderr():
+        def _print_stderr(log):
             _v_ = process._stderr_queue is None or process.start.pass_stderr
             if not (_v_ or self.stderr is False):
                 _v_ = sys.stderr if self.stderr is True else self.stderr
-                self._print_stream(process.get_stderr_strings(), _v_, True, process)
+                self._print_stream(
+                    process.get_stderr_strings(), _v_, True, log, process
+                )
 
-        if self.logs:
-            _print_stderr()
+        if self.logs is True:
+            _print_stderr(True)
             _print_stdout()
+            return_code = process._wait()
 
         else:
             _print_stdout()
-            _print_stderr()
+            return_code = process._wait()
 
-        return_code = process._wait()
+            _v_ = self.logs is None and not (
+                self.return_codes is not None and return_code not in self.return_codes
+            )
+            _print_stderr(_v_)
 
         if isinstance(process.start.stdout, (str, pathlib.Path)):
             typing.cast(typing.IO, process._stdout).close()
 
         if isinstance(process.start.stderr, (str, pathlib.Path)):
             typing.cast(typing.IO, process._stderr).close()
 
         if self.return_codes is not None and return_code not in self.return_codes:
             raise ProcessFailedError(process)
 
         return return_code
 
-    def _print_stream(self, strings, file, is_stderr, process):
+    def _print_stream(self, strings, file, is_stderr, log, process):
         strings = iter(strings)
 
         string = next(strings, None)
         if string is None:
             return
 
         newline_string = (
@@ -838,22 +860,22 @@
 
             class _Highlighter(_v_):
                 base_style = "m."
 
                 _v_ = f"(?P<p1>{re.escape(newline_string)})"
                 highlights = [r"^(?P<p1>[^`]*`).*(?P<p2>` (running|returned ))", _v_]
 
-            color_name = (
-                (self.log_color if self.logs else self.stderr_color)
+            style = (
+                (self.log_style if log else self.error_style)
                 if is_stderr
-                else self.stdout_color
+                else self.stdout_style
             )
 
             _v_ = typing.cast(types.ModuleType, self._r_theme)
-            _v_ = _v_.Theme({"m.p1": color_name, "m.p2": color_name})
+            _v_ = _v_.Theme({"m.p1": style, "m.p2": style})
             console = typing.cast(types.ModuleType, self._r_console).Console(
                 file=file, soft_wrap=True, highlighter=_Highlighter(), theme=_v_
             )
 
             def _print(*args, **kwargs):
                 console.out(*args, **kwargs)
                 file.flush()
```

### Comparing `subprocess_shell-0.1.0/src/subprocess_shell.egg-info/PKG-INFO` & `subprocess_shell-1.0.0/src/subprocess_shell.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subprocess_shell
-Version: 0.1.0
+Version: 1.0.0
 Summary: A shell for subprocess
 Author-email: Andreas Rappold <not_evil@rappold1.at>
 License: MIT License
         
         Copyright (c) 2023 Andreas Rappold
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,15 +42,15 @@
 
 is a Python package providing an alternative interface to sub processes. The aim is simplicity comparable to shell scripting and transparency for more complex use cases.
 
 [[_TOC_]]
 
 ![`videos/aperitif.mp4`](videos/aperitif.mp4)
 
-**Update:** the showcase presents an earlier version which didn't provide `run`
+**Update:** the showcase presents an earlier version which didn't provide `run()` and `wait(logs=...)`
 
 ## Features
 
 - Simple
     - e.g. 5 functions (`start`, `write`, `wait`, `read`, `run`) and 3 operators (`>>`, `+`, `-`)
 - Transparent
     - usability layer for [*subprocess*](https://docs.python.org/3/library/subprocess.html) except streams
@@ -423,15 +423,15 @@
 process = arguments >> start(
     stdin=subprocess.PIPE,
     stdout=subprocess.PIPE,
     pass_stdout=False,
     stderr=subprocess.PIPE,
     pass_stderr=False,
     queue_size=0,
-    logs=False,
+    logs=None,
     return_codes=(0,),
     force_color=True,
     async_=False,
     **{},
 )
 ```
 
@@ -658,33 +658,29 @@
       <td>
 
 `logs`
 
 </td>
       <td>
 
-`False`
+`None`
 
 </td>
       <td>
 
-if in a chain: analog of `wait(logs=False)`
+if in a chain: analog of `wait(logs=None)`
 
 </td>
     </tr>
     <tr>
       <td></td>
+      <td>boolean</td>
       <td>
 
-`True`
-
-</td>
-      <td>
-
-if in a chain: analog of `wait(logs=True)`
+if in a chain: analog of `wait(logs=False)` or `wait(logs=True)`
 
 </td>
     </tr>
     <tr>
       <td>
 
 `return_codes`
@@ -693,41 +689,28 @@
       <td>
 
 `(0,)`
 
 </td>
       <td>
 
-if in a chain: analog of `wait(return_code=(0,))`
+if in a chain: analog of `wait(return_codes=(0,))`
 
 </td>
     </tr>
     <tr>
       <td></td>
       <td>
 
-collection `object`
+collection `object` or `None`
 
 </td>
       <td>
 
-if in a chain: analog of `wait(return_code=object)`
-
-</td>
-    </tr>
-    <tr>
-      <td></td>
-      <td>
-
-`None`
-
-</td>
-      <td>
-
-if in a chain: analog of `wait(return_code=None)`
+if in a chain: analog of `wait(return_codes=object)` or `wait(return_codes=None)`
 
 </td>
     </tr>
     <tr>
       <td>
 
 `force_color`
@@ -857,20 +840,20 @@
 
 ### Wait for process
 
 ```python
 return_code = process >> wait(
     stdout=True,
     stderr=True,
-    logs=False,
+    logs=None,
     return_codes=(0,),
     rich=True,
-    stdout_color="green",
-    stderr_color="red",
-    log_color="dark_orange3",
+    stdout_style="green",
+    log_style="dark_orange3",
+    error_style="red",
     ascii=False,
 )
 ```
 
 <table>
   <tbody>
     <tr>
@@ -955,45 +938,74 @@
       <td>
 
 `logs`
 
 </td>
       <td>
 
+`None`
+
+</td>
+      <td>
+
+write stdout first and use `log_style` for stderr if the return code assert succeeds or `error_style` otherwise
+
+</td>
+    </tr>
+    <tr>
+      <td></td>
+      <td>
+
 `False`
 
 </td>
-      <td>write stdout first</td>
+      <td>
+
+write stdout first and use `error_style` for stderr
+
+</td>
     </tr>
     <tr>
       <td></td>
       <td>
 
 `True`
 
 </td>
-      <td>write stderr first</td>
+      <td>
+
+write stderr first and use `log_style`
+
+</td>
     </tr>
     <tr>
       <td>
 
 `return_codes`
 
 </td>
       <td>
 
 `(0,)`
 
 </td>
-      <td>assert the return code is 0</td>
+      <td>assert that the return code is 0</td>
     </tr>
     <tr>
       <td></td>
-      <td>collection</td>
-      <td>assert the return code is in the collection</td>
+      <td>
+
+collection `object`
+
+</td>
+      <td>
+
+assert that the return code is in `object`
+
+</td>
     </tr>
     <tr>
       <td></td>
       <td>
 
 `None`
 
@@ -1029,74 +1041,82 @@
 don't use *Rich*
 
 </td>
     </tr>
     <tr>
       <td>
 
-`stdout_color`
+`stdout_style`
 
 </td>
       <td>
 
 `"green"`
 
 </td>
-      <td>use green for stdout frame</td>
+      <td>use color "green" for stdout frame</td>
     </tr>
     <tr>
       <td></td>
-      <td>else</td>
+      <td>style object or string</td>
       <td>
 
-see [Standard Colors](https://rich.readthedocs.io/en/stable/appendix/colors.html)
+use style for stdout frame, see [Styles](https://rich.readthedocs.io/en/stable/style.html)
 
 </td>
     </tr>
     <tr>
       <td>
 
-`stderr_color`
+`log_style`
 
 </td>
       <td>
 
-`"red"`
+`"dark_orange3"`
+
+</td>
+      <td>
+
+use color "dark_orange3" for stderr frame, see argument `logs`
 
 </td>
-      <td>use red for stderr frame</td>
     </tr>
     <tr>
       <td></td>
-      <td>else</td>
+      <td>style object or string</td>
       <td>
 
-see [Standard Colors](https://rich.readthedocs.io/en/stable/appendix/colors.html)
+use style for stderr frame, see argument `logs` and [Styles](https://rich.readthedocs.io/en/stable/style.html)
 
 </td>
     </tr>
     <tr>
       <td>
 
-`log_color`
+`error_style`
 
 </td>
       <td>
 
-`"dark_orange3"`
+`"red"`
+
+</td>
+      <td>
+
+use color "red" for stderr frame, see argument `logs`
 
 </td>
-      <td>if logs: use "dark_orange3" for stderr frame</td>
     </tr>
     <tr>
       <td></td>
-      <td>else</td>
+      <td>style object or string</td>
       <td>
 
-see [Standard Colors](https://rich.readthedocs.io/en/stable/appendix/colors.html)
+use style for stderr frame, see argument `logs` and [Styles](https://rich.readthedocs.io/en/stable/style.html)
 
 </td>
     </tr>
     <tr>
       <td>
 
 `ascii`
```

### Comparing `subprocess_shell-0.1.0/tests/test_subprocess_shell.py` & `subprocess_shell-1.0.0/tests/test_subprocess_shell.py`

 * *Files identical despite different names*

