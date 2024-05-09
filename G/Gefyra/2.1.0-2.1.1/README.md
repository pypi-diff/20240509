# Comparing `tmp/gefyra-2.1.0.tar.gz` & `tmp/gefyra-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gefyra-2.1.0.tar", max compression
+gzip compressed data, was "gefyra-2.1.1.tar", max compression
```

## Comparing `gefyra-2.1.0.tar` & `gefyra-2.1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     2151 2024-04-22 07:14:08.776777 gefyra-2.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-22 07:14:08.776777 gefyra-2.1.0/gefyra/__init__.py
--rw-r--r--   0        0        0      239 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/__init__.py
--rw-r--r--   0        0        0     8859 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/bridge.py
--rw-r--r--   0        0        0     3981 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/clients.py
--rw-r--r--   0        0        0    10597 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/connect.py
--rw-r--r--   0        0        0     5845 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/install.py
--rw-r--r--   0        0        0     3066 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/list.py
--rw-r--r--   0        0        0     2797 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/reflect.py
--rw-r--r--   0        0        0     4422 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/run.py
--rw-r--r--   0        0        0     5375 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/status.py
--rw-r--r--   0        0        0     2179 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/api/utils.py
--rw-r--r--   0        0        0        0 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/__init__.py
--rw-r--r--   0        0        0     4298 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/bridge.py
--rw-r--r--   0        0        0     3763 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/clients.py
--rw-r--r--   0        0        0     5310 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/connections.py
--rw-r--r--   0        0        0      268 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/console.py
--rw-r--r--   0        0        0     2800 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/installation.py
--rw-r--r--   0        0        0     2937 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/list.py
--rw-r--r--   0        0        0     2367 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/main.py
--rw-r--r--   0        0        0     2261 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/run.py
--rw-r--r--   0        0        0      384 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/self.py
--rw-r--r--   0        0        0      217 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/status.py
--rw-r--r--   0        0        0     4859 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/telemetry.py
--rw-r--r--   0        0        0     7345 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/updown.py
--rw-r--r--   0        0        0     7961 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/utils.py
--rw-r--r--   0        0        0     1024 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cli/version.py
--rw-r--r--   0        0        0        0 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cluster/__init__.py
--rw-r--r--   0        0        0     4642 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cluster/resources.py
--rw-r--r--   0        0        0     5385 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/cluster/utils.py
--rw-r--r--   0        0        0    13270 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/configuration.py
--rw-r--r--   0        0        0      516 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/exceptions.py
--rw-r--r--   0        0        0      441 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/__init__.py
--rw-r--r--   0        0        0     6579 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/bridge.py
--rw-r--r--   0        0        0     1927 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/cargo.py
--rw-r--r--   0        0        0     4167 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/clients.py
--rw-r--r--   0        0        0     2237 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/minikube.py
--rw-r--r--   0        0        0     4594 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/networking.py
--rw-r--r--   0        0        0     4354 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/local/utils.py
--rw-r--r--   0        0        0        0 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/__init__.py
--rw-r--r--   0        0        0      214 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/comps/__init__.py
--rw-r--r--   0        0        0     4741 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/comps/deployment.py
--rw-r--r--   0        0        0      331 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/comps/namespace.py
--rw-r--r--   0        0        0     3200 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/comps/rbac.py
--rw-r--r--   0        0        0     2106 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/comps/service.py
--rw-r--r--   0        0        0     4530 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/comps/webhook.py
--rw-r--r--   0        0        0     1583 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/install.py
--rw-r--r--   0        0        0     2887 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/uninstall.py
--rw-r--r--   0        0        0      486 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/misc/utils.py
--rw-r--r--   0        0        0    10557 2024-04-22 07:14:08.780777 gefyra-2.1.0/gefyra/types.py
--rw-r--r--   0        0        0     1849 2024-04-22 07:14:08.780777 gefyra-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 gefyra-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2151 2024-04-26 14:40:35.249659 gefyra-2.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/__init__.py
+-rw-r--r--   0        0        0      239 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/api/__init__.py
+-rw-r--r--   0        0        0     8859 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/api/bridge.py
+-rw-r--r--   0        0        0     3981 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/api/clients.py
+-rw-r--r--   0        0        0    10597 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/api/connect.py
+-rw-r--r--   0        0        0     5845 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/api/install.py
+-rw-r--r--   0        0        0     3066 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/api/list.py
+-rw-r--r--   0        0        0     2797 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/api/reflect.py
+-rw-r--r--   0        0        0     4422 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/api/run.py
+-rw-r--r--   0        0        0     5375 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/api/status.py
+-rw-r--r--   0        0        0     2179 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/api/utils.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/__init__.py
+-rw-r--r--   0        0        0     4298 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/bridge.py
+-rw-r--r--   0        0        0     3763 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/clients.py
+-rw-r--r--   0        0        0     5310 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/connections.py
+-rw-r--r--   0        0        0      268 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/console.py
+-rw-r--r--   0        0        0     2800 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/installation.py
+-rw-r--r--   0        0        0     2937 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/list.py
+-rw-r--r--   0        0        0     2367 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/main.py
+-rw-r--r--   0        0        0     2366 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/run.py
+-rw-r--r--   0        0        0      384 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/self.py
+-rw-r--r--   0        0        0      217 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/status.py
+-rw-r--r--   0        0        0     4859 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/telemetry.py
+-rw-r--r--   0        0        0     7345 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/updown.py
+-rw-r--r--   0        0        0     8537 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/utils.py
+-rw-r--r--   0        0        0     1024 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cli/version.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cluster/__init__.py
+-rw-r--r--   0        0        0     4642 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cluster/resources.py
+-rw-r--r--   0        0        0     5385 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/cluster/utils.py
+-rw-r--r--   0        0        0    13270 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/configuration.py
+-rw-r--r--   0        0        0      516 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/exceptions.py
+-rw-r--r--   0        0        0      441 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/local/__init__.py
+-rw-r--r--   0        0        0     6579 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/local/bridge.py
+-rw-r--r--   0        0        0     1927 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/local/cargo.py
+-rw-r--r--   0        0        0     4167 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/local/clients.py
+-rw-r--r--   0        0        0     2237 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/local/minikube.py
+-rw-r--r--   0        0        0     4594 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/local/networking.py
+-rw-r--r--   0        0        0     4354 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/local/utils.py
+-rw-r--r--   0        0        0        0 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/misc/__init__.py
+-rw-r--r--   0        0        0      214 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/misc/comps/__init__.py
+-rw-r--r--   0        0        0     4741 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/misc/comps/deployment.py
+-rw-r--r--   0        0        0      331 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/misc/comps/namespace.py
+-rw-r--r--   0        0        0     3200 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/misc/comps/rbac.py
+-rw-r--r--   0        0        0     2106 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/misc/comps/service.py
+-rw-r--r--   0        0        0     4530 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/misc/comps/webhook.py
+-rw-r--r--   0        0        0     1583 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/misc/install.py
+-rw-r--r--   0        0        0     2887 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/misc/uninstall.py
+-rw-r--r--   0        0        0      486 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/misc/utils.py
+-rw-r--r--   0        0        0    10557 2024-04-26 14:40:35.249659 gefyra-2.1.1/gefyra/types.py
+-rw-r--r--   0        0        0     1849 2024-04-26 14:40:35.249659 gefyra-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 gefyra-2.1.1/PKG-INFO
```

### Comparing `gefyra-2.1.0/README.md` & `gefyra-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/api/bridge.py` & `gefyra-2.1.1/gefyra/api/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/api/clients.py` & `gefyra-2.1.1/gefyra/api/clients.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/api/connect.py` & `gefyra-2.1.1/gefyra/api/connect.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/api/install.py` & `gefyra-2.1.1/gefyra/api/install.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/api/list.py` & `gefyra-2.1.1/gefyra/api/list.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/api/reflect.py` & `gefyra-2.1.1/gefyra/api/reflect.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/api/run.py` & `gefyra-2.1.1/gefyra/api/run.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/api/status.py` & `gefyra-2.1.1/gefyra/api/status.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/api/utils.py` & `gefyra-2.1.1/gefyra/api/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/cli/bridge.py` & `gefyra-2.1.1/gefyra/cli/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/cli/clients.py` & `gefyra-2.1.1/gefyra/cli/clients.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/cli/connections.py` & `gefyra-2.1.1/gefyra/cli/connections.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/cli/installation.py` & `gefyra-2.1.1/gefyra/cli/installation.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/cli/list.py` & `gefyra-2.1.1/gefyra/cli/list.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/cli/main.py` & `gefyra-2.1.1/gefyra/cli/main.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/cli/run.py` & `gefyra-2.1.1/gefyra/cli/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 import ast
 import click
-from gefyra.cli.utils import OptionEatAll, check_connection_name, parse_ip_port_map
+from gefyra.cli.utils import (
+    OptionEatAll,
+    check_connection_name,
+    parse_env,
+    parse_ip_port_map,
+    parse_workload,
+)
 
 
 @click.command()
 @click.option(
     "-d",
     "--detach",
     help="Run container in background and print container ID",
@@ -28,14 +34,15 @@
     multiple=True,
     callback=parse_ip_port_map,
 )
 @click.option(
     "--env-from",
     help="Copy the environment from the container in the notation 'Pod/Container'",
     type=str,
+    callback=parse_workload,
 )
 @click.option(
     "-v",
     "--volume",
     help=(
         "Bind mount a volume into the container in notation src:dest, allowed multiple"
         " times"
@@ -46,14 +53,15 @@
 @click.option(
     "--env",
     help=(
         "Set or override environment variables in the form ENV=value, allowed multiple"
         " times"
     ),
     type=str,
+    callback=parse_env,
     multiple=True,
 )
 @click.option(
     "-n", "--namespace", help="The namespace for this container to run in", type=str
 )
 @click.option(
     "-c",
```

### Comparing `gefyra-2.1.0/gefyra/cli/telemetry.py` & `gefyra-2.1.1/gefyra/cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/cli/updown.py` & `gefyra-2.1.1/gefyra/cli/updown.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/cli/utils.py` & `gefyra-2.1.1/gefyra/cli/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -212,14 +212,35 @@
         elif len(_value) == 3:
             res[v(_value[2])] = (_value[0], v(_value[1]))
         else:
             raise ValueError("Invalid value for port mapping.")
     return res
 
 
+def parse_env(ctx, param, envs: Tuple[str]) -> List[str]:
+    res = []
+    for env in envs:
+        if "=" not in env:
+            raise ValueError("Invalid value for env variable. Please use 'ENV=value'.")
+        res.append(env)
+    return res
+
+
+def parse_workload(ctx, param, workload: str) -> str:
+    MSG = (
+        "Invalid workload format. Please provide the workload "
+        "in the format 'type/name' or 'type/name/container-name'."
+    )
+    if not workload:
+        return workload
+    if "/" not in workload:
+        raise ValueError(MSG)
+    return workload
+
+
 def check_connection_name(ctx, param, selected: Optional[str] = None) -> str:
     from gefyra import api
 
     conn_list = api.list_connections()
     if not conn_list:
         raise click.UsageError(
             message="No Gefyra connection found. Please connect to a cluster first or run by "
```

### Comparing `gefyra-2.1.0/gefyra/cli/version.py` & `gefyra-2.1.1/gefyra/cli/version.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/cluster/resources.py` & `gefyra-2.1.1/gefyra/cluster/resources.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/cluster/utils.py` & `gefyra-2.1.1/gefyra/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/configuration.py` & `gefyra-2.1.1/gefyra/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     CARGO_ENDPOINT_LABEL,
     ACTIVE_KUBECONFIG_LABEL,
     CLIENT_ID_LABEL,
 )
 
 logger = logging.getLogger("gefyra")
 
-__VERSION__ = "2.1.0"
+__VERSION__ = "2.1.1"
 USER_HOME = os.path.expanduser("~")
 
 
 def fix_pywin32_in_frozen_build() -> None:  # pragma: no cover
     import os
     import site
```

### Comparing `gefyra-2.1.0/gefyra/exceptions.py` & `gefyra-2.1.1/gefyra/exceptions.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/local/bridge.py` & `gefyra-2.1.1/gefyra/local/bridge.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/local/cargo.py` & `gefyra-2.1.1/gefyra/local/cargo.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/local/clients.py` & `gefyra-2.1.1/gefyra/local/clients.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/local/minikube.py` & `gefyra-2.1.1/gefyra/local/minikube.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/local/networking.py` & `gefyra-2.1.1/gefyra/local/networking.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/local/utils.py` & `gefyra-2.1.1/gefyra/local/utils.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/misc/comps/deployment.py` & `gefyra-2.1.1/gefyra/misc/comps/deployment.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/misc/comps/rbac.py` & `gefyra-2.1.1/gefyra/misc/comps/rbac.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/misc/comps/service.py` & `gefyra-2.1.1/gefyra/misc/comps/service.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/misc/comps/webhook.py` & `gefyra-2.1.1/gefyra/misc/comps/webhook.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/misc/install.py` & `gefyra-2.1.1/gefyra/misc/install.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/misc/uninstall.py` & `gefyra-2.1.1/gefyra/misc/uninstall.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/gefyra/types.py` & `gefyra-2.1.1/gefyra/types.py`

 * *Files identical despite different names*

### Comparing `gefyra-2.1.0/pyproject.toml` & `gefyra-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Gefyra"
-version = "2.1.0"
+version = "2.1.1"
 description = "Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure"
 authors = ["Michael Schilonka <michael@blueshoe.io>"]
 readme = "README.md"
 homepage = "https://gefyra.dev"
 repository = "https://github.com/gefyrahq/gefyra"
 documentation = "https://gefyra.dev"
 keywords = [
```

### Comparing `gefyra-2.1.0/PKG-INFO` & `gefyra-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Gefyra
-Version: 2.1.0
+Version: 2.1.1
 Summary: Gefyra runs all developer machine side components of Gefyra's Kubernetes-based development infrastructure
 Home-page: https://gefyra.dev
 Keywords: Kubernetes,Development,Cloud-native
 Author: Michael Schilonka
 Author-email: michael@blueshoe.io
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

