# Comparing `tmp/pulumi_kafka-3.8.0a1715089862.tar.gz` & `tmp/pulumi_kafka-3.8.0a1715233851.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kafka-3.8.0a1715089862.tar", last modified: Tue May  7 13:53:31 2024, max compression
+gzip compressed data, was "pulumi_kafka-3.8.0a1715233851.tar", last modified: Thu May  9 05:54:22 2024, max compression
```

## Comparing `pulumi_kafka-3.8.0a1715089862.tar` & `pulumi_kafka-3.8.0a1715233851.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:53:31.666741 pulumi_kafka-3.8.0a1715089862/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-07 13:53:31.666741 pulumi_kafka-3.8.0a1715089862/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:53:31.662741 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23117 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/acl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:53:31.666741 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/get_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    31331 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka/user_scram_credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 13:53:31.666741 pulumi_kafka-3.8.0a1715089862/pulumi_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-07 13:53:31.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-07 13:53:31.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 13:53:31.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-07 13:53:31.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 13:53:31.000000 pulumi_kafka-3.8.0a1715089862/pulumi_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-07 13:53:25.000000 pulumi_kafka-3.8.0a1715089862/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 13:53:31.666741 pulumi_kafka-3.8.0a1715089862/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:54:22.151376 pulumi_kafka-3.8.0a1715233851/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-09 05:54:22.151376 pulumi_kafka-3.8.0a1715233851/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2995 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:54:22.147376 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23117 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/acl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:54:22.151376 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/get_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31331 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka/user_scram_credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:54:22.151376 pulumi_kafka-3.8.0a1715233851/pulumi_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-09 05:54:22.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-09 05:54:22.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:54:22.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 05:54:22.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 05:54:22.000000 pulumi_kafka-3.8.0a1715233851/pulumi_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-09 05:54:15.000000 pulumi_kafka-3.8.0a1715233851/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:54:22.151376 pulumi_kafka-3.8.0a1715233851/setup.cfg
```

### Comparing `pulumi_kafka-3.8.0a1715089862/PKG-INFO` & `pulumi_kafka-3.8.0a1715233851/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kafka
-Version: 3.8.0a1715089862
+Version: 3.8.0a1715233851
 Summary: A Pulumi package for creating and managing Kafka.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi,kafka
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.8.0a1715089862/README.md` & `pulumi_kafka-3.8.0a1715233851/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715089862/pulumi_kafka/__init__.py` & `pulumi_kafka-3.8.0a1715233851/pulumi_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715089862/pulumi_kafka/_utilities.py` & `pulumi_kafka-3.8.0a1715233851/pulumi_kafka/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715089862/pulumi_kafka/acl.py` & `pulumi_kafka-3.8.0a1715233851/pulumi_kafka/acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715089862/pulumi_kafka/config/__init__.pyi` & `pulumi_kafka-3.8.0a1715233851/pulumi_kafka/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715089862/pulumi_kafka/config/vars.py` & `pulumi_kafka-3.8.0a1715233851/pulumi_kafka/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715089862/pulumi_kafka/get_topic.py` & `pulumi_kafka-3.8.0a1715233851/pulumi_kafka/get_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715089862/pulumi_kafka/provider.py` & `pulumi_kafka-3.8.0a1715233851/pulumi_kafka/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715089862/pulumi_kafka/quota.py` & `pulumi_kafka-3.8.0a1715233851/pulumi_kafka/quota.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715089862/pulumi_kafka/topic.py` & `pulumi_kafka-3.8.0a1715233851/pulumi_kafka/topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715089862/pulumi_kafka/user_scram_credential.py` & `pulumi_kafka-3.8.0a1715233851/pulumi_kafka/user_scram_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715089862/pulumi_kafka.egg-info/PKG-INFO` & `pulumi_kafka-3.8.0a1715233851/pulumi_kafka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kafka
-Version: 3.8.0a1715089862
+Version: 3.8.0a1715233851
 Summary: A Pulumi package for creating and managing Kafka.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-kafka
 Keywords: pulumi,kafka
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_kafka-3.8.0a1715089862/pulumi_kafka.egg-info/SOURCES.txt` & `pulumi_kafka-3.8.0a1715233851/pulumi_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kafka-3.8.0a1715089862/pyproject.toml` & `pulumi_kafka-3.8.0a1715233851/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kafka"
   description = "A Pulumi package for creating and managing Kafka."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "kafka"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.8.0a1715089862"
+  version = "3.8.0a1715233851"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-kafka"
 
 [build-system]
```

