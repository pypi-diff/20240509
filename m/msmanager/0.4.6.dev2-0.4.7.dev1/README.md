# Comparing `tmp/msmanager-0.4.6.dev2.tar.gz` & `tmp/msmanager-0.4.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.4.6.dev2.tar", max compression
+gzip compressed data, was "msmanager-0.4.7.dev1.tar", max compression
```

## Comparing `msmanager-0.4.6.dev2.tar` & `msmanager-0.4.7.dev1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1081 2024-01-04 00:20:05.740172 msmanager-0.4.6.dev2/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.4.6.dev2/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.4.6.dev2/msmanager/__main__.py
--rw-r--r--   0        0        0    15407 2024-05-06 13:31:06.653571 msmanager-0.4.6.dev2/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.4.6.dev2/msmanager/config.py
--rw-r--r--   0        0        0     3307 2024-05-06 07:43:04.185624 msmanager-0.4.6.dev2/msmanager/exceptions.py
--rw-r--r--   0        0        0     4190 2024-05-06 13:11:57.556601 msmanager-0.4.6.dev2/msmanager/functions.py
--rw-r--r--   0        0        0      562 2024-05-06 12:56:09.812783 msmanager-0.4.6.dev2/msmanager/models.py
--rw-r--r--   0        0        0     3232 2024-05-06 12:57:54.532626 msmanager-0.4.6.dev2/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.4.6.dev2/msmanager/types.py
--rw-r--r--   0        0        0      601 2024-05-06 13:31:15.774560 msmanager-0.4.6.dev2/msmanager/units.py
--rw-r--r--   0        0        0      667 2024-05-06 13:31:19.417718 msmanager-0.4.6.dev2/pyproject.toml
--rw-r--r--   0        0        0      928 2024-05-06 09:35:49.035878 msmanager-0.4.6.dev2/README.md
--rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 msmanager-0.4.6.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-01-04 00:20:05.740172 msmanager-0.4.7.dev1/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.4.7.dev1/msmanager/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.4.7.dev1/msmanager/__main__.py
+-rw-r--r--   0        0        0    17036 2024-05-09 14:12:51.352876 msmanager-0.4.7.dev1/msmanager/cli.py
+-rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.4.7.dev1/msmanager/config.py
+-rw-r--r--   0        0        0     3307 2024-05-06 07:43:04.185624 msmanager-0.4.7.dev1/msmanager/exceptions.py
+-rw-r--r--   0        0        0     4179 2024-05-09 13:35:11.911231 msmanager-0.4.7.dev1/msmanager/functions.py
+-rw-r--r--   0        0        0      562 2024-05-06 12:56:09.812783 msmanager-0.4.7.dev1/msmanager/models.py
+-rw-r--r--   0        0        0     3232 2024-05-09 10:25:09.248623 msmanager-0.4.7.dev1/msmanager/msm.py
+-rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.4.7.dev1/msmanager/types.py
+-rw-r--r--   0        0        0      727 2024-05-09 14:13:30.505395 msmanager-0.4.7.dev1/msmanager/units.py
+-rw-r--r--   0        0        0      667 2024-05-09 14:13:34.300461 msmanager-0.4.7.dev1/pyproject.toml
+-rw-r--r--   0        0        0      928 2024-05-06 09:35:49.035878 msmanager-0.4.7.dev1/README.md
+-rw-r--r--   0        0        0     1757 1970-01-01 00:00:00.000000 msmanager-0.4.7.dev1/PKG-INFO
```

### Comparing `msmanager-0.4.6.dev2/LICENSE` & `msmanager-0.4.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev2/msmanager/cli.py` & `msmanager-0.4.7.dev1/msmanager/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,70 @@
 import os
 import time
 import json
 import click
+import datetime
 from rich.console import Console
 from typing import Literal, Optional, Union, Iterable, Callable, List, Dict, Any
 # > Local Imports
 from .msm import MSManager
 from .units import (
     __title__ as prog_name,
-    __version__ as prog_version
+    __version__ as prog_version,
+    ERRORLOG_DIRPATH
 )
 from .models import (
     MindustryServerConfig,
     JsonOutput
 )
 from .functions import (
+    remove_color,
     rich_exception,
     is_server_connect_correct,
     wait_start_server,
-    ping, pingok, endicext, parse_connect_data
+    ping, pingok,
+    endicext, parse_connect_data
 )
 from .exceptions import (
-    VBMLParseError, IncorrectConnectionDataError
+    VBMLParseError, IncorrectConnectionDataError,
+    ServerIsStoppedError, ServerIsStartedError
 )
 
 # ! Vars
 console = Console()
 debug_mode = False
+verbose_mode = False
 msmanager: MSManager = ...
 oformat: Literal['text', 'json'] = 'text'
 
 # ! Functions
-def printexcept(e: Exception):
+def print_exception(e: Exception) -> None:
     if debug_mode:
         console.print_exception(word_wrap=True, show_locals=True)
     else:
         console.print(rich_exception(e))
 
+def save_print_exception() -> None:
+    cdt = datetime.datetime.now()
+    with console.capture() as cap:
+        console.print_exception(word_wrap=True, show_locals=True)
+    text = remove_color(cap.get())
+    with open(os.path.join(ERRORLOG_DIRPATH, "last.log"), "w") as logfile:
+        logfile.write(text)
+    with open(os.path.join(ERRORLOG_DIRPATH, f"{round(cdt.timestamp())}.log"), "w") as logfile:
+        logfile.write(text)
+
 def hand_exception():
     def hand_exception_wrapper(func: Callable[..., Any]):
         def hand_exception_wrapped(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except Exception as e:
                 if oformat == 'text':
-                    printexcept(e)
+                    print_exception(e)
                 elif oformat == 'json':
                     printjson(
                         JsonOutput(
                             status='error',
                             data={
                                 'name': e.__class__.__name__,
                                 'args': list(e.args),
@@ -307,28 +323,40 @@
     "--localhost", "-l", "localhost", 
     help="The ping will take place not by the host settings, but by the local IP.",
     default=False, is_flag=True
 )
 @click.option(
     "--start-delay", "-d", "start_delay",
     help="The delay before watchdog starts (in secounds).",
-    type=click.INT, default=120, show_default=True
+    type=click.INT, default=60, show_default=True
 )
 @click.option(
-    "--check-timeout", "-ct", "-t", "check_timeout",
+    "--check-timeout", "-ct", "check_timeout",
     help="The delay between process checks (in secounds).",
     type=click.INT, default=1, show_default=True
 )
 @click.option(
     "--checks", "-c", "checks",
     help="How many times to check one server.",
     type=click.INT, default=3, show_default=True
 )
+@click.option(
+    "--all-timeout", "-at", "all_timeout",
+    help="Runs a check of all servers once in a while (in secounds).",
+    type=click.INT, default=600, show_default=True
+)
 @hand_exception()
-def watchdog(scn: str, localhost: bool, start_delay: int, check_timeout: int, checks: int):
+def watchdog(
+    scn: str,
+    localhost: bool,
+    start_delay: int,
+    check_timeout: int,
+    checks: int,
+    all_timeout: int
+):
     screens_names = scn.split(",")
     servers_config: List[MindustryServerConfig] = []
     for screen_name in screens_names:
         if (server_config := msmanager.get_server_config(screen_name)) is not None:
             if (server_config.host is not None) or (server_config.port is not None):
                 servers_config.append(server_config)
                 console.print(f"[green]>[/green] The server was found in the config: {repr(screen_name)}")
@@ -339,63 +367,83 @@
     console.print(f"[green]>[/green] Waiting {start_delay} second(s) before starting the watchdog operation.")
     time.sleep(start_delay)
     console.print("[green]>[/green] Watchdog is started!")
     try:
         while True:
             for server_config in servers_config:
                 oks, server_host = 0, "localhost" if localhost else server_config.host
-                if debug_mode:
+                if verbose_mode:
                     console.print(f"[yellow]>[/yellow] Checking: {repr(server_config.screen_name)}")
                 for _ in range(checks):
                     if pingok(server_host, server_config.port):
                         oks += 1
-                        if debug_mode:
+                        if verbose_mode:
                             console.print(f"[yellow]>[/yellow] Checked: [green]ON[/green]")
                     else:
-                        if debug_mode:
+                        if verbose_mode:
                             console.print(f"[yellow]>[/yellow] Checked: [red]OFF[/red]")
                     time.sleep(check_timeout)
                 if oks == 0:
-                    console.print(f"[red]>[/red] Restarting server: {repr(server_config.screen_name)}")
-                    msmanager.restart_server(server_config.screen_name)
-                    wait_start_server(server_config.host, server_config.port, server_config.input_port)
-                    console.print(f"[green]>[/green] Restarted server: {repr(server_config.screen_name)}")
+                    ok = False
+                    while not ok:
+                        console.print(f"[red]>[/red] Attempt to restart the server: {repr(server_config.screen_name)}")
+                        try:
+                            msmanager.stop_server(server_config.screen_name)
+                        except ServerIsStoppedError:
+                            pass
+                        try:
+                            msmanager.start_server(server_config.screen_name)
+                            wait_start_server(server_config.host, server_config.port, server_config.input_port)
+                            ok = True
+                        except ServerIsStartedError:
+                            save_print_exception()
+                            ok = False
+                        if ok:
+                            console.print(f"[green]>[/green] The server has been restarted: {repr(server_config.screen_name)}")
+            time.sleep(all_timeout)
     except KeyboardInterrupt:
         pass
     console.print("[green]>[/green] Watchdog is shutdown!")
 
 # ! Main Group
 @click.group()
 @click.option(
     "--check-environment", "check_environment",
     help="Enables checks for GNU Screen, Java and system support.",
     is_flag=True, default=False
 )
+
+@click.option(
+    "--format", "-f", "output_format",
+    help="The output format.", type=click.Choice(['text', 'json']),
+    default="text", show_default=True
+)
 @click.option(
     "--debug", "-d", "debug",
     help="Enables debug mode of operation.",
-    is_flag=True
+    is_flag=True, default=False
 )
 @click.option(
-    "--format", "-f", "output_format",
-    help="The output format.", type=click.Choice(['text', 'json']),
-    default="text", show_default=True
+    "--verbose", "verbose",
+    help="Displaying more detailed logs.",
+    is_flag=True, default=False
 )
 @click.version_option(
     version=prog_version,
     prog_name=prog_name
 )
 @hand_exception()
 def main(
     check_environment: bool,
+    output_format: Literal['text', 'json'],
     debug: bool,
-    output_format: Literal['text', 'json']
+    verbose: bool
 ):
-    global msmanager, debug_mode, oformat
-    debug_mode, oformat = debug, output_format
+    global msmanager, debug_mode, oformat, verbose_mode
+    debug_mode, verbose_mode, oformat = debug, verbose, output_format
     msmanager = MSManager(check_environment=check_environment)
 
 # ! Add in Group
 main.add_command(adder)
 main.add_command(remover)
 main.add_command(starter)
 main.add_command(stoper)
```

### Comparing `msmanager-0.4.6.dev2/msmanager/config.py` & `msmanager-0.4.7.dev1/msmanager/config.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev2/msmanager/exceptions.py` & `msmanager-0.4.7.dev1/msmanager/exceptions.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev2/msmanager/functions.py` & `msmanager-0.4.7.dev1/msmanager/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import re
 import pydustry
 import platform
 from versioner import Version
 from vbml import Pattern, Patcher
 from subprocess import getstatusoutput
 from typing import Tuple, Dict, Any, Iterable, Optional
 # * Local Imports
 from .types import DefaultVersioner, DefaultVBMLPacther
-from .units import SUPPORT_PLATFORMS, COLORS_STRINGS_REPLACEBLE
+from .units import SUPPORT_PLATFORMS, COLOR_PATTERN
 from .exceptions import (
     VBMLParseError, 
     PlatformSupportError,
     ScreenNotWorkingError,
     JavaNotFound
 )
 
@@ -67,15 +68,15 @@
     return (out == 0) or (out == 1)
 
 def exists_java() -> bool:
     return runner("java", "--version")[0] == 0
 
 # ! Parse Functions
 def remove_color(text: str) -> str:
-    return replaces(text, COLORS_STRINGS_REPLACEBLE)
+    return re.sub(COLOR_PATTERN, "", text)
 
 def parse_vbml(text: str, pattern: str, *, pacther: Patcher=DefaultVBMLPacther) -> Dict[str, Any]:
     data = pacther.check(Pattern(pattern), text)
     if isinstance(data, dict):
         return data
     raise VBMLParseError()
```

### Comparing `msmanager-0.4.6.dev2/msmanager/models.py` & `msmanager-0.4.7.dev1/msmanager/models.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev2/msmanager/msm.py` & `msmanager-0.4.7.dev1/msmanager/msm.py`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev2/pyproject.toml` & `msmanager-0.4.7.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msmanager"
-version = "0.4.6.dev2"
+version = "0.4.7.dev1"
 description = "Manager for managing Mindustry servers."
 authors = ["Romanin <semina054@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "msmanager"}]
 classifiers = [
     "Operating System :: POSIX :: Linux",
```

### Comparing `msmanager-0.4.6.dev2/README.md` & `msmanager-0.4.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `msmanager-0.4.6.dev2/PKG-INFO` & `msmanager-0.4.7.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.4.6.dev2
+Version: 0.4.7.dev1
 Summary: Manager for managing Mindustry servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

