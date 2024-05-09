# Comparing `tmp/cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0.tar.gz` & `tmp/cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0.tar", last modified: Tue May  7 19:02:39 2024, max compression
+gzip compressed data, was "cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1.tar", last modified: Thu May  9 14:18:46 2024, max compression
```

## Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0.tar` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:39.746483 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-07 19:02:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 19:02:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-07 19:02:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-07 19:02:39.746483 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-07 19:02:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-07 19:02:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 19:02:39.746483 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-07 19:02:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:39.742483 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:39.742483 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:39.742483 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs/cdk_aws_iot_thing_certificate_policy/
--rw-r--r--   0 runner    (1001) docker     (127)    21476 2024-05-07 19:02:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:39.746483 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-07 19:02:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1212301 2024-05-07 19:02:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/cdk-aws-iot-thing-certificate-policy@0.0.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:02:28.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs/cdk_aws_iot_thing_certificate_policy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 19:02:39.742483 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-07 19:02:39.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-07 19:02:39.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 19:02:39.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 19:02:39.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 19:02:39.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:18:46.604357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-09 14:18:46.604357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:18:46.604357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:18:46.600357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:18:46.600357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:18:46.600357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/
+-rw-r--r--   0 runner    (1001) docker     (127)    22931 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:18:46.600357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1212807 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/cdk-aws-iot-thing-certificate-policy@0.0.1.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:18:34.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:18:46.600357 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-05-09 14:18:46.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-09 14:18:46.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:18:46.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 14:18:46.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 14:18:46.000000 cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/LICENSE` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/PKG-INFO` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,19 @@
-Metadata-Version: 2.1
-Name: cdklabs.cdk-aws-iot-thing-certificate-policy
-Version: 0.0.0
-Summary: Creates an AWS IoT thing, certificate, policy, and associates the three together
-Home-page: https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git
-Author: Amazon Web Services<aws-cdk-dev@amazon.com>
-License: Apache-2.0
-Project-URL: Source, https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: JavaScript
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved
-Requires-Python: ~=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: NOTICE
-
 # AWS IoT Thing, Certificate, and Policy Construct Library
 
+[![NPM](https://img.shields.io/npm/v/@cdklabs/cdk-aws-iot-thing-certificate-policy?label=npm+cdk+v2)](https://www.npmjs.com/package/@cdklabs/cdk-aws-iot-thing-certificate-policy)
+[![PyPI](https://img.shields.io/pypi/v/cdklabs.cdk-aws-iot-thing-certificate-policy?label=pypi+cdk+v2)](https://pypi.org/project/cdklabs.cdk-aws-iot-thing-certificate-policy/)
+[![Maven version](https://img.shields.io/maven-central/v/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy?label=maven+cdk+v2)](https://central.sonatype.com/artifact/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy)
+[![NuGet version](https://img.shields.io/nuget/v/Cdklabs.CdkAwsIotThingCertificatePolicy?label=nuget+cdk+v2)](https://www.nuget.org/packages/Cdklabs.CdkNag)
+[![Go version](https://img.shields.io/github/go-mod/go-version/cdklabs/cdk-aws-iot-thing-certificate-policy?label=go+cdk+v2)](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go)
+[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-cdk-constructs/blob/main/LICENSE)
+
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
-[![View on Construct Hub](https://constructs.dev/badge?package=cdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/cdk-aws-iot-thing-certificate-policy)
+[![View on Construct Hub](https://constructs.dev/badge?package=@cdklabs/cdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/@cdklabs/cdk-aws-iot-thing-certificate-policy)
 
 An [L3 CDK construct](https://docs.aws.amazon.com/cdk/v2/guide/constructs.html#constructs_lib) to create and associate a singular AWS IoT Thing, Certificate, and IoT Policy. The construct also retrieves and returns AWS IoT account specific details such as the AWS IoT data endpoint and the AWS IoT Credential provider endpoint.
 
 The certificate and its private key are stored as AWS Systems Manager Parameter Store parameters that can be retrieved via the AWS Console or programmatically via construct members.
 
 ## Installation and use
 
@@ -39,29 +22,29 @@
 
 **Installation:**
 
 ```shell
 npm install cdk-aws-iot-thing-certificate-policy
 ```
 
-[**API Reference**](doc/api-typescript.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-typescript.md)
 
 **Example:**
 
 ```python
 import aws_cdk as cdk
 from cdklabs.cdk_aws_iot_thing_certificate_policy import IotThingCertificatePolicy
 
 #
 # A minimum IoT Policy template using substitution variables for actual
 # policy to be deployed for "region", "account", and "thingname". Allows
 # the thing to publish and subscribe on any topics under "thing/*" topic
 # namespace. Normal IoT Policy conventions such as "*", apply.
 #
-minimal_io_tPolicy = """{
+minimal_iot_policy = """{
   "Version": "2012-10-17",
   "Statement": [
     {
       "Effect": "Allow",
       "Action": ["iot:Connect"],
       "Resource": "arn:aws:iot:{{region}}:{{account}}:client/{{thingname}}"
     },
@@ -94,15 +77,15 @@
 #
 # Create the thing, certificate, and policy, then associate the
 # certificate to both the thing and the policy and fully activate.
 #
 foo_thing = IotThingCertificatePolicy(app, "MyFooThing",
     thing_name="foo-thing",  # Name to assign to AWS IoT thing, and value for {{thingname}} in policy template
     iot_policy_name="foo-iot-policy",  # Name to assign to AWS IoT policy
-    iot_policy=minimal_io_tPolicy,  # Policy with or without substitution parameters from above
+    iot_policy=minimal_iot_policy,  # Policy with or without substitution parameters from above
     encryption_algorithm="ECC",  # Algorithm to use to private key (RSA or ECC)
     policy_parameter_mapping=[PolicyMapping(
         name="region",
         value=cdk.Fn.ref("AWS::Region")
     ), PolicyMapping(
         name="account",
         value=cdk.Fn.ref("AWS::AccountId")
@@ -123,18 +106,18 @@
 
 </details><details>
   <summary><b>Python</b></summary>
 
 **Installation:**
 
 ```shell
-pip install cdk-aws-iot-thing-certificate-policy
+pip install cdklabs.cdk-aws-iot-thing-certificate-policy
 ```
 
-[**API Reference**](doc/api-python.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-python.md)
 
 **Example:**
 
 ```python
 import aws_cdk as cdk
 from cdklabs.cdk_aws_iot_thing_certificate_policy import (
     IotThingCertificatePolicy,
@@ -173,15 +156,15 @@
 }"""
 
 app = cdk.App()
 
 foo_thing = IotThingCertificatePolicy(
     app,
     "MyFooThing",
-    thing_name="foo-thin",
+    thing_name="foo-thing",
     iot_policy_name="foo-iot-policy",
     iot_policy=minimal_iot_policy,
     encryption_algorithm="ECC",
     policy_parameter_mapping=[
         {
             "name": "region",
             "value": cdk.Fn.ref("AWS::Region")
@@ -190,51 +173,49 @@
             "name": "account",
             "value": cdk.Fn.ref("AWS::AccountId")
         }
     ],
 )
 cdk.CfnOutput(app, "ThingArn", value=foo_thing.thing_arn)
 cdk.CfnOutput(app, "IotEndpoint", value=foo_thing.data_ats_endpoint_address)
-
-app.synth()
 ```
 
 </details><details>
   <summary><b>Java</b></summary>
 
 **Installation:**
 
 ```shell
 Coming Soon
 ```
 
-[**API Reference**](doc/api-java.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-java.md)
 
 **Example:** *Coming soon*
 
 </details><details>
   <summary><b>C#</b></summary>
 
 **Installation:**
 
 ```shell
 dotnet add package Cdklabs.CdkAwsIotThingCertificatePolicy
 ```
 
-[**API Reference**](doc/api-csharp.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-csharp.md)
 
 **Example:** *coming soon*
 
 </details><details>
   <summary><b>Go</b></summary>
 
 **Installation:**
 
 ```shell
 Coming soon
 ```
 
-[**API Reference**](doc/api-go.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-go.md)
 
 **Example:** *coming soon*
 
 </details>
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/setup.py` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-aws-iot-thing-certificate-policy",
-    "version": "0.0.0",
+    "version": "0.0.1",
     "description": "Creates an AWS IoT thing, certificate, policy, and associates the three together",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdklabs.cdk_aws_iot_thing_certificate_policy",
         "cdklabs.cdk_aws_iot_thing_certificate_policy._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_aws_iot_thing_certificate_policy._jsii": [
-            "cdk-aws-iot-thing-certificate-policy@0.0.0.jsii.tgz"
+            "cdk-aws-iot-thing-certificate-policy@0.0.1.jsii.tgz"
         ],
         "cdklabs.cdk_aws_iot_thing_certificate_policy": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 '''
 # AWS IoT Thing, Certificate, and Policy Construct Library
 
+[![NPM](https://img.shields.io/npm/v/@cdklabs/cdk-aws-iot-thing-certificate-policy?label=npm+cdk+v2)](https://www.npmjs.com/package/@cdklabs/cdk-aws-iot-thing-certificate-policy)
+[![PyPI](https://img.shields.io/pypi/v/cdklabs.cdk-aws-iot-thing-certificate-policy?label=pypi+cdk+v2)](https://pypi.org/project/cdklabs.cdk-aws-iot-thing-certificate-policy/)
+[![Maven version](https://img.shields.io/maven-central/v/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy?label=maven+cdk+v2)](https://central.sonatype.com/artifact/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy)
+[![NuGet version](https://img.shields.io/nuget/v/Cdklabs.CdkAwsIotThingCertificatePolicy?label=nuget+cdk+v2)](https://www.nuget.org/packages/Cdklabs.CdkNag)
+[![Go version](https://img.shields.io/github/go-mod/go-version/cdklabs/cdk-aws-iot-thing-certificate-policy?label=go+cdk+v2)](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go)
+[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-cdk-constructs/blob/main/LICENSE)
+
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
-[![View on Construct Hub](https://constructs.dev/badge?package=cdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/cdk-aws-iot-thing-certificate-policy)
+[![View on Construct Hub](https://constructs.dev/badge?package=@cdklabs/cdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/@cdklabs/cdk-aws-iot-thing-certificate-policy)
 
 An [L3 CDK construct](https://docs.aws.amazon.com/cdk/v2/guide/constructs.html#constructs_lib) to create and associate a singular AWS IoT Thing, Certificate, and IoT Policy. The construct also retrieves and returns AWS IoT account specific details such as the AWS IoT data endpoint and the AWS IoT Credential provider endpoint.
 
 The certificate and its private key are stored as AWS Systems Manager Parameter Store parameters that can be retrieved via the AWS Console or programmatically via construct members.
 
 ## Installation and use
 
@@ -16,29 +23,29 @@
 
 **Installation:**
 
 ```shell
 npm install cdk-aws-iot-thing-certificate-policy
 ```
 
-[**API Reference**](doc/api-typescript.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-typescript.md)
 
 **Example:**
 
 ```python
 import aws_cdk as cdk
 from cdklabs.cdk_aws_iot_thing_certificate_policy import IotThingCertificatePolicy
 
 #
 # A minimum IoT Policy template using substitution variables for actual
 # policy to be deployed for "region", "account", and "thingname". Allows
 # the thing to publish and subscribe on any topics under "thing/*" topic
 # namespace. Normal IoT Policy conventions such as "*", apply.
 #
-minimal_io_tPolicy = """{
+minimal_iot_policy = """{
   "Version": "2012-10-17",
   "Statement": [
     {
       "Effect": "Allow",
       "Action": ["iot:Connect"],
       "Resource": "arn:aws:iot:{{region}}:{{account}}:client/{{thingname}}"
     },
@@ -71,15 +78,15 @@
 #
 # Create the thing, certificate, and policy, then associate the
 # certificate to both the thing and the policy and fully activate.
 #
 foo_thing = IotThingCertificatePolicy(app, "MyFooThing",
     thing_name="foo-thing",  # Name to assign to AWS IoT thing, and value for {{thingname}} in policy template
     iot_policy_name="foo-iot-policy",  # Name to assign to AWS IoT policy
-    iot_policy=minimal_io_tPolicy,  # Policy with or without substitution parameters from above
+    iot_policy=minimal_iot_policy,  # Policy with or without substitution parameters from above
     encryption_algorithm="ECC",  # Algorithm to use to private key (RSA or ECC)
     policy_parameter_mapping=[PolicyMapping(
         name="region",
         value=cdk.Fn.ref("AWS::Region")
     ), PolicyMapping(
         name="account",
         value=cdk.Fn.ref("AWS::AccountId")
@@ -100,18 +107,18 @@
 
 </details><details>
   <summary><b>Python</b></summary>
 
 **Installation:**
 
 ```shell
-pip install cdk-aws-iot-thing-certificate-policy
+pip install cdklabs.cdk-aws-iot-thing-certificate-policy
 ```
 
-[**API Reference**](doc/api-python.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-python.md)
 
 **Example:**
 
 ```python
 import aws_cdk as cdk
 from cdklabs.cdk_aws_iot_thing_certificate_policy import (
     IotThingCertificatePolicy,
@@ -150,15 +157,15 @@
 }"""
 
 app = cdk.App()
 
 foo_thing = IotThingCertificatePolicy(
     app,
     "MyFooThing",
-    thing_name="foo-thin",
+    thing_name="foo-thing",
     iot_policy_name="foo-iot-policy",
     iot_policy=minimal_iot_policy,
     encryption_algorithm="ECC",
     policy_parameter_mapping=[
         {
             "name": "region",
             "value": cdk.Fn.ref("AWS::Region")
@@ -167,54 +174,52 @@
             "name": "account",
             "value": cdk.Fn.ref("AWS::AccountId")
         }
     ],
 )
 cdk.CfnOutput(app, "ThingArn", value=foo_thing.thing_arn)
 cdk.CfnOutput(app, "IotEndpoint", value=foo_thing.data_ats_endpoint_address)
-
-app.synth()
 ```
 
 </details><details>
   <summary><b>Java</b></summary>
 
 **Installation:**
 
 ```shell
 Coming Soon
 ```
 
-[**API Reference**](doc/api-java.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-java.md)
 
 **Example:** *Coming soon*
 
 </details><details>
   <summary><b>C#</b></summary>
 
 **Installation:**
 
 ```shell
 dotnet add package Cdklabs.CdkAwsIotThingCertificatePolicy
 ```
 
-[**API Reference**](doc/api-csharp.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-csharp.md)
 
 **Example:** *coming soon*
 
 </details><details>
   <summary><b>Go</b></summary>
 
 **Installation:**
 
 ```shell
 Coming soon
 ```
 
-[**API Reference**](doc/api-go.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-go.md)
 
 **Example:** *coming soon*
 
 </details>
 '''
 from pkgutil import extend_path
 __path__ = extend_path(__path__, __name__)
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdklabs/cdk-aws-iot-thing-certificate-policy",
-    "0.0.0",
+    "0.0.1",
     __name__[0:-6],
-    "cdk-aws-iot-thing-certificate-policy@0.0.0.jsii.tgz",
+    "cdk-aws-iot-thing-certificate-policy@0.0.1.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/PKG-INFO` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-aws-iot-thing-certificate-policy
-Version: 0.0.0
+Version: 0.0.1
 Summary: Creates an AWS IoT thing, certificate, policy, and associates the three together
 Home-page: https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -20,17 +20,24 @@
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # AWS IoT Thing, Certificate, and Policy Construct Library
 
+[![NPM](https://img.shields.io/npm/v/@cdklabs/cdk-aws-iot-thing-certificate-policy?label=npm+cdk+v2)](https://www.npmjs.com/package/@cdklabs/cdk-aws-iot-thing-certificate-policy)
+[![PyPI](https://img.shields.io/pypi/v/cdklabs.cdk-aws-iot-thing-certificate-policy?label=pypi+cdk+v2)](https://pypi.org/project/cdklabs.cdk-aws-iot-thing-certificate-policy/)
+[![Maven version](https://img.shields.io/maven-central/v/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy?label=maven+cdk+v2)](https://central.sonatype.com/artifact/io.github.cdklabs/cdk-aws-iot-thing-certificate-policy)
+[![NuGet version](https://img.shields.io/nuget/v/Cdklabs.CdkAwsIotThingCertificatePolicy?label=nuget+cdk+v2)](https://www.nuget.org/packages/Cdklabs.CdkNag)
+[![Go version](https://img.shields.io/github/go-mod/go-version/cdklabs/cdk-aws-iot-thing-certificate-policy?label=go+cdk+v2)](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy-go)
+[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-cdk-constructs/blob/main/LICENSE)
+
 ![cdk-constructs: Experimental](https://img.shields.io/badge/cdk--constructs-experimental-important.svg?style=for-the-badge)
 
-[![View on Construct Hub](https://constructs.dev/badge?package=cdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/cdk-aws-iot-thing-certificate-policy)
+[![View on Construct Hub](https://constructs.dev/badge?package=@cdklabs/cdk-aws-iot-thing-certificate-policy)](https://constructs.dev/packages/@cdklabs/cdk-aws-iot-thing-certificate-policy)
 
 An [L3 CDK construct](https://docs.aws.amazon.com/cdk/v2/guide/constructs.html#constructs_lib) to create and associate a singular AWS IoT Thing, Certificate, and IoT Policy. The construct also retrieves and returns AWS IoT account specific details such as the AWS IoT data endpoint and the AWS IoT Credential provider endpoint.
 
 The certificate and its private key are stored as AWS Systems Manager Parameter Store parameters that can be retrieved via the AWS Console or programmatically via construct members.
 
 ## Installation and use
 
@@ -39,29 +46,29 @@
 
 **Installation:**
 
 ```shell
 npm install cdk-aws-iot-thing-certificate-policy
 ```
 
-[**API Reference**](doc/api-typescript.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-typescript.md)
 
 **Example:**
 
 ```python
 import aws_cdk as cdk
 from cdklabs.cdk_aws_iot_thing_certificate_policy import IotThingCertificatePolicy
 
 #
 # A minimum IoT Policy template using substitution variables for actual
 # policy to be deployed for "region", "account", and "thingname". Allows
 # the thing to publish and subscribe on any topics under "thing/*" topic
 # namespace. Normal IoT Policy conventions such as "*", apply.
 #
-minimal_io_tPolicy = """{
+minimal_iot_policy = """{
   "Version": "2012-10-17",
   "Statement": [
     {
       "Effect": "Allow",
       "Action": ["iot:Connect"],
       "Resource": "arn:aws:iot:{{region}}:{{account}}:client/{{thingname}}"
     },
@@ -94,15 +101,15 @@
 #
 # Create the thing, certificate, and policy, then associate the
 # certificate to both the thing and the policy and fully activate.
 #
 foo_thing = IotThingCertificatePolicy(app, "MyFooThing",
     thing_name="foo-thing",  # Name to assign to AWS IoT thing, and value for {{thingname}} in policy template
     iot_policy_name="foo-iot-policy",  # Name to assign to AWS IoT policy
-    iot_policy=minimal_io_tPolicy,  # Policy with or without substitution parameters from above
+    iot_policy=minimal_iot_policy,  # Policy with or without substitution parameters from above
     encryption_algorithm="ECC",  # Algorithm to use to private key (RSA or ECC)
     policy_parameter_mapping=[PolicyMapping(
         name="region",
         value=cdk.Fn.ref("AWS::Region")
     ), PolicyMapping(
         name="account",
         value=cdk.Fn.ref("AWS::AccountId")
@@ -123,18 +130,18 @@
 
 </details><details>
   <summary><b>Python</b></summary>
 
 **Installation:**
 
 ```shell
-pip install cdk-aws-iot-thing-certificate-policy
+pip install cdklabs.cdk-aws-iot-thing-certificate-policy
 ```
 
-[**API Reference**](doc/api-python.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-python.md)
 
 **Example:**
 
 ```python
 import aws_cdk as cdk
 from cdklabs.cdk_aws_iot_thing_certificate_policy import (
     IotThingCertificatePolicy,
@@ -173,15 +180,15 @@
 }"""
 
 app = cdk.App()
 
 foo_thing = IotThingCertificatePolicy(
     app,
     "MyFooThing",
-    thing_name="foo-thin",
+    thing_name="foo-thing",
     iot_policy_name="foo-iot-policy",
     iot_policy=minimal_iot_policy,
     encryption_algorithm="ECC",
     policy_parameter_mapping=[
         {
             "name": "region",
             "value": cdk.Fn.ref("AWS::Region")
@@ -190,51 +197,49 @@
             "name": "account",
             "value": cdk.Fn.ref("AWS::AccountId")
         }
     ],
 )
 cdk.CfnOutput(app, "ThingArn", value=foo_thing.thing_arn)
 cdk.CfnOutput(app, "IotEndpoint", value=foo_thing.data_ats_endpoint_address)
-
-app.synth()
 ```
 
 </details><details>
   <summary><b>Java</b></summary>
 
 **Installation:**
 
 ```shell
 Coming Soon
 ```
 
-[**API Reference**](doc/api-java.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-java.md)
 
 **Example:** *Coming soon*
 
 </details><details>
   <summary><b>C#</b></summary>
 
 **Installation:**
 
 ```shell
 dotnet add package Cdklabs.CdkAwsIotThingCertificatePolicy
 ```
 
-[**API Reference**](doc/api-csharp.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-csharp.md)
 
 **Example:** *coming soon*
 
 </details><details>
   <summary><b>Go</b></summary>
 
 **Installation:**
 
 ```shell
 Coming soon
 ```
 
-[**API Reference**](doc/api-go.md)
+[**API Reference**](https://github.com/cdklabs/cdk-aws-iot-thing-certificate-policy/blob/main/doc/api-go.md)
 
 **Example:** *coming soon*
 
 </details>
```

### Comparing `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.0/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt` & `cdklabs.cdk-aws-iot-thing-certificate-policy-0.0.1/src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/SOURCES.txt
 src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/dependency_links.txt
 src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/requires.txt
 src/cdklabs.cdk_aws_iot_thing_certificate_policy.egg-info/top_level.txt
 src/cdklabs/cdk_aws_iot_thing_certificate_policy/__init__.py
 src/cdklabs/cdk_aws_iot_thing_certificate_policy/py.typed
 src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/__init__.py
-src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/cdk-aws-iot-thing-certificate-policy@0.0.0.jsii.tgz
+src/cdklabs/cdk_aws_iot_thing_certificate_policy/_jsii/cdk-aws-iot-thing-certificate-policy@0.0.1.jsii.tgz
```

