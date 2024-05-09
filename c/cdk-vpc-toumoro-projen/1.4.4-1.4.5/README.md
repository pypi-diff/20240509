# Comparing `tmp/cdk-vpc-toumoro-projen-1.4.4.tar.gz` & `tmp/cdk-vpc-toumoro-projen-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-vpc-toumoro-projen-1.4.4.tar", last modified: Wed May  8 17:58:29 2024, max compression
+gzip compressed data, was "cdk-vpc-toumoro-projen-1.4.5.tar", last modified: Thu May  9 13:43:48 2024, max compression
```

## Comparing `cdk-vpc-toumoro-projen-1.4.4.tar` & `cdk-vpc-toumoro-projen-1.4.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:58:29.943760 cdk-vpc-toumoro-projen-1.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-08 17:58:19.000000 cdk-vpc-toumoro-projen-1.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 17:58:19.000000 cdk-vpc-toumoro-projen-1.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 17:58:29.943760 cdk-vpc-toumoro-projen-1.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 17:58:19.000000 cdk-vpc-toumoro-projen-1.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-08 17:58:19.000000 cdk-vpc-toumoro-projen-1.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 17:58:29.943760 cdk-vpc-toumoro-projen-1.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-08 17:58:19.000000 cdk-vpc-toumoro-projen-1.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:58:29.939760 cdk-vpc-toumoro-projen-1.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:58:29.939760 cdk-vpc-toumoro-projen-1.4.4/src/cdk-vpc-toumoro-projen/
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-08 17:58:19.000000 cdk-vpc-toumoro-projen-1.4.4/src/cdk-vpc-toumoro-projen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:58:29.943760 cdk-vpc-toumoro-projen-1.4.4/src/cdk-vpc-toumoro-projen/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-08 17:58:19.000000 cdk-vpc-toumoro-projen-1.4.4/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30660 2024-05-08 17:58:19.000000 cdk-vpc-toumoro-projen-1.4.4/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpc-toumoro-projen@1.4.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:58:19.000000 cdk-vpc-toumoro-projen-1.4.4/src/cdk-vpc-toumoro-projen/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 17:58:29.943760 cdk-vpc-toumoro-projen-1.4.4/src/cdk_vpc_toumoro_projen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-08 17:58:29.000000 cdk-vpc-toumoro-projen-1.4.4/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-08 17:58:29.000000 cdk-vpc-toumoro-projen-1.4.4/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 17:58:29.000000 cdk-vpc-toumoro-projen-1.4.4/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-08 17:58:29.000000 cdk-vpc-toumoro-projen-1.4.4/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-08 17:58:29.000000 cdk-vpc-toumoro-projen-1.4.4/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:43:48.719408 cdk-vpc-toumoro-projen-1.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-09 13:43:38.000000 cdk-vpc-toumoro-projen-1.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 13:43:38.000000 cdk-vpc-toumoro-projen-1.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 13:43:48.719408 cdk-vpc-toumoro-projen-1.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-09 13:43:38.000000 cdk-vpc-toumoro-projen-1.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-09 13:43:38.000000 cdk-vpc-toumoro-projen-1.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:43:48.719408 cdk-vpc-toumoro-projen-1.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-09 13:43:38.000000 cdk-vpc-toumoro-projen-1.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:43:48.715408 cdk-vpc-toumoro-projen-1.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:43:48.719408 cdk-vpc-toumoro-projen-1.4.5/src/cdk-vpc-toumoro-projen/
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-09 13:43:38.000000 cdk-vpc-toumoro-projen-1.4.5/src/cdk-vpc-toumoro-projen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:43:48.719408 cdk-vpc-toumoro-projen-1.4.5/src/cdk-vpc-toumoro-projen/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-09 13:43:38.000000 cdk-vpc-toumoro-projen-1.4.5/src/cdk-vpc-toumoro-projen/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27340 2024-05-09 13:43:38.000000 cdk-vpc-toumoro-projen-1.4.5/src/cdk-vpc-toumoro-projen/_jsii/cdk-vpc-toumoro-projen@1.4.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:43:38.000000 cdk-vpc-toumoro-projen-1.4.5/src/cdk-vpc-toumoro-projen/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:43:48.719408 cdk-vpc-toumoro-projen-1.4.5/src/cdk_vpc_toumoro_projen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-09 13:43:48.000000 cdk-vpc-toumoro-projen-1.4.5/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-09 13:43:48.000000 cdk-vpc-toumoro-projen-1.4.5/src/cdk_vpc_toumoro_projen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:43:48.000000 cdk-vpc-toumoro-projen-1.4.5/src/cdk_vpc_toumoro_projen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 13:43:48.000000 cdk-vpc-toumoro-projen-1.4.5/src/cdk_vpc_toumoro_projen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 13:43:48.000000 cdk-vpc-toumoro-projen-1.4.5/src/cdk_vpc_toumoro_projen.egg-info/top_level.txt
```

### Comparing `cdk-vpc-toumoro-projen-1.4.4/LICENSE` & `cdk-vpc-toumoro-projen-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-vpc-toumoro-projen-1.4.4/PKG-INFO` & `cdk-vpc-toumoro-projen-1.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-toumoro-projen
-Version: 1.4.4
+Version: 1.4.5
 Summary: A CDK construct library to create a VPC with public and private subnets.
 Home-page: https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-vpc-toumoro-projen-1.4.4/setup.py` & `cdk-vpc-toumoro-projen-1.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-vpc-toumoro-projen",
-    "version": "1.4.4",
+    "version": "1.4.5",
     "description": "A CDK construct library to create a VPC with public and private subnets.",
     "license": "GPL-3.0-or-later",
     "url": "https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git",
     "long_description_content_type": "text/markdown",
     "author": "tm-lcarvalho<lucio.carvalho@toumoro.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk-vpc-toumoro-projen",
         "cdk-vpc-toumoro-projen._jsii"
     ],
     "package_data": {
         "cdk-vpc-toumoro-projen._jsii": [
-            "cdk-vpc-toumoro-projen@1.4.4.jsii.tgz"
+            "cdk-vpc-toumoro-projen@1.4.5.jsii.tgz"
         ],
         "cdk-vpc-toumoro-projen": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-vpc-toumoro-projen-1.4.4/src/cdk-vpc-toumoro-projen/__init__.py` & `cdk-vpc-toumoro-projen-1.4.5/src/cdk-vpc-toumoro-projen/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "natGateways"))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, IVpcBase).__jsii_proxy_class__ = lambda : _IVpcBaseProxy
 
 
 class VpcBase(
-    _aws_cdk_aws_ec2_ceddda9d.Vpc,
+    _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-vpc-toumoro-projen.VpcBase",
 ):
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
```

### Comparing `cdk-vpc-toumoro-projen-1.4.4/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO` & `cdk-vpc-toumoro-projen-1.4.5/src/cdk_vpc_toumoro_projen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-vpc-toumoro-projen
-Version: 1.4.4
+Version: 1.4.5
 Summary: A CDK construct library to create a VPC with public and private subnets.
 Home-page: https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-vpc-toumoro-projen.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

