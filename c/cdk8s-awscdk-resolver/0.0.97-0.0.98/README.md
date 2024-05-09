# Comparing `tmp/cdk8s-awscdk-resolver-0.0.97.tar.gz` & `tmp/cdk8s-awscdk-resolver-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-awscdk-resolver-0.0.97.tar", last modified: Mon May  6 12:22:46 2024, max compression
+gzip compressed data, was "cdk8s-awscdk-resolver-0.0.98.tar", last modified: Thu May  9 06:13:44 2024, max compression
```

## Comparing `cdk8s-awscdk-resolver-0.0.97.tar` & `cdk8s-awscdk-resolver-0.0.98.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:22:46.586800 cdk8s-awscdk-resolver-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-06 12:22:31.000000 cdk8s-awscdk-resolver-0.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-06 12:22:31.000000 cdk8s-awscdk-resolver-0.0.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-06 12:22:46.586800 cdk8s-awscdk-resolver-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-06 12:22:31.000000 cdk8s-awscdk-resolver-0.0.97/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-06 12:22:31.000000 cdk8s-awscdk-resolver-0.0.97/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:22:46.586800 cdk8s-awscdk-resolver-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-06 12:22:31.000000 cdk8s-awscdk-resolver-0.0.97/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:22:46.582800 cdk8s-awscdk-resolver-0.0.97/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:22:46.582800 cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver/
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-06 12:22:31.000000 cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:22:46.582800 cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-06 12:22:31.000000 cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   977553 2024-05-06 12:22:31.000000 cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.97.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:22:31.000000 cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:22:46.582800 cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-06 12:22:46.000000 cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-06 12:22:46.000000 cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:22:46.000000 cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 12:22:46.000000 cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 12:22:46.000000 cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:13:44.467697 cdk8s-awscdk-resolver-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-09 06:13:44.467697 cdk8s-awscdk-resolver-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:13:44.467697 cdk8s-awscdk-resolver-0.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:13:44.463698 cdk8s-awscdk-resolver-0.0.98/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:13:44.463698 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:13:44.463698 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   981048 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.98.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:13:32.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:13:44.463698 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-09 06:13:44.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-09 06:13:44.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:13:44.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 06:13:44.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-09 06:13:44.000000 cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/top_level.txt
```

### Comparing `cdk8s-awscdk-resolver-0.0.97/LICENSE` & `cdk8s-awscdk-resolver-0.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.97/PKG-INFO` & `cdk8s-awscdk-resolver-0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-awscdk-resolver
-Version: 0.0.97
+Version: 0.0.98
 Summary: @cdk8s/awscdk-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-awscdk-resolver-0.0.97/README.md` & `cdk8s-awscdk-resolver-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.97/setup.py` & `cdk8s-awscdk-resolver-0.0.98/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-awscdk-resolver",
-    "version": "0.0.97",
+    "version": "0.0.98",
     "description": "@cdk8s/awscdk-resolver",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk8s_awscdk_resolver",
         "cdk8s_awscdk_resolver._jsii"
     ],
     "package_data": {
         "cdk8s_awscdk_resolver._jsii": [
-            "awscdk-resolver@0.0.97.jsii.tgz"
+            "awscdk-resolver@0.0.98.jsii.tgz"
         ],
         "cdk8s_awscdk_resolver": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver/__init__.py` & `cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver/_jsii/__init__.py` & `cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import cdk8s._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdk8s/awscdk-resolver",
-    "0.0.97",
+    "0.0.98",
     __name__[0:-6],
-    "awscdk-resolver@0.0.97.jsii.tgz",
+    "awscdk-resolver@0.0.98.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.97.jsii.tgz` & `cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver/_jsii/awscdk-resolver@0.0.98.jsii.tgz`

 * *Files 24% similar despite different names*

#### Comparing `awscdk-resolver@0.0.97.jsii.tgz-content` & `awscdk-resolver@0.0.98.jsii.tgz-content`

##### file list

```diff
@@ -684,59 +684,59 @@
 -rw-r--r--   0        0        0      361 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/client-sts/dist-es/commands/index.js
 -rw-r--r--   0        0        0      213 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/client-sts/dist-es/index.js
 -rw-r--r--   0        0        0       28 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/client-sts/dist-es/models/index.js
 -rw-r--r--   0        0        0       40 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-cjs/client/index.js
 -rw-r--r--   0        0        0       43 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-cjs/httpAuthSchemes/aws_sdk/index.js
 -rw-r--r--   0        0        0       40 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-cjs/httpAuthSchemes/index.js
 -rw-r--r--   0        0        0       43 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-cjs/httpAuthSchemes/utils/index.js
--rw-r--r--   0        0        0    15823 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-cjs/index.js
+-rw-r--r--   0        0        0    15837 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-cjs/index.js
 -rw-r--r--   0        0        0       40 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-cjs/protocols/index.js
 -rw-r--r--   0        0        0       51 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-es/client/index.js
 -rw-r--r--   0        0        0       81 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-es/httpAuthSchemes/aws_sdk/index.js
 -rw-r--r--   0        0        0       27 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-es/httpAuthSchemes/index.js
 -rw-r--r--   0        0        0      120 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-es/httpAuthSchemes/utils/index.js
 -rw-r--r--   0        0        0      108 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-es/index.js
 -rw-r--r--   0        0        0      153 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-es/protocols/index.js
 -rw-r--r--   0        0        0     2508 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-env/dist-cjs/index.js
 -rw-r--r--   0        0        0       27 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-env/dist-es/index.js
 -rw-r--r--   0        0        0      269 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-http/dist-cjs/index.js
 -rw-r--r--   0        0        0       48 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-http/dist-es/index.js
--rw-r--r--   0        0        0    10128 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-ini/dist-cjs/index.js
+-rw-r--r--   0        0        0    10142 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-ini/dist-cjs/index.js
 -rw-r--r--   0        0        0       27 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-ini/dist-es/index.js
--rw-r--r--   0        0        0     6283 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-node/dist-cjs/index.js
+-rw-r--r--   0        0        0     6297 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-node/dist-cjs/index.js
 -rw-r--r--   0        0        0       35 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-node/dist-es/index.js
--rw-r--r--   0        0        0     4025 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-process/dist-cjs/index.js
+-rw-r--r--   0        0        0     4039 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-process/dist-cjs/index.js
 -rw-r--r--   0        0        0       31 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-process/dist-es/index.js
--rw-r--r--   0        0        0     8031 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-sso/dist-cjs/index.js
+-rw-r--r--   0        0        0     8063 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-sso/dist-cjs/index.js
 -rw-r--r--   0        0        0      122 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-sso/dist-es/index.js
 -rw-r--r--   0        0        0     1152 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-web-identity/dist-cjs/index.js
 -rw-r--r--   0        0        0       65 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-web-identity/dist-es/index.js
 -rw-r--r--   0        0        0     2664 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-host-header/dist-cjs/index.js
 -rw-r--r--   0        0        0     1176 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-host-header/dist-es/index.js
 -rw-r--r--   0        0        0     3122 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-logger/dist-cjs/index.js
 -rw-r--r--   0        0        0       36 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-logger/dist-es/index.js
 -rw-r--r--   0        0        0     2767 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-recursion-detection/dist-cjs/index.js
 -rw-r--r--   0        0        0     1287 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-recursion-detection/dist-es/index.js
--rw-r--r--   0        0        0     4753 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-user-agent/dist-cjs/index.js
+-rw-r--r--   0        0        0     4767 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-user-agent/dist-cjs/index.js
 -rw-r--r--   0        0        0       75 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-user-agent/dist-es/index.js
 -rw-r--r--   0        0        0       40 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/region-config-resolver/dist-cjs/extensions/index.js
--rw-r--r--   0        0        0     4205 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/region-config-resolver/dist-cjs/index.js
+-rw-r--r--   0        0        0     4219 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/region-config-resolver/dist-cjs/index.js
 -rw-r--r--   0        0        0       40 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/region-config-resolver/dist-cjs/regionConfig/index.js
 -rw-r--r--   0        0        0      748 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/region-config-resolver/dist-es/extensions/index.js
 -rw-r--r--   0        0        0       62 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/region-config-resolver/dist-es/index.js
 -rw-r--r--   0        0        0       65 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/region-config-resolver/dist-es/regionConfig/index.js
--rw-r--r--   0        0        0     8424 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/token-providers/dist-cjs/index.js
+-rw-r--r--   0        0        0     8438 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/token-providers/dist-cjs/index.js
 -rw-r--r--   0        0        0       89 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/token-providers/dist-es/index.js
 -rw-r--r--   0        0        0       40 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/dist-cjs/extensions/index.js
 -rw-r--r--   0        0        0       40 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/dist-cjs/identity/index.js
 -rw-r--r--   0        0        0    11879 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/dist-cjs/index.js
 -rw-r--r--   0        0        0       11 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/dist-es/extensions/index.js
 -rw-r--r--   0        0        0      172 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/dist-es/identity/index.js
 -rw-r--r--   0        0        0      867 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/dist-es/index.js
--rw-r--r--   0        0        0    11556 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-endpoints/dist-cjs/index.js
+-rw-r--r--   0        0        0    11570 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-endpoints/dist-cjs/index.js
 -rw-r--r--   0        0        0       43 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-endpoints/dist-cjs/lib/aws/index.js
 -rw-r--r--   0        0        0       40 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-endpoints/dist-cjs/types/index.js
 -rw-r--r--   0        0        0      155 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-endpoints/dist-es/index.js
 -rw-r--r--   0        0        0      102 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-endpoints/dist-es/lib/aws/index.js
 -rw-r--r--   0        0        0      199 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-endpoints/dist-es/types/index.js
 -rw-r--r--   0        0        0     1368 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-locate-window/dist-cjs/index.js
 -rw-r--r--   0        0        0      230 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-locate-window/dist-es/index.js
@@ -1527,25 +1527,25 @@
 -rw-r--r--   0        0        0     3731 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/client-cloudformation/package.json
 -rw-r--r--   0        0        0     3564 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/client-sso-oidc/package.json
 -rw-r--r--   0        0        0     3444 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/client-sso/package.json
 -rw-r--r--   0        0        0     3644 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/client-sts/package.json
 -rw-r--r--   0        0        0     1835 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/package.json
 -rw-r--r--   0        0        0     1778 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-env/package.json
 -rw-r--r--   0        0        0     2049 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-http/package.json
--rw-r--r--   0        0        0     2169 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-ini/package.json
+-rw-r--r--   0        0        0     2168 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-ini/package.json
 -rw-r--r--   0        0        0     2252 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-node/package.json
 -rw-r--r--   0        0        0     1858 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-process/package.json
 -rw-r--r--   0        0        0     1928 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-sso/package.json
 -rw-r--r--   0        0        0     2078 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/credential-provider-web-identity/package.json
 -rw-r--r--   0        0        0     1642 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-host-header/package.json
 -rw-r--r--   0        0        0     1650 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-logger/package.json
 -rw-r--r--   0        0        0     1674 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-recursion-detection/package.json
 -rw-r--r--   0        0        0     1747 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/middleware-user-agent/package.json
 -rw-r--r--   0        0        0     1759 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/region-config-resolver/package.json
--rw-r--r--   0        0        0     1922 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/token-providers/package.json
+-rw-r--r--   0        0        0     1921 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/token-providers/package.json
 -rwxr-xr-x   0        0        0     1597 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/package.json
 -rw-r--r--   0        0        0     1675 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-endpoints/package.json
 -rw-r--r--   0        0        0     1498 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-locate-window/package.json
 -rw-r--r--   0        0        0     1613 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-user-agent-browser/package.json
 -rw-r--r--   0        0        0     1750 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-user-agent-node/package.json
 -rw-r--r--   0        0        0     1478 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-utf8-browser/package.json
 -rw-r--r--   0        0        0     2000 1985-10-26 08:15:00.000000 package/node_modules/@smithy/abort-controller/package.json
@@ -1629,15 +1629,15 @@
 -rw-r--r--   0        0        0     1959 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/sha256-browser/build/webCryptoSha256.js.map
 -rw-r--r--   0        0        0     6527 1985-10-26 08:15:00.000000 package/API.md
 -rw-r--r--   0        0        0     3300 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/ie11-detection/CHANGELOG.md
 -rw-r--r--   0        0        0     6169 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/sha256-browser/CHANGELOG.md
 -rw-r--r--   0        0        0     5971 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/sha256-js/CHANGELOG.md
 -rw-r--r--   0        0        0     3370 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/supports-web-crypto/CHANGELOG.md
 -rw-r--r--   0        0        0     2672 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/util/CHANGELOG.md
--rw-r--r--   0        0        0     7916 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/CHANGELOG.md
+-rw-r--r--   0        0        0     8067 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/CHANGELOG.md
 -rw-r--r--   0        0        0     7228 1985-10-26 08:15:00.000000 package/node_modules/bowser/CHANGELOG.md
 -rw-r--r--   0        0        0    19905 1985-10-26 08:15:00.000000 package/node_modules/fast-xml-parser/CHANGELOG.md
 -rw-r--r--   0        0        0    16207 1985-10-26 08:15:00.000000 package/node_modules/uuid/CHANGELOG.md
 -rw-r--r--   0        0        0      149 1985-10-26 08:15:00.000000 package/CODE_OF_CONDUCT.md
 -rw-r--r--   0        0        0      513 1985-10-26 08:15:00.000000 package/node_modules/uuid/CONTRIBUTING.md
 -rw-r--r--   0        0        0     1109 1985-10-26 08:15:00.000000 package/node_modules/uuid/LICENSE.md
 -rw-r--r--   0        0        0      307 1985-10-26 08:15:00.000000 package/git-hooks/README.md
@@ -2039,15 +2039,15 @@
 -rw-r--r--   0        0        0     1369 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/client-cloudformation/dist-types/ts3.4/commands/DetectStackSetDriftCommand.d.ts
 -rw-r--r--   0        0        0     2559 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/dist-types/dns.d.ts
 -rw-r--r--   0        0        0      481 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/dist-types/ts3.4/dns.d.ts
 -rw-r--r--   0        0        0      255 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-types/client/emitWarningIfUnsupportedVersion.d.ts
 -rw-r--r--   0        0        0       81 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-types/ts3.4/client/emitWarningIfUnsupportedVersion.d.ts
 -rw-r--r--   0        0        0      236 1985-10-26 08:15:00.000000 package/node_modules/@smithy/smithy-client/dist-types/emitWarningIfUnsupportedVersion.d.ts
 -rw-r--r--   0        0        0      244 1985-10-26 08:15:00.000000 package/node_modules/@smithy/smithy-client/dist-types/ts3.4/emitWarningIfUnsupportedVersion.d.ts
--rw-r--r--   0        0        0     2615 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/src/client/emitWarningIfUnsupportedVersion.spec.ts
+-rw-r--r--   0        0        0     2620 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/src/client/emitWarningIfUnsupportedVersion.spec.ts
 -rw-r--r--   0        0        0      907 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/src/client/emitWarningIfUnsupportedVersion.ts
 -rw-r--r--   0        0        0      101 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/dist-types/encode.d.ts
 -rw-r--r--   0        0        0      110 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/dist-types/ts3.4/encode.d.ts
 -rw-r--r--   0        0        0      558 1985-10-26 08:15:00.000000 package/node_modules/@smithy/types/dist-types/encode.d.ts
 -rw-r--r--   0        0        0      577 1985-10-26 08:15:00.000000 package/node_modules/@smithy/types/dist-types/ts3.4/encode.d.ts
 -rw-r--r--   0        0        0      153 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/dist-types/endpoint.d.ts
 -rw-r--r--   0        0        0      167 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/types/dist-types/ts3.4/endpoint.d.ts
@@ -2844,15 +2844,15 @@
 -rw-r--r--   0        0        0     1807 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/src/protocols/json/parseJsonBody.ts
 -rw-r--r--   0        0        0      470 1985-10-26 08:15:00.000000 package/node_modules/@smithy/shared-ini-file-loader/dist-types/parseKnownFiles.d.ts
 -rw-r--r--   0        0        0      485 1985-10-26 08:15:00.000000 package/node_modules/@smithy/shared-ini-file-loader/dist-types/ts3.4/parseKnownFiles.d.ts
 -rw-r--r--   0        0        0      224 1985-10-26 08:15:00.000000 package/node_modules/@smithy/util-endpoints/dist-types/lib/parseURL.d.ts
 -rw-r--r--   0        0        0      229 1985-10-26 08:15:00.000000 package/node_modules/@smithy/util-endpoints/dist-types/ts3.4/lib/parseURL.d.ts
 -rw-r--r--   0        0        0      346 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-types/protocols/xml/parseXmlBody.d.ts
 -rw-r--r--   0        0        0      359 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/dist-types/ts3.4/protocols/xml/parseXmlBody.d.ts
--rw-r--r--   0        0        0     1847 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/src/protocols/xml/parseXmlBody.spec.ts
+-rw-r--r--   0        0        0     1857 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/src/protocols/xml/parseXmlBody.spec.ts
 -rw-r--r--   0        0        0     2010 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/src/protocols/xml/parseXmlBody.ts
 -rw-r--r--   0        0        0     1148 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-endpoints/dist-types/lib/aws/partition.d.ts
 -rw-r--r--   0        0        0      726 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/util-endpoints/dist-types/ts3.4/lib/aws/partition.d.ts
 -rw-r--r--   0        0        0      431 1985-10-26 08:15:00.000000 package/node_modules/@smithy/config-resolver/dist-types/regionInfo/PartitionHash.d.ts
 -rw-r--r--   0        0        0      445 1985-10-26 08:15:00.000000 package/node_modules/@smithy/config-resolver/dist-types/ts3.4/regionInfo/PartitionHash.d.ts
 -rw-r--r--   0        0        0      660 1985-10-26 08:15:00.000000 package/node_modules/@smithy/util-waiter/dist-types/poller.d.ts
 -rw-r--r--   0        0        0      670 1985-10-26 08:15:00.000000 package/node_modules/@smithy/util-waiter/dist-types/ts3.4/poller.d.ts
@@ -3253,17 +3253,17 @@
 -rw-r--r--   0        0        0      964 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/client-cloudformation/dist-types/waiters/waitForTypeRegistrationComplete.d.ts
 -rw-r--r--   0        0        0      302 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/sha256-browser/build/webCryptoSha256.d.ts
 -rw-r--r--   0        0        0     1875 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/sha256-browser/src/webCryptoSha256.ts
 -rw-r--r--   0        0        0      585 1985-10-26 08:15:00.000000 package/node_modules/@smithy/node-http-handler/dist-types/ts3.4/write-request-body.d.ts
 -rw-r--r--   0        0        0      604 1985-10-26 08:15:00.000000 package/node_modules/@smithy/node-http-handler/dist-types/write-request-body.d.ts
 -rw-r--r--   0        0        0      158 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/token-providers/dist-types/ts3.4/writeSSOTokenToFile.d.ts
 -rw-r--r--   0        0        0      249 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/token-providers/dist-types/writeSSOTokenToFile.d.ts
--rw-r--r--   0        0        0    55282 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/tsconfig.cjs.tsbuildinfo
--rw-r--r--   0        0        0    55282 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/tsconfig.es.tsbuildinfo
--rw-r--r--   0        0        0    56128 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/tsconfig.types.tsbuildinfo
+-rw-r--r--   0        0        0    59923 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/tsconfig.cjs.tsbuildinfo
+-rw-r--r--   0        0        0    59086 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/tsconfig.es.tsbuildinfo
+-rw-r--r--   0        0        0    61005 1985-10-26 08:15:00.000000 package/node_modules/@aws-sdk/core/tsconfig.types.tsbuildinfo
 -rw-r--r--   0        0        0      824 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/ie11-detection/node_modules/tslib/CopyrightNotice.txt
 -rw-r--r--   0        0        0      824 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/sha256-browser/node_modules/tslib/CopyrightNotice.txt
 -rw-r--r--   0        0        0      824 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/sha256-js/node_modules/tslib/CopyrightNotice.txt
 -rw-r--r--   0        0        0      824 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/supports-web-crypto/node_modules/tslib/CopyrightNotice.txt
 -rw-r--r--   0        0        0      824 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/util/node_modules/tslib/CopyrightNotice.txt
 -rw-r--r--   0        0        0      822 1985-10-26 08:15:00.000000 package/node_modules/tslib/CopyrightNotice.txt
 -rw-r--r--   0        0        0      655 1985-10-26 08:15:00.000000 package/node_modules/@aws-crypto/ie11-detection/node_modules/tslib/LICENSE.txt
```

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9305555555555556%*

 * *Differences: {"'bundled'": "{'@aws-sdk/client-cloudformation': '^3.572.0'}",*

 * * "'fingerprint'": "'NPiiq87YlbBOmYTtNxlWUo0rhtHrJh0J+LKDpRwTh7g='",*

 * * "'version'": "'0.0.98'"}*

```diff
@@ -3,15 +3,15 @@
         "name": "Amazon Web Services",
         "roles": [
             "author"
         ],
         "url": "https://aws.amazon.com"
     },
     "bundled": {
-        "@aws-sdk/client-cloudformation": "^3.569.0"
+        "@aws-sdk/client-cloudformation": "^3.572.0"
     },
     "dependencies": {
         "aws-cdk-lib": "^2.106.1",
         "cdk8s": "^2.68.3",
         "constructs": "^10.3.0"
     },
     "dependencyClosure": {
@@ -3580,15 +3580,15 @@
             }
         }
     },
     "description": "@cdk8s/awscdk-resolver",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "dwgfthUp9p4b98qW3TKPBVLltd8sRpLrCJsT+V51Lcs=",
+    "fingerprint": "NPiiq87YlbBOmYTtNxlWUo0rhtHrJh0J+LKDpRwTh7g=",
     "homepage": "https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git",
     "jsiiVersion": "5.4.12 (build bc82b08)",
     "license": "Apache-2.0",
     "metadata": {
         "jsii": {
             "pacmak": {
                 "hasDefaultInterfaces": true
@@ -3671,9 +3671,9 @@
                     ]
                 }
             ],
             "name": "AwsCdkResolver",
             "symbolId": "src/resolve:AwsCdkResolver"
         }
     },
-    "version": "0.0.97"
+    "version": "0.0.98"
 }
```

##### package/node_modules/@aws-sdk/core/dist-cjs/index.js

###### js-beautify {}

```diff
@@ -1,7 +1,8 @@
+"use strict";
 var __defProp = Object.defineProperty;
 var __getOwnPropDesc = Object.getOwnPropertyDescriptor;
 var __getOwnPropNames = Object.getOwnPropertyNames;
 var __hasOwnProp = Object.prototype.hasOwnProperty;
 var __name = (target, value) => __defProp(target, "name", {
     value,
     configurable: true
```

##### package/node_modules/@aws-sdk/credential-provider-ini/dist-cjs/index.js

###### js-beautify {}

```diff
@@ -1,7 +1,8 @@
+"use strict";
 var __create = Object.create;
 var __defProp = Object.defineProperty;
 var __getOwnPropDesc = Object.getOwnPropertyDescriptor;
 var __getOwnPropNames = Object.getOwnPropertyNames;
 var __getProtoOf = Object.getPrototypeOf;
 var __hasOwnProp = Object.prototype.hasOwnProperty;
 var __name = (target, value) => __defProp(target, "name", {
```

##### package/node_modules/@aws-sdk/credential-provider-node/dist-cjs/index.js

###### js-beautify {}

```diff
@@ -1,7 +1,8 @@
+"use strict";
 var __create = Object.create;
 var __defProp = Object.defineProperty;
 var __getOwnPropDesc = Object.getOwnPropertyDescriptor;
 var __getOwnPropNames = Object.getOwnPropertyNames;
 var __getProtoOf = Object.getPrototypeOf;
 var __hasOwnProp = Object.prototype.hasOwnProperty;
 var __name = (target, value) => __defProp(target, "name", {
```

##### package/node_modules/@aws-sdk/credential-provider-process/dist-cjs/index.js

###### js-beautify {}

```diff
@@ -1,7 +1,8 @@
+"use strict";
 var __defProp = Object.defineProperty;
 var __getOwnPropDesc = Object.getOwnPropertyDescriptor;
 var __getOwnPropNames = Object.getOwnPropertyNames;
 var __hasOwnProp = Object.prototype.hasOwnProperty;
 var __name = (target, value) => __defProp(target, "name", {
     value,
     configurable: true
```

##### package/node_modules/@aws-sdk/credential-provider-sso/dist-cjs/index.js

###### js-beautify {}

```diff
@@ -1,7 +1,8 @@
+"use strict";
 var __defProp = Object.defineProperty;
 var __getOwnPropDesc = Object.getOwnPropertyDescriptor;
 var __getOwnPropNames = Object.getOwnPropertyNames;
 var __hasOwnProp = Object.prototype.hasOwnProperty;
 var __name = (target, value) => __defProp(target, "name", {
     value,
     configurable: true
@@ -36,14 +37,15 @@
 __export(loadSso_exports, {
     GetRoleCredentialsCommand: () => import_client_sso.GetRoleCredentialsCommand,
     SSOClient: () => import_client_sso.SSOClient
 });
 var import_client_sso;
 var init_loadSso = __esm({
     "src/loadSso.ts"() {
+        "use strict";
         import_client_sso = require("@aws-sdk/client-sso");
     }
 });
 
 // src/index.ts
 var src_exports = {};
 __export(src_exports, {
```

##### package/node_modules/@aws-sdk/middleware-user-agent/dist-cjs/index.js

###### js-beautify {}

```diff
@@ -1,7 +1,8 @@
+"use strict";
 var __defProp = Object.defineProperty;
 var __getOwnPropDesc = Object.getOwnPropertyDescriptor;
 var __getOwnPropNames = Object.getOwnPropertyNames;
 var __hasOwnProp = Object.prototype.hasOwnProperty;
 var __name = (target, value) => __defProp(target, "name", {
     value,
     configurable: true
```

##### package/node_modules/@aws-sdk/region-config-resolver/dist-cjs/index.js

###### js-beautify {}

```diff
@@ -1,7 +1,8 @@
+"use strict";
 var __defProp = Object.defineProperty;
 var __getOwnPropDesc = Object.getOwnPropertyDescriptor;
 var __getOwnPropNames = Object.getOwnPropertyNames;
 var __hasOwnProp = Object.prototype.hasOwnProperty;
 var __name = (target, value) => __defProp(target, "name", {
     value,
     configurable: true
```

##### package/node_modules/@aws-sdk/token-providers/dist-cjs/index.js

###### js-beautify {}

```diff
@@ -1,7 +1,8 @@
+"use strict";
 var __create = Object.create;
 var __defProp = Object.defineProperty;
 var __getOwnPropDesc = Object.getOwnPropertyDescriptor;
 var __getOwnPropNames = Object.getOwnPropertyNames;
 var __getProtoOf = Object.getPrototypeOf;
 var __hasOwnProp = Object.prototype.hasOwnProperty;
 var __name = (target, value) => __defProp(target, "name", {
```

##### package/node_modules/@aws-sdk/util-endpoints/dist-cjs/index.js

###### js-beautify {}

```diff
@@ -1,7 +1,8 @@
+"use strict";
 var __defProp = Object.defineProperty;
 var __getOwnPropDesc = Object.getOwnPropertyDescriptor;
 var __getOwnPropNames = Object.getOwnPropertyNames;
 var __hasOwnProp = Object.prototype.hasOwnProperty;
 var __name = (target, value) => __defProp(target, "name", {
     value,
     configurable: true
```

##### package/lib/resolve.js

###### js-beautify {}

```diff
@@ -63,10 +63,10 @@
         }).toString().trim());
     }
 }
 exports.AwsCdkResolver = AwsCdkResolver;
 _a = JSII_RTTI_SYMBOL_1;
 AwsCdkResolver[_a] = {
     fqn: "@cdk8s/awscdk-resolver.AwsCdkResolver",
-    version: "0.0.97"
+    version: "0.0.98"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoicmVzb2x2ZS5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3NyYy9yZXNvbHZlLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7Ozs7O0FBQUEsaURBQTZDO0FBQzdDLDZCQUE2QjtBQUM3Qiw2Q0FBK0U7QUFJL0UsTUFBYSxjQUFjO0lBRWxCLE9BQU8sQ0FBQyxPQUEwQjtRQUV2QyxJQUFJLENBQUMsbUJBQUssQ0FBQyxZQUFZLENBQUMsT0FBTyxDQUFDLEtBQUssQ0FBQyxFQUFFLENBQUM7WUFDdkMsT0FBTztRQUNULENBQUM7UUFFRCxJQUFJLE9BQU8sT0FBTyxDQUFDLEtBQUssS0FBSyxRQUFRLEVBQUUsQ0FBQztZQUN0QywrREFBK0Q7WUFDL0QsbUJBQW1CO1lBQ25CLE1BQU0sSUFBSSxLQUFLLENBQUMsdUJBQXVCLE9BQU0sQ0FBQyxPQUFPLENBQUMsS0FBSyxDQUFDLHNCQUFzQixDQUFDLENBQUM7UUFDdEYsQ0FBQztRQUVELE1BQU0sTUFBTSxHQUFHLElBQUksQ0FBQyxVQUFVLENBQUMsT0FBTyxDQUFDLEtBQUssQ0FBQyxDQUFDO1FBQzlDLElBQUksQ0FBQztZQUNILE1BQU0sV0FBVyxHQUFHLElBQUksQ0FBQyxnQkFBZ0IsQ0FBQyxNQUFNLENBQUMsQ0FBQztZQUNsRCxPQUFPLENBQUMsWUFBWSxDQUFDLFdBQVcsQ0FBQyxDQUFDO1FBQ3BDLENBQUM7UUFBQyxPQUFPLEdBQUcsRUFBRSxDQUFDO1lBQ2IsMkVBQTJFO1lBQzNFLGtFQUFrRTtZQUNsRSwyRUFBMkU7WUFDM0UsK0VBQStFO1lBQy9FLCtDQUErQztZQUMvQyxPQUFPLENBQUMsWUFBWSxDQUFDLG9DQUFvQyxNQUFNLENBQUMsSUFBSSxDQUFDLElBQUksS0FBSyxHQUFHLEVBQUUsQ0FBQyxDQUFDO1FBQ3ZGLENBQUM7SUFFSCxDQUFDO0lBRU8sVUFBVSxDQUFDLEtBQWE7UUFFOUIsTUFBTSxlQUFlLEdBQVksRUFBRSxDQUFDO1FBRXBDLEtBQUssTUFBTSxLQUFLLElBQUksMEJBQVksQ0FBQyxhQUFhLENBQUMsS0FBSyxDQUFDLENBQUMsTUFBTSxFQUFFLENBQUM7WUFDN0QsSUFBSSx1QkFBUyxDQUFDLFdBQVcsQ0FBQyxLQUFLLENBQUMsRUFBRSxDQUFDO2dCQUNqQyxNQUFNLEtBQUssR0FBRyxtQkFBSyxDQUFDLEVBQUUsQ0FBQyxLQUFLLENBQUMsTUFBTSxDQUFDLENBQUM7Z0JBQ3JDLGVBQWUsQ0FBQyxJQUFJLENBQUMsS0FBSyxDQUFDLENBQUM7Z0JBQzVCLE1BQU0sTUFBTSxHQUFHLEtBQUssQ0FBQyxJQUFJLENBQUMsT0FBTyxFQUFFLENBQUMsTUFBTSxDQUFDLENBQUMsQ0FBQyxFQUFFLENBQUMsQ0FBQyxZQUFZLHVCQUFTLElBQUksQ0FBQyxDQUFDLEtBQUssS0FBSyxLQUFLLENBQUMsQ0FBQyxDQUFDLENBQWMsQ0FBQztnQkFDN0csa0ZBQWtGO2dCQUNsRix3REFBd0Q7Z0JBQ3hELElBQUksTUFBTTtvQkFBRSxPQUFPLE1BQU0sQ0FBQztZQUM1QixDQUFDO1FBQ0gsQ0FBQztRQUVELDZCQUE2QjtRQUM3Qiw2QkFBNkI7UUFDN0Isb0NBQW9DO1FBQ3BDLG9GQUFvRjtRQUNwRiwrREFBK0Q7UUFDL0QsTUFBTSxJQUFJLEtBQUssQ0FBQyxxQ0FBcUMsS0FBSyx1QkFBdUIsZUFBZSxDQUFDLEdBQUcsQ0FBQyxDQUFDLENBQUMsRUFBRSxDQUFDLENBQUMsQ0FBQyxTQUFTLENBQUMsQ0FBQyxJQUFJLENBQUMsR0FBRyxDQUFDLEdBQUcsQ0FBQyxDQUFDO0lBRXZJLENBQUM7SUFFTyxnQkFBZ0IsQ0FBQyxNQUFpQjtRQUV4QyxNQUFNLE1BQU0sR0FBRyxJQUFJLENBQUMsSUFBSSxDQUFDLFNBQVMsRUFBRSxJQUFJLEVBQUUsS0FBSyxFQUFFLHVCQUF1QixDQUFDLENBQUM7UUFDMUUsT0FBTyxJQUFJLENBQUMsS0FBSyxDQUFDLElBQUEsNEJBQVksRUFBQyxPQUFPLENBQUMsUUFBUSxFQUFFO1lBQy9DLE1BQU07WUFDTixtQkFBSyxDQUFDLEVBQUUsQ0FBQyxNQUFNLENBQUMsQ0FBQyxTQUFTO1lBQzFCLE1BQU0sQ0FBQyxJQUFJLENBQUMsRUFBRTtTQUNmLEVBQUUsRUFBRSxRQUFRLEVBQUUsT0FBTyxFQUFFLEtBQUssRUFBRSxDQUFDLE1BQU0sQ0FBQyxFQUFFLENBQUMsQ0FBQyxRQUFRLEVBQUUsQ0FBQyxJQUFJLEVBQUUsQ0FBQyxDQUFDO0lBRWhFLENBQUM7O0FBOURILHdDQWdFQyIsInNvdXJjZXNDb250ZW50IjpbImltcG9ydCB7IGV4ZWNGaWxlU3luYyB9IGZyb20gJ2NoaWxkX3Byb2Nlc3MnO1xuaW1wb3J0ICogYXMgcGF0aCBmcm9tICdwYXRoJztcbmltcG9ydCB7IFRva2VuLCBTdGFjaywgVG9rZW5pemF0aW9uLCBSZWZlcmVuY2UsIENmbk91dHB1dCB9IGZyb20gJ2F3cy1jZGstbGliJztcbmltcG9ydCB7IElSZXNvbHZlciwgUmVzb2x1dGlvbkNvbnRleHQgfSBmcm9tICdjZGs4cyc7XG5cblxuZXhwb3J0IGNsYXNzIEF3c0Nka1Jlc29sdmVyIGltcGxlbWVudHMgSVJlc29sdmVyIHtcblxuICBwdWJsaWMgcmVzb2x2ZShjb250ZXh0OiBSZXNvbHV0aW9uQ29udGV4dCkge1xuXG4gICAgaWYgKCFUb2tlbi5pc1VucmVzb2x2ZWQoY29udGV4dC52YWx1ZSkpIHtcbiAgICAgIHJldHVybjtcbiAgICB9XG5cbiAgICBpZiAodHlwZW9mIGNvbnRleHQudmFsdWUgIT09ICdzdHJpbmcnKSB7XG4gICAgICAvLyBzaG91bGQgYmUgb2sgYmVjYXVzZSB3ZSBvbmx5IHJlc29sdmUgQ2ZuT3V0cHV0IHZhbHVlcywgd2hpY2hcbiAgICAgIC8vIG11c3QgYmUgc3RyaW5ncy5cbiAgICAgIHRocm93IG5ldyBFcnJvcihgSW52YWxpZCB2YWx1ZSB0eXBlOiAke3R5cGVvZihjb250ZXh0LnZhbHVlKX0gKEV4cGVjdGVkICdzdHJpbmcnKWApO1xuICAgIH1cblxuICAgIGNvbnN0IG91dHB1dCA9IHRoaXMuZmluZE91dHB1dChjb250ZXh0LnZhbHVlKTtcbiAgICB0cnkge1xuICAgICAgY29uc3Qgb3V0cHV0VmFsdWUgPSB0aGlzLmZldGNoT3V0cHV0VmFsdWUob3V0cHV0KTtcbiAgICAgIGNvbnRleHQucmVwbGFjZVZhbHVlKG91dHB1dFZhbHVlKTtcbiAgICB9IGNhdGNoIChlcnIpIHtcbiAgICAgIC8vIGlmIGJvdGggY2RrOHMgYW5kIEFXUyBDREsgYXBwbGljYXRpb25zIGFyZSBkZWZpbmVkIHdpdGhpbiB0aGUgc2FtZSBmaWxlLFxuICAgICAgLy8gYSBjZGs4cyBzeW50aCBpcyBnb2luZyB0byBoYXBwZW4gYmVmb3JlIHRoZSBBV1MgQ0RLIGRlcGxveW1lbnQuXG4gICAgICAvLyBpbiB0aGlzIGNhc2Ugd2UgbXVzdCBzd2FsbG93IHRoZSBlcnJvciwgb3RoZXJ3aXNlIHRoZSBBV1MgQ0RLIGRlcGxveW1lbnRcbiAgICAgIC8vIHdvbid0IGJlIGFibGUgdG8gZ28gdGhyb3VnaC4gd2UgcmVwbGFjZSB0aGUgdmFsdWUgd2l0aCBzb21ldGhpbmcgdG8gaW5kaWNhdGVcbiAgICAgIC8vIHRoYXQgYSBmZXRjaGluZyBhdHRlbXB0IHdhcyBtYWRlIGFuZCBmYWlsZWQuXG4gICAgICBjb250ZXh0LnJlcGxhY2VWYWx1ZShgRmFpbGVkIGZldGNoaW5nIHZhbHVlIGZvciBvdXRwdXQgJHtvdXRwdXQubm9kZS5wYXRofTogJHtlcnJ9YCk7XG4gICAgfVxuXG4gIH1cblxuICBwcml2YXRlIGZpbmRPdXRwdXQodmFsdWU6IHN0cmluZykge1xuXG4gICAgY29uc3QgaW5zcGVjdGVkU3RhY2tzOiBTdGFja1tdID0gW107XG5cbiAgICBmb3IgKGNvbnN0IHRva2VuIG9mIFRva2VuaXphdGlvbi5yZXZlcnNlU3RyaW5nKHZhbHVlKS50b2tlbnMpIHtcbiAgICAgIGlmIChSZWZlcmVuY2UuaXNSZWZlcmVuY2UodG9rZW4pKSB7XG4gICAgICAgIGNvbnN0IHN0YWNrID0gU3RhY2sub2YodG9rZW4udGFyZ2V0KTtcbiAgICAgICAgaW5zcGVjdGVkU3RhY2tzLnB1c2goc3RhY2spO1xuICAgICAgICBjb25zdCBvdXRwdXQgPSBzdGFjay5ub2RlLmZpbmRBbGwoKS5maWx0ZXIoYyA9PiBjIGluc3RhbmNlb2YgQ2ZuT3V0cHV0ICYmIGMudmFsdWUgPT09IHZhbHVlKVswXSBhcyBDZm5PdXRwdXQ7XG4gICAgICAgIC8vIHdlIGRvbid0IHJlYWxseSBjYXJlIGlmIHRoZXJlIGFyZSBtb3JlIG91dHB1dHMgKHBvc3NpYmx5IGZyb20gZGlmZmVyZW50IHN0YWNrcylcbiAgICAgICAgLy8gdGhhdCBwb2ludCB0byB0aGUgc2FtZSB2YWx1ZS4gdGhlIGZpcnN0IHdpbGwgc3VmZmljZS5cbiAgICAgICAgaWYgKG91dHB1dCkgcmV0dXJuIG91dHB1dDtcbiAgICAgIH1cbiAgICB9XG5cbiAgICAvLyBUaGlzIGNhbiBoYXBwZW4gaWYgZWl0aGVyOlxuICAgIC8vIC0tLS0tLS0tLS0tLS0tLS0tLS0tLS0tLS0tXG4gICAgLy8gIDEuIFVzZXIgZGlkbid0IGRlZmluZSBhbiBvdXRwdXQuXG4gICAgLy8gIDIuIE91dHB1dCB3YXMgZGVmaW5lZCBpbiBhIGRpZmZlcmVudCBzdGFjayB0aGFuIHRoZSB0b2tlbnMgY29tcHJpc2luZyBpdHMgdmFsdWUuXG4gICAgLy8gIDMuIE5vbmUgb2YgdGhlIHRva2VucyBjb21wcmlzaW5nIHRoZSB2YWx1ZSBhcmUgYSBSZWZlcmVuY2UuXG4gICAgdGhyb3cgbmV3IEVycm9yKGBVbmFibGUgdG8gZmluZCBvdXRwdXQgZGVmaW5lZCBmb3IgJHt2YWx1ZX0gKEluc3BlY3RlZCBzdGFja3M6ICR7aW5zcGVjdGVkU3RhY2tzLm1hcChzID0+IHMuc3RhY2tOYW1lKS5qb2luKCcsJyl9KWApO1xuXG4gIH1cblxuICBwcml2YXRlIGZldGNoT3V0cHV0VmFsdWUob3V0cHV0OiBDZm5PdXRwdXQpIHtcblxuICAgIGNvbnN0IHNjcmlwdCA9IHBhdGguam9pbihfX2Rpcm5hbWUsICcuLicsICdsaWInLCAnZmV0Y2gtb3V0cHV0LXZhbHVlLmpzJyk7XG4gICAgcmV0dXJuIEpTT04ucGFyc2UoZXhlY0ZpbGVTeW5jKHByb2Nlc3MuZXhlY1BhdGgsIFtcbiAgICAgIHNjcmlwdCxcbiAgICAgIFN0YWNrLm9mKG91dHB1dCkuc3RhY2tOYW1lLFxuICAgICAgb3V0cHV0Lm5vZGUuaWQsXG4gICAgXSwgeyBlbmNvZGluZzogJ3V0Zi04Jywgc3RkaW86IFsncGlwZSddIH0pLnRvU3RyaW5nKCkudHJpbSgpKTtcblxuICB9XG5cbn1cbiJdfQ==
```

##### package/node_modules/@aws-sdk/client-cloudformation/package.json

###### Pretty-printed

 * *Similarity: 0.9715422276621788%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/client-sso-oidc': '3.572.0', '@aws-sdk/client-sts': '3.572.0', "*

 * *                   "'@aws-sdk/core': '3.572.0', '@aws-sdk/credential-provider-node': '3.572.0', "*

 * *                   "'@aws-sdk/middleware-user-agent': '3.572.0', "*

 * *                   "'@aws-sdk/region-config-resolver': '3.572.0', '@aws-sdk/util-endpoints': "*

 * *                   "'3.572.0'}",*

 * * "'version'": "'3.572.0'"}*

```diff
@@ -5,25 +5,25 @@
     },
     "browser": {
         "./dist-es/runtimeConfig": "./dist-es/runtimeConfig.browser"
     },
     "dependencies": {
         "@aws-crypto/sha256-browser": "3.0.0",
         "@aws-crypto/sha256-js": "3.0.0",
-        "@aws-sdk/client-sso-oidc": "3.569.0",
-        "@aws-sdk/client-sts": "3.569.0",
-        "@aws-sdk/core": "3.567.0",
-        "@aws-sdk/credential-provider-node": "3.569.0",
+        "@aws-sdk/client-sso-oidc": "3.572.0",
+        "@aws-sdk/client-sts": "3.572.0",
+        "@aws-sdk/core": "3.572.0",
+        "@aws-sdk/credential-provider-node": "3.572.0",
         "@aws-sdk/middleware-host-header": "3.567.0",
         "@aws-sdk/middleware-logger": "3.568.0",
         "@aws-sdk/middleware-recursion-detection": "3.567.0",
-        "@aws-sdk/middleware-user-agent": "3.567.0",
-        "@aws-sdk/region-config-resolver": "3.567.0",
+        "@aws-sdk/middleware-user-agent": "3.572.0",
+        "@aws-sdk/region-config-resolver": "3.572.0",
         "@aws-sdk/types": "3.567.0",
-        "@aws-sdk/util-endpoints": "3.567.0",
+        "@aws-sdk/util-endpoints": "3.572.0",
         "@aws-sdk/util-user-agent-browser": "3.567.0",
         "@aws-sdk/util-user-agent-node": "3.568.0",
         "@smithy/config-resolver": "^2.2.0",
         "@smithy/core": "^1.4.2",
         "@smithy/fetch-http-handler": "^2.5.0",
         "@smithy/hash-node": "^2.2.0",
         "@smithy/invalid-dependency": "^2.2.0",
@@ -96,9 +96,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.569.0"
+    "version": "3.572.0"
 }
```

##### package/node_modules/@aws-sdk/client-sso-oidc/package.json

###### Pretty-printed

 * *Similarity: 0.9717105263157894%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/client-sts': '3.572.0', '@aws-sdk/core': '3.572.0', "*

 * *                   "'@aws-sdk/credential-provider-node': '3.572.0', "*

 * *                   "'@aws-sdk/middleware-user-agent': '3.572.0', "*

 * *                   "'@aws-sdk/region-config-resolver': '3.572.0', '@aws-sdk/util-endpoints': "*

 * *                   "'3.572.0'}",*

 * * "'version'": "'3.572.0'"}*

```diff
@@ -5,24 +5,24 @@
     },
     "browser": {
         "./dist-es/runtimeConfig": "./dist-es/runtimeConfig.browser"
     },
     "dependencies": {
         "@aws-crypto/sha256-browser": "3.0.0",
         "@aws-crypto/sha256-js": "3.0.0",
-        "@aws-sdk/client-sts": "3.569.0",
-        "@aws-sdk/core": "3.567.0",
-        "@aws-sdk/credential-provider-node": "3.569.0",
+        "@aws-sdk/client-sts": "3.572.0",
+        "@aws-sdk/core": "3.572.0",
+        "@aws-sdk/credential-provider-node": "3.572.0",
         "@aws-sdk/middleware-host-header": "3.567.0",
         "@aws-sdk/middleware-logger": "3.568.0",
         "@aws-sdk/middleware-recursion-detection": "3.567.0",
-        "@aws-sdk/middleware-user-agent": "3.567.0",
-        "@aws-sdk/region-config-resolver": "3.567.0",
+        "@aws-sdk/middleware-user-agent": "3.572.0",
+        "@aws-sdk/region-config-resolver": "3.572.0",
         "@aws-sdk/types": "3.567.0",
-        "@aws-sdk/util-endpoints": "3.567.0",
+        "@aws-sdk/util-endpoints": "3.572.0",
         "@aws-sdk/util-user-agent-browser": "3.567.0",
         "@aws-sdk/util-user-agent-node": "3.568.0",
         "@smithy/config-resolver": "^2.2.0",
         "@smithy/core": "^1.4.2",
         "@smithy/fetch-http-handler": "^2.5.0",
         "@smithy/hash-node": "^2.2.0",
         "@smithy/invalid-dependency": "^2.2.0",
@@ -92,9 +92,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.569.0"
+    "version": "3.572.0"
 }
```

##### package/node_modules/@aws-sdk/client-sso/package.json

###### Pretty-printed

 * *Similarity: 0.9722991689750692%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/core': '3.572.0', '@aws-sdk/middleware-user-agent': '3.572.0', "*

 * *                   "'@aws-sdk/region-config-resolver': '3.572.0', '@aws-sdk/util-endpoints': "*

 * *                   "'3.572.0'}",*

 * * "'version'": "'3.572.0'"}*

```diff
@@ -5,22 +5,22 @@
     },
     "browser": {
         "./dist-es/runtimeConfig": "./dist-es/runtimeConfig.browser"
     },
     "dependencies": {
         "@aws-crypto/sha256-browser": "3.0.0",
         "@aws-crypto/sha256-js": "3.0.0",
-        "@aws-sdk/core": "3.567.0",
+        "@aws-sdk/core": "3.572.0",
         "@aws-sdk/middleware-host-header": "3.567.0",
         "@aws-sdk/middleware-logger": "3.568.0",
         "@aws-sdk/middleware-recursion-detection": "3.567.0",
-        "@aws-sdk/middleware-user-agent": "3.567.0",
-        "@aws-sdk/region-config-resolver": "3.567.0",
+        "@aws-sdk/middleware-user-agent": "3.572.0",
+        "@aws-sdk/region-config-resolver": "3.572.0",
         "@aws-sdk/types": "3.567.0",
-        "@aws-sdk/util-endpoints": "3.567.0",
+        "@aws-sdk/util-endpoints": "3.572.0",
         "@aws-sdk/util-user-agent-browser": "3.567.0",
         "@aws-sdk/util-user-agent-node": "3.568.0",
         "@smithy/config-resolver": "^2.2.0",
         "@smithy/core": "^1.4.2",
         "@smithy/fetch-http-handler": "^2.5.0",
         "@smithy/hash-node": "^2.2.0",
         "@smithy/invalid-dependency": "^2.2.0",
@@ -90,9 +90,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.568.0"
+    "version": "3.572.0"
 }
```

##### package/node_modules/@aws-sdk/client-sts/package.json

###### Pretty-printed

 * *Similarity: 0.9717105263157894%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/client-sso-oidc': '3.572.0', '@aws-sdk/core': '3.572.0', "*

 * *                   "'@aws-sdk/credential-provider-node': '3.572.0', "*

 * *                   "'@aws-sdk/middleware-user-agent': '3.572.0', "*

 * *                   "'@aws-sdk/region-config-resolver': '3.572.0', '@aws-sdk/util-endpoints': "*

 * *                   "'3.572.0'}",*

 * * "'version'": "'3.572.0'"}*

```diff
@@ -5,24 +5,24 @@
     },
     "browser": {
         "./dist-es/runtimeConfig": "./dist-es/runtimeConfig.browser"
     },
     "dependencies": {
         "@aws-crypto/sha256-browser": "3.0.0",
         "@aws-crypto/sha256-js": "3.0.0",
-        "@aws-sdk/client-sso-oidc": "3.569.0",
-        "@aws-sdk/core": "3.567.0",
-        "@aws-sdk/credential-provider-node": "3.569.0",
+        "@aws-sdk/client-sso-oidc": "3.572.0",
+        "@aws-sdk/core": "3.572.0",
+        "@aws-sdk/credential-provider-node": "3.572.0",
         "@aws-sdk/middleware-host-header": "3.567.0",
         "@aws-sdk/middleware-logger": "3.568.0",
         "@aws-sdk/middleware-recursion-detection": "3.567.0",
-        "@aws-sdk/middleware-user-agent": "3.567.0",
-        "@aws-sdk/region-config-resolver": "3.567.0",
+        "@aws-sdk/middleware-user-agent": "3.572.0",
+        "@aws-sdk/region-config-resolver": "3.572.0",
         "@aws-sdk/types": "3.567.0",
-        "@aws-sdk/util-endpoints": "3.567.0",
+        "@aws-sdk/util-endpoints": "3.572.0",
         "@aws-sdk/util-user-agent-browser": "3.567.0",
         "@aws-sdk/util-user-agent-node": "3.568.0",
         "@smithy/config-resolver": "^2.2.0",
         "@smithy/core": "^1.4.2",
         "@smithy/fetch-http-handler": "^2.5.0",
         "@smithy/hash-node": "^2.2.0",
         "@smithy/invalid-dependency": "^2.2.0",
@@ -94,9 +94,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.569.0"
+    "version": "3.572.0"
 }
```

##### package/node_modules/@aws-sdk/core/package.json

###### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'3.572.0'"}*

```diff
@@ -51,9 +51,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.572.0"
 }
```

##### package/node_modules/@aws-sdk/credential-provider-ini/package.json

###### Pretty-printed

 * *Similarity: 0.9555555555555555%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/credential-provider-process': '3.572.0', "*

 * *                   "'@aws-sdk/credential-provider-sso': '3.572.0'}",*

 * * "'peerDependencies'": "{'@aws-sdk/client-sts': '3.572.0'}",*

 * * "'version'": "'3.572.0'"}*

```diff
@@ -1,16 +1,16 @@
 {
     "author": {
         "name": "AWS SDK for JavaScript Team",
         "url": "https://aws.amazon.com/javascript/"
     },
     "dependencies": {
         "@aws-sdk/credential-provider-env": "3.568.0",
-        "@aws-sdk/credential-provider-process": "3.568.0",
-        "@aws-sdk/credential-provider-sso": "3.568.0",
+        "@aws-sdk/credential-provider-process": "3.572.0",
+        "@aws-sdk/credential-provider-sso": "3.572.0",
         "@aws-sdk/credential-provider-web-identity": "3.568.0",
         "@aws-sdk/types": "3.567.0",
         "@smithy/credential-provider-imds": "^2.3.0",
         "@smithy/property-provider": "^2.2.0",
         "@smithy/shared-ini-file-loader": "^2.4.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
@@ -36,15 +36,15 @@
         "credentials"
     ],
     "license": "Apache-2.0",
     "main": "./dist-cjs/index.js",
     "module": "./dist-es/index.js",
     "name": "@aws-sdk/credential-provider-ini",
     "peerDependencies": {
-        "@aws-sdk/client-sts": "^3.568.0"
+        "@aws-sdk/client-sts": "3.572.0"
     },
     "repository": {
         "directory": "packages/credential-provider-ini",
         "type": "git",
         "url": "https://github.com/aws/aws-sdk-js-v3.git"
     },
     "scripts": {
@@ -61,9 +61,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.568.0"
+    "version": "3.572.0"
 }
```

##### package/node_modules/@aws-sdk/credential-provider-node/package.json

###### Pretty-printed

 * *Similarity: 0.9669117647058824%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/credential-provider-ini': '3.572.0', "*

 * *                   "'@aws-sdk/credential-provider-process': '3.572.0', "*

 * *                   "'@aws-sdk/credential-provider-sso': '3.572.0'}",*

 * * "'version'": "'3.572.0'"}*

```diff
@@ -2,17 +2,17 @@
     "author": {
         "name": "AWS SDK for JavaScript Team",
         "url": "https://aws.amazon.com/javascript/"
     },
     "dependencies": {
         "@aws-sdk/credential-provider-env": "3.568.0",
         "@aws-sdk/credential-provider-http": "3.568.0",
-        "@aws-sdk/credential-provider-ini": "3.568.0",
-        "@aws-sdk/credential-provider-process": "3.568.0",
-        "@aws-sdk/credential-provider-sso": "3.568.0",
+        "@aws-sdk/credential-provider-ini": "3.572.0",
+        "@aws-sdk/credential-provider-process": "3.572.0",
+        "@aws-sdk/credential-provider-sso": "3.572.0",
         "@aws-sdk/credential-provider-web-identity": "3.568.0",
         "@aws-sdk/types": "3.567.0",
         "@smithy/credential-provider-imds": "^2.3.0",
         "@smithy/property-provider": "^2.2.0",
         "@smithy/shared-ini-file-loader": "^2.4.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
@@ -61,9 +61,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.569.0"
+    "version": "3.572.0"
 }
```

##### package/node_modules/@aws-sdk/credential-provider-process/package.json

###### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'version'": "'3.572.0'"}*

```diff
@@ -53,9 +53,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.568.0"
+    "version": "3.572.0"
 }
```

##### package/node_modules/@aws-sdk/credential-provider-sso/package.json

###### Pretty-printed

 * *Similarity: 0.9663865546218489%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/client-sso': '3.572.0', '@aws-sdk/token-providers': '3.572.0'}",*

 * * "'version'": "'3.572.0'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": {
         "name": "AWS SDK for JavaScript Team",
         "url": "https://aws.amazon.com/javascript/"
     },
     "dependencies": {
-        "@aws-sdk/client-sso": "3.568.0",
-        "@aws-sdk/token-providers": "3.568.0",
+        "@aws-sdk/client-sso": "3.572.0",
+        "@aws-sdk/token-providers": "3.572.0",
         "@aws-sdk/types": "3.567.0",
         "@smithy/property-provider": "^2.2.0",
         "@smithy/shared-ini-file-loader": "^2.4.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
     },
     "description": "AWS credential provider that exchanges a resolved SSO login token file for temporary AWS credentials",
@@ -55,9 +55,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.568.0"
+    "version": "3.572.0"
 }
```

##### package/node_modules/@aws-sdk/middleware-user-agent/package.json

###### Pretty-printed

 * *Similarity: 0.9633333333333333%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/util-endpoints': '3.572.0'}", "'version'": "'3.572.0'"}*

```diff
@@ -1,15 +1,15 @@
 {
     "author": {
         "name": "AWS SDK for JavaScript Team",
         "url": "https://aws.amazon.com/javascript/"
     },
     "dependencies": {
         "@aws-sdk/types": "3.567.0",
-        "@aws-sdk/util-endpoints": "3.567.0",
+        "@aws-sdk/util-endpoints": "3.572.0",
         "@smithy/protocol-http": "^3.3.0",
         "@smithy/types": "^2.12.0",
         "tslib": "^2.6.2"
     },
     "devDependencies": {
         "@tsconfig/recommended": "1.0.1",
         "concurrently": "7.0.0",
@@ -49,9 +49,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.572.0"
 }
```

##### package/node_modules/@aws-sdk/region-config-resolver/package.json

###### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'3.572.0'"}*

```diff
@@ -50,9 +50,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.572.0"
 }
```

##### package/node_modules/@aws-sdk/token-providers/package.json

###### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'peerDependencies'": "{'@aws-sdk/client-sso-oidc': '3.572.0'}", "'version'": "'3.572.0'"}*

```diff
@@ -32,15 +32,15 @@
         "token"
     ],
     "license": "Apache-2.0",
     "main": "./dist-cjs/index.js",
     "module": "./dist-es/index.js",
     "name": "@aws-sdk/token-providers",
     "peerDependencies": {
-        "@aws-sdk/client-sso-oidc": "^3.568.0"
+        "@aws-sdk/client-sso-oidc": "3.572.0"
     },
     "react-native": {},
     "repository": {
         "directory": "packages/token-providers",
         "type": "git",
         "url": "https://github.com/aws/aws-sdk-js-v3.git"
     },
@@ -60,9 +60,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.568.0"
+    "version": "3.572.0"
 }
```

##### package/node_modules/@aws-sdk/util-endpoints/package.json

###### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'3.572.0'"}*

```diff
@@ -48,9 +48,9 @@
     "typesVersions": {
         "<4.0": {
             "dist-types/*": [
                 "dist-types/ts3.4/*"
             ]
         }
     },
-    "version": "3.567.0"
+    "version": "3.572.0"
 }
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9590643274853801%*

 * *Differences: {"'dependencies'": "{'@aws-sdk/client-cloudformation': '^3.572.0'}",*

 * * "'devDependencies'": "{'@cdk8s/projen-common': '0.0.519', 'cdk8s-cli': '^2.198.113', 'projen': "*

 * *                      "'^0.81.8'}",*

 * * "'version'": "'0.0.98'"}*

```diff
@@ -5,40 +5,40 @@
         "organization": false,
         "url": "https://aws.amazon.com"
     },
     "bundledDependencies": [
         "@aws-sdk/client-cloudformation"
     ],
     "dependencies": {
-        "@aws-sdk/client-cloudformation": "^3.569.0"
+        "@aws-sdk/client-cloudformation": "^3.572.0"
     },
     "devDependencies": {
-        "@cdk8s/projen-common": "0.0.518",
+        "@cdk8s/projen-common": "0.0.519",
         "@types/fs-extra": "^11.0.4",
         "@types/jest": "^27",
         "@types/node": "16.18.78",
         "@typescript-eslint/eslint-plugin": "^6",
         "@typescript-eslint/parser": "^6",
         "aws-cdk": "^2.140.0",
         "aws-cdk-lib": "2.109.0",
         "cdk8s": "2.68.4",
-        "cdk8s-cli": "^2.198.109",
+        "cdk8s-cli": "^2.198.113",
         "constructs": "10.3.0",
         "eslint": "^8",
         "eslint-import-resolver-typescript": "^3.6.1",
         "eslint-plugin-import": "^2.29.1",
         "fs-extra": "^11.2.0",
         "jest": "^27",
         "jest-junit": "^15",
         "jsii": "^5",
         "jsii-diff": "^1.98.0",
         "jsii-docgen": "^9.2.2",
         "jsii-pacmak": "^1.98.0",
         "jsii-rosetta": "^5",
-        "projen": "^0.81.5",
+        "projen": "^0.81.8",
         "standard-version": "^9",
         "ts-jest": "^27",
         "ts-node": "^10.9.2",
         "typescript": "^5.4.5"
     },
     "engines": {
         "node": ">= 16.20.0"
@@ -160,9 +160,9 @@
         "upgrade-configuration": "npx projen upgrade-configuration",
         "upgrade-dev-dependencies": "npx projen upgrade-dev-dependencies",
         "upgrade-runtime-dependencies": "npx projen upgrade-runtime-dependencies",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "0.0.97"
+    "version": "0.0.98"
 }
```

##### package/node_modules/@aws-sdk/core/CHANGELOG.md

```diff
@@ -1,12 +1,20 @@
 # Change Log
 
 All notable changes to this project will be documented in this file.
 See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.
 
+# [3.572.0](https://github.com/aws/aws-sdk-js-v3/compare/v3.571.0...v3.572.0) (2024-05-08)
+
+**Note:** Version bump only for package @aws-sdk/core
+
+
+
+
+
 # [3.567.0](https://github.com/aws/aws-sdk-js-v3/compare/v3.566.0...v3.567.0) (2024-05-01)
 
 
 ### Features
 
 * end support for Node.js 14.x ([#6034](https://github.com/aws/aws-sdk-js-v3/issues/6034)) ([d196411](https://github.com/aws/aws-sdk-js-v3/commit/d19641119f07d62c29f12348f448cd834d841533))
```

##### package/node_modules/@aws-sdk/core/src/client/emitWarningIfUnsupportedVersion.spec.ts

```diff
@@ -1,9 +1,9 @@
 describe("emitWarningIfUnsupportedVersion", () => {
-  let emitWarningIfUnsupportedVersion;
+  let emitWarningIfUnsupportedVersion: any;
   const emitWarning = process.emitWarning;
   const supportedVersion = "16.0.0";
 
   beforeEach(() => {
     const module = require("./emitWarningIfUnsupportedVersion");
     emitWarningIfUnsupportedVersion = module.emitWarningIfUnsupportedVersion;
   });
```

##### package/node_modules/@aws-sdk/core/src/protocols/xml/parseXmlBody.spec.ts

```diff
@@ -39,22 +39,22 @@
       </Bucket>
    </Buckets>
    <Owner>
       <DisplayName>string</DisplayName>
       <ID>string</ID>
    </Owner>
 `);
-    const parsed = await parseXmlBody(xml, context as any as SerdeContext).catch((_) => _);
+    const parsed = await parseXmlBody(xml, context as any as SerdeContext).catch((_: any) => _);
     expect(parsed.toString()).toEqual(`Error: Unclosed tag 'ListAllMyBucketsResult'.:2:1`);
   });
 
   it("should throw on incomplete xml", async () => {
     const xml = Buffer.from(`<?xml version="1.0" encoding="UTF-8"?>
 <ListAllMyBucketsResult>
    <Buckets>
       <Bucket>
          <CreationDate>timestamp</Creatio
 `);
-    const parsed = await parseXmlBody(xml, context as any as SerdeContext).catch((_) => _);
+    const parsed = await parseXmlBody(xml, context as any as SerdeContext).catch((_: any) => _);
     expect(parsed.toString()).toEqual(`Error: Closing tag 'Creatio' doesn't have proper closing.:6:1`);
   });
 });
```

##### package/node_modules/@aws-sdk/core/tsconfig.cjs.tsbuildinfo

###### Pretty-printed

 * *Similarity: 0.9333639155754201%*

 * *Differences: {"'program'": "{'fileNames': {insert: [(5, '../../node_modules/typescript/lib/lib.es2019.d.ts'), "*

 * *              "(6, '../../node_modules/typescript/lib/lib.es2020.d.ts'), (7, "*

 * *              "'../../node_modules/typescript/lib/lib.es2021.d.ts'), (30, "*

 * *              "'../../node_modules/typescript/lib/lib.es2019.array.d.ts'), (31, "*

 * *              "'../../node_modules/typescript/lib/lib.es2019.object.d.ts'), (32, "*

 * *              "'../../node_modules/typescript/lib/lib.es2019.string.d.ts'), (33, "*

 * *           […]*

```diff
@@ -1,1771 +1,1798 @@
 {
     "program": {
         "exportedModulesMap": [
             [
-                208,
+                235,
                 1
             ],
             [
-                212,
+                239,
                 2
             ],
             [
-                195,
+                222,
                 3
             ],
             [
-                196,
+                223,
                 3
             ],
             [
-                194,
+                221,
                 1
             ],
             [
-                197,
+                224,
                 4
             ],
             [
-                199,
+                226,
                 1
             ],
             [
-                198,
+                225,
                 1
             ],
             [
-                200,
+                227,
                 5
             ],
             [
-                209,
+                236,
                 1
             ],
             [
-                211,
+                238,
                 1
             ],
             [
-                210,
+                237,
                 6
             ],
             [
-                201,
+                228,
                 1
             ],
             [
-                202,
+                229,
                 6
             ],
             [
-                203,
+                230,
                 6
             ],
             [
-                205,
+                232,
                 7
             ],
             [
-                204,
+                231,
                 1
             ],
             [
-                207,
+                234,
                 8
             ],
             [
-                206,
+                233,
                 1
             ],
             [
-                159,
+                186,
                 9
             ],
             [
-                161,
+                188,
                 10
             ],
             [
-                160,
+                187,
                 1
             ],
             [
-                162,
+                189,
                 9
             ],
             [
-                163,
+                190,
                 9
             ],
             [
-                164,
+                191,
                 11
             ],
             [
-                157,
+                184,
                 1
             ],
             [
-                145,
+                172,
                 1
             ],
             [
-                146,
+                173,
                 12
             ],
             [
-                143,
+                170,
                 13
             ],
             [
-                144,
+                171,
                 14
             ],
             [
-                142,
+                169,
                 15
             ],
             [
-                140,
+                167,
                 1
             ],
             [
-                141,
+                168,
                 1
             ],
             [
-                149,
+                176,
                 16
             ],
             [
-                148,
+                175,
                 1
             ],
             [
-                213,
+                240,
                 1
             ],
             [
-                219,
+                246,
                 1
             ],
             [
-                214,
+                241,
                 1
             ],
             [
-                215,
+                242,
                 1
             ],
             [
-                216,
+                243,
                 1
             ],
             [
-                220,
+                247,
                 17
             ],
             [
-                217,
+                244,
                 1
             ],
             [
-                218,
+                245,
                 1
             ],
             [
-                150,
+                177,
                 1
             ],
             [
-                151,
+                178,
                 1
             ],
             [
-                156,
+                183,
                 18
             ],
             [
-                165,
+                192,
                 19
             ],
             [
-                167,
+                194,
                 20
             ],
             [
-                176,
+                203,
                 1
             ],
             [
-                172,
+                199,
                 1
             ],
             [
-                174,
+                201,
                 21
             ],
             [
-                175,
+                202,
                 22
             ],
             [
-                173,
+                200,
                 1
             ],
             [
-                187,
+                214,
                 23
             ],
             [
-                47,
+                65,
                 24
             ],
             [
-                48,
+                66,
                 25
             ],
             [
-                45,
+                63,
                 26
             ],
             [
-                46,
+                64,
                 27
             ],
             [
-                49,
+                67,
                 28
             ],
             [
-                96,
+                123,
                 29
             ],
             [
-                98,
+                125,
                 30
             ],
             [
-                100,
+                127,
                 31
             ],
             [
-                99,
+                126,
                 32
             ],
             [
-                105,
+                132,
                 33
             ],
             [
-                103,
+                130,
                 34
             ],
             [
-                107,
+                134,
                 35
             ],
             [
-                38,
+                56,
                 36
             ],
             [
-                109,
+                136,
                 37
             ],
             [
-                110,
+                137,
                 38
             ],
             [
-                112,
+                139,
                 39
             ],
             [
-                111,
+                138,
                 40
             ],
             [
-                113,
+                140,
                 41
             ],
             [
-                108,
+                135,
                 42
             ],
             [
-                106,
+                133,
                 43
             ],
             [
-                114,
+                141,
                 44
             ],
             [
-                115,
+                142,
                 45
             ],
             [
-                119,
+                146,
                 46
             ],
             [
-                120,
+                147,
                 47
             ],
             [
-                118,
+                145,
                 48
             ],
             [
-                95,
+                122,
                 49
             ],
             [
-                41,
+                59,
                 50
             ],
             [
-                121,
+                148,
                 51
             ],
             [
-                122,
+                149,
                 52
             ],
             [
-                123,
+                150,
                 52
             ],
             [
-                125,
+                152,
                 53
             ],
             [
-                124,
+                151,
                 52
             ],
             [
-                139,
+                166,
                 54
             ],
             [
-                44,
+                62,
                 55
             ],
             [
-                126,
+                153,
                 56
             ],
             [
-                117,
+                144,
                 57
             ],
             [
-                128,
+                155,
                 58
             ],
             [
-                116,
+                143,
                 59
             ],
             [
-                129,
+                156,
                 60
             ],
             [
-                130,
+                157,
                 61
             ],
             [
-                131,
+                158,
                 29
             ],
             [
-                132,
+                159,
                 29
             ],
             [
-                133,
+                160,
                 62
             ],
             [
-                135,
+                162,
                 63
             ],
             [
-                136,
+                163,
                 64
             ],
             [
-                137,
+                164,
                 56
             ],
             [
-                40,
+                58,
                 65
             ],
             [
-                43,
+                61,
                 43
             ],
             [
-                138,
+                165,
                 66
             ],
             [
-                153,
+                180,
                 67
             ],
             [
-                155,
+                182,
                 68
             ],
             [
-                154,
+                181,
                 69
             ],
             [
-                242,
+                269,
                 70
             ],
             [
-                236,
+                263,
                 71
             ],
             [
-                234,
+                261,
                 71
             ],
             [
-                239,
+                266,
                 72
             ],
             [
-                237,
+                264,
                 71
             ],
             [
-                241,
+                268,
                 71
             ],
             [
-                244,
+                271,
                 73
             ],
             [
-                245,
+                272,
                 73
             ],
             [
-                246,
+                273,
                 74
             ],
             [
-                251,
+                278,
                 75
             ],
             [
-                250,
+                277,
                 76
             ],
             [
-                252,
+                279,
                 77
             ],
             [
-                253,
+                280,
                 77
             ],
             [
-                255,
+                282,
                 78
             ],
             [
-                256,
+                283,
                 79
             ],
             [
-                265,
+                292,
                 80
             ],
             [
-                260,
+                287,
                 81
             ],
             [
-                264,
+                291,
                 82
             ],
             [
-                262,
+                289,
                 83
             ],
             [
-                263,
+                290,
                 84
             ],
             [
-                261,
+                288,
                 85
             ],
             [
-                280,
+                307,
                 86
             ],
             [
-                281,
+                308,
                 87
             ],
             [
-                284,
+                311,
                 88
             ],
             [
-                285,
+                312,
                 89
             ],
             [
-                283,
+                310,
                 90
             ],
             [
-                286,
+                313,
                 91
             ],
             [
-                287,
+                314,
                 92
             ],
             [
-                288,
+                315,
                 93
             ],
             [
-                289,
+                316,
                 94
             ],
             [
-                290,
+                317,
                 95
             ],
             [
-                291,
+                318,
                 96
             ],
             [
-                292,
+                319,
                 97
             ],
             [
-                293,
+                320,
                 98
             ],
             [
-                294,
+                321,
                 99
             ],
             [
-                295,
+                322,
                 100
             ],
             [
-                50,
+                68,
                 101
             ],
             [
-                52,
+                69,
+                101
+            ],
+            [
+                71,
                 102
             ],
             [
-                53,
+                72,
                 103
             ],
             [
-                54,
+                73,
                 104
             ],
             [
-                55,
+                74,
                 105
             ],
             [
-                56,
+                75,
                 106
             ],
             [
-                57,
+                76,
                 107
             ],
             [
-                58,
+                77,
                 108
             ],
             [
-                59,
+                78,
                 109
             ],
             [
-                60,
+                79,
                 110
             ],
             [
-                61,
+                80,
                 111
             ],
             [
-                62,
+                81,
+                111
+            ],
+            [
+                82,
                 112
             ],
             [
-                63,
+                83,
                 113
             ],
             [
-                64,
+                84,
                 114
             ],
             [
-                65,
+                85,
                 115
             ],
             [
-                66,
+                86,
                 116
             ],
             [
-                67,
+                87,
                 117
             ],
             [
-                93,
+                88,
                 118
             ],
             [
-                68,
+                89,
                 119
             ],
             [
-                69,
+                120,
                 120
             ],
             [
-                70,
+                90,
                 121
             ],
             [
-                71,
+                91,
                 122
             ],
             [
-                72,
+                92,
                 123
             ],
             [
-                73,
+                93,
                 124
             ],
             [
-                74,
+                94,
                 125
             ],
             [
-                75,
+                95,
                 126
             ],
             [
-                76,
+                96,
                 127
             ],
             [
-                77,
+                97,
                 128
             ],
             [
-                78,
+                98,
                 129
             ],
             [
-                79,
+                99,
                 130
             ],
             [
-                80,
+                100,
                 131
             ],
             [
-                81,
+                101,
                 132
             ],
             [
-                82,
+                103,
                 133
             ],
             [
-                83,
+                102,
                 134
             ],
             [
-                84,
+                104,
                 135
             ],
             [
-                85,
+                105,
                 136
             ],
             [
-                86,
+                107,
                 137
             ],
             [
-                87,
+                108,
                 138
             ],
             [
-                88,
+                109,
                 139
             ],
             [
-                89,
+                110,
                 140
             ],
             [
-                90,
+                111,
                 141
             ],
             [
-                91,
+                112,
                 142
             ],
             [
-                325,
+                113,
                 143
             ],
             [
-                326,
+                114,
                 144
             ],
             [
-                301,
+                115,
                 145
             ],
             [
-                304,
-                145
+                116,
+                146
             ],
             [
-                323,
-                143
+                117,
+                147
             ],
             [
-                324,
-                143
+                118,
+                148
             ],
             [
-                314,
-                143
+                352,
+                149
             ],
             [
-                313,
-                146
+                353,
+                150
             ],
             [
-                311,
-                143
+                328,
+                151
             ],
             [
-                306,
-                143
+                331,
+                151
             ],
             [
-                319,
-                143
+                350,
+                149
             ],
             [
-                317,
-                143
+                351,
+                149
             ],
             [
-                321,
-                143
+                341,
+                149
             ],
             [
-                305,
-                143
+                340,
+                152
             ],
             [
-                318,
-                143
+                338,
+                149
             ],
             [
-                322,
-                143
+                333,
+                149
             ],
             [
-                307,
-                143
+                346,
+                149
             ],
             [
-                308,
-                143
+                344,
+                149
             ],
             [
-                320,
-                143
+                348,
+                149
             ],
             [
-                302,
-                143
+                332,
+                149
             ],
             [
-                309,
-                143
+                345,
+                149
             ],
             [
-                310,
-                143
+                349,
+                149
             ],
             [
-                312,
-                143
+                334,
+                149
             ],
             [
-                316,
-                143
+                335,
+                149
             ],
             [
-                327,
-                147
+                347,
+                149
             ],
             [
-                315,
-                143
+                329,
+                149
             ],
             [
-                303,
-                143
+                336,
+                149
             ],
             [
-                340,
-                148
+                337,
+                149
             ],
             [
-                334,
-                147
+                339,
+                149
             ],
             [
-                336,
+                343,
                 149
             ],
             [
-                335,
-                147
+                354,
+                153
             ],
             [
-                328,
-                147
+                342,
+                149
             ],
             [
-                329,
-                147
+                330,
+                149
             ],
             [
-                331,
-                147
+                367,
+                154
             ],
             [
-                333,
-                147
+                361,
+                153
             ],
             [
-                337,
-                149
+                363,
+                155
             ],
             [
-                338,
-                149
+                362,
+                153
             ],
             [
-                330,
-                149
+                355,
+                153
             ],
             [
-                332,
-                149
+                356,
+                153
             ],
             [
-                343,
-                150
+                358,
+                153
             ],
             [
-                345,
-                151
+                360,
+                153
             ],
             [
-                268,
-                152
+                364,
+                155
             ],
             [
-                277,
-                153
+                365,
+                155
             ],
             [
-                267,
-                154
+                357,
+                155
             ],
             [
-                278,
+                359,
                 155
             ],
             [
-                273,
+                370,
                 156
             ],
             [
-                274,
+                372,
                 157
             ],
             [
-                272,
+                295,
                 158
             ],
             [
-                276,
+                304,
                 159
             ],
             [
-                270,
+                294,
                 160
             ],
             [
-                269,
+                305,
                 161
             ],
             [
-                275,
+                300,
                 162
             ],
             [
-                271,
-                153
-            ],
-            [
-                32,
+                301,
                 163
             ],
             [
-                33,
+                299,
                 164
             ],
             [
-                193,
+                303,
                 165
             ],
             [
-                222,
+                297,
                 166
             ],
             [
-                221,
+                296,
                 167
             ],
             [
-                223,
+                302,
                 168
             ],
             [
-                188,
-                169
+                298,
+                159
             ],
             [
-                189,
-                163
+                50,
+                169
             ],
             [
-                191,
+                51,
                 170
             ],
             [
-                192,
+                220,
                 171
             ],
             [
-                190,
+                249,
                 172
             ],
             [
-                231,
+                248,
                 173
             ],
             [
-                224,
-                163
-            ],
-            [
-                226,
+                250,
                 174
             ],
             [
-                230,
+                215,
                 175
             ],
             [
-                225,
+                216,
+                169
+            ],
+            [
+                218,
                 176
             ],
             [
-                227,
+                219,
                 177
             ],
             [
-                229,
+                217,
                 178
+            ],
+            [
+                258,
+                179
+            ],
+            [
+                251,
+                169
+            ],
+            [
+                253,
+                180
+            ],
+            [
+                257,
+                181
+            ],
+            [
+                252,
+                182
+            ],
+            [
+                254,
+                183
+            ],
+            [
+                256,
+                184
             ]
         ],
         "fileIdsList": [
             [
-                139
+                166
             ],
             [
-                197,
-                200,
-                207,
-                208,
-                209,
-                210,
-                211
+                224,
+                227,
+                234,
+                235,
+                236,
+                237,
+                238
             ],
             [
-                139,
-                194
+                166,
+                221
             ],
             [
-                194,
-                195,
-                196
+                221,
+                222,
+                223
             ],
             [
-                198,
-                199
+                225,
+                226
             ],
             [
-                139,
-                149
+                166,
+                176
             ],
             [
-                202,
-                203,
-                204
+                229,
+                230,
+                231
             ],
             [
-                201,
-                205,
-                206
+                228,
+                232,
+                233
             ],
             [
-                139,
-                157,
-                158
+                166,
+                184,
+                185
             ],
             [
-                159,
-                160
+                186,
+                187
             ],
             [
-                157,
-                158,
-                161,
-                162,
-                163
+                184,
+                185,
+                188,
+                189,
+                190
             ],
             [
-                139,
-                145
+                166,
+                172
             ],
             [
-                142
+                169
             ],
             [
-                143
+                170
             ],
             [
-                139,
-                140,
-                141
+                166,
+                167,
+                168
             ],
             [
-                140,
-                141,
-                142,
-                144,
-                145,
-                146,
-                147,
-                148
+                167,
+                168,
+                169,
+                171,
+                172,
+                173,
+                174,
+                175
             ],
             [
-                213,
-                214,
-                215,
-                216,
-                217,
-                218,
-                219
+                240,
+                241,
+                242,
+                243,
+                244,
+                245,
+                246
             ],
             [
-                139,
-                155
+                166,
+                182
             ],
             [
-                139,
-                164
+                166,
+                191
             ],
             [
-                151
+                178
             ],
             [
-                139,
-                172,
-                173
+                166,
+                199,
+                200
             ],
             [
-                174
+                201
             ],
             [
-                139,
-                150,
-                151,
-                156,
-                165,
                 166,
-                167,
-                168,
-                169,
-                170,
-                171,
-                175,
-                176,
                 177,
                 178,
-                179,
-                180,
-                181,
-                182,
                 183,
-                184,
-                185,
-                186
+                192,
+                193,
+                194,
+                195,
+                196,
+                197,
+                198,
+                202,
+                203,
+                204,
+                205,
+                206,
+                207,
+                208,
+                209,
+                210,
+                211,
+                212,
+                213
             ],
             [
-                37,
-                44,
-                45,
-                46
+                55,
+                62,
+                63,
+                64
             ],
             [
-                44,
-                47
+                62,
+                65
             ],
             [
-                37,
-                41
+                55,
+                59
             ],
             [
-                37,
-                47
+                55,
+                65
             ],
             [
-                35,
-                36,
-                45,
-                46,
-                47,
-                48
+                53,
+                54,
+                63,
+                64,
+                65,
+                66
             ],
             [
-                79,
-                93,
-                95
+                101,
+                120,
+                122
             ],
             [
-                97
+                124
             ],
             [
-                42,
-                43,
-                44,
-                99
+                60,
+                61,
+                62,
+                126
             ],
             [
-                42,
-                44
+                60,
+                62
             ],
             [
-                101,
-                103,
-                104
+                128,
+                130,
+                131
             ],
             [
-                101,
-                102
+                128,
+                129
             ],
             [
-                106
+                133
             ],
             [
-                35
+                53
             ],
             [
-                38,
-                108
+                56,
+                135
             ],
             [
-                108
+                135
             ],
             [
-                111
+                138
             ],
             [
-                108,
-                109,
-                110
+                135,
+                136,
+                137
             ],
             [
-                108,
-                109,
-                110,
-                111,
-                112
+                135,
+                136,
+                137,
+                138,
+                139
             ],
             [
-                39
+                57
             ],
             [
-                41,
-                42,
-                44
+                59,
+                60,
+                62
             ],
             [
-                97,
-                98
+                124,
+                125
             ],
             [
-                114
+                141
             ],
             [
-                114,
-                118
+                141,
+                145
             ],
             [
-                114,
-                115,
-                118,
-                119
+                141,
+                142,
+                145,
+                146
             ],
             [
-                43,
-                117
+                61,
+                144
             ],
             [
-                94
+                121
             ],
             [
-                34,
-                40
+                52,
+                58
             ],
             [
-                65,
-                67,
-                93
+                87,
+                89,
+                120
             ],
             [
-                37
+                55
             ],
             [
-                37,
-                122,
-                123,
-                124
+                55,
+                149,
+                150,
+                151
             ],
             [
-                34,
-                38,
-                39,
-                40,
-                41,
-                42,
-                43,
-                44,
-                49,
-                96,
-                97,
-                98,
-                99,
-                100,
-                102,
-                105,
-                106,
-                107,
-                113,
-                116,
-                117,
-                120,
-                121,
+                52,
+                56,
+                57,
+                58,
+                59,
+                60,
+                61,
+                62,
+                67,
+                123,
+                124,
                 125,
                 126,
                 127,
-                128,
                 129,
-                130,
-                131,
                 132,
                 133,
                 134,
-                136,
-                137,
-                138
+                140,
+                143,
+                144,
+                147,
+                148,
+                152,
+                153,
+                154,
+                155,
+                156,
+                157,
+                158,
+                159,
+                160,
+                161,
+                163,
+                164,
+                165
             ],
             [
-                35,
-                38,
-                39,
-                43
+                53,
+                56,
+                57,
+                61
             ],
             [
-                100
+                127
             ],
             [
-                116
+                143
             ],
             [
-                41,
-                43,
-                102
+                59,
+                61,
+                129
             ],
             [
-                41,
-                42
+                59,
+                60
             ],
             [
-                41,
-                106
+                59,
+                133
             ],
             [
-                43,
-                97,
-                98
+                61,
+                124,
+                125
             ],
             [
-                65,
-                79,
-                93,
-                95,
-                128
+                87,
+                101,
+                120,
+                122,
+                155
             ],
             [
-                42,
-                99,
-                133,
-                134
+                60,
+                126,
+                160,
+                161
             ],
             [
-                41,
-                65,
-                66,
-                93,
-                100,
-                128,
-                132,
-                134,
-                135
+                59,
+                87,
+                88,
+                120,
+                127,
+                155,
+                159,
+                161,
+                162
             ],
             [
-                41
+                59
             ],
             [
-                34
+                52
             ],
             [
-                79,
-                93,
-                139
+                101,
+                120,
+                166
             ],
             [
-                152,
-                153,
-                154
+                179,
+                180,
+                181
             ],
             [
-                79,
-                139
+                101,
+                166
             ],
             [
-                233,
-                234,
-                236,
-                239,
-                241
+                260,
+                261,
+                263,
+                266,
+                268
             ],
             [
-                233
+                260
             ],
             [
-                233,
-                236
+                260,
+                263
             ],
             [
-                243
+                270
             ],
             [
-                65,
-                93
+                87,
+                120
             ],
             [
-                248,
-                250
+                275,
+                277
             ],
             [
-                247,
-                248,
-                249
+                274,
+                275,
+                276
             ],
             [
-                63,
-                93
+                85,
+                120
             ],
             [
-                254
+                281
             ],
             [
-                255
+                282
             ],
             [
-                261,
-                264
+                288,
+                291
             ],
             [
-                259
+                286
             ],
             [
-                52,
-                93,
-                257,
-                263
+                71,
+                120,
+                284,
+                290
             ],
             [
-                261
+                288
             ],
             [
-                258,
-                262
+                285,
+                289
             ],
             [
-                260
+                287
             ],
             [
-                62,
-                88,
-                93,
-                278,
-                279,
-                281
+                84,
+                115,
+                120,
+                305,
+                306,
+                308
             ],
             [
-                280
+                307
             ],
             [
-                283,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                310,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                283,
-                284,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                310,
+                311,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                283,
-                284,
-                285,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                310,
+                311,
+                312,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                310,
+                311,
+                312,
+                313,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                310,
+                311,
+                312,
+                313,
+                314,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                291,
-                292,
-                293,
-                294,
-                295
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                292,
-                293,
-                294,
-                295
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                293,
-                294,
-                295
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                320,
+                321,
+                322
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                294,
-                295
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                321,
+                322
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                295
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                322
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321
             ],
             [
-                50
+                68
             ],
             [
-                52
+                71
             ],
             [
-                53,
-                58
+                72,
+                77,
+                104
             ],
             [
-                54,
-                62,
-                63,
-                70,
-                79
+                73,
+                84,
+                85,
+                92,
+                101,
+                112
             ],
             [
-                54,
-                55,
-                62,
-                70
+                73,
+                74,
+                84,
+                92
             ],
             [
-                56,
-                86
+                75,
+                113
             ],
             [
-                57,
-                58,
-                63,
-                71
+                76,
+                77,
+                85,
+                93
+            ],
+            [
+                77,
+                101,
+                109
+            ],
+            [
+                78,
+                80,
+                84,
+                92
             ],
             [
-                58,
                 79
             ],
             [
-                59,
-                60,
-                62,
-                70
+                80,
+                81
             ],
             [
-                60
+                84
             ],
             [
-                61,
-                62
+                83,
+                84
             ],
             [
-                62
+                71,
+                84
             ],
             [
-                62,
-                63,
-                64,
-                79,
-                85
+                84,
+                85,
+                86,
+                101,
+                112
             ],
             [
-                63,
-                64
+                84,
+                85,
+                86,
+                101
             ],
             [
-                62,
-                65,
-                70,
-                79,
-                85
+                84,
+                87,
+                92,
+                101,
+                112
             ],
             [
-                62,
-                63,
-                65,
-                66,
-                70,
-                79,
-                82,
-                85
+                84,
+                85,
+                87,
+                88,
+                92,
+                101,
+                109,
+                112
             ],
             [
-                65,
-                67,
-                79,
-                82,
-                85
+                87,
+                89,
+                101,
+                109,
+                112
             ],
             [
-                50,
-                51,
-                52,
-                53,
-                54,
-                55,
-                56,
-                57,
-                58,
-                59,
-                60,
-                61,
-                62,
-                63,
-                64,
-                65,
-                66,
-                67,
                 68,
                 69,
                 70,
                 71,
                 72,
                 73,
                 74,
@@ -1782,337 +1809,396 @@
                 85,
                 86,
                 87,
                 88,
                 89,
                 90,
                 91,
-                92
+                92,
+                93,
+                94,
+                95,
+                96,
+                97,
+                98,
+                99,
+                100,
+                101,
+                102,
+                103,
+                104,
+                105,
+                106,
+                107,
+                108,
+                109,
+                110,
+                111,
+                112,
+                113,
+                114,
+                115,
+                116,
+                117,
+                118,
+                119
             ],
             [
-                62,
-                68
+                84,
+                90
             ],
             [
-                69,
-                85
+                91,
+                112,
+                117
             ],
             [
-                60,
-                62,
-                70,
-                79
+                80,
+                84,
+                92,
+                101
             ],
             [
-                71
+                93
             ],
             [
-                72
+                94
             ],
             [
-                52,
-                73
+                71,
+                95
             ],
             [
-                74,
-                84
+                96,
+                111,
+                117
             ],
             [
-                75
+                97
             ],
             [
-                76
+                98
             ],
             [
-                62,
-                77
+                84,
+                99
             ],
             [
-                77,
-                78,
-                86,
-                88
+                99,
+                100,
+                113,
+                115
             ],
             [
-                62,
-                79
+                72,
+                84,
+                101,
+                102,
+                103
             ],
             [
-                80
+                72,
+                101,
+                103
             ],
             [
-                81
+                101,
+                102
             ],
             [
-                70,
-                79,
-                82
+                104
             ],
             [
-                83
+                105
             ],
             [
-                70,
-                84
+                84,
+                107,
+                108
             ],
             [
-                65,
-                76,
-                85
+                107,
+                108
             ],
             [
-                86
+                77,
+                92,
+                101,
+                109
             ],
             [
-                79,
-                87
+                110
             ],
             [
-                88
+                92,
+                111
             ],
             [
-                89
+                72,
+                87,
+                98,
+                112
             ],
             [
-                62,
-                64,
-                79,
-                85,
-                88,
-                90
+                77,
+                113
             ],
             [
-                79,
-                91
+                101,
+                114
             ],
             [
-                301,
-                340
+                115
             ],
             [
-                301,
-                325,
-                340
+                116
             ],
             [
-                340
+                72,
+                77,
+                84,
+                86,
+                95,
+                101,
+                112,
+                115,
+                117
             ],
             [
-                301
+                101,
+                118
             ],
             [
-                301,
-                326,
-                340
+                328,
+                367
+            ],
+            [
+                328,
+                352,
+                367
+            ],
+            [
+                367
+            ],
+            [
+                328
+            ],
+            [
+                328,
+                353,
+                367
             ],
             [
-                301,
-                302,
-                303,
-                304,
-                305,
-                306,
-                307,
-                308,
-                309,
-                310,
-                311,
-                312,
-                313,
-                314,
-                315,
-                316,
-                317,
-                318,
-                319,
-                320,
-                321,
-                322,
-                323,
-                324,
-                325,
-                326,
-                327,
                 328,
                 329,
                 330,
                 331,
                 332,
                 333,
                 334,
                 335,
                 336,
                 337,
                 338,
-                339
+                339,
+                340,
+                341,
+                342,
+                343,
+                344,
+                345,
+                346,
+                347,
+                348,
+                349,
+                350,
+                351,
+                352,
+                353,
+                354,
+                355,
+                356,
+                357,
+                358,
+                359,
+                360,
+                361,
+                362,
+                363,
+                364,
+                365,
+                366
             ],
             [
-                326,
-                340
+                353,
+                367
             ],
             [
-                62,
-                65,
-                67,
-                70,
-                79,
-                82,
-                85,
-                91,
-                93
+                84,
+                87,
+                89,
+                92,
+                101,
+                109,
+                112,
+                118,
+                120
             ],
             [
-                344
+                371
             ],
             [
-                267
+                294
             ],
             [
-                266,
-                267
+                293,
+                294
             ],
             [
-                266
+                293
             ],
             [
-                266,
-                267,
-                268,
-                270,
-                271,
-                274,
-                275,
-                276,
-                277
+                293,
+                294,
+                295,
+                297,
+                298,
+                301,
+                302,
+                303,
+                304
             ],
             [
-                267,
-                271
+                294,
+                298
             ],
             [
-                266,
-                267,
-                268,
-                270,
-                271,
-                272,
-                273
+                293,
+                294,
+                295,
+                297,
+                298,
+                299,
+                300
             ],
             [
-                266,
-                271
+                293,
+                298
             ],
             [
-                271,
-                275
+                298,
+                302
             ],
             [
-                267,
-                268,
-                269
+                294,
+                295,
+                296
             ],
             [
-                268
+                295
             ],
             [
-                266,
-                267,
-                271
+                293,
+                294,
+                298
             ],
             [
-                31
+                49
             ],
             [
-                31,
-                32
+                49,
+                50
             ],
             [
-                31,
-                139,
-                149,
-                187,
-                192
+                49,
+                166,
+                176,
+                214,
+                219
             ],
             [
-                31,
-                193,
-                221
+                49,
+                220,
+                248
             ],
             [
-                31,
-                139,
-                212,
-                220
+                49,
+                166,
+                239,
+                247
             ],
             [
-                31,
-                222
+                49,
+                249
             ],
             [
-                31,
-                149
+                49,
+                176
             ],
             [
-                31,
-                190
+                49,
+                217
             ],
             [
-                31,
-                188,
-                189,
-                191
+                49,
+                215,
+                216,
+                218
             ],
             [
-                31,
-                189
+                49,
+                216
             ],
             [
-                31,
-                33,
-                223,
-                230
+                49,
+                51,
+                250,
+                257
             ],
             [
-                31,
-                139,
-                187
+                49,
+                166,
+                214
             ],
             [
-                31,
-                224,
-                225,
-                227,
-                229
+                49,
+                251,
+                252,
+                254,
+                256
             ],
             [
-                31,
-                187
+                49,
+                214
             ],
             [
-                31,
-                139,
-                226
+                49,
+                166,
+                253
             ],
             [
-                31,
-                139,
-                187,
-                226,
-                228
+                49,
+                166,
+                214,
+                253,
+                255
             ]
         ],
         "fileInfos": [
             {
                 "affectsGlobalScope": true,
                 "version": "8730f4bf322026ff5229336391a18bcaa1f94d4f82416c8b2f3954e2ccaae2ba"
             },
             "dc47c4fa66b9b9890cf076304de2a9c5201e94b740cffdf09f87296d877d71f6",
             "7a387c58583dfca701b6c85e0adaf43fb17d590fb16d5b2dc0a2fbd89f35c467",
             "8a12173c586e95f4433e0c6dc446bc88346be73ffe9ca6eec7aa63c8f3dca7f9",
             "5f4e733ced4e129482ae2186aae29fde948ab7182844c3a5a51dd346182c7b06",
+            "4b421cbfb3a38a27c279dec1e9112c3d1da296f77a1a85ddadf7e7a425d45d18",
+            "1fc5ab7a764205c68fa10d381b08417795fc73111d6dd16b5b1ed36badb743d9",
+            "746d62152361558ea6d6115cf0da4dd10ede041d14882ede3568bce5dc4b4f1f",
             {
                 "affectsGlobalScope": true,
                 "version": "3aafcb693fe5b5c3bd277bd4c3a617b53db474fe498fc5df067c5603b1eebde7"
             },
             {
                 "affectsGlobalScope": true,
                 "version": "f3d4da15233e593eacb3965cde7960f3fddf5878528d882bcedd5cbaba0193c7"
@@ -2195,22 +2281,82 @@
             },
             {
                 "affectsGlobalScope": true,
                 "version": "c80df75850fea5caa2afe43b9949338ce4e2de086f91713e9af1a06f973872b8"
             },
             {
                 "affectsGlobalScope": true,
+                "version": "9d57b2b5d15838ed094aa9ff1299eecef40b190722eb619bac4616657a05f951"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "6c51b5dd26a2c31dbf37f00cfc32b2aa6a92e19c995aefb5b97a3a64f1ac99de"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "6e7997ef61de3132e4d4b2250e75343f487903ddf5370e7ce33cf1b9db9a63ed"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "2ad234885a4240522efccd77de6c7d99eecf9b4de0914adb9a35c0c22433f993"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "5e5e095c4470c8bab227dbbc61374878ecead104c74ab9960d3adcccfee23205"
+            },
+            {
+                "affectsGlobalScope": true,
                 "version": "09aa50414b80c023553090e2f53827f007a301bc34b0495bfb2c3c08ab9ad1eb"
             },
             {
                 "affectsGlobalScope": true,
+                "version": "d7f680a43f8cd12a6b6122c07c54ba40952b0c8aa140dcfcf32eb9e6cb028596"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "3787b83e297de7c315d55d4a7c546ae28e5f6c0a361b7a1dcec1f1f50a54ef11"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "e7e8e1d368290e9295ef18ca23f405cf40d5456fa9f20db6373a61ca45f75f40"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "faf0221ae0465363c842ce6aa8a0cbda5d9296940a8e26c86e04cc4081eea21e"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "06393d13ea207a1bfe08ec8d7be562549c5e2da8983f2ee074e00002629d1871"
+            },
+            {
+                "affectsGlobalScope": true,
                 "version": "2768ef564cfc0689a1b76106c421a2909bdff0acbe87da010785adab80efdd5c"
             },
             {
                 "affectsGlobalScope": true,
+                "version": "b248e32ca52e8f5571390a4142558ae4f203ae2f94d5bac38a3084d529ef4e58"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "6c55633c733c8378db65ac3da7a767c3cf2cf3057f0565a9124a16a3a2019e87"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "fb4416144c1bf0323ccbc9afb0ab289c07312214e8820ad17d709498c865a3fe"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "5b0ca94ec819d68d33da516306c15297acec88efeb0ae9e2b39f71dbd9685ef7"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "34c839eaaa6d78c8674ae2c37af2236dee6831b13db7b4ef4df3ec889a04d4f2"
+            },
+            {
+                "affectsGlobalScope": true,
                 "version": "52d1bb7ab7a3306fd0375c8bff560feed26ed676a5b0457fa8027b563aecb9a4"
             },
             "7a1971efcba559ea9002ada4c4e3c925004fb67a755300d53b5edf9399354900",
             "6d93b19d11edb10bce1aa933bae0fdf55c57785d376c4617e32506783791cd03",
             "38f6da5b6f318c33e18dd7c983cab3fe52f510c9a2573948fb13f012e01b1ba6",
             "c55ae709f94155174ff63647edd2a7e3acbd02a2909aa2541569e8b8bac9fc40",
             "530e5c7e4f74267b7800f1702cf0c576282296a960acbdb2960389b2b1d0875b",
@@ -2224,79 +2370,103 @@
             "b7b881ced4ed4dee13d6e0ccdb2296f66663ba6b1419767271090b3ff3478bb9",
             "06289b9873760aac77aed4035ea6c60b1e0879b8afe47a4530bc8522b9b804b1",
             "63c36aa73242aa745fae813c40585111ead225394b0a0ba985c2683baa6b0ef9",
             "3e7ffc7dd797e5d44d387d0892bc288480493e73dcab9832812907d1389e4a98",
             "db011ec9589fd51995cbd0765673838e38e6485a6559163cc53dcf508b480909",
             "e1a4253f0cca15c14516f52a2ad36c3520b140b5dfb3b3880a368cd75d45d6d9",
             "159af954f2633a12fdee68605009e7e5b150dbeb6d70c46672fd41059c154d53",
-            "4c2c4f53e8eedd970f8afa369d7371544fb6231bf95e659f8602e09abe74d5a5",
+            "5b3cd03ae354ea96eff1f74d7c410fe4852e6382227e8b0ecf87ab5e3a5bbcd4",
+            "7394959e5a741b185456e1ef5d64599c36c60a323207450991e7a42e08911419",
+            {
+                "affectsGlobalScope": true,
+                "version": "056097110efd16869ec118cedb44ecbac9a019576eee808d61304ca6d5cb2cbe"
+            },
+            "f51b4042a3ac86f1f707500a9768f88d0b0c1fc3f3e45a73333283dea720cdc6",
+            {
+                "affectsGlobalScope": true,
+                "version": "6fb8358e10ed92a7f515b7d79da3904c955a3ffd4e14aa9df6f0ea113041f1cf"
+            },
+            "45c831238c6dac21c72da5f335747736a56a3847192bf03c84b958a7e9ec93e2",
+            "661a11d16ad2e3543a77c53bcd4017ee9a450f47ab7def3ab493a86eae4d550c",
+            {
+                "affectsGlobalScope": true,
+                "version": "8cdc646cec7819581ef343b83855b1bfe4fe674f2c84f4fb8dc90d82fb56bd3a"
+            },
+            "a40826e8476694e90da94aa008283a7de50d1dafd37beada623863f1901cb7fb",
+            "9dd56225cc2d8cb8fe5ceb0043ff386987637e12fecc6078896058a99deae284",
+            "2375ed4b439215aa3b6d0c6fd175c78a4384b30cb43cbadaecbf0a18954c98cb",
+            "7693b90b3075deaccafd5efb467bf9f2b747a3075be888652ef73e64396d8628",
+            "41231da15bb5e3e806a8395bd15c7befd2ec90f9f4e3c9d0ae1356bccb76dbb0",
+            "fccfef201d057cb407fa515311bd608549bab6c7b8adcf8f2df31f5d3b796478",
+            {
+                "affectsGlobalScope": true,
+                "version": "ee1ee365d88c4c6c0c0a5a5701d66ebc27ccd0bcfcfaa482c6e2e7fe7b98edf7"
+            },
+            "5f20d20b7607174caf1a6da9141aeb9f2142159ae2410ca30c7a0fccd1d19c99",
             {
                 "affectsGlobalScope": true,
-                "version": "cb5a780979155e80a2184eb987cc411a95c9a1686019ade06918c312a0b7c9b2"
+                "version": "464762c6213566d072f1ced5e8e9a954785ec5e53883b7397198abb5ef5b8f71"
             },
-            "c2b5085f47e41d6940bbc5b0d3bd7cc0037c752efb18aecd243c9cf83ad0c0b7",
-            "3143a5add0467b83150961ecd33773b561a1207aec727002aa1d70333068eb1b",
-            "f87191b7fafe7a0edad375710d99f900e49cef560b66bf309cf3f8e1b7177126",
-            "586af7d2abe2f9d59c5e757c370087d6c6baea81b033250f43b8df808d6dfb33",
+            "6387920dc3e18927335b086deec75bf8e50f879a5e273d32ee7bb7a55ba50572",
+            "9bba37424094688c4663c177a1379b229f919b8912889a472f32fdc5f08ddb4d",
+            "29a4be13b3a30d3e66667b75c58ec61fb2df8fa0422534fdee3cfb30c5dbf450",
+            "83366d901beda79d6eb37aaaf6ca248dcd88946302b2a7d975590783be51e88e",
+            "bf268a0aea37ad4ae3b7a9b58559190b6fc01ea16a31e35cd05817a0a60f895a",
+            "43ec77c369473e92e2ecebf0554a0fdaa9c256644a6070f28228dfcceec77351",
             {
                 "affectsGlobalScope": true,
-                "version": "1a048ff164b8d9609f5de3139d4e37f6e8a82af82087ac414b9208f52ef8aac7"
+                "version": "d7dad6db394a3d9f7b49755e4b610fbf8ed6eb0c9810ae5f1a119f6b5d76de45"
             },
-            "3111079f3cb5f2b9c812ca3f46161562bce5bfb355e915f46ed46c41714dc1c3",
-            "e7bee4a6d9bb78afa390b25e0ce97a2f94787a1eb17f0a16e732dcbebba3f3ee",
-            "b32b6b16cb0bda68199582ad6f22242d07ee75fac9b1f28a98cd838afc5eea45",
-            "4441ee4119824bfaebc49308559edd7545978f9cb41a40f115074e1031dde75f",
+            "95ed02bacb4502c985b69742ec82a4576d4ff4a6620ecc91593f611d502ae546",
+            "bf755525c4e6f85a970b98c4755d98e8aa1b6dbd83a5d8fcc57d3d497351b936",
+            "dd67d2b5e4e8a182a38de8e69fb736945eaa4588e0909c14e01a14bd3cc1fd1e",
             {
                 "affectsGlobalScope": true,
-                "version": "60693a88462d0e97900123b5bf7c73e146ce0cc94da46a61fe6775b430d2ff05"
+                "version": "28084e15b63e6211769db2fe646d8bc5c4c6776321e0deffe2d12eefd52cb6b9"
             },
             {
                 "affectsGlobalScope": true,
-                "version": "588c69eda58b9202676ec7ca11a72c3762819b46a0ed72462c769846153c447c"
+                "version": "aed37dabf86c99d6c8508700576ecede86688397bc12523541858705a0c737c2"
             },
-            "ae064ed4f855716b7ff348639ddcd6a6d354a72fae82f506608a7dc9266aa24c",
-            "92f019c55b21c939616f6a48f678e714ac7b109444cbbf23ad69310ce66ecbdc",
-            "bba259efdf9ab95e0c7d3cc8e99250f56bb6b31d6129efdf733ca4eb1d01feea",
-            "499b7544062cf44fab253daeaea8ba28877d9e7ff4149246b1f0154d1c9ed535",
-            "139fd681eff7771a38d0c025d13c7a11c5474f6aab61e01c41511d71496df173",
-            "f614c3f61e46ccc2cb58702d5a158338ea57ee09099fde5db4cfc63ed0ce4d74",
-            "44e42ed6ec9c4451ebe89524e80ac8564e9dd0988c56e6c58f393c810730595d",
-            "a504c109b872b0e653549bd258eb06584c148c98d79406c7516995865a6d5089",
-            "155865f5f76db0996cd5e20cc5760613ea170ee5ad594c1f3d76fcaa05382161",
-            "e92852d673c836fc64e10c38640abcd67c463456e5df55723ac699b8e6ab3a8a",
-            "4455c78d226d061b1203c7614c6c6eb5f4f9db5f00d44ff47d0112de8766fbc4",
+            "cc6ef5733d4ea6d2e06310a32dffd2c16418b467c5033d49cecc4f3a25de7497",
+            "94768454c3348b6ebe48e45fbad8c92e2bb7af4a35243edbe2b90823d0bd7f9a",
+            "0be79b3ff0f16b6c2f9bc8c4cc7097ea417d8d67f8267f7e1eec8e32b548c2ff",
+            "1c61ffa3a71b77363b30d19832c269ef62fba787f5610cac7254728d3b69ab2e",
+            "84da3c28344e621fd1d591f2c09e9595292d2b70018da28a553268ac122597d4",
+            "269929a24b2816343a178008ac9ae9248304d92a8ba8e233055e0ed6dbe6ef71",
+            "6e191fea1db6e9e4fa828259cf489e820ec9170effff57fb081a2f3295db4722",
+            "aed943465fbce1efe49ee16b5ea409050f15cd8eaf116f6fadb64ef0772e7d95",
+            "70d08483a67bf7050dbedace398ef3fee9f436fcd60517c97c4c1e22e3c6f3e8",
+            "c40fdf7b2e18df49ce0568e37f0292c12807a0748be79e272745e7216bed2606",
             {
                 "affectsGlobalScope": true,
-                "version": "ec369bb9d97c4dc09dd2a4093b7ca3ba69ad284831fccac8a1977785e9e38ce5"
+                "version": "e933de8143e1d12dd51d89b398760fd5a9081896be366dad88a922d0b29f3c69"
             },
-            "4465a636f5f6e9665a90e30691862c9e0a3ac2edc0e66296704f10865e924f2a",
-            "9af781f03d44f5635ed7844be0ce370d9d595d4b4ec67cad88f0fac03255257e",
-            "f9fd4c3ef6de27fa0e256f4e75b61711c4be05a3399f7714621d3edc832e36b0",
-            "e49290b7a927995c0d7e6b2b9c8296284b68a9036d9966531de65185269258d7",
-            "aa95cc73ea5315e4f6fc8c6db43d49e3b7de3780cae20a4f1319032809013038",
-            "874ca809b79276460011480a2829f4c8d4db29416dd411f71efbf8f497f0ac09",
-            "6c903bceaf3f3bc04f2d4c7dcd89ce9fb148b3ba0a5f5408d8f6de2b7eecc7ea",
-            "504d049d9e550a65466b73ca39da6469ab41786074ea1d16d37c8853f9f6ab2e",
-            "23a28f834a078986bbf58f4e3705956983ff81c3c2493f3db3e5f0e8a9507779",
-            "4febdf7f3ec92706c58e0b4e8159cd6de718284ef384260b07c9641c13fc70ce",
+            "4e228e78c1e9b0a75c70588d59288f63a6258e8b1fe4a67b0c53fe03461421d9",
+            "b38d55d08708c2410a3039687db70b4a5bfa69fc4845617c313b5a10d9c5c637",
+            "205d50c24359ead003dc537b9b65d2a64208dfdffe368f403cf9e0357831db9e",
+            "1265fddcd0c68be9d2a3b29805d0280484c961264dd95e0b675f7bd91f777e78",
             {
                 "affectsGlobalScope": true,
-                "version": "bf241ed073916ec9e21a3c138936edd444b6787d874844c0d05fc00a8f109d19"
+                "version": "a05e2d784c9be7051c4ac87a407c66d2106e23490c18c038bbd0712bde7602fd"
             },
-            "7335933d9f30dcfd2c4b6080a8b78e81912a7fcefb1dafccb67ca4cb4b3ac23d",
-            "a6bfe9de9adef749010c118104b071d14943802ff0614732b47ce4f1c3e383cd",
-            "4c3d0e10396646db4a1e917fb852077ee77ae62e512913bef9cccc2bb0f8bd0e",
-            "3b220849d58140dcc6718f5b52dcd29fdb79c45bc28f561cbd29eb1cac6cce13",
-            "0ee22fce41f7417a24c808d266e91b850629113c104713a35854393d55994beb",
-            "22d1b1d965baba05766613e2e6c753bb005d4386c448cafd72c309ba689e8c24",
             {
                 "affectsGlobalScope": true,
-                "version": "2708349d5a11a5c2e5f3a0765259ebe7ee00cdcc8161cb9990cb4910328442a1"
+                "version": "df90b9d0e9980762da8daf8adf6ffa0c853e76bfd269c377be0d07a9ad87acd2"
             },
-            "c6c0bd221bb1e94768e94218f8298e47633495529d60cae7d8da9374247a1cf5",
+            "cf434b5c04792f62d6f4bdd5e2c8673f36e638e910333c172614d5def9b17f98",
+            "1d65d4798df9c2df008884035c41d3e67731f29db5ecb64cd7378797c7c53a2f",
+            "0faee6b555890a1cb106e2adc5d3ffd89545b1da894d474e9d436596d654998f",
+            "c6c01ea1c42508edf11a36d13b70f6e35774f74355ba5d358354d4a77cc67ea1",
+            "867f95abf1df444aab146b19847391fc2f922a55f6a970a27ed8226766cee29f",
+            {
+                "affectsGlobalScope": true,
+                "version": "ab9b9a36e5284fd8d3bf2f7d5fcbc60052f25f27e4d20954782099282c60d23e"
+            },
+            "b0297b09e607bec9698cac7cf55463d6731406efb1161ee4d448293b47397c84",
             "a1b36a1f91a54daf2e89e12b834fa41fb7338bc044d1f08a80817efc93c99ee5",
             "8bb4a5b632dd5a868f3271750895cb61b0e20cff82032d87e89288faee8dd6e2",
             "0c1aabfd9fb1818afb2e798f91f669edafce59cd7e3423d25b1cfccfaaf2c403",
             "017de6fdabea79015d493bf71e56cbbff092525253c1d76003b3d58280cd82a0",
             "ab9ea2596cb7800bd79d1526930c785606ec4f439c275adbca5adc1ddf87747d",
             "aee8faa433dde04beedb779b3329456a286a966462d666c138c19113ce78c79e",
             "d620ec36bfc6f8ed6fdecbe036d55cec81637f32fd34dc7bb7e60eba1764e910",
@@ -2566,14 +2736,17 @@
         ],
         "fileNames": [
             "../../node_modules/typescript/lib/lib.es5.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.d.ts",
             "../../node_modules/typescript/lib/lib.es2016.d.ts",
             "../../node_modules/typescript/lib/lib.es2017.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.d.ts",
+            "../../node_modules/typescript/lib/lib.es2021.d.ts",
             "../../node_modules/typescript/lib/lib.dom.d.ts",
             "../../node_modules/typescript/lib/lib.dom.iterable.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.core.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.collection.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.generator.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.iterable.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.promise.d.ts",
@@ -2588,16 +2761,31 @@
             "../../node_modules/typescript/lib/lib.es2017.intl.d.ts",
             "../../node_modules/typescript/lib/lib.es2017.typedarrays.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.asyncgenerator.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.asynciterable.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.intl.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.promise.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.regexp.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.array.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.object.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.string.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.symbol.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.intl.d.ts",
             "../../node_modules/typescript/lib/lib.es2020.bigint.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.date.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.promise.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.sharedmemory.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.string.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.symbol.wellknown.d.ts",
             "../../node_modules/typescript/lib/lib.es2020.intl.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.number.d.ts",
+            "../../node_modules/typescript/lib/lib.es2021.promise.d.ts",
+            "../../node_modules/typescript/lib/lib.es2021.string.d.ts",
+            "../../node_modules/typescript/lib/lib.es2021.weakref.d.ts",
+            "../../node_modules/typescript/lib/lib.es2021.intl.d.ts",
             "../../node_modules/typescript/lib/lib.esnext.intl.d.ts",
             "../../node_modules/tslib/tslib.d.ts",
             "./src/client/emitWarningIfUnsupportedVersion.ts",
             "./src/client/index.ts",
             "../../node_modules/@smithy/types/dist-types/abort.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/auth.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/HttpApiKeyAuth.d.ts",
@@ -2611,24 +2799,28 @@
             "../../node_modules/@smithy/types/dist-types/middleware.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/HttpSigner.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/IdentityProviderConfig.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/HttpAuthScheme.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/HttpAuthSchemeProvider.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/index.d.ts",
             "../../node_modules/@types/node/assert.d.ts",
+            "../../node_modules/@types/node/assert/strict.d.ts",
             "../../node_modules/@types/node/globals.d.ts",
             "../../node_modules/@types/node/async_hooks.d.ts",
             "../../node_modules/@types/node/buffer.d.ts",
             "../../node_modules/@types/node/child_process.d.ts",
             "../../node_modules/@types/node/cluster.d.ts",
             "../../node_modules/@types/node/console.d.ts",
             "../../node_modules/@types/node/constants.d.ts",
             "../../node_modules/@types/node/crypto.d.ts",
             "../../node_modules/@types/node/dgram.d.ts",
+            "../../node_modules/@types/node/diagnostics_channel.d.ts",
             "../../node_modules/@types/node/dns.d.ts",
+            "../../node_modules/@types/node/dns/promises.d.ts",
+            "../../node_modules/@types/node/dom-events.d.ts",
             "../../node_modules/@types/node/domain.d.ts",
             "../../node_modules/@types/node/events.d.ts",
             "../../node_modules/@types/node/fs.d.ts",
             "../../node_modules/@types/node/fs/promises.d.ts",
             "../../node_modules/@types/node/http.d.ts",
             "../../node_modules/@types/node/http2.d.ts",
             "../../node_modules/@types/node/https.d.ts",
@@ -2640,16 +2832,21 @@
             "../../node_modules/@types/node/perf_hooks.d.ts",
             "../../node_modules/@types/node/process.d.ts",
             "../../node_modules/@types/node/punycode.d.ts",
             "../../node_modules/@types/node/querystring.d.ts",
             "../../node_modules/@types/node/readline.d.ts",
             "../../node_modules/@types/node/repl.d.ts",
             "../../node_modules/@types/node/stream.d.ts",
+            "../../node_modules/@types/node/stream/promises.d.ts",
+            "../../node_modules/@types/node/stream/consumers.d.ts",
+            "../../node_modules/@types/node/stream/web.d.ts",
             "../../node_modules/@types/node/string_decoder.d.ts",
+            "../../node_modules/@types/node/test.d.ts",
             "../../node_modules/@types/node/timers.d.ts",
+            "../../node_modules/@types/node/timers/promises.d.ts",
             "../../node_modules/@types/node/tls.d.ts",
             "../../node_modules/@types/node/trace_events.d.ts",
             "../../node_modules/@types/node/tty.d.ts",
             "../../node_modules/@types/node/url.d.ts",
             "../../node_modules/@types/node/util.d.ts",
             "../../node_modules/@types/node/v8.d.ts",
             "../../node_modules/@types/node/vm.d.ts",
@@ -2920,1252 +3117,1264 @@
             "module": 1,
             "noEmitHelpers": false,
             "noFallthroughCasesInSwitch": true,
             "outDir": "./dist-cjs",
             "preserveConstEnums": true,
             "removeComments": true,
             "rootDir": "./src",
+            "skipLibCheck": true,
             "strict": true,
-            "target": 5,
+            "target": 8,
             "useUnknownInCatchVariables": false
         },
         "referencedMap": [
             [
-                208,
+                235,
                 1
             ],
             [
-                212,
+                239,
                 2
             ],
             [
-                195,
+                222,
                 3
             ],
             [
-                196,
+                223,
                 3
             ],
             [
-                194,
+                221,
                 1
             ],
             [
-                197,
+                224,
                 4
             ],
             [
-                199,
+                226,
                 1
             ],
             [
-                198,
+                225,
                 1
             ],
             [
-                200,
+                227,
                 5
             ],
             [
-                209,
+                236,
                 1
             ],
             [
-                211,
+                238,
                 1
             ],
             [
-                210,
+                237,
                 6
             ],
             [
-                201,
+                228,
                 1
             ],
             [
-                202,
+                229,
                 6
             ],
             [
-                203,
+                230,
                 6
             ],
             [
-                205,
+                232,
                 7
             ],
             [
-                204,
+                231,
                 1
             ],
             [
-                207,
+                234,
                 8
             ],
             [
-                206,
+                233,
                 1
             ],
             [
-                159,
+                186,
                 9
             ],
             [
-                161,
+                188,
                 10
             ],
             [
-                160,
+                187,
                 1
             ],
             [
-                162,
+                189,
                 9
             ],
             [
-                163,
+                190,
                 9
             ],
             [
-                164,
+                191,
                 11
             ],
             [
-                157,
+                184,
                 1
             ],
             [
-                145,
+                172,
                 1
             ],
             [
-                146,
+                173,
                 12
             ],
             [
-                143,
+                170,
                 13
             ],
             [
-                144,
+                171,
                 14
             ],
             [
-                142,
+                169,
                 15
             ],
             [
-                140,
+                167,
                 1
             ],
             [
-                141,
+                168,
                 1
             ],
             [
-                149,
+                176,
                 16
             ],
             [
-                148,
+                175,
                 1
             ],
             [
-                213,
+                240,
                 1
             ],
             [
-                219,
+                246,
                 1
             ],
             [
-                214,
+                241,
                 1
             ],
             [
-                215,
+                242,
                 1
             ],
             [
-                216,
+                243,
                 1
             ],
             [
-                220,
+                247,
                 17
             ],
             [
-                217,
+                244,
                 1
             ],
             [
-                218,
+                245,
                 1
             ],
             [
-                150,
+                177,
                 1
             ],
             [
-                151,
+                178,
                 1
             ],
             [
-                156,
+                183,
                 18
             ],
             [
-                165,
+                192,
                 19
             ],
             [
-                167,
+                194,
                 20
             ],
             [
-                176,
+                203,
                 1
             ],
             [
-                172,
+                199,
                 1
             ],
             [
-                174,
+                201,
                 21
             ],
             [
-                175,
+                202,
                 22
             ],
             [
-                173,
+                200,
                 1
             ],
             [
-                187,
+                214,
                 23
             ],
             [
-                47,
+                65,
                 24
             ],
             [
-                48,
+                66,
                 25
             ],
             [
-                45,
+                63,
                 26
             ],
             [
-                46,
+                64,
                 27
             ],
             [
-                49,
+                67,
                 28
             ],
             [
-                96,
+                123,
                 29
             ],
             [
-                98,
+                125,
                 30
             ],
             [
-                100,
+                127,
                 31
             ],
             [
-                99,
+                126,
                 32
             ],
             [
-                105,
+                132,
                 33
             ],
             [
-                103,
+                130,
                 34
             ],
             [
-                107,
+                134,
                 35
             ],
             [
-                38,
+                56,
                 36
             ],
             [
-                109,
+                136,
                 37
             ],
             [
-                110,
+                137,
                 38
             ],
             [
-                112,
+                139,
                 39
             ],
             [
-                111,
+                138,
                 40
             ],
             [
-                113,
+                140,
                 41
             ],
             [
-                108,
+                135,
                 42
             ],
             [
-                106,
+                133,
                 43
             ],
             [
-                114,
+                141,
                 44
             ],
             [
-                115,
+                142,
                 45
             ],
             [
-                119,
+                146,
                 46
             ],
             [
-                120,
+                147,
                 47
             ],
             [
-                118,
+                145,
                 48
             ],
             [
-                95,
+                122,
                 49
             ],
             [
-                41,
+                59,
                 50
             ],
             [
-                121,
+                148,
                 51
             ],
             [
-                122,
+                149,
                 52
             ],
             [
-                123,
+                150,
                 52
             ],
             [
-                125,
+                152,
                 53
             ],
             [
-                124,
+                151,
                 52
             ],
             [
-                139,
+                166,
                 54
             ],
             [
-                44,
+                62,
                 55
             ],
             [
-                126,
+                153,
                 56
             ],
             [
-                117,
+                144,
                 57
             ],
             [
-                128,
+                155,
                 58
             ],
             [
-                116,
+                143,
                 59
             ],
             [
-                129,
+                156,
                 60
             ],
             [
-                130,
+                157,
                 61
             ],
             [
-                131,
+                158,
                 29
             ],
             [
-                132,
+                159,
                 29
             ],
             [
-                133,
+                160,
                 62
             ],
             [
-                135,
+                162,
                 63
             ],
             [
-                136,
+                163,
                 64
             ],
             [
-                137,
+                164,
                 56
             ],
             [
-                40,
+                58,
                 65
             ],
             [
-                43,
+                61,
                 43
             ],
             [
-                138,
+                165,
                 66
             ],
             [
-                153,
+                180,
                 67
             ],
             [
-                155,
+                182,
                 68
             ],
             [
-                154,
+                181,
                 69
             ],
             [
-                242,
+                269,
                 70
             ],
             [
-                236,
+                263,
                 71
             ],
             [
-                234,
+                261,
                 71
             ],
             [
-                239,
+                266,
                 72
             ],
             [
-                237,
+                264,
                 71
             ],
             [
-                241,
+                268,
                 71
             ],
             [
-                244,
+                271,
                 73
             ],
             [
-                245,
+                272,
                 73
             ],
             [
-                246,
+                273,
                 74
             ],
             [
-                251,
+                278,
                 75
             ],
             [
-                250,
+                277,
                 76
             ],
             [
-                252,
+                279,
                 77
             ],
             [
-                253,
+                280,
                 77
             ],
             [
-                255,
+                282,
                 78
             ],
             [
-                256,
+                283,
                 79
             ],
             [
-                265,
+                292,
                 80
             ],
             [
-                260,
+                287,
                 81
             ],
             [
-                264,
+                291,
                 82
             ],
             [
-                262,
+                289,
                 83
             ],
             [
-                263,
+                290,
                 84
             ],
             [
-                261,
+                288,
                 85
             ],
             [
-                280,
+                307,
                 86
             ],
             [
-                281,
+                308,
                 87
             ],
             [
-                284,
+                311,
                 88
             ],
             [
-                285,
+                312,
                 89
             ],
             [
-                283,
+                310,
                 90
             ],
             [
-                286,
+                313,
                 91
             ],
             [
-                287,
+                314,
                 92
             ],
             [
-                288,
+                315,
                 93
             ],
             [
-                289,
+                316,
                 94
             ],
             [
-                290,
+                317,
                 95
             ],
             [
-                291,
+                318,
                 96
             ],
             [
-                292,
+                319,
                 97
             ],
             [
-                293,
+                320,
                 98
             ],
             [
-                294,
+                321,
                 99
             ],
             [
-                295,
+                322,
                 100
             ],
             [
-                50,
+                68,
                 101
             ],
             [
-                52,
+                69,
+                101
+            ],
+            [
+                71,
                 102
             ],
             [
-                53,
+                72,
                 103
             ],
             [
-                54,
+                73,
                 104
             ],
             [
-                55,
+                74,
                 105
             ],
             [
-                56,
+                75,
                 106
             ],
             [
-                57,
+                76,
                 107
             ],
             [
-                58,
+                77,
                 108
             ],
             [
-                59,
+                78,
                 109
             ],
             [
-                60,
+                79,
                 110
             ],
             [
-                61,
+                80,
                 111
             ],
             [
-                62,
+                81,
+                111
+            ],
+            [
+                82,
                 112
             ],
             [
-                63,
+                83,
                 113
             ],
             [
-                64,
+                84,
                 114
             ],
             [
-                65,
+                85,
                 115
             ],
             [
-                66,
+                86,
                 116
             ],
             [
-                67,
+                87,
                 117
             ],
             [
-                93,
+                88,
                 118
             ],
             [
-                68,
+                89,
                 119
             ],
             [
-                69,
+                120,
                 120
             ],
             [
-                70,
+                90,
                 121
             ],
             [
-                71,
+                91,
                 122
             ],
             [
-                72,
+                92,
                 123
             ],
             [
-                73,
+                93,
                 124
             ],
             [
-                74,
+                94,
                 125
             ],
             [
-                75,
+                95,
                 126
             ],
             [
-                76,
+                96,
                 127
             ],
             [
-                77,
+                97,
                 128
             ],
             [
-                78,
+                98,
                 129
             ],
             [
-                79,
+                99,
                 130
             ],
             [
-                80,
+                100,
                 131
             ],
             [
-                81,
+                101,
                 132
             ],
             [
-                82,
+                103,
                 133
             ],
             [
-                83,
+                102,
                 134
             ],
             [
-                84,
+                104,
                 135
             ],
             [
-                85,
+                105,
                 136
             ],
             [
-                86,
+                107,
                 137
             ],
             [
-                87,
+                108,
                 138
             ],
             [
-                88,
+                109,
                 139
             ],
             [
-                89,
+                110,
                 140
             ],
             [
-                90,
+                111,
                 141
             ],
             [
-                91,
+                112,
                 142
             ],
             [
-                325,
+                113,
                 143
             ],
             [
-                326,
+                114,
                 144
             ],
             [
-                301,
+                115,
                 145
             ],
             [
-                304,
-                145
+                116,
+                146
             ],
             [
-                323,
-                143
+                117,
+                147
             ],
             [
-                324,
-                143
+                118,
+                148
             ],
             [
-                314,
-                143
+                352,
+                149
             ],
             [
-                313,
-                146
+                353,
+                150
             ],
             [
-                311,
-                143
+                328,
+                151
             ],
             [
-                306,
-                143
+                331,
+                151
             ],
             [
-                319,
-                143
+                350,
+                149
             ],
             [
-                317,
-                143
+                351,
+                149
             ],
             [
-                321,
-                143
+                341,
+                149
             ],
             [
-                305,
-                143
+                340,
+                152
             ],
             [
-                318,
-                143
+                338,
+                149
             ],
             [
-                322,
-                143
+                333,
+                149
             ],
             [
-                307,
-                143
+                346,
+                149
             ],
             [
-                308,
-                143
+                344,
+                149
             ],
             [
-                320,
-                143
+                348,
+                149
             ],
             [
-                302,
-                143
+                332,
+                149
             ],
             [
-                309,
-                143
+                345,
+                149
             ],
             [
-                310,
-                143
+                349,
+                149
             ],
             [
-                312,
-                143
+                334,
+                149
             ],
             [
-                316,
-                143
+                335,
+                149
             ],
             [
-                327,
-                147
+                347,
+                149
             ],
             [
-                315,
-                143
+                329,
+                149
             ],
             [
-                303,
-                143
+                336,
+                149
             ],
             [
-                340,
-                148
+                337,
+                149
             ],
             [
-                334,
-                147
+                339,
+                149
             ],
             [
-                336,
+                343,
                 149
             ],
             [
-                335,
-                147
+                354,
+                153
             ],
             [
-                328,
-                147
+                342,
+                149
             ],
             [
-                329,
-                147
+                330,
+                149
             ],
             [
-                331,
-                147
+                367,
+                154
             ],
             [
-                333,
-                147
+                361,
+                153
             ],
             [
-                337,
-                149
+                363,
+                155
             ],
             [
-                338,
-                149
+                362,
+                153
             ],
             [
-                330,
-                149
+                355,
+                153
             ],
             [
-                332,
-                149
+                356,
+                153
             ],
             [
-                343,
-                150
+                358,
+                153
             ],
             [
-                345,
-                151
+                360,
+                153
             ],
             [
-                268,
-                152
+                364,
+                155
             ],
             [
-                277,
-                153
+                365,
+                155
             ],
             [
-                267,
-                154
+                357,
+                155
             ],
             [
-                278,
+                359,
                 155
             ],
             [
-                273,
+                370,
                 156
             ],
             [
-                274,
+                372,
                 157
             ],
             [
-                272,
+                295,
                 158
             ],
             [
-                276,
+                304,
                 159
             ],
             [
-                270,
+                294,
                 160
             ],
             [
-                269,
+                305,
                 161
             ],
             [
-                275,
+                300,
                 162
             ],
             [
-                271,
-                153
-            ],
-            [
-                32,
+                301,
                 163
             ],
             [
-                33,
+                299,
                 164
             ],
             [
-                193,
+                303,
                 165
             ],
             [
-                222,
+                297,
                 166
             ],
             [
-                221,
+                296,
                 167
             ],
             [
-                223,
+                302,
                 168
             ],
             [
-                188,
-                169
+                298,
+                159
             ],
             [
-                189,
-                163
+                50,
+                169
             ],
             [
-                191,
+                51,
                 170
             ],
             [
-                192,
+                220,
                 171
             ],
             [
-                190,
+                249,
                 172
             ],
             [
-                231,
+                248,
                 173
             ],
             [
-                224,
-                163
-            ],
-            [
-                226,
+                250,
                 174
             ],
             [
-                230,
+                215,
                 175
             ],
             [
-                225,
+                216,
+                169
+            ],
+            [
+                218,
                 176
             ],
             [
-                227,
+                219,
                 177
             ],
             [
-                229,
+                217,
                 178
+            ],
+            [
+                258,
+                179
+            ],
+            [
+                251,
+                169
+            ],
+            [
+                253,
+                180
+            ],
+            [
+                257,
+                181
+            ],
+            [
+                252,
+                182
+            ],
+            [
+                254,
+                183
+            ],
+            [
+                256,
+                184
             ]
         ],
         "semanticDiagnosticsPerFile": [
-            259,
-            208,
-            212,
+            286,
+            235,
+            239,
+            222,
+            223,
+            221,
+            224,
+            226,
+            225,
+            227,
+            236,
+            238,
+            237,
+            228,
+            229,
+            230,
+            232,
+            231,
+            234,
+            233,
+            186,
+            188,
+            187,
+            189,
+            190,
+            191,
+            184,
+            185,
+            172,
+            173,
+            170,
+            171,
+            169,
+            167,
+            168,
+            176,
+            174,
+            175,
+            240,
+            246,
+            241,
+            242,
+            243,
+            247,
+            244,
+            245,
+            177,
+            178,
+            183,
+            192,
+            193,
+            194,
             195,
             196,
-            194,
             197,
-            199,
             198,
-            200,
-            209,
-            211,
-            210,
+            203,
+            204,
+            199,
             201,
             202,
-            203,
+            200,
             205,
-            204,
-            207,
             206,
-            159,
-            161,
-            160,
-            162,
-            163,
-            164,
-            157,
-            158,
-            145,
-            146,
-            143,
-            144,
-            142,
-            140,
-            141,
-            149,
-            147,
-            148,
-            213,
-            219,
             214,
-            215,
-            216,
-            220,
-            217,
-            218,
-            150,
-            151,
-            156,
-            165,
-            166,
-            167,
-            168,
-            169,
-            170,
-            171,
-            176,
-            177,
-            172,
-            174,
-            175,
-            173,
-            178,
-            179,
-            187,
-            180,
-            181,
-            182,
-            183,
-            184,
-            185,
-            186,
-            34,
-            36,
-            47,
-            48,
-            45,
-            46,
-            35,
-            49,
-            96,
-            98,
-            100,
-            99,
-            101,
-            105,
-            103,
-            104,
-            97,
-            107,
-            38,
-            109,
-            110,
-            112,
-            111,
-            113,
-            108,
-            106,
-            114,
-            115,
-            119,
-            120,
-            118,
-            95,
-            41,
-            121,
-            122,
+            207,
+            208,
+            209,
+            210,
+            211,
+            212,
+            213,
+            52,
+            54,
+            65,
+            66,
+            63,
+            64,
+            53,
+            67,
             123,
-            37,
             125,
-            124,
-            139,
-            39,
-            44,
-            126,
             127,
-            42,
-            117,
+            126,
             128,
-            116,
-            129,
+            132,
             130,
             131,
-            132,
-            133,
-            102,
-            135,
+            124,
+            134,
+            56,
             136,
-            94,
             137,
-            134,
-            40,
-            43,
+            139,
             138,
+            140,
+            135,
+            133,
+            141,
+            142,
+            146,
+            147,
+            145,
+            122,
+            59,
+            148,
+            149,
+            150,
+            55,
             152,
+            151,
+            166,
+            57,
+            62,
             153,
-            155,
             154,
-            232,
-            242,
-            236,
-            235,
-            234,
-            233,
-            239,
-            237,
-            238,
-            241,
-            240,
-            244,
-            245,
-            243,
-            246,
-            251,
-            247,
-            250,
-            248,
-            252,
-            253,
-            254,
-            255,
-            256,
-            265,
-            257,
-            260,
-            264,
-            262,
+            60,
+            144,
+            155,
+            143,
+            156,
+            157,
+            158,
+            159,
+            160,
+            129,
+            162,
+            163,
+            121,
+            164,
+            161,
+            58,
+            61,
+            165,
+            179,
+            180,
+            182,
+            181,
+            259,
+            269,
             263,
+            262,
             261,
+            260,
+            266,
+            264,
+            265,
+            268,
+            267,
+            271,
+            272,
+            270,
+            273,
+            278,
+            274,
+            277,
+            275,
+            279,
             280,
             281,
-            249,
             282,
-            284,
-            285,
             283,
-            286,
+            292,
+            284,
             287,
-            288,
+            291,
             289,
             290,
-            291,
-            292,
-            293,
-            294,
-            295,
-            296,
-            297,
-            50,
-            52,
-            53,
-            54,
-            55,
-            56,
-            57,
-            58,
-            59,
-            60,
-            61,
-            62,
-            63,
-            64,
-            51,
-            92,
-            65,
-            66,
-            67,
-            93,
+            288,
+            307,
+            308,
+            276,
+            309,
+            311,
+            312,
+            310,
+            313,
+            314,
+            315,
+            316,
+            317,
+            318,
+            319,
+            320,
+            321,
+            322,
+            323,
+            324,
             68,
             69,
-            70,
             71,
             72,
             73,
             74,
             75,
             76,
             77,
@@ -4174,129 +4383,177 @@
             80,
             81,
             82,
             83,
             84,
             85,
             86,
+            70,
+            119,
             87,
             88,
             89,
+            120,
             90,
             91,
-            298,
-            299,
-            300,
+            92,
+            93,
+            94,
+            95,
+            96,
+            97,
+            98,
+            99,
+            100,
+            101,
+            103,
+            102,
+            104,
+            105,
+            106,
+            107,
+            108,
+            109,
+            110,
+            111,
+            112,
+            113,
+            114,
+            115,
+            116,
+            117,
+            118,
             325,
             326,
-            301,
-            304,
-            323,
-            324,
-            314,
-            313,
-            311,
-            306,
-            319,
-            317,
-            321,
-            305,
-            318,
-            322,
-            307,
-            308,
-            320,
-            302,
-            309,
-            310,
-            312,
-            316,
             327,
-            315,
-            303,
+            352,
+            353,
+            328,
+            331,
+            350,
+            351,
+            341,
             340,
-            339,
+            338,
+            333,
+            346,
+            344,
+            348,
+            332,
+            345,
+            349,
             334,
-            336,
             335,
-            328,
+            347,
             329,
-            331,
-            333,
+            336,
             337,
-            338,
-            330,
-            332,
-            341,
-            279,
-            342,
+            339,
             343,
-            344,
-            345,
-            258,
-            228,
-            268,
-            277,
-            266,
-            267,
-            278,
-            273,
-            274,
-            272,
-            276,
-            270,
-            269,
-            275,
-            271,
-            31,
-            6,
-            7,
+            354,
+            342,
+            330,
+            367,
+            366,
+            361,
+            363,
+            362,
+            355,
+            356,
+            358,
+            360,
+            364,
+            365,
+            357,
+            359,
+            368,
+            306,
+            369,
+            370,
+            371,
+            372,
+            285,
+            255,
+            295,
+            304,
+            293,
+            294,
+            305,
+            300,
+            301,
+            299,
+            303,
+            297,
+            296,
+            302,
+            298,
+            49,
             9,
-            8,
-            2,
             10,
-            11,
             12,
+            11,
+            2,
             13,
             14,
             15,
             16,
             17,
-            3,
-            4,
-            21,
             18,
             19,
             20,
+            3,
+            4,
+            24,
+            21,
             22,
             23,
-            24,
-            5,
             25,
             26,
             27,
+            5,
             28,
             29,
-            1,
             30,
+            31,
+            6,
+            35,
             32,
             33,
-            193,
-            222,
-            221,
-            223,
-            188,
-            189,
-            191,
-            192,
-            190,
-            231,
-            224,
-            226,
-            230,
-            225,
-            227,
-            229
+            34,
+            36,
+            7,
+            37,
+            42,
+            43,
+            38,
+            39,
+            40,
+            41,
+            8,
+            47,
+            44,
+            45,
+            46,
+            1,
+            48,
+            50,
+            51,
+            220,
+            249,
+            248,
+            250,
+            215,
+            216,
+            218,
+            219,
+            217,
+            258,
+            251,
+            253,
+            257,
+            252,
+            254,
+            256
         ]
     },
     "version": "4.9.5"
 }
```

##### package/node_modules/@aws-sdk/core/tsconfig.es.tsbuildinfo

###### Pretty-printed

 * *Similarity: 0.9342602182833604%*

 * *Differences: {"'program'": "{'fileNames': {insert: [(5, '../../node_modules/typescript/lib/lib.es2019.d.ts'), "*

 * *              "(6, '../../node_modules/typescript/lib/lib.es2020.d.ts'), (29, "*

 * *              "'../../node_modules/typescript/lib/lib.es2019.array.d.ts'), (30, "*

 * *              "'../../node_modules/typescript/lib/lib.es2019.object.d.ts'), (31, "*

 * *              "'../../node_modules/typescript/lib/lib.es2019.string.d.ts'), (32, "*

 * *              "'../../node_modules/typescript/lib/lib.es2019.symbol.d.ts'), (33, "*

 * *   […]*

```diff
@@ -1,1766 +1,1798 @@
 {
     "program": {
         "exportedModulesMap": [
             [
-                208,
+                230,
                 1
             ],
             [
-                212,
+                234,
                 2
             ],
             [
-                195,
+                217,
                 3
             ],
             [
-                196,
+                218,
                 3
             ],
             [
-                194,
+                216,
                 1
             ],
             [
-                197,
+                219,
                 4
             ],
             [
-                199,
+                221,
                 1
             ],
             [
-                198,
+                220,
                 1
             ],
             [
-                200,
+                222,
                 5
             ],
             [
-                209,
+                231,
                 1
             ],
             [
-                211,
+                233,
                 1
             ],
             [
-                210,
+                232,
                 6
             ],
             [
-                201,
+                223,
                 1
             ],
             [
-                202,
+                224,
                 6
             ],
             [
-                203,
+                225,
                 6
             ],
             [
-                205,
+                227,
                 7
             ],
             [
-                204,
+                226,
                 1
             ],
             [
-                207,
+                229,
                 8
             ],
             [
-                206,
+                228,
                 1
             ],
             [
-                159,
+                181,
                 9
             ],
             [
-                161,
+                183,
                 10
             ],
             [
-                160,
+                182,
                 1
             ],
             [
-                162,
+                184,
                 9
             ],
             [
-                163,
+                185,
                 9
             ],
             [
-                164,
+                186,
                 11
             ],
             [
-                157,
+                179,
                 1
             ],
             [
-                145,
+                167,
                 1
             ],
             [
-                146,
+                168,
                 12
             ],
             [
-                143,
+                165,
                 13
             ],
             [
-                144,
+                166,
                 14
             ],
             [
-                142,
+                164,
                 15
             ],
             [
-                140,
+                162,
                 1
             ],
             [
-                141,
+                163,
                 1
             ],
             [
-                149,
+                171,
                 16
             ],
             [
-                148,
+                170,
                 1
             ],
             [
-                213,
+                235,
                 1
             ],
             [
-                219,
+                241,
                 1
             ],
             [
-                214,
+                236,
                 1
             ],
             [
-                215,
+                237,
                 1
             ],
             [
-                216,
+                238,
                 1
             ],
             [
-                220,
+                242,
                 17
             ],
             [
-                217,
+                239,
                 1
             ],
             [
-                218,
+                240,
                 1
             ],
             [
-                150,
+                172,
                 1
             ],
             [
-                151,
+                173,
                 1
             ],
             [
-                156,
+                178,
                 18
             ],
             [
-                165,
+                187,
                 19
             ],
             [
-                167,
+                189,
                 20
             ],
             [
-                176,
+                198,
                 1
             ],
             [
-                172,
+                194,
                 1
             ],
             [
-                174,
+                196,
                 21
             ],
             [
-                175,
+                197,
                 22
             ],
             [
-                173,
+                195,
                 1
             ],
             [
-                187,
+                209,
                 23
             ],
             [
-                47,
+                60,
                 24
             ],
             [
-                48,
+                61,
                 25
             ],
             [
-                45,
+                58,
                 26
             ],
             [
-                46,
+                59,
                 27
             ],
             [
-                49,
+                62,
                 28
             ],
             [
-                96,
+                118,
                 29
             ],
             [
-                98,
+                120,
                 30
             ],
             [
-                100,
+                122,
                 31
             ],
             [
-                99,
+                121,
                 32
             ],
             [
-                105,
+                127,
                 33
             ],
             [
-                103,
+                125,
                 34
             ],
             [
-                107,
+                129,
                 35
             ],
             [
-                38,
+                51,
                 36
             ],
             [
-                109,
+                131,
                 37
             ],
             [
-                110,
+                132,
                 38
             ],
             [
-                112,
+                134,
                 39
             ],
             [
-                111,
+                133,
                 40
             ],
             [
-                113,
+                135,
                 41
             ],
             [
-                108,
+                130,
                 42
             ],
             [
-                106,
+                128,
                 43
             ],
             [
-                114,
+                136,
                 44
             ],
             [
-                115,
+                137,
                 45
             ],
             [
-                119,
+                141,
                 46
             ],
             [
-                120,
+                142,
                 47
             ],
             [
-                118,
+                140,
                 48
             ],
             [
-                95,
+                117,
                 49
             ],
             [
-                41,
+                54,
                 50
             ],
             [
-                121,
+                143,
                 51
             ],
             [
-                122,
+                144,
                 52
             ],
             [
-                123,
+                145,
                 52
             ],
             [
-                125,
+                147,
                 53
             ],
             [
-                124,
+                146,
                 52
             ],
             [
-                139,
+                161,
                 54
             ],
             [
-                44,
+                57,
                 55
             ],
             [
-                126,
+                148,
                 56
             ],
             [
-                117,
+                139,
                 57
             ],
             [
-                128,
+                150,
                 58
             ],
             [
-                116,
+                138,
                 59
             ],
             [
-                129,
+                151,
                 60
             ],
             [
-                130,
+                152,
                 61
             ],
             [
-                131,
+                153,
                 29
             ],
             [
-                132,
+                154,
                 29
             ],
             [
-                133,
+                155,
                 62
             ],
             [
-                135,
+                157,
                 63
             ],
             [
-                136,
+                158,
                 64
             ],
             [
-                137,
+                159,
                 56
             ],
             [
-                40,
+                53,
                 65
             ],
             [
-                43,
+                56,
                 43
             ],
             [
-                138,
+                160,
                 66
             ],
             [
-                153,
+                175,
                 67
             ],
             [
-                155,
+                177,
                 68
             ],
             [
-                154,
+                176,
                 69
             ],
             [
-                242,
+                264,
                 70
             ],
             [
-                236,
+                258,
                 71
             ],
             [
-                234,
+                256,
                 71
             ],
             [
-                239,
+                261,
                 72
             ],
             [
-                237,
+                259,
                 71
             ],
             [
-                241,
+                263,
                 71
             ],
             [
-                244,
+                266,
                 73
             ],
             [
-                245,
+                267,
                 73
             ],
             [
-                246,
+                268,
                 74
             ],
             [
-                251,
+                273,
                 75
             ],
             [
-                250,
+                272,
                 76
             ],
             [
-                252,
+                274,
                 77
             ],
             [
-                253,
+                275,
                 77
             ],
             [
-                255,
+                277,
                 78
             ],
             [
-                256,
+                278,
                 79
             ],
             [
-                265,
+                287,
                 80
             ],
             [
-                260,
+                282,
                 81
             ],
             [
-                264,
+                286,
                 82
             ],
             [
-                262,
+                284,
                 83
             ],
             [
-                263,
+                285,
                 84
             ],
             [
-                261,
+                283,
                 85
             ],
             [
-                280,
+                302,
                 86
             ],
             [
-                281,
+                303,
                 87
             ],
             [
-                284,
+                306,
                 88
             ],
             [
-                285,
+                307,
                 89
             ],
             [
-                283,
+                305,
                 90
             ],
             [
-                286,
+                308,
                 91
             ],
             [
-                287,
+                309,
                 92
             ],
             [
-                288,
+                310,
                 93
             ],
             [
-                289,
+                311,
                 94
             ],
             [
-                290,
+                312,
                 95
             ],
             [
-                291,
+                313,
                 96
             ],
             [
-                292,
+                314,
                 97
             ],
             [
-                293,
+                315,
                 98
             ],
             [
-                294,
+                316,
                 99
             ],
             [
-                295,
+                317,
                 100
             ],
             [
-                50,
+                63,
                 101
             ],
             [
-                52,
+                64,
+                101
+            ],
+            [
+                66,
                 102
             ],
             [
-                53,
+                67,
                 103
             ],
             [
-                54,
+                68,
                 104
             ],
             [
-                55,
+                69,
                 105
             ],
             [
-                56,
+                70,
                 106
             ],
             [
-                57,
+                71,
                 107
             ],
             [
-                58,
+                72,
                 108
             ],
             [
-                59,
+                73,
                 109
             ],
             [
-                60,
+                74,
                 110
             ],
             [
-                61,
+                75,
                 111
             ],
             [
-                62,
+                76,
+                111
+            ],
+            [
+                77,
                 112
             ],
             [
-                63,
+                78,
                 113
             ],
             [
-                64,
+                79,
                 114
             ],
             [
-                65,
+                80,
                 115
             ],
             [
-                66,
+                81,
                 116
             ],
             [
-                67,
+                82,
                 117
             ],
             [
-                93,
+                83,
                 118
             ],
             [
-                68,
+                84,
                 119
             ],
             [
-                69,
+                115,
                 120
             ],
             [
-                70,
+                85,
                 121
             ],
             [
-                71,
+                86,
                 122
             ],
             [
-                72,
+                87,
                 123
             ],
             [
-                73,
+                88,
                 124
             ],
             [
-                74,
+                89,
                 125
             ],
             [
-                75,
+                90,
                 126
             ],
             [
-                76,
+                91,
                 127
             ],
             [
-                77,
+                92,
                 128
             ],
             [
-                78,
+                93,
                 129
             ],
             [
-                79,
+                94,
                 130
             ],
             [
-                80,
+                95,
                 131
             ],
             [
-                81,
+                96,
                 132
             ],
             [
-                82,
+                98,
                 133
             ],
             [
-                83,
+                97,
                 134
             ],
             [
-                84,
+                99,
                 135
             ],
             [
-                85,
+                100,
                 136
             ],
             [
-                86,
+                102,
                 137
             ],
             [
-                87,
+                103,
                 138
             ],
             [
-                88,
+                104,
                 139
             ],
             [
-                89,
+                105,
                 140
             ],
             [
-                90,
+                106,
                 141
             ],
             [
-                91,
+                107,
                 142
             ],
             [
-                325,
+                108,
                 143
             ],
             [
-                326,
+                109,
                 144
             ],
             [
-                301,
+                110,
                 145
             ],
             [
-                304,
-                145
+                111,
+                146
             ],
             [
-                323,
-                143
+                112,
+                147
             ],
             [
-                324,
-                143
+                113,
+                148
             ],
             [
-                314,
-                143
+                347,
+                149
             ],
             [
-                313,
-                146
+                348,
+                150
             ],
             [
-                311,
-                143
+                323,
+                151
             ],
             [
-                306,
-                143
+                326,
+                151
             ],
             [
-                319,
-                143
+                345,
+                149
             ],
             [
-                317,
-                143
+                346,
+                149
             ],
             [
-                321,
-                143
+                336,
+                149
             ],
             [
-                305,
-                143
+                335,
+                152
             ],
             [
-                318,
-                143
+                333,
+                149
             ],
             [
-                322,
-                143
+                328,
+                149
             ],
             [
-                307,
-                143
+                341,
+                149
             ],
             [
-                308,
-                143
+                339,
+                149
             ],
             [
-                320,
-                143
+                343,
+                149
             ],
             [
-                302,
-                143
+                327,
+                149
             ],
             [
-                309,
-                143
+                340,
+                149
             ],
             [
-                310,
-                143
+                344,
+                149
             ],
             [
-                312,
-                143
+                329,
+                149
             ],
             [
-                316,
-                143
+                330,
+                149
             ],
             [
-                327,
-                147
+                342,
+                149
             ],
             [
-                315,
-                143
+                324,
+                149
             ],
             [
-                303,
-                143
+                331,
+                149
             ],
             [
-                340,
-                148
+                332,
+                149
             ],
             [
                 334,
-                147
+                149
             ],
             [
-                336,
+                338,
                 149
             ],
             [
-                335,
-                147
+                349,
+                153
             ],
             [
-                328,
-                147
+                337,
+                149
             ],
             [
-                329,
-                147
+                325,
+                149
             ],
             [
-                331,
-                147
+                362,
+                154
             ],
             [
-                333,
-                147
+                356,
+                153
             ],
             [
-                337,
-                149
+                358,
+                155
             ],
             [
-                338,
-                149
+                357,
+                153
             ],
             [
-                330,
-                149
+                350,
+                153
             ],
             [
-                332,
-                149
+                351,
+                153
             ],
             [
-                343,
-                150
+                353,
+                153
             ],
             [
-                345,
-                151
+                355,
+                153
             ],
             [
-                268,
-                152
+                359,
+                155
             ],
             [
-                277,
-                153
+                360,
+                155
             ],
             [
-                267,
-                154
+                352,
+                155
             ],
             [
-                278,
+                354,
                 155
             ],
             [
-                273,
+                365,
                 156
             ],
             [
-                274,
+                367,
                 157
             ],
             [
-                272,
+                290,
                 158
             ],
             [
-                276,
+                299,
                 159
             ],
             [
-                270,
+                289,
                 160
             ],
             [
-                269,
+                300,
                 161
             ],
             [
-                275,
+                295,
                 162
             ],
             [
-                271,
-                153
-            ],
-            [
-                32,
+                296,
                 163
             ],
             [
-                33,
+                294,
                 164
             ],
             [
-                193,
+                298,
                 165
             ],
             [
-                222,
+                292,
                 166
             ],
             [
-                221,
+                291,
                 167
             ],
             [
-                223,
+                297,
                 168
             ],
             [
-                188,
-                169
+                293,
+                159
             ],
             [
-                189,
-                163
+                45,
+                169
             ],
             [
-                191,
+                46,
                 170
             ],
             [
-                192,
+                215,
                 171
             ],
             [
-                190,
+                244,
                 172
             ],
             [
-                231,
+                243,
                 173
             ],
             [
-                224,
-                163
-            ],
-            [
-                226,
+                245,
                 174
             ],
             [
-                230,
+                210,
                 175
             ],
             [
-                225,
+                211,
+                169
+            ],
+            [
+                213,
                 176
             ],
             [
-                227,
+                214,
                 177
             ],
             [
-                229,
+                212,
                 178
-            ]
-        ],
-        "fileIdsList": [
-            [
-                139
             ],
             [
-                197,
-                200,
-                207,
-                208,
-                209,
-                210,
-                211
+                253,
+                179
             ],
             [
-                139,
-                194
+                246,
+                169
             ],
             [
-                194,
-                195,
-                196
+                248,
+                180
             ],
             [
-                198,
-                199
+                252,
+                181
             ],
             [
-                139,
-                149
+                247,
+                182
             ],
             [
-                202,
-                203,
-                204
+                249,
+                183
             ],
             [
-                201,
-                205,
-                206
-            ],
+                251,
+                184
+            ]
+        ],
+        "fileIdsList": [
             [
-                139,
-                157,
-                158
+                161
             ],
             [
-                159,
-                160
+                219,
+                222,
+                229,
+                230,
+                231,
+                232,
+                233
             ],
             [
-                157,
-                158,
                 161,
-                162,
-                163
+                216
             ],
             [
-                139,
-                145
+                216,
+                217,
+                218
             ],
             [
-                142
+                220,
+                221
             ],
             [
-                143
+                161,
+                171
             ],
             [
-                139,
-                140,
-                141
+                224,
+                225,
+                226
             ],
             [
-                140,
-                141,
-                142,
-                144,
-                145,
-                146,
-                147,
-                148
+                223,
+                227,
+                228
             ],
             [
-                213,
-                214,
-                215,
-                216,
-                217,
-                218,
-                219
+                161,
+                179,
+                180
             ],
             [
-                139,
-                155
+                181,
+                182
             ],
             [
-                139,
-                164
+                179,
+                180,
+                183,
+                184,
+                185
             ],
             [
-                151
+                161,
+                167
             ],
             [
-                139,
-                172,
-                173
+                164
             ],
             [
-                174
+                165
             ],
             [
-                139,
-                150,
-                151,
-                156,
-                165,
+                161,
+                162,
+                163
+            ],
+            [
+                162,
+                163,
+                164,
                 166,
                 167,
                 168,
                 169,
-                170,
-                171,
-                175,
-                176,
-                177,
-                178,
-                179,
-                180,
-                181,
-                182,
-                183,
-                184,
-                185,
+                170
+            ],
+            [
+                235,
+                236,
+                237,
+                238,
+                239,
+                240,
+                241
+            ],
+            [
+                161,
+                177
+            ],
+            [
+                161,
                 186
             ],
             [
-                37,
-                44,
-                45,
-                46
+                173
             ],
             [
-                44,
-                47
+                161,
+                194,
+                195
             ],
             [
-                37,
-                41
+                196
             ],
             [
-                37,
-                47
+                161,
+                172,
+                173,
+                178,
+                187,
+                188,
+                189,
+                190,
+                191,
+                192,
+                193,
+                197,
+                198,
+                199,
+                200,
+                201,
+                202,
+                203,
+                204,
+                205,
+                206,
+                207,
+                208
             ],
             [
-                35,
-                36,
-                45,
-                46,
-                47,
-                48
+                50,
+                57,
+                58,
+                59
             ],
             [
-                79,
-                93,
-                95
+                57,
+                60
             ],
             [
-                97
+                50,
+                54
             ],
             [
-                42,
-                43,
-                44,
-                99
+                50,
+                60
             ],
             [
-                42,
-                44
+                48,
+                49,
+                58,
+                59,
+                60,
+                61
             ],
             [
-                101,
-                103,
-                104
+                96,
+                115,
+                117
             ],
             [
-                101,
-                102
+                119
             ],
             [
-                106
+                55,
+                56,
+                57,
+                121
             ],
             [
-                35
+                55,
+                57
             ],
             [
-                38,
-                108
+                123,
+                125,
+                126
             ],
             [
-                108
+                123,
+                124
             ],
             [
-                111
+                128
             ],
             [
-                108,
-                109,
-                110
+                48
             ],
             [
-                108,
-                109,
-                110,
-                111,
-                112
+                51,
+                130
             ],
             [
-                39
+                130
             ],
             [
-                41,
-                42,
-                44
+                133
             ],
             [
-                97,
-                98
+                130,
+                131,
+                132
             ],
             [
-                114
+                130,
+                131,
+                132,
+                133,
+                134
             ],
             [
-                114,
-                118
+                52
             ],
             [
-                114,
-                115,
-                118,
-                119
+                54,
+                55,
+                57
             ],
             [
-                43,
-                117
+                119,
+                120
             ],
             [
-                94
+                136
             ],
             [
-                34,
-                40
+                136,
+                140
             ],
             [
-                65,
-                67,
-                93
+                136,
+                137,
+                140,
+                141
             ],
             [
-                37
+                56,
+                139
             ],
             [
-                37,
-                122,
-                123,
-                124
+                116
             ],
             [
-                34,
-                38,
-                39,
-                40,
-                41,
-                42,
-                43,
-                44,
-                49,
-                96,
-                97,
-                98,
-                99,
-                100,
-                102,
-                105,
-                106,
-                107,
-                113,
-                116,
-                117,
+                47,
+                53
+            ],
+            [
+                82,
+                84,
+                115
+            ],
+            [
+                50
+            ],
+            [
+                50,
+                144,
+                145,
+                146
+            ],
+            [
+                47,
+                51,
+                52,
+                53,
+                54,
+                55,
+                56,
+                57,
+                62,
+                118,
+                119,
                 120,
                 121,
-                125,
-                126,
+                122,
+                124,
                 127,
                 128,
                 129,
-                130,
-                131,
-                132,
-                133,
-                134,
-                136,
-                137,
-                138
+                135,
+                138,
+                139,
+                142,
+                143,
+                147,
+                148,
+                149,
+                150,
+                151,
+                152,
+                153,
+                154,
+                155,
+                156,
+                158,
+                159,
+                160
             ],
             [
-                35,
-                38,
-                39,
-                43
+                48,
+                51,
+                52,
+                56
             ],
             [
-                100
+                122
             ],
             [
-                116
+                138
             ],
             [
-                41,
-                43,
-                102
+                54,
+                56,
+                124
             ],
             [
-                41,
-                42
+                54,
+                55
             ],
             [
-                41,
-                106
+                54,
+                128
             ],
             [
-                43,
-                97,
-                98
+                56,
+                119,
+                120
             ],
             [
-                65,
-                79,
-                93,
-                95,
-                128
+                82,
+                96,
+                115,
+                117,
+                150
             ],
             [
-                42,
-                99,
-                133,
-                134
+                55,
+                121,
+                155,
+                156
             ],
             [
-                41,
-                65,
-                66,
-                93,
-                100,
-                128,
-                132,
-                134,
-                135
+                54,
+                82,
+                83,
+                115,
+                122,
+                150,
+                154,
+                156,
+                157
             ],
             [
-                41
+                54
             ],
             [
-                34
+                47
             ],
             [
-                79,
-                93,
-                139
+                96,
+                115,
+                161
             ],
             [
-                152,
-                153,
-                154
+                174,
+                175,
+                176
             ],
             [
-                79,
-                139
+                96,
+                161
             ],
             [
-                233,
-                234,
-                236,
-                239,
-                241
+                255,
+                256,
+                258,
+                261,
+                263
             ],
             [
-                233
+                255
             ],
             [
-                233,
-                236
+                255,
+                258
             ],
             [
-                243
+                265
             ],
             [
-                65,
-                93
+                82,
+                115
             ],
             [
-                248,
-                250
+                270,
+                272
             ],
             [
-                247,
-                248,
-                249
+                269,
+                270,
+                271
             ],
             [
-                63,
-                93
+                80,
+                115
             ],
             [
-                254
+                276
             ],
             [
-                255
+                277
             ],
             [
-                261,
-                264
+                283,
+                286
             ],
             [
-                259
+                281
             ],
             [
-                52,
-                93,
-                257,
-                263
+                66,
+                115,
+                279,
+                285
             ],
             [
-                261
+                283
             ],
             [
-                258,
-                262
+                280,
+                284
             ],
             [
-                260
+                282
             ],
             [
-                62,
-                88,
-                93,
-                278,
-                279,
-                281
+                79,
+                110,
+                115,
+                300,
+                301,
+                303
             ],
             [
-                280
+                302
             ],
             [
-                283,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                305,
+                307,
+                308,
+                309,
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317
             ],
             [
-                283,
-                284,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                305,
+                306,
+                308,
+                309,
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317
             ],
             [
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                306,
+                307,
+                308,
+                309,
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317
             ],
             [
-                283,
-                284,
-                285,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                305,
+                306,
+                307,
+                309,
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                305,
+                306,
+                307,
+                308,
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                305,
+                306,
+                307,
+                308,
+                309,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                290,
-                291,
-                292,
-                293,
-                294,
-                295
+                305,
+                306,
+                307,
+                308,
+                309,
+                310,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                291,
-                292,
-                293,
-                294,
-                295
+                305,
+                306,
+                307,
+                308,
+                309,
+                310,
+                311,
+                313,
+                314,
+                315,
+                316,
+                317
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                292,
-                293,
-                294,
-                295
+                305,
+                306,
+                307,
+                308,
+                309,
+                310,
+                311,
+                312,
+                314,
+                315,
+                316,
+                317
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                293,
-                294,
-                295
+                305,
+                306,
+                307,
+                308,
+                309,
+                310,
+                311,
+                312,
+                313,
+                315,
+                316,
+                317
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                294,
-                295
+                305,
+                306,
+                307,
+                308,
+                309,
+                310,
+                311,
+                312,
+                313,
+                314,
+                316,
+                317
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                295
+                305,
+                306,
+                307,
+                308,
+                309,
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                317
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294
+                305,
+                306,
+                307,
+                308,
+                309,
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316
             ],
             [
-                50
+                63
             ],
             [
-                52
+                66
             ],
             [
-                53,
-                58
+                67,
+                72,
+                99
+            ],
+            [
+                68,
+                79,
+                80,
+                87,
+                96,
+                107
+            ],
+            [
+                68,
+                69,
+                79,
+                87
             ],
             [
-                54,
-                62,
-                63,
                 70,
-                79
+                108
             ],
             [
-                54,
-                55,
-                62,
-                70
+                71,
+                72,
+                80,
+                88
             ],
             [
-                56,
-                86
+                72,
+                96,
+                104
             ],
             [
-                57,
-                58,
-                63,
-                71
+                73,
+                75,
+                79,
+                87
             ],
             [
-                58,
-                79
+                74
             ],
             [
-                59,
-                60,
-                62,
-                70
+                75,
+                76
             ],
             [
-                60
+                79
             ],
             [
-                61,
-                62
+                78,
+                79
             ],
             [
-                62
+                66,
+                79
             ],
             [
-                62,
-                63,
-                64,
                 79,
-                85
+                80,
+                81,
+                96,
+                107
             ],
             [
-                63,
-                64
+                79,
+                80,
+                81,
+                96
             ],
             [
-                62,
-                65,
-                70,
                 79,
-                85
+                82,
+                87,
+                96,
+                107
             ],
             [
-                62,
-                63,
-                65,
-                66,
-                70,
                 79,
+                80,
                 82,
-                85
+                83,
+                87,
+                96,
+                104,
+                107
             ],
             [
-                65,
-                67,
-                79,
                 82,
-                85
+                84,
+                96,
+                104,
+                107
             ],
             [
-                50,
-                51,
-                52,
-                53,
-                54,
-                55,
-                56,
-                57,
-                58,
-                59,
-                60,
-                61,
-                62,
                 63,
                 64,
                 65,
                 66,
                 67,
                 68,
                 69,
@@ -1782,155 +1814,184 @@
                 85,
                 86,
                 87,
                 88,
                 89,
                 90,
                 91,
-                92
+                92,
+                93,
+                94,
+                95,
+                96,
+                97,
+                98,
+                99,
+                100,
+                101,
+                102,
+                103,
+                104,
+                105,
+                106,
+                107,
+                108,
+                109,
+                110,
+                111,
+                112,
+                113,
+                114
             ],
             [
-                62,
-                68
+                79,
+                85
             ],
             [
-                69,
-                85
+                86,
+                107,
+                112
             ],
             [
-                60,
-                62,
-                70,
-                79
+                75,
+                79,
+                87,
+                96
             ],
             [
-                71
+                88
             ],
             [
-                72
+                89
             ],
             [
-                52,
-                73
+                66,
+                90
             ],
             [
-                74,
-                84
+                91,
+                106,
+                112
             ],
             [
-                75
+                92
             ],
             [
-                76
+                93
             ],
             [
-                62,
-                77
+                79,
+                94
             ],
             [
-                77,
-                78,
-                86,
-                88
+                94,
+                95,
+                108,
+                110
             ],
             [
-                62,
-                79
+                67,
+                79,
+                96,
+                97,
+                98
             ],
             [
-                80
+                67,
+                96,
+                98
             ],
             [
-                81
+                96,
+                97
+            ],
+            [
+                99
+            ],
+            [
+                100
             ],
             [
-                70,
                 79,
-                82
+                102,
+                103
             ],
             [
-                83
+                102,
+                103
             ],
             [
-                70,
-                84
+                72,
+                87,
+                96,
+                104
             ],
             [
-                65,
-                76,
-                85
+                105
             ],
             [
-                86
+                87,
+                106
             ],
             [
-                79,
-                87
+                67,
+                82,
+                93,
+                107
             ],
             [
-                88
+                72,
+                108
             ],
             [
-                89
+                96,
+                109
             ],
             [
-                62,
-                64,
-                79,
-                85,
-                88,
-                90
+                110
             ],
             [
+                111
+            ],
+            [
+                67,
+                72,
                 79,
-                91
+                81,
+                90,
+                96,
+                107,
+                110,
+                112
             ],
             [
-                301,
-                340
+                96,
+                113
             ],
             [
-                301,
-                325,
-                340
+                323,
+                362
             ],
             [
-                340
+                323,
+                347,
+                362
             ],
             [
-                301
+                362
             ],
             [
-                301,
-                326,
-                340
+                323
+            ],
+            [
+                323,
+                348,
+                362
             ],
             [
-                301,
-                302,
-                303,
-                304,
-                305,
-                306,
-                307,
-                308,
-                309,
-                310,
-                311,
-                312,
-                313,
-                314,
-                315,
-                316,
-                317,
-                318,
-                319,
-                320,
-                321,
-                322,
                 323,
                 324,
                 325,
                 326,
                 327,
                 328,
                 329,
@@ -1939,180 +2000,204 @@
                 332,
                 333,
                 334,
                 335,
                 336,
                 337,
                 338,
-                339
+                339,
+                340,
+                341,
+                342,
+                343,
+                344,
+                345,
+                346,
+                347,
+                348,
+                349,
+                350,
+                351,
+                352,
+                353,
+                354,
+                355,
+                356,
+                357,
+                358,
+                359,
+                360,
+                361
             ],
             [
-                326,
-                340
+                348,
+                362
             ],
             [
-                62,
-                65,
-                67,
-                70,
                 79,
                 82,
-                85,
-                91,
-                93
+                84,
+                87,
+                96,
+                104,
+                107,
+                113,
+                115
             ],
             [
-                344
+                366
             ],
             [
-                267
+                289
             ],
             [
-                266,
-                267
+                288,
+                289
             ],
             [
-                266
+                288
             ],
             [
-                266,
-                267,
-                268,
-                270,
-                271,
-                274,
-                275,
-                276,
-                277
+                288,
+                289,
+                290,
+                292,
+                293,
+                296,
+                297,
+                298,
+                299
             ],
             [
-                267,
-                271
+                289,
+                293
             ],
             [
-                266,
-                267,
-                268,
-                270,
-                271,
-                272,
-                273
+                288,
+                289,
+                290,
+                292,
+                293,
+                294,
+                295
             ],
             [
-                266,
-                271
+                288,
+                293
             ],
             [
-                271,
-                275
+                293,
+                297
             ],
             [
-                267,
-                268,
-                269
+                289,
+                290,
+                291
             ],
             [
-                268
+                290
             ],
             [
-                266,
-                267,
-                271
+                288,
+                289,
+                293
             ],
             [
-                31
+                44
             ],
             [
-                31,
-                32
+                44,
+                45
             ],
             [
-                31,
-                139,
-                149,
-                187,
-                192
+                44,
+                161,
+                171,
+                209,
+                214
             ],
             [
-                31,
-                193,
-                221
+                44,
+                215,
+                243
             ],
             [
-                31,
-                139,
-                212,
-                220
+                44,
+                161,
+                234,
+                242
             ],
             [
-                31,
-                222
+                44,
+                244
             ],
             [
-                31,
-                149
+                44,
+                171
             ],
             [
-                31,
-                190
+                44,
+                212
             ],
             [
-                31,
-                188,
-                189,
-                191
+                44,
+                210,
+                211,
+                213
             ],
             [
-                31,
-                189
+                44,
+                211
             ],
             [
-                31,
-                33,
-                223,
-                230
+                44,
+                46,
+                245,
+                252
             ],
             [
-                31,
-                139,
-                187
+                44,
+                161,
+                209
             ],
             [
-                31,
-                224,
-                225,
-                227,
-                229
+                44,
+                246,
+                247,
+                249,
+                251
             ],
             [
-                31,
-                187
+                44,
+                209
             ],
             [
-                31,
-                139,
-                226
+                44,
+                161,
+                248
             ],
             [
-                31,
-                139,
-                187,
-                226,
-                228
+                44,
+                161,
+                209,
+                248,
+                250
             ]
         ],
         "fileInfos": [
             {
                 "affectsGlobalScope": true,
                 "version": "8730f4bf322026ff5229336391a18bcaa1f94d4f82416c8b2f3954e2ccaae2ba"
             },
             "dc47c4fa66b9b9890cf076304de2a9c5201e94b740cffdf09f87296d877d71f6",
             "7a387c58583dfca701b6c85e0adaf43fb17d590fb16d5b2dc0a2fbd89f35c467",
             "8a12173c586e95f4433e0c6dc446bc88346be73ffe9ca6eec7aa63c8f3dca7f9",
             "5f4e733ced4e129482ae2186aae29fde948ab7182844c3a5a51dd346182c7b06",
+            "4b421cbfb3a38a27c279dec1e9112c3d1da296f77a1a85ddadf7e7a425d45d18",
+            "1fc5ab7a764205c68fa10d381b08417795fc73111d6dd16b5b1ed36badb743d9",
             {
                 "affectsGlobalScope": true,
                 "version": "3aafcb693fe5b5c3bd277bd4c3a617b53db474fe498fc5df067c5603b1eebde7"
             },
             {
                 "affectsGlobalScope": true,
                 "version": "f3d4da15233e593eacb3965cde7960f3fddf5878528d882bcedd5cbaba0193c7"
@@ -2195,22 +2280,66 @@
             },
             {
                 "affectsGlobalScope": true,
                 "version": "c80df75850fea5caa2afe43b9949338ce4e2de086f91713e9af1a06f973872b8"
             },
             {
                 "affectsGlobalScope": true,
+                "version": "9d57b2b5d15838ed094aa9ff1299eecef40b190722eb619bac4616657a05f951"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "6c51b5dd26a2c31dbf37f00cfc32b2aa6a92e19c995aefb5b97a3a64f1ac99de"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "6e7997ef61de3132e4d4b2250e75343f487903ddf5370e7ce33cf1b9db9a63ed"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "2ad234885a4240522efccd77de6c7d99eecf9b4de0914adb9a35c0c22433f993"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "5e5e095c4470c8bab227dbbc61374878ecead104c74ab9960d3adcccfee23205"
+            },
+            {
+                "affectsGlobalScope": true,
                 "version": "09aa50414b80c023553090e2f53827f007a301bc34b0495bfb2c3c08ab9ad1eb"
             },
             {
                 "affectsGlobalScope": true,
+                "version": "d7f680a43f8cd12a6b6122c07c54ba40952b0c8aa140dcfcf32eb9e6cb028596"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "3787b83e297de7c315d55d4a7c546ae28e5f6c0a361b7a1dcec1f1f50a54ef11"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "e7e8e1d368290e9295ef18ca23f405cf40d5456fa9f20db6373a61ca45f75f40"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "faf0221ae0465363c842ce6aa8a0cbda5d9296940a8e26c86e04cc4081eea21e"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "06393d13ea207a1bfe08ec8d7be562549c5e2da8983f2ee074e00002629d1871"
+            },
+            {
+                "affectsGlobalScope": true,
                 "version": "2768ef564cfc0689a1b76106c421a2909bdff0acbe87da010785adab80efdd5c"
             },
             {
                 "affectsGlobalScope": true,
+                "version": "b248e32ca52e8f5571390a4142558ae4f203ae2f94d5bac38a3084d529ef4e58"
+            },
+            {
+                "affectsGlobalScope": true,
                 "version": "52d1bb7ab7a3306fd0375c8bff560feed26ed676a5b0457fa8027b563aecb9a4"
             },
             "7a1971efcba559ea9002ada4c4e3c925004fb67a755300d53b5edf9399354900",
             "6d93b19d11edb10bce1aa933bae0fdf55c57785d376c4617e32506783791cd03",
             "38f6da5b6f318c33e18dd7c983cab3fe52f510c9a2573948fb13f012e01b1ba6",
             "c55ae709f94155174ff63647edd2a7e3acbd02a2909aa2541569e8b8bac9fc40",
             "530e5c7e4f74267b7800f1702cf0c576282296a960acbdb2960389b2b1d0875b",
@@ -2224,79 +2353,103 @@
             "b7b881ced4ed4dee13d6e0ccdb2296f66663ba6b1419767271090b3ff3478bb9",
             "06289b9873760aac77aed4035ea6c60b1e0879b8afe47a4530bc8522b9b804b1",
             "63c36aa73242aa745fae813c40585111ead225394b0a0ba985c2683baa6b0ef9",
             "3e7ffc7dd797e5d44d387d0892bc288480493e73dcab9832812907d1389e4a98",
             "db011ec9589fd51995cbd0765673838e38e6485a6559163cc53dcf508b480909",
             "e1a4253f0cca15c14516f52a2ad36c3520b140b5dfb3b3880a368cd75d45d6d9",
             "159af954f2633a12fdee68605009e7e5b150dbeb6d70c46672fd41059c154d53",
-            "4c2c4f53e8eedd970f8afa369d7371544fb6231bf95e659f8602e09abe74d5a5",
+            "5b3cd03ae354ea96eff1f74d7c410fe4852e6382227e8b0ecf87ab5e3a5bbcd4",
+            "7394959e5a741b185456e1ef5d64599c36c60a323207450991e7a42e08911419",
+            {
+                "affectsGlobalScope": true,
+                "version": "056097110efd16869ec118cedb44ecbac9a019576eee808d61304ca6d5cb2cbe"
+            },
+            "f51b4042a3ac86f1f707500a9768f88d0b0c1fc3f3e45a73333283dea720cdc6",
             {
                 "affectsGlobalScope": true,
-                "version": "cb5a780979155e80a2184eb987cc411a95c9a1686019ade06918c312a0b7c9b2"
+                "version": "6fb8358e10ed92a7f515b7d79da3904c955a3ffd4e14aa9df6f0ea113041f1cf"
             },
-            "c2b5085f47e41d6940bbc5b0d3bd7cc0037c752efb18aecd243c9cf83ad0c0b7",
-            "3143a5add0467b83150961ecd33773b561a1207aec727002aa1d70333068eb1b",
-            "f87191b7fafe7a0edad375710d99f900e49cef560b66bf309cf3f8e1b7177126",
-            "586af7d2abe2f9d59c5e757c370087d6c6baea81b033250f43b8df808d6dfb33",
+            "45c831238c6dac21c72da5f335747736a56a3847192bf03c84b958a7e9ec93e2",
+            "661a11d16ad2e3543a77c53bcd4017ee9a450f47ab7def3ab493a86eae4d550c",
             {
                 "affectsGlobalScope": true,
-                "version": "1a048ff164b8d9609f5de3139d4e37f6e8a82af82087ac414b9208f52ef8aac7"
+                "version": "8cdc646cec7819581ef343b83855b1bfe4fe674f2c84f4fb8dc90d82fb56bd3a"
             },
-            "3111079f3cb5f2b9c812ca3f46161562bce5bfb355e915f46ed46c41714dc1c3",
-            "e7bee4a6d9bb78afa390b25e0ce97a2f94787a1eb17f0a16e732dcbebba3f3ee",
-            "b32b6b16cb0bda68199582ad6f22242d07ee75fac9b1f28a98cd838afc5eea45",
-            "4441ee4119824bfaebc49308559edd7545978f9cb41a40f115074e1031dde75f",
+            "a40826e8476694e90da94aa008283a7de50d1dafd37beada623863f1901cb7fb",
+            "9dd56225cc2d8cb8fe5ceb0043ff386987637e12fecc6078896058a99deae284",
+            "2375ed4b439215aa3b6d0c6fd175c78a4384b30cb43cbadaecbf0a18954c98cb",
+            "7693b90b3075deaccafd5efb467bf9f2b747a3075be888652ef73e64396d8628",
+            "41231da15bb5e3e806a8395bd15c7befd2ec90f9f4e3c9d0ae1356bccb76dbb0",
+            "fccfef201d057cb407fa515311bd608549bab6c7b8adcf8f2df31f5d3b796478",
             {
                 "affectsGlobalScope": true,
-                "version": "60693a88462d0e97900123b5bf7c73e146ce0cc94da46a61fe6775b430d2ff05"
+                "version": "ee1ee365d88c4c6c0c0a5a5701d66ebc27ccd0bcfcfaa482c6e2e7fe7b98edf7"
             },
+            "5f20d20b7607174caf1a6da9141aeb9f2142159ae2410ca30c7a0fccd1d19c99",
             {
                 "affectsGlobalScope": true,
-                "version": "588c69eda58b9202676ec7ca11a72c3762819b46a0ed72462c769846153c447c"
+                "version": "464762c6213566d072f1ced5e8e9a954785ec5e53883b7397198abb5ef5b8f71"
             },
-            "ae064ed4f855716b7ff348639ddcd6a6d354a72fae82f506608a7dc9266aa24c",
-            "92f019c55b21c939616f6a48f678e714ac7b109444cbbf23ad69310ce66ecbdc",
-            "bba259efdf9ab95e0c7d3cc8e99250f56bb6b31d6129efdf733ca4eb1d01feea",
-            "499b7544062cf44fab253daeaea8ba28877d9e7ff4149246b1f0154d1c9ed535",
-            "139fd681eff7771a38d0c025d13c7a11c5474f6aab61e01c41511d71496df173",
-            "f614c3f61e46ccc2cb58702d5a158338ea57ee09099fde5db4cfc63ed0ce4d74",
-            "44e42ed6ec9c4451ebe89524e80ac8564e9dd0988c56e6c58f393c810730595d",
-            "a504c109b872b0e653549bd258eb06584c148c98d79406c7516995865a6d5089",
-            "155865f5f76db0996cd5e20cc5760613ea170ee5ad594c1f3d76fcaa05382161",
-            "e92852d673c836fc64e10c38640abcd67c463456e5df55723ac699b8e6ab3a8a",
-            "4455c78d226d061b1203c7614c6c6eb5f4f9db5f00d44ff47d0112de8766fbc4",
+            "6387920dc3e18927335b086deec75bf8e50f879a5e273d32ee7bb7a55ba50572",
+            "9bba37424094688c4663c177a1379b229f919b8912889a472f32fdc5f08ddb4d",
+            "29a4be13b3a30d3e66667b75c58ec61fb2df8fa0422534fdee3cfb30c5dbf450",
+            "83366d901beda79d6eb37aaaf6ca248dcd88946302b2a7d975590783be51e88e",
+            "bf268a0aea37ad4ae3b7a9b58559190b6fc01ea16a31e35cd05817a0a60f895a",
+            "43ec77c369473e92e2ecebf0554a0fdaa9c256644a6070f28228dfcceec77351",
             {
                 "affectsGlobalScope": true,
-                "version": "ec369bb9d97c4dc09dd2a4093b7ca3ba69ad284831fccac8a1977785e9e38ce5"
+                "version": "d7dad6db394a3d9f7b49755e4b610fbf8ed6eb0c9810ae5f1a119f6b5d76de45"
             },
-            "4465a636f5f6e9665a90e30691862c9e0a3ac2edc0e66296704f10865e924f2a",
-            "9af781f03d44f5635ed7844be0ce370d9d595d4b4ec67cad88f0fac03255257e",
-            "f9fd4c3ef6de27fa0e256f4e75b61711c4be05a3399f7714621d3edc832e36b0",
-            "e49290b7a927995c0d7e6b2b9c8296284b68a9036d9966531de65185269258d7",
-            "aa95cc73ea5315e4f6fc8c6db43d49e3b7de3780cae20a4f1319032809013038",
-            "874ca809b79276460011480a2829f4c8d4db29416dd411f71efbf8f497f0ac09",
-            "6c903bceaf3f3bc04f2d4c7dcd89ce9fb148b3ba0a5f5408d8f6de2b7eecc7ea",
-            "504d049d9e550a65466b73ca39da6469ab41786074ea1d16d37c8853f9f6ab2e",
-            "23a28f834a078986bbf58f4e3705956983ff81c3c2493f3db3e5f0e8a9507779",
-            "4febdf7f3ec92706c58e0b4e8159cd6de718284ef384260b07c9641c13fc70ce",
+            "95ed02bacb4502c985b69742ec82a4576d4ff4a6620ecc91593f611d502ae546",
+            "bf755525c4e6f85a970b98c4755d98e8aa1b6dbd83a5d8fcc57d3d497351b936",
+            "dd67d2b5e4e8a182a38de8e69fb736945eaa4588e0909c14e01a14bd3cc1fd1e",
             {
                 "affectsGlobalScope": true,
-                "version": "bf241ed073916ec9e21a3c138936edd444b6787d874844c0d05fc00a8f109d19"
+                "version": "28084e15b63e6211769db2fe646d8bc5c4c6776321e0deffe2d12eefd52cb6b9"
             },
-            "7335933d9f30dcfd2c4b6080a8b78e81912a7fcefb1dafccb67ca4cb4b3ac23d",
-            "a6bfe9de9adef749010c118104b071d14943802ff0614732b47ce4f1c3e383cd",
-            "4c3d0e10396646db4a1e917fb852077ee77ae62e512913bef9cccc2bb0f8bd0e",
-            "3b220849d58140dcc6718f5b52dcd29fdb79c45bc28f561cbd29eb1cac6cce13",
-            "0ee22fce41f7417a24c808d266e91b850629113c104713a35854393d55994beb",
-            "22d1b1d965baba05766613e2e6c753bb005d4386c448cafd72c309ba689e8c24",
             {
                 "affectsGlobalScope": true,
-                "version": "2708349d5a11a5c2e5f3a0765259ebe7ee00cdcc8161cb9990cb4910328442a1"
+                "version": "aed37dabf86c99d6c8508700576ecede86688397bc12523541858705a0c737c2"
             },
-            "c6c0bd221bb1e94768e94218f8298e47633495529d60cae7d8da9374247a1cf5",
+            "cc6ef5733d4ea6d2e06310a32dffd2c16418b467c5033d49cecc4f3a25de7497",
+            "94768454c3348b6ebe48e45fbad8c92e2bb7af4a35243edbe2b90823d0bd7f9a",
+            "0be79b3ff0f16b6c2f9bc8c4cc7097ea417d8d67f8267f7e1eec8e32b548c2ff",
+            "1c61ffa3a71b77363b30d19832c269ef62fba787f5610cac7254728d3b69ab2e",
+            "84da3c28344e621fd1d591f2c09e9595292d2b70018da28a553268ac122597d4",
+            "269929a24b2816343a178008ac9ae9248304d92a8ba8e233055e0ed6dbe6ef71",
+            "6e191fea1db6e9e4fa828259cf489e820ec9170effff57fb081a2f3295db4722",
+            "aed943465fbce1efe49ee16b5ea409050f15cd8eaf116f6fadb64ef0772e7d95",
+            "70d08483a67bf7050dbedace398ef3fee9f436fcd60517c97c4c1e22e3c6f3e8",
+            "c40fdf7b2e18df49ce0568e37f0292c12807a0748be79e272745e7216bed2606",
+            {
+                "affectsGlobalScope": true,
+                "version": "e933de8143e1d12dd51d89b398760fd5a9081896be366dad88a922d0b29f3c69"
+            },
+            "4e228e78c1e9b0a75c70588d59288f63a6258e8b1fe4a67b0c53fe03461421d9",
+            "b38d55d08708c2410a3039687db70b4a5bfa69fc4845617c313b5a10d9c5c637",
+            "205d50c24359ead003dc537b9b65d2a64208dfdffe368f403cf9e0357831db9e",
+            "1265fddcd0c68be9d2a3b29805d0280484c961264dd95e0b675f7bd91f777e78",
+            {
+                "affectsGlobalScope": true,
+                "version": "a05e2d784c9be7051c4ac87a407c66d2106e23490c18c038bbd0712bde7602fd"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "df90b9d0e9980762da8daf8adf6ffa0c853e76bfd269c377be0d07a9ad87acd2"
+            },
+            "cf434b5c04792f62d6f4bdd5e2c8673f36e638e910333c172614d5def9b17f98",
+            "1d65d4798df9c2df008884035c41d3e67731f29db5ecb64cd7378797c7c53a2f",
+            "0faee6b555890a1cb106e2adc5d3ffd89545b1da894d474e9d436596d654998f",
+            "c6c01ea1c42508edf11a36d13b70f6e35774f74355ba5d358354d4a77cc67ea1",
+            "867f95abf1df444aab146b19847391fc2f922a55f6a970a27ed8226766cee29f",
+            {
+                "affectsGlobalScope": true,
+                "version": "ab9b9a36e5284fd8d3bf2f7d5fcbc60052f25f27e4d20954782099282c60d23e"
+            },
+            "b0297b09e607bec9698cac7cf55463d6731406efb1161ee4d448293b47397c84",
             "a1b36a1f91a54daf2e89e12b834fa41fb7338bc044d1f08a80817efc93c99ee5",
             "8bb4a5b632dd5a868f3271750895cb61b0e20cff82032d87e89288faee8dd6e2",
             "0c1aabfd9fb1818afb2e798f91f669edafce59cd7e3423d25b1cfccfaaf2c403",
             "017de6fdabea79015d493bf71e56cbbff092525253c1d76003b3d58280cd82a0",
             "ab9ea2596cb7800bd79d1526930c785606ec4f439c275adbca5adc1ddf87747d",
             "aee8faa433dde04beedb779b3329456a286a966462d666c138c19113ce78c79e",
             "d620ec36bfc6f8ed6fdecbe036d55cec81637f32fd34dc7bb7e60eba1764e910",
@@ -2566,14 +2719,16 @@
         ],
         "fileNames": [
             "../../node_modules/typescript/lib/lib.es5.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.d.ts",
             "../../node_modules/typescript/lib/lib.es2016.d.ts",
             "../../node_modules/typescript/lib/lib.es2017.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.d.ts",
             "../../node_modules/typescript/lib/lib.dom.d.ts",
             "../../node_modules/typescript/lib/lib.dom.iterable.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.core.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.collection.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.generator.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.iterable.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.promise.d.ts",
@@ -2588,16 +2743,27 @@
             "../../node_modules/typescript/lib/lib.es2017.intl.d.ts",
             "../../node_modules/typescript/lib/lib.es2017.typedarrays.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.asyncgenerator.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.asynciterable.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.intl.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.promise.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.regexp.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.array.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.object.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.string.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.symbol.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.intl.d.ts",
             "../../node_modules/typescript/lib/lib.es2020.bigint.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.date.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.promise.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.sharedmemory.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.string.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.symbol.wellknown.d.ts",
             "../../node_modules/typescript/lib/lib.es2020.intl.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.number.d.ts",
             "../../node_modules/typescript/lib/lib.esnext.intl.d.ts",
             "../../node_modules/tslib/tslib.d.ts",
             "./src/client/emitWarningIfUnsupportedVersion.ts",
             "./src/client/index.ts",
             "../../node_modules/@smithy/types/dist-types/abort.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/auth.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/HttpApiKeyAuth.d.ts",
@@ -2611,24 +2777,28 @@
             "../../node_modules/@smithy/types/dist-types/middleware.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/HttpSigner.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/IdentityProviderConfig.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/HttpAuthScheme.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/HttpAuthSchemeProvider.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/index.d.ts",
             "../../node_modules/@types/node/assert.d.ts",
+            "../../node_modules/@types/node/assert/strict.d.ts",
             "../../node_modules/@types/node/globals.d.ts",
             "../../node_modules/@types/node/async_hooks.d.ts",
             "../../node_modules/@types/node/buffer.d.ts",
             "../../node_modules/@types/node/child_process.d.ts",
             "../../node_modules/@types/node/cluster.d.ts",
             "../../node_modules/@types/node/console.d.ts",
             "../../node_modules/@types/node/constants.d.ts",
             "../../node_modules/@types/node/crypto.d.ts",
             "../../node_modules/@types/node/dgram.d.ts",
+            "../../node_modules/@types/node/diagnostics_channel.d.ts",
             "../../node_modules/@types/node/dns.d.ts",
+            "../../node_modules/@types/node/dns/promises.d.ts",
+            "../../node_modules/@types/node/dom-events.d.ts",
             "../../node_modules/@types/node/domain.d.ts",
             "../../node_modules/@types/node/events.d.ts",
             "../../node_modules/@types/node/fs.d.ts",
             "../../node_modules/@types/node/fs/promises.d.ts",
             "../../node_modules/@types/node/http.d.ts",
             "../../node_modules/@types/node/http2.d.ts",
             "../../node_modules/@types/node/https.d.ts",
@@ -2640,16 +2810,21 @@
             "../../node_modules/@types/node/perf_hooks.d.ts",
             "../../node_modules/@types/node/process.d.ts",
             "../../node_modules/@types/node/punycode.d.ts",
             "../../node_modules/@types/node/querystring.d.ts",
             "../../node_modules/@types/node/readline.d.ts",
             "../../node_modules/@types/node/repl.d.ts",
             "../../node_modules/@types/node/stream.d.ts",
+            "../../node_modules/@types/node/stream/promises.d.ts",
+            "../../node_modules/@types/node/stream/consumers.d.ts",
+            "../../node_modules/@types/node/stream/web.d.ts",
             "../../node_modules/@types/node/string_decoder.d.ts",
+            "../../node_modules/@types/node/test.d.ts",
             "../../node_modules/@types/node/timers.d.ts",
+            "../../node_modules/@types/node/timers/promises.d.ts",
             "../../node_modules/@types/node/tls.d.ts",
             "../../node_modules/@types/node/trace_events.d.ts",
             "../../node_modules/@types/node/tty.d.ts",
             "../../node_modules/@types/node/url.d.ts",
             "../../node_modules/@types/node/util.d.ts",
             "../../node_modules/@types/node/v8.d.ts",
             "../../node_modules/@types/node/vm.d.ts",
@@ -2920,1383 +3095,1438 @@
             "module": 99,
             "noEmitHelpers": false,
             "noFallthroughCasesInSwitch": true,
             "outDir": "./dist-es",
             "preserveConstEnums": true,
             "removeComments": true,
             "rootDir": "./src",
+            "skipLibCheck": true,
             "strict": true,
-            "target": 7,
+            "target": 8,
             "useUnknownInCatchVariables": false
         },
         "referencedMap": [
             [
-                208,
+                230,
                 1
             ],
             [
-                212,
+                234,
                 2
             ],
             [
-                195,
+                217,
                 3
             ],
             [
-                196,
+                218,
                 3
             ],
             [
-                194,
+                216,
                 1
             ],
             [
-                197,
+                219,
                 4
             ],
             [
-                199,
+                221,
                 1
             ],
             [
-                198,
+                220,
                 1
             ],
             [
-                200,
+                222,
                 5
             ],
             [
-                209,
+                231,
                 1
             ],
             [
-                211,
+                233,
                 1
             ],
             [
-                210,
+                232,
                 6
             ],
             [
-                201,
+                223,
                 1
             ],
             [
-                202,
+                224,
                 6
             ],
             [
-                203,
+                225,
                 6
             ],
             [
-                205,
+                227,
                 7
             ],
             [
-                204,
+                226,
                 1
             ],
             [
-                207,
+                229,
                 8
             ],
             [
-                206,
+                228,
                 1
             ],
             [
-                159,
+                181,
                 9
             ],
             [
-                161,
+                183,
                 10
             ],
             [
-                160,
+                182,
                 1
             ],
             [
-                162,
+                184,
                 9
             ],
             [
-                163,
+                185,
                 9
             ],
             [
-                164,
+                186,
                 11
             ],
             [
-                157,
+                179,
                 1
             ],
             [
-                145,
+                167,
                 1
             ],
             [
-                146,
+                168,
                 12
             ],
             [
-                143,
+                165,
                 13
             ],
             [
-                144,
+                166,
                 14
             ],
             [
-                142,
+                164,
                 15
             ],
             [
-                140,
+                162,
                 1
             ],
             [
-                141,
+                163,
                 1
             ],
             [
-                149,
+                171,
                 16
             ],
             [
-                148,
+                170,
                 1
             ],
             [
-                213,
+                235,
                 1
             ],
             [
-                219,
+                241,
                 1
             ],
             [
-                214,
+                236,
                 1
             ],
             [
-                215,
+                237,
                 1
             ],
             [
-                216,
+                238,
                 1
             ],
             [
-                220,
+                242,
                 17
             ],
             [
-                217,
+                239,
                 1
             ],
             [
-                218,
+                240,
                 1
             ],
             [
-                150,
+                172,
                 1
             ],
             [
-                151,
+                173,
                 1
             ],
             [
-                156,
+                178,
                 18
             ],
             [
-                165,
+                187,
                 19
             ],
             [
-                167,
+                189,
                 20
             ],
             [
-                176,
+                198,
                 1
             ],
             [
-                172,
+                194,
                 1
             ],
             [
-                174,
+                196,
                 21
             ],
             [
-                175,
+                197,
                 22
             ],
             [
-                173,
+                195,
                 1
             ],
             [
-                187,
+                209,
                 23
             ],
             [
-                47,
+                60,
                 24
             ],
             [
-                48,
+                61,
                 25
             ],
             [
-                45,
+                58,
                 26
             ],
             [
-                46,
+                59,
                 27
             ],
             [
-                49,
+                62,
                 28
             ],
             [
-                96,
+                118,
                 29
             ],
             [
-                98,
+                120,
                 30
             ],
             [
-                100,
+                122,
                 31
             ],
             [
-                99,
+                121,
                 32
             ],
             [
-                105,
+                127,
                 33
             ],
             [
-                103,
+                125,
                 34
             ],
             [
-                107,
+                129,
                 35
             ],
             [
-                38,
+                51,
                 36
             ],
             [
-                109,
+                131,
                 37
             ],
             [
-                110,
+                132,
                 38
             ],
             [
-                112,
+                134,
                 39
             ],
             [
-                111,
+                133,
                 40
             ],
             [
-                113,
+                135,
                 41
             ],
             [
-                108,
+                130,
                 42
             ],
             [
-                106,
+                128,
                 43
             ],
             [
-                114,
+                136,
                 44
             ],
             [
-                115,
+                137,
                 45
             ],
             [
-                119,
+                141,
                 46
             ],
             [
-                120,
+                142,
                 47
             ],
             [
-                118,
+                140,
                 48
             ],
             [
-                95,
+                117,
                 49
             ],
             [
-                41,
+                54,
                 50
             ],
             [
-                121,
+                143,
                 51
             ],
             [
-                122,
+                144,
                 52
             ],
             [
-                123,
+                145,
                 52
             ],
             [
-                125,
+                147,
                 53
             ],
             [
-                124,
+                146,
                 52
             ],
             [
-                139,
+                161,
                 54
             ],
             [
-                44,
+                57,
                 55
             ],
             [
-                126,
+                148,
                 56
             ],
             [
-                117,
+                139,
                 57
             ],
             [
-                128,
+                150,
                 58
             ],
             [
-                116,
+                138,
                 59
             ],
             [
-                129,
+                151,
                 60
             ],
             [
-                130,
+                152,
                 61
             ],
             [
-                131,
+                153,
                 29
             ],
             [
-                132,
+                154,
                 29
             ],
             [
-                133,
+                155,
                 62
             ],
             [
-                135,
+                157,
                 63
             ],
             [
-                136,
+                158,
                 64
             ],
             [
-                137,
+                159,
                 56
             ],
             [
-                40,
+                53,
                 65
             ],
             [
-                43,
+                56,
                 43
             ],
             [
-                138,
+                160,
                 66
             ],
             [
-                153,
+                175,
                 67
             ],
             [
-                155,
+                177,
                 68
             ],
             [
-                154,
+                176,
                 69
             ],
             [
-                242,
+                264,
                 70
             ],
             [
-                236,
+                258,
                 71
             ],
             [
-                234,
+                256,
                 71
             ],
             [
-                239,
+                261,
                 72
             ],
             [
-                237,
+                259,
                 71
             ],
             [
-                241,
+                263,
                 71
             ],
             [
-                244,
+                266,
                 73
             ],
             [
-                245,
+                267,
                 73
             ],
             [
-                246,
+                268,
                 74
             ],
             [
-                251,
+                273,
                 75
             ],
             [
-                250,
+                272,
                 76
             ],
             [
-                252,
+                274,
                 77
             ],
             [
-                253,
+                275,
                 77
             ],
             [
-                255,
+                277,
                 78
             ],
             [
-                256,
+                278,
                 79
             ],
             [
-                265,
+                287,
                 80
             ],
             [
-                260,
+                282,
                 81
             ],
             [
-                264,
+                286,
                 82
             ],
             [
-                262,
+                284,
                 83
             ],
             [
-                263,
+                285,
                 84
             ],
             [
-                261,
+                283,
                 85
             ],
             [
-                280,
+                302,
                 86
             ],
             [
-                281,
+                303,
                 87
             ],
             [
-                284,
+                306,
                 88
             ],
             [
-                285,
+                307,
                 89
             ],
             [
-                283,
+                305,
                 90
             ],
             [
-                286,
+                308,
                 91
             ],
             [
-                287,
+                309,
                 92
             ],
             [
-                288,
+                310,
                 93
             ],
             [
-                289,
+                311,
                 94
             ],
             [
-                290,
+                312,
                 95
             ],
             [
-                291,
+                313,
                 96
             ],
             [
-                292,
+                314,
                 97
             ],
             [
-                293,
+                315,
                 98
             ],
             [
-                294,
+                316,
                 99
             ],
             [
-                295,
+                317,
                 100
             ],
             [
-                50,
+                63,
                 101
             ],
             [
-                52,
+                64,
+                101
+            ],
+            [
+                66,
                 102
             ],
             [
-                53,
+                67,
                 103
             ],
             [
-                54,
+                68,
                 104
             ],
             [
-                55,
+                69,
                 105
             ],
             [
-                56,
+                70,
                 106
             ],
             [
-                57,
+                71,
                 107
             ],
             [
-                58,
+                72,
                 108
             ],
             [
-                59,
+                73,
                 109
             ],
             [
-                60,
+                74,
                 110
             ],
             [
-                61,
+                75,
                 111
             ],
             [
-                62,
+                76,
+                111
+            ],
+            [
+                77,
                 112
             ],
             [
-                63,
+                78,
                 113
             ],
             [
-                64,
+                79,
                 114
             ],
             [
-                65,
+                80,
                 115
             ],
             [
-                66,
+                81,
                 116
             ],
             [
-                67,
+                82,
                 117
             ],
             [
-                93,
+                83,
                 118
             ],
             [
-                68,
+                84,
                 119
             ],
             [
-                69,
+                115,
                 120
             ],
             [
-                70,
+                85,
                 121
             ],
             [
-                71,
+                86,
                 122
             ],
             [
-                72,
+                87,
                 123
             ],
             [
-                73,
+                88,
                 124
             ],
             [
-                74,
+                89,
                 125
             ],
             [
-                75,
+                90,
                 126
             ],
             [
-                76,
+                91,
                 127
             ],
             [
-                77,
+                92,
                 128
             ],
             [
-                78,
+                93,
                 129
             ],
             [
-                79,
+                94,
                 130
             ],
             [
-                80,
+                95,
                 131
             ],
             [
-                81,
+                96,
                 132
             ],
             [
-                82,
+                98,
                 133
             ],
             [
-                83,
+                97,
                 134
             ],
             [
-                84,
+                99,
                 135
             ],
             [
-                85,
+                100,
                 136
             ],
             [
-                86,
+                102,
                 137
             ],
             [
-                87,
+                103,
                 138
             ],
             [
-                88,
+                104,
                 139
             ],
             [
-                89,
+                105,
                 140
             ],
             [
-                90,
+                106,
                 141
             ],
             [
-                91,
+                107,
                 142
             ],
             [
-                325,
+                108,
                 143
             ],
             [
-                326,
+                109,
                 144
             ],
             [
-                301,
+                110,
                 145
             ],
             [
-                304,
-                145
+                111,
+                146
             ],
             [
-                323,
-                143
+                112,
+                147
             ],
             [
-                324,
-                143
+                113,
+                148
             ],
             [
-                314,
-                143
+                347,
+                149
             ],
             [
-                313,
-                146
+                348,
+                150
             ],
             [
-                311,
-                143
+                323,
+                151
             ],
             [
-                306,
-                143
+                326,
+                151
             ],
             [
-                319,
-                143
+                345,
+                149
             ],
             [
-                317,
-                143
+                346,
+                149
             ],
             [
-                321,
-                143
+                336,
+                149
             ],
             [
-                305,
-                143
+                335,
+                152
             ],
             [
-                318,
-                143
+                333,
+                149
             ],
             [
-                322,
-                143
+                328,
+                149
             ],
             [
-                307,
-                143
+                341,
+                149
             ],
             [
-                308,
-                143
+                339,
+                149
             ],
             [
-                320,
-                143
+                343,
+                149
             ],
             [
-                302,
-                143
+                327,
+                149
             ],
             [
-                309,
-                143
+                340,
+                149
             ],
             [
-                310,
-                143
+                344,
+                149
             ],
             [
-                312,
-                143
+                329,
+                149
             ],
             [
-                316,
-                143
+                330,
+                149
             ],
             [
-                327,
-                147
+                342,
+                149
             ],
             [
-                315,
-                143
+                324,
+                149
             ],
             [
-                303,
-                143
+                331,
+                149
             ],
             [
-                340,
-                148
+                332,
+                149
             ],
             [
                 334,
-                147
+                149
             ],
             [
-                336,
+                338,
                 149
             ],
             [
-                335,
-                147
+                349,
+                153
             ],
             [
-                328,
-                147
+                337,
+                149
             ],
             [
-                329,
-                147
+                325,
+                149
             ],
             [
-                331,
-                147
+                362,
+                154
             ],
             [
-                333,
-                147
+                356,
+                153
             ],
             [
-                337,
-                149
+                358,
+                155
             ],
             [
-                338,
-                149
+                357,
+                153
             ],
             [
-                330,
-                149
+                350,
+                153
             ],
             [
-                332,
-                149
+                351,
+                153
             ],
             [
-                343,
-                150
+                353,
+                153
             ],
             [
-                345,
-                151
+                355,
+                153
             ],
             [
-                268,
-                152
+                359,
+                155
             ],
             [
-                277,
-                153
+                360,
+                155
             ],
             [
-                267,
-                154
+                352,
+                155
             ],
             [
-                278,
+                354,
                 155
             ],
             [
-                273,
+                365,
                 156
             ],
             [
-                274,
+                367,
                 157
             ],
             [
-                272,
+                290,
                 158
             ],
             [
-                276,
+                299,
                 159
             ],
             [
-                270,
+                289,
                 160
             ],
             [
-                269,
+                300,
                 161
             ],
             [
-                275,
+                295,
                 162
             ],
             [
-                271,
-                153
-            ],
-            [
-                32,
+                296,
                 163
             ],
             [
-                33,
+                294,
                 164
             ],
             [
-                193,
+                298,
                 165
             ],
             [
-                222,
+                292,
                 166
             ],
             [
-                221,
+                291,
                 167
             ],
             [
-                223,
+                297,
                 168
             ],
             [
-                188,
-                169
+                293,
+                159
             ],
             [
-                189,
-                163
+                45,
+                169
             ],
             [
-                191,
+                46,
                 170
             ],
             [
-                192,
+                215,
                 171
             ],
             [
-                190,
+                244,
                 172
             ],
             [
-                231,
+                243,
                 173
             ],
             [
-                224,
-                163
-            ],
-            [
-                226,
+                245,
                 174
             ],
             [
-                230,
+                210,
                 175
             ],
             [
-                225,
+                211,
+                169
+            ],
+            [
+                213,
                 176
             ],
             [
-                227,
+                214,
                 177
             ],
             [
-                229,
+                212,
                 178
+            ],
+            [
+                253,
+                179
+            ],
+            [
+                246,
+                169
+            ],
+            [
+                248,
+                180
+            ],
+            [
+                252,
+                181
+            ],
+            [
+                247,
+                182
+            ],
+            [
+                249,
+                183
+            ],
+            [
+                251,
+                184
             ]
         ],
         "semanticDiagnosticsPerFile": [
-            259,
-            208,
-            212,
-            195,
-            196,
-            194,
-            197,
-            199,
-            198,
-            200,
-            209,
-            211,
-            210,
-            201,
-            202,
-            203,
-            205,
-            204,
-            207,
-            206,
-            159,
-            161,
-            160,
-            162,
-            163,
-            164,
-            157,
-            158,
-            145,
-            146,
-            143,
-            144,
-            142,
-            140,
-            141,
-            149,
-            147,
-            148,
-            213,
-            219,
-            214,
-            215,
-            216,
-            220,
+            281,
+            230,
+            234,
             217,
             218,
-            150,
-            151,
-            156,
-            165,
-            166,
+            216,
+            219,
+            221,
+            220,
+            222,
+            231,
+            233,
+            232,
+            223,
+            224,
+            225,
+            227,
+            226,
+            229,
+            228,
+            181,
+            183,
+            182,
+            184,
+            185,
+            186,
+            179,
+            180,
             167,
             168,
+            165,
+            166,
+            164,
+            162,
+            163,
+            171,
             169,
             170,
-            171,
-            176,
-            177,
+            235,
+            241,
+            236,
+            237,
+            238,
+            242,
+            239,
+            240,
             172,
-            174,
-            175,
             173,
             178,
-            179,
             187,
-            180,
-            181,
-            182,
-            183,
-            184,
-            185,
-            186,
-            34,
-            36,
+            188,
+            189,
+            190,
+            191,
+            192,
+            193,
+            198,
+            199,
+            194,
+            196,
+            197,
+            195,
+            200,
+            201,
+            209,
+            202,
+            203,
+            204,
+            205,
+            206,
+            207,
+            208,
             47,
-            48,
-            45,
-            46,
-            35,
             49,
-            96,
-            98,
-            100,
-            99,
-            101,
-            105,
-            103,
-            104,
-            97,
-            107,
-            38,
-            109,
-            110,
-            112,
-            111,
-            113,
-            108,
-            106,
-            114,
-            115,
-            119,
-            120,
+            60,
+            61,
+            58,
+            59,
+            48,
+            62,
             118,
-            95,
-            41,
-            121,
+            120,
             122,
+            121,
             123,
-            37,
+            127,
             125,
-            124,
-            139,
-            39,
-            44,
             126,
-            127,
-            42,
-            117,
-            128,
-            116,
+            119,
             129,
-            130,
+            51,
             131,
             132,
+            134,
             133,
-            102,
             135,
+            130,
+            128,
             136,
-            94,
             137,
-            134,
-            40,
-            43,
+            141,
+            142,
+            140,
+            117,
+            54,
+            143,
+            144,
+            145,
+            50,
+            147,
+            146,
+            161,
+            52,
+            57,
+            148,
+            149,
+            55,
+            139,
+            150,
             138,
+            151,
             152,
             153,
-            155,
             154,
-            232,
-            242,
-            236,
-            235,
-            234,
-            233,
-            239,
-            237,
-            238,
-            241,
-            240,
-            244,
-            245,
-            243,
-            246,
-            251,
-            247,
-            250,
-            248,
-            252,
-            253,
+            155,
+            124,
+            157,
+            158,
+            116,
+            159,
+            156,
+            53,
+            56,
+            160,
+            174,
+            175,
+            177,
+            176,
             254,
-            255,
-            256,
-            265,
+            264,
+            258,
             257,
+            256,
+            255,
+            261,
+            259,
             260,
-            264,
-            262,
             263,
-            261,
-            280,
-            281,
-            249,
+            262,
+            266,
+            267,
+            265,
+            268,
+            273,
+            269,
+            272,
+            270,
+            274,
+            275,
+            276,
+            277,
+            278,
+            287,
+            279,
             282,
+            286,
             284,
             285,
             283,
-            286,
-            287,
-            288,
-            289,
-            290,
-            291,
-            292,
-            293,
-            294,
-            295,
-            296,
-            297,
-            50,
-            52,
-            53,
-            54,
-            55,
-            56,
-            57,
-            58,
-            59,
-            60,
-            61,
-            62,
+            302,
+            303,
+            271,
+            304,
+            306,
+            307,
+            305,
+            308,
+            309,
+            310,
+            311,
+            312,
+            313,
+            314,
+            315,
+            316,
+            317,
+            318,
+            319,
             63,
             64,
-            51,
-            92,
-            65,
             66,
             67,
-            93,
             68,
             69,
             70,
             71,
             72,
             73,
             74,
             75,
             76,
             77,
             78,
             79,
             80,
             81,
+            65,
+            114,
             82,
             83,
             84,
+            115,
             85,
             86,
             87,
             88,
             89,
             90,
             91,
-            298,
-            299,
-            300,
-            325,
-            326,
-            301,
-            304,
-            323,
-            324,
-            314,
-            313,
-            311,
-            306,
-            319,
-            317,
+            92,
+            93,
+            94,
+            95,
+            96,
+            98,
+            97,
+            99,
+            100,
+            101,
+            102,
+            103,
+            104,
+            105,
+            106,
+            107,
+            108,
+            109,
+            110,
+            111,
+            112,
+            113,
+            320,
             321,
-            305,
-            318,
             322,
-            307,
-            308,
-            320,
-            302,
-            309,
-            310,
-            312,
-            316,
-            327,
-            315,
-            303,
-            340,
-            339,
-            334,
+            347,
+            348,
+            323,
+            326,
+            345,
+            346,
             336,
             335,
-            328,
-            329,
-            331,
             333,
-            337,
-            338,
-            330,
-            332,
+            328,
             341,
-            279,
-            342,
+            339,
             343,
+            327,
+            340,
             344,
-            345,
-            258,
-            228,
-            268,
-            277,
-            266,
-            267,
-            278,
-            273,
-            274,
-            272,
-            276,
-            270,
-            269,
-            275,
-            271,
-            31,
-            6,
-            7,
-            9,
+            329,
+            330,
+            342,
+            324,
+            331,
+            332,
+            334,
+            338,
+            349,
+            337,
+            325,
+            362,
+            361,
+            356,
+            358,
+            357,
+            350,
+            351,
+            353,
+            355,
+            359,
+            360,
+            352,
+            354,
+            363,
+            301,
+            364,
+            365,
+            366,
+            367,
+            280,
+            250,
+            290,
+            299,
+            288,
+            289,
+            300,
+            295,
+            296,
+            294,
+            298,
+            292,
+            291,
+            297,
+            293,
+            44,
             8,
-            2,
-            10,
+            9,
             11,
+            10,
+            2,
             12,
             13,
             14,
             15,
             16,
             17,
-            3,
-            4,
-            21,
             18,
             19,
+            3,
+            4,
+            23,
             20,
+            21,
             22,
-            23,
             24,
-            5,
             25,
             26,
+            5,
             27,
             28,
             29,
-            1,
             30,
+            6,
+            34,
+            31,
             32,
             33,
-            193,
-            222,
-            221,
-            223,
-            188,
-            189,
-            191,
-            192,
-            190,
-            231,
-            224,
-            226,
-            230,
-            225,
-            227,
-            229
+            35,
+            7,
+            36,
+            41,
+            42,
+            37,
+            38,
+            39,
+            40,
+            1,
+            43,
+            45,
+            46,
+            215,
+            244,
+            243,
+            245,
+            210,
+            211,
+            213,
+            214,
+            212,
+            253,
+            246,
+            248,
+            252,
+            247,
+            249,
+            251
         ]
     },
     "version": "4.9.5"
 }
```

##### package/node_modules/@aws-sdk/core/tsconfig.types.tsbuildinfo

###### Pretty-printed

 * *Similarity: 0.9314734272714922%*

 * *Differences: {"'program'": "{'fileNames': {insert: [(5, '../../node_modules/typescript/lib/lib.es2019.d.ts'), "*

 * *              "(6, '../../node_modules/typescript/lib/lib.es2020.d.ts'), (7, "*

 * *              "'../../node_modules/typescript/lib/lib.es2021.d.ts'), (30, "*

 * *              "'../../node_modules/typescript/lib/lib.es2019.array.d.ts'), (31, "*

 * *              "'../../node_modules/typescript/lib/lib.es2019.object.d.ts'), (32, "*

 * *              "'../../node_modules/typescript/lib/lib.es2019.string.d.ts'), (33, "*

 * *           […]*

```diff
@@ -1,1744 +1,1770 @@
 {
     "program": {
         "exportedModulesMap": [
             [
-                207,
+                235,
                 1
             ],
             [
-                211,
+                239,
                 2
             ],
             [
-                194,
+                222,
                 3
             ],
             [
-                195,
+                223,
                 3
             ],
             [
-                193,
+                221,
                 1
             ],
             [
-                196,
+                224,
                 4
             ],
             [
-                198,
+                226,
                 1
             ],
             [
-                197,
+                225,
                 1
             ],
             [
-                199,
+                227,
                 5
             ],
             [
-                208,
+                236,
                 1
             ],
             [
-                210,
+                238,
                 1
             ],
             [
-                209,
+                237,
                 6
             ],
             [
-                200,
+                228,
                 1
             ],
             [
-                201,
+                229,
                 6
             ],
             [
-                202,
+                230,
                 6
             ],
             [
-                204,
+                232,
                 7
             ],
             [
-                203,
+                231,
                 1
             ],
             [
-                206,
+                234,
                 8
             ],
             [
-                205,
+                233,
                 1
             ],
             [
-                158,
+                186,
                 9
             ],
             [
-                160,
+                188,
                 10
             ],
             [
-                159,
+                187,
                 1
             ],
             [
-                161,
+                189,
                 9
             ],
             [
-                162,
+                190,
                 9
             ],
             [
-                163,
+                191,
                 11
             ],
             [
-                156,
+                184,
                 1
             ],
             [
-                144,
+                172,
                 1
             ],
             [
-                145,
+                173,
                 12
             ],
             [
-                142,
+                170,
                 13
             ],
             [
-                143,
+                171,
                 14
             ],
             [
-                141,
+                169,
                 15
             ],
             [
-                139,
+                167,
                 1
             ],
             [
-                140,
+                168,
                 1
             ],
             [
-                148,
+                176,
                 16
             ],
             [
-                147,
+                175,
                 1
             ],
             [
-                212,
+                240,
                 1
             ],
             [
-                218,
+                246,
                 1
             ],
             [
-                213,
+                241,
                 1
             ],
             [
-                214,
+                242,
                 1
             ],
             [
-                215,
+                243,
                 1
             ],
             [
-                219,
+                247,
                 17
             ],
             [
-                216,
+                244,
                 1
             ],
             [
-                217,
+                245,
                 1
             ],
             [
-                149,
+                177,
                 1
             ],
             [
-                150,
+                178,
                 1
             ],
             [
-                155,
+                183,
                 18
             ],
             [
-                164,
+                192,
                 19
             ],
             [
-                166,
+                194,
                 20
             ],
             [
-                175,
+                203,
                 1
             ],
             [
-                171,
+                199,
                 1
             ],
             [
-                173,
+                201,
                 21
             ],
             [
-                174,
+                202,
                 22
             ],
             [
-                172,
+                200,
                 1
             ],
             [
-                186,
+                214,
                 23
             ],
             [
-                46,
+                65,
                 24
             ],
             [
-                47,
+                66,
                 25
             ],
             [
-                44,
+                63,
                 26
             ],
             [
-                45,
+                64,
                 27
             ],
             [
-                48,
+                67,
                 28
             ],
             [
-                95,
+                123,
                 29
             ],
             [
-                97,
+                125,
                 30
             ],
             [
-                99,
+                127,
                 31
             ],
             [
-                98,
+                126,
                 32
             ],
             [
-                104,
+                132,
                 33
             ],
             [
-                102,
+                130,
                 34
             ],
             [
-                106,
+                134,
                 35
             ],
             [
-                37,
+                56,
                 36
             ],
             [
-                108,
+                136,
                 37
             ],
             [
-                109,
+                137,
                 38
             ],
             [
-                111,
+                139,
                 39
             ],
             [
-                110,
+                138,
                 40
             ],
             [
-                112,
+                140,
                 41
             ],
             [
-                107,
+                135,
                 42
             ],
             [
-                105,
+                133,
                 43
             ],
             [
-                113,
+                141,
                 44
             ],
             [
-                114,
+                142,
                 45
             ],
             [
-                118,
+                146,
                 46
             ],
             [
-                119,
+                147,
                 47
             ],
             [
-                117,
+                145,
                 48
             ],
             [
-                94,
+                122,
                 49
             ],
             [
-                40,
+                59,
                 50
             ],
             [
-                120,
+                148,
                 51
             ],
             [
-                121,
+                149,
                 52
             ],
             [
-                122,
+                150,
                 52
             ],
             [
-                124,
+                152,
                 53
             ],
             [
-                123,
+                151,
                 52
             ],
             [
-                138,
+                166,
                 54
             ],
             [
-                43,
+                62,
                 55
             ],
             [
-                125,
+                153,
                 56
             ],
             [
-                116,
+                144,
                 57
             ],
             [
-                127,
+                155,
                 58
             ],
             [
-                115,
+                143,
                 59
             ],
             [
-                128,
+                156,
                 60
             ],
             [
-                129,
+                157,
                 61
             ],
             [
-                130,
+                158,
                 29
             ],
             [
-                131,
+                159,
                 29
             ],
             [
-                132,
+                160,
                 62
             ],
             [
-                134,
+                162,
                 63
             ],
             [
-                135,
+                163,
                 64
             ],
             [
-                136,
+                164,
                 56
             ],
             [
-                39,
+                58,
                 65
             ],
             [
-                42,
+                61,
                 43
             ],
             [
-                137,
+                165,
                 66
             ],
             [
-                152,
+                180,
                 67
             ],
             [
-                154,
+                182,
                 68
             ],
             [
-                153,
+                181,
                 69
             ],
             [
-                241,
+                269,
                 70
             ],
             [
-                235,
+                263,
                 71
             ],
             [
-                233,
+                261,
                 71
             ],
             [
-                238,
+                266,
                 72
             ],
             [
-                236,
+                264,
                 71
             ],
             [
-                240,
+                268,
                 71
             ],
             [
-                243,
+                271,
                 73
             ],
             [
-                244,
+                272,
                 73
             ],
             [
-                245,
+                273,
                 74
             ],
             [
-                250,
+                278,
                 75
             ],
             [
-                249,
+                277,
                 76
             ],
             [
-                251,
+                279,
                 77
             ],
             [
-                252,
+                280,
                 77
             ],
             [
-                254,
+                282,
                 78
             ],
             [
-                255,
+                283,
                 79
             ],
             [
-                264,
+                292,
                 80
             ],
             [
-                259,
+                287,
                 81
             ],
             [
-                263,
+                291,
                 82
             ],
             [
-                261,
+                289,
                 83
             ],
             [
-                262,
+                290,
                 84
             ],
             [
-                260,
+                288,
                 85
             ],
             [
-                279,
+                307,
                 86
             ],
             [
-                280,
+                308,
                 87
             ],
             [
-                283,
+                311,
                 88
             ],
             [
-                284,
+                312,
                 89
             ],
             [
-                282,
+                310,
                 90
             ],
             [
-                285,
+                313,
                 91
             ],
             [
-                286,
+                314,
                 92
             ],
             [
-                287,
+                315,
                 93
             ],
             [
-                288,
+                316,
                 94
             ],
             [
-                289,
+                317,
                 95
             ],
             [
-                290,
+                318,
                 96
             ],
             [
-                291,
+                319,
                 97
             ],
             [
-                292,
+                320,
                 98
             ],
             [
-                293,
+                321,
                 99
             ],
             [
-                294,
+                322,
                 100
             ],
             [
-                49,
+                68,
                 101
             ],
             [
-                51,
+                69,
+                101
+            ],
+            [
+                71,
                 102
             ],
             [
-                52,
+                72,
                 103
             ],
             [
-                53,
+                73,
                 104
             ],
             [
-                54,
+                74,
                 105
             ],
             [
-                55,
+                75,
                 106
             ],
             [
-                56,
+                76,
                 107
             ],
             [
-                57,
+                77,
                 108
             ],
             [
-                58,
+                78,
                 109
             ],
             [
-                59,
+                79,
                 110
             ],
             [
-                60,
+                80,
                 111
             ],
             [
-                61,
+                81,
+                111
+            ],
+            [
+                82,
                 112
             ],
             [
-                62,
+                83,
                 113
             ],
             [
-                63,
+                84,
                 114
             ],
             [
-                64,
+                85,
                 115
             ],
             [
-                65,
+                86,
                 116
             ],
             [
-                66,
+                87,
                 117
             ],
             [
-                92,
+                88,
                 118
             ],
             [
-                67,
+                89,
                 119
             ],
             [
-                68,
+                120,
                 120
             ],
             [
-                69,
+                90,
                 121
             ],
             [
-                70,
+                91,
                 122
             ],
             [
-                71,
+                92,
                 123
             ],
             [
-                72,
+                93,
                 124
             ],
             [
-                73,
+                94,
                 125
             ],
             [
-                74,
+                95,
                 126
             ],
             [
-                75,
+                96,
                 127
             ],
             [
-                76,
+                97,
                 128
             ],
             [
-                77,
+                98,
                 129
             ],
             [
-                78,
+                99,
                 130
             ],
             [
-                79,
+                100,
                 131
             ],
             [
-                80,
+                101,
                 132
             ],
             [
-                81,
+                103,
                 133
             ],
             [
-                82,
+                102,
                 134
             ],
             [
-                83,
+                104,
                 135
             ],
             [
-                84,
+                105,
                 136
             ],
             [
-                85,
+                107,
                 137
             ],
             [
-                86,
+                108,
                 138
             ],
             [
-                87,
+                109,
                 139
             ],
             [
-                88,
+                110,
                 140
             ],
             [
-                89,
+                111,
                 141
             ],
             [
-                90,
+                112,
                 142
             ],
             [
-                324,
+                113,
                 143
             ],
             [
-                325,
+                114,
                 144
             ],
             [
-                300,
+                115,
                 145
             ],
             [
-                303,
-                145
+                116,
+                146
             ],
             [
-                322,
-                143
+                117,
+                147
             ],
             [
-                323,
-                143
+                118,
+                148
             ],
             [
-                313,
-                143
+                352,
+                149
             ],
             [
-                312,
-                146
+                353,
+                150
             ],
             [
-                310,
-                143
+                328,
+                151
             ],
             [
-                305,
-                143
+                331,
+                151
             ],
             [
-                318,
-                143
+                350,
+                149
             ],
             [
-                316,
-                143
+                351,
+                149
             ],
             [
-                320,
-                143
+                341,
+                149
             ],
             [
-                304,
-                143
+                340,
+                152
             ],
             [
-                317,
-                143
+                338,
+                149
             ],
             [
-                321,
-                143
+                333,
+                149
             ],
             [
-                306,
-                143
+                346,
+                149
             ],
             [
-                307,
-                143
+                344,
+                149
             ],
             [
-                319,
-                143
+                348,
+                149
             ],
             [
-                301,
-                143
+                332,
+                149
             ],
             [
-                308,
-                143
+                345,
+                149
             ],
             [
-                309,
-                143
+                349,
+                149
             ],
             [
-                311,
-                143
+                334,
+                149
             ],
             [
-                315,
-                143
+                335,
+                149
             ],
             [
-                326,
-                147
+                347,
+                149
             ],
             [
-                314,
-                143
+                329,
+                149
             ],
             [
-                302,
-                143
+                336,
+                149
             ],
             [
-                339,
-                148
+                337,
+                149
             ],
             [
-                333,
-                147
+                339,
+                149
             ],
             [
-                335,
+                343,
                 149
             ],
             [
-                334,
-                147
+                354,
+                153
             ],
             [
-                327,
-                147
+                342,
+                149
             ],
             [
-                328,
-                147
+                330,
+                149
             ],
             [
-                330,
-                147
+                367,
+                154
             ],
             [
-                332,
-                147
+                361,
+                153
             ],
             [
-                336,
-                149
+                363,
+                155
             ],
             [
-                337,
-                149
+                362,
+                153
             ],
             [
-                329,
-                149
+                355,
+                153
             ],
             [
-                331,
-                149
+                356,
+                153
             ],
             [
-                342,
-                150
+                358,
+                153
             ],
             [
-                344,
-                151
+                360,
+                153
             ],
             [
-                267,
-                152
+                364,
+                155
             ],
             [
-                276,
-                153
+                365,
+                155
             ],
             [
-                266,
-                154
+                357,
+                155
             ],
             [
-                277,
+                359,
                 155
             ],
             [
-                272,
+                370,
                 156
             ],
             [
-                273,
+                372,
                 157
             ],
             [
-                271,
+                295,
                 158
             ],
             [
-                275,
+                304,
                 159
             ],
             [
-                269,
+                294,
                 160
             ],
             [
-                268,
+                305,
                 161
             ],
             [
-                274,
+                300,
                 162
             ],
             [
-                270,
-                153
-            ],
-            [
-                32,
+                301,
                 163
             ],
             [
-                192,
-                1
+                299,
+                164
             ],
             [
-                221,
+                303,
                 165
             ],
             [
-                220,
-                178
+                297,
+                166
             ],
             [
-                222,
+                296,
                 167
             ],
             [
-                191,
+                302,
+                168
+            ],
+            [
+                298,
+                159
+            ],
+            [
+                51,
                 170
             ],
             [
-                230,
+                220,
+                1
+            ],
+            [
+                249,
                 172
             ],
             [
-                225,
-                1
+                248,
+                185
             ],
             [
-                229,
+                250,
                 174
             ],
             [
-                226,
+                219,
+                177
+            ],
+            [
+                258,
+                179
+            ],
+            [
+                253,
                 1
             ],
             [
-                228,
+                257,
+                181
+            ],
+            [
+                254,
+                1
+            ],
+            [
+                256,
                 1
             ]
         ],
         "fileIdsList": [
             [
-                138
+                166
             ],
             [
-                196,
-                199,
-                206,
-                207,
-                208,
-                209,
-                210
+                224,
+                227,
+                234,
+                235,
+                236,
+                237,
+                238
             ],
             [
-                138,
-                193
+                166,
+                221
             ],
             [
-                193,
-                194,
-                195
+                221,
+                222,
+                223
             ],
             [
-                197,
-                198
+                225,
+                226
             ],
             [
-                138,
-                148
+                166,
+                176
             ],
             [
-                201,
-                202,
-                203
+                229,
+                230,
+                231
             ],
             [
-                200,
-                204,
-                205
+                228,
+                232,
+                233
             ],
             [
-                138,
-                156,
-                157
+                166,
+                184,
+                185
             ],
             [
-                158,
-                159
+                186,
+                187
             ],
             [
-                156,
-                157,
-                160,
-                161,
-                162
+                184,
+                185,
+                188,
+                189,
+                190
             ],
             [
-                138,
-                144
+                166,
+                172
             ],
             [
-                141
+                169
             ],
             [
-                142
+                170
             ],
             [
-                138,
-                139,
-                140
+                166,
+                167,
+                168
             ],
             [
-                139,
-                140,
-                141,
-                143,
-                144,
-                145,
-                146,
-                147
+                167,
+                168,
+                169,
+                171,
+                172,
+                173,
+                174,
+                175
             ],
             [
-                212,
-                213,
-                214,
-                215,
-                216,
-                217,
-                218
+                240,
+                241,
+                242,
+                243,
+                244,
+                245,
+                246
             ],
             [
-                138,
-                154
+                166,
+                182
             ],
             [
-                138,
-                163
+                166,
+                191
             ],
             [
-                150
+                178
             ],
             [
-                138,
-                171,
-                172
+                166,
+                199,
+                200
             ],
             [
-                173
+                201
             ],
             [
-                138,
-                149,
-                150,
-                155,
-                164,
-                165,
                 166,
-                167,
-                168,
-                169,
-                170,
-                174,
-                175,
-                176,
                 177,
                 178,
-                179,
-                180,
-                181,
-                182,
                 183,
-                184,
-                185
+                192,
+                193,
+                194,
+                195,
+                196,
+                197,
+                198,
+                202,
+                203,
+                204,
+                205,
+                206,
+                207,
+                208,
+                209,
+                210,
+                211,
+                212,
+                213
             ],
             [
-                36,
-                43,
-                44,
-                45
+                55,
+                62,
+                63,
+                64
             ],
             [
-                43,
-                46
+                62,
+                65
             ],
             [
-                36,
-                40
+                55,
+                59
             ],
             [
-                36,
-                46
+                55,
+                65
             ],
             [
-                34,
-                35,
-                44,
-                45,
-                46,
-                47
+                53,
+                54,
+                63,
+                64,
+                65,
+                66
             ],
             [
-                78,
-                92,
-                94
+                101,
+                120,
+                122
             ],
             [
-                96
+                124
             ],
             [
-                41,
-                42,
-                43,
-                98
+                60,
+                61,
+                62,
+                126
             ],
             [
-                41,
-                43
+                60,
+                62
             ],
             [
-                100,
-                102,
-                103
+                128,
+                130,
+                131
             ],
             [
-                100,
-                101
+                128,
+                129
             ],
             [
-                105
+                133
             ],
             [
-                34
+                53
             ],
             [
-                37,
-                107
+                56,
+                135
             ],
             [
-                107
+                135
             ],
             [
-                110
+                138
             ],
             [
-                107,
-                108,
-                109
+                135,
+                136,
+                137
             ],
             [
-                107,
-                108,
-                109,
-                110,
-                111
+                135,
+                136,
+                137,
+                138,
+                139
             ],
             [
-                38
+                57
             ],
             [
-                40,
-                41,
-                43
+                59,
+                60,
+                62
             ],
             [
-                96,
-                97
+                124,
+                125
             ],
             [
-                113
+                141
             ],
             [
-                113,
-                117
+                141,
+                145
             ],
             [
-                113,
-                114,
-                117,
-                118
+                141,
+                142,
+                145,
+                146
             ],
             [
-                42,
-                116
+                61,
+                144
             ],
             [
-                93
+                121
             ],
             [
-                33,
-                39
+                52,
+                58
             ],
             [
-                64,
-                66,
-                92
+                87,
+                89,
+                120
             ],
             [
-                36
+                55
             ],
             [
-                36,
-                121,
-                122,
-                123
+                55,
+                149,
+                150,
+                151
             ],
             [
-                33,
-                37,
-                38,
-                39,
-                40,
-                41,
-                42,
-                43,
-                48,
-                95,
-                96,
-                97,
-                98,
-                99,
-                101,
-                104,
-                105,
-                106,
-                112,
-                115,
-                116,
-                119,
-                120,
+                52,
+                56,
+                57,
+                58,
+                59,
+                60,
+                61,
+                62,
+                67,
+                123,
                 124,
                 125,
                 126,
                 127,
-                128,
                 129,
-                130,
-                131,
                 132,
                 133,
-                135,
-                136,
-                137
+                134,
+                140,
+                143,
+                144,
+                147,
+                148,
+                152,
+                153,
+                154,
+                155,
+                156,
+                157,
+                158,
+                159,
+                160,
+                161,
+                163,
+                164,
+                165
             ],
             [
-                34,
-                37,
-                38,
-                42
+                53,
+                56,
+                57,
+                61
             ],
             [
-                99
+                127
             ],
             [
-                115
+                143
             ],
             [
-                40,
-                42,
-                101
+                59,
+                61,
+                129
             ],
             [
-                40,
-                41
+                59,
+                60
             ],
             [
-                40,
-                105
+                59,
+                133
             ],
             [
-                42,
-                96,
-                97
+                61,
+                124,
+                125
             ],
             [
-                64,
-                78,
-                92,
-                94,
-                127
+                87,
+                101,
+                120,
+                122,
+                155
             ],
             [
-                41,
-                98,
-                132,
-                133
+                60,
+                126,
+                160,
+                161
             ],
             [
-                40,
-                64,
-                65,
-                92,
-                99,
+                59,
+                87,
+                88,
+                120,
                 127,
-                131,
-                133,
-                134
+                155,
+                159,
+                161,
+                162
             ],
             [
-                40
+                59
             ],
             [
-                33
+                52
             ],
             [
-                78,
-                92,
-                138
+                101,
+                120,
+                166
             ],
             [
-                151,
-                152,
-                153
+                179,
+                180,
+                181
             ],
             [
-                78,
-                138
+                101,
+                166
             ],
             [
-                232,
-                233,
-                235,
-                238,
-                240
+                260,
+                261,
+                263,
+                266,
+                268
             ],
             [
-                232
+                260
             ],
             [
-                232,
-                235
+                260,
+                263
             ],
             [
-                242
+                270
             ],
             [
-                64,
-                92
+                87,
+                120
             ],
             [
-                247,
-                249
+                275,
+                277
             ],
             [
-                246,
-                247,
-                248
+                274,
+                275,
+                276
             ],
             [
-                62,
-                92
+                85,
+                120
             ],
             [
-                253
+                281
             ],
             [
-                254
+                282
             ],
             [
-                260,
-                263
+                288,
+                291
             ],
             [
-                258
+                286
             ],
             [
-                51,
-                92,
-                256,
-                262
+                71,
+                120,
+                284,
+                290
             ],
             [
-                260
+                288
             ],
             [
-                257,
-                261
+                285,
+                289
             ],
             [
-                259
+                287
             ],
             [
-                61,
-                87,
-                92,
-                277,
-                278,
-                280
+                84,
+                115,
+                120,
+                305,
+                306,
+                308
             ],
             [
-                279
+                307
             ],
             [
-                282,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294
+                310,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                282,
-                283,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294
+                310,
+                311,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                282,
-                283,
-                284,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294
+                310,
+                311,
+                312,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                282,
-                283,
-                284,
-                285,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294
+                310,
+                311,
+                312,
+                313,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                282,
-                283,
-                284,
-                285,
-                286,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294
+                310,
+                311,
+                312,
+                313,
+                314,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                282,
-                283,
-                284,
-                285,
-                286,
-                287,
-                289,
-                290,
-                291,
-                292,
-                293,
-                294
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                317,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                282,
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                290,
-                291,
-                292,
-                293,
-                294
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                318,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                282,
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                291,
-                292,
-                293,
-                294
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                319,
+                320,
+                321,
+                322
             ],
             [
-                282,
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                292,
-                293,
-                294
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                320,
+                321,
+                322
             ],
             [
-                282,
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                293,
-                294
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                321,
+                322
             ],
             [
-                282,
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                294
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                322
             ],
             [
-                282,
-                283,
-                284,
-                285,
-                286,
-                287,
-                288,
-                289,
-                290,
-                291,
-                292,
-                293
+                310,
+                311,
+                312,
+                313,
+                314,
+                315,
+                316,
+                317,
+                318,
+                319,
+                320,
+                321
             ],
             [
-                49
+                68
             ],
             [
-                51
+                71
             ],
             [
-                52,
-                57
+                72,
+                77,
+                104
             ],
             [
-                53,
-                61,
-                62,
-                69,
-                78
+                73,
+                84,
+                85,
+                92,
+                101,
+                112
             ],
             [
-                53,
-                54,
-                61,
-                69
+                73,
+                74,
+                84,
+                92
             ],
             [
-                55,
-                85
+                75,
+                113
             ],
             [
-                56,
-                57,
-                62,
-                70
+                76,
+                77,
+                85,
+                93
             ],
             [
-                57,
-                78
+                77,
+                101,
+                109
             ],
             [
-                58,
-                59,
-                61,
-                69
+                78,
+                80,
+                84,
+                92
             ],
             [
-                59
+                79
             ],
             [
-                60,
-                61
+                80,
+                81
             ],
             [
-                61
+                84
             ],
             [
-                61,
-                62,
-                63,
-                78,
+                83,
                 84
             ],
             [
-                62,
-                63
+                71,
+                84
             ],
             [
-                61,
-                64,
-                69,
-                78,
-                84
+                84,
+                85,
+                86,
+                101,
+                112
             ],
             [
-                61,
-                62,
-                64,
-                65,
-                69,
-                78,
-                81,
-                84
+                84,
+                85,
+                86,
+                101
             ],
             [
-                64,
-                66,
-                78,
-                81,
-                84
+                84,
+                87,
+                92,
+                101,
+                112
+            ],
+            [
+                84,
+                85,
+                87,
+                88,
+                92,
+                101,
+                109,
+                112
+            ],
+            [
+                87,
+                89,
+                101,
+                109,
+                112
             ],
             [
-                49,
-                50,
-                51,
-                52,
-                53,
-                54,
-                55,
-                56,
-                57,
-                58,
-                59,
-                60,
-                61,
-                62,
-                63,
-                64,
-                65,
-                66,
-                67,
                 68,
                 69,
                 70,
                 71,
                 72,
                 73,
                 74,
@@ -1754,323 +1780,401 @@
                 84,
                 85,
                 86,
                 87,
                 88,
                 89,
                 90,
-                91
+                91,
+                92,
+                93,
+                94,
+                95,
+                96,
+                97,
+                98,
+                99,
+                100,
+                101,
+                102,
+                103,
+                104,
+                105,
+                106,
+                107,
+                108,
+                109,
+                110,
+                111,
+                112,
+                113,
+                114,
+                115,
+                116,
+                117,
+                118,
+                119
             ],
             [
-                61,
-                67
+                84,
+                90
             ],
             [
-                68,
-                84
+                91,
+                112,
+                117
             ],
             [
-                59,
-                61,
-                69,
-                78
+                80,
+                84,
+                92,
+                101
             ],
             [
-                70
+                93
             ],
             [
-                71
+                94
             ],
             [
-                51,
-                72
+                71,
+                95
             ],
             [
-                73,
-                83
+                96,
+                111,
+                117
             ],
             [
-                74
+                97
             ],
             [
-                75
+                98
             ],
             [
-                61,
-                76
+                84,
+                99
             ],
             [
-                76,
-                77,
-                85,
-                87
+                99,
+                100,
+                113,
+                115
             ],
             [
-                61,
-                78
+                72,
+                84,
+                101,
+                102,
+                103
             ],
             [
-                79
+                72,
+                101,
+                103
             ],
             [
-                80
+                101,
+                102
             ],
             [
-                69,
-                78,
-                81
+                104
             ],
             [
-                82
+                105
             ],
             [
-                69,
-                83
+                84,
+                107,
+                108
             ],
             [
-                64,
-                75,
-                84
+                107,
+                108
             ],
             [
-                85
+                77,
+                92,
+                101,
+                109
             ],
             [
-                78,
-                86
+                110
             ],
             [
-                87
+                92,
+                111
             ],
             [
-                88
+                72,
+                87,
+                98,
+                112
             ],
             [
-                61,
-                63,
-                78,
+                77,
+                113
+            ],
+            [
+                101,
+                114
+            ],
+            [
+                115
+            ],
+            [
+                116
+            ],
+            [
+                72,
+                77,
                 84,
-                87,
-                89
+                86,
+                95,
+                101,
+                112,
+                115,
+                117
             ],
             [
-                78,
-                90
+                101,
+                118
             ],
             [
-                300,
-                339
+                328,
+                367
             ],
             [
-                300,
-                324,
-                339
+                328,
+                352,
+                367
             ],
             [
-                339
+                367
             ],
             [
-                300
+                328
             ],
             [
-                300,
-                325,
-                339
+                328,
+                353,
+                367
             ],
             [
-                300,
-                301,
-                302,
-                303,
-                304,
-                305,
-                306,
-                307,
-                308,
-                309,
-                310,
-                311,
-                312,
-                313,
-                314,
-                315,
-                316,
-                317,
-                318,
-                319,
-                320,
-                321,
-                322,
-                323,
-                324,
-                325,
-                326,
-                327,
                 328,
                 329,
                 330,
                 331,
                 332,
                 333,
                 334,
                 335,
                 336,
                 337,
-                338
+                338,
+                339,
+                340,
+                341,
+                342,
+                343,
+                344,
+                345,
+                346,
+                347,
+                348,
+                349,
+                350,
+                351,
+                352,
+                353,
+                354,
+                355,
+                356,
+                357,
+                358,
+                359,
+                360,
+                361,
+                362,
+                363,
+                364,
+                365,
+                366
             ],
             [
-                325,
-                339
+                353,
+                367
             ],
             [
-                61,
-                64,
-                66,
-                69,
-                78,
-                81,
                 84,
-                90,
-                92
+                87,
+                89,
+                92,
+                101,
+                109,
+                112,
+                118,
+                120
             ],
             [
-                343
+                371
             ],
             [
-                266
+                294
             ],
             [
-                265,
-                266
+                293,
+                294
             ],
             [
-                265
+                293
             ],
             [
-                265,
-                266,
-                267,
-                269,
-                270,
-                273,
-                274,
-                275,
-                276
+                293,
+                294,
+                295,
+                297,
+                298,
+                301,
+                302,
+                303,
+                304
             ],
             [
-                266,
-                270
+                294,
+                298
             ],
             [
-                265,
-                266,
-                267,
-                269,
-                270,
-                271,
-                272
+                293,
+                294,
+                295,
+                297,
+                298,
+                299,
+                300
             ],
             [
-                265,
-                270
+                293,
+                298
             ],
             [
-                270,
-                274
+                298,
+                302
             ],
             [
-                266,
-                267,
-                268
+                294,
+                295,
+                296
             ],
             [
-                267
+                295
             ],
             [
-                265,
-                266,
-                270
+                293,
+                294,
+                298
             ],
             [
-                31
+                49
             ],
             [
-                138,
-                148,
-                186,
-                191
+                49,
+                50
             ],
             [
-                192,
-                220
+                49,
+                166,
+                176,
+                214,
+                219
             ],
             [
-                138,
-                211,
-                219
+                49,
+                220,
+                248
             ],
             [
-                221
+                49,
+                166,
+                239,
+                247
             ],
             [
-                148
+                49,
+                249
             ],
             [
-                189
+                49,
+                176
             ],
             [
-                187,
-                188,
-                190
+                49,
+                217
             ],
             [
-                188
+                49,
+                215,
+                216,
+                218
             ],
             [
-                32,
-                222,
-                229
+                49,
+                216
             ],
             [
-                138,
-                186
+                49,
+                51,
+                250,
+                257
             ],
             [
-                223,
-                224,
-                226,
-                228
+                49,
+                166,
+                214
             ],
             [
-                186
+                49,
+                251,
+                252,
+                254,
+                256
             ],
             [
-                138,
-                225
+                49,
+                214
             ],
             [
-                138,
-                186,
-                225,
-                227
+                49,
+                166,
+                253
             ],
             [
-                138,
-                219
+                49,
+                166,
+                214,
+                253,
+                255
+            ],
+            [
+                166,
+                247
             ]
         ],
         "fileInfos": [
             {
                 "affectsGlobalScope": true,
                 "version": "8730f4bf322026ff5229336391a18bcaa1f94d4f82416c8b2f3954e2ccaae2ba"
             },
             "dc47c4fa66b9b9890cf076304de2a9c5201e94b740cffdf09f87296d877d71f6",
             "7a387c58583dfca701b6c85e0adaf43fb17d590fb16d5b2dc0a2fbd89f35c467",
             "8a12173c586e95f4433e0c6dc446bc88346be73ffe9ca6eec7aa63c8f3dca7f9",
             "5f4e733ced4e129482ae2186aae29fde948ab7182844c3a5a51dd346182c7b06",
+            "4b421cbfb3a38a27c279dec1e9112c3d1da296f77a1a85ddadf7e7a425d45d18",
+            "1fc5ab7a764205c68fa10d381b08417795fc73111d6dd16b5b1ed36badb743d9",
+            "746d62152361558ea6d6115cf0da4dd10ede041d14882ede3568bce5dc4b4f1f",
             {
                 "affectsGlobalScope": true,
                 "version": "3aafcb693fe5b5c3bd277bd4c3a617b53db474fe498fc5df067c5603b1eebde7"
             },
             {
                 "affectsGlobalScope": true,
                 "version": "f3d4da15233e593eacb3965cde7960f3fddf5878528d882bcedd5cbaba0193c7"
@@ -2153,24 +2257,85 @@
             },
             {
                 "affectsGlobalScope": true,
                 "version": "c80df75850fea5caa2afe43b9949338ce4e2de086f91713e9af1a06f973872b8"
             },
             {
                 "affectsGlobalScope": true,
+                "version": "9d57b2b5d15838ed094aa9ff1299eecef40b190722eb619bac4616657a05f951"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "6c51b5dd26a2c31dbf37f00cfc32b2aa6a92e19c995aefb5b97a3a64f1ac99de"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "6e7997ef61de3132e4d4b2250e75343f487903ddf5370e7ce33cf1b9db9a63ed"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "2ad234885a4240522efccd77de6c7d99eecf9b4de0914adb9a35c0c22433f993"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "5e5e095c4470c8bab227dbbc61374878ecead104c74ab9960d3adcccfee23205"
+            },
+            {
+                "affectsGlobalScope": true,
                 "version": "09aa50414b80c023553090e2f53827f007a301bc34b0495bfb2c3c08ab9ad1eb"
             },
             {
                 "affectsGlobalScope": true,
+                "version": "d7f680a43f8cd12a6b6122c07c54ba40952b0c8aa140dcfcf32eb9e6cb028596"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "3787b83e297de7c315d55d4a7c546ae28e5f6c0a361b7a1dcec1f1f50a54ef11"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "e7e8e1d368290e9295ef18ca23f405cf40d5456fa9f20db6373a61ca45f75f40"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "faf0221ae0465363c842ce6aa8a0cbda5d9296940a8e26c86e04cc4081eea21e"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "06393d13ea207a1bfe08ec8d7be562549c5e2da8983f2ee074e00002629d1871"
+            },
+            {
+                "affectsGlobalScope": true,
                 "version": "2768ef564cfc0689a1b76106c421a2909bdff0acbe87da010785adab80efdd5c"
             },
             {
                 "affectsGlobalScope": true,
+                "version": "b248e32ca52e8f5571390a4142558ae4f203ae2f94d5bac38a3084d529ef4e58"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "6c55633c733c8378db65ac3da7a767c3cf2cf3057f0565a9124a16a3a2019e87"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "fb4416144c1bf0323ccbc9afb0ab289c07312214e8820ad17d709498c865a3fe"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "5b0ca94ec819d68d33da516306c15297acec88efeb0ae9e2b39f71dbd9685ef7"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "34c839eaaa6d78c8674ae2c37af2236dee6831b13db7b4ef4df3ec889a04d4f2"
+            },
+            {
+                "affectsGlobalScope": true,
                 "version": "52d1bb7ab7a3306fd0375c8bff560feed26ed676a5b0457fa8027b563aecb9a4"
             },
+            "7a1971efcba559ea9002ada4c4e3c925004fb67a755300d53b5edf9399354900",
             {
                 "signature": "02ec1ffcc0823cb9c9ba420c619d3af2c726e3a674b66a91941c07a3e7f65dba",
                 "version": "6d93b19d11edb10bce1aa933bae0fdf55c57785d376c4617e32506783791cd03"
             },
             "38f6da5b6f318c33e18dd7c983cab3fe52f510c9a2573948fb13f012e01b1ba6",
             "c55ae709f94155174ff63647edd2a7e3acbd02a2909aa2541569e8b8bac9fc40",
             "530e5c7e4f74267b7800f1702cf0c576282296a960acbdb2960389b2b1d0875b",
@@ -2184,79 +2349,103 @@
             "b7b881ced4ed4dee13d6e0ccdb2296f66663ba6b1419767271090b3ff3478bb9",
             "06289b9873760aac77aed4035ea6c60b1e0879b8afe47a4530bc8522b9b804b1",
             "63c36aa73242aa745fae813c40585111ead225394b0a0ba985c2683baa6b0ef9",
             "3e7ffc7dd797e5d44d387d0892bc288480493e73dcab9832812907d1389e4a98",
             "db011ec9589fd51995cbd0765673838e38e6485a6559163cc53dcf508b480909",
             "e1a4253f0cca15c14516f52a2ad36c3520b140b5dfb3b3880a368cd75d45d6d9",
             "159af954f2633a12fdee68605009e7e5b150dbeb6d70c46672fd41059c154d53",
-            "4c2c4f53e8eedd970f8afa369d7371544fb6231bf95e659f8602e09abe74d5a5",
+            "5b3cd03ae354ea96eff1f74d7c410fe4852e6382227e8b0ecf87ab5e3a5bbcd4",
+            "7394959e5a741b185456e1ef5d64599c36c60a323207450991e7a42e08911419",
             {
                 "affectsGlobalScope": true,
-                "version": "cb5a780979155e80a2184eb987cc411a95c9a1686019ade06918c312a0b7c9b2"
+                "version": "056097110efd16869ec118cedb44ecbac9a019576eee808d61304ca6d5cb2cbe"
             },
-            "c2b5085f47e41d6940bbc5b0d3bd7cc0037c752efb18aecd243c9cf83ad0c0b7",
-            "3143a5add0467b83150961ecd33773b561a1207aec727002aa1d70333068eb1b",
-            "f87191b7fafe7a0edad375710d99f900e49cef560b66bf309cf3f8e1b7177126",
-            "586af7d2abe2f9d59c5e757c370087d6c6baea81b033250f43b8df808d6dfb33",
+            "f51b4042a3ac86f1f707500a9768f88d0b0c1fc3f3e45a73333283dea720cdc6",
             {
                 "affectsGlobalScope": true,
-                "version": "1a048ff164b8d9609f5de3139d4e37f6e8a82af82087ac414b9208f52ef8aac7"
+                "version": "6fb8358e10ed92a7f515b7d79da3904c955a3ffd4e14aa9df6f0ea113041f1cf"
             },
-            "3111079f3cb5f2b9c812ca3f46161562bce5bfb355e915f46ed46c41714dc1c3",
-            "e7bee4a6d9bb78afa390b25e0ce97a2f94787a1eb17f0a16e732dcbebba3f3ee",
-            "b32b6b16cb0bda68199582ad6f22242d07ee75fac9b1f28a98cd838afc5eea45",
-            "4441ee4119824bfaebc49308559edd7545978f9cb41a40f115074e1031dde75f",
+            "45c831238c6dac21c72da5f335747736a56a3847192bf03c84b958a7e9ec93e2",
+            "661a11d16ad2e3543a77c53bcd4017ee9a450f47ab7def3ab493a86eae4d550c",
             {
                 "affectsGlobalScope": true,
-                "version": "60693a88462d0e97900123b5bf7c73e146ce0cc94da46a61fe6775b430d2ff05"
+                "version": "8cdc646cec7819581ef343b83855b1bfe4fe674f2c84f4fb8dc90d82fb56bd3a"
             },
+            "a40826e8476694e90da94aa008283a7de50d1dafd37beada623863f1901cb7fb",
+            "9dd56225cc2d8cb8fe5ceb0043ff386987637e12fecc6078896058a99deae284",
+            "2375ed4b439215aa3b6d0c6fd175c78a4384b30cb43cbadaecbf0a18954c98cb",
+            "7693b90b3075deaccafd5efb467bf9f2b747a3075be888652ef73e64396d8628",
+            "41231da15bb5e3e806a8395bd15c7befd2ec90f9f4e3c9d0ae1356bccb76dbb0",
+            "fccfef201d057cb407fa515311bd608549bab6c7b8adcf8f2df31f5d3b796478",
             {
                 "affectsGlobalScope": true,
-                "version": "588c69eda58b9202676ec7ca11a72c3762819b46a0ed72462c769846153c447c"
+                "version": "ee1ee365d88c4c6c0c0a5a5701d66ebc27ccd0bcfcfaa482c6e2e7fe7b98edf7"
             },
-            "ae064ed4f855716b7ff348639ddcd6a6d354a72fae82f506608a7dc9266aa24c",
-            "92f019c55b21c939616f6a48f678e714ac7b109444cbbf23ad69310ce66ecbdc",
-            "bba259efdf9ab95e0c7d3cc8e99250f56bb6b31d6129efdf733ca4eb1d01feea",
-            "499b7544062cf44fab253daeaea8ba28877d9e7ff4149246b1f0154d1c9ed535",
-            "139fd681eff7771a38d0c025d13c7a11c5474f6aab61e01c41511d71496df173",
-            "f614c3f61e46ccc2cb58702d5a158338ea57ee09099fde5db4cfc63ed0ce4d74",
-            "44e42ed6ec9c4451ebe89524e80ac8564e9dd0988c56e6c58f393c810730595d",
-            "a504c109b872b0e653549bd258eb06584c148c98d79406c7516995865a6d5089",
-            "155865f5f76db0996cd5e20cc5760613ea170ee5ad594c1f3d76fcaa05382161",
-            "e92852d673c836fc64e10c38640abcd67c463456e5df55723ac699b8e6ab3a8a",
-            "4455c78d226d061b1203c7614c6c6eb5f4f9db5f00d44ff47d0112de8766fbc4",
+            "5f20d20b7607174caf1a6da9141aeb9f2142159ae2410ca30c7a0fccd1d19c99",
             {
                 "affectsGlobalScope": true,
-                "version": "ec369bb9d97c4dc09dd2a4093b7ca3ba69ad284831fccac8a1977785e9e38ce5"
+                "version": "464762c6213566d072f1ced5e8e9a954785ec5e53883b7397198abb5ef5b8f71"
             },
-            "4465a636f5f6e9665a90e30691862c9e0a3ac2edc0e66296704f10865e924f2a",
-            "9af781f03d44f5635ed7844be0ce370d9d595d4b4ec67cad88f0fac03255257e",
-            "f9fd4c3ef6de27fa0e256f4e75b61711c4be05a3399f7714621d3edc832e36b0",
-            "e49290b7a927995c0d7e6b2b9c8296284b68a9036d9966531de65185269258d7",
-            "aa95cc73ea5315e4f6fc8c6db43d49e3b7de3780cae20a4f1319032809013038",
-            "874ca809b79276460011480a2829f4c8d4db29416dd411f71efbf8f497f0ac09",
-            "6c903bceaf3f3bc04f2d4c7dcd89ce9fb148b3ba0a5f5408d8f6de2b7eecc7ea",
-            "504d049d9e550a65466b73ca39da6469ab41786074ea1d16d37c8853f9f6ab2e",
-            "23a28f834a078986bbf58f4e3705956983ff81c3c2493f3db3e5f0e8a9507779",
-            "4febdf7f3ec92706c58e0b4e8159cd6de718284ef384260b07c9641c13fc70ce",
+            "6387920dc3e18927335b086deec75bf8e50f879a5e273d32ee7bb7a55ba50572",
+            "9bba37424094688c4663c177a1379b229f919b8912889a472f32fdc5f08ddb4d",
+            "29a4be13b3a30d3e66667b75c58ec61fb2df8fa0422534fdee3cfb30c5dbf450",
+            "83366d901beda79d6eb37aaaf6ca248dcd88946302b2a7d975590783be51e88e",
+            "bf268a0aea37ad4ae3b7a9b58559190b6fc01ea16a31e35cd05817a0a60f895a",
+            "43ec77c369473e92e2ecebf0554a0fdaa9c256644a6070f28228dfcceec77351",
             {
                 "affectsGlobalScope": true,
-                "version": "bf241ed073916ec9e21a3c138936edd444b6787d874844c0d05fc00a8f109d19"
+                "version": "d7dad6db394a3d9f7b49755e4b610fbf8ed6eb0c9810ae5f1a119f6b5d76de45"
             },
-            "7335933d9f30dcfd2c4b6080a8b78e81912a7fcefb1dafccb67ca4cb4b3ac23d",
-            "a6bfe9de9adef749010c118104b071d14943802ff0614732b47ce4f1c3e383cd",
-            "4c3d0e10396646db4a1e917fb852077ee77ae62e512913bef9cccc2bb0f8bd0e",
-            "3b220849d58140dcc6718f5b52dcd29fdb79c45bc28f561cbd29eb1cac6cce13",
-            "0ee22fce41f7417a24c808d266e91b850629113c104713a35854393d55994beb",
-            "22d1b1d965baba05766613e2e6c753bb005d4386c448cafd72c309ba689e8c24",
+            "95ed02bacb4502c985b69742ec82a4576d4ff4a6620ecc91593f611d502ae546",
+            "bf755525c4e6f85a970b98c4755d98e8aa1b6dbd83a5d8fcc57d3d497351b936",
+            "dd67d2b5e4e8a182a38de8e69fb736945eaa4588e0909c14e01a14bd3cc1fd1e",
             {
                 "affectsGlobalScope": true,
-                "version": "2708349d5a11a5c2e5f3a0765259ebe7ee00cdcc8161cb9990cb4910328442a1"
+                "version": "28084e15b63e6211769db2fe646d8bc5c4c6776321e0deffe2d12eefd52cb6b9"
             },
-            "c6c0bd221bb1e94768e94218f8298e47633495529d60cae7d8da9374247a1cf5",
+            {
+                "affectsGlobalScope": true,
+                "version": "aed37dabf86c99d6c8508700576ecede86688397bc12523541858705a0c737c2"
+            },
+            "cc6ef5733d4ea6d2e06310a32dffd2c16418b467c5033d49cecc4f3a25de7497",
+            "94768454c3348b6ebe48e45fbad8c92e2bb7af4a35243edbe2b90823d0bd7f9a",
+            "0be79b3ff0f16b6c2f9bc8c4cc7097ea417d8d67f8267f7e1eec8e32b548c2ff",
+            "1c61ffa3a71b77363b30d19832c269ef62fba787f5610cac7254728d3b69ab2e",
+            "84da3c28344e621fd1d591f2c09e9595292d2b70018da28a553268ac122597d4",
+            "269929a24b2816343a178008ac9ae9248304d92a8ba8e233055e0ed6dbe6ef71",
+            "6e191fea1db6e9e4fa828259cf489e820ec9170effff57fb081a2f3295db4722",
+            "aed943465fbce1efe49ee16b5ea409050f15cd8eaf116f6fadb64ef0772e7d95",
+            "70d08483a67bf7050dbedace398ef3fee9f436fcd60517c97c4c1e22e3c6f3e8",
+            "c40fdf7b2e18df49ce0568e37f0292c12807a0748be79e272745e7216bed2606",
+            {
+                "affectsGlobalScope": true,
+                "version": "e933de8143e1d12dd51d89b398760fd5a9081896be366dad88a922d0b29f3c69"
+            },
+            "4e228e78c1e9b0a75c70588d59288f63a6258e8b1fe4a67b0c53fe03461421d9",
+            "b38d55d08708c2410a3039687db70b4a5bfa69fc4845617c313b5a10d9c5c637",
+            "205d50c24359ead003dc537b9b65d2a64208dfdffe368f403cf9e0357831db9e",
+            "1265fddcd0c68be9d2a3b29805d0280484c961264dd95e0b675f7bd91f777e78",
+            {
+                "affectsGlobalScope": true,
+                "version": "a05e2d784c9be7051c4ac87a407c66d2106e23490c18c038bbd0712bde7602fd"
+            },
+            {
+                "affectsGlobalScope": true,
+                "version": "df90b9d0e9980762da8daf8adf6ffa0c853e76bfd269c377be0d07a9ad87acd2"
+            },
+            "cf434b5c04792f62d6f4bdd5e2c8673f36e638e910333c172614d5def9b17f98",
+            "1d65d4798df9c2df008884035c41d3e67731f29db5ecb64cd7378797c7c53a2f",
+            "0faee6b555890a1cb106e2adc5d3ffd89545b1da894d474e9d436596d654998f",
+            "c6c01ea1c42508edf11a36d13b70f6e35774f74355ba5d358354d4a77cc67ea1",
+            "867f95abf1df444aab146b19847391fc2f922a55f6a970a27ed8226766cee29f",
+            {
+                "affectsGlobalScope": true,
+                "version": "ab9b9a36e5284fd8d3bf2f7d5fcbc60052f25f27e4d20954782099282c60d23e"
+            },
+            "b0297b09e607bec9698cac7cf55463d6731406efb1161ee4d448293b47397c84",
             "a1b36a1f91a54daf2e89e12b834fa41fb7338bc044d1f08a80817efc93c99ee5",
             "8bb4a5b632dd5a868f3271750895cb61b0e20cff82032d87e89288faee8dd6e2",
             "0c1aabfd9fb1818afb2e798f91f669edafce59cd7e3423d25b1cfccfaaf2c403",
             "017de6fdabea79015d493bf71e56cbbff092525253c1d76003b3d58280cd82a0",
             "ab9ea2596cb7800bd79d1526930c785606ec4f439c275adbca5adc1ddf87747d",
             "aee8faa433dde04beedb779b3329456a286a966462d666c138c19113ce78c79e",
             "d620ec36bfc6f8ed6fdecbe036d55cec81637f32fd34dc7bb7e60eba1764e910",
@@ -2559,14 +2748,17 @@
         ],
         "fileNames": [
             "../../node_modules/typescript/lib/lib.es5.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.d.ts",
             "../../node_modules/typescript/lib/lib.es2016.d.ts",
             "../../node_modules/typescript/lib/lib.es2017.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.d.ts",
+            "../../node_modules/typescript/lib/lib.es2021.d.ts",
             "../../node_modules/typescript/lib/lib.dom.d.ts",
             "../../node_modules/typescript/lib/lib.dom.iterable.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.core.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.collection.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.generator.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.iterable.d.ts",
             "../../node_modules/typescript/lib/lib.es2015.promise.d.ts",
@@ -2581,17 +2773,33 @@
             "../../node_modules/typescript/lib/lib.es2017.intl.d.ts",
             "../../node_modules/typescript/lib/lib.es2017.typedarrays.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.asyncgenerator.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.asynciterable.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.intl.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.promise.d.ts",
             "../../node_modules/typescript/lib/lib.es2018.regexp.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.array.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.object.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.string.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.symbol.d.ts",
+            "../../node_modules/typescript/lib/lib.es2019.intl.d.ts",
             "../../node_modules/typescript/lib/lib.es2020.bigint.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.date.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.promise.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.sharedmemory.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.string.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.symbol.wellknown.d.ts",
             "../../node_modules/typescript/lib/lib.es2020.intl.d.ts",
+            "../../node_modules/typescript/lib/lib.es2020.number.d.ts",
+            "../../node_modules/typescript/lib/lib.es2021.promise.d.ts",
+            "../../node_modules/typescript/lib/lib.es2021.string.d.ts",
+            "../../node_modules/typescript/lib/lib.es2021.weakref.d.ts",
+            "../../node_modules/typescript/lib/lib.es2021.intl.d.ts",
             "../../node_modules/typescript/lib/lib.esnext.intl.d.ts",
+            "../../node_modules/tslib/tslib.d.ts",
             "./src/client/emitWarningIfUnsupportedVersion.ts",
             "./src/client/index.ts",
             "../../node_modules/@smithy/types/dist-types/abort.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/auth.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/HttpApiKeyAuth.d.ts",
             "../../node_modules/@smithy/types/dist-types/identity/identity.d.ts",
             "../../node_modules/@smithy/types/dist-types/endpoint.d.ts",
@@ -2603,24 +2811,28 @@
             "../../node_modules/@smithy/types/dist-types/middleware.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/HttpSigner.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/IdentityProviderConfig.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/HttpAuthScheme.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/HttpAuthSchemeProvider.d.ts",
             "../../node_modules/@smithy/types/dist-types/auth/index.d.ts",
             "../../node_modules/@types/node/assert.d.ts",
+            "../../node_modules/@types/node/assert/strict.d.ts",
             "../../node_modules/@types/node/globals.d.ts",
             "../../node_modules/@types/node/async_hooks.d.ts",
             "../../node_modules/@types/node/buffer.d.ts",
             "../../node_modules/@types/node/child_process.d.ts",
             "../../node_modules/@types/node/cluster.d.ts",
             "../../node_modules/@types/node/console.d.ts",
             "../../node_modules/@types/node/constants.d.ts",
             "../../node_modules/@types/node/crypto.d.ts",
             "../../node_modules/@types/node/dgram.d.ts",
+            "../../node_modules/@types/node/diagnostics_channel.d.ts",
             "../../node_modules/@types/node/dns.d.ts",
+            "../../node_modules/@types/node/dns/promises.d.ts",
+            "../../node_modules/@types/node/dom-events.d.ts",
             "../../node_modules/@types/node/domain.d.ts",
             "../../node_modules/@types/node/events.d.ts",
             "../../node_modules/@types/node/fs.d.ts",
             "../../node_modules/@types/node/fs/promises.d.ts",
             "../../node_modules/@types/node/http.d.ts",
             "../../node_modules/@types/node/http2.d.ts",
             "../../node_modules/@types/node/https.d.ts",
@@ -2632,16 +2844,21 @@
             "../../node_modules/@types/node/perf_hooks.d.ts",
             "../../node_modules/@types/node/process.d.ts",
             "../../node_modules/@types/node/punycode.d.ts",
             "../../node_modules/@types/node/querystring.d.ts",
             "../../node_modules/@types/node/readline.d.ts",
             "../../node_modules/@types/node/repl.d.ts",
             "../../node_modules/@types/node/stream.d.ts",
+            "../../node_modules/@types/node/stream/promises.d.ts",
+            "../../node_modules/@types/node/stream/consumers.d.ts",
+            "../../node_modules/@types/node/stream/web.d.ts",
             "../../node_modules/@types/node/string_decoder.d.ts",
+            "../../node_modules/@types/node/test.d.ts",
             "../../node_modules/@types/node/timers.d.ts",
+            "../../node_modules/@types/node/timers/promises.d.ts",
             "../../node_modules/@types/node/tls.d.ts",
             "../../node_modules/@types/node/trace_events.d.ts",
             "../../node_modules/@types/node/tty.d.ts",
             "../../node_modules/@types/node/url.d.ts",
             "../../node_modules/@types/node/util.d.ts",
             "../../node_modules/@types/node/v8.d.ts",
             "../../node_modules/@types/node/vm.d.ts",
@@ -2906,1247 +3123,1272 @@
         "options": {
             "declaration": true,
             "declarationDir": "./dist-types",
             "downlevelIteration": true,
             "emitDeclarationOnly": true,
             "esModuleInterop": true,
             "experimentalDecorators": true,
+            "importHelpers": true,
             "jsx": 2,
             "module": 1,
+            "noEmitHelpers": false,
             "noFallthroughCasesInSwitch": true,
             "preserveConstEnums": true,
             "removeComments": false,
             "rootDir": "./src",
+            "skipLibCheck": true,
             "strict": true,
-            "target": 1,
+            "target": 8,
             "useUnknownInCatchVariables": false
         },
         "referencedMap": [
             [
-                207,
+                235,
                 1
             ],
             [
-                211,
+                239,
                 2
             ],
             [
-                194,
+                222,
                 3
             ],
             [
-                195,
+                223,
                 3
             ],
             [
-                193,
+                221,
                 1
             ],
             [
-                196,
+                224,
                 4
             ],
             [
-                198,
+                226,
                 1
             ],
             [
-                197,
+                225,
                 1
             ],
             [
-                199,
+                227,
                 5
             ],
             [
-                208,
+                236,
                 1
             ],
             [
-                210,
+                238,
                 1
             ],
             [
-                209,
+                237,
                 6
             ],
             [
-                200,
+                228,
                 1
             ],
             [
-                201,
+                229,
                 6
             ],
             [
-                202,
+                230,
                 6
             ],
             [
-                204,
+                232,
                 7
             ],
             [
-                203,
+                231,
                 1
             ],
             [
-                206,
+                234,
                 8
             ],
             [
-                205,
+                233,
                 1
             ],
             [
-                158,
+                186,
                 9
             ],
             [
-                160,
+                188,
                 10
             ],
             [
-                159,
+                187,
                 1
             ],
             [
-                161,
+                189,
                 9
             ],
             [
-                162,
+                190,
                 9
             ],
             [
-                163,
+                191,
                 11
             ],
             [
-                156,
+                184,
                 1
             ],
             [
-                144,
+                172,
                 1
             ],
             [
-                145,
+                173,
                 12
             ],
             [
-                142,
+                170,
                 13
             ],
             [
-                143,
+                171,
                 14
             ],
             [
-                141,
+                169,
                 15
             ],
             [
-                139,
+                167,
                 1
             ],
             [
-                140,
+                168,
                 1
             ],
             [
-                148,
+                176,
                 16
             ],
             [
-                147,
+                175,
                 1
             ],
             [
-                212,
+                240,
                 1
             ],
             [
-                218,
+                246,
                 1
             ],
             [
-                213,
+                241,
                 1
             ],
             [
-                214,
+                242,
                 1
             ],
             [
-                215,
+                243,
                 1
             ],
             [
-                219,
+                247,
                 17
             ],
             [
-                216,
+                244,
                 1
             ],
             [
-                217,
+                245,
                 1
             ],
             [
-                149,
+                177,
                 1
             ],
             [
-                150,
+                178,
                 1
             ],
             [
-                155,
+                183,
                 18
             ],
             [
-                164,
+                192,
                 19
             ],
             [
-                166,
+                194,
                 20
             ],
             [
-                175,
+                203,
                 1
             ],
             [
-                171,
+                199,
                 1
             ],
             [
-                173,
+                201,
                 21
             ],
             [
-                174,
+                202,
                 22
             ],
             [
-                172,
+                200,
                 1
             ],
             [
-                186,
+                214,
                 23
             ],
             [
-                46,
+                65,
                 24
             ],
             [
-                47,
+                66,
                 25
             ],
             [
-                44,
+                63,
                 26
             ],
             [
-                45,
+                64,
                 27
             ],
             [
-                48,
+                67,
                 28
             ],
             [
-                95,
+                123,
                 29
             ],
             [
-                97,
+                125,
                 30
             ],
             [
-                99,
+                127,
                 31
             ],
             [
-                98,
+                126,
                 32
             ],
             [
-                104,
+                132,
                 33
             ],
             [
-                102,
+                130,
                 34
             ],
             [
-                106,
+                134,
                 35
             ],
             [
-                37,
+                56,
                 36
             ],
             [
-                108,
+                136,
                 37
             ],
             [
-                109,
+                137,
                 38
             ],
             [
-                111,
+                139,
                 39
             ],
             [
-                110,
+                138,
                 40
             ],
             [
-                112,
+                140,
                 41
             ],
             [
-                107,
+                135,
                 42
             ],
             [
-                105,
+                133,
                 43
             ],
             [
-                113,
+                141,
                 44
             ],
             [
-                114,
+                142,
                 45
             ],
             [
-                118,
+                146,
                 46
             ],
             [
-                119,
+                147,
                 47
             ],
             [
-                117,
+                145,
                 48
             ],
             [
-                94,
+                122,
                 49
             ],
             [
-                40,
+                59,
                 50
             ],
             [
-                120,
+                148,
                 51
             ],
             [
-                121,
+                149,
                 52
             ],
             [
-                122,
+                150,
                 52
             ],
             [
-                124,
+                152,
                 53
             ],
             [
-                123,
+                151,
                 52
             ],
             [
-                138,
+                166,
                 54
             ],
             [
-                43,
+                62,
                 55
             ],
             [
-                125,
+                153,
                 56
             ],
             [
-                116,
+                144,
                 57
             ],
             [
-                127,
+                155,
                 58
             ],
             [
-                115,
+                143,
                 59
             ],
             [
-                128,
+                156,
                 60
             ],
             [
-                129,
+                157,
                 61
             ],
             [
-                130,
+                158,
                 29
             ],
             [
-                131,
+                159,
                 29
             ],
             [
-                132,
+                160,
                 62
             ],
             [
-                134,
+                162,
                 63
             ],
             [
-                135,
+                163,
                 64
             ],
             [
-                136,
+                164,
                 56
             ],
             [
-                39,
+                58,
                 65
             ],
             [
-                42,
+                61,
                 43
             ],
             [
-                137,
+                165,
                 66
             ],
             [
-                152,
+                180,
                 67
             ],
             [
-                154,
+                182,
                 68
             ],
             [
-                153,
+                181,
                 69
             ],
             [
-                241,
+                269,
                 70
             ],
             [
-                235,
+                263,
                 71
             ],
             [
-                233,
+                261,
                 71
             ],
             [
-                238,
+                266,
                 72
             ],
             [
-                236,
+                264,
                 71
             ],
             [
-                240,
+                268,
                 71
             ],
             [
-                243,
+                271,
                 73
             ],
             [
-                244,
+                272,
                 73
             ],
             [
-                245,
+                273,
                 74
             ],
             [
-                250,
+                278,
                 75
             ],
             [
-                249,
+                277,
                 76
             ],
             [
-                251,
+                279,
                 77
             ],
             [
-                252,
+                280,
                 77
             ],
             [
-                254,
+                282,
                 78
             ],
             [
-                255,
+                283,
                 79
             ],
             [
-                264,
+                292,
                 80
             ],
             [
-                259,
+                287,
                 81
             ],
             [
-                263,
+                291,
                 82
             ],
             [
-                261,
+                289,
                 83
             ],
             [
-                262,
+                290,
                 84
             ],
             [
-                260,
+                288,
                 85
             ],
             [
-                279,
+                307,
                 86
             ],
             [
-                280,
+                308,
                 87
             ],
             [
-                283,
+                311,
                 88
             ],
             [
-                284,
+                312,
                 89
             ],
             [
-                282,
+                310,
                 90
             ],
             [
-                285,
+                313,
                 91
             ],
             [
-                286,
+                314,
                 92
             ],
             [
-                287,
+                315,
                 93
             ],
             [
-                288,
+                316,
                 94
             ],
             [
-                289,
+                317,
                 95
             ],
             [
-                290,
+                318,
                 96
             ],
             [
-                291,
+                319,
                 97
             ],
             [
-                292,
+                320,
                 98
             ],
             [
-                293,
+                321,
                 99
             ],
             [
-                294,
+                322,
                 100
             ],
             [
-                49,
+                68,
                 101
             ],
             [
-                51,
+                69,
+                101
+            ],
+            [
+                71,
                 102
             ],
             [
-                52,
+                72,
                 103
             ],
             [
-                53,
+                73,
                 104
             ],
             [
-                54,
+                74,
                 105
             ],
             [
-                55,
+                75,
                 106
             ],
             [
-                56,
+                76,
                 107
             ],
             [
-                57,
+                77,
                 108
             ],
             [
-                58,
+                78,
                 109
             ],
             [
-                59,
+                79,
                 110
             ],
             [
-                60,
+                80,
                 111
             ],
             [
-                61,
+                81,
+                111
+            ],
+            [
+                82,
                 112
             ],
             [
-                62,
+                83,
                 113
             ],
             [
-                63,
+                84,
                 114
             ],
             [
-                64,
+                85,
                 115
             ],
             [
-                65,
+                86,
                 116
             ],
             [
-                66,
+                87,
                 117
             ],
             [
-                92,
+                88,
                 118
             ],
             [
-                67,
+                89,
                 119
             ],
             [
-                68,
+                120,
                 120
             ],
             [
-                69,
+                90,
                 121
             ],
             [
-                70,
+                91,
                 122
             ],
             [
-                71,
+                92,
                 123
             ],
             [
-                72,
+                93,
                 124
             ],
             [
-                73,
+                94,
                 125
             ],
             [
-                74,
+                95,
                 126
             ],
             [
-                75,
+                96,
                 127
             ],
             [
-                76,
+                97,
                 128
             ],
             [
-                77,
+                98,
                 129
             ],
             [
-                78,
+                99,
                 130
             ],
             [
-                79,
+                100,
                 131
             ],
             [
-                80,
+                101,
                 132
             ],
             [
-                81,
+                103,
                 133
             ],
             [
-                82,
+                102,
                 134
             ],
             [
-                83,
+                104,
                 135
             ],
             [
-                84,
+                105,
                 136
             ],
             [
-                85,
+                107,
                 137
             ],
             [
-                86,
+                108,
                 138
             ],
             [
-                87,
+                109,
                 139
             ],
             [
-                88,
+                110,
                 140
             ],
             [
-                89,
+                111,
                 141
             ],
             [
-                90,
+                112,
                 142
             ],
             [
-                324,
+                113,
                 143
             ],
             [
-                325,
+                114,
                 144
             ],
             [
-                300,
+                115,
                 145
             ],
             [
-                303,
-                145
+                116,
+                146
             ],
             [
-                322,
-                143
+                117,
+                147
             ],
             [
-                323,
-                143
+                118,
+                148
             ],
             [
-                313,
-                143
+                352,
+                149
             ],
             [
-                312,
-                146
+                353,
+                150
             ],
             [
-                310,
-                143
+                328,
+                151
             ],
             [
-                305,
-                143
+                331,
+                151
             ],
             [
-                318,
-                143
+                350,
+                149
             ],
             [
-                316,
-                143
+                351,
+                149
             ],
             [
-                320,
-                143
+                341,
+                149
             ],
             [
-                304,
-                143
+                340,
+                152
             ],
             [
-                317,
-                143
+                338,
+                149
             ],
             [
-                321,
-                143
+                333,
+                149
             ],
             [
-                306,
-                143
+                346,
+                149
             ],
             [
-                307,
-                143
+                344,
+                149
             ],
             [
-                319,
-                143
+                348,
+                149
             ],
             [
-                301,
-                143
+                332,
+                149
             ],
             [
-                308,
-                143
+                345,
+                149
             ],
             [
-                309,
-                143
+                349,
+                149
             ],
             [
-                311,
-                143
+                334,
+                149
             ],
             [
-                315,
-                143
+                335,
+                149
             ],
             [
-                326,
-                147
+                347,
+                149
             ],
             [
-                314,
-                143
+                329,
+                149
             ],
             [
-                302,
-                143
+                336,
+                149
             ],
             [
-                339,
-                148
+                337,
+                149
             ],
             [
-                333,
-                147
+                339,
+                149
             ],
             [
-                335,
+                343,
                 149
             ],
             [
-                334,
-                147
+                354,
+                153
             ],
             [
-                327,
-                147
+                342,
+                149
             ],
             [
-                328,
-                147
+                330,
+                149
             ],
             [
-                330,
-                147
+                367,
+                154
             ],
             [
-                332,
-                147
+                361,
+                153
             ],
             [
-                336,
-                149
+                363,
+                155
             ],
             [
-                337,
-                149
+                362,
+                153
             ],
             [
-                329,
-                149
+                355,
+                153
             ],
             [
-                331,
-                149
+                356,
+                153
             ],
             [
-                342,
-                150
+                358,
+                153
             ],
             [
-                344,
-                151
+                360,
+                153
             ],
             [
-                267,
-                152
+                364,
+                155
             ],
             [
-                276,
-                153
+                365,
+                155
             ],
             [
-                266,
-                154
+                357,
+                155
             ],
             [
-                277,
+                359,
                 155
             ],
             [
-                272,
+                370,
                 156
             ],
             [
-                273,
+                372,
                 157
             ],
             [
-                271,
+                295,
                 158
             ],
             [
-                275,
+                304,
                 159
             ],
             [
-                269,
+                294,
                 160
             ],
             [
-                268,
+                305,
                 161
             ],
             [
-                274,
+                300,
                 162
             ],
             [
-                270,
-                153
-            ],
-            [
-                32,
+                301,
                 163
             ],
             [
-                192,
+                299,
                 164
             ],
             [
-                221,
+                303,
                 165
             ],
             [
-                220,
+                297,
                 166
             ],
             [
-                222,
+                296,
                 167
             ],
             [
-                187,
+                302,
                 168
             ],
             [
-                190,
+                298,
+                159
+            ],
+            [
+                50,
                 169
             ],
             [
-                191,
+                51,
                 170
             ],
             [
-                189,
+                220,
                 171
             ],
             [
-                230,
+                249,
                 172
             ],
             [
-                225,
+                248,
                 173
             ],
             [
-                229,
+                250,
                 174
             ],
             [
-                224,
+                215,
                 175
             ],
             [
-                226,
+                216,
+                169
+            ],
+            [
+                218,
                 176
             ],
             [
-                228,
+                219,
                 177
+            ],
+            [
+                217,
+                178
+            ],
+            [
+                258,
+                179
+            ],
+            [
+                251,
+                169
+            ],
+            [
+                253,
+                180
+            ],
+            [
+                257,
+                181
+            ],
+            [
+                252,
+                182
+            ],
+            [
+                254,
+                183
+            ],
+            [
+                256,
+                184
             ]
         ],
         "semanticDiagnosticsPerFile": [
-            258,
-            207,
-            211,
+            286,
+            235,
+            239,
+            222,
+            223,
+            221,
+            224,
+            226,
+            225,
+            227,
+            236,
+            238,
+            237,
+            228,
+            229,
+            230,
+            232,
+            231,
+            234,
+            233,
+            186,
+            188,
+            187,
+            189,
+            190,
+            191,
+            184,
+            185,
+            172,
+            173,
+            170,
+            171,
+            169,
+            167,
+            168,
+            176,
+            174,
+            175,
+            240,
+            246,
+            241,
+            242,
+            243,
+            247,
+            244,
+            245,
+            177,
+            178,
+            183,
+            192,
+            193,
             194,
             195,
-            193,
             196,
-            198,
             197,
+            198,
+            203,
+            204,
             199,
-            208,
-            210,
-            209,
-            200,
             201,
             202,
-            204,
-            203,
-            206,
+            200,
             205,
-            158,
-            160,
-            159,
-            161,
-            162,
-            163,
-            156,
-            157,
-            144,
-            145,
-            142,
-            143,
-            141,
-            139,
-            140,
-            148,
-            146,
-            147,
+            206,
+            214,
+            207,
+            208,
+            209,
+            210,
+            211,
             212,
-            218,
             213,
-            214,
-            215,
-            219,
-            216,
-            217,
-            149,
-            150,
-            155,
-            164,
-            165,
-            166,
-            167,
-            168,
-            169,
-            170,
-            175,
-            176,
-            171,
-            173,
-            174,
-            172,
-            177,
-            178,
-            186,
-            179,
-            180,
-            181,
-            182,
-            183,
-            184,
-            185,
-            33,
-            35,
-            46,
-            47,
-            44,
-            45,
-            34,
-            48,
-            95,
-            97,
-            99,
-            98,
-            100,
-            104,
-            102,
-            103,
-            96,
-            106,
-            37,
-            108,
-            109,
-            111,
-            110,
-            112,
-            107,
-            105,
-            113,
-            114,
-            118,
-            119,
-            117,
-            94,
-            40,
-            120,
-            121,
-            122,
-            36,
-            124,
+            52,
+            54,
+            65,
+            66,
+            63,
+            64,
+            53,
+            67,
             123,
-            138,
-            38,
-            43,
             125,
-            126,
-            41,
-            116,
             127,
-            115,
+            126,
             128,
-            129,
+            132,
             130,
             131,
-            132,
-            101,
+            124,
             134,
-            135,
-            93,
+            56,
             136,
-            133,
-            39,
-            42,
             137,
-            151,
+            139,
+            138,
+            140,
+            135,
+            133,
+            141,
+            142,
+            146,
+            147,
+            145,
+            122,
+            59,
+            148,
+            149,
+            150,
+            55,
             152,
-            154,
+            151,
+            166,
+            57,
+            62,
             153,
-            231,
-            241,
-            235,
-            234,
-            233,
-            232,
-            238,
-            236,
-            237,
-            240,
-            239,
-            243,
-            244,
-            242,
-            245,
-            250,
-            246,
-            249,
-            247,
-            251,
-            252,
-            253,
-            254,
-            255,
-            264,
-            256,
+            154,
+            60,
+            144,
+            155,
+            143,
+            156,
+            157,
+            158,
+            159,
+            160,
+            129,
+            162,
+            163,
+            121,
+            164,
+            161,
+            58,
+            61,
+            165,
+            179,
+            180,
+            182,
+            181,
             259,
+            269,
             263,
-            261,
             262,
+            261,
             260,
+            266,
+            264,
+            265,
+            268,
+            267,
+            271,
+            272,
+            270,
+            273,
+            278,
+            274,
+            277,
+            275,
             279,
             280,
-            248,
             281,
+            282,
             283,
+            292,
             284,
-            282,
-            285,
-            286,
             287,
-            288,
+            291,
             289,
             290,
-            291,
-            292,
-            293,
-            294,
-            295,
-            296,
-            49,
-            51,
-            52,
-            53,
-            54,
-            55,
-            56,
-            57,
-            58,
-            59,
-            60,
-            61,
-            62,
-            63,
-            50,
-            91,
-            64,
-            65,
-            66,
-            92,
-            67,
+            288,
+            307,
+            308,
+            276,
+            309,
+            311,
+            312,
+            310,
+            313,
+            314,
+            315,
+            316,
+            317,
+            318,
+            319,
+            320,
+            321,
+            322,
+            323,
+            324,
             68,
             69,
-            70,
             71,
             72,
             73,
             74,
             75,
             76,
             77,
@@ -4155,127 +4397,177 @@
             80,
             81,
             82,
             83,
             84,
             85,
             86,
+            70,
+            119,
             87,
             88,
             89,
+            120,
             90,
-            297,
-            298,
-            299,
-            324,
+            91,
+            92,
+            93,
+            94,
+            95,
+            96,
+            97,
+            98,
+            99,
+            100,
+            101,
+            103,
+            102,
+            104,
+            105,
+            106,
+            107,
+            108,
+            109,
+            110,
+            111,
+            112,
+            113,
+            114,
+            115,
+            116,
+            117,
+            118,
             325,
-            300,
-            303,
-            322,
-            323,
-            313,
-            312,
-            310,
-            305,
-            318,
-            316,
-            320,
-            304,
-            317,
-            321,
-            306,
-            307,
-            319,
-            301,
-            308,
-            309,
-            311,
-            315,
             326,
-            314,
-            302,
-            339,
-            338,
-            333,
-            335,
-            334,
             327,
+            352,
+            353,
             328,
-            330,
+            331,
+            350,
+            351,
+            341,
+            340,
+            338,
+            333,
+            346,
+            344,
+            348,
             332,
+            345,
+            349,
+            334,
+            335,
+            347,
+            329,
             336,
             337,
-            329,
-            331,
-            340,
-            278,
-            341,
-            342,
+            339,
             343,
-            344,
-            257,
-            227,
-            267,
-            276,
-            265,
-            266,
-            277,
-            272,
-            273,
-            271,
-            275,
-            269,
-            268,
-            274,
-            270,
-            6,
-            7,
+            354,
+            342,
+            330,
+            367,
+            366,
+            361,
+            363,
+            362,
+            355,
+            356,
+            358,
+            360,
+            364,
+            365,
+            357,
+            359,
+            368,
+            306,
+            369,
+            370,
+            371,
+            372,
+            285,
+            255,
+            295,
+            304,
+            293,
+            294,
+            305,
+            300,
+            301,
+            299,
+            303,
+            297,
+            296,
+            302,
+            298,
+            49,
             9,
-            8,
-            2,
             10,
-            11,
             12,
+            11,
+            2,
             13,
             14,
             15,
             16,
             17,
-            3,
-            4,
-            21,
             18,
             19,
             20,
+            3,
+            4,
+            24,
+            21,
             22,
             23,
-            24,
-            5,
             25,
             26,
             27,
+            5,
             28,
             29,
-            1,
             30,
             31,
+            6,
+            35,
             32,
-            192,
-            221,
+            33,
+            34,
+            36,
+            7,
+            37,
+            42,
+            43,
+            38,
+            39,
+            40,
+            41,
+            8,
+            47,
+            44,
+            45,
+            46,
+            1,
+            48,
+            50,
+            51,
             220,
-            222,
-            187,
-            188,
-            190,
-            191,
-            189,
-            230,
-            223,
-            225,
-            229,
-            224,
-            226,
-            228
+            249,
+            248,
+            250,
+            215,
+            216,
+            218,
+            219,
+            217,
+            258,
+            251,
+            253,
+            257,
+            252,
+            254,
+            256
         ]
     },
     "version": "4.9.5"
 }
```

### Comparing `cdk8s-awscdk-resolver-0.0.97/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO` & `cdk8s-awscdk-resolver-0.0.98/src/cdk8s_awscdk_resolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-awscdk-resolver
-Version: 0.0.97
+Version: 0.0.98
 Summary: @cdk8s/awscdk-resolver
 Home-page: https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-awscdk-resolver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

