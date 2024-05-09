# Comparing `tmp/faasmsctl-0.0.2.tar.gz` & `tmp/faasmsctl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmsctl-0.0.2.tar", last modified: Tue Apr 30 06:03:27 2024, max compression
+gzip compressed data, was "faasmsctl-0.0.3.tar", last modified: Thu May  9 06:02:34 2024, max compression
```

## Comparing `faasmsctl-0.0.2.tar` & `faasmsctl-0.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:03:27.916379 faasmsctl-0.0.2/
--rw-r--r--   0 root         (0) root         (0)    11343 2024-03-17 03:05:30.000000 faasmsctl-0.0.2/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1369 2024-04-30 06:03:27.916379 faasmsctl-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      777 2024-03-17 03:05:30.000000 faasmsctl-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:03:27.908379 faasmsctl-0.0.2/faasmsctl/
--rw-r--r--   0 root         (0) root         (0)       55 2024-03-17 07:29:35.000000 faasmsctl-0.0.2/faasmsctl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:03:27.908379 faasmsctl-0.0.2/faasmsctl/bin/
--rwxr-xr-x   0 root         (0) root         (0)     3438 2024-03-17 03:05:30.000000 faasmsctl-0.0.2/faasmsctl/bin/gen_proto_files.py
--rw-r--r--   0 root         (0) root         (0)      316 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:03:27.912379 faasmsctl-0.0.2/faasmsctl/tasks/
--rw-r--r--   0 root         (0) root         (0)      415 2024-04-30 03:22:38.000000 faasmsctl-0.0.2/faasmsctl/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5691 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/tasks/cli.py
--rw-r--r--   0 root         (0) root         (0)      826 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/tasks/delete.py
--rw-r--r--   0 root         (0) root         (0)     3414 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/tasks/deploy.py
--rw-r--r--   0 root         (0) root         (0)      657 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/tasks/flush.py
--rw-r--r--   0 root         (0) root         (0)      396 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/tasks/generate.py
--rw-r--r--   0 root         (0) root         (0)     3457 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/tasks/invoke.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/tasks/logs.py
--rw-r--r--   0 root         (0) root         (0)     9494 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/tasks/monitor.py
--rw-r--r--   0 root         (0) root         (0)      897 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/tasks/restart.py
--rw-r--r--   0 root         (0) root         (0)      811 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/tasks/status.py
--rw-r--r--   0 root         (0) root         (0)     1347 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/tasks/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:03:27.916379 faasmsctl-0.0.2/faasmsctl/util/
--rw-r--r--   0 root         (0) root         (0)       48 2024-03-17 03:05:30.000000 faasmsctl-0.0.2/faasmsctl/util/backend.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/util/batch.py
--rw-r--r--   0 root         (0) root         (0)    13036 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/util/compose.py
--rw-r--r--   0 root         (0) root         (0)     2136 2024-03-17 03:05:30.000000 faasmsctl-0.0.2/faasmsctl/util/config.py
--rw-r--r--   0 root         (0) root         (0)     5978 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/util/deploy.py
--rw-r--r--   0 root         (0) root         (0)     1698 2024-03-17 03:05:30.000000 faasmsctl-0.0.2/faasmsctl/util/docker.py
--rw-r--r--   0 root         (0) root         (0)      471 2024-03-17 03:05:30.000000 faasmsctl-0.0.2/faasmsctl/util/env.py
--rw-r--r--   0 root         (0) root         (0)      670 2024-03-17 03:05:30.000000 faasmsctl-0.0.2/faasmsctl/util/faasm.py
--rw-r--r--   0 root         (0) root         (0)     1072 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/util/flush.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:03:27.916379 faasmsctl-0.0.2/faasmsctl/util/gen_proto/
--rw-r--r--   0 root         (0) root         (0)     8601 2024-03-17 03:24:35.000000 faasmsctl-0.0.2/faasmsctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4816 2024-03-17 03:24:35.000000 faasmsctl-0.0.2/faasmsctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5301 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/util/invoke.py
--rw-r--r--   0 root         (0) root         (0)    10550 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/util/k8s.py
--rw-r--r--   0 root         (0) root         (0)      360 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/util/message.py
--rw-r--r--   0 root         (0) root         (0)     1094 2024-03-17 03:05:30.000000 faasmsctl-0.0.2/faasmsctl/util/network.py
--rw-r--r--   0 root         (0) root         (0)     4471 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/util/planner.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-03-17 03:05:30.000000 faasmsctl-0.0.2/faasmsctl/util/random.py
--rw-r--r--   0 root         (0) root         (0)     1371 2024-03-17 03:05:30.000000 faasmsctl-0.0.2/faasmsctl/util/results.py
--rw-r--r--   0 root         (0) root         (0)     2019 2024-04-30 05:49:44.000000 faasmsctl-0.0.2/faasmsctl/util/upload.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-03-17 03:05:30.000000 faasmsctl-0.0.2/faasmsctl/util/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 06:03:27.916379 faasmsctl-0.0.2/faasmsctl.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1369 2024-04-30 06:03:27.000000 faasmsctl-0.0.2/faasmsctl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1158 2024-04-30 06:03:27.000000 faasmsctl-0.0.2/faasmsctl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 06:03:27.000000 faasmsctl-0.0.2/faasmsctl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-30 06:03:27.000000 faasmsctl-0.0.2/faasmsctl.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-04-30 06:03:27.000000 faasmsctl-0.0.2/faasmsctl.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-30 06:03:27.000000 faasmsctl-0.0.2/faasmsctl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      739 2024-04-30 05:50:38.000000 faasmsctl-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       90 2024-04-30 06:03:27.916379 faasmsctl-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:34.371420 faasmsctl-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)    11343 2024-03-17 03:05:30.000000 faasmsctl-0.0.3/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1369 2024-05-09 06:02:34.371420 faasmsctl-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      777 2024-03-17 03:05:30.000000 faasmsctl-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:34.363420 faasmsctl-0.0.3/faasmsctl/
+-rw-r--r--   0 root         (0) root         (0)       55 2024-03-17 07:29:35.000000 faasmsctl-0.0.3/faasmsctl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:34.367420 faasmsctl-0.0.3/faasmsctl/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     3457 2024-05-09 05:44:24.000000 faasmsctl-0.0.3/faasmsctl/bin/gen_proto_files.py
+-rw-r--r--   0 root         (0) root         (0)      319 2024-04-30 06:18:57.000000 faasmsctl-0.0.3/faasmsctl/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:34.367420 faasmsctl-0.0.3/faasmsctl/tasks/
+-rw-r--r--   0 root         (0) root         (0)      415 2024-04-30 03:22:38.000000 faasmsctl-0.0.3/faasmsctl/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5691 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/tasks/cli.py
+-rw-r--r--   0 root         (0) root         (0)      826 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/tasks/delete.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2024-04-30 06:19:11.000000 faasmsctl-0.0.3/faasmsctl/tasks/deploy.py
+-rw-r--r--   0 root         (0) root         (0)      657 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/tasks/flush.py
+-rw-r--r--   0 root         (0) root         (0)      396 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/tasks/generate.py
+-rw-r--r--   0 root         (0) root         (0)     3457 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/tasks/invoke.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/tasks/logs.py
+-rw-r--r--   0 root         (0) root         (0)     9494 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/tasks/monitor.py
+-rw-r--r--   0 root         (0) root         (0)      897 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/tasks/restart.py
+-rw-r--r--   0 root         (0) root         (0)      811 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/tasks/status.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2024-04-30 06:19:14.000000 faasmsctl-0.0.3/faasmsctl/tasks/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:34.371420 faasmsctl-0.0.3/faasmsctl/util/
+-rw-r--r--   0 root         (0) root         (0)       48 2024-03-17 03:05:30.000000 faasmsctl-0.0.3/faasmsctl/util/backend.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/util/batch.py
+-rw-r--r--   0 root         (0) root         (0)    13036 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/util/compose.py
+-rw-r--r--   0 root         (0) root         (0)     2136 2024-03-17 03:05:30.000000 faasmsctl-0.0.3/faasmsctl/util/config.py
+-rw-r--r--   0 root         (0) root         (0)     5980 2024-04-30 06:19:15.000000 faasmsctl-0.0.3/faasmsctl/util/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     1700 2024-04-30 06:19:16.000000 faasmsctl-0.0.3/faasmsctl/util/docker.py
+-rw-r--r--   0 root         (0) root         (0)      474 2024-04-30 06:19:31.000000 faasmsctl-0.0.3/faasmsctl/util/env.py
+-rw-r--r--   0 root         (0) root         (0)      671 2024-04-30 06:19:17.000000 faasmsctl-0.0.3/faasmsctl/util/faasm.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/util/flush.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:34.371420 faasmsctl-0.0.3/faasmsctl/util/gen_proto/
+-rw-r--r--   0 root         (0) root         (0)     8601 2024-03-17 03:24:35.000000 faasmsctl-0.0.3/faasmsctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4816 2024-05-08 02:36:31.000000 faasmsctl-0.0.3/faasmsctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/util/invoke.py
+-rw-r--r--   0 root         (0) root         (0)    10550 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/util/k8s.py
+-rw-r--r--   0 root         (0) root         (0)      360 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/util/message.py
+-rw-r--r--   0 root         (0) root         (0)     1094 2024-03-17 03:05:30.000000 faasmsctl-0.0.3/faasmsctl/util/network.py
+-rw-r--r--   0 root         (0) root         (0)     4471 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/util/planner.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-03-17 03:05:30.000000 faasmsctl-0.0.3/faasmsctl/util/random.py
+-rw-r--r--   0 root         (0) root         (0)     1371 2024-03-17 03:05:30.000000 faasmsctl-0.0.3/faasmsctl/util/results.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-04-30 05:49:44.000000 faasmsctl-0.0.3/faasmsctl/util/upload.py
+-rw-r--r--   0 root         (0) root         (0)       79 2024-04-30 06:19:20.000000 faasmsctl-0.0.3/faasmsctl/util/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 06:02:34.371420 faasmsctl-0.0.3/faasmsctl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1369 2024-05-09 06:02:34.000000 faasmsctl-0.0.3/faasmsctl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1158 2024-05-09 06:02:34.000000 faasmsctl-0.0.3/faasmsctl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 06:02:34.000000 faasmsctl-0.0.3/faasmsctl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-09 06:02:34.000000 faasmsctl-0.0.3/faasmsctl.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-09 06:02:34.000000 faasmsctl-0.0.3/faasmsctl.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-09 06:02:34.000000 faasmsctl-0.0.3/faasmsctl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2024-05-09 05:45:28.000000 faasmsctl-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-09 06:02:34.371420 faasmsctl-0.0.3/setup.cfg
```

### Comparing `faasmsctl-0.0.2/LICENSE.md` & `faasmsctl-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/PKG-INFO` & `faasmsctl-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmsctl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Command line tool to deploy, manage, and interact with Faasm Stream
 Author-email: Faasm Team <foo@bar.com>, Tianyu <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `faasmsctl-0.0.2/README.md` & `faasmsctl-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/bin/gen_proto_files.py` & `faasmsctl-0.0.3/faasmsctl/bin/gen_proto_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 from os import environ, listdir, makedirs
 from os.path import dirname, exists, join, realpath
 from shutil import rmtree
 from sys import argv
 from subprocess import run
 
-FAASMCTL_ROOT = dirname(dirname(realpath(__file__)))
+faasmsctl_ROOT = dirname(dirname(realpath(__file__)))
 
 # Unfortunately, we need to duplicate this constants here as we need to be
 # able to run this file in standalone mode, as if the proto files are not
-# generated, some imports in `faasmctl` will fail
-GEN_PROTO_DIR = join(FAASMCTL_ROOT, "util", "gen_proto")
+# generated, some imports in `faasmsctl` will fail
+GEN_PROTO_DIR = join(faasmsctl_ROOT, "util", "gen_proto")
 FAASM_CLI_IMAGE = "faasm.azurecr.io/cli"
 
 PROTO_FILES = [
     "faabric_pb2.py",
     "planner_pb2.py",
 ]
 
 
-# We can not import faasmctl here
+# We can not import faasmsctl here
 def get_faasm_version():
-    ver_file = join(FAASMCTL_ROOT, "util", "faasm.py")
+    ver_file = join(faasmsctl_ROOT, "util", "faasm.py")
     cmd = "cat {} | grep 'FAASM_VERSION =' | cut -d' ' -f3".format(ver_file)
     version = (
         run(cmd, shell=True, check=True, capture_output=True)
         .stdout.decode("utf-8")
         .strip()[1:-1]
     )
 
@@ -76,31 +76,31 @@
 
     # Generate python protobuf files
     code_dir = "/usr/local/code/faasm/faabric"
     protoc_cmd = [
         p_bin,
         "--proto_path={}".format(code_dir),
         "--python_out={}".format(code_dir),
-        "{}/src/planner/planner.proto".format(code_dir),
-        "{}/src/proto/faabric.proto".format(code_dir),
+        "{}/src/planner/plannerstream.proto".format(code_dir),
+        "{}/src/proto/faabricstream.proto".format(code_dir),
     ]
     protoc_cmd = " ".join(protoc_cmd)
     docker_cmd = "{} bash -c '{}'".format(docker_exec_prefix, protoc_cmd)
     run(docker_cmd, shell=True, check=True)
 
     # Finally, copy the generated protobuf files to the desired location
     for proto_file in PROTO_FILES:
         if "planner" in proto_file:
             proto_ctr_path = join(code_dir, "src", "planner", proto_file)
         else:
             proto_ctr_path = join(code_dir, "src", "proto", proto_file)
-        proto_faasmctl_path = join(GEN_PROTO_DIR, proto_file)
+        proto_faasmsctl_path = join(GEN_PROTO_DIR, proto_file)
 
         docker_cp_cmd = "docker cp {}:{} {}".format(
-            tmp_ctr_name, proto_ctr_path, proto_faasmctl_path
+            tmp_ctr_name, proto_ctr_path, proto_faasmsctl_path
         )
         run(docker_cp_cmd, shell=True, check=True)
 
     # Delete container
     run("docker rm -f {}".format(tmp_ctr_name), shell=True, check=True)
     print("Done generating protobuf files!")
```

### Comparing `faasmsctl-0.0.2/faasmsctl/tasks/cli.py` & `faasmsctl-0.0.3/faasmsctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/tasks/delete.py` & `faasmsctl-0.0.3/faasmsctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/tasks/deploy.py` & `faasmsctl-0.0.3/faasmsctl/tasks/deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         )
         mount_source = True
 
         # If mounting the source code, we need to populate the host's
         # sysroot to mount it into the containers
         populate_host_sysroot(faasm_checkout)
     else:
-        # Otherwise, we will check out the code in a faasmctl-specific working
+        # Otherwise, we will check out the code in a faasmsctl-specific working
         # directoy
         mount_source = False
         faasm_checkout, faasm_ver = fetch_faasm_code(force=clean)
 
     return deploy_compose_cluster(faasm_checkout, workers, mount_source, ini_file)
```

### Comparing `faasmsctl-0.0.2/faasmsctl/tasks/flush.py` & `faasmsctl-0.0.3/faasmsctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/tasks/invoke.py` & `faasmsctl-0.0.3/faasmsctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/tasks/logs.py` & `faasmsctl-0.0.3/faasmsctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/tasks/monitor.py` & `faasmsctl-0.0.3/faasmsctl/tasks/monitor.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/tasks/restart.py` & `faasmsctl-0.0.3/faasmsctl/tasks/restart.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/tasks/status.py` & `faasmsctl-0.0.3/faasmsctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/tasks/upload.py` & `faasmsctl-0.0.3/faasmsctl/tasks/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     Arguments:
     - user (str): user to register the function with
     - func (str): name to register the function with
     - ini_file (str): optional path to the INI file
     """
     # Directly call the util function so that it uses the same code than the
-    # API consumers (i.e. using faasmctl in a python script)
+    # API consumers (i.e. using faasmsctl in a python script)
     upload_wasm(user, func, wasm_file, ini_file)
 
 
 @task()
 def file(ctx, host_path, faasm_path, ini_file=None):
     """
     Upload a file to Faasm's distributed filesystem
@@ -28,9 +28,9 @@
 
     Parameters:
     - host_path (str): path in the host system to read the file from
     - faasm_path (str): path in the Faasm file system to store the file to
     - ini_file (str): path to the cluster's INI file
     """
     # Directly call the util function so that it uses the same code than the
-    # API consumers (i.e. using faasmctl in a python script)
+    # API consumers (i.e. using faasmsctl in a python script)
     upload_file(host_path, faasm_path, ini_file)
```

### Comparing `faasmsctl-0.0.2/faasmsctl/util/compose.py` & `faasmsctl-0.0.3/faasmsctl/util/compose.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/util/config.py` & `faasmsctl-0.0.3/faasmsctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/util/deploy.py` & `faasmsctl-0.0.3/faasmsctl/util/deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from os.path import abspath, exists, join
 from shutil import rmtree
 from subprocess import CalledProcessError, run
 
 
 def _check_version_mismatch(checkout_path):
     # Check if there's a mismatch between the checked-out code version and
-    # faasmctl's pinned faasm version
+    # faasmsctl's pinned faasm version
     with open(join(checkout_path, "VERSION"), "r") as fh:
         faasm_ver = fh.read()
         faasm_ver = faasm_ver.strip()
     if faasm_ver != get_faasm_version():
         print(
             "WARNING: mismatch between the checked-out version and"
-            " faasmctl's pinned faasm version ({} != {}) using {}".format(
+            " faasmsctl's pinned faasm version ({} != {}) using {}".format(
                 faasm_ver, get_faasm_version(), faasm_ver
             )
         )
 
     return faasm_ver
```

### Comparing `faasmsctl-0.0.2/faasmsctl/util/docker.py` & `faasmsctl-0.0.3/faasmsctl/util/docker.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 ]
 
 
 def in_docker():
     """
     Work-out wether we are being called from inside a docker container
 
-    faasmctl can be invoked both from outside and inside a docker container.
-    When invoked from inside a docker container, faasmctl can only be used to
+    faasmsctl can be invoked both from outside and inside a docker container.
+    When invoked from inside a docker container, faasmsctl can only be used to
     interact with a cluster running on docker compose. In that case, we need to
     use a different IP for the services in the cluster. Fortunately, Faasm
     sets certain env. vars when running inside a container. This function
     checks for them and returns True if successful
     """
     for env_var in IN_DOCKER_ENV_VARS:
         if env_var in environ and environ[env_var] == "on":
```

### Comparing `faasmsctl-0.0.2/faasmsctl/util/faasm.py` & `faasmsctl-0.0.3/faasmsctl/util/faasm.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 FAASM_VERSION = "0.17.0"
 
 
 def get_version():
     """
     Get the Faasm version to check-out the source from
 
-    Faasmctl ships with a default Faasm version (`FAASM_VERSION` in this file)
+    faasmsctl ships with a default Faasm version (`FAASM_VERSION` in this file)
     but it also supports overwriting its value by setting the env. variable
     FAASM_VERSION
 
     Returns:
     - A string with the corresponding Faasm version
     """
     if "FAASM_VERSION" in environ:
```

### Comparing `faasmsctl-0.0.2/faasmsctl/util/flush.py` & `faasmsctl-0.0.3/faasmsctl/util/flush.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/util/gen_proto/faabric_pb2.py` & `faasmsctl-0.0.3/faasmsctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/util/gen_proto/planner_pb2.py` & `faasmsctl-0.0.3/faasmsctl/util/gen_proto/planner_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/util/invoke.py` & `faasmsctl-0.0.3/faasmsctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/util/k8s.py` & `faasmsctl-0.0.3/faasmsctl/util/k8s.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/util/network.py` & `faasmsctl-0.0.3/faasmsctl/util/network.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/util/planner.py` & `faasmsctl-0.0.3/faasmsctl/util/planner.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/util/results.py` & `faasmsctl-0.0.3/faasmsctl/util/results.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl/util/upload.py` & `faasmsctl-0.0.3/faasmsctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/faasmsctl.egg-info/PKG-INFO` & `faasmsctl-0.0.3/faasmsctl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmsctl
-Version: 0.0.2
+Version: 0.0.3
 Summary: Command line tool to deploy, manage, and interact with Faasm Stream
 Author-email: Faasm Team <foo@bar.com>, Tianyu <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `faasmsctl-0.0.2/faasmsctl.egg-info/SOURCES.txt` & `faasmsctl-0.0.3/faasmsctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faasmsctl-0.0.2/pyproject.toml` & `faasmsctl-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmsctl"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
   { name="Tianyu", email="foo@bar.com"}
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm Stream"
 readme = "README.md"
 requires-python = ">=3.7"
@@ -23,8 +23,8 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/faasm/faasmctl"
 "Bug Tracker" = "https://github.com/faasm/faasmctl/issues"
 
 [project.scripts]
-faasmsctl = "faasmctl.main:main"
+faasmsctl = "faasmsctl.main:main"
```

