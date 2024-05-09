# Comparing `tmp/truefoundry-0.2.1.tar.gz` & `tmp/truefoundry-0.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truefoundry-0.2.1.tar", max compression
+gzip compressed data, was "truefoundry-0.2.2rc1.tar", max compression
```

## Comparing `truefoundry-0.2.1.tar` & `truefoundry-0.2.2rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      871 2024-05-08 09:54:41.781041 truefoundry-0.2.1/README.md
--rw-r--r--   0        0        0     1145 2024-05-08 09:54:50.441035 truefoundry-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-08 09:54:41.781041 truefoundry-0.2.1/truefoundry/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:54:41.781041 truefoundry-0.2.1/truefoundry/autodeploy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:54:41.781041 truefoundry-0.2.1/truefoundry/autodeploy/agents/__init__.py
--rw-r--r--   0        0        0     6405 2024-05-08 09:54:41.781041 truefoundry-0.2.1/truefoundry/autodeploy/agents/base.py
--rw-r--r--   0        0        0     4126 2024-05-08 09:54:41.781041 truefoundry-0.2.1/truefoundry/autodeploy/agents/developer.py
--rw-r--r--   0        0        0     4438 2024-05-08 09:54:41.781041 truefoundry-0.2.1/truefoundry/autodeploy/agents/project_identifier.py
--rw-r--r--   0        0        0     2352 2024-05-08 09:54:41.781041 truefoundry-0.2.1/truefoundry/autodeploy/agents/tester.py
--rw-r--r--   0        0        0    13651 2024-05-08 09:54:41.781041 truefoundry-0.2.1/truefoundry/autodeploy/cli.py
--rw-r--r--   0        0        0     1553 2024-05-08 09:54:41.781041 truefoundry-0.2.1/truefoundry/autodeploy/constants.py
--rw-r--r--   0        0        0      158 2024-05-08 09:54:41.781041 truefoundry-0.2.1/truefoundry/autodeploy/exception.py
--rw-r--r--   0        0        0      325 2024-05-08 09:54:41.781041 truefoundry-0.2.1/truefoundry/autodeploy/logger.py
--rw-r--r--   0        0        0      875 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/tools/__init__.py
--rw-r--r--   0        0        0      856 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/tools/ask.py
--rw-r--r--   0        0        0      665 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/tools/base.py
--rw-r--r--   0        0        0     5990 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/tools/commit.py
--rw-r--r--   0        0        0     3931 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/tools/docker_build.py
--rw-r--r--   0        0        0     4993 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/tools/docker_run.py
--rw-r--r--   0        0        0     2288 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/tools/file_type_counts.py
--rw-r--r--   0        0        0     2577 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/tools/list_files.py
--rw-r--r--   0        0        0     2187 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/tools/read_file.py
--rw-r--r--   0        0        0     1614 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/tools/send_request.py
--rw-r--r--   0        0        0     3130 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/tools/write_file.py
--rw-r--r--   0        0        0      453 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/utils/client.py
--rw-r--r--   0        0        0     5358 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/utils/diff.py
--rw-r--r--   0        0        0      412 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/autodeploy/utils/pydantic_compat.py
--rw-r--r--   0        0        0        0 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/cli/__init__.py
--rw-r--r--   0        0        0      916 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/cli/__main__.py
--rw-r--r--   0        0        0       43 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/deploy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/deploy/cli/__init__.py
--rw-r--r--   0        0        0     3113 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/deploy/cli/cli.py
--rw-r--r--   0        0        0     5105 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/deploy/cli/deploy.py
--rw-r--r--   0        0        0       53 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/langchain/__init__.py
--rw-r--r--   0        0        0      179 2024-05-08 09:54:41.785041 truefoundry-0.2.1/truefoundry/ml/__init__.py
--rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 truefoundry-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      871 2024-05-09 16:53:57.991343 truefoundry-0.2.2rc1/README.md
+-rw-r--r--   0        0        0     1148 2024-05-09 16:54:07.603477 truefoundry-0.2.2rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-09 16:53:57.991343 truefoundry-0.2.2rc1/truefoundry/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/__init__.py
+-rw-r--r--   0        0        0     6405 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/base.py
+-rw-r--r--   0        0        0     4126 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/developer.py
+-rw-r--r--   0        0        0     4438 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/project_identifier.py
+-rw-r--r--   0        0        0     2352 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/tester.py
+-rw-r--r--   0        0        0    13651 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/cli.py
+-rw-r--r--   0        0        0     1553 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/constants.py
+-rw-r--r--   0        0        0      158 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/exception.py
+-rw-r--r--   0        0        0      325 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/logger.py
+-rw-r--r--   0        0        0      875 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/__init__.py
+-rw-r--r--   0        0        0      856 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/ask.py
+-rw-r--r--   0        0        0      665 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/base.py
+-rw-r--r--   0        0        0     5990 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/commit.py
+-rw-r--r--   0        0        0     3931 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/docker_build.py
+-rw-r--r--   0        0        0     4993 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/docker_run.py
+-rw-r--r--   0        0        0     2288 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/file_type_counts.py
+-rw-r--r--   0        0        0     2577 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/list_files.py
+-rw-r--r--   0        0        0     2187 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/read_file.py
+-rw-r--r--   0        0        0     1614 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/send_request.py
+-rw-r--r--   0        0        0     3130 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/write_file.py
+-rw-r--r--   0        0        0      453 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/utils/client.py
+-rw-r--r--   0        0        0     5358 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/utils/diff.py
+-rw-r--r--   0        0        0      412 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/autodeploy/utils/pydantic_compat.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      916 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/cli/__main__.py
+-rw-r--r--   0        0        0       43 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/deploy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/deploy/cli/__init__.py
+-rw-r--r--   0        0        0     3135 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/deploy/cli/cli.py
+-rw-r--r--   0        0        0     5105 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/deploy/cli/deploy.py
+-rw-r--r--   0        0        0       53 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/langchain/__init__.py
+-rw-r--r--   0        0        0      179 2024-05-09 16:53:57.995343 truefoundry-0.2.2rc1/truefoundry/ml/__init__.py
+-rw-r--r--   0        0        0     1839 1970-01-01 00:00:00.000000 truefoundry-0.2.2rc1/PKG-INFO
```

### Comparing `truefoundry-0.2.1/README.md` & `truefoundry-0.2.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/pyproject.toml` & `truefoundry-0.2.2rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truefoundry"
-version = "0.2.1"
+version = "0.2.2rc1"
 description = "Truefoundry CLI"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.13"
 servicefoundry = "0.10.11"
```

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/agents/base.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/agents/developer.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/developer.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/agents/project_identifier.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/project_identifier.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/agents/tester.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/agents/tester.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/cli.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/cli.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/constants.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/constants.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/tools/__init__.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/tools/ask.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/ask.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/tools/base.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/base.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/tools/commit.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/commit.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/tools/docker_build.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/docker_build.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/tools/docker_run.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/docker_run.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/tools/file_type_counts.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/file_type_counts.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/tools/list_files.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/list_files.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/tools/read_file.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/read_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/tools/send_request.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/send_request.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/tools/write_file.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/tools/write_file.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/autodeploy/utils/diff.py` & `truefoundry-0.2.2rc1/truefoundry/autodeploy/utils/diff.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/cli/__main__.py` & `truefoundry-0.2.2rc1/truefoundry/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/truefoundry/deploy/cli/cli.py` & `truefoundry-0.2.2rc1/truefoundry/deploy/cli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import sys
 
 import rich_click as click
 from servicefoundry import logger
 from servicefoundry.cli.commands import (
     deploy_patch_v2_command,
+    get_delete_command,
     get_login_command,
     get_logout_command,
     get_patch_command,
 )
 from servicefoundry.cli.config import CliConfig
 from servicefoundry.cli.const import GROUP_CLS
 from servicefoundry.cli.util import setup_rich_click
@@ -34,15 +35,15 @@
     Returns:
         function: main CLI functions will all added sub-commands
     """
     cli = truefoundry_cli
     cli.add_command(get_login_command())
     # cli.add_command(get_get_command())
     # cli.add_command(get_list_command())
-    # cli.add_command(get_delete_command())
+    cli.add_command(get_delete_command())
     # cli.add_command(get_create_command())
     # cli.add_command(get_redeploy_command())
     cli.add_command(get_logout_command())
     # cli.add_command(get_build_command())
     cli.add_command(deploy_v2_command)
     cli.add_command(deploy_patch_v2_command)
     # cli.add_command(get_build_logs_command())
```

### Comparing `truefoundry-0.2.1/truefoundry/deploy/cli/deploy.py` & `truefoundry-0.2.2rc1/truefoundry/deploy/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `truefoundry-0.2.1/PKG-INFO` & `truefoundry-0.2.2rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truefoundry
-Version: 0.2.1
+Version: 0.2.2rc1
 Summary: Truefoundry CLI
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

