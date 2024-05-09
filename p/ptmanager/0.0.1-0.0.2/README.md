# Comparing `tmp/ptmanager-0.0.1.tar.gz` & `tmp/ptmanager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptmanager-0.0.1.tar", last modified: Thu May  9 13:47:05 2024, max compression
+gzip compressed data, was "ptmanager-0.0.2.tar", last modified: Thu May  9 19:10:13 2024, max compression
```

## Comparing `ptmanager-0.0.1.tar` & `ptmanager-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,31 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:47:05.925350 ptmanager-0.0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2024-04-29 08:46:01.000000 ptmanager-0.0.1/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3491 2024-05-09 13:47:05.925350 ptmanager-0.0.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     3034 2024-05-09 13:44:19.000000 ptmanager-0.0.1/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:47:05.925350 ptmanager-0.0.1/ptmanager/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:46:01.000000 ptmanager-0.0.1/ptmanager/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-04-29 08:46:01.000000 ptmanager-0.0.1/ptmanager/_version.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:47:05.925350 ptmanager-0.0.1/ptmanager/modules/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:46:01.000000 ptmanager-0.0.1/ptmanager/modules/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2720 2024-04-29 08:46:01.000000 ptmanager-0.0.1/ptmanager/modules/config.py
--rw-r--r--   0 kali      (1000) kali      (1000)      644 2024-04-29 08:46:01.000000 ptmanager-0.0.1/ptmanager/modules/process.py
--rw-r--r--   0 kali      (1000) kali      (1000)    13322 2024-04-29 08:46:01.000000 ptmanager-0.0.1/ptmanager/modules/process_manager.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8692 2024-05-09 13:46:13.000000 ptmanager-0.0.1/ptmanager/modules/project_manager.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6494 2024-05-09 13:46:09.000000 ptmanager-0.0.1/ptmanager/modules/tools_manager.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8302 2024-05-09 13:14:32.000000 ptmanager-0.0.1/ptmanager/ptmanager.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:47:05.925350 ptmanager-0.0.1/ptmanager.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3491 2024-05-09 13:47:05.000000 ptmanager-0.0.1/ptmanager.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      489 2024-05-09 13:47:05.000000 ptmanager-0.0.1/ptmanager.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 13:47:05.000000 ptmanager-0.0.1/ptmanager.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       55 2024-05-09 13:47:05.000000 ptmanager-0.0.1/ptmanager.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-09 13:47:05.000000 ptmanager-0.0.1/ptmanager.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       10 2024-05-09 13:47:05.000000 ptmanager-0.0.1/ptmanager.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 13:47:05.925350 ptmanager-0.0.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      934 2024-05-09 13:44:31.000000 ptmanager-0.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 19:10:13.089690 ptmanager-0.0.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2024-04-29 08:46:01.000000 ptmanager-0.0.2/LICENSE
+-rwxr-xr-x   0 kali      (1000) kali      (1000)       38 2024-05-09 13:49:22.000000 ptmanager-0.0.2/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)     3491 2024-05-09 19:10:13.089690 ptmanager-0.0.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     3034 2024-05-09 13:44:19.000000 ptmanager-0.0.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 19:10:13.089690 ptmanager-0.0.2/ptmanager/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:46:01.000000 ptmanager-0.0.2/ptmanager/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-09 13:51:04.000000 ptmanager-0.0.2/ptmanager/_version.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 19:10:13.089690 ptmanager-0.0.2/ptmanager/modules/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:46:01.000000 ptmanager-0.0.2/ptmanager/modules/__init__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 19:10:13.089690 ptmanager-0.0.2/ptmanager/modules/__pycache__/
+-rw-r--r--   0 kali      (1000) kali      (1000)      176 2024-04-29 08:46:37.000000 ptmanager-0.0.2/ptmanager/modules/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)     7250 2024-04-29 08:46:37.000000 ptmanager-0.0.2/ptmanager/modules/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)     1462 2024-04-29 08:46:37.000000 ptmanager-0.0.2/ptmanager/modules/__pycache__/process.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)    15945 2024-05-09 18:11:35.000000 ptmanager-0.0.2/ptmanager/modules/__pycache__/project_manager.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)    12358 2024-05-09 19:00:48.000000 ptmanager-0.0.2/ptmanager/modules/__pycache__/tools_manager.cpython-311.pyc
+-rw-r--r--   0 kali      (1000) kali      (1000)     2720 2024-04-29 08:46:01.000000 ptmanager-0.0.2/ptmanager/modules/config.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      644 2024-04-29 08:46:01.000000 ptmanager-0.0.2/ptmanager/modules/process.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    13322 2024-04-29 08:46:01.000000 ptmanager-0.0.2/ptmanager/modules/process_manager.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     8692 2024-05-09 13:46:13.000000 ptmanager-0.0.2/ptmanager/modules/project_manager.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7472 2024-05-09 19:00:41.000000 ptmanager-0.0.2/ptmanager/modules/tools_manager.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     9009 2024-05-09 19:00:27.000000 ptmanager-0.0.2/ptmanager/ptmanager.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 19:10:13.089690 ptmanager-0.0.2/ptmanager.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3491 2024-05-09 19:10:13.000000 ptmanager-0.0.2/ptmanager.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      785 2024-05-09 19:10:13.000000 ptmanager-0.0.2/ptmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 19:10:13.000000 ptmanager-0.0.2/ptmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       55 2024-05-09 19:10:13.000000 ptmanager-0.0.2/ptmanager.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-09 19:10:13.000000 ptmanager-0.0.2/ptmanager.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       10 2024-05-09 19:10:13.000000 ptmanager-0.0.2/ptmanager.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 19:10:13.089690 ptmanager-0.0.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      934 2024-05-09 13:44:31.000000 ptmanager-0.0.2/setup.py
```

### Comparing `ptmanager-0.0.1/LICENSE` & `ptmanager-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptmanager-0.0.1/PKG-INFO` & `ptmanager-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptmanager
-Version: 0.0.1
+Version: 0.0.2
 Summary: Penterep Script Management Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `ptmanager-0.0.1/README.md` & `ptmanager-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ptmanager-0.0.1/ptmanager/modules/config.py` & `ptmanager-0.0.2/ptmanager/modules/config.py`

 * *Files identical despite different names*

### Comparing `ptmanager-0.0.1/ptmanager/modules/process.py` & `ptmanager-0.0.2/ptmanager/modules/process.py`

 * *Files identical despite different names*

### Comparing `ptmanager-0.0.1/ptmanager/modules/process_manager.py` & `ptmanager-0.0.2/ptmanager/modules/process_manager.py`

 * *Files identical despite different names*

### Comparing `ptmanager-0.0.1/ptmanager/modules/project_manager.py` & `ptmanager-0.0.2/ptmanager/modules/project_manager.py`

 * *Files identical despite different names*

### Comparing `ptmanager-0.0.1/ptmanager/modules/tools_manager.py` & `ptmanager-0.0.2/ptmanager/modules/tools_manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,47 +11,60 @@
     def __init__(self, ptjsonlib: ptjsonlib.PtJsonLib, use_json: bool) -> None:
         self.ptjsonlib = ptjsonlib
         self.use_json = use_json
 
     def print_available_tools(self) -> None:
         self._print_tools_table(self._get_script_list_from_api())
 
-    def _print_tools_table(self, tool_list_from_api, tools2update: list = None, tools2install: list = None) -> None:
+    def _print_tools_table(self, tool_list_from_api, tools2update: list = None, tools2install: list = None, tools2delete: list = None) -> None:
         print(f"{ptprinthelper.get_colored_text('Tool name', 'TITLE')}{' '*9}{ptprinthelper.get_colored_text('Installed', 'TITLE')}{' '*10}{ptprinthelper.get_colored_text('Latest', 'TITLE')}")
         print(f"{'-'*20}{'-'*19}{'-'*19}{'-'*6}")
 
         for ptscript in tool_list_from_api:
             is_installed, local_version = self.check_if_tool_is_installed(ptscript['name'])
             remote_version = ptscript["version"]
 
-            print(f"{ptscript['name']}{' '*(20-len(ptscript['name']))}{local_version}{' '*(19-len(local_version))}{remote_version}{' '*5}", end="" if tools2update or tools2install else "\n", flush=True)
+            print(f"{ptscript['name']}{' '*(20-len(ptscript['name']))}{local_version}{' '*(19-len(local_version))}{remote_version}{' '*5}", end="" if tools2update or tools2install or tools2delete else "\n", flush=True)
 
             if tools2install:
                 if ptscript["name"] in tools2install:
                     if not is_installed:
-                        print(self.install_update(tool_name=ptscript["name"], do_install=True))
+                        print(self._install_update_delete_tools(tool_name=ptscript["name"], do_install=True))
                     else:
                         print("Already installed")
                 else:
                     print("")
 
+            if tools2delete:
+                if ptscript["name"] in tools2delete:
+                    if is_installed:
+                        print(self._install_update_delete_tools(tool_name=ptscript["name"], do_delete=True))
+                    else:
+                        print("Already uninstalled")
+                else:
+                    print("")
+
             if tools2update:
                 if ptscript["name"] in tools2update:
                     if is_installed:
                         if local_version.replace(".", "") < remote_version.replace(".", ""):
-                            print(self.install_update(tool_name=ptscript["name"], local_version=local_version, do_update=True))
+                            print(self._install_update_delete_tools(tool_name=ptscript["name"], local_version=local_version, do_update=True))
                         elif local_version.replace(".", "") == remote_version.replace(".", ""):
                             print("Already latest version")
                         else:
                             print("Current version is > than the available version.")
                     else:
                         print("Install first before updating")
                 else:
                     print("")
 
+
+        #print(f"{'-'*20}{'-'*19}{'-'*19}{'-'*6}")
+
+
     def _get_script_list_from_api(self) -> list:
         """Retrieve available tools from API"""
         print("Fetching tools...", end="\r")
         try:
             available_tools = requests.get("https://raw.githubusercontent.com/Penterep/ptmanager/main/ptmanager/available_tools.txt").text.split("\n")
             available_tools = sorted(list(set([tool.strip() for tool in available_tools if tool.strip() and not tool.startswith("#")])))
             script_list = []
@@ -60,19 +73,14 @@
                 if response.status_code != 200:
                     continue
                 response = response.json()
                 script_list.append({"name": tool, "version": list(response['releases'].keys())[-1]})
         except Exception as e:
             self.ptjsonlib.end_error(f"Error retrieving tools from api - {e}", self.use_json)
 
-        """
-        for script in result:
-            if len(script.keys()) != 2 or not re.fullmatch("[a-z]+", script["name"]) or not re.fullmatch("[\d.]+", script["version"]):
-                self.ptjsonlib.end_error("Downloaded tool list is invalid", self.use_json)
-        """
         return sorted(script_list, key=lambda x: x['name'])
 
     def check_if_tool_is_installed(self, tool_name) -> tuple[bool, str]:
         try:
             p = subprocess.run([tool_name, "-v"], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
             local_version = p.stdout.split()[-1] # gets version
             is_installed = True
@@ -81,48 +89,67 @@
             is_installed = False
         except IndexError:
             local_version = "-"
             is_installed = False
         return is_installed, local_version
 
 
-    def install_update(self, tool_name:str, do_install=False, do_update=False, local_version=None) -> str:
-        assert do_update or do_install
+    def _install_update_delete_tools(self, tool_name:str, do_install=False, do_update=False, do_delete=False, local_version=None) -> str:
+        assert do_update or do_install or do_delete
+
         if do_install:
             process_args = ["pip", "install", tool_name]
+
         if do_update:
             process_args = ["pip", "install", tool_name, "--upgrade"]
-        process = subprocess.run(process_args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True) # install
-        try:
-            process = subprocess.run([tool_name, "-v"], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True) # check new version
-            new_version = process.stdout.split()[1]
-        except Exception as e:
-            return f"- -> Updated: Error - {e}"
-        if do_update:
-            return f"{local_version} -> {new_version} Updated: OK"
+
+        if do_delete:
+            if tool_name in ["ptlibs"]:
+                return "Cannot be deleted from ptmanager"
+            process_args = ["pip", "uninstall", tool_name, "-y"]
+
+
+        process = subprocess.run(process_args, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True) # install/update/delete
+        if do_delete:
+            try:
+                process = subprocess.run([tool_name, "-v"], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True) # check new version
+            except FileNotFoundError as e:
+                return f"Uninstall: OK"
+            except:
+                return f"Uninstall: {e}"
         else:
-            return f"Installed: OK"
+            try:
+                process = subprocess.run([tool_name, "-v"], stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True) # check new version
+                new_version = process.stdout.split()[1]
+            except Exception as e:
+                return f"- -> Updated: Error - {e}"
+            if do_update:
+                return f"{local_version} -> {new_version} Updated: OK"
+            else:
+                return f"Installed: OK"
 
 
-    def prepare_install_update_tools(self, tools2prepare: list, do_update: bool=None, do_install: bool=None) -> None:
-        """Prepare provided tools for installation or update"""
+    def prepare_install_update_delete_tools(self, tools2prepare: list, do_update: bool=None, do_install: bool=None, do_delete: bool = None) -> None:
+        """Prepare provided tools for installation or update or deletion"""
         tools2prepare = set([tool.lower() for unparsed_tool in tools2prepare for tool in unparsed_tool.split(",") if tool])
         script_list = self._get_script_list_from_api()
 
         if "all" in tools2prepare:
             tools2prepare = [tool["name"] for tool in script_list]
 
         valid_tool_names = [tool for tool in tools2prepare if self._check_if_tool_exists(tool, script_list)]
         invalid_tool_names = [tool for tool in tools2prepare if not self._check_if_tool_exists(tool, script_list)] if len(valid_tool_names) < len(tools2prepare) else []
 
         if valid_tool_names:
             if do_install:
                 self._print_tools_table(script_list, tools2install=valid_tool_names)
             if do_update:
                 self._print_tools_table(script_list, tools2update=valid_tool_names)
+            if do_delete:
+                self._print_tools_table(script_list, tools2delete=valid_tool_names)
 
         if invalid_tool_names:
             if not valid_tool_names:
                 self._print_tools_table(script_list)
             print("")
             self.ptjsonlib.end_error(f"Unrecognized Tool(s): [{', '.join(invalid_tool_names)}]", self.use_json)
```

### Comparing `ptmanager-0.0.1/ptmanager/ptmanager.py` & `ptmanager-0.0.2/ptmanager/ptmanager.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 
 import argparse
 import os
 import sys; sys.path.extend([__file__.rsplit("/", 1)[0], os.path.join(__file__.rsplit("/", 1)[0], "modules")])
 import pathlib
 import threading
 
+if os.getuid() == 0:
+    print("This script should not be run as root. Exiting.")
+    sys.exit(1)
+
 from _version import __version__
 from modules.config import Config
 from modules.project_manager import ProjectManager
 from modules.tools_manager import ToolsManager
 
 import requests
 from ptlibs import ptprinthelper, ptjsonlib
@@ -62,17 +66,20 @@
         elif args.project_list:
             self._get_project_manager().list_projects()
 
         # Handle Tool Manager
         elif args.tools_list:
             self._get_tools_manager().print_available_tools()
         elif args.tools_install:
-            self._get_tools_manager().prepare_install_update_tools(args.tools_install, do_install=True)
+            self._get_tools_manager().prepare_install_update_delete_tools(args.tools_install, do_install=True)
         elif args.tools_update:
-            self._get_tools_manager().prepare_install_update_tools(args.tools_update, do_update=True)
+            self._get_tools_manager().prepare_install_update_delete_tools(args.tools_update, do_update=True)
+        elif args.tools_delete:
+            self._get_tools_manager().prepare_install_update_delete_tools(args.tools_delete, do_delete=True)
+
 
         # Start Daemon
         elif args.connect:
             connect_thread = threading.Thread(target=self._connect, args=(args.target, args.auth, args.sid, args.threads, args._project_id))
             connect_thread.start()
         else:
             self.ptjsonlib.end_error("Bad argument combination", self.use_json)
@@ -100,28 +107,30 @@
     return [
         {"description": ["Penterep Tools Manager"]},
         {"usage": ["ptmanager <options>"]},
         {"usage_example": [
             "ptmanager --init",
             "ptmanager --project-new --target <target> --auth <auth>",
             "ptmanager --project-start 1",
+            "ptmanager --install-tools ptaxfr ptwebdiscover",
         ]},
         {"Manager options": [
             ["-pn",  "--project-new",          "",                 "Register new project"],
             ["-pl",  "--project-list",         "",                 "List available projects"],
             ["-ps",  "--project-start",        "<project_id>",     "Start project"],
             ["-pr",  "--project-reset",        "<project_id>",     "Restart project"],
             ["-pd",  "--project-delete",       "<project_id>",     "Delete project"],
             ["-pe",  "--project-end",          "<project_id>",     "End project"],
             ]
         },
         {"Tools options": [
-            ["-tl",  "--tools-list",             "",                "List available tools"],
-            ["-tu",  "--tools-update",           "<tools>",         "Update tool or update all tools"],
-            ["-ti",  "--tools-install",          "<tools>",         "Install tool or install all tools"],
+            ["-tl",  "--tools-list",             "",               "List available tools"],
+            ["-ti",  "--tools-install",          "<tool>",         "Install <tool>"],
+            ["-tu",  "--tools-update",           "<tool>",         "Update <tool>"],
+            ["-td",  "--tools-delete",           "<tool>",         "Delete <tool>"],
             ]
         },
         {"options": [
             ["-i",   "--initialize",             "",                 "Initialize ptmanager"],
             ["-T",   "--target",                 "<target>",         "Set target server"],
             ["-a",   "--auth",                   "<auth>",           "Set authorization code"],
             ["-S",   "--sid",                    "<sid>",            "Set session ID"],
@@ -130,14 +139,20 @@
             ["-nv",  "--no-ssl-verify",          "",                 "Do not verify SSL connections"],
             ["-v",   "--version",                "",                 "Show script version and exit"],
             ["-h",   "--help",                   "",                 "Show this help message and exit"],
             ]
         },
         ]
 
+def handle_tools_args(args):
+    attributes_to_check = ['tools_install', 'tools_update', 'tools_delete']
+    for attr in attributes_to_check:
+        if getattr(args, attr, None) == []:
+            setattr(args, attr, ["all"])
+    return args
 
 def parse_args():
     parser = argparse.ArgumentParser(add_help=False, usage=f"{SCRIPTNAME}.py <options>")
     parser.add_argument("-p",    "--proxy",           type=str)
     parser.add_argument("-nv",   "--no-ssl-verify",   action="store_false")
 
     parser.add_argument("-i",    "--init",            action="store_true")
@@ -146,37 +161,40 @@
     parser.add_argument("-pl",   "--project-list",    action="store_true")
     parser.add_argument("-ps",   "--project-start",   type=str)
     parser.add_argument("-pe",   "--project-end",     type=str)
     parser.add_argument("-pr",   "--project-reset",   type=str)
     parser.add_argument("-pd",   "--project-delete",  type=str)
 
     parser.add_argument("-tl", "-lt",  "--tools-list",      action="store_true")
-    parser.add_argument("-ti", "-it",  "--tools-install",   type=str, nargs="+")
-    parser.add_argument("-tu", "-ut",  "--tools-update",    type=str, nargs="+")
+    parser.add_argument("-ti", "-it",  "--tools-install",   type=str, nargs="*")
+    parser.add_argument("-tu", "-ut",  "--tools-update",    type=str, nargs="*")
+    parser.add_argument("-td", "-dt",  "--tools-delete",    type=str, nargs="*")
 
     parser.add_argument("-T",    "--target",          type=str)
     parser.add_argument("-a",    "--auth",            type=str)
     parser.add_argument("-S",    "--sid",             type=str)
     parser.add_argument("-prj",  "--_project_id",     type=str)
     parser.add_argument("-c",    "--connect",         action="store_true")
 
     parser.add_argument("-t",    "--threads",         type=int, default=20)
     parser.add_argument("-v",    "--version",         action="version", version=f"{SCRIPTNAME} {__version__}")
 
+
     if len(sys.argv) == 1 or "-h" in sys.argv or "--help" in sys.argv:
         ptprinthelper.help_print(get_help(), SCRIPTNAME, __version__)
         sys.exit(0)
+
     args = parser.parse_args()
     ptprinthelper.print_banner(SCRIPTNAME, __version__, False)
     return args
 
 
 def main():
     global SCRIPTNAME
     SCRIPTNAME = "ptmanager"
-    args = parse_args()
+    args = handle_tools_args(parse_args())
     manager = PtManager(args)
     manager.run(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ptmanager-0.0.1/ptmanager.egg-info/PKG-INFO` & `ptmanager-0.0.2/ptmanager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptmanager
-Version: 0.0.1
+Version: 0.0.2
 Summary: Penterep Script Management Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `ptmanager-0.0.1/setup.py` & `ptmanager-0.0.2/setup.py`

 * *Files identical despite different names*

