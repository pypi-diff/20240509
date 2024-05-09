# Comparing `tmp/lightkube-models-1.30.0.7.tar.gz` & `tmp/lightkube-models-1.30.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightkube-models-1.30.0.7.tar", last modified: Sun Apr 21 10:51:17 2024, max compression
+gzip compressed data, was "lightkube-models-1.30.0.8.tar", last modified: Thu May  9 09:09:23 2024, max compression
```

## Comparing `lightkube-models-1.30.0.7.tar` & `lightkube-models-1.30.0.8.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-04-21 10:51:17.510192 lightkube-models-1.30.0.7/
--rw-r--r--   0 tribulat   (501) staff       (20)     1096 2021-01-09 13:57:13.000000 lightkube-models-1.30.0.7/LICENSE
--rw-r--r--   0 tribulat   (501) staff       (20)     1378 2024-04-21 10:51:17.509579 lightkube-models-1.30.0.7/PKG-INFO
--rw-r--r--   0 tribulat   (501) staff       (20)      417 2020-09-14 18:55:30.000000 lightkube-models-1.30.0.7/README.md
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-04-21 10:51:17.450213 lightkube-models-1.30.0.7/lightkube/
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-04-21 10:51:17.481671 lightkube-models-1.30.0.7/lightkube/models/
--rw-r--r--   0 tribulat   (501) staff       (20)       25 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/__init__.py
--rw-r--r--   0 tribulat   (501) staff       (20)      871 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/_schema.py
--rw-r--r--   0 tribulat   (501) staff       (20)    65196 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/admissionregistration_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    37935 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/admissionregistration_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    38343 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/admissionregistration_v1beta1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    43556 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/apiextensions_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     8199 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/apiregistration_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     5951 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/apiserverinternal_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    47886 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/apps_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    10607 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/authentication_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2325 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/authentication_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2325 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/authentication_v1beta1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    16856 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/authorization_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     9179 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/autoscaling_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    26370 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/autoscaling_v2.py
--rw-r--r--   0 tribulat   (501) staff       (20)    35482 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/batch_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    13593 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/certificates_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     5459 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/certificates_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     3963 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/coordination_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)   333061 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/core_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    10437 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/discovery_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     7345 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/events_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    27780 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/flowcontrol_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    27612 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/flowcontrol_v1beta3.py
--rw-r--r--   0 tribulat   (501) staff       (20)    39009 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/meta_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    31870 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/networking_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     8474 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/networking_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     5709 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/node_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    10583 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/policy_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    15009 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/models/rbac_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      287 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/resource.py
--rw-r--r--   0 tribulat   (501) staff       (20)    41462 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/resource_v1alpha2.py
--rw-r--r--   0 tribulat   (501) staff       (20)      316 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/runtime.py
--rw-r--r--   0 tribulat   (501) staff       (20)     4010 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/scheduling_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    35278 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/storage_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     4091 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/storage_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     5645 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/storagemigration_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      327 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/util_intstr.py
--rw-r--r--   0 tribulat   (501) staff       (20)      909 2024-04-21 10:51:12.000000 lightkube-models-1.30.0.7/lightkube/models/version.py
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-04-21 10:51:17.505703 lightkube-models-1.30.0.7/lightkube/resources/
--rw-r--r--   0 tribulat   (501) staff       (20)     3562 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/admissionregistration_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2330 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/admissionregistration_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2318 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/admissionregistration_v1beta1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1504 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/apiextensions_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1340 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/apiregistration_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     7160 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/apps_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      974 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/authentication_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      607 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/authentication_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      602 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/authentication_v1beta1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1952 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/authorization_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1525 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/autoscaling_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1525 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/autoscaling_v2.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2342 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/batch_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2249 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/certificates_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      746 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/certificates_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      716 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/coordination_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)    17870 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/core_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      741 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/discovery_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      686 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/events_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2732 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/flowcontrol_apiserver_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2812 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/flowcontrol_apiserver_v1beta3.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1467 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/internal_apiserver_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2471 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/networking_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1900 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/networking_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      647 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/node_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1428 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/policy_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     2360 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/rbac_authorization_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     5916 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/resource_v1alpha2.py
--rw-r--r--   0 tribulat   (501) staff       (20)      682 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/scheduling_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     3503 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/storage_v1.py
--rw-r--r--   0 tribulat   (501) staff       (20)      737 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/storage_v1alpha1.py
--rw-r--r--   0 tribulat   (501) staff       (20)     1572 2024-04-21 10:51:11.000000 lightkube-models-1.30.0.7/lightkube/resources/storagemigration_v1alpha1.py
-drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-04-21 10:51:17.508772 lightkube-models-1.30.0.7/lightkube_models.egg-info/
--rw-r--r--   0 tribulat   (501) staff       (20)     1378 2024-04-21 10:51:17.000000 lightkube-models-1.30.0.7/lightkube_models.egg-info/PKG-INFO
--rw-r--r--   0 tribulat   (501) staff       (20)     2887 2024-04-21 10:51:17.000000 lightkube-models-1.30.0.7/lightkube_models.egg-info/SOURCES.txt
--rw-r--r--   0 tribulat   (501) staff       (20)        1 2024-04-21 10:51:17.000000 lightkube-models-1.30.0.7/lightkube_models.egg-info/dependency_links.txt
--rw-r--r--   0 tribulat   (501) staff       (20)       10 2024-04-21 10:51:17.000000 lightkube-models-1.30.0.7/lightkube_models.egg-info/top_level.txt
--rw-r--r--   0 tribulat   (501) staff       (20)       38 2024-04-21 10:51:17.510323 lightkube-models-1.30.0.7/setup.cfg
--rw-r--r--   0 tribulat   (501) staff       (20)     1109 2023-12-20 10:03:39.000000 lightkube-models-1.30.0.7/setup.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-05-09 09:09:23.178811 lightkube-models-1.30.0.8/
+-rw-r--r--   0 tribulat   (501) staff       (20)     1096 2021-01-09 13:57:13.000000 lightkube-models-1.30.0.8/LICENSE
+-rw-r--r--   0 tribulat   (501) staff       (20)     1378 2024-05-09 09:09:23.178430 lightkube-models-1.30.0.8/PKG-INFO
+-rw-r--r--   0 tribulat   (501) staff       (20)      417 2020-09-14 18:55:30.000000 lightkube-models-1.30.0.8/README.md
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-05-09 09:09:23.116892 lightkube-models-1.30.0.8/lightkube/
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-05-09 09:09:23.154641 lightkube-models-1.30.0.8/lightkube/models/
+-rw-r--r--   0 tribulat   (501) staff       (20)       25 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/__init__.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      871 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/_schema.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    65222 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/admissionregistration_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    37952 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/admissionregistration_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    38360 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/admissionregistration_v1beta1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    43575 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/apiextensions_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     8205 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/apiregistration_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5956 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/apiserverinternal_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    47916 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/apps_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    10617 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/authentication_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2327 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/authentication_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2327 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/authentication_v1beta1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    16869 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/authorization_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     9187 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/autoscaling_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    26394 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/autoscaling_v2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    35499 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/batch_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    13598 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/certificates_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5462 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/certificates_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     3966 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/coordination_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)   333267 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/core_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    10444 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/discovery_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     7348 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/events_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    27803 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/flowcontrol_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    27635 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/flowcontrol_v1beta3.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    39029 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/meta_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    31896 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/networking_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     8482 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/networking_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5713 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/node_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    10588 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/policy_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    15021 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/rbac_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      287 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/resource.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    41501 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/resource_v1alpha2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      316 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/runtime.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     4012 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/scheduling_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    35297 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/storage_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     4093 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/storage_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5651 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/storagemigration_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      327 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/util_intstr.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      910 2024-05-09 09:09:17.000000 lightkube-models-1.30.0.8/lightkube/models/version.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-05-09 09:09:23.175547 lightkube-models-1.30.0.8/lightkube/resources/
+-rw-r--r--   0 tribulat   (501) staff       (20)     3562 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/admissionregistration_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2330 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/admissionregistration_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2318 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/admissionregistration_v1beta1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1504 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/apiextensions_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1340 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/apiregistration_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     7160 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/apps_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      974 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/authentication_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      607 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/authentication_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      602 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/authentication_v1beta1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1952 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/authorization_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1525 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/autoscaling_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1525 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/autoscaling_v2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2342 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/batch_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2249 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/certificates_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      746 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/certificates_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      716 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/coordination_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)    17870 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/core_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      741 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/discovery_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      686 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/events_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2732 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/flowcontrol_apiserver_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2812 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/flowcontrol_apiserver_v1beta3.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1467 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/internal_apiserver_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2471 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/networking_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1900 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/networking_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      647 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/node_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1428 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/policy_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     2360 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/rbac_authorization_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     5916 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/resource_v1alpha2.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      682 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/scheduling_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     3503 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/storage_v1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)      737 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/storage_v1alpha1.py
+-rw-r--r--   0 tribulat   (501) staff       (20)     1572 2024-05-09 09:09:16.000000 lightkube-models-1.30.0.8/lightkube/resources/storagemigration_v1alpha1.py
+drwxr-xr-x   0 tribulat   (501) staff       (20)        0 2024-05-09 09:09:23.177791 lightkube-models-1.30.0.8/lightkube_models.egg-info/
+-rw-r--r--   0 tribulat   (501) staff       (20)     1378 2024-05-09 09:09:23.000000 lightkube-models-1.30.0.8/lightkube_models.egg-info/PKG-INFO
+-rw-r--r--   0 tribulat   (501) staff       (20)     2887 2024-05-09 09:09:23.000000 lightkube-models-1.30.0.8/lightkube_models.egg-info/SOURCES.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)        1 2024-05-09 09:09:23.000000 lightkube-models-1.30.0.8/lightkube_models.egg-info/dependency_links.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)       10 2024-05-09 09:09:23.000000 lightkube-models-1.30.0.8/lightkube_models.egg-info/top_level.txt
+-rw-r--r--   0 tribulat   (501) staff       (20)       38 2024-05-09 09:09:23.178960 lightkube-models-1.30.0.8/setup.cfg
+-rw-r--r--   0 tribulat   (501) staff       (20)     1109 2023-12-20 10:03:39.000000 lightkube-models-1.30.0.8/setup.py
```

### Comparing `lightkube-models-1.30.0.7/LICENSE` & `lightkube-models-1.30.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/PKG-INFO` & `lightkube-models-1.30.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightkube-models
-Version: 1.30.0.7
+Version: 1.30.0.8
 Summary: Models and Resources for lightkube module
 Home-page: https://github.com/gtsystem/lightkube-models
 Author: Giuseppe Tribulato
 Author-email: gtsystem@gmail.com
 License: Apache Software License
 Description: # lightkube-models
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/_schema.py` & `lightkube-models-1.30.0.8/lightkube/models/_schema.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/models/admissionregistration_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/admissionregistration_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class AuditAnnotation(DictMixin):
-    """AuditAnnotation describes how to produce an audit annotation for an API
+    r"""AuditAnnotation describes how to produce an audit annotation for an API
       request.
 
       **parameters**
 
       * **key** ``str`` - key specifies the audit annotation key. The audit annotation keys of a
         ValidatingAdmissionPolicy must be unique. The key must be a qualified name
         ([A-Za-z0-9][-A-Za-z0-9_.]*) no more than 63 bytes in length.
@@ -42,15 +42,15 @@
     """
     key: 'str'
     valueExpression: 'str'
 
 
 @dataclass
 class ExpressionWarning(DictMixin):
-    """ExpressionWarning is a warning information that targets a specific expression.
+    r"""ExpressionWarning is a warning information that targets a specific expression.
 
       **parameters**
 
       * **fieldRef** ``str`` - The path to the field that refers the expression. For example, the reference
         to the expression of the first item of validations is
         "spec.validations[0].expression"
       * **warning** ``str`` - The content of type checking information in a human-readable form. Each line
@@ -59,15 +59,15 @@
     """
     fieldRef: 'str'
     warning: 'str'
 
 
 @dataclass
 class MatchCondition(DictMixin):
-    """MatchCondition represents a condition which must by fulfilled for a request to
+    r"""MatchCondition represents a condition which must by fulfilled for a request to
       be sent to a webhook.
 
       **parameters**
 
       * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. Must
         evaluate to bool. CEL expressions have access to the contents of the
         AdmissionRequest and Authorizer, organized into CEL variables:
@@ -95,15 +95,15 @@
     """
     expression: 'str'
     name: 'str'
 
 
 @dataclass
 class MatchResources(DictMixin):
-    """MatchResources decides whether to run the admission control policy on an
+    r"""MatchResources decides whether to run the admission control policy on an
       object based on whether it meets the match criteria. The exclude rules take
       precedence over include rules (if a resource matches both, it is excluded)
 
       **parameters**
 
       * **excludeResourceRules** ``Optional[List[NamedRuleWithOperations]]`` - ExcludeResourceRules describes what operations on what resources/subresources
         the ValidatingAdmissionPolicy should not care about. The exclude rules take
@@ -176,15 +176,15 @@
     namespaceSelector: 'Optional[meta_v1.LabelSelector]' = None
     objectSelector: 'Optional[meta_v1.LabelSelector]' = None
     resourceRules: 'Optional[List[NamedRuleWithOperations]]' = None
 
 
 @dataclass
 class MutatingWebhook(DictMixin):
-    """MutatingWebhook describes an admission webhook and the resources and
+    r"""MutatingWebhook describes an admission webhook and the resources and
       operations it applies to.
 
       **parameters**
 
       * **admissionReviewVersions** ``List[str]`` - AdmissionReviewVersions is an ordered list of preferred `AdmissionReview`
         versions the Webhook expects. API server will try to use first version in the
         list which it supports. If none of the versions specified in this list
@@ -316,15 +316,15 @@
     reinvocationPolicy: 'Optional[str]' = None
     rules: 'Optional[List[RuleWithOperations]]' = None
     timeoutSeconds: 'Optional[int]' = None
 
 
 @dataclass
 class MutatingWebhookConfiguration(DictMixin):
-    """MutatingWebhookConfiguration describes the configuration of and admission
+    r"""MutatingWebhookConfiguration describes the configuration of and admission
       webhook that accept or reject and may change the object.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -341,15 +341,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     webhooks: 'Optional[List[MutatingWebhook]]' = None
 
 
 @dataclass
 class MutatingWebhookConfigurationList(DictMixin):
-    """MutatingWebhookConfigurationList is a list of MutatingWebhookConfiguration.
+    r"""MutatingWebhookConfigurationList is a list of MutatingWebhookConfiguration.
 
       **parameters**
 
       * **items** ``List[MutatingWebhookConfiguration]`` - List of MutatingWebhookConfiguration.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -365,15 +365,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class NamedRuleWithOperations(DictMixin):
-    """NamedRuleWithOperations is a tuple of Operations and Resources with
+    r"""NamedRuleWithOperations is a tuple of Operations and Resources with
       ResourceNames.
 
       **parameters**
 
       * **apiGroups** ``Optional[List[str]]`` - APIGroups is the API groups the resources belong to. '*' is all groups. If '*'
         is present, the length of the slice must be one. Required.
       * **apiVersions** ``Optional[List[str]]`` - APIVersions is the API versions the resources belong to. '*' is all versions.
@@ -406,29 +406,29 @@
     resourceNames: 'Optional[List[str]]' = None
     resources: 'Optional[List[str]]' = None
     scope: 'Optional[str]' = None
 
 
 @dataclass
 class ParamKind(DictMixin):
-    """ParamKind is a tuple of Group Kind and Version.
+    r"""ParamKind is a tuple of Group Kind and Version.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion is the API group version the resources belong to. In format of
         "group/version". Required.
       * **kind** ``Optional[str]`` - Kind is the API kind the resources belong to. Required.
     """
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
 
 
 @dataclass
 class ParamRef(DictMixin):
-    """ParamRef describes how to locate the params to be used as input to expressions
+    r"""ParamRef describes how to locate the params to be used as input to expressions
       of rules applied by a policy binding.
 
       **parameters**
 
       * **name** ``Optional[str]`` - name is the name of the resource being referenced.
         One of `name` or `selector` must be set, but `name` and `selector` are
         mutually exclusive properties. If one is set, the other must be unset.
@@ -465,15 +465,15 @@
     namespace: 'Optional[str]' = None
     parameterNotFoundAction: 'Optional[str]' = None
     selector: 'Optional[meta_v1.LabelSelector]' = None
 
 
 @dataclass
 class RuleWithOperations(DictMixin):
-    """RuleWithOperations is a tuple of Operations and Resources. It is recommended
+    r"""RuleWithOperations is a tuple of Operations and Resources. It is recommended
       to make sure that all the tuple expansions are valid.
 
       **parameters**
 
       * **apiGroups** ``Optional[List[str]]`` - APIGroups is the API groups the resources belong to. '*' is all groups. If '*'
         is present, the length of the slice must be one. Required.
       * **apiVersions** ``Optional[List[str]]`` - APIVersions is the API versions the resources belong to. '*' is all versions.
@@ -503,15 +503,15 @@
     operations: 'Optional[List[str]]' = None
     resources: 'Optional[List[str]]' = None
     scope: 'Optional[str]' = None
 
 
 @dataclass
 class ServiceReference(DictMixin):
-    """ServiceReference holds a reference to Service.legacy.k8s.io
+    r"""ServiceReference holds a reference to Service.legacy.k8s.io
 
       **parameters**
 
       * **name** ``str`` - `name` is the name of the service. Required
       * **namespace** ``str`` - `namespace` is the namespace of the service. Required
       * **path** ``Optional[str]`` - `path` is an optional URL path which will be sent in any request to this
         service.
@@ -523,27 +523,27 @@
     namespace: 'str'
     path: 'Optional[str]' = None
     port: 'Optional[int]' = None
 
 
 @dataclass
 class TypeChecking(DictMixin):
-    """TypeChecking contains results of type checking the expressions in the
+    r"""TypeChecking contains results of type checking the expressions in the
       ValidatingAdmissionPolicy
 
       **parameters**
 
       * **expressionWarnings** ``Optional[List[ExpressionWarning]]`` - The type checking warnings for each expression.
     """
     expressionWarnings: 'Optional[List[ExpressionWarning]]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicy(DictMixin):
-    """ValidatingAdmissionPolicy describes the definition of an admission validation
+    r"""ValidatingAdmissionPolicy describes the definition of an admission validation
       policy that accepts or rejects an object without changing it.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -564,15 +564,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[ValidatingAdmissionPolicySpec]' = None
     status: 'Optional[ValidatingAdmissionPolicyStatus]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyBinding(DictMixin):
-    """ValidatingAdmissionPolicyBinding binds the ValidatingAdmissionPolicy with
+    r"""ValidatingAdmissionPolicyBinding binds the ValidatingAdmissionPolicy with
       paramerized resources. ValidatingAdmissionPolicyBinding and parameter CRDs
       together define how cluster administrators configure policies for clusters.
       
       For a given admission request, each binding will cause its policy to be
       evaluated N times, where N is 1 for policies/bindings that don't use params,
       otherwise N is the number of parameters selected by the binding.
       
@@ -600,15 +600,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[ValidatingAdmissionPolicyBindingSpec]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyBindingList(DictMixin):
-    """ValidatingAdmissionPolicyBindingList is a list of
+    r"""ValidatingAdmissionPolicyBindingList is a list of
       ValidatingAdmissionPolicyBinding.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -625,15 +625,15 @@
     items: 'Optional[List[ValidatingAdmissionPolicyBinding]]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyBindingSpec(DictMixin):
-    """ValidatingAdmissionPolicyBindingSpec is the specification of the
+    r"""ValidatingAdmissionPolicyBindingSpec is the specification of the
       ValidatingAdmissionPolicyBinding.
 
       **parameters**
 
       * **matchResources** ``Optional[MatchResources]`` - MatchResources declares what resources match this binding and will be
         validated by it. Note that this is intersected with the policy's
         matchConstraints, so only requests that are matched by the policy can be
@@ -691,15 +691,15 @@
     paramRef: 'Optional[ParamRef]' = None
     policyName: 'Optional[str]' = None
     validationActions: 'Optional[List[str]]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyList(DictMixin):
-    """ValidatingAdmissionPolicyList is a list of ValidatingAdmissionPolicy.
+    r"""ValidatingAdmissionPolicyList is a list of ValidatingAdmissionPolicy.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -715,15 +715,15 @@
     items: 'Optional[List[ValidatingAdmissionPolicy]]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicySpec(DictMixin):
-    """ValidatingAdmissionPolicySpec is the specification of the desired behavior of
+    r"""ValidatingAdmissionPolicySpec is the specification of the desired behavior of
       the AdmissionPolicy.
 
       **parameters**
 
       * **auditAnnotations** ``Optional[List[AuditAnnotation]]`` - auditAnnotations contains CEL expressions which are used to produce audit
         annotations for the audit event of the API request. validations and
         auditAnnotations may not both be empty; a least one of validations or
@@ -782,15 +782,15 @@
     paramKind: 'Optional[ParamKind]' = None
     validations: 'Optional[List[Validation]]' = None
     variables: 'Optional[List[Variable]]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyStatus(DictMixin):
-    """ValidatingAdmissionPolicyStatus represents the status of an admission
+    r"""ValidatingAdmissionPolicyStatus represents the status of an admission
       validation policy.
 
       **parameters**
 
       * **conditions** ``Optional[List[meta_v1.Condition]]`` - The conditions represent the latest available observations of a policy's
         current state.
       * **observedGeneration** ``Optional[int]`` - The generation observed by the controller.
@@ -800,15 +800,15 @@
     conditions: 'Optional[List[meta_v1.Condition]]' = None
     observedGeneration: 'Optional[int]' = None
     typeChecking: 'Optional[TypeChecking]' = None
 
 
 @dataclass
 class ValidatingWebhook(DictMixin):
-    """ValidatingWebhook describes an admission webhook and the resources and
+    r"""ValidatingWebhook describes an admission webhook and the resources and
       operations it applies to.
 
       **parameters**
 
       * **admissionReviewVersions** ``List[str]`` - AdmissionReviewVersions is an ordered list of preferred `AdmissionReview`
         versions the Webhook expects. API server will try to use first version in the
         list which it supports. If none of the versions specified in this list
@@ -923,15 +923,15 @@
     objectSelector: 'Optional[meta_v1.LabelSelector]' = None
     rules: 'Optional[List[RuleWithOperations]]' = None
     timeoutSeconds: 'Optional[int]' = None
 
 
 @dataclass
 class ValidatingWebhookConfiguration(DictMixin):
-    """ValidatingWebhookConfiguration describes the configuration of and admission
+    r"""ValidatingWebhookConfiguration describes the configuration of and admission
       webhook that accept or reject and object without changing it.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -948,15 +948,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     webhooks: 'Optional[List[ValidatingWebhook]]' = None
 
 
 @dataclass
 class ValidatingWebhookConfigurationList(DictMixin):
-    """ValidatingWebhookConfigurationList is a list of
+    r"""ValidatingWebhookConfigurationList is a list of
       ValidatingWebhookConfiguration.
 
       **parameters**
 
       * **items** ``List[ValidatingWebhookConfiguration]`` - List of ValidatingWebhookConfiguration.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -973,15 +973,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class Validation(DictMixin):
-    """Validation specifies the CEL expression which is used to apply the validation.
+    r"""Validation specifies the CEL expression which is used to apply the validation.
 
       **parameters**
 
       * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. ref:
         https://github.com/google/cel-spec CEL expressions have access to the contents
         of the API request/response, organized into CEL variables as well as some
         other useful variables:
@@ -1064,15 +1064,15 @@
     message: 'Optional[str]' = None
     messageExpression: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class Variable(DictMixin):
-    """Variable is the definition of a variable that is used for composition. A
+    r"""Variable is the definition of a variable that is used for composition. A
       variable is defined as a named expression.
 
       **parameters**
 
       * **expression** ``str`` - Expression is the expression that will be evaluated as the value of the
         variable. The CEL expression has access to the same identifiers as the CEL
         expressions in Validation.
@@ -1083,15 +1083,15 @@
     """
     expression: 'str'
     name: 'str'
 
 
 @dataclass
 class WebhookClientConfig(DictMixin):
-    """WebhookClientConfig contains the information to make a TLS connection with the
+    r"""WebhookClientConfig contains the information to make a TLS connection with the
       webhook
 
       **parameters**
 
       * **caBundle** ``Optional[str]`` - `caBundle` is a PEM encoded CA bundle which will be used to validate the
         webhook's server certificate. If unspecified, system trust roots on the
         apiserver are used.
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/admissionregistration_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/models/admissionregistration_v1alpha1.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class AuditAnnotation(DictMixin):
-    """AuditAnnotation describes how to produce an audit annotation for an API
+    r"""AuditAnnotation describes how to produce an audit annotation for an API
       request.
 
       **parameters**
 
       * **key** ``str`` - key specifies the audit annotation key. The audit annotation keys of a
         ValidatingAdmissionPolicy must be unique. The key must be a qualified name
         ([A-Za-z0-9][-A-Za-z0-9_.]*) no more than 63 bytes in length.
@@ -42,15 +42,15 @@
     """
     key: 'str'
     valueExpression: 'str'
 
 
 @dataclass
 class ExpressionWarning(DictMixin):
-    """ExpressionWarning is a warning information that targets a specific expression.
+    r"""ExpressionWarning is a warning information that targets a specific expression.
 
       **parameters**
 
       * **fieldRef** ``str`` - The path to the field that refers the expression. For example, the reference
         to the expression of the first item of validations is
         "spec.validations[0].expression"
       * **warning** ``str`` - The content of type checking information in a human-readable form. Each line
@@ -59,15 +59,15 @@
     """
     fieldRef: 'str'
     warning: 'str'
 
 
 @dataclass
 class MatchCondition(DictMixin):
-    """
+    r"""
 
       **parameters**
 
       * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. Must
         evaluate to bool. CEL expressions have access to the contents of the
         AdmissionRequest and Authorizer, organized into CEL variables:
         'object' - The object from the incoming request. The value is null for DELETE
@@ -94,15 +94,15 @@
     """
     expression: 'str'
     name: 'str'
 
 
 @dataclass
 class MatchResources(DictMixin):
-    """MatchResources decides whether to run the admission control policy on an
+    r"""MatchResources decides whether to run the admission control policy on an
       object based on whether it meets the match criteria. The exclude rules take
       precedence over include rules (if a resource matches both, it is excluded)
 
       **parameters**
 
       * **excludeResourceRules** ``Optional[List[NamedRuleWithOperations]]`` - ExcludeResourceRules describes what operations on what resources/subresources
         the ValidatingAdmissionPolicy should not care about. The exclude rules take
@@ -175,15 +175,15 @@
     namespaceSelector: 'Optional[meta_v1.LabelSelector]' = None
     objectSelector: 'Optional[meta_v1.LabelSelector]' = None
     resourceRules: 'Optional[List[NamedRuleWithOperations]]' = None
 
 
 @dataclass
 class NamedRuleWithOperations(DictMixin):
-    """NamedRuleWithOperations is a tuple of Operations and Resources with
+    r"""NamedRuleWithOperations is a tuple of Operations and Resources with
       ResourceNames.
 
       **parameters**
 
       * **apiGroups** ``Optional[List[str]]`` - APIGroups is the API groups the resources belong to. '*' is all groups. If '*'
         is present, the length of the slice must be one. Required.
       * **apiVersions** ``Optional[List[str]]`` - APIVersions is the API versions the resources belong to. '*' is all versions.
@@ -216,29 +216,29 @@
     resourceNames: 'Optional[List[str]]' = None
     resources: 'Optional[List[str]]' = None
     scope: 'Optional[str]' = None
 
 
 @dataclass
 class ParamKind(DictMixin):
-    """ParamKind is a tuple of Group Kind and Version.
+    r"""ParamKind is a tuple of Group Kind and Version.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion is the API group version the resources belong to. In format of
         "group/version". Required.
       * **kind** ``Optional[str]`` - Kind is the API kind the resources belong to. Required.
     """
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
 
 
 @dataclass
 class ParamRef(DictMixin):
-    """ParamRef describes how to locate the params to be used as input to expressions
+    r"""ParamRef describes how to locate the params to be used as input to expressions
       of rules applied by a policy binding.
 
       **parameters**
 
       * **name** ``Optional[str]`` - `name` is the name of the resource being referenced.
         `name` and `selector` are mutually exclusive properties. If one is set, the
         other must be unset.
@@ -271,27 +271,27 @@
     namespace: 'Optional[str]' = None
     parameterNotFoundAction: 'Optional[str]' = None
     selector: 'Optional[meta_v1.LabelSelector]' = None
 
 
 @dataclass
 class TypeChecking(DictMixin):
-    """TypeChecking contains results of type checking the expressions in the
+    r"""TypeChecking contains results of type checking the expressions in the
       ValidatingAdmissionPolicy
 
       **parameters**
 
       * **expressionWarnings** ``Optional[List[ExpressionWarning]]`` - The type checking warnings for each expression.
     """
     expressionWarnings: 'Optional[List[ExpressionWarning]]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicy(DictMixin):
-    """ValidatingAdmissionPolicy describes the definition of an admission validation
+    r"""ValidatingAdmissionPolicy describes the definition of an admission validation
       policy that accepts or rejects an object without changing it.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -312,15 +312,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[ValidatingAdmissionPolicySpec]' = None
     status: 'Optional[ValidatingAdmissionPolicyStatus]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyBinding(DictMixin):
-    """ValidatingAdmissionPolicyBinding binds the ValidatingAdmissionPolicy with
+    r"""ValidatingAdmissionPolicyBinding binds the ValidatingAdmissionPolicy with
       paramerized resources. ValidatingAdmissionPolicyBinding and parameter CRDs
       together define how cluster administrators configure policies for clusters.
       
       For a given admission request, each binding will cause its policy to be
       evaluated N times, where N is 1 for policies/bindings that don't use params,
       otherwise N is the number of parameters selected by the binding.
       
@@ -348,15 +348,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[ValidatingAdmissionPolicyBindingSpec]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyBindingList(DictMixin):
-    """ValidatingAdmissionPolicyBindingList is a list of
+    r"""ValidatingAdmissionPolicyBindingList is a list of
       ValidatingAdmissionPolicyBinding.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -373,15 +373,15 @@
     items: 'Optional[List[ValidatingAdmissionPolicyBinding]]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyBindingSpec(DictMixin):
-    """ValidatingAdmissionPolicyBindingSpec is the specification of the
+    r"""ValidatingAdmissionPolicyBindingSpec is the specification of the
       ValidatingAdmissionPolicyBinding.
 
       **parameters**
 
       * **matchResources** ``Optional[MatchResources]`` - MatchResources declares what resources match this binding and will be
         validated by it. Note that this is intersected with the policy's
         matchConstraints, so only requests that are matched by the policy can be
@@ -439,15 +439,15 @@
     paramRef: 'Optional[ParamRef]' = None
     policyName: 'Optional[str]' = None
     validationActions: 'Optional[List[str]]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyList(DictMixin):
-    """ValidatingAdmissionPolicyList is a list of ValidatingAdmissionPolicy.
+    r"""ValidatingAdmissionPolicyList is a list of ValidatingAdmissionPolicy.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -463,15 +463,15 @@
     items: 'Optional[List[ValidatingAdmissionPolicy]]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicySpec(DictMixin):
-    """ValidatingAdmissionPolicySpec is the specification of the desired behavior of
+    r"""ValidatingAdmissionPolicySpec is the specification of the desired behavior of
       the AdmissionPolicy.
 
       **parameters**
 
       * **auditAnnotations** ``Optional[List[AuditAnnotation]]`` - auditAnnotations contains CEL expressions which are used to produce audit
         annotations for the audit event of the API request. validations and
         auditAnnotations may not both be empty; a least one of validations or
@@ -530,15 +530,15 @@
     paramKind: 'Optional[ParamKind]' = None
     validations: 'Optional[List[Validation]]' = None
     variables: 'Optional[List[Variable]]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyStatus(DictMixin):
-    """ValidatingAdmissionPolicyStatus represents the status of a
+    r"""ValidatingAdmissionPolicyStatus represents the status of a
       ValidatingAdmissionPolicy.
 
       **parameters**
 
       * **conditions** ``Optional[List[meta_v1.Condition]]`` - The conditions represent the latest available observations of a policy's
         current state.
       * **observedGeneration** ``Optional[int]`` - The generation observed by the controller.
@@ -548,15 +548,15 @@
     conditions: 'Optional[List[meta_v1.Condition]]' = None
     observedGeneration: 'Optional[int]' = None
     typeChecking: 'Optional[TypeChecking]' = None
 
 
 @dataclass
 class Validation(DictMixin):
-    """Validation specifies the CEL expression which is used to apply the validation.
+    r"""Validation specifies the CEL expression which is used to apply the validation.
 
       **parameters**
 
       * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. ref:
         https://github.com/google/cel-spec CEL expressions have access to the contents
         of the API request/response, organized into CEL variables as well as some
         other useful variables:
@@ -639,15 +639,15 @@
     message: 'Optional[str]' = None
     messageExpression: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class Variable(DictMixin):
-    """Variable is the definition of a variable that is used for composition.
+    r"""Variable is the definition of a variable that is used for composition.
 
       **parameters**
 
       * **expression** ``str`` - Expression is the expression that will be evaluated as the value of the
         variable. The CEL expression has access to the same identifiers as the CEL
         expressions in Validation.
       * **name** ``str`` - Name is the name of the variable. The name must be a valid CEL identifier and
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/admissionregistration_v1beta1.py` & `lightkube-models-1.30.0.8/lightkube/models/admissionregistration_v1beta1.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class AuditAnnotation(DictMixin):
-    """AuditAnnotation describes how to produce an audit annotation for an API
+    r"""AuditAnnotation describes how to produce an audit annotation for an API
       request.
 
       **parameters**
 
       * **key** ``str`` - key specifies the audit annotation key. The audit annotation keys of a
         ValidatingAdmissionPolicy must be unique. The key must be a qualified name
         ([A-Za-z0-9][-A-Za-z0-9_.]*) no more than 63 bytes in length.
@@ -42,15 +42,15 @@
     """
     key: 'str'
     valueExpression: 'str'
 
 
 @dataclass
 class ExpressionWarning(DictMixin):
-    """ExpressionWarning is a warning information that targets a specific expression.
+    r"""ExpressionWarning is a warning information that targets a specific expression.
 
       **parameters**
 
       * **fieldRef** ``str`` - The path to the field that refers the expression. For example, the reference
         to the expression of the first item of validations is
         "spec.validations[0].expression"
       * **warning** ``str`` - The content of type checking information in a human-readable form. Each line
@@ -59,15 +59,15 @@
     """
     fieldRef: 'str'
     warning: 'str'
 
 
 @dataclass
 class MatchCondition(DictMixin):
-    """MatchCondition represents a condition which must be fulfilled for a request to
+    r"""MatchCondition represents a condition which must be fulfilled for a request to
       be sent to a webhook.
 
       **parameters**
 
       * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. Must
         evaluate to bool. CEL expressions have access to the contents of the
         AdmissionRequest and Authorizer, organized into CEL variables:
@@ -95,15 +95,15 @@
     """
     expression: 'str'
     name: 'str'
 
 
 @dataclass
 class MatchResources(DictMixin):
-    """MatchResources decides whether to run the admission control policy on an
+    r"""MatchResources decides whether to run the admission control policy on an
       object based on whether it meets the match criteria. The exclude rules take
       precedence over include rules (if a resource matches both, it is excluded)
 
       **parameters**
 
       * **excludeResourceRules** ``Optional[List[NamedRuleWithOperations]]`` - ExcludeResourceRules describes what operations on what resources/subresources
         the ValidatingAdmissionPolicy should not care about. The exclude rules take
@@ -176,15 +176,15 @@
     namespaceSelector: 'Optional[meta_v1.LabelSelector]' = None
     objectSelector: 'Optional[meta_v1.LabelSelector]' = None
     resourceRules: 'Optional[List[NamedRuleWithOperations]]' = None
 
 
 @dataclass
 class NamedRuleWithOperations(DictMixin):
-    """NamedRuleWithOperations is a tuple of Operations and Resources with
+    r"""NamedRuleWithOperations is a tuple of Operations and Resources with
       ResourceNames.
 
       **parameters**
 
       * **apiGroups** ``Optional[List[str]]`` - APIGroups is the API groups the resources belong to. '*' is all groups. If '*'
         is present, the length of the slice must be one. Required.
       * **apiVersions** ``Optional[List[str]]`` - APIVersions is the API versions the resources belong to. '*' is all versions.
@@ -217,29 +217,29 @@
     resourceNames: 'Optional[List[str]]' = None
     resources: 'Optional[List[str]]' = None
     scope: 'Optional[str]' = None
 
 
 @dataclass
 class ParamKind(DictMixin):
-    """ParamKind is a tuple of Group Kind and Version.
+    r"""ParamKind is a tuple of Group Kind and Version.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion is the API group version the resources belong to. In format of
         "group/version". Required.
       * **kind** ``Optional[str]`` - Kind is the API kind the resources belong to. Required.
     """
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
 
 
 @dataclass
 class ParamRef(DictMixin):
-    """ParamRef describes how to locate the params to be used as input to expressions
+    r"""ParamRef describes how to locate the params to be used as input to expressions
       of rules applied by a policy binding.
 
       **parameters**
 
       * **name** ``Optional[str]`` - name is the name of the resource being referenced.
         One of `name` or `selector` must be set, but `name` and `selector` are
         mutually exclusive properties. If one is set, the other must be unset.
@@ -276,27 +276,27 @@
     namespace: 'Optional[str]' = None
     parameterNotFoundAction: 'Optional[str]' = None
     selector: 'Optional[meta_v1.LabelSelector]' = None
 
 
 @dataclass
 class TypeChecking(DictMixin):
-    """TypeChecking contains results of type checking the expressions in the
+    r"""TypeChecking contains results of type checking the expressions in the
       ValidatingAdmissionPolicy
 
       **parameters**
 
       * **expressionWarnings** ``Optional[List[ExpressionWarning]]`` - The type checking warnings for each expression.
     """
     expressionWarnings: 'Optional[List[ExpressionWarning]]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicy(DictMixin):
-    """ValidatingAdmissionPolicy describes the definition of an admission validation
+    r"""ValidatingAdmissionPolicy describes the definition of an admission validation
       policy that accepts or rejects an object without changing it.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -317,15 +317,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[ValidatingAdmissionPolicySpec]' = None
     status: 'Optional[ValidatingAdmissionPolicyStatus]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyBinding(DictMixin):
-    """ValidatingAdmissionPolicyBinding binds the ValidatingAdmissionPolicy with
+    r"""ValidatingAdmissionPolicyBinding binds the ValidatingAdmissionPolicy with
       paramerized resources. ValidatingAdmissionPolicyBinding and parameter CRDs
       together define how cluster administrators configure policies for clusters.
       
       For a given admission request, each binding will cause its policy to be
       evaluated N times, where N is 1 for policies/bindings that don't use params,
       otherwise N is the number of parameters selected by the binding.
       
@@ -353,15 +353,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[ValidatingAdmissionPolicyBindingSpec]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyBindingList(DictMixin):
-    """ValidatingAdmissionPolicyBindingList is a list of
+    r"""ValidatingAdmissionPolicyBindingList is a list of
       ValidatingAdmissionPolicyBinding.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -378,15 +378,15 @@
     items: 'Optional[List[ValidatingAdmissionPolicyBinding]]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyBindingSpec(DictMixin):
-    """ValidatingAdmissionPolicyBindingSpec is the specification of the
+    r"""ValidatingAdmissionPolicyBindingSpec is the specification of the
       ValidatingAdmissionPolicyBinding.
 
       **parameters**
 
       * **matchResources** ``Optional[MatchResources]`` - MatchResources declares what resources match this binding and will be
         validated by it. Note that this is intersected with the policy's
         matchConstraints, so only requests that are matched by the policy can be
@@ -444,15 +444,15 @@
     paramRef: 'Optional[ParamRef]' = None
     policyName: 'Optional[str]' = None
     validationActions: 'Optional[List[str]]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyList(DictMixin):
-    """ValidatingAdmissionPolicyList is a list of ValidatingAdmissionPolicy.
+    r"""ValidatingAdmissionPolicyList is a list of ValidatingAdmissionPolicy.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -468,15 +468,15 @@
     items: 'Optional[List[ValidatingAdmissionPolicy]]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicySpec(DictMixin):
-    """ValidatingAdmissionPolicySpec is the specification of the desired behavior of
+    r"""ValidatingAdmissionPolicySpec is the specification of the desired behavior of
       the AdmissionPolicy.
 
       **parameters**
 
       * **auditAnnotations** ``Optional[List[AuditAnnotation]]`` - auditAnnotations contains CEL expressions which are used to produce audit
         annotations for the audit event of the API request. validations and
         auditAnnotations may not both be empty; a least one of validations or
@@ -535,15 +535,15 @@
     paramKind: 'Optional[ParamKind]' = None
     validations: 'Optional[List[Validation]]' = None
     variables: 'Optional[List[Variable]]' = None
 
 
 @dataclass
 class ValidatingAdmissionPolicyStatus(DictMixin):
-    """ValidatingAdmissionPolicyStatus represents the status of an admission
+    r"""ValidatingAdmissionPolicyStatus represents the status of an admission
       validation policy.
 
       **parameters**
 
       * **conditions** ``Optional[List[meta_v1.Condition]]`` - The conditions represent the latest available observations of a policy's
         current state.
       * **observedGeneration** ``Optional[int]`` - The generation observed by the controller.
@@ -553,15 +553,15 @@
     conditions: 'Optional[List[meta_v1.Condition]]' = None
     observedGeneration: 'Optional[int]' = None
     typeChecking: 'Optional[TypeChecking]' = None
 
 
 @dataclass
 class Validation(DictMixin):
-    """Validation specifies the CEL expression which is used to apply the validation.
+    r"""Validation specifies the CEL expression which is used to apply the validation.
 
       **parameters**
 
       * **expression** ``str`` - Expression represents the expression which will be evaluated by CEL. ref:
         https://github.com/google/cel-spec CEL expressions have access to the contents
         of the API request/response, organized into CEL variables as well as some
         other useful variables:
@@ -644,15 +644,15 @@
     message: 'Optional[str]' = None
     messageExpression: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class Variable(DictMixin):
-    """Variable is the definition of a variable that is used for composition. A
+    r"""Variable is the definition of a variable that is used for composition. A
       variable is defined as a named expression.
 
       **parameters**
 
       * **expression** ``str`` - Expression is the expression that will be evaluated as the value of the
         variable. The CEL expression has access to the same identifiers as the CEL
         expressions in Validation.
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/apiextensions_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/apiextensions_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from typing import Any
-from typing import Dict
 from . import meta_v1
+from typing import Dict
+from typing import Any
 
 
 @dataclass
 class CustomResourceColumnDefinition(DictMixin):
-    """CustomResourceColumnDefinition specifies a column for server side printing.
+    r"""CustomResourceColumnDefinition specifies a column for server side printing.
 
       **parameters**
 
       * **jsonPath** ``str`` - jsonPath is a simple JSON path (i.e. with array notation) which is evaluated
         against each custom resource to produce the value for this column.
       * **name** ``str`` - name is a human readable name for the column.
       * **type** ``str`` - type is an OpenAPI type definition for this column. See
@@ -40,15 +40,15 @@
     description: 'Optional[str]' = None
     format: 'Optional[str]' = None
     priority: 'Optional[int]' = None
 
 
 @dataclass
 class CustomResourceConversion(DictMixin):
-    """CustomResourceConversion describes how to convert different versions of a CR.
+    r"""CustomResourceConversion describes how to convert different versions of a CR.
 
       **parameters**
 
       * **strategy** ``str`` - strategy specifies how custom resources are converted between versions.
         Allowed values are: - `"None"`: The converter only change the apiVersion and
         would not touch any other field in the custom resource. - `"Webhook"`: API
         Server will call to an external webhook to do the conversion. Additional
@@ -60,15 +60,15 @@
     """
     strategy: 'str'
     webhook: 'Optional[WebhookConversion]' = None
 
 
 @dataclass
 class CustomResourceDefinition(DictMixin):
-    """CustomResourceDefinition represents a resource that should be exposed on the
+    r"""CustomResourceDefinition represents a resource that should be exposed on the
       API server.  Its name MUST be in the format <.spec.name>.<.spec.group>.
 
       **parameters**
 
       * **spec** ``CustomResourceDefinitionSpec`` - spec describes how the user wants the resources to appear
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -87,15 +87,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[CustomResourceDefinitionStatus]' = None
 
 
 @dataclass
 class CustomResourceDefinitionCondition(DictMixin):
-    """CustomResourceDefinitionCondition contains details for the current condition
+    r"""CustomResourceDefinitionCondition contains details for the current condition
       of this pod.
 
       **parameters**
 
       * **status** ``str`` - status is the status of the condition. Can be True, False, Unknown.
       * **type** ``str`` - type is the type of the condition. Types include Established, NamesAccepted
         and Terminating.
@@ -110,15 +110,15 @@
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class CustomResourceDefinitionList(DictMixin):
-    """CustomResourceDefinitionList is a list of CustomResourceDefinition objects.
+    r"""CustomResourceDefinitionList is a list of CustomResourceDefinition objects.
 
       **parameters**
 
       * **items** ``List[CustomResourceDefinition]`` - items list individual CustomResourceDefinition objects
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -134,15 +134,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class CustomResourceDefinitionNames(DictMixin):
-    """CustomResourceDefinitionNames indicates the names to serve this
+    r"""CustomResourceDefinitionNames indicates the names to serve this
       CustomResourceDefinition
 
       **parameters**
 
       * **kind** ``str`` - kind is the serialized kind of the resource. It is normally CamelCase and
         singular. Custom resource instances will use this value as the `kind`
         attribute in API calls.
@@ -167,15 +167,15 @@
     listKind: 'Optional[str]' = None
     shortNames: 'Optional[List[str]]' = None
     singular: 'Optional[str]' = None
 
 
 @dataclass
 class CustomResourceDefinitionSpec(DictMixin):
-    """CustomResourceDefinitionSpec describes how a user wants their resource to
+    r"""CustomResourceDefinitionSpec describes how a user wants their resource to
       appear
 
       **parameters**
 
       * **group** ``str`` - group is the API group of the defined custom resource. The custom resources
         are served under `/apis/<group>/...`. Must match the name of the
         CustomResourceDefinition (in the form `<names.plural>.<group>`).
@@ -207,15 +207,15 @@
     versions: 'List[CustomResourceDefinitionVersion]'
     conversion: 'Optional[CustomResourceConversion]' = None
     preserveUnknownFields: 'Optional[bool]' = None
 
 
 @dataclass
 class CustomResourceDefinitionStatus(DictMixin):
-    """CustomResourceDefinitionStatus indicates the state of the
+    r"""CustomResourceDefinitionStatus indicates the state of the
       CustomResourceDefinition
 
       **parameters**
 
       * **acceptedNames** ``Optional[CustomResourceDefinitionNames]`` - acceptedNames are the names that are actually being used to serve discovery.
         They may be different than the names in spec.
       * **conditions** ``Optional[List[CustomResourceDefinitionCondition]]`` - conditions indicate state for particular aspects of a CustomResourceDefinition
@@ -229,15 +229,15 @@
     acceptedNames: 'Optional[CustomResourceDefinitionNames]' = None
     conditions: 'Optional[List[CustomResourceDefinitionCondition]]' = None
     storedVersions: 'Optional[List[str]]' = None
 
 
 @dataclass
 class CustomResourceDefinitionVersion(DictMixin):
-    """CustomResourceDefinitionVersion describes a version for CRD.
+    r"""CustomResourceDefinitionVersion describes a version for CRD.
 
       **parameters**
 
       * **name** ``str`` - name is the version name, e.g. “v1”, “v2beta1”, etc. The custom resources are
         served under this version at `/apis/<group>/<version>/...` if `served` is
         true.
       * **served** ``bool`` - served is a flag enabling/disabling this version from being served via REST
@@ -273,15 +273,15 @@
     schema: 'Optional[CustomResourceValidation]' = None
     selectableFields: 'Optional[List[SelectableField]]' = None
     subresources: 'Optional[CustomResourceSubresources]' = None
 
 
 @dataclass
 class CustomResourceSubresourceScale(DictMixin):
-    """CustomResourceSubresourceScale defines how to serve the scale subresource for
+    r"""CustomResourceSubresourceScale defines how to serve the scale subresource for
       CustomResources.
 
       **parameters**
 
       * **specReplicasPath** ``str`` - specReplicasPath defines the JSON path inside of a custom resource that
         corresponds to Scale `spec.replicas`. Only JSON paths without the array
         notation are allowed. Must be a JSON Path under `.spec`. If there is no value
@@ -309,15 +309,15 @@
 
 
 CustomResourceSubresourceStatus = Dict
 
 
 @dataclass
 class CustomResourceSubresources(DictMixin):
-    """CustomResourceSubresources defines the status and scale subresources for
+    r"""CustomResourceSubresources defines the status and scale subresources for
       CustomResources.
 
       **parameters**
 
       * **scale** ``Optional[CustomResourceSubresourceScale]`` - scale indicates the custom resource should serve a `/scale` subresource that
         returns an `autoscaling/v1` Scale object.
       * **status** ``Optional[CustomResourceSubresourceStatus]`` - status indicates the custom resource should serve a `/status` subresource.
@@ -328,26 +328,26 @@
     """
     scale: 'Optional[CustomResourceSubresourceScale]' = None
     status: 'Optional[CustomResourceSubresourceStatus]' = None
 
 
 @dataclass
 class CustomResourceValidation(DictMixin):
-    """CustomResourceValidation is a list of validation methods for CustomResources.
+    r"""CustomResourceValidation is a list of validation methods for CustomResources.
 
       **parameters**
 
       * **openAPIV3Schema** ``Optional[JSONSchemaProps]`` - openAPIV3Schema is the OpenAPI v3 schema to use for validation and pruning.
     """
     openAPIV3Schema: 'Optional[JSONSchemaProps]' = None
 
 
 @dataclass
 class ExternalDocumentation(DictMixin):
-    """ExternalDocumentation allows referencing an external resource for extended
+    r"""ExternalDocumentation allows referencing an external resource for extended
       documentation.
 
       **parameters**
 
       * **description** ``Optional[str]`` - 
       * **url** ``Optional[str]`` - 
     """
@@ -356,15 +356,15 @@
 
 
 JSON = Any
 
 
 @dataclass
 class JSONSchemaProps(DictMixin):
-    """JSONSchemaProps is a JSON-Schema following Specification Draft 4
+    r"""JSONSchemaProps is a JSON-Schema following Specification Draft 4
       (http://json-schema.org/).
 
       **parameters**
 
       * **d_ref** ``Optional[str]`` - 
       * **d_schema** ``Optional[str]`` - 
       * **additionalItems** ``Optional[JSONSchemaPropsOrBool]`` - 
@@ -548,15 +548,15 @@
 
 
 JSONSchemaPropsOrStringArray = Any
 
 
 @dataclass
 class SelectableField(DictMixin):
-    """SelectableField specifies the JSON path of a field that may be used with field
+    r"""SelectableField specifies the JSON path of a field that may be used with field
       selectors.
 
       **parameters**
 
       * **jsonPath** ``str`` - jsonPath is a simple JSON path which is evaluated against each custom resource
         to produce a field selector value. Only JSON paths without the array notation
         are allowed. Must point to a field of type string, boolean or integer. Types
@@ -565,15 +565,15 @@
         not point to metdata fields. Required.
     """
     jsonPath: 'str'
 
 
 @dataclass
 class ServiceReference(DictMixin):
-    """ServiceReference holds a reference to Service.legacy.k8s.io
+    r"""ServiceReference holds a reference to Service.legacy.k8s.io
 
       **parameters**
 
       * **name** ``str`` - name is the name of the service. Required
       * **namespace** ``str`` - namespace is the namespace of the service. Required
       * **path** ``Optional[str]`` - path is an optional URL path at which the webhook will be contacted.
       * **port** ``Optional[int]`` - port is an optional service port at which the webhook will be contacted.
@@ -584,15 +584,15 @@
     namespace: 'str'
     path: 'Optional[str]' = None
     port: 'Optional[int]' = None
 
 
 @dataclass
 class ValidationRule(DictMixin):
-    """ValidationRule describes a validation rule written in the CEL expression
+    r"""ValidationRule describes a validation rule written in the CEL expression
       language.
 
       **parameters**
 
       * **rule** ``str`` - Rule represents the expression which will be evaluated by CEL. ref:
         https://github.com/google/cel-spec The Rule is scoped to the location of the
         x-kubernetes-validations extension in the schema. The `self` variable in the
@@ -719,15 +719,15 @@
     messageExpression: 'Optional[str]' = None
     optionalOldSelf: 'Optional[bool]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class WebhookClientConfig(DictMixin):
-    """WebhookClientConfig contains the information to make a TLS connection with the
+    r"""WebhookClientConfig contains the information to make a TLS connection with the
       webhook.
 
       **parameters**
 
       * **caBundle** ``Optional[str]`` - caBundle is a PEM encoded CA bundle which will be used to validate the
         webhook's server certificate. If unspecified, system trust roots on the
         apiserver are used.
@@ -755,15 +755,15 @@
     caBundle: 'Optional[str]' = None
     service: 'Optional[ServiceReference]' = None
     url: 'Optional[str]' = None
 
 
 @dataclass
 class WebhookConversion(DictMixin):
-    """WebhookConversion describes how to call a conversion webhook
+    r"""WebhookConversion describes how to call a conversion webhook
 
       **parameters**
 
       * **conversionReviewVersions** ``List[str]`` - conversionReviewVersions is an ordered list of preferred `ConversionReview`
         versions the Webhook expects. The API server will use the first version in the
         list which it supports. If none of the versions specified in this list are
         supported by API server, conversion will fail for the custom resource. If a
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/apiregistration_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/apiregistration_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class APIService(DictMixin):
-    """APIService represents a server for a particular GroupVersion. Name must be
+    r"""APIService represents a server for a particular GroupVersion. Name must be
       "version.group".
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -34,15 +34,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[APIServiceSpec]' = None
     status: 'Optional[APIServiceStatus]' = None
 
 
 @dataclass
 class APIServiceCondition(DictMixin):
-    """APIServiceCondition describes the state of an APIService at a particular point
+    r"""APIServiceCondition describes the state of an APIService at a particular point
 
       **parameters**
 
       * **status** ``str`` - Status is the status of the condition. Can be True, False, Unknown.
       * **type** ``str`` - Type is the type of the condition.
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - Last time the condition transitioned from one status to another.
       * **message** ``Optional[str]`` - Human-readable message indicating details about last transition.
@@ -53,15 +53,15 @@
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class APIServiceList(DictMixin):
-    """APIServiceList is a list of APIService objects.
+    r"""APIServiceList is a list of APIService objects.
 
       **parameters**
 
       * **items** ``List[APIService]`` - Items is the list of APIService
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -77,15 +77,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class APIServiceSpec(DictMixin):
-    """APIServiceSpec contains information for locating and communicating with a
+    r"""APIServiceSpec contains information for locating and communicating with a
       server. Only https is supported, though you are able to disable certificate
       verification.
 
       **parameters**
 
       * **groupPriorityMinimum** ``int`` - GroupPriorityMinimum is the priority this group should have at least. Higher
         priority means that the group is preferred by clients over lower priority
@@ -129,26 +129,26 @@
     insecureSkipTLSVerify: 'Optional[bool]' = None
     service: 'Optional[ServiceReference]' = None
     version: 'Optional[str]' = None
 
 
 @dataclass
 class APIServiceStatus(DictMixin):
-    """APIServiceStatus contains derived information about an API server
+    r"""APIServiceStatus contains derived information about an API server
 
       **parameters**
 
       * **conditions** ``Optional[List[APIServiceCondition]]`` - Current service state of apiService.
     """
     conditions: 'Optional[List[APIServiceCondition]]' = None
 
 
 @dataclass
 class ServiceReference(DictMixin):
-    """ServiceReference holds a reference to Service.legacy.k8s.io
+    r"""ServiceReference holds a reference to Service.legacy.k8s.io
 
       **parameters**
 
       * **name** ``Optional[str]`` - Name is the name of the service
       * **namespace** ``Optional[str]`` - Namespace is the namespace of the service
       * **port** ``Optional[int]`` - If specified, the port on the service that hosting webhook. Default to 443 for
         backward compatibility. `port` should be a valid port number (1-65535,
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/apiserverinternal_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/models/apiserverinternal_v1alpha1.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from typing import Dict
 from . import meta_v1
+from typing import Dict
 
 
 @dataclass
 class ServerStorageVersion(DictMixin):
-    """An API server instance reports the version it can decode and the version it
+    r"""An API server instance reports the version it can decode and the version it
       encodes objects to when persisting objects in the backend.
 
       **parameters**
 
       * **apiServerID** ``Optional[str]`` - The ID of the reporting API server.
       * **decodableVersions** ``Optional[List[str]]`` - The API server can decode objects encoded in these versions. The
         encodingVersion must be included in the decodableVersions.
@@ -29,15 +29,15 @@
     decodableVersions: 'Optional[List[str]]' = None
     encodingVersion: 'Optional[str]' = None
     servedVersions: 'Optional[List[str]]' = None
 
 
 @dataclass
 class StorageVersion(DictMixin):
-    """Storage version of a specific resource.
+    r"""Storage version of a specific resource.
 
       **parameters**
 
       * **spec** ``StorageVersionSpec`` - Spec is an empty spec. It is here to comply with Kubernetes API style.
       * **status** ``StorageVersionStatus`` - API server instances report the version they can decode and the version they
         encode objects to when persisting objects in the backend.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
@@ -55,15 +55,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
 class StorageVersionCondition(DictMixin):
-    """Describes the state of the storageVersion at a certain point.
+    r"""Describes the state of the storageVersion at a certain point.
 
       **parameters**
 
       * **message** ``str`` - A human readable message indicating details about the transition.
       * **reason** ``str`` - The reason for the condition's last transition.
       * **status** ``str`` - Status of the condition, one of True, False, Unknown.
       * **type** ``str`` - Type of the condition.
@@ -77,15 +77,15 @@
     type: 'str'
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     observedGeneration: 'Optional[int]' = None
 
 
 @dataclass
 class StorageVersionList(DictMixin):
-    """A list of StorageVersions.
+    r"""A list of StorageVersions.
 
       **parameters**
 
       * **items** ``List[StorageVersion]`` - Items holds a list of StorageVersion
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -104,15 +104,15 @@
 
 
 StorageVersionSpec = Dict
 
 
 @dataclass
 class StorageVersionStatus(DictMixin):
-    """API server instances report the versions they can decode and the version they
+    r"""API server instances report the versions they can decode and the version they
       encode objects to when persisting objects in the backend.
 
       **parameters**
 
       * **commonEncodingVersion** ``Optional[str]`` - If all API server instances agree on the same encoding storage version, then
         this field is set to that version. Otherwise this field is left empty. API
         servers should finish updating its storageVersionStatus entry before serving
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/apps_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/apps_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from . import core_v1
 from . import runtime
 from . import util_intstr
+from . import core_v1
 from . import meta_v1
 
 
 @dataclass
 class ControllerRevision(DictMixin):
-    """ControllerRevision implements an immutable snapshot of state data. Clients are
+    r"""ControllerRevision implements an immutable snapshot of state data. Clients are
       responsible for serializing and deserializing the objects that contain their
       internal state. Once a ControllerRevision has been successfully created, it
       can not be updated. The API Server will fail validation of all requests that
       attempt to mutate the Data field. ControllerRevisions may, however, be
       deleted. Note that, due to its use by both the DaemonSet and StatefulSet
       controllers for update and rollback, this object is beta. However, it may be
       subject to name and representation changes in future releases, and clients
@@ -45,15 +45,15 @@
     data: 'Optional[runtime.RawExtension]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
 class ControllerRevisionList(DictMixin):
-    """ControllerRevisionList is a resource containing a list of ControllerRevision
+    r"""ControllerRevisionList is a resource containing a list of ControllerRevision
       objects.
 
       **parameters**
 
       * **items** ``List[ControllerRevision]`` - Items is the list of ControllerRevisions
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -70,15 +70,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class DaemonSet(DictMixin):
-    """DaemonSet represents the configuration of a daemon set.
+    r"""DaemonSet represents the configuration of a daemon set.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -99,15 +99,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[DaemonSetSpec]' = None
     status: 'Optional[DaemonSetStatus]' = None
 
 
 @dataclass
 class DaemonSetCondition(DictMixin):
-    """DaemonSetCondition describes the state of a DaemonSet at a certain point.
+    r"""DaemonSetCondition describes the state of a DaemonSet at a certain point.
 
       **parameters**
 
       * **status** ``str`` - Status of the condition, one of True, False, Unknown.
       * **type** ``str`` - Type of DaemonSet condition.
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - Last time the condition transitioned from one status to another.
       * **message** ``Optional[str]`` - A human readable message indicating details about the transition.
@@ -118,15 +118,15 @@
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class DaemonSetList(DictMixin):
-    """DaemonSetList is a collection of daemon sets.
+    r"""DaemonSetList is a collection of daemon sets.
 
       **parameters**
 
       * **items** ``List[DaemonSet]`` - A list of daemon sets.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -142,15 +142,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class DaemonSetSpec(DictMixin):
-    """DaemonSetSpec is the specification of a daemon set.
+    r"""DaemonSetSpec is the specification of a daemon set.
 
       **parameters**
 
       * **selector** ``meta_v1.LabelSelector`` - A label query over pods that are managed by the daemon set. Must match in
         order to be controlled. It must match the pod template's labels. More info:
         https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#label-selectors
       * **template** ``core_v1.PodTemplateSpec`` - An object that describes the pod that will be created. The DaemonSet will
@@ -171,15 +171,15 @@
     minReadySeconds: 'Optional[int]' = None
     revisionHistoryLimit: 'Optional[int]' = None
     updateStrategy: 'Optional[DaemonSetUpdateStrategy]' = None
 
 
 @dataclass
 class DaemonSetStatus(DictMixin):
-    """DaemonSetStatus represents the current status of a daemon set.
+    r"""DaemonSetStatus represents the current status of a daemon set.
 
       **parameters**
 
       * **currentNumberScheduled** ``int`` - The number of nodes that are running at least 1 daemon pod and are supposed to
         run the daemon pod. More info:
         https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/
       * **desiredNumberScheduled** ``int`` - The total number of nodes that should be running the daemon pod (including
@@ -212,30 +212,30 @@
     numberUnavailable: 'Optional[int]' = None
     observedGeneration: 'Optional[int]' = None
     updatedNumberScheduled: 'Optional[int]' = None
 
 
 @dataclass
 class DaemonSetUpdateStrategy(DictMixin):
-    """DaemonSetUpdateStrategy is a struct used to control the update strategy for a
+    r"""DaemonSetUpdateStrategy is a struct used to control the update strategy for a
       DaemonSet.
 
       **parameters**
 
       * **rollingUpdate** ``Optional[RollingUpdateDaemonSet]`` - Rolling update config params. Present only if type = "RollingUpdate".
       * **type** ``Optional[str]`` - Type of daemon set update. Can be "RollingUpdate" or "OnDelete". Default is
         RollingUpdate.
     """
     rollingUpdate: 'Optional[RollingUpdateDaemonSet]' = None
     type: 'Optional[str]' = None
 
 
 @dataclass
 class Deployment(DictMixin):
-    """Deployment enables declarative updates for Pods and ReplicaSets.
+    r"""Deployment enables declarative updates for Pods and ReplicaSets.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -253,15 +253,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[DeploymentSpec]' = None
     status: 'Optional[DeploymentStatus]' = None
 
 
 @dataclass
 class DeploymentCondition(DictMixin):
-    """DeploymentCondition describes the state of a deployment at a certain point.
+    r"""DeploymentCondition describes the state of a deployment at a certain point.
 
       **parameters**
 
       * **status** ``str`` - Status of the condition, one of True, False, Unknown.
       * **type** ``str`` - Type of deployment condition.
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - Last time the condition transitioned from one status to another.
       * **lastUpdateTime** ``Optional[meta_v1.Time]`` - The last time this condition was updated.
@@ -274,15 +274,15 @@
     lastUpdateTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class DeploymentList(DictMixin):
-    """DeploymentList is a list of Deployments.
+    r"""DeploymentList is a list of Deployments.
 
       **parameters**
 
       * **items** ``List[Deployment]`` - Items is the list of Deployments.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -297,15 +297,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class DeploymentSpec(DictMixin):
-    """DeploymentSpec is the specification of the desired behavior of the Deployment.
+    r"""DeploymentSpec is the specification of the desired behavior of the Deployment.
 
       **parameters**
 
       * **selector** ``meta_v1.LabelSelector`` - Label selector for pods. Existing ReplicaSets whose pods are selected by this
         will be the ones affected by this deployment. It must match the pod template's
         labels.
       * **template** ``core_v1.PodTemplateSpec`` - Template describes the pods that will be created. The only allowed
@@ -333,15 +333,15 @@
     replicas: 'Optional[int]' = None
     revisionHistoryLimit: 'Optional[int]' = None
     strategy: 'Optional[DeploymentStrategy]' = None
 
 
 @dataclass
 class DeploymentStatus(DictMixin):
-    """DeploymentStatus is the most recently observed status of the Deployment.
+    r"""DeploymentStatus is the most recently observed status of the Deployment.
 
       **parameters**
 
       * **availableReplicas** ``Optional[int]`` - Total number of available pods (ready for at least minReadySeconds) targeted
         by this deployment.
       * **collisionCount** ``Optional[int]`` - Count of hash collisions for the Deployment. The Deployment controller uses
         this field as a collision avoidance mechanism when it needs to create the name
@@ -367,30 +367,30 @@
     replicas: 'Optional[int]' = None
     unavailableReplicas: 'Optional[int]' = None
     updatedReplicas: 'Optional[int]' = None
 
 
 @dataclass
 class DeploymentStrategy(DictMixin):
-    """DeploymentStrategy describes how to replace existing pods with new ones.
+    r"""DeploymentStrategy describes how to replace existing pods with new ones.
 
       **parameters**
 
       * **rollingUpdate** ``Optional[RollingUpdateDeployment]`` - Rolling update config params. Present only if DeploymentStrategyType =
         RollingUpdate.
       * **type** ``Optional[str]`` - Type of deployment. Can be "Recreate" or "RollingUpdate". Default is
         RollingUpdate.
     """
     rollingUpdate: 'Optional[RollingUpdateDeployment]' = None
     type: 'Optional[str]' = None
 
 
 @dataclass
 class ReplicaSet(DictMixin):
-    """ReplicaSet ensures that a specified number of pod replicas are running at any
+    r"""ReplicaSet ensures that a specified number of pod replicas are running at any
       given time.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -415,15 +415,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[ReplicaSetSpec]' = None
     status: 'Optional[ReplicaSetStatus]' = None
 
 
 @dataclass
 class ReplicaSetCondition(DictMixin):
-    """ReplicaSetCondition describes the state of a replica set at a certain point.
+    r"""ReplicaSetCondition describes the state of a replica set at a certain point.
 
       **parameters**
 
       * **status** ``str`` - Status of the condition, one of True, False, Unknown.
       * **type** ``str`` - Type of replica set condition.
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - The last time the condition transitioned from one status to another.
       * **message** ``Optional[str]`` - A human readable message indicating details about the transition.
@@ -434,15 +434,15 @@
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class ReplicaSetList(DictMixin):
-    """ReplicaSetList is a collection of ReplicaSets.
+    r"""ReplicaSetList is a collection of ReplicaSets.
 
       **parameters**
 
       * **items** ``List[ReplicaSet]`` - List of ReplicaSets. More info:
         https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -459,15 +459,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ReplicaSetSpec(DictMixin):
-    """ReplicaSetSpec is the specification of a ReplicaSet.
+    r"""ReplicaSetSpec is the specification of a ReplicaSet.
 
       **parameters**
 
       * **selector** ``meta_v1.LabelSelector`` - Selector is a label query over pods that should match the replica count. Label
         keys and values that must match in order to be controlled by this replica set.
         It must match the pod template's labels. More info:
         https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#label-selectors
@@ -485,15 +485,15 @@
     minReadySeconds: 'Optional[int]' = None
     replicas: 'Optional[int]' = None
     template: 'Optional[core_v1.PodTemplateSpec]' = None
 
 
 @dataclass
 class ReplicaSetStatus(DictMixin):
-    """ReplicaSetStatus represents the current status of a ReplicaSet.
+    r"""ReplicaSetStatus represents the current status of a ReplicaSet.
 
       **parameters**
 
       * **replicas** ``int`` - Replicas is the most recently observed number of replicas. More info:
         https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller/#what-is-a-replicationcontroller
       * **availableReplicas** ``Optional[int]`` - The number of available replicas (ready for at least minReadySeconds) for this
         replica set.
@@ -511,15 +511,15 @@
     fullyLabeledReplicas: 'Optional[int]' = None
     observedGeneration: 'Optional[int]' = None
     readyReplicas: 'Optional[int]' = None
 
 
 @dataclass
 class RollingUpdateDaemonSet(DictMixin):
-    """Spec to control the desired behavior of daemon set rolling update.
+    r"""Spec to control the desired behavior of daemon set rolling update.
 
       **parameters**
 
       * **maxSurge** ``Optional[util_intstr.IntOrString]`` - The maximum number of nodes with an existing available DaemonSet pod that can
         have an updated DaemonSet pod during during an update. Value can be an
         absolute number (ex: 5) or a percentage of desired pods (ex: 10%). This can
         not be 0 if MaxUnavailable is 0. Absolute number is calculated from percentage
@@ -550,15 +550,15 @@
     """
     maxSurge: 'Optional[util_intstr.IntOrString]' = None
     maxUnavailable: 'Optional[util_intstr.IntOrString]' = None
 
 
 @dataclass
 class RollingUpdateDeployment(DictMixin):
-    """Spec to control the desired behavior of rolling update.
+    r"""Spec to control the desired behavior of rolling update.
 
       **parameters**
 
       * **maxSurge** ``Optional[util_intstr.IntOrString]`` - The maximum number of pods that can be scheduled above the desired number of
         pods. Value can be an absolute number (ex: 5) or a percentage of desired pods
         (ex: 10%). This can not be 0 if MaxUnavailable is 0. Absolute number is
         calculated from percentage by rounding up. Defaults to 25%. Example: when this
@@ -579,15 +579,15 @@
     """
     maxSurge: 'Optional[util_intstr.IntOrString]' = None
     maxUnavailable: 'Optional[util_intstr.IntOrString]' = None
 
 
 @dataclass
 class RollingUpdateStatefulSetStrategy(DictMixin):
-    """RollingUpdateStatefulSetStrategy is used to communicate parameter for
+    r"""RollingUpdateStatefulSetStrategy is used to communicate parameter for
       RollingUpdateStatefulSetStrategyType.
 
       **parameters**
 
       * **maxUnavailable** ``Optional[util_intstr.IntOrString]`` - The maximum number of pods that can be unavailable during the update. Value
         can be an absolute number (ex: 5) or a percentage of desired pods (ex: 10%).
         Absolute number is calculated from percentage by rounding up. This can not be
@@ -603,15 +603,15 @@
     """
     maxUnavailable: 'Optional[util_intstr.IntOrString]' = None
     partition: 'Optional[int]' = None
 
 
 @dataclass
 class StatefulSet(DictMixin):
-    """StatefulSet represents a set of pods with consistent identities. Identities
+    r"""StatefulSet represents a set of pods with consistent identities. Identities
       are defined as:
         - Network: A single stable DNS and hostname.
         - Storage: As many VolumeClaims as requested.
       
       The StatefulSet guarantees that a given network identity will always map to
       the same storage identity.
 
@@ -636,15 +636,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[StatefulSetSpec]' = None
     status: 'Optional[StatefulSetStatus]' = None
 
 
 @dataclass
 class StatefulSetCondition(DictMixin):
-    """StatefulSetCondition describes the state of a statefulset at a certain point.
+    r"""StatefulSetCondition describes the state of a statefulset at a certain point.
 
       **parameters**
 
       * **status** ``str`` - Status of the condition, one of True, False, Unknown.
       * **type** ``str`` - Type of statefulset condition.
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - Last time the condition transitioned from one status to another.
       * **message** ``Optional[str]`` - A human readable message indicating details about the transition.
@@ -655,15 +655,15 @@
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class StatefulSetList(DictMixin):
-    """StatefulSetList is a collection of StatefulSets.
+    r"""StatefulSetList is a collection of StatefulSets.
 
       **parameters**
 
       * **items** ``List[StatefulSet]`` - Items is the list of stateful sets.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -679,15 +679,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class StatefulSetOrdinals(DictMixin):
-    """StatefulSetOrdinals describes the policy used for replica ordinal assignment
+    r"""StatefulSetOrdinals describes the policy used for replica ordinal assignment
       in this StatefulSet.
 
       **parameters**
 
       * **start** ``Optional[int]`` - start is the number representing the first replica's index. It may be used to
         number replicas from an alternate index (eg: 1-indexed) over the default
         0-indexed names, or to orchestrate progressive movement of replicas from one
@@ -697,15 +697,15 @@
           [0, .spec.replicas).
     """
     start: 'Optional[int]' = None
 
 
 @dataclass
 class StatefulSetPersistentVolumeClaimRetentionPolicy(DictMixin):
-    """StatefulSetPersistentVolumeClaimRetentionPolicy describes the policy used for
+    r"""StatefulSetPersistentVolumeClaimRetentionPolicy describes the policy used for
       PVCs created from the StatefulSet VolumeClaimTemplates.
 
       **parameters**
 
       * **whenDeleted** ``Optional[str]`` - WhenDeleted specifies what happens to PVCs created from StatefulSet
         VolumeClaimTemplates when the StatefulSet is deleted. The default policy of
         `Retain` causes PVCs to not be affected by StatefulSet deletion. The `Delete`
@@ -718,15 +718,15 @@
     """
     whenDeleted: 'Optional[str]' = None
     whenScaled: 'Optional[str]' = None
 
 
 @dataclass
 class StatefulSetSpec(DictMixin):
-    """A StatefulSetSpec is the specification of a StatefulSet.
+    r"""A StatefulSetSpec is the specification of a StatefulSet.
 
       **parameters**
 
       * **selector** ``meta_v1.LabelSelector`` - selector is a label query over pods that should match the replica count. It
         must match the pod template's labels. More info:
         https://kubernetes.io/docs/concepts/overview/working-with-objects/labels/#label-selectors
       * **serviceName** ``str`` - serviceName is the name of the service that governs this StatefulSet. This
@@ -791,15 +791,15 @@
     revisionHistoryLimit: 'Optional[int]' = None
     updateStrategy: 'Optional[StatefulSetUpdateStrategy]' = None
     volumeClaimTemplates: 'Optional[List[core_v1.PersistentVolumeClaim]]' = None
 
 
 @dataclass
 class StatefulSetStatus(DictMixin):
-    """StatefulSetStatus represents the current state of a StatefulSet.
+    r"""StatefulSetStatus represents the current state of a StatefulSet.
 
       **parameters**
 
       * **replicas** ``int`` - replicas is the number of Pods created by the StatefulSet controller.
       * **availableReplicas** ``Optional[int]`` - Total number of available pods (ready for at least minReadySeconds) targeted
         by this statefulset.
       * **collisionCount** ``Optional[int]`` - collisionCount is the count of hash collisions for the StatefulSet. The
@@ -830,15 +830,15 @@
     readyReplicas: 'Optional[int]' = None
     updateRevision: 'Optional[str]' = None
     updatedReplicas: 'Optional[int]' = None
 
 
 @dataclass
 class StatefulSetUpdateStrategy(DictMixin):
-    """StatefulSetUpdateStrategy indicates the strategy that the StatefulSet
+    r"""StatefulSetUpdateStrategy indicates the strategy that the StatefulSet
       controller will use to perform updates. It includes any additional parameters
       necessary to perform the update for the indicated strategy.
 
       **parameters**
 
       * **rollingUpdate** ``Optional[RollingUpdateStatefulSetStrategy]`` - RollingUpdate is used to communicate parameters when Type is
         RollingUpdateStatefulSetStrategyType.
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/authentication_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/authentication_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class BoundObjectReference(DictMixin):
-    """BoundObjectReference is a reference to an object that a token is bound to.
+    r"""BoundObjectReference is a reference to an object that a token is bound to.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - API version of the referent.
       * **kind** ``Optional[str]`` - Kind of the referent. Valid kinds are 'Pod' and 'Secret'.
       * **name** ``Optional[str]`` - Name of the referent.
       * **uid** ``Optional[str]`` - UID of the referent.
@@ -24,15 +24,15 @@
     kind: 'Optional[str]' = None
     name: 'Optional[str]' = None
     uid: 'Optional[str]' = None
 
 
 @dataclass
 class SelfSubjectReview(DictMixin):
-    """SelfSubjectReview contains the user information that the kube-apiserver has
+    r"""SelfSubjectReview contains the user information that the kube-apiserver has
       about the user making this request. When using impersonation, users will
       receive the user info of the user being impersonated.  If impersonation or
       request header authentication is used, any extra keys will have their case
       ignored and returned as lowercase.
 
       **parameters**
 
@@ -52,27 +52,27 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[SelfSubjectReviewStatus]' = None
 
 
 @dataclass
 class SelfSubjectReviewStatus(DictMixin):
-    """SelfSubjectReviewStatus is filled by the kube-apiserver and sent back to a
+    r"""SelfSubjectReviewStatus is filled by the kube-apiserver and sent back to a
       user.
 
       **parameters**
 
       * **userInfo** ``Optional[UserInfo]`` - User attributes of the user making this request.
     """
     userInfo: 'Optional[UserInfo]' = None
 
 
 @dataclass
 class TokenRequest(DictMixin):
-    """TokenRequest requests a token for a given service account.
+    r"""TokenRequest requests a token for a given service account.
 
       **parameters**
 
       * **spec** ``TokenRequestSpec`` - Spec holds information about the request being evaluated
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -91,15 +91,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[TokenRequestStatus]' = None
 
 
 @dataclass
 class TokenRequestSpec(DictMixin):
-    """TokenRequestSpec contains client provided parameters of a token request.
+    r"""TokenRequestSpec contains client provided parameters of a token request.
 
       **parameters**
 
       * **audiences** ``List[str]`` - Audiences are the intendend audiences of the token. A recipient of a token
         must identify themself with an identifier in the list of audiences of the
         token, and otherwise should reject the token. A token issued for multiple
         audiences may be used to authenticate against any of the audiences listed but
@@ -115,28 +115,28 @@
     audiences: 'List[str]'
     boundObjectRef: 'Optional[BoundObjectReference]' = None
     expirationSeconds: 'Optional[int]' = None
 
 
 @dataclass
 class TokenRequestStatus(DictMixin):
-    """TokenRequestStatus is the result of a token request.
+    r"""TokenRequestStatus is the result of a token request.
 
       **parameters**
 
       * **expirationTimestamp** ``meta_v1.Time`` - ExpirationTimestamp is the time of expiration of the returned token.
       * **token** ``str`` - Token is the opaque bearer token.
     """
     expirationTimestamp: 'meta_v1.Time'
     token: 'str'
 
 
 @dataclass
 class TokenReview(DictMixin):
-    """TokenReview attempts to authenticate a token to a known user. Note:
+    r"""TokenReview attempts to authenticate a token to a known user. Note:
       TokenReview requests may be cached by the webhook token authenticator plugin
       in the kube-apiserver.
 
       **parameters**
 
       * **spec** ``TokenReviewSpec`` - Spec holds information about the request being evaluated
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
@@ -157,15 +157,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[TokenReviewStatus]' = None
 
 
 @dataclass
 class TokenReviewSpec(DictMixin):
-    """TokenReviewSpec is a description of the token authentication request.
+    r"""TokenReviewSpec is a description of the token authentication request.
 
       **parameters**
 
       * **audiences** ``Optional[List[str]]`` - Audiences is a list of the identifiers that the resource server presented with
         the token identifies as. Audience-aware token authenticators will verify that
         the token was intended for at least one of the audiences in this list. If no
         audiences are provided, the audience will default to the audience of the
@@ -174,15 +174,15 @@
     """
     audiences: 'Optional[List[str]]' = None
     token: 'Optional[str]' = None
 
 
 @dataclass
 class TokenReviewStatus(DictMixin):
-    """TokenReviewStatus is the result of the token authentication request.
+    r"""TokenReviewStatus is the result of the token authentication request.
 
       **parameters**
 
       * **audiences** ``Optional[List[str]]`` - Audiences are audience identifiers chosen by the authenticator that are
         compatible with both the TokenReview and token. An identifier is any
         identifier in the intersection of the TokenReviewSpec audiences and the
         token's audiences. A client of the TokenReview API that sets the
@@ -199,15 +199,15 @@
     authenticated: 'Optional[bool]' = None
     error: 'Optional[str]' = None
     user: 'Optional[UserInfo]' = None
 
 
 @dataclass
 class UserInfo(DictMixin):
-    """UserInfo holds the information about the user needed to implement the
+    r"""UserInfo holds the information about the user needed to implement the
       user.Info interface.
 
       **parameters**
 
       * **extra** ``Optional[dict]`` - Any additional information provided by the authenticator.
       * **groups** ``Optional[List[str]]`` - The names of groups this user is a part of.
       * **uid** ``Optional[str]`` - A unique value that identifies this user across time. If this user is deleted
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/authentication_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/models/authentication_v1alpha1.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from . import authentication_v1
 from . import meta_v1
 
 
 @dataclass
 class SelfSubjectReview(DictMixin):
-    """SelfSubjectReview contains the user information that the kube-apiserver has
+    r"""SelfSubjectReview contains the user information that the kube-apiserver has
       about the user making this request. When using impersonation, users will
       receive the user info of the user being impersonated.  If impersonation or
       request header authentication is used, any extra keys will have their case
       ignored and returned as lowercase.
 
       **parameters**
 
@@ -36,15 +36,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[SelfSubjectReviewStatus]' = None
 
 
 @dataclass
 class SelfSubjectReviewStatus(DictMixin):
-    """SelfSubjectReviewStatus is filled by the kube-apiserver and sent back to a
+    r"""SelfSubjectReviewStatus is filled by the kube-apiserver and sent back to a
       user.
 
       **parameters**
 
       * **userInfo** ``Optional[authentication_v1.UserInfo]`` - User attributes of the user making this request.
     """
     userInfo: 'Optional[authentication_v1.UserInfo]' = None
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/authentication_v1beta1.py` & `lightkube-models-1.30.0.8/lightkube/models/authentication_v1beta1.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from . import authentication_v1
 from . import meta_v1
 
 
 @dataclass
 class SelfSubjectReview(DictMixin):
-    """SelfSubjectReview contains the user information that the kube-apiserver has
+    r"""SelfSubjectReview contains the user information that the kube-apiserver has
       about the user making this request. When using impersonation, users will
       receive the user info of the user being impersonated.  If impersonation or
       request header authentication is used, any extra keys will have their case
       ignored and returned as lowercase.
 
       **parameters**
 
@@ -36,15 +36,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[SelfSubjectReviewStatus]' = None
 
 
 @dataclass
 class SelfSubjectReviewStatus(DictMixin):
-    """SelfSubjectReviewStatus is filled by the kube-apiserver and sent back to a
+    r"""SelfSubjectReviewStatus is filled by the kube-apiserver and sent back to a
       user.
 
       **parameters**
 
       * **userInfo** ``Optional[authentication_v1.UserInfo]`` - User attributes of the user making this request.
     """
     userInfo: 'Optional[authentication_v1.UserInfo]' = None
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/authorization_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/authorization_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class LocalSubjectAccessReview(DictMixin):
-    """LocalSubjectAccessReview checks whether or not a user or group can perform an
+    r"""LocalSubjectAccessReview checks whether or not a user or group can perform an
       action in a given namespace. Having a namespace scoped resource makes it much
       easier to grant namespace scoped policy that includes permissions checking.
 
       **parameters**
 
       * **spec** ``SubjectAccessReviewSpec`` - Spec holds information about the request being evaluated.  spec.namespace must
         be equal to the namespace you made the request against.  If empty, it is
@@ -38,44 +38,44 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[SubjectAccessReviewStatus]' = None
 
 
 @dataclass
 class NonResourceAttributes(DictMixin):
-    """NonResourceAttributes includes the authorization attributes available for
+    r"""NonResourceAttributes includes the authorization attributes available for
       non-resource requests to the Authorizer interface
 
       **parameters**
 
       * **path** ``Optional[str]`` - Path is the URL path of the request
       * **verb** ``Optional[str]`` - Verb is the standard HTTP verb
     """
     path: 'Optional[str]' = None
     verb: 'Optional[str]' = None
 
 
 @dataclass
 class NonResourceRule(DictMixin):
-    """NonResourceRule holds information that describes a rule for the non-resource
+    r"""NonResourceRule holds information that describes a rule for the non-resource
 
       **parameters**
 
       * **verbs** ``List[str]`` - Verb is a list of kubernetes non-resource API verbs, like: get, post, put,
         delete, patch, head, options.  "*" means all.
       * **nonResourceURLs** ``Optional[List[str]]`` - NonResourceURLs is a set of partial urls that a user should have access to.
         *s are allowed, but only as the full, final step in the path.  "*" means all.
     """
     verbs: 'List[str]'
     nonResourceURLs: 'Optional[List[str]]' = None
 
 
 @dataclass
 class ResourceAttributes(DictMixin):
-    """ResourceAttributes includes the authorization attributes available for
+    r"""ResourceAttributes includes the authorization attributes available for
       resource requests to the Authorizer interface
 
       **parameters**
 
       * **group** ``Optional[str]`` - Group is the API Group of the Resource.  "*" means all.
       * **name** ``Optional[str]`` - Name is the name of the resource being requested for a "get" or deleted for a
         "delete". "" (empty) means all.
@@ -97,15 +97,15 @@
     subresource: 'Optional[str]' = None
     verb: 'Optional[str]' = None
     version: 'Optional[str]' = None
 
 
 @dataclass
 class ResourceRule(DictMixin):
-    """ResourceRule is the list of actions the subject is allowed to perform on
+    r"""ResourceRule is the list of actions the subject is allowed to perform on
       resources. The list ordering isn't significant, may contain duplicates, and
       possibly be incomplete.
 
       **parameters**
 
       * **verbs** ``List[str]`` - Verb is a list of kubernetes resource API verbs, like: get, list, watch,
         create, update, delete, proxy.  "*" means all.
@@ -123,15 +123,15 @@
     apiGroups: 'Optional[List[str]]' = None
     resourceNames: 'Optional[List[str]]' = None
     resources: 'Optional[List[str]]' = None
 
 
 @dataclass
 class SelfSubjectAccessReview(DictMixin):
-    """SelfSubjectAccessReview checks whether or the current user can perform an
+    r"""SelfSubjectAccessReview checks whether or the current user can perform an
       action.  Not filling in a spec.namespace means "in all namespaces".  Self is a
       special case, because users should always be able to check whether they can
       perform an action
 
       **parameters**
 
       * **spec** ``SelfSubjectAccessReviewSpec`` - Spec holds information about the request being evaluated.  user and groups
@@ -154,15 +154,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[SubjectAccessReviewStatus]' = None
 
 
 @dataclass
 class SelfSubjectAccessReviewSpec(DictMixin):
-    """SelfSubjectAccessReviewSpec is a description of the access request.  Exactly
+    r"""SelfSubjectAccessReviewSpec is a description of the access request.  Exactly
       one of ResourceAuthorizationAttributes and NonResourceAuthorizationAttributes
       must be set
 
       **parameters**
 
       * **nonResourceAttributes** ``Optional[NonResourceAttributes]`` - NonResourceAttributes describes information for a non-resource access request
       * **resourceAttributes** ``Optional[ResourceAttributes]`` - ResourceAuthorizationAttributes describes information for a resource access
@@ -170,15 +170,15 @@
     """
     nonResourceAttributes: 'Optional[NonResourceAttributes]' = None
     resourceAttributes: 'Optional[ResourceAttributes]' = None
 
 
 @dataclass
 class SelfSubjectRulesReview(DictMixin):
-    """SelfSubjectRulesReview enumerates the set of actions the current user can
+    r"""SelfSubjectRulesReview enumerates the set of actions the current user can
       perform within a namespace. The returned list of actions may be incomplete
       depending on the server's authorization mode, and any errors experienced
       during the evaluation. SelfSubjectRulesReview should be used by UIs to
       show/hide actions, or to quickly let an end user reason about their
       permissions. It should NOT Be used by external systems to drive authorization
       decisions as this raises confused deputy, cache lifetime/revocation, and
       correctness concerns. SubjectAccessReview, and LocalAccessReview are the
@@ -205,27 +205,27 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[SubjectRulesReviewStatus]' = None
 
 
 @dataclass
 class SelfSubjectRulesReviewSpec(DictMixin):
-    """SelfSubjectRulesReviewSpec defines the specification for
+    r"""SelfSubjectRulesReviewSpec defines the specification for
       SelfSubjectRulesReview.
 
       **parameters**
 
       * **namespace** ``Optional[str]`` - Namespace to evaluate rules for. Required.
     """
     namespace: 'Optional[str]' = None
 
 
 @dataclass
 class SubjectAccessReview(DictMixin):
-    """SubjectAccessReview checks whether or not a user or group can perform an
+    r"""SubjectAccessReview checks whether or not a user or group can perform an
       action.
 
       **parameters**
 
       * **spec** ``SubjectAccessReviewSpec`` - Spec holds information about the request being evaluated
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -245,15 +245,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[SubjectAccessReviewStatus]' = None
 
 
 @dataclass
 class SubjectAccessReviewSpec(DictMixin):
-    """SubjectAccessReviewSpec is a description of the access request.  Exactly one
+    r"""SubjectAccessReviewSpec is a description of the access request.  Exactly one
       of ResourceAuthorizationAttributes and NonResourceAuthorizationAttributes must
       be set
 
       **parameters**
 
       * **extra** ``Optional[dict]`` - Extra corresponds to the user.Info.GetExtra() method from the authenticator.
         Since that is input to the authorizer it needs a reflection here.
@@ -271,15 +271,15 @@
     resourceAttributes: 'Optional[ResourceAttributes]' = None
     uid: 'Optional[str]' = None
     user: 'Optional[str]' = None
 
 
 @dataclass
 class SubjectAccessReviewStatus(DictMixin):
-    """SubjectAccessReviewStatus
+    r"""SubjectAccessReviewStatus
 
       **parameters**
 
       * **allowed** ``bool`` - Allowed is required. True if the action would be allowed, false otherwise.
       * **denied** ``Optional[bool]`` - Denied is optional. True if the action would be denied, otherwise false. If
         both allowed is false and denied is false, then the authorizer has no opinion
         on whether to authorize the action. Denied may not be true if Allowed is true.
@@ -294,15 +294,15 @@
     denied: 'Optional[bool]' = None
     evaluationError: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class SubjectRulesReviewStatus(DictMixin):
-    """SubjectRulesReviewStatus contains the result of a rules check. This check can
+    r"""SubjectRulesReviewStatus contains the result of a rules check. This check can
       be incomplete depending on the set of authorizers the server is configured
       with and any errors experienced during evaluation. Because authorization rules
       are additive, if a rule appears in a list it's safe to assume the subject has
       that permission, even if that list is incomplete.
 
       **parameters**
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/autoscaling_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/autoscaling_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class CrossVersionObjectReference(DictMixin):
-    """CrossVersionObjectReference contains enough information to let you identify
+    r"""CrossVersionObjectReference contains enough information to let you identify
       the referred resource.
 
       **parameters**
 
       * **kind** ``str`` - kind is the kind of the referent; More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **name** ``str`` - name is the name of the referent; More info:
@@ -25,15 +25,15 @@
     kind: 'str'
     name: 'str'
     apiVersion: 'Optional[str]' = None
 
 
 @dataclass
 class HorizontalPodAutoscaler(DictMixin):
-    """configuration of a horizontal pod autoscaler.
+    r"""configuration of a horizontal pod autoscaler.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -52,15 +52,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[HorizontalPodAutoscalerSpec]' = None
     status: 'Optional[HorizontalPodAutoscalerStatus]' = None
 
 
 @dataclass
 class HorizontalPodAutoscalerList(DictMixin):
-    """list of horizontal pod autoscaler objects.
+    r"""list of horizontal pod autoscaler objects.
 
       **parameters**
 
       * **items** ``List[HorizontalPodAutoscaler]`` - items is the list of horizontal pod autoscaler objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -75,15 +75,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class HorizontalPodAutoscalerSpec(DictMixin):
-    """specification of a horizontal pod autoscaler.
+    r"""specification of a horizontal pod autoscaler.
 
       **parameters**
 
       * **maxReplicas** ``int`` - maxReplicas is the upper limit for the number of pods that can be set by the
         autoscaler; cannot be smaller than MinReplicas.
       * **scaleTargetRef** ``CrossVersionObjectReference`` - reference to scaled resource; horizontal pod autoscaler will learn the current
         resource consumption and will set the desired number of pods by using its
@@ -101,15 +101,15 @@
     scaleTargetRef: 'CrossVersionObjectReference'
     minReplicas: 'Optional[int]' = None
     targetCPUUtilizationPercentage: 'Optional[int]' = None
 
 
 @dataclass
 class HorizontalPodAutoscalerStatus(DictMixin):
-    """current status of a horizontal pod autoscaler
+    r"""current status of a horizontal pod autoscaler
 
       **parameters**
 
       * **currentReplicas** ``int`` - currentReplicas is the current number of replicas of pods managed by this
         autoscaler.
       * **desiredReplicas** ``int`` - desiredReplicas is the  desired number of replicas of pods managed by this
         autoscaler.
@@ -126,15 +126,15 @@
     currentCPUUtilizationPercentage: 'Optional[int]' = None
     lastScaleTime: 'Optional[meta_v1.Time]' = None
     observedGeneration: 'Optional[int]' = None
 
 
 @dataclass
 class Scale(DictMixin):
-    """Scale represents a scaling request for a resource.
+    r"""Scale represents a scaling request for a resource.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -155,26 +155,26 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[ScaleSpec]' = None
     status: 'Optional[ScaleStatus]' = None
 
 
 @dataclass
 class ScaleSpec(DictMixin):
-    """ScaleSpec describes the attributes of a scale subresource.
+    r"""ScaleSpec describes the attributes of a scale subresource.
 
       **parameters**
 
       * **replicas** ``Optional[int]`` - replicas is the desired number of instances for the scaled object.
     """
     replicas: 'Optional[int]' = None
 
 
 @dataclass
 class ScaleStatus(DictMixin):
-    """ScaleStatus represents the current status of a scale subresource.
+    r"""ScaleStatus represents the current status of a scale subresource.
 
       **parameters**
 
       * **replicas** ``int`` - replicas is the actual number of observed instances of the scaled object.
       * **selector** ``Optional[str]`` - selector is the label query over pods that should match the replicas count.
         This is same as the label selector but in the string format to avoid
         introspection by clients. The string will be in the same format as the
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/autoscaling_v2.py` & `lightkube-models-1.30.0.8/lightkube/models/autoscaling_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from . import resource
 from . import meta_v1
+from . import resource
 
 
 @dataclass
 class ContainerResourceMetricSource(DictMixin):
-    """ContainerResourceMetricSource indicates how to scale on a resource metric
+    r"""ContainerResourceMetricSource indicates how to scale on a resource metric
       known to Kubernetes, as specified in requests and limits, describing each pod
       in the current scale target (e.g. CPU or memory).  The values will be averaged
       together before being compared to the target.  Such metrics are built in to
       Kubernetes, and have special scaling options on top of those available to
       normal per-pod metrics using the "pods" source.  Only one "target" type should
       be set.
 
@@ -29,15 +29,15 @@
     container: 'str'
     name: 'str'
     target: 'MetricTarget'
 
 
 @dataclass
 class ContainerResourceMetricStatus(DictMixin):
-    """ContainerResourceMetricStatus indicates the current value of a resource metric
+    r"""ContainerResourceMetricStatus indicates the current value of a resource metric
       known to Kubernetes, as specified in requests and limits, describing a single
       container in each pod in the current scale target (e.g. CPU or memory).  Such
       metrics are built in to Kubernetes, and have special scaling options on top of
       those available to normal per-pod metrics using the "pods" source.
 
       **parameters**
 
@@ -48,15 +48,15 @@
     container: 'str'
     current: 'MetricValueStatus'
     name: 'str'
 
 
 @dataclass
 class CrossVersionObjectReference(DictMixin):
-    """CrossVersionObjectReference contains enough information to let you identify
+    r"""CrossVersionObjectReference contains enough information to let you identify
       the referred resource.
 
       **parameters**
 
       * **kind** ``str`` - kind is the kind of the referent; More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#types-kinds
       * **name** ``str`` - name is the name of the referent; More info:
@@ -66,44 +66,44 @@
     kind: 'str'
     name: 'str'
     apiVersion: 'Optional[str]' = None
 
 
 @dataclass
 class ExternalMetricSource(DictMixin):
-    """ExternalMetricSource indicates how to scale on a metric not associated with
+    r"""ExternalMetricSource indicates how to scale on a metric not associated with
       any Kubernetes object (for example length of queue in cloud messaging service,
       or QPS from loadbalancer running outside of cluster).
 
       **parameters**
 
       * **metric** ``MetricIdentifier`` - metric identifies the target metric by name and selector
       * **target** ``MetricTarget`` - target specifies the target value for the given metric
     """
     metric: 'MetricIdentifier'
     target: 'MetricTarget'
 
 
 @dataclass
 class ExternalMetricStatus(DictMixin):
-    """ExternalMetricStatus indicates the current value of a global metric not
+    r"""ExternalMetricStatus indicates the current value of a global metric not
       associated with any Kubernetes object.
 
       **parameters**
 
       * **current** ``MetricValueStatus`` - current contains the current value for the given metric
       * **metric** ``MetricIdentifier`` - metric identifies the target metric by name and selector
     """
     current: 'MetricValueStatus'
     metric: 'MetricIdentifier'
 
 
 @dataclass
 class HPAScalingPolicy(DictMixin):
-    """HPAScalingPolicy is a single policy which must hold true for a specified past
+    r"""HPAScalingPolicy is a single policy which must hold true for a specified past
       interval.
 
       **parameters**
 
       * **periodSeconds** ``int`` - periodSeconds specifies the window of time for which the policy should hold
         true. PeriodSeconds must be greater than zero and less than or equal to 1800
         (30 min).
@@ -114,15 +114,15 @@
     periodSeconds: 'int'
     type: 'str'
     value: 'int'
 
 
 @dataclass
 class HPAScalingRules(DictMixin):
-    """HPAScalingRules configures the scaling behavior for one direction. These Rules
+    r"""HPAScalingRules configures the scaling behavior for one direction. These Rules
       are applied after calculating DesiredReplicas from metrics for the HPA. They
       can limit the scaling velocity by specifying scaling policies. They can
       prevent flapping by specifying the stabilization window, so that the number of
       replicas is not set instantly, instead, the safest value from the
       stabilization window is chosen.
 
       **parameters**
@@ -142,15 +142,15 @@
     policies: 'Optional[List[HPAScalingPolicy]]' = None
     selectPolicy: 'Optional[str]' = None
     stabilizationWindowSeconds: 'Optional[int]' = None
 
 
 @dataclass
 class HorizontalPodAutoscaler(DictMixin):
-    """HorizontalPodAutoscaler is the configuration for a horizontal pod autoscaler,
+    r"""HorizontalPodAutoscaler is the configuration for a horizontal pod autoscaler,
       which automatically manages the replica count of any resource implementing the
       scale subresource based on the metrics specified.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -171,15 +171,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[HorizontalPodAutoscalerSpec]' = None
     status: 'Optional[HorizontalPodAutoscalerStatus]' = None
 
 
 @dataclass
 class HorizontalPodAutoscalerBehavior(DictMixin):
-    """HorizontalPodAutoscalerBehavior configures the scaling behavior of the target
+    r"""HorizontalPodAutoscalerBehavior configures the scaling behavior of the target
       in both Up and Down directions (scaleUp and scaleDown fields respectively).
 
       **parameters**
 
       * **scaleDown** ``Optional[HPAScalingRules]`` - scaleDown is scaling policy for scaling Down. If not set, the default value is
         to allow to scale down to minReplicas pods, with a 300 second stabilization
         window (i.e., the highest recommendation for the last 300sec is used).
@@ -191,15 +191,15 @@
     """
     scaleDown: 'Optional[HPAScalingRules]' = None
     scaleUp: 'Optional[HPAScalingRules]' = None
 
 
 @dataclass
 class HorizontalPodAutoscalerCondition(DictMixin):
-    """HorizontalPodAutoscalerCondition describes the state of a
+    r"""HorizontalPodAutoscalerCondition describes the state of a
       HorizontalPodAutoscaler at a certain point.
 
       **parameters**
 
       * **status** ``str`` - status is the status of the condition (True, False, Unknown)
       * **type** ``str`` - type describes the current condition
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - lastTransitionTime is the last time the condition transitioned from one status
@@ -213,15 +213,15 @@
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class HorizontalPodAutoscalerList(DictMixin):
-    """HorizontalPodAutoscalerList is a list of horizontal pod autoscaler objects.
+    r"""HorizontalPodAutoscalerList is a list of horizontal pod autoscaler objects.
 
       **parameters**
 
       * **items** ``List[HorizontalPodAutoscaler]`` - items is the list of horizontal pod autoscaler objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -236,15 +236,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class HorizontalPodAutoscalerSpec(DictMixin):
-    """HorizontalPodAutoscalerSpec describes the desired functionality of the
+    r"""HorizontalPodAutoscalerSpec describes the desired functionality of the
       HorizontalPodAutoscaler.
 
       **parameters**
 
       * **maxReplicas** ``int`` - maxReplicas is the upper limit for the number of replicas to which the
         autoscaler can scale up. It cannot be less that minReplicas.
       * **scaleTargetRef** ``CrossVersionObjectReference`` - scaleTargetRef points to the target resource to scale, and is used to the pods
@@ -272,15 +272,15 @@
     behavior: 'Optional[HorizontalPodAutoscalerBehavior]' = None
     metrics: 'Optional[List[MetricSpec]]' = None
     minReplicas: 'Optional[int]' = None
 
 
 @dataclass
 class HorizontalPodAutoscalerStatus(DictMixin):
-    """HorizontalPodAutoscalerStatus describes the current status of a horizontal pod
+    r"""HorizontalPodAutoscalerStatus describes the current status of a horizontal pod
       autoscaler.
 
       **parameters**
 
       * **desiredReplicas** ``int`` - desiredReplicas is the desired number of replicas of pods managed by this
         autoscaler, as last calculated by the autoscaler.
       * **conditions** ``Optional[List[HorizontalPodAutoscalerCondition]]`` - conditions is the set of conditions required for this autoscaler to scale its
@@ -299,15 +299,15 @@
     currentReplicas: 'Optional[int]' = None
     lastScaleTime: 'Optional[meta_v1.Time]' = None
     observedGeneration: 'Optional[int]' = None
 
 
 @dataclass
 class MetricIdentifier(DictMixin):
-    """MetricIdentifier defines the name and optionally selector for a metric
+    r"""MetricIdentifier defines the name and optionally selector for a metric
 
       **parameters**
 
       * **name** ``str`` - name is the name of the given metric
       * **selector** ``Optional[meta_v1.LabelSelector]`` - selector is the string-encoded form of a standard kubernetes label selector
         for the given metric When set, it is passed as an additional parameter to the
         metrics server for more specific metrics scoping. When unset, just the
@@ -315,15 +315,15 @@
     """
     name: 'str'
     selector: 'Optional[meta_v1.LabelSelector]' = None
 
 
 @dataclass
 class MetricSpec(DictMixin):
-    """MetricSpec specifies how to scale based on a single metric (only `type` and
+    r"""MetricSpec specifies how to scale based on a single metric (only `type` and
       one other matching field should be set at once).
 
       **parameters**
 
       * **type** ``str`` - type is the type of metric source.  It should be one of "ContainerResource",
         "External", "Object", "Pods" or "Resource", each mapping to a matching field
         in the object. Note: "ContainerResource" type is available on when the
@@ -355,15 +355,15 @@
     object: 'Optional[ObjectMetricSource]' = None
     pods: 'Optional[PodsMetricSource]' = None
     resource: 'Optional[ResourceMetricSource]' = None
 
 
 @dataclass
 class MetricStatus(DictMixin):
-    """MetricStatus describes the last-read state of a single metric.
+    r"""MetricStatus describes the last-read state of a single metric.
 
       **parameters**
 
       * **type** ``str`` - type is the type of metric source.  It will be one of "ContainerResource",
         "External", "Object", "Pods" or "Resource", each corresponds to a matching
         field in the object. Note: "ContainerResource" type is available on when the
         feature-gate HPAContainerMetrics is enabled
@@ -393,15 +393,15 @@
     object: 'Optional[ObjectMetricStatus]' = None
     pods: 'Optional[PodsMetricStatus]' = None
     resource: 'Optional[ResourceMetricStatus]' = None
 
 
 @dataclass
 class MetricTarget(DictMixin):
-    """MetricTarget defines the target value, average value, or average utilization
+    r"""MetricTarget defines the target value, average value, or average utilization
       of a specific metric
 
       **parameters**
 
       * **type** ``str`` - type represents whether the metric type is Utilization, Value, or AverageValue
       * **averageUtilization** ``Optional[int]`` - averageUtilization is the target value of the average of the resource metric
         across all relevant pods, represented as a percentage of the requested value
@@ -415,15 +415,15 @@
     averageUtilization: 'Optional[int]' = None
     averageValue: 'Optional[resource.Quantity]' = None
     value: 'Optional[resource.Quantity]' = None
 
 
 @dataclass
 class MetricValueStatus(DictMixin):
-    """MetricValueStatus holds the current value for a metric
+    r"""MetricValueStatus holds the current value for a metric
 
       **parameters**
 
       * **averageUtilization** ``Optional[int]`` - currentAverageUtilization is the current value of the average of the resource
         metric across all relevant pods, represented as a percentage of the requested
         value of the resource for the pods.
       * **averageValue** ``Optional[resource.Quantity]`` - averageValue is the current value of the average of the metric across all
@@ -433,15 +433,15 @@
     averageUtilization: 'Optional[int]' = None
     averageValue: 'Optional[resource.Quantity]' = None
     value: 'Optional[resource.Quantity]' = None
 
 
 @dataclass
 class ObjectMetricSource(DictMixin):
-    """ObjectMetricSource indicates how to scale on a metric describing a kubernetes
+    r"""ObjectMetricSource indicates how to scale on a metric describing a kubernetes
       object (for example, hits-per-second on an Ingress object).
 
       **parameters**
 
       * **describedObject** ``CrossVersionObjectReference`` - describedObject specifies the descriptions of a object,such as kind,name
         apiVersion
       * **metric** ``MetricIdentifier`` - metric identifies the target metric by name and selector
@@ -450,15 +450,15 @@
     describedObject: 'CrossVersionObjectReference'
     metric: 'MetricIdentifier'
     target: 'MetricTarget'
 
 
 @dataclass
 class ObjectMetricStatus(DictMixin):
-    """ObjectMetricStatus indicates the current value of a metric describing a
+    r"""ObjectMetricStatus indicates the current value of a metric describing a
       kubernetes object (for example, hits-per-second on an Ingress object).
 
       **parameters**
 
       * **current** ``MetricValueStatus`` - current contains the current value for the given metric
       * **describedObject** ``CrossVersionObjectReference`` - DescribedObject specifies the descriptions of a object,such as kind,name
         apiVersion
@@ -467,44 +467,44 @@
     current: 'MetricValueStatus'
     describedObject: 'CrossVersionObjectReference'
     metric: 'MetricIdentifier'
 
 
 @dataclass
 class PodsMetricSource(DictMixin):
-    """PodsMetricSource indicates how to scale on a metric describing each pod in the
+    r"""PodsMetricSource indicates how to scale on a metric describing each pod in the
       current scale target (for example, transactions-processed-per-second). The
       values will be averaged together before being compared to the target value.
 
       **parameters**
 
       * **metric** ``MetricIdentifier`` - metric identifies the target metric by name and selector
       * **target** ``MetricTarget`` - target specifies the target value for the given metric
     """
     metric: 'MetricIdentifier'
     target: 'MetricTarget'
 
 
 @dataclass
 class PodsMetricStatus(DictMixin):
-    """PodsMetricStatus indicates the current value of a metric describing each pod
+    r"""PodsMetricStatus indicates the current value of a metric describing each pod
       in the current scale target (for example, transactions-processed-per-second).
 
       **parameters**
 
       * **current** ``MetricValueStatus`` - current contains the current value for the given metric
       * **metric** ``MetricIdentifier`` - metric identifies the target metric by name and selector
     """
     current: 'MetricValueStatus'
     metric: 'MetricIdentifier'
 
 
 @dataclass
 class ResourceMetricSource(DictMixin):
-    """ResourceMetricSource indicates how to scale on a resource metric known to
+    r"""ResourceMetricSource indicates how to scale on a resource metric known to
       Kubernetes, as specified in requests and limits, describing each pod in the
       current scale target (e.g. CPU or memory).  The values will be averaged
       together before being compared to the target.  Such metrics are built in to
       Kubernetes, and have special scaling options on top of those available to
       normal per-pod metrics using the "pods" source.  Only one "target" type should
       be set.
 
@@ -515,15 +515,15 @@
     """
     name: 'str'
     target: 'MetricTarget'
 
 
 @dataclass
 class ResourceMetricStatus(DictMixin):
-    """ResourceMetricStatus indicates the current value of a resource metric known to
+    r"""ResourceMetricStatus indicates the current value of a resource metric known to
       Kubernetes, as specified in requests and limits, describing each pod in the
       current scale target (e.g. CPU or memory).  Such metrics are built in to
       Kubernetes, and have special scaling options on top of those available to
       normal per-pod metrics using the "pods" source.
 
       **parameters**
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/batch_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/batch_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from . import core_v1
 from . import meta_v1
+from . import core_v1
 
 
 @dataclass
 class CronJob(DictMixin):
-    """CronJob represents the configuration of a single cron job.
+    r"""CronJob represents the configuration of a single cron job.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -37,15 +37,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[CronJobSpec]' = None
     status: 'Optional[CronJobStatus]' = None
 
 
 @dataclass
 class CronJobList(DictMixin):
-    """CronJobList is a collection of cron jobs.
+    r"""CronJobList is a collection of cron jobs.
 
       **parameters**
 
       * **items** ``List[CronJob]`` - items is the list of CronJobs.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -61,15 +61,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class CronJobSpec(DictMixin):
-    """CronJobSpec describes how the job execution will look like and when it will
+    r"""CronJobSpec describes how the job execution will look like and when it will
       actually run.
 
       **parameters**
 
       * **jobTemplate** ``JobTemplateSpec`` - Specifies the job that will be created when executing a CronJob.
       * **schedule** ``str`` - The schedule in Cron format, see https://en.wikipedia.org/wiki/Cron.
       * **concurrencyPolicy** ``Optional[str]`` - Specifies how to treat concurrent executions of a Job. Valid values are:
@@ -105,30 +105,30 @@
     successfulJobsHistoryLimit: 'Optional[int]' = None
     suspend: 'Optional[bool]' = None
     timeZone: 'Optional[str]' = None
 
 
 @dataclass
 class CronJobStatus(DictMixin):
-    """CronJobStatus represents the current state of a cron job.
+    r"""CronJobStatus represents the current state of a cron job.
 
       **parameters**
 
       * **active** ``Optional[List[core_v1.ObjectReference]]`` - A list of pointers to currently running jobs.
       * **lastScheduleTime** ``Optional[meta_v1.Time]`` - Information when was the last time the job was successfully scheduled.
       * **lastSuccessfulTime** ``Optional[meta_v1.Time]`` - Information when was the last time the job successfully completed.
     """
     active: 'Optional[List[core_v1.ObjectReference]]' = None
     lastScheduleTime: 'Optional[meta_v1.Time]' = None
     lastSuccessfulTime: 'Optional[meta_v1.Time]' = None
 
 
 @dataclass
 class Job(DictMixin):
-    """Job represents the configuration of a single job.
+    r"""Job represents the configuration of a single job.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -148,15 +148,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[JobSpec]' = None
     status: 'Optional[JobStatus]' = None
 
 
 @dataclass
 class JobCondition(DictMixin):
-    """JobCondition describes current state of a job.
+    r"""JobCondition describes current state of a job.
 
       **parameters**
 
       * **status** ``str`` - Status of the condition, one of True, False, Unknown.
       * **type** ``str`` - Type of job condition, Complete or Failed.
       * **lastProbeTime** ``Optional[meta_v1.Time]`` - Last time the condition was checked.
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - Last time the condition transit from one status to another.
@@ -169,15 +169,15 @@
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class JobList(DictMixin):
-    """JobList is a collection of jobs.
+    r"""JobList is a collection of jobs.
 
       **parameters**
 
       * **items** ``List[Job]`` - items is the list of Jobs.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -193,15 +193,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class JobSpec(DictMixin):
-    """JobSpec describes how the job execution will look like.
+    r"""JobSpec describes how the job execution will look like.
 
       **parameters**
 
       * **template** ``core_v1.PodTemplateSpec`` - Describes the pod that will be created when executing a job. The only allowed
         template.spec.restartPolicy values are "Never" or "OnFailure". More info:
         https://kubernetes.io/docs/concepts/workloads/controllers/jobs-run-to-completion/
       * **activeDeadlineSeconds** ``Optional[int]`` - Specifies the duration in seconds relative to the startTime that the job may
@@ -330,15 +330,15 @@
     successPolicy: 'Optional[SuccessPolicy]' = None
     suspend: 'Optional[bool]' = None
     ttlSecondsAfterFinished: 'Optional[int]' = None
 
 
 @dataclass
 class JobStatus(DictMixin):
-    """JobStatus represents the current state of a Job.
+    r"""JobStatus represents the current state of a Job.
 
       **parameters**
 
       * **active** ``Optional[int]`` - The number of pending and running pods which are not terminating (without a
         deletionTimestamp). The value is zero for finished jobs.
       * **completedIndexes** ``Optional[str]`` - completedIndexes holds the completed indexes when .spec.completionMode =
         "Indexed" in a text format. The indexes are represented as decimal integers
@@ -412,15 +412,15 @@
     succeeded: 'Optional[int]' = None
     terminating: 'Optional[int]' = None
     uncountedTerminatedPods: 'Optional[UncountedTerminatedPods]' = None
 
 
 @dataclass
 class JobTemplateSpec(DictMixin):
-    """JobTemplateSpec describes the data a Job should have when created from a
+    r"""JobTemplateSpec describes the data a Job should have when created from a
       template
 
       **parameters**
 
       * **metadata** ``Optional[meta_v1.ObjectMeta]`` - Standard object's metadata of the jobs created from this template. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
       * **spec** ``Optional[JobSpec]`` - Specification of the desired behavior of the job. More info:
@@ -428,30 +428,30 @@
     """
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[JobSpec]' = None
 
 
 @dataclass
 class PodFailurePolicy(DictMixin):
-    """PodFailurePolicy describes how failed pods influence the backoffLimit.
+    r"""PodFailurePolicy describes how failed pods influence the backoffLimit.
 
       **parameters**
 
       * **rules** ``List[PodFailurePolicyRule]`` - A list of pod failure policy rules. The rules are evaluated in order. Once a
         rule matches a Pod failure, the remaining of the rules are ignored. When no
         rule matches the Pod failure, the default handling applies - the counter of
         pod failures is incremented and it is checked against the backoffLimit. At
         most 20 elements are allowed.
     """
     rules: 'List[PodFailurePolicyRule]'
 
 
 @dataclass
 class PodFailurePolicyOnExitCodesRequirement(DictMixin):
-    """PodFailurePolicyOnExitCodesRequirement describes the requirement for handling
+    r"""PodFailurePolicyOnExitCodesRequirement describes the requirement for handling
       a failed pod based on its container exit codes. In particular, it lookups the
       .state.terminated.exitCode for each app container and init container status,
       represented by the .status.containerStatuses and .status.initContainerStatuses
       fields in the Pod status, respectively. Containers completed with success
       (exit code 0) are excluded from the requirement check.
 
       **parameters**
@@ -479,15 +479,15 @@
     operator: 'str'
     values: 'List[int]'
     containerName: 'Optional[str]' = None
 
 
 @dataclass
 class PodFailurePolicyOnPodConditionsPattern(DictMixin):
-    """PodFailurePolicyOnPodConditionsPattern describes a pattern for matching an
+    r"""PodFailurePolicyOnPodConditionsPattern describes a pattern for matching an
       actual pod condition type.
 
       **parameters**
 
       * **status** ``str`` - Specifies the required Pod condition status. To match a pod condition it is
         required that the specified status equals the pod condition status. Defaults
         to True.
@@ -496,15 +496,15 @@
     """
     status: 'str'
     type: 'str'
 
 
 @dataclass
 class PodFailurePolicyRule(DictMixin):
-    """PodFailurePolicyRule describes how a pod failure is handled when the
+    r"""PodFailurePolicyRule describes how a pod failure is handled when the
       requirements are met. One of onExitCodes and onPodConditions, but not both,
       can be used in each rule.
 
       **parameters**
 
       * **action** ``str`` - Specifies the action taken on a pod failure when the requirements are
         satisfied. Possible values are:
@@ -529,15 +529,15 @@
     action: 'str'
     onExitCodes: 'Optional[PodFailurePolicyOnExitCodesRequirement]' = None
     onPodConditions: 'Optional[List[PodFailurePolicyOnPodConditionsPattern]]' = None
 
 
 @dataclass
 class SuccessPolicy(DictMixin):
-    """SuccessPolicy describes when a Job can be declared as succeeded based on the
+    r"""SuccessPolicy describes when a Job can be declared as succeeded based on the
       success of some indexes.
 
       **parameters**
 
       * **rules** ``List[SuccessPolicyRule]`` - rules represents the list of alternative rules for the declaring the Jobs as
         successful before `.status.succeeded >= .spec.completions`. Once any of the
         rules are met, the "SucceededCriteriaMet" condition is added, and the
@@ -547,15 +547,15 @@
         are allowed.
     """
     rules: 'List[SuccessPolicyRule]'
 
 
 @dataclass
 class SuccessPolicyRule(DictMixin):
-    """SuccessPolicyRule describes rule for declaring a Job as succeeded. Each rule
+    r"""SuccessPolicyRule describes rule for declaring a Job as succeeded. Each rule
       must have at least one of the "succeededIndexes" or "succeededCount"
       specified.
 
       **parameters**
 
       * **succeededCount** ``Optional[int]`` - succeededCount specifies the minimal required size of the actual set of the
         succeeded indexes for the Job. When succeededCount is used along with
@@ -579,15 +579,15 @@
     """
     succeededCount: 'Optional[int]' = None
     succeededIndexes: 'Optional[str]' = None
 
 
 @dataclass
 class UncountedTerminatedPods(DictMixin):
-    """UncountedTerminatedPods holds UIDs of Pods that have terminated but haven't
+    r"""UncountedTerminatedPods holds UIDs of Pods that have terminated but haven't
       been accounted in Job status counters.
 
       **parameters**
 
       * **failed** ``Optional[List[str]]`` - failed holds UIDs of failed Pods.
       * **succeeded** ``Optional[List[str]]`` - succeeded holds UIDs of succeeded Pods.
     """
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/certificates_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/certificates_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class CertificateSigningRequest(DictMixin):
-    """CertificateSigningRequest objects provide a mechanism to obtain x509
+    r"""CertificateSigningRequest objects provide a mechanism to obtain x509
       certificates by submitting a certificate signing request, and having it
       asynchronously approved and issued.
       
       Kubelets use this API to obtain:
        1. client certificates to authenticate to kube-apiserver (with the
       "kubernetes.io/kube-apiserver-client-kubelet" signerName).
        2. serving certificates for TLS endpoints kube-apiserver can connect to
@@ -49,15 +49,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[CertificateSigningRequestStatus]' = None
 
 
 @dataclass
 class CertificateSigningRequestCondition(DictMixin):
-    """CertificateSigningRequestCondition describes a condition of a
+    r"""CertificateSigningRequestCondition describes a condition of a
       CertificateSigningRequest object
 
       **parameters**
 
       * **status** ``str`` - status of the condition, one of True, False, Unknown. Approved, Denied, and
         Failed conditions may not be "False" or "Unknown".
       * **type** ``str`` - type of the condition. Known conditions are "Approved", "Denied", and
@@ -84,15 +84,15 @@
     lastUpdateTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class CertificateSigningRequestList(DictMixin):
-    """CertificateSigningRequestList is a collection of CertificateSigningRequest
+    r"""CertificateSigningRequestList is a collection of CertificateSigningRequest
       objects
 
       **parameters**
 
       * **items** ``List[CertificateSigningRequest]`` - items is a collection of CertificateSigningRequest objects
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -108,15 +108,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class CertificateSigningRequestSpec(DictMixin):
-    """CertificateSigningRequestSpec contains the certificate request.
+    r"""CertificateSigningRequestSpec contains the certificate request.
 
       **parameters**
 
       * **request** ``str`` - request contains an x509 certificate signing request encoded in a "CERTIFICATE
         REQUEST" PEM block. When serialized as JSON or YAML, the data is additionally
         base64-encoded.
       * **signerName** ``str`` - signerName indicates the requested signer, and is a qualified name.
@@ -196,15 +196,15 @@
     uid: 'Optional[str]' = None
     usages: 'Optional[List[str]]' = None
     username: 'Optional[str]' = None
 
 
 @dataclass
 class CertificateSigningRequestStatus(DictMixin):
-    """CertificateSigningRequestStatus contains conditions used to indicate
+    r"""CertificateSigningRequestStatus contains conditions used to indicate
       approved/denied/failed status of the request, and the issued certificate.
 
       **parameters**
 
       * **certificate** ``Optional[str]`` - certificate is populated with an issued certificate by the signer after an
         Approved condition is present. This field is set via the /status subresource.
         Once populated, this field is immutable.
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/certificates_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/models/certificates_v1alpha1.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class ClusterTrustBundle(DictMixin):
-    """ClusterTrustBundle is a cluster-scoped container for X.509 trust anchors (root
+    r"""ClusterTrustBundle is a cluster-scoped container for X.509 trust anchors (root
       certificates).
       
       ClusterTrustBundle objects are considered to be readable by any authenticated
       user in the cluster, because they can be mounted by pods using the
       `clusterTrustBundle` projection.  All service accounts have read access to
       ClusterTrustBundles by default.  Users who only have namespace-level access to
       a cluster can read ClusterTrustBundles by impersonating a serviceaccount that
@@ -44,15 +44,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
 class ClusterTrustBundleList(DictMixin):
-    """ClusterTrustBundleList is a collection of ClusterTrustBundle objects
+    r"""ClusterTrustBundleList is a collection of ClusterTrustBundle objects
 
       **parameters**
 
       * **items** ``List[ClusterTrustBundle]`` - items is a collection of ClusterTrustBundle objects
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -67,15 +67,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ClusterTrustBundleSpec(DictMixin):
-    """ClusterTrustBundleSpec contains the signer and trust anchors.
+    r"""ClusterTrustBundleSpec contains the signer and trust anchors.
 
       **parameters**
 
       * **trustBundle** ``str`` - trustBundle contains the individual X.509 trust anchors for this bundle, as
         PEM bundle of PEM-wrapped, DER-formatted X.509 certificates.
         The data must consist only of PEM certificate blocks that parse as valid X.509
         certificates.  Each certificate must include a basic constraints extension
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/coordination_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/coordination_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class Lease(DictMixin):
-    """Lease defines a lease concept.
+    r"""Lease defines a lease concept.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -32,15 +32,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[LeaseSpec]' = None
 
 
 @dataclass
 class LeaseList(DictMixin):
-    """LeaseList is a list of Lease objects.
+    r"""LeaseList is a list of Lease objects.
 
       **parameters**
 
       * **items** ``List[Lease]`` - items is a list of schema objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -56,15 +56,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class LeaseSpec(DictMixin):
-    """LeaseSpec is a specification of a Lease.
+    r"""LeaseSpec is a specification of a Lease.
 
       **parameters**
 
       * **acquireTime** ``Optional[meta_v1.MicroTime]`` - acquireTime is a time when the current lease was acquired.
       * **holderIdentity** ``Optional[str]`` - holderIdentity contains the identity of the holder of a current lease.
       * **leaseDurationSeconds** ``Optional[int]`` - leaseDurationSeconds is a duration that candidates for a lease need to wait to
         force acquire it. This is measure against time of last observed renewTime.
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/core_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/core_v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
 from . import resource
-from . import util_intstr
 from . import meta_v1
+from . import util_intstr
 
 
 @dataclass
 class AWSElasticBlockStoreVolumeSource(DictMixin):
-    """Represents a Persistent Disk resource in AWS.
+    r"""Represents a Persistent Disk resource in AWS.
       
       An AWS EBS disk must exist before mounting to a container. The disk must also
       be in the same AWS zone as the kubelet. An AWS EBS disk can only be mounted as
       read/write once. AWS EBS volumes support ownership management and SELinux
       relabeling.
 
       **parameters**
@@ -41,15 +41,15 @@
     fsType: 'Optional[str]' = None
     partition: 'Optional[int]' = None
     readOnly: 'Optional[bool]' = None
 
 
 @dataclass
 class Affinity(DictMixin):
-    """Affinity is a group of affinity scheduling rules.
+    r"""Affinity is a group of affinity scheduling rules.
 
       **parameters**
 
       * **nodeAffinity** ``Optional[NodeAffinity]`` - Describes node affinity scheduling rules for the pod.
       * **podAffinity** ``Optional[PodAffinity]`` - Describes pod affinity scheduling rules (e.g. co-locate this pod in the same
         node, zone, etc. as some other pod(s)).
       * **podAntiAffinity** ``Optional[PodAntiAffinity]`` - Describes pod anti-affinity scheduling rules (e.g. avoid putting this pod in
@@ -58,15 +58,15 @@
     nodeAffinity: 'Optional[NodeAffinity]' = None
     podAffinity: 'Optional[PodAffinity]' = None
     podAntiAffinity: 'Optional[PodAntiAffinity]' = None
 
 
 @dataclass
 class AppArmorProfile(DictMixin):
-    """AppArmorProfile defines a pod or container's AppArmor settings.
+    r"""AppArmorProfile defines a pod or container's AppArmor settings.
 
       **parameters**
 
       * **type** ``str`` - type indicates which kind of AppArmor profile will be applied. Valid options
         are:
           Localhost - a profile pre-loaded on the node.
           RuntimeDefault - the container runtime's default profile.
@@ -77,28 +77,28 @@
     """
     type: 'str'
     localhostProfile: 'Optional[str]' = None
 
 
 @dataclass
 class AttachedVolume(DictMixin):
-    """AttachedVolume describes a volume attached to a node
+    r"""AttachedVolume describes a volume attached to a node
 
       **parameters**
 
       * **devicePath** ``str`` - DevicePath represents the device path where the volume should be available
       * **name** ``str`` - Name of the attached volume
     """
     devicePath: 'str'
     name: 'str'
 
 
 @dataclass
 class AzureDiskVolumeSource(DictMixin):
-    """AzureDisk represents an Azure Data Disk mount on the host and bind mount to
+    r"""AzureDisk represents an Azure Data Disk mount on the host and bind mount to
       the pod.
 
       **parameters**
 
       * **diskName** ``str`` - diskName is the Name of the data disk in the blob storage
       * **diskURI** ``str`` - diskURI is the URI of data disk in the blob storage
       * **cachingMode** ``Optional[str]`` - cachingMode is the Host Caching mode: None, Read Only, Read Write.
@@ -117,15 +117,15 @@
     fsType: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     readOnly: 'Optional[bool]' = None
 
 
 @dataclass
 class AzureFilePersistentVolumeSource(DictMixin):
-    """AzureFile represents an Azure File Service mount on the host and bind mount to
+    r"""AzureFile represents an Azure File Service mount on the host and bind mount to
       the pod.
 
       **parameters**
 
       * **secretName** ``str`` - secretName is the name of secret that contains Azure Storage Account Name and
         Key
       * **shareName** ``str`` - shareName is the azure Share Name
@@ -138,15 +138,15 @@
     shareName: 'str'
     readOnly: 'Optional[bool]' = None
     secretNamespace: 'Optional[str]' = None
 
 
 @dataclass
 class AzureFileVolumeSource(DictMixin):
-    """AzureFile represents an Azure File Service mount on the host and bind mount to
+    r"""AzureFile represents an Azure File Service mount on the host and bind mount to
       the pod.
 
       **parameters**
 
       * **secretName** ``str`` - secretName is the  name of secret that contains Azure Storage Account Name and
         Key
       * **shareName** ``str`` - shareName is the azure share Name
@@ -156,15 +156,15 @@
     secretName: 'str'
     shareName: 'str'
     readOnly: 'Optional[bool]' = None
 
 
 @dataclass
 class Binding(DictMixin):
-    """Binding ties one object to another; for example, a pod is bound to a node by a
+    r"""Binding ties one object to another; for example, a pod is bound to a node by a
       scheduler. Deprecated in 1.7, please use the bindings subresource of pods
       instead.
 
       **parameters**
 
       * **target** ``ObjectReference`` - The target object that you want to bind to the standard object.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
@@ -182,15 +182,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
 class CSIPersistentVolumeSource(DictMixin):
-    """Represents storage that is managed by an external CSI volume driver (Beta
+    r"""Represents storage that is managed by an external CSI volume driver (Beta
       feature)
 
       **parameters**
 
       * **driver** ``str`` - driver is the name of the driver to use for this volume. Required.
       * **volumeHandle** ``str`` - volumeHandle is the unique volume name returned by the CSI volume plugin’s
         CreateVolume to refer to the volume on all subsequent calls. Required.
@@ -234,15 +234,15 @@
     nodeStageSecretRef: 'Optional[SecretReference]' = None
     readOnly: 'Optional[bool]' = None
     volumeAttributes: 'Optional[dict]' = None
 
 
 @dataclass
 class CSIVolumeSource(DictMixin):
-    """Represents a source location of a volume to mount, managed by an external CSI
+    r"""Represents a source location of a volume to mount, managed by an external CSI
       driver
 
       **parameters**
 
       * **driver** ``str`` - driver is the name of the CSI driver that handles this volume. Consult with
         your admin for the correct name as registered in the cluster.
       * **fsType** ``Optional[str]`` - fsType to mount. Ex. "ext4", "xfs", "ntfs". If not provided, the empty value
@@ -263,28 +263,28 @@
     nodePublishSecretRef: 'Optional[LocalObjectReference]' = None
     readOnly: 'Optional[bool]' = None
     volumeAttributes: 'Optional[dict]' = None
 
 
 @dataclass
 class Capabilities(DictMixin):
-    """Adds and removes POSIX capabilities from running containers.
+    r"""Adds and removes POSIX capabilities from running containers.
 
       **parameters**
 
       * **add** ``Optional[List[str]]`` - Added capabilities
       * **drop** ``Optional[List[str]]`` - Removed capabilities
     """
     add: 'Optional[List[str]]' = None
     drop: 'Optional[List[str]]' = None
 
 
 @dataclass
 class CephFSPersistentVolumeSource(DictMixin):
-    """Represents a Ceph Filesystem mount that lasts the lifetime of a pod Cephfs
+    r"""Represents a Ceph Filesystem mount that lasts the lifetime of a pod Cephfs
       volumes do not support ownership management or SELinux relabeling.
 
       **parameters**
 
       * **monitors** ``List[str]`` - monitors is Required: Monitors is a collection of Ceph monitors More info:
         https://examples.k8s.io/volumes/cephfs/README.md#how-to-use-it
       * **path** ``Optional[str]`` - path is Optional: Used as the mounted root, rather than the full Ceph tree,
@@ -307,15 +307,15 @@
     secretFile: 'Optional[str]' = None
     secretRef: 'Optional[SecretReference]' = None
     user: 'Optional[str]' = None
 
 
 @dataclass
 class CephFSVolumeSource(DictMixin):
-    """Represents a Ceph Filesystem mount that lasts the lifetime of a pod Cephfs
+    r"""Represents a Ceph Filesystem mount that lasts the lifetime of a pod Cephfs
       volumes do not support ownership management or SELinux relabeling.
 
       **parameters**
 
       * **monitors** ``List[str]`` - monitors is Required: Monitors is a collection of Ceph monitors More info:
         https://examples.k8s.io/volumes/cephfs/README.md#how-to-use-it
       * **path** ``Optional[str]`` - path is Optional: Used as the mounted root, rather than the full Ceph tree,
@@ -338,15 +338,15 @@
     secretFile: 'Optional[str]' = None
     secretRef: 'Optional[LocalObjectReference]' = None
     user: 'Optional[str]' = None
 
 
 @dataclass
 class CinderPersistentVolumeSource(DictMixin):
-    """Represents a cinder volume resource in Openstack. A Cinder volume must exist
+    r"""Represents a cinder volume resource in Openstack. A Cinder volume must exist
       before mounting to a container. The volume must also be in the same region as
       the kubelet. Cinder volumes support ownership management and SELinux
       relabeling.
 
       **parameters**
 
       * **volumeID** ``str`` - volumeID used to identify the volume in cinder. More info:
@@ -365,15 +365,15 @@
     fsType: 'Optional[str]' = None
     readOnly: 'Optional[bool]' = None
     secretRef: 'Optional[SecretReference]' = None
 
 
 @dataclass
 class CinderVolumeSource(DictMixin):
-    """Represents a cinder volume resource in Openstack. A Cinder volume must exist
+    r"""Represents a cinder volume resource in Openstack. A Cinder volume must exist
       before mounting to a container. The volume must also be in the same region as
       the kubelet. Cinder volumes support ownership management and SELinux
       relabeling.
 
       **parameters**
 
       * **volumeID** ``str`` - volumeID used to identify the volume in cinder. More info:
@@ -392,15 +392,15 @@
     fsType: 'Optional[str]' = None
     readOnly: 'Optional[bool]' = None
     secretRef: 'Optional[LocalObjectReference]' = None
 
 
 @dataclass
 class ClaimSource(DictMixin):
-    """ClaimSource describes a reference to a ResourceClaim.
+    r"""ClaimSource describes a reference to a ResourceClaim.
       
       Exactly one of these fields should be set.  Consumers of this type must treat
       an empty object as if it has an unknown value.
 
       **parameters**
 
       * **resourceClaimName** ``Optional[str]`` - ResourceClaimName is the name of a ResourceClaim object in the same namespace
@@ -417,29 +417,29 @@
     """
     resourceClaimName: 'Optional[str]' = None
     resourceClaimTemplateName: 'Optional[str]' = None
 
 
 @dataclass
 class ClientIPConfig(DictMixin):
-    """ClientIPConfig represents the configurations of Client IP based session
+    r"""ClientIPConfig represents the configurations of Client IP based session
       affinity.
 
       **parameters**
 
       * **timeoutSeconds** ``Optional[int]`` - timeoutSeconds specifies the seconds of ClientIP type session sticky time. The
         value must be >0 && <=86400(for 1 day) if ServiceAffinity == "ClientIP".
         Default value is 10800(for 3 hours).
     """
     timeoutSeconds: 'Optional[int]' = None
 
 
 @dataclass
 class ClusterTrustBundleProjection(DictMixin):
-    """ClusterTrustBundleProjection describes how to select a set of
+    r"""ClusterTrustBundleProjection describes how to select a set of
       ClusterTrustBundle objects and project their contents into the pod filesystem.
 
       **parameters**
 
       * **path** ``str`` - Relative path from the volume root to write the bundle.
       * **labelSelector** ``Optional[meta_v1.LabelSelector]`` - Select all ClusterTrustBundles that match this label selector.  Only has
         effect if signerName is set.  Mutually-exclusive with name.  If unset,
@@ -460,15 +460,15 @@
     name: 'Optional[str]' = None
     optional: 'Optional[bool]' = None
     signerName: 'Optional[str]' = None
 
 
 @dataclass
 class ComponentCondition(DictMixin):
-    """Information about the condition of a component.
+    r"""Information about the condition of a component.
 
       **parameters**
 
       * **status** ``str`` - Status of the condition for a component. Valid values for "Healthy": "True",
         "False", or "Unknown".
       * **type** ``str`` - Type of condition for a component. Valid value: "Healthy"
       * **error** ``Optional[str]`` - Condition error code for a component. For example, a health check error code.
@@ -479,15 +479,15 @@
     type: 'str'
     error: 'Optional[str]' = None
     message: 'Optional[str]' = None
 
 
 @dataclass
 class ComponentStatus(DictMixin):
-    """ComponentStatus (and ComponentStatusList) holds the cluster validation info.
+    r"""ComponentStatus (and ComponentStatusList) holds the cluster validation info.
       Deprecated: This API is deprecated in v1.19+
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -504,15 +504,15 @@
     conditions: 'Optional[List[ComponentCondition]]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
 class ComponentStatusList(DictMixin):
-    """Status of all the conditions for the component as a list of ComponentStatus
+    r"""Status of all the conditions for the component as a list of ComponentStatus
       objects. Deprecated: This API is deprecated in v1.19+
 
       **parameters**
 
       * **items** ``List[ComponentStatus]`` - List of ComponentStatus objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -529,15 +529,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ConfigMap(DictMixin):
-    """ConfigMap holds configuration data for pods to consume.
+    r"""ConfigMap holds configuration data for pods to consume.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -566,15 +566,15 @@
     immutable: 'Optional[bool]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
 class ConfigMapEnvSource(DictMixin):
-    """ConfigMapEnvSource selects a ConfigMap to populate the environment variables
+    r"""ConfigMapEnvSource selects a ConfigMap to populate the environment variables
       with.
       
       The contents of the target ConfigMap's Data field will represent the key-value
       pairs as environment variables.
 
       **parameters**
 
@@ -584,15 +584,15 @@
     """
     name: 'Optional[str]' = None
     optional: 'Optional[bool]' = None
 
 
 @dataclass
 class ConfigMapKeySelector(DictMixin):
-    """Selects a key from a ConfigMap.
+    r"""Selects a key from a ConfigMap.
 
       **parameters**
 
       * **key** ``str`` - The key to select.
       * **name** ``Optional[str]`` - Name of the referent. More info:
         https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names
       * **optional** ``Optional[bool]`` - Specify whether the ConfigMap or its key must be defined
@@ -600,15 +600,15 @@
     key: 'str'
     name: 'Optional[str]' = None
     optional: 'Optional[bool]' = None
 
 
 @dataclass
 class ConfigMapList(DictMixin):
-    """ConfigMapList is a resource containing a list of ConfigMap objects.
+    r"""ConfigMapList is a resource containing a list of ConfigMap objects.
 
       **parameters**
 
       * **items** ``List[ConfigMap]`` - Items is the list of ConfigMaps.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -624,15 +624,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ConfigMapNodeConfigSource(DictMixin):
-    """ConfigMapNodeConfigSource contains the information to reference a ConfigMap as
+    r"""ConfigMapNodeConfigSource contains the information to reference a ConfigMap as
       a config source for the Node. This API is deprecated since 1.22:
       https://git.k8s.io/enhancements/keps/sig-node/281-dynamic-kubelet-configuration
 
       **parameters**
 
       * **kubeletConfigKey** ``str`` - KubeletConfigKey declares which key of the referenced ConfigMap corresponds to
         the KubeletConfiguration structure This field is required in all cases.
@@ -650,15 +650,15 @@
     namespace: 'str'
     resourceVersion: 'Optional[str]' = None
     uid: 'Optional[str]' = None
 
 
 @dataclass
 class ConfigMapProjection(DictMixin):
-    """Adapts a ConfigMap into a projected volume.
+    r"""Adapts a ConfigMap into a projected volume.
       
       The contents of the target ConfigMap's Data field will be presented in a
       projected volume as files using the keys in the Data field as the file names,
       unless the items element is populated with specific mappings of keys to paths.
       Note that this is identical to a configmap volume source without the default
       mode.
 
@@ -678,15 +678,15 @@
     items: 'Optional[List[KeyToPath]]' = None
     name: 'Optional[str]' = None
     optional: 'Optional[bool]' = None
 
 
 @dataclass
 class ConfigMapVolumeSource(DictMixin):
-    """Adapts a ConfigMap into a volume.
+    r"""Adapts a ConfigMap into a volume.
       
       The contents of the target ConfigMap's Data field will be presented in a
       volume as files using the keys in the Data field as the file names, unless the
       items element is populated with specific mappings of keys to paths. ConfigMap
       volumes support ownership management and SELinux relabeling.
 
       **parameters**
@@ -713,15 +713,15 @@
     items: 'Optional[List[KeyToPath]]' = None
     name: 'Optional[str]' = None
     optional: 'Optional[bool]' = None
 
 
 @dataclass
 class Container(DictMixin):
-    """A single application container that you want to run within a pod.
+    r"""A single application container that you want to run within a pod.
 
       **parameters**
 
       * **name** ``str`` - Name of the container specified as a DNS_LABEL. Each container in a pod must
         have a unique name (DNS_LABEL). Cannot be updated.
       * **args** ``Optional[List[str]]`` - Arguments to the entrypoint. The container image's CMD is used if this is not
         provided. Variable references $(VAR_NAME) are expanded using the container's
@@ -853,30 +853,30 @@
     volumeDevices: 'Optional[List[VolumeDevice]]' = None
     volumeMounts: 'Optional[List[VolumeMount]]' = None
     workingDir: 'Optional[str]' = None
 
 
 @dataclass
 class ContainerImage(DictMixin):
-    """Describe a container image
+    r"""Describe a container image
 
       **parameters**
 
       * **names** ``Optional[List[str]]`` - Names by which this image is known. e.g.
         ["kubernetes.example/hyperkube:v1.0.7",
         "cloud-vendor.registry.example/cloud-vendor/hyperkube:v1.0.7"]
       * **sizeBytes** ``Optional[int]`` - The size of the image in bytes.
     """
     names: 'Optional[List[str]]' = None
     sizeBytes: 'Optional[int]' = None
 
 
 @dataclass
 class ContainerPort(DictMixin):
-    """ContainerPort represents a network port in a single container.
+    r"""ContainerPort represents a network port in a single container.
 
       **parameters**
 
       * **containerPort** ``int`` - Number of port to expose on the pod's IP address. This must be a valid port
         number, 0 < x < 65536.
       * **hostIP** ``Optional[str]`` - What host IP to bind the external port to.
       * **hostPort** ``Optional[int]`` - Number of port to expose on the host. If specified, this must be a valid port
@@ -892,30 +892,30 @@
     hostPort: 'Optional[int]' = None
     name: 'Optional[str]' = None
     protocol: 'Optional[str]' = None
 
 
 @dataclass
 class ContainerResizePolicy(DictMixin):
-    """ContainerResizePolicy represents resource resize policy for the container.
+    r"""ContainerResizePolicy represents resource resize policy for the container.
 
       **parameters**
 
       * **resourceName** ``str`` - Name of the resource to which this resource resize policy applies. Supported
         values: cpu, memory.
       * **restartPolicy** ``str`` - Restart policy to apply when specified resource is resized. If not specified,
         it defaults to NotRequired.
     """
     resourceName: 'str'
     restartPolicy: 'str'
 
 
 @dataclass
 class ContainerState(DictMixin):
-    """ContainerState holds a possible state of container. Only one of its members
+    r"""ContainerState holds a possible state of container. Only one of its members
       may be specified. If none of them is specified, the default one is
       ContainerStateWaiting.
 
       **parameters**
 
       * **running** ``Optional[ContainerStateRunning]`` - Details about a running container
       * **terminated** ``Optional[ContainerStateTerminated]`` - Details about a terminated container
@@ -924,26 +924,26 @@
     running: 'Optional[ContainerStateRunning]' = None
     terminated: 'Optional[ContainerStateTerminated]' = None
     waiting: 'Optional[ContainerStateWaiting]' = None
 
 
 @dataclass
 class ContainerStateRunning(DictMixin):
-    """ContainerStateRunning is a running state of a container.
+    r"""ContainerStateRunning is a running state of a container.
 
       **parameters**
 
       * **startedAt** ``Optional[meta_v1.Time]`` - Time at which the container was last (re-)started
     """
     startedAt: 'Optional[meta_v1.Time]' = None
 
 
 @dataclass
 class ContainerStateTerminated(DictMixin):
-    """ContainerStateTerminated is a terminated state of a container.
+    r"""ContainerStateTerminated is a terminated state of a container.
 
       **parameters**
 
       * **exitCode** ``int`` - Exit status from the last termination of the container
       * **containerID** ``Optional[str]`` - Container's ID in the format '<type>://<container_id>'
       * **finishedAt** ``Optional[meta_v1.Time]`` - Time at which the container last terminated
       * **message** ``Optional[str]`` - Message regarding the last termination of the container
@@ -958,28 +958,28 @@
     reason: 'Optional[str]' = None
     signal: 'Optional[int]' = None
     startedAt: 'Optional[meta_v1.Time]' = None
 
 
 @dataclass
 class ContainerStateWaiting(DictMixin):
-    """ContainerStateWaiting is a waiting state of a container.
+    r"""ContainerStateWaiting is a waiting state of a container.
 
       **parameters**
 
       * **message** ``Optional[str]`` - Message regarding why the container is not yet running.
       * **reason** ``Optional[str]`` - (brief) reason the container is not yet running.
     """
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class ContainerStatus(DictMixin):
-    """ContainerStatus contains details for the current status of this container.
+    r"""ContainerStatus contains details for the current status of this container.
 
       **parameters**
 
       * **image** ``str`` - Image is the name of container image that the container is running. The
         container image may not match the image used in the PodSpec, as it may have
         been resolved by the runtime. More info:
         https://kubernetes.io/docs/concepts/containers/images.
@@ -1034,38 +1034,38 @@
     started: 'Optional[bool]' = None
     state: 'Optional[ContainerState]' = None
     volumeMounts: 'Optional[List[VolumeMountStatus]]' = None
 
 
 @dataclass
 class DaemonEndpoint(DictMixin):
-    """DaemonEndpoint contains information about a single Daemon endpoint.
+    r"""DaemonEndpoint contains information about a single Daemon endpoint.
 
       **parameters**
 
       * **Port** ``int`` - Port number of the given endpoint.
     """
     Port: 'int'
 
 
 @dataclass
 class DownwardAPIProjection(DictMixin):
-    """Represents downward API info for projecting into a projected volume. Note that
+    r"""Represents downward API info for projecting into a projected volume. Note that
       this is identical to a downwardAPI volume source without the default mode.
 
       **parameters**
 
       * **items** ``Optional[List[DownwardAPIVolumeFile]]`` - Items is a list of DownwardAPIVolume file
     """
     items: 'Optional[List[DownwardAPIVolumeFile]]' = None
 
 
 @dataclass
 class DownwardAPIVolumeFile(DictMixin):
-    """DownwardAPIVolumeFile represents information to create the file containing the
+    r"""DownwardAPIVolumeFile represents information to create the file containing the
       pod field
 
       **parameters**
 
       * **path** ``str`` - Required: Path is  the relative path name of the file to be created. Must not
         be absolute or contain the '..' path. Must be utf-8 encoded. The first item of
         the relative path must not start with '..'
@@ -1085,15 +1085,15 @@
     fieldRef: 'Optional[ObjectFieldSelector]' = None
     mode: 'Optional[int]' = None
     resourceFieldRef: 'Optional[ResourceFieldSelector]' = None
 
 
 @dataclass
 class DownwardAPIVolumeSource(DictMixin):
-    """DownwardAPIVolumeSource represents a volume containing downward API info.
+    r"""DownwardAPIVolumeSource represents a volume containing downward API info.
       Downward API volumes support ownership management and SELinux relabeling.
 
       **parameters**
 
       * **defaultMode** ``Optional[int]`` - Optional: mode bits to use on created files by default. Must be a Optional:
         mode bits used to set permissions on created files by default. Must be an
         octal value between 0000 and 0777 or a decimal value between 0 and 511. YAML
@@ -1105,15 +1105,15 @@
     """
     defaultMode: 'Optional[int]' = None
     items: 'Optional[List[DownwardAPIVolumeFile]]' = None
 
 
 @dataclass
 class EmptyDirVolumeSource(DictMixin):
-    """Represents an empty directory for a pod. Empty directory volumes support
+    r"""Represents an empty directory for a pod. Empty directory volumes support
       ownership management and SELinux relabeling.
 
       **parameters**
 
       * **medium** ``Optional[str]`` - medium represents what type of storage medium should back this directory. The
         default is "" which means to use the node's default medium. Must be an empty
         string (default) or Memory. More info:
@@ -1127,15 +1127,15 @@
     """
     medium: 'Optional[str]' = None
     sizeLimit: 'Optional[resource.Quantity]' = None
 
 
 @dataclass
 class EndpointAddress(DictMixin):
-    """EndpointAddress is a tuple that describes single IP address.
+    r"""EndpointAddress is a tuple that describes single IP address.
 
       **parameters**
 
       * **ip** ``str`` - The IP of this endpoint. May not be loopback (127.0.0.0/8 or ::1), link-local
         (169.254.0.0/16 or fe80::/10), or link-local multicast (224.0.0.0/24 or
         ff02::/16).
       * **hostname** ``Optional[str]`` - The Hostname of this endpoint
@@ -1147,15 +1147,15 @@
     hostname: 'Optional[str]' = None
     nodeName: 'Optional[str]' = None
     targetRef: 'Optional[ObjectReference]' = None
 
 
 @dataclass
 class EndpointPort(DictMixin):
-    """EndpointPort is a tuple that describes a single port.
+    r"""EndpointPort is a tuple that describes a single port.
 
       **parameters**
 
       * **port** ``int`` - The port number of the endpoint.
       * **appProtocol** ``Optional[str]`` - The application protocol for this port. This is used as a hint for
         implementations to offer richer behavior for protocols that they understand.
         This field follows standard Kubernetes label syntax. Valid values are either:
@@ -1179,15 +1179,15 @@
     appProtocol: 'Optional[str]' = None
     name: 'Optional[str]' = None
     protocol: 'Optional[str]' = None
 
 
 @dataclass
 class EndpointSubset(DictMixin):
-    """EndpointSubset is a group of addresses with a common set of ports. The
+    r"""EndpointSubset is a group of addresses with a common set of ports. The
       expanded set of endpoints is the Cartesian product of Addresses x Ports. For
       example, given:
       
       	{
       	  Addresses: [{"ip": "10.10.1.1"}, {"ip": "10.10.2.2"}],
       	  Ports:     [{"name": "a", "port": 8675}, {"name": "b", "port": 309}]
       	}
@@ -1209,15 +1209,15 @@
     addresses: 'Optional[List[EndpointAddress]]' = None
     notReadyAddresses: 'Optional[List[EndpointAddress]]' = None
     ports: 'Optional[List[EndpointPort]]' = None
 
 
 @dataclass
 class Endpoints(DictMixin):
-    """Endpoints is a collection of endpoints that implement the actual service.
+    r"""Endpoints is a collection of endpoints that implement the actual service.
       Example:
       
       	 Name: "mysvc",
       	 Subsets: [
       	   {
       	     Addresses: [{"ip": "10.10.1.1"}, {"ip": "10.10.2.2"}],
       	     Ports: [{"name": "a", "port": 8675}, {"name": "b", "port": 309}]
@@ -1252,15 +1252,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     subsets: 'Optional[List[EndpointSubset]]' = None
 
 
 @dataclass
 class EndpointsList(DictMixin):
-    """EndpointsList is a list of endpoints.
+    r"""EndpointsList is a list of endpoints.
 
       **parameters**
 
       * **items** ``List[Endpoints]`` - List of endpoints.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -1276,15 +1276,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class EnvFromSource(DictMixin):
-    """EnvFromSource represents the source of a set of ConfigMaps
+    r"""EnvFromSource represents the source of a set of ConfigMaps
 
       **parameters**
 
       * **configMapRef** ``Optional[ConfigMapEnvSource]`` - The ConfigMap to select from
       * **prefix** ``Optional[str]`` - An optional identifier to prepend to each key in the ConfigMap. Must be a
         C_IDENTIFIER.
       * **secretRef** ``Optional[SecretEnvSource]`` - The Secret to select from
@@ -1292,15 +1292,15 @@
     configMapRef: 'Optional[ConfigMapEnvSource]' = None
     prefix: 'Optional[str]' = None
     secretRef: 'Optional[SecretEnvSource]' = None
 
 
 @dataclass
 class EnvVar(DictMixin):
-    """EnvVar represents an environment variable present in a Container.
+    r"""EnvVar represents an environment variable present in a Container.
 
       **parameters**
 
       * **name** ``str`` - Name of the environment variable. Must be a C_IDENTIFIER.
       * **value** ``Optional[str]`` - Variable references $(VAR_NAME) are expanded using the previously defined
         environment variables in the container and any service environment variables.
         If a variable cannot be resolved, the reference in the input string will be
@@ -1314,15 +1314,15 @@
     name: 'str'
     value: 'Optional[str]' = None
     valueFrom: 'Optional[EnvVarSource]' = None
 
 
 @dataclass
 class EnvVarSource(DictMixin):
-    """EnvVarSource represents a source for the value of an EnvVar.
+    r"""EnvVarSource represents a source for the value of an EnvVar.
 
       **parameters**
 
       * **configMapKeyRef** ``Optional[ConfigMapKeySelector]`` - Selects a key of a ConfigMap.
       * **fieldRef** ``Optional[ObjectFieldSelector]`` - Selects a field of the pod: supports metadata.name, metadata.namespace,
         `metadata.labels['<KEY>']`, `metadata.annotations['<KEY>']`, spec.nodeName,
         spec.serviceAccountName, status.hostIP, status.podIP, status.podIPs.
@@ -1335,15 +1335,15 @@
     fieldRef: 'Optional[ObjectFieldSelector]' = None
     resourceFieldRef: 'Optional[ResourceFieldSelector]' = None
     secretKeyRef: 'Optional[SecretKeySelector]' = None
 
 
 @dataclass
 class EphemeralContainer(DictMixin):
-    """An EphemeralContainer is a temporary container that you may add to an existing
+    r"""An EphemeralContainer is a temporary container that you may add to an existing
       Pod for user-initiated activities such as debugging. Ephemeral containers have
       no resource or scheduling guarantees, and they will not be restarted when they
       exit or when a Pod is removed or restarted. The kubelet may evict a Pod if an
       ephemeral container causes the Pod to exceed its resource allocation.
       
       To add an ephemeral container, use the ephemeralcontainers subresource of an
       existing Pod. Ephemeral containers may not be removed or restarted.
@@ -1460,15 +1460,15 @@
     volumeDevices: 'Optional[List[VolumeDevice]]' = None
     volumeMounts: 'Optional[List[VolumeMount]]' = None
     workingDir: 'Optional[str]' = None
 
 
 @dataclass
 class EphemeralVolumeSource(DictMixin):
-    """Represents an ephemeral volume that is handled by a normal storage driver.
+    r"""Represents an ephemeral volume that is handled by a normal storage driver.
 
       **parameters**
 
       * **volumeClaimTemplate** ``Optional[PersistentVolumeClaimTemplate]`` - Will be used to create a stand-alone PVC to provision the volume. The pod in
         which this EphemeralVolumeSource is embedded will be the owner of the PVC,
         i.e. the PVC will be deleted together with the pod.  The name of the PVC will
         be `<pod name>-<volume name>` where `<volume name>` is the name from the
@@ -1485,15 +1485,15 @@
         Required, must not be nil.
     """
     volumeClaimTemplate: 'Optional[PersistentVolumeClaimTemplate]' = None
 
 
 @dataclass
 class Event(DictMixin):
-    """Event is a report of an event somewhere in the cluster.  Events have a limited
+    r"""Event is a report of an event somewhere in the cluster.  Events have a limited
       retention time and triggers and messages may evolve with time.  Event
       consumers should not rely on the timing of an event with a given Reason
       reflecting a consistent underlying trigger, or the continued existence of
       events with that Reason.  Events should be treated as informative,
       best-effort, supplemental data.
 
       **parameters**
@@ -1544,15 +1544,15 @@
     series: 'Optional[EventSeries]' = None
     source: 'Optional[EventSource]' = None
     type: 'Optional[str]' = None
 
 
 @dataclass
 class EventList(DictMixin):
-    """EventList is a list of events.
+    r"""EventList is a list of events.
 
       **parameters**
 
       * **items** ``List[Event]`` - List of events
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -1568,42 +1568,42 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class EventSeries(DictMixin):
-    """EventSeries contain information on series of events, i.e. thing that was/is
+    r"""EventSeries contain information on series of events, i.e. thing that was/is
       happening continuously for some time.
 
       **parameters**
 
       * **count** ``Optional[int]`` - Number of occurrences in this series up to the last heartbeat time
       * **lastObservedTime** ``Optional[meta_v1.MicroTime]`` - Time of the last occurrence observed
     """
     count: 'Optional[int]' = None
     lastObservedTime: 'Optional[meta_v1.MicroTime]' = None
 
 
 @dataclass
 class EventSource(DictMixin):
-    """EventSource contains information for an event.
+    r"""EventSource contains information for an event.
 
       **parameters**
 
       * **component** ``Optional[str]`` - Component from which the event is generated.
       * **host** ``Optional[str]`` - Node name on which the event is generated.
     """
     component: 'Optional[str]' = None
     host: 'Optional[str]' = None
 
 
 @dataclass
 class ExecAction(DictMixin):
-    """ExecAction describes a "run in container" action.
+    r"""ExecAction describes a "run in container" action.
 
       **parameters**
 
       * **command** ``Optional[List[str]]`` - Command is the command line to execute inside the container, the working
         directory for the command  is root ('/') in the container's filesystem. The
         command is simply exec'd, it is not run inside a shell, so traditional shell
         instructions ('|', etc) won't work. To use a shell, you need to explicitly
@@ -1611,15 +1611,15 @@
         non-zero is unhealthy.
     """
     command: 'Optional[List[str]]' = None
 
 
 @dataclass
 class FCVolumeSource(DictMixin):
-    """Represents a Fibre Channel volume. Fibre Channel volumes can only be mounted
+    r"""Represents a Fibre Channel volume. Fibre Channel volumes can only be mounted
       as read/write once. Fibre Channel volumes support ownership management and
       SELinux relabeling.
 
       **parameters**
 
       * **fsType** ``Optional[str]`` - fsType is the filesystem type to mount. Must be a filesystem type supported by
         the host operating system. Ex. "ext4", "xfs", "ntfs". Implicitly inferred to
@@ -1636,15 +1636,15 @@
     readOnly: 'Optional[bool]' = None
     targetWWNs: 'Optional[List[str]]' = None
     wwids: 'Optional[List[str]]' = None
 
 
 @dataclass
 class FlexPersistentVolumeSource(DictMixin):
-    """FlexPersistentVolumeSource represents a generic persistent volume resource
+    r"""FlexPersistentVolumeSource represents a generic persistent volume resource
       that is provisioned/attached using an exec based plugin.
 
       **parameters**
 
       * **driver** ``str`` - driver is the name of the driver to use for this volume.
       * **fsType** ``Optional[str]`` - fsType is the Filesystem type to mount. Must be a filesystem type supported by
         the host operating system. Ex. "ext4", "xfs", "ntfs". The default filesystem
@@ -1662,15 +1662,15 @@
     options: 'Optional[dict]' = None
     readOnly: 'Optional[bool]' = None
     secretRef: 'Optional[SecretReference]' = None
 
 
 @dataclass
 class FlexVolumeSource(DictMixin):
-    """FlexVolume represents a generic volume resource that is provisioned/attached
+    r"""FlexVolume represents a generic volume resource that is provisioned/attached
       using an exec based plugin.
 
       **parameters**
 
       * **driver** ``str`` - driver is the name of the driver to use for this volume.
       * **fsType** ``Optional[str]`` - fsType is the filesystem type to mount. Must be a filesystem type supported by
         the host operating system. Ex. "ext4", "xfs", "ntfs". The default filesystem
@@ -1688,15 +1688,15 @@
     options: 'Optional[dict]' = None
     readOnly: 'Optional[bool]' = None
     secretRef: 'Optional[LocalObjectReference]' = None
 
 
 @dataclass
 class FlockerVolumeSource(DictMixin):
-    """Represents a Flocker volume mounted by the Flocker agent. One and only one of
+    r"""Represents a Flocker volume mounted by the Flocker agent. One and only one of
       datasetName and datasetUUID should be set. Flocker volumes do not support
       ownership management or SELinux relabeling.
 
       **parameters**
 
       * **datasetName** ``Optional[str]`` - datasetName is Name of the dataset stored as metadata -> name on the dataset
         for Flocker should be considered as deprecated
@@ -1705,15 +1705,15 @@
     """
     datasetName: 'Optional[str]' = None
     datasetUUID: 'Optional[str]' = None
 
 
 @dataclass
 class GCEPersistentDiskVolumeSource(DictMixin):
-    """Represents a Persistent Disk resource in Google Compute Engine.
+    r"""Represents a Persistent Disk resource in Google Compute Engine.
       
       A GCE PD must exist before mounting to a container. The disk must also be in
       the same GCE project and zone as the kubelet. A GCE PD can only be mounted as
       read/write once or read-only many times. GCE PDs support ownership management
       and SELinux relabeling.
 
       **parameters**
@@ -1738,30 +1738,30 @@
     fsType: 'Optional[str]' = None
     partition: 'Optional[int]' = None
     readOnly: 'Optional[bool]' = None
 
 
 @dataclass
 class GRPCAction(DictMixin):
-    """
+    r"""
 
       **parameters**
 
       * **port** ``int`` - Port number of the gRPC service. Number must be in the range 1 to 65535.
       * **service** ``Optional[str]`` - Service is the name of the service to place in the gRPC HealthCheckRequest
         (see https://github.com/grpc/grpc/blob/master/doc/health-checking.md).
         If this is not specified, the default behavior is defined by gRPC.
     """
     port: 'int'
     service: 'Optional[str]' = None
 
 
 @dataclass
 class GitRepoVolumeSource(DictMixin):
-    """Represents a volume that is populated with the contents of a git repository.
+    r"""Represents a volume that is populated with the contents of a git repository.
       Git repo volumes do not support ownership management. Git repo volumes support
       SELinux relabeling.
       
       DEPRECATED: GitRepo is deprecated. To provision a container with a git repo,
       mount an EmptyDir into an InitContainer that clones the repo using git, then
       mount the EmptyDir into the Pod's container.
 
@@ -1777,15 +1777,15 @@
     repository: 'str'
     directory: 'Optional[str]' = None
     revision: 'Optional[str]' = None
 
 
 @dataclass
 class GlusterfsPersistentVolumeSource(DictMixin):
-    """Represents a Glusterfs mount that lasts the lifetime of a pod. Glusterfs
+    r"""Represents a Glusterfs mount that lasts the lifetime of a pod. Glusterfs
       volumes do not support ownership management or SELinux relabeling.
 
       **parameters**
 
       * **endpoints** ``str`` - endpoints is the endpoint name that details Glusterfs topology. More info:
         https://examples.k8s.io/volumes/glusterfs/README.md#create-a-pod
       * **path** ``str`` - path is the Glusterfs volume path. More info:
@@ -1802,15 +1802,15 @@
     path: 'str'
     endpointsNamespace: 'Optional[str]' = None
     readOnly: 'Optional[bool]' = None
 
 
 @dataclass
 class GlusterfsVolumeSource(DictMixin):
-    """Represents a Glusterfs mount that lasts the lifetime of a pod. Glusterfs
+    r"""Represents a Glusterfs mount that lasts the lifetime of a pod. Glusterfs
       volumes do not support ownership management or SELinux relabeling.
 
       **parameters**
 
       * **endpoints** ``str`` - endpoints is the endpoint name that details Glusterfs topology. More info:
         https://examples.k8s.io/volumes/glusterfs/README.md#create-a-pod
       * **path** ``str`` - path is the Glusterfs volume path. More info:
@@ -1822,15 +1822,15 @@
     endpoints: 'str'
     path: 'str'
     readOnly: 'Optional[bool]' = None
 
 
 @dataclass
 class HTTPGetAction(DictMixin):
-    """HTTPGetAction describes an action based on HTTP Get requests.
+    r"""HTTPGetAction describes an action based on HTTP Get requests.
 
       **parameters**
 
       * **port** ``util_intstr.IntOrString`` - Name or number of the port to access on the container. Number must be in the
         range 1 to 65535. Name must be an IANA_SVC_NAME.
       * **host** ``Optional[str]`` - Host name to connect to, defaults to the pod IP. You probably want to set
         "Host" in httpHeaders instead.
@@ -1843,54 +1843,54 @@
     httpHeaders: 'Optional[List[HTTPHeader]]' = None
     path: 'Optional[str]' = None
     scheme: 'Optional[str]' = None
 
 
 @dataclass
 class HTTPHeader(DictMixin):
-    """HTTPHeader describes a custom header to be used in HTTP probes
+    r"""HTTPHeader describes a custom header to be used in HTTP probes
 
       **parameters**
 
       * **name** ``str`` - The header field name. This will be canonicalized upon output, so case-variant
         names will be understood as the same header.
       * **value** ``str`` - The header field value
     """
     name: 'str'
     value: 'str'
 
 
 @dataclass
 class HostAlias(DictMixin):
-    """HostAlias holds the mapping between IP and hostnames that will be injected as
+    r"""HostAlias holds the mapping between IP and hostnames that will be injected as
       an entry in the pod's hosts file.
 
       **parameters**
 
       * **hostnames** ``Optional[List[str]]`` - Hostnames for the above IP address.
       * **ip** ``Optional[str]`` - IP address of the host file entry.
     """
     hostnames: 'Optional[List[str]]' = None
     ip: 'Optional[str]' = None
 
 
 @dataclass
 class HostIP(DictMixin):
-    """HostIP represents a single IP address allocated to the host.
+    r"""HostIP represents a single IP address allocated to the host.
 
       **parameters**
 
       * **ip** ``Optional[str]`` - IP is the IP address assigned to the host
     """
     ip: 'Optional[str]' = None
 
 
 @dataclass
 class HostPathVolumeSource(DictMixin):
-    """Represents a host path mapped into a pod. Host path volumes do not support
+    r"""Represents a host path mapped into a pod. Host path volumes do not support
       ownership management or SELinux relabeling.
 
       **parameters**
 
       * **path** ``str`` - path of the directory on the host. If the path is a symlink, it will follow
         the link to the real path. More info:
         https://kubernetes.io/docs/concepts/storage/volumes#hostpath
@@ -1899,15 +1899,15 @@
     """
     path: 'str'
     type: 'Optional[str]' = None
 
 
 @dataclass
 class ISCSIPersistentVolumeSource(DictMixin):
-    """ISCSIPersistentVolumeSource represents an ISCSI disk. ISCSI volumes can only
+    r"""ISCSIPersistentVolumeSource represents an ISCSI disk. ISCSI volumes can only
       be mounted as read/write once. ISCSI volumes support ownership management and
       SELinux relabeling.
 
       **parameters**
 
       * **iqn** ``str`` - iqn is Target iSCSI Qualified Name.
       * **lun** ``int`` - lun is iSCSI Target Lun number.
@@ -1944,15 +1944,15 @@
     portals: 'Optional[List[str]]' = None
     readOnly: 'Optional[bool]' = None
     secretRef: 'Optional[SecretReference]' = None
 
 
 @dataclass
 class ISCSIVolumeSource(DictMixin):
-    """Represents an ISCSI disk. ISCSI volumes can only be mounted as read/write
+    r"""Represents an ISCSI disk. ISCSI volumes can only be mounted as read/write
       once. ISCSI volumes support ownership management and SELinux relabeling.
 
       **parameters**
 
       * **iqn** ``str`` - iqn is the target iSCSI Qualified Name.
       * **lun** ``int`` - lun represents iSCSI Target Lun number.
       * **targetPortal** ``str`` - targetPortal is iSCSI Target Portal. The Portal is either an IP or
@@ -1988,15 +1988,15 @@
     portals: 'Optional[List[str]]' = None
     readOnly: 'Optional[bool]' = None
     secretRef: 'Optional[LocalObjectReference]' = None
 
 
 @dataclass
 class KeyToPath(DictMixin):
-    """Maps a string key to a path within a volume.
+    r"""Maps a string key to a path within a volume.
 
       **parameters**
 
       * **key** ``str`` - key is the key to project.
       * **path** ``str`` - path is the relative path of the file to map the key to. May not be an
         absolute path. May not contain the path element '..'. May not start with the
         string '..'.
@@ -2010,15 +2010,15 @@
     key: 'str'
     path: 'str'
     mode: 'Optional[int]' = None
 
 
 @dataclass
 class Lifecycle(DictMixin):
-    """Lifecycle describes actions that the management system should take in response
+    r"""Lifecycle describes actions that the management system should take in response
       to container lifecycle events. For the PostStart and PreStop lifecycle
       handlers, management of the container blocks until the action is complete,
       unless the container process fails, in which case the handler is aborted.
 
       **parameters**
 
       * **postStart** ``Optional[LifecycleHandler]`` - PostStart is called immediately after a container is created. If the handler
@@ -2039,15 +2039,15 @@
     """
     postStart: 'Optional[LifecycleHandler]' = None
     preStop: 'Optional[LifecycleHandler]' = None
 
 
 @dataclass
 class LifecycleHandler(DictMixin):
-    """LifecycleHandler defines a specific action that should be taken in a lifecycle
+    r"""LifecycleHandler defines a specific action that should be taken in a lifecycle
       hook. One and only one of the fields, except TCPSocket must be specified.
 
       **parameters**
 
       * **exec** ``Optional[ExecAction]`` - Exec specifies the action to take.
       * **httpGet** ``Optional[HTTPGetAction]`` - HTTPGet specifies the http request to perform.
       * **sleep** ``Optional[SleepAction]`` - Sleep represents the duration that the container should sleep before being
@@ -2060,15 +2060,15 @@
     httpGet: 'Optional[HTTPGetAction]' = None
     sleep: 'Optional[SleepAction]' = None
     tcpSocket: 'Optional[TCPSocketAction]' = None
 
 
 @dataclass
 class LimitRange(DictMixin):
-    """LimitRange sets resource usage limits for each kind of resource in a
+    r"""LimitRange sets resource usage limits for each kind of resource in a
       Namespace.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -2086,15 +2086,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[LimitRangeSpec]' = None
 
 
 @dataclass
 class LimitRangeItem(DictMixin):
-    """LimitRangeItem defines a min/max usage limit for any resource that matches on
+    r"""LimitRangeItem defines a min/max usage limit for any resource that matches on
       kind.
 
       **parameters**
 
       * **type** ``str`` - Type of resource that this limit applies to.
       * **default** ``Optional[dict]`` - Default resource requirement limit value by resource name if resource limit is
         omitted.
@@ -2113,15 +2113,15 @@
     max: 'Optional[dict]' = None
     maxLimitRequestRatio: 'Optional[dict]' = None
     min: 'Optional[dict]' = None
 
 
 @dataclass
 class LimitRangeList(DictMixin):
-    """LimitRangeList is a list of LimitRange items.
+    r"""LimitRangeList is a list of LimitRange items.
 
       **parameters**
 
       * **items** ``List[LimitRange]`` - Items is a list of LimitRange objects. More info:
         https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -2138,26 +2138,26 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class LimitRangeSpec(DictMixin):
-    """LimitRangeSpec defines a min/max usage limit for resources that match on kind.
+    r"""LimitRangeSpec defines a min/max usage limit for resources that match on kind.
 
       **parameters**
 
       * **limits** ``List[LimitRangeItem]`` - Limits is the list of LimitRangeItem objects that are enforced.
     """
     limits: 'List[LimitRangeItem]'
 
 
 @dataclass
 class LoadBalancerIngress(DictMixin):
-    """LoadBalancerIngress represents the status of a load-balancer ingress point:
+    r"""LoadBalancerIngress represents the status of a load-balancer ingress point:
       traffic intended for the service should be sent to an ingress point.
 
       **parameters**
 
       * **hostname** ``Optional[str]`` - Hostname is set for load-balancer ingress points that are DNS based (typically
         AWS load-balancers)
       * **ip** ``Optional[str]`` - IP is set for load-balancer ingress points that are IP based (typically GCE or
@@ -2176,40 +2176,40 @@
     ip: 'Optional[str]' = None
     ipMode: 'Optional[str]' = None
     ports: 'Optional[List[PortStatus]]' = None
 
 
 @dataclass
 class LoadBalancerStatus(DictMixin):
-    """LoadBalancerStatus represents the status of a load-balancer.
+    r"""LoadBalancerStatus represents the status of a load-balancer.
 
       **parameters**
 
       * **ingress** ``Optional[List[LoadBalancerIngress]]`` - Ingress is a list containing ingress points for the load-balancer. Traffic
         intended for the service should be sent to these ingress points.
     """
     ingress: 'Optional[List[LoadBalancerIngress]]' = None
 
 
 @dataclass
 class LocalObjectReference(DictMixin):
-    """LocalObjectReference contains enough information to let you locate the
+    r"""LocalObjectReference contains enough information to let you locate the
       referenced object inside the same namespace.
 
       **parameters**
 
       * **name** ``Optional[str]`` - Name of the referent. More info:
         https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names
     """
     name: 'Optional[str]' = None
 
 
 @dataclass
 class LocalVolumeSource(DictMixin):
-    """Local represents directly-attached storage with node affinity (Beta feature)
+    r"""Local represents directly-attached storage with node affinity (Beta feature)
 
       **parameters**
 
       * **path** ``str`` - path of the full path to the volume on the node. It can be either a directory
         or block device (disk, partition, ...).
       * **fsType** ``Optional[str]`` - fsType is the filesystem type to mount. It applies only when the Path is a
         block device. Must be a filesystem type supported by the host operating
@@ -2218,15 +2218,15 @@
     """
     path: 'str'
     fsType: 'Optional[str]' = None
 
 
 @dataclass
 class ModifyVolumeStatus(DictMixin):
-    """ModifyVolumeStatus represents the status object of ControllerModifyVolume
+    r"""ModifyVolumeStatus represents the status object of ControllerModifyVolume
       operation
 
       **parameters**
 
       * **status** ``str`` - status is the status of the ControllerModifyVolume operation. It can be in any
         of following states:
          - Pending
@@ -2246,15 +2246,15 @@
     """
     status: 'str'
     targetVolumeAttributesClassName: 'Optional[str]' = None
 
 
 @dataclass
 class NFSVolumeSource(DictMixin):
-    """Represents an NFS mount that lasts the lifetime of a pod. NFS volumes do not
+    r"""Represents an NFS mount that lasts the lifetime of a pod. NFS volumes do not
       support ownership management or SELinux relabeling.
 
       **parameters**
 
       * **path** ``str`` - path that is exported by the NFS server. More info:
         https://kubernetes.io/docs/concepts/storage/volumes#nfs
       * **server** ``str`` - server is the hostname or IP address of the NFS server. More info:
@@ -2266,15 +2266,15 @@
     path: 'str'
     server: 'str'
     readOnly: 'Optional[bool]' = None
 
 
 @dataclass
 class Namespace(DictMixin):
-    """Namespace provides a scope for Names. Use of multiple namespaces is optional.
+    r"""Namespace provides a scope for Names. Use of multiple namespaces is optional.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -2294,15 +2294,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[NamespaceSpec]' = None
     status: 'Optional[NamespaceStatus]' = None
 
 
 @dataclass
 class NamespaceCondition(DictMixin):
-    """NamespaceCondition contains details about state of namespace.
+    r"""NamespaceCondition contains details about state of namespace.
 
       **parameters**
 
       * **status** ``str`` - Status of the condition, one of True, False, Unknown.
       * **type** ``str`` - Type of namespace controller condition.
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - 
       * **message** ``Optional[str]`` - 
@@ -2313,15 +2313,15 @@
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class NamespaceList(DictMixin):
-    """NamespaceList is a list of Namespaces.
+    r"""NamespaceList is a list of Namespaces.
 
       **parameters**
 
       * **items** ``List[Namespace]`` - Items is the list of Namespace objects in the list. More info:
         https://kubernetes.io/docs/concepts/overview/working-with-objects/namespaces/
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -2338,42 +2338,42 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class NamespaceSpec(DictMixin):
-    """NamespaceSpec describes the attributes on a Namespace.
+    r"""NamespaceSpec describes the attributes on a Namespace.
 
       **parameters**
 
       * **finalizers** ``Optional[List[str]]`` - Finalizers is an opaque list of values that must be empty to permanently
         remove object from storage. More info:
         https://kubernetes.io/docs/tasks/administer-cluster/namespaces/
     """
     finalizers: 'Optional[List[str]]' = None
 
 
 @dataclass
 class NamespaceStatus(DictMixin):
-    """NamespaceStatus is information about the current status of a Namespace.
+    r"""NamespaceStatus is information about the current status of a Namespace.
 
       **parameters**
 
       * **conditions** ``Optional[List[NamespaceCondition]]`` - Represents the latest available observations of a namespace's current state.
       * **phase** ``Optional[str]`` - Phase is the current lifecycle phase of the namespace. More info:
         https://kubernetes.io/docs/tasks/administer-cluster/namespaces/
     """
     conditions: 'Optional[List[NamespaceCondition]]' = None
     phase: 'Optional[str]' = None
 
 
 @dataclass
 class Node(DictMixin):
-    """Node is a worker node in Kubernetes. Each node will have a unique identifier
+    r"""Node is a worker node in Kubernetes. Each node will have a unique identifier
       in the cache (i.e. in etcd).
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -2395,28 +2395,28 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[NodeSpec]' = None
     status: 'Optional[NodeStatus]' = None
 
 
 @dataclass
 class NodeAddress(DictMixin):
-    """NodeAddress contains information for the node's address.
+    r"""NodeAddress contains information for the node's address.
 
       **parameters**
 
       * **address** ``str`` - The node address.
       * **type** ``str`` - Node address type, one of Hostname, ExternalIP or InternalIP.
     """
     address: 'str'
     type: 'str'
 
 
 @dataclass
 class NodeAffinity(DictMixin):
-    """Node affinity is a group of node affinity scheduling rules.
+    r"""Node affinity is a group of node affinity scheduling rules.
 
       **parameters**
 
       * **preferredDuringSchedulingIgnoredDuringExecution** ``Optional[List[PreferredSchedulingTerm]]`` - The scheduler will prefer to schedule pods to nodes that satisfy the affinity
         expressions specified by this field, but it may choose a node that violates
         one or more of the expressions. The node that is most preferred is the one
         with the greatest sum of weights, i.e. for each node that meets all of the
@@ -2432,15 +2432,15 @@
     """
     preferredDuringSchedulingIgnoredDuringExecution: 'Optional[List[PreferredSchedulingTerm]]' = None
     requiredDuringSchedulingIgnoredDuringExecution: 'Optional[NodeSelector]' = None
 
 
 @dataclass
 class NodeCondition(DictMixin):
-    """NodeCondition contains condition information for a node.
+    r"""NodeCondition contains condition information for a node.
 
       **parameters**
 
       * **status** ``str`` - Status of the condition, one of True, False, Unknown.
       * **type** ``str`` - Type of node condition.
       * **lastHeartbeatTime** ``Optional[meta_v1.Time]`` - Last time we got an update on a given condition.
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - Last time the condition transit from one status to another.
@@ -2453,28 +2453,28 @@
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class NodeConfigSource(DictMixin):
-    """NodeConfigSource specifies a source of node configuration. Exactly one
+    r"""NodeConfigSource specifies a source of node configuration. Exactly one
       subfield (excluding metadata) must be non-nil. This API is deprecated since
       1.22
 
       **parameters**
 
       * **configMap** ``Optional[ConfigMapNodeConfigSource]`` - ConfigMap is a reference to a Node's ConfigMap
     """
     configMap: 'Optional[ConfigMapNodeConfigSource]' = None
 
 
 @dataclass
 class NodeConfigStatus(DictMixin):
-    """NodeConfigStatus describes the status of the config assigned by
+    r"""NodeConfigStatus describes the status of the config assigned by
       Node.Spec.ConfigSource.
 
       **parameters**
 
       * **active** ``Optional[NodeConfigSource]`` - Active reports the checkpointed config the node is actively using. Active will
         represent either the current version of the Assigned config, or the current
         LastKnownGood config, depending on whether attempting to use the Assigned
@@ -2517,26 +2517,26 @@
     assigned: 'Optional[NodeConfigSource]' = None
     error: 'Optional[str]' = None
     lastKnownGood: 'Optional[NodeConfigSource]' = None
 
 
 @dataclass
 class NodeDaemonEndpoints(DictMixin):
-    """NodeDaemonEndpoints lists ports opened by daemons running on the Node.
+    r"""NodeDaemonEndpoints lists ports opened by daemons running on the Node.
 
       **parameters**
 
       * **kubeletEndpoint** ``Optional[DaemonEndpoint]`` - Endpoint on which Kubelet is listening.
     """
     kubeletEndpoint: 'Optional[DaemonEndpoint]' = None
 
 
 @dataclass
 class NodeList(DictMixin):
-    """NodeList is the whole list of all Nodes which have been registered with
+    r"""NodeList is the whole list of all Nodes which have been registered with
       master.
 
       **parameters**
 
       * **items** ``List[Node]`` - List of nodes
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -2553,53 +2553,53 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class NodeRuntimeHandler(DictMixin):
-    """NodeRuntimeHandler is a set of runtime handler information.
+    r"""NodeRuntimeHandler is a set of runtime handler information.
 
       **parameters**
 
       * **features** ``Optional[NodeRuntimeHandlerFeatures]`` - Supported features.
       * **name** ``Optional[str]`` - Runtime handler name. Empty for the default runtime handler.
     """
     features: 'Optional[NodeRuntimeHandlerFeatures]' = None
     name: 'Optional[str]' = None
 
 
 @dataclass
 class NodeRuntimeHandlerFeatures(DictMixin):
-    """NodeRuntimeHandlerFeatures is a set of runtime features.
+    r"""NodeRuntimeHandlerFeatures is a set of runtime features.
 
       **parameters**
 
       * **recursiveReadOnlyMounts** ``Optional[bool]`` - RecursiveReadOnlyMounts is set to true if the runtime handler supports
         RecursiveReadOnlyMounts.
     """
     recursiveReadOnlyMounts: 'Optional[bool]' = None
 
 
 @dataclass
 class NodeSelector(DictMixin):
-    """A node selector represents the union of the results of one or more label
+    r"""A node selector represents the union of the results of one or more label
       queries over a set of nodes; that is, it represents the OR of the selectors
       represented by the node selector terms.
 
       **parameters**
 
       * **nodeSelectorTerms** ``List[NodeSelectorTerm]`` - Required. A list of node selector terms. The terms are ORed.
     """
     nodeSelectorTerms: 'List[NodeSelectorTerm]'
 
 
 @dataclass
 class NodeSelectorRequirement(DictMixin):
-    """A node selector requirement is a selector that contains values, a key, and an
+    r"""A node selector requirement is a selector that contains values, a key, and an
       operator that relates the key and values.
 
       **parameters**
 
       * **key** ``str`` - The label key that the selector applies to.
       * **operator** ``str`` - Represents a key's relationship to a set of values. Valid operators are In,
         NotIn, Exists, DoesNotExist. Gt, and Lt.
@@ -2612,30 +2612,30 @@
     key: 'str'
     operator: 'str'
     values: 'Optional[List[str]]' = None
 
 
 @dataclass
 class NodeSelectorTerm(DictMixin):
-    """A null or empty node selector term matches no objects. The requirements of
+    r"""A null or empty node selector term matches no objects. The requirements of
       them are ANDed. The TopologySelectorTerm type implements a subset of the
       NodeSelectorTerm.
 
       **parameters**
 
       * **matchExpressions** ``Optional[List[NodeSelectorRequirement]]`` - A list of node selector requirements by node's labels.
       * **matchFields** ``Optional[List[NodeSelectorRequirement]]`` - A list of node selector requirements by node's fields.
     """
     matchExpressions: 'Optional[List[NodeSelectorRequirement]]' = None
     matchFields: 'Optional[List[NodeSelectorRequirement]]' = None
 
 
 @dataclass
 class NodeSpec(DictMixin):
-    """NodeSpec describes the attributes that a node is created with.
+    r"""NodeSpec describes the attributes that a node is created with.
 
       **parameters**
 
       * **configSource** ``Optional[NodeConfigSource]`` - Deprecated: Previously used to specify the source of the node's configuration
         for the DynamicKubeletConfig feature. This feature is removed.
       * **externalID** ``Optional[str]`` - Deprecated. Not all kubelets will set this field. Remove field after 1.13.
         see: https://issues.k8s.io/61966
@@ -2657,15 +2657,15 @@
     providerID: 'Optional[str]' = None
     taints: 'Optional[List[Taint]]' = None
     unschedulable: 'Optional[bool]' = None
 
 
 @dataclass
 class NodeStatus(DictMixin):
-    """NodeStatus is information about the current status of a node.
+    r"""NodeStatus is information about the current status of a node.
 
       **parameters**
 
       * **addresses** ``Optional[List[NodeAddress]]`` - List of addresses reachable to the node. Queried from cloud provider, if
         available. More info:
         https://kubernetes.io/docs/concepts/nodes/node/#addresses Note: This field is
         declared as mergeable, but the merge key is not sufficiently unique, which can
@@ -2706,15 +2706,15 @@
     runtimeHandlers: 'Optional[List[NodeRuntimeHandler]]' = None
     volumesAttached: 'Optional[List[AttachedVolume]]' = None
     volumesInUse: 'Optional[List[str]]' = None
 
 
 @dataclass
 class NodeSystemInfo(DictMixin):
-    """NodeSystemInfo is a set of ids/uuids to uniquely identify the node.
+    r"""NodeSystemInfo is a set of ids/uuids to uniquely identify the node.
 
       **parameters**
 
       * **architecture** ``str`` - The Architecture reported by the node
       * **bootID** ``str`` - Boot ID reported by the node.
       * **containerRuntimeVersion** ``str`` - ContainerRuntime Version reported by the node through runtime remote API (e.g.
         containerd://1.4.2).
@@ -2742,28 +2742,28 @@
     operatingSystem: 'str'
     osImage: 'str'
     systemUUID: 'str'
 
 
 @dataclass
 class ObjectFieldSelector(DictMixin):
-    """ObjectFieldSelector selects an APIVersioned field of an object.
+    r"""ObjectFieldSelector selects an APIVersioned field of an object.
 
       **parameters**
 
       * **fieldPath** ``str`` - Path of the field to select in the specified API version.
       * **apiVersion** ``Optional[str]`` - Version of the schema the FieldPath is written in terms of, defaults to "v1".
     """
     fieldPath: 'str'
     apiVersion: 'Optional[str]' = None
 
 
 @dataclass
 class ObjectReference(DictMixin):
-    """ObjectReference contains enough information to let you inspect or modify the
+    r"""ObjectReference contains enough information to let you inspect or modify the
       referred object.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - API version of the referent.
       * **fieldPath** ``Optional[str]`` - If referring to a piece of an object instead of an entire object, this string
         should contain a valid JSON/Go field access statement, such as
@@ -2791,15 +2791,15 @@
     namespace: 'Optional[str]' = None
     resourceVersion: 'Optional[str]' = None
     uid: 'Optional[str]' = None
 
 
 @dataclass
 class PersistentVolume(DictMixin):
-    """PersistentVolume (PV) is a storage resource provisioned by an administrator.
+    r"""PersistentVolume (PV) is a storage resource provisioned by an administrator.
       It is analogous to a node. More info:
       https://kubernetes.io/docs/concepts/storage/persistent-volumes
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -2823,15 +2823,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[PersistentVolumeSpec]' = None
     status: 'Optional[PersistentVolumeStatus]' = None
 
 
 @dataclass
 class PersistentVolumeClaim(DictMixin):
-    """PersistentVolumeClaim is a user's request for and claim to a persistent volume
+    r"""PersistentVolumeClaim is a user's request for and claim to a persistent volume
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -2853,15 +2853,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[PersistentVolumeClaimSpec]' = None
     status: 'Optional[PersistentVolumeClaimStatus]' = None
 
 
 @dataclass
 class PersistentVolumeClaimCondition(DictMixin):
-    """PersistentVolumeClaimCondition contains details about state of pvc
+    r"""PersistentVolumeClaimCondition contains details about state of pvc
 
       **parameters**
 
       * **status** ``str`` - 
       * **type** ``str`` - 
       * **lastProbeTime** ``Optional[meta_v1.Time]`` - lastProbeTime is the time we probed the condition.
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - lastTransitionTime is the time the condition transitioned from one status to
@@ -2878,15 +2878,15 @@
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class PersistentVolumeClaimList(DictMixin):
-    """PersistentVolumeClaimList is a list of PersistentVolumeClaim items.
+    r"""PersistentVolumeClaimList is a list of PersistentVolumeClaim items.
 
       **parameters**
 
       * **items** ``List[PersistentVolumeClaim]`` - items is a list of persistent volume claims. More info:
         https://kubernetes.io/docs/concepts/storage/persistent-volumes#persistentvolumeclaims
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -2903,15 +2903,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class PersistentVolumeClaimSpec(DictMixin):
-    """PersistentVolumeClaimSpec describes the common attributes of storage devices
+    r"""PersistentVolumeClaimSpec describes the common attributes of storage devices
       and allows a Source for provider-specific attributes
 
       **parameters**
 
       * **accessModes** ``Optional[List[str]]`` - accessModes contains the desired access modes the volume should have. More
         info:
         https://kubernetes.io/docs/concepts/storage/persistent-volumes#access-modes-1
@@ -2983,15 +2983,15 @@
     volumeAttributesClassName: 'Optional[str]' = None
     volumeMode: 'Optional[str]' = None
     volumeName: 'Optional[str]' = None
 
 
 @dataclass
 class PersistentVolumeClaimStatus(DictMixin):
-    """PersistentVolumeClaimStatus is the current status of a persistent volume
+    r"""PersistentVolumeClaimStatus is the current status of a persistent volume
       claim.
 
       **parameters**
 
       * **accessModes** ``Optional[List[str]]`` - accessModes contains the actual access modes the volume backing the PVC has.
         More info:
         https://kubernetes.io/docs/concepts/storage/persistent-volumes#access-modes-1
@@ -3083,15 +3083,15 @@
     currentVolumeAttributesClassName: 'Optional[str]' = None
     modifyVolumeStatus: 'Optional[ModifyVolumeStatus]' = None
     phase: 'Optional[str]' = None
 
 
 @dataclass
 class PersistentVolumeClaimTemplate(DictMixin):
-    """PersistentVolumeClaimTemplate is used to produce PersistentVolumeClaim objects
+    r"""PersistentVolumeClaimTemplate is used to produce PersistentVolumeClaim objects
       as part of an EphemeralVolumeSource.
 
       **parameters**
 
       * **spec** ``PersistentVolumeClaimSpec`` - The specification for the PersistentVolumeClaim. The entire content is copied
         unchanged into the PVC that gets created from this template. The same fields
         as in a PersistentVolumeClaim are also valid here.
@@ -3101,15 +3101,15 @@
     """
     spec: 'PersistentVolumeClaimSpec'
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
 class PersistentVolumeClaimVolumeSource(DictMixin):
-    """PersistentVolumeClaimVolumeSource references the user's PVC in the same
+    r"""PersistentVolumeClaimVolumeSource references the user's PVC in the same
       namespace. This volume finds the bound PV and mounts that volume for the pod.
       A PersistentVolumeClaimVolumeSource is, essentially, a wrapper around another
       type of volume that is owned by someone else (the system).
 
       **parameters**
 
       * **claimName** ``str`` - claimName is the name of a PersistentVolumeClaim in the same namespace as the
@@ -3119,15 +3119,15 @@
     """
     claimName: 'str'
     readOnly: 'Optional[bool]' = None
 
 
 @dataclass
 class PersistentVolumeList(DictMixin):
-    """PersistentVolumeList is a list of PersistentVolume items.
+    r"""PersistentVolumeList is a list of PersistentVolume items.
 
       **parameters**
 
       * **items** ``List[PersistentVolume]`` - items is a list of persistent volumes. More info:
         https://kubernetes.io/docs/concepts/storage/persistent-volumes
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -3144,15 +3144,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class PersistentVolumeSpec(DictMixin):
-    """PersistentVolumeSpec is the specification of a persistent volume.
+    r"""PersistentVolumeSpec is the specification of a persistent volume.
 
       **parameters**
 
       * **accessModes** ``Optional[List[str]]`` - accessModes contains all ways the volume can be mounted. More info:
         https://kubernetes.io/docs/concepts/storage/persistent-volumes#access-modes
       * **awsElasticBlockStore** ``Optional[AWSElasticBlockStoreVolumeSource]`` - awsElasticBlockStore represents an AWS Disk resource that is attached to a
         kubelet's host machine and then exposed to the pod. More info:
@@ -3268,15 +3268,15 @@
     volumeAttributesClassName: 'Optional[str]' = None
     volumeMode: 'Optional[str]' = None
     vsphereVolume: 'Optional[VsphereVirtualDiskVolumeSource]' = None
 
 
 @dataclass
 class PersistentVolumeStatus(DictMixin):
-    """PersistentVolumeStatus is the current status of a persistent volume.
+    r"""PersistentVolumeStatus is the current status of a persistent volume.
 
       **parameters**
 
       * **lastPhaseTransitionTime** ``Optional[meta_v1.Time]`` - lastPhaseTransitionTime is the time the phase transitioned from one to another
         and automatically resets to current time everytime a volume phase transitions.
         This is a beta field and requires the PersistentVolumeLastPhaseTransitionTime
         feature to be enabled (enabled by default).
@@ -3292,30 +3292,30 @@
     message: 'Optional[str]' = None
     phase: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class PhotonPersistentDiskVolumeSource(DictMixin):
-    """Represents a Photon Controller persistent disk resource.
+    r"""Represents a Photon Controller persistent disk resource.
 
       **parameters**
 
       * **pdID** ``str`` - pdID is the ID that identifies Photon Controller persistent disk
       * **fsType** ``Optional[str]`` - fsType is the filesystem type to mount. Must be a filesystem type supported by
         the host operating system. Ex. "ext4", "xfs", "ntfs". Implicitly inferred to
         be "ext4" if unspecified.
     """
     pdID: 'str'
     fsType: 'Optional[str]' = None
 
 
 @dataclass
 class Pod(DictMixin):
-    """Pod is a collection of containers that can run on a host. This resource is
+    r"""Pod is a collection of containers that can run on a host. This resource is
       created by clients and scheduled onto hosts.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -3337,15 +3337,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[PodSpec]' = None
     status: 'Optional[PodStatus]' = None
 
 
 @dataclass
 class PodAffinity(DictMixin):
-    """Pod affinity is a group of inter pod affinity scheduling rules.
+    r"""Pod affinity is a group of inter pod affinity scheduling rules.
 
       **parameters**
 
       * **preferredDuringSchedulingIgnoredDuringExecution** ``Optional[List[WeightedPodAffinityTerm]]`` - The scheduler will prefer to schedule pods to nodes that satisfy the affinity
         expressions specified by this field, but it may choose a node that violates
         one or more of the expressions. The node that is most preferred is the one
         with the greatest sum of weights, i.e. for each node that meets all of the
@@ -3364,15 +3364,15 @@
     """
     preferredDuringSchedulingIgnoredDuringExecution: 'Optional[List[WeightedPodAffinityTerm]]' = None
     requiredDuringSchedulingIgnoredDuringExecution: 'Optional[List[PodAffinityTerm]]' = None
 
 
 @dataclass
 class PodAffinityTerm(DictMixin):
-    """Defines a set of pods (namely those matching the labelSelector relative to the
+    r"""Defines a set of pods (namely those matching the labelSelector relative to the
       given namespace(s)) that this pod should be co-located (affinity) or not
       co-located (anti-affinity) with, where co-located is defined as running on a
       node whose value of the label with key <topologyKey> matches that of any node
       on which a pod of the set of pods is running
 
       **parameters**
 
@@ -3418,15 +3418,15 @@
     mismatchLabelKeys: 'Optional[List[str]]' = None
     namespaceSelector: 'Optional[meta_v1.LabelSelector]' = None
     namespaces: 'Optional[List[str]]' = None
 
 
 @dataclass
 class PodAntiAffinity(DictMixin):
-    """Pod anti affinity is a group of inter pod anti affinity scheduling rules.
+    r"""Pod anti affinity is a group of inter pod anti affinity scheduling rules.
 
       **parameters**
 
       * **preferredDuringSchedulingIgnoredDuringExecution** ``Optional[List[WeightedPodAffinityTerm]]`` - The scheduler will prefer to schedule pods to nodes that satisfy the
         anti-affinity expressions specified by this field, but it may choose a node
         that violates one or more of the expressions. The node that is most preferred
         is the one with the greatest sum of weights, i.e. for each node that meets all
@@ -3445,15 +3445,15 @@
     """
     preferredDuringSchedulingIgnoredDuringExecution: 'Optional[List[WeightedPodAffinityTerm]]' = None
     requiredDuringSchedulingIgnoredDuringExecution: 'Optional[List[PodAffinityTerm]]' = None
 
 
 @dataclass
 class PodCondition(DictMixin):
-    """PodCondition contains details for the current condition of this pod.
+    r"""PodCondition contains details for the current condition of this pod.
 
       **parameters**
 
       * **status** ``str`` - Status is the status of the condition. Can be True, False, Unknown. More info:
         https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#pod-conditions
       * **type** ``str`` - Type is the type of the condition. More info:
         https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#pod-conditions
@@ -3468,15 +3468,15 @@
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class PodDNSConfig(DictMixin):
-    """PodDNSConfig defines the DNS parameters of a pod in addition to those
+    r"""PodDNSConfig defines the DNS parameters of a pod in addition to those
       generated from DNSPolicy.
 
       **parameters**
 
       * **nameservers** ``Optional[List[str]]`` - A list of DNS name server IP addresses. This will be appended to the base
         nameservers generated from DNSPolicy. Duplicated nameservers will be removed.
       * **options** ``Optional[List[PodDNSConfigOption]]`` - A list of DNS resolver options. This will be merged with the base options
@@ -3490,39 +3490,39 @@
     nameservers: 'Optional[List[str]]' = None
     options: 'Optional[List[PodDNSConfigOption]]' = None
     searches: 'Optional[List[str]]' = None
 
 
 @dataclass
 class PodDNSConfigOption(DictMixin):
-    """PodDNSConfigOption defines DNS resolver options of a pod.
+    r"""PodDNSConfigOption defines DNS resolver options of a pod.
 
       **parameters**
 
       * **name** ``Optional[str]`` - Required.
       * **value** ``Optional[str]`` - 
     """
     name: 'Optional[str]' = None
     value: 'Optional[str]' = None
 
 
 @dataclass
 class PodIP(DictMixin):
-    """PodIP represents a single IP address allocated to the pod.
+    r"""PodIP represents a single IP address allocated to the pod.
 
       **parameters**
 
       * **ip** ``Optional[str]`` - IP is the IP address assigned to the pod
     """
     ip: 'Optional[str]' = None
 
 
 @dataclass
 class PodList(DictMixin):
-    """PodList is a list of Pods.
+    r"""PodList is a list of Pods.
 
       **parameters**
 
       * **items** ``List[Pod]`` - List of pods. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -3539,15 +3539,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class PodOS(DictMixin):
-    """PodOS defines the OS parameters of a pod.
+    r"""PodOS defines the OS parameters of a pod.
 
       **parameters**
 
       * **name** ``str`` - Name is the name of the operating system. The currently supported values are
         linux and windows. Additional value may be defined in future and can be one
         of:
         https://github.com/opencontainers/runtime-spec/blob/master/config.md#platform-specific-configuration
@@ -3555,27 +3555,27 @@
         values in this field as os: null
     """
     name: 'str'
 
 
 @dataclass
 class PodReadinessGate(DictMixin):
-    """PodReadinessGate contains the reference to a pod condition
+    r"""PodReadinessGate contains the reference to a pod condition
 
       **parameters**
 
       * **conditionType** ``str`` - ConditionType refers to a condition in the pod's condition list with matching
         type.
     """
     conditionType: 'str'
 
 
 @dataclass
 class PodResourceClaim(DictMixin):
-    """PodResourceClaim references exactly one ResourceClaim through a ClaimSource.
+    r"""PodResourceClaim references exactly one ResourceClaim through a ClaimSource.
       It adds a name to it that uniquely identifies the ResourceClaim inside the
       Pod. Containers that need access to the ResourceClaim reference it with this
       name.
 
       **parameters**
 
       * **name** ``str`` - Name uniquely identifies this resource claim inside the pod. This must be a
@@ -3584,15 +3584,15 @@
     """
     name: 'str'
     source: 'Optional[ClaimSource]' = None
 
 
 @dataclass
 class PodResourceClaimStatus(DictMixin):
-    """PodResourceClaimStatus is stored in the PodStatus for each PodResourceClaim
+    r"""PodResourceClaimStatus is stored in the PodStatus for each PodResourceClaim
       which references a ResourceClaimTemplate. It stores the generated name for the
       corresponding ResourceClaim.
 
       **parameters**
 
       * **name** ``str`` - Name uniquely identifies this resource claim inside the pod. This must match
         the name of an entry in pod.spec.resourceClaims, which implies that the string
@@ -3604,27 +3604,27 @@
     """
     name: 'str'
     resourceClaimName: 'Optional[str]' = None
 
 
 @dataclass
 class PodSchedulingGate(DictMixin):
-    """PodSchedulingGate is associated to a Pod to guard its scheduling.
+    r"""PodSchedulingGate is associated to a Pod to guard its scheduling.
 
       **parameters**
 
       * **name** ``str`` - Name of the scheduling gate. Each scheduling gate must have a unique name
         field.
     """
     name: 'str'
 
 
 @dataclass
 class PodSecurityContext(DictMixin):
-    """PodSecurityContext holds pod-level security attributes and common container
+    r"""PodSecurityContext holds pod-level security attributes and common container
       settings. Some fields are also present in container.securityContext.  Field
       values of container.securityContext take precedence over field values of
       PodSecurityContext.
 
       **parameters**
 
       * **appArmorProfile** ``Optional[AppArmorProfile]`` - appArmorProfile is the AppArmor options to use by the containers in this pod.
@@ -3695,15 +3695,15 @@
     supplementalGroups: 'Optional[List[int]]' = None
     sysctls: 'Optional[List[Sysctl]]' = None
     windowsOptions: 'Optional[WindowsSecurityContextOptions]' = None
 
 
 @dataclass
 class PodSpec(DictMixin):
-    """PodSpec is a description of a pod.
+    r"""PodSpec is a description of a pod.
 
       **parameters**
 
       * **containers** ``List[Container]`` - List of containers belonging to the pod. Containers cannot currently be added
         or removed. There must be at least one container in a Pod. Cannot be updated.
       * **activeDeadlineSeconds** ``Optional[int]`` - Optional duration in seconds the pod may be active on the node relative to
         StartTime before the system will actively try to mark it failed and kill
@@ -3913,15 +3913,15 @@
     tolerations: 'Optional[List[Toleration]]' = None
     topologySpreadConstraints: 'Optional[List[TopologySpreadConstraint]]' = None
     volumes: 'Optional[List[Volume]]' = None
 
 
 @dataclass
 class PodStatus(DictMixin):
-    """PodStatus represents information about the status of a pod. Status may trail
+    r"""PodStatus represents information about the status of a pod. Status may trail
       the actual state of a system, especially if the node that hosts the pod cannot
       contact the control plane.
 
       **parameters**
 
       * **conditions** ``Optional[List[PodCondition]]`` - Current service state of pod. More info:
         https://kubernetes.io/docs/concepts/workloads/pods/pod-lifecycle#pod-conditions
@@ -4003,15 +4003,15 @@
     resize: 'Optional[str]' = None
     resourceClaimStatuses: 'Optional[List[PodResourceClaimStatus]]' = None
     startTime: 'Optional[meta_v1.Time]' = None
 
 
 @dataclass
 class PodTemplate(DictMixin):
-    """PodTemplate describes a template for creating copies of a predefined pod.
+    r"""PodTemplate describes a template for creating copies of a predefined pod.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -4028,15 +4028,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     template: 'Optional[PodTemplateSpec]' = None
 
 
 @dataclass
 class PodTemplateList(DictMixin):
-    """PodTemplateList is a list of PodTemplates.
+    r"""PodTemplateList is a list of PodTemplates.
 
       **parameters**
 
       * **items** ``List[PodTemplate]`` - List of pod templates
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -4052,15 +4052,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class PodTemplateSpec(DictMixin):
-    """PodTemplateSpec describes the data a pod should have when created from a
+    r"""PodTemplateSpec describes the data a pod should have when created from a
       template
 
       **parameters**
 
       * **metadata** ``Optional[meta_v1.ObjectMeta]`` - Standard object's metadata. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#metadata
       * **spec** ``Optional[PodSpec]`` - Specification of the desired behavior of the pod. More info:
@@ -4068,15 +4068,15 @@
     """
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[PodSpec]' = None
 
 
 @dataclass
 class PortStatus(DictMixin):
-    """
+    r"""
 
       **parameters**
 
       * **port** ``int`` - Port is the port number of the service port of which status is recorded here
       * **protocol** ``str`` - Protocol is the protocol of the service port of which status is recorded here
         The supported values are: "TCP", "UDP", "SCTP"
       * **error** ``Optional[str]`` - Error is to record the problem with the service port The format of the error
@@ -4089,15 +4089,15 @@
     port: 'int'
     protocol: 'str'
     error: 'Optional[str]' = None
 
 
 @dataclass
 class PortworxVolumeSource(DictMixin):
-    """PortworxVolumeSource represents a Portworx volume resource.
+    r"""PortworxVolumeSource represents a Portworx volume resource.
 
       **parameters**
 
       * **volumeID** ``str`` - volumeID uniquely identifies a Portworx volume
       * **fsType** ``Optional[str]`` - fSType represents the filesystem type to mount Must be a filesystem type
         supported by the host operating system. Ex. "ext4", "xfs". Implicitly inferred
         to be "ext4" if unspecified.
@@ -4107,15 +4107,15 @@
     volumeID: 'str'
     fsType: 'Optional[str]' = None
     readOnly: 'Optional[bool]' = None
 
 
 @dataclass
 class PreferredSchedulingTerm(DictMixin):
-    """An empty preferred scheduling term matches all objects with implicit weight 0
+    r"""An empty preferred scheduling term matches all objects with implicit weight 0
       (i.e. it's a no-op). A null preferred scheduling term matches no objects (i.e.
       is also a no-op).
 
       **parameters**
 
       * **preference** ``NodeSelectorTerm`` - A node selector term, associated with the corresponding weight.
       * **weight** ``int`` - Weight associated with matching the corresponding nodeSelectorTerm, in the
@@ -4123,15 +4123,15 @@
     """
     preference: 'NodeSelectorTerm'
     weight: 'int'
 
 
 @dataclass
 class Probe(DictMixin):
-    """Probe describes a health check to be performed against a container to
+    r"""Probe describes a health check to be performed against a container to
       determine whether it is alive or ready to receive traffic.
 
       **parameters**
 
       * **exec** ``Optional[ExecAction]`` - Exec specifies the action to take.
       * **failureThreshold** ``Optional[int]`` - Minimum consecutive failures for the probe to be considered failed after
         having succeeded. Defaults to 3. Minimum value is 1.
@@ -4171,15 +4171,15 @@
     tcpSocket: 'Optional[TCPSocketAction]' = None
     terminationGracePeriodSeconds: 'Optional[int]' = None
     timeoutSeconds: 'Optional[int]' = None
 
 
 @dataclass
 class ProjectedVolumeSource(DictMixin):
-    """Represents a projected volume source
+    r"""Represents a projected volume source
 
       **parameters**
 
       * **defaultMode** ``Optional[int]`` - defaultMode are the mode bits used to set permissions on created files by
         default. Must be an octal value between 0000 and 0777 or a decimal value
         between 0 and 511. YAML accepts both octal and decimal values, JSON requires
         decimal values for mode bits. Directories within the path are not affected by
@@ -4189,15 +4189,15 @@
     """
     defaultMode: 'Optional[int]' = None
     sources: 'Optional[List[VolumeProjection]]' = None
 
 
 @dataclass
 class QuobyteVolumeSource(DictMixin):
-    """Represents a Quobyte mount that lasts the lifetime of a pod. Quobyte volumes
+    r"""Represents a Quobyte mount that lasts the lifetime of a pod. Quobyte volumes
       do not support ownership management or SELinux relabeling.
 
       **parameters**
 
       * **registry** ``str`` - registry represents a single or multiple Quobyte Registry services specified
         as a string as host:port pair (multiple entries are separated with commas)
         which acts as the central registry for volumes
@@ -4215,15 +4215,15 @@
     readOnly: 'Optional[bool]' = None
     tenant: 'Optional[str]' = None
     user: 'Optional[str]' = None
 
 
 @dataclass
 class RBDPersistentVolumeSource(DictMixin):
-    """Represents a Rados Block Device mount that lasts the lifetime of a pod. RBD
+    r"""Represents a Rados Block Device mount that lasts the lifetime of a pod. RBD
       volumes support ownership management and SELinux relabeling.
 
       **parameters**
 
       * **image** ``str`` - image is the rados image name. More info:
         https://examples.k8s.io/volumes/rbd/README.md#how-to-use-it
       * **monitors** ``List[str]`` - monitors is a collection of Ceph monitors. More info:
@@ -4253,15 +4253,15 @@
     readOnly: 'Optional[bool]' = None
     secretRef: 'Optional[SecretReference]' = None
     user: 'Optional[str]' = None
 
 
 @dataclass
 class RBDVolumeSource(DictMixin):
-    """Represents a Rados Block Device mount that lasts the lifetime of a pod. RBD
+    r"""Represents a Rados Block Device mount that lasts the lifetime of a pod. RBD
       volumes support ownership management and SELinux relabeling.
 
       **parameters**
 
       * **image** ``str`` - image is the rados image name. More info:
         https://examples.k8s.io/volumes/rbd/README.md#how-to-use-it
       * **monitors** ``List[str]`` - monitors is a collection of Ceph monitors. More info:
@@ -4291,15 +4291,15 @@
     readOnly: 'Optional[bool]' = None
     secretRef: 'Optional[LocalObjectReference]' = None
     user: 'Optional[str]' = None
 
 
 @dataclass
 class ReplicationController(DictMixin):
-    """ReplicationController represents the configuration of a replication
+    r"""ReplicationController represents the configuration of a replication
       controller.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -4325,15 +4325,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[ReplicationControllerSpec]' = None
     status: 'Optional[ReplicationControllerStatus]' = None
 
 
 @dataclass
 class ReplicationControllerCondition(DictMixin):
-    """ReplicationControllerCondition describes the state of a replication controller
+    r"""ReplicationControllerCondition describes the state of a replication controller
       at a certain point.
 
       **parameters**
 
       * **status** ``str`` - Status of the condition, one of True, False, Unknown.
       * **type** ``str`` - Type of replication controller condition.
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - The last time the condition transitioned from one status to another.
@@ -4345,15 +4345,15 @@
     lastTransitionTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class ReplicationControllerList(DictMixin):
-    """ReplicationControllerList is a collection of replication controllers.
+    r"""ReplicationControllerList is a collection of replication controllers.
 
       **parameters**
 
       * **items** ``List[ReplicationController]`` - List of replication controllers. More info:
         https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -4370,15 +4370,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ReplicationControllerSpec(DictMixin):
-    """ReplicationControllerSpec is the specification of a replication controller.
+    r"""ReplicationControllerSpec is the specification of a replication controller.
 
       **parameters**
 
       * **minReadySeconds** ``Optional[int]`` - Minimum number of seconds for which a newly created pod should be ready
         without any of its container crashing, for it to be considered available.
         Defaults to 0 (pod will be considered available as soon as it is ready)
       * **replicas** ``Optional[int]`` - Replicas is the number of desired replicas. This is a pointer to distinguish
@@ -4399,15 +4399,15 @@
     replicas: 'Optional[int]' = None
     selector: 'Optional[dict]' = None
     template: 'Optional[PodTemplateSpec]' = None
 
 
 @dataclass
 class ReplicationControllerStatus(DictMixin):
-    """ReplicationControllerStatus represents the current status of a replication
+    r"""ReplicationControllerStatus represents the current status of a replication
       controller.
 
       **parameters**
 
       * **replicas** ``int`` - Replicas is the most recently observed number of replicas. More info:
         https://kubernetes.io/docs/concepts/workloads/controllers/replicationcontroller#what-is-a-replicationcontroller
       * **availableReplicas** ``Optional[int]`` - The number of available replicas (ready for at least minReadySeconds) for this
@@ -4426,27 +4426,27 @@
     fullyLabeledReplicas: 'Optional[int]' = None
     observedGeneration: 'Optional[int]' = None
     readyReplicas: 'Optional[int]' = None
 
 
 @dataclass
 class ResourceClaim(DictMixin):
-    """ResourceClaim references one entry in PodSpec.ResourceClaims.
+    r"""ResourceClaim references one entry in PodSpec.ResourceClaims.
 
       **parameters**
 
       * **name** ``str`` - Name must match the name of one entry in pod.spec.resourceClaims of the Pod
         where this field is used. It makes that resource available inside a container.
     """
     name: 'str'
 
 
 @dataclass
 class ResourceFieldSelector(DictMixin):
-    """ResourceFieldSelector represents container resources (cpu, memory) and their
+    r"""ResourceFieldSelector represents container resources (cpu, memory) and their
       output format
 
       **parameters**
 
       * **resource** ``str`` - Required: resource to select
       * **containerName** ``Optional[str]`` - Container name: required for volumes, optional for env vars
       * **divisor** ``Optional[resource.Quantity]`` - Specifies the output format of the exposed resources, defaults to "1"
@@ -4454,15 +4454,15 @@
     resource: 'str'
     containerName: 'Optional[str]' = None
     divisor: 'Optional[resource.Quantity]' = None
 
 
 @dataclass
 class ResourceQuota(DictMixin):
-    """ResourceQuota sets aggregate quota restrictions enforced per namespace
+    r"""ResourceQuota sets aggregate quota restrictions enforced per namespace
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -4482,15 +4482,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[ResourceQuotaSpec]' = None
     status: 'Optional[ResourceQuotaStatus]' = None
 
 
 @dataclass
 class ResourceQuotaList(DictMixin):
-    """ResourceQuotaList is a list of ResourceQuota items.
+    r"""ResourceQuotaList is a list of ResourceQuota items.
 
       **parameters**
 
       * **items** ``List[ResourceQuota]`` - Items is a list of ResourceQuota objects. More info:
         https://kubernetes.io/docs/concepts/policy/resource-quotas/
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -4507,15 +4507,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ResourceQuotaSpec(DictMixin):
-    """ResourceQuotaSpec defines the desired hard limits to enforce for Quota.
+    r"""ResourceQuotaSpec defines the desired hard limits to enforce for Quota.
 
       **parameters**
 
       * **hard** ``Optional[dict]`` - hard is the set of desired hard limits for each named resource. More info:
         https://kubernetes.io/docs/concepts/policy/resource-quotas/
       * **scopeSelector** ``Optional[ScopeSelector]`` - scopeSelector is also a collection of filters like scopes that must match each
         object tracked by a quota but expressed using ScopeSelectorOperator in
@@ -4527,29 +4527,29 @@
     hard: 'Optional[dict]' = None
     scopeSelector: 'Optional[ScopeSelector]' = None
     scopes: 'Optional[List[str]]' = None
 
 
 @dataclass
 class ResourceQuotaStatus(DictMixin):
-    """ResourceQuotaStatus defines the enforced hard limits and observed use.
+    r"""ResourceQuotaStatus defines the enforced hard limits and observed use.
 
       **parameters**
 
       * **hard** ``Optional[dict]`` - Hard is the set of enforced hard limits for each named resource. More info:
         https://kubernetes.io/docs/concepts/policy/resource-quotas/
       * **used** ``Optional[dict]`` - Used is the current observed total usage of the resource in the namespace.
     """
     hard: 'Optional[dict]' = None
     used: 'Optional[dict]' = None
 
 
 @dataclass
 class ResourceRequirements(DictMixin):
-    """ResourceRequirements describes the compute resource requirements.
+    r"""ResourceRequirements describes the compute resource requirements.
 
       **parameters**
 
       * **claims** ``Optional[List[ResourceClaim]]`` - Claims lists the names of resources, defined in spec.resourceClaims, that are
         used by this container.
         This is an alpha field and requires enabling the DynamicResourceAllocation
         feature gate.
@@ -4565,15 +4565,15 @@
     claims: 'Optional[List[ResourceClaim]]' = None
     limits: 'Optional[dict]' = None
     requests: 'Optional[dict]' = None
 
 
 @dataclass
 class SELinuxOptions(DictMixin):
-    """SELinuxOptions are the labels to be applied to the container
+    r"""SELinuxOptions are the labels to be applied to the container
 
       **parameters**
 
       * **level** ``Optional[str]`` - Level is SELinux level label that applies to the container.
       * **role** ``Optional[str]`` - Role is a SELinux role label that applies to the container.
       * **type** ``Optional[str]`` - Type is a SELinux type label that applies to the container.
       * **user** ``Optional[str]`` - User is a SELinux user label that applies to the container.
@@ -4582,15 +4582,15 @@
     role: 'Optional[str]' = None
     type: 'Optional[str]' = None
     user: 'Optional[str]' = None
 
 
 @dataclass
 class ScaleIOPersistentVolumeSource(DictMixin):
-    """ScaleIOPersistentVolumeSource represents a persistent ScaleIO volume
+    r"""ScaleIOPersistentVolumeSource represents a persistent ScaleIO volume
 
       **parameters**
 
       * **gateway** ``str`` - gateway is the host address of the ScaleIO API Gateway.
       * **secretRef** ``SecretReference`` - secretRef references to the secret for ScaleIO user and other sensitive
         information. If this is not provided, Login operation will fail.
       * **system** ``str`` - system is the name of the storage system as configured in ScaleIO.
@@ -4618,15 +4618,15 @@
     storageMode: 'Optional[str]' = None
     storagePool: 'Optional[str]' = None
     volumeName: 'Optional[str]' = None
 
 
 @dataclass
 class ScaleIOVolumeSource(DictMixin):
-    """ScaleIOVolumeSource represents a persistent ScaleIO volume
+    r"""ScaleIOVolumeSource represents a persistent ScaleIO volume
 
       **parameters**
 
       * **gateway** ``str`` - gateway is the host address of the ScaleIO API Gateway.
       * **secretRef** ``LocalObjectReference`` - secretRef references to the secret for ScaleIO user and other sensitive
         information. If this is not provided, Login operation will fail.
       * **system** ``str`` - system is the name of the storage system as configured in ScaleIO.
@@ -4653,27 +4653,27 @@
     storageMode: 'Optional[str]' = None
     storagePool: 'Optional[str]' = None
     volumeName: 'Optional[str]' = None
 
 
 @dataclass
 class ScopeSelector(DictMixin):
-    """A scope selector represents the AND of the selectors represented by the
+    r"""A scope selector represents the AND of the selectors represented by the
       scoped-resource selector requirements.
 
       **parameters**
 
       * **matchExpressions** ``Optional[List[ScopedResourceSelectorRequirement]]`` - A list of scope selector requirements by scope of the resources.
     """
     matchExpressions: 'Optional[List[ScopedResourceSelectorRequirement]]' = None
 
 
 @dataclass
 class ScopedResourceSelectorRequirement(DictMixin):
-    """A scoped-resource selector requirement is a selector that contains values, a
+    r"""A scoped-resource selector requirement is a selector that contains values, a
       scope name, and an operator that relates the scope name and values.
 
       **parameters**
 
       * **operator** ``str`` - Represents a scope's relationship to a set of values. Valid operators are In,
         NotIn, Exists, DoesNotExist.
       * **scopeName** ``str`` - The name of the scope that the selector applies to.
@@ -4684,15 +4684,15 @@
     operator: 'str'
     scopeName: 'str'
     values: 'Optional[List[str]]' = None
 
 
 @dataclass
 class SeccompProfile(DictMixin):
-    """SeccompProfile defines a pod/container's seccomp profile settings. Only one
+    r"""SeccompProfile defines a pod/container's seccomp profile settings. Only one
       profile source may be set.
 
       **parameters**
 
       * **type** ``str`` - type indicates which kind of seccomp profile will be applied. Valid options
         are:
         Localhost - a profile defined in a file on the node should be used.
@@ -4706,15 +4706,15 @@
     """
     type: 'str'
     localhostProfile: 'Optional[str]' = None
 
 
 @dataclass
 class Secret(DictMixin):
-    """Secret holds secret data of a certain type. The total bytes of the values in
+    r"""Secret holds secret data of a certain type. The total bytes of the values in
       the Data field must be less than MaxSecretSize bytes.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -4746,15 +4746,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     stringData: 'Optional[dict]' = None
     type: 'Optional[str]' = None
 
 
 @dataclass
 class SecretEnvSource(DictMixin):
-    """SecretEnvSource selects a Secret to populate the environment variables with.
+    r"""SecretEnvSource selects a Secret to populate the environment variables with.
       
       The contents of the target Secret's Data field will represent the key-value
       pairs as environment variables.
 
       **parameters**
 
       * **name** ``Optional[str]`` - Name of the referent. More info:
@@ -4763,15 +4763,15 @@
     """
     name: 'Optional[str]' = None
     optional: 'Optional[bool]' = None
 
 
 @dataclass
 class SecretKeySelector(DictMixin):
-    """SecretKeySelector selects a key of a Secret.
+    r"""SecretKeySelector selects a key of a Secret.
 
       **parameters**
 
       * **key** ``str`` - The key of the secret to select from.  Must be a valid secret key.
       * **name** ``Optional[str]`` - Name of the referent. More info:
         https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names
       * **optional** ``Optional[bool]`` - Specify whether the Secret or its key must be defined
@@ -4779,15 +4779,15 @@
     key: 'str'
     name: 'Optional[str]' = None
     optional: 'Optional[bool]' = None
 
 
 @dataclass
 class SecretList(DictMixin):
-    """SecretList is a list of Secret.
+    r"""SecretList is a list of Secret.
 
       **parameters**
 
       * **items** ``List[Secret]`` - Items is a list of secret objects. More info:
         https://kubernetes.io/docs/concepts/configuration/secret
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -4804,15 +4804,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class SecretProjection(DictMixin):
-    """Adapts a secret into a projected volume.
+    r"""Adapts a secret into a projected volume.
       
       The contents of the target Secret's Data field will be presented in a
       projected volume as files using the keys in the Data field as the file names.
       Note that this is identical to a secret volume source without the default
       mode.
 
       **parameters**
@@ -4831,29 +4831,29 @@
     items: 'Optional[List[KeyToPath]]' = None
     name: 'Optional[str]' = None
     optional: 'Optional[bool]' = None
 
 
 @dataclass
 class SecretReference(DictMixin):
-    """SecretReference represents a Secret Reference. It has enough information to
+    r"""SecretReference represents a Secret Reference. It has enough information to
       retrieve secret in any namespace
 
       **parameters**
 
       * **name** ``Optional[str]`` - name is unique within a namespace to reference a secret resource.
       * **namespace** ``Optional[str]`` - namespace defines the space within which the secret name must be unique.
     """
     name: 'Optional[str]' = None
     namespace: 'Optional[str]' = None
 
 
 @dataclass
 class SecretVolumeSource(DictMixin):
-    """Adapts a Secret into a volume.
+    r"""Adapts a Secret into a volume.
       
       The contents of the target Secret's Data field will be presented in a volume
       as files using the keys in the Data field as the file names. Secret volumes
       support ownership management and SELinux relabeling.
 
       **parameters**
 
@@ -4879,15 +4879,15 @@
     items: 'Optional[List[KeyToPath]]' = None
     optional: 'Optional[bool]' = None
     secretName: 'Optional[str]' = None
 
 
 @dataclass
 class SecurityContext(DictMixin):
-    """SecurityContext holds security configuration that will be applied to a
+    r"""SecurityContext holds security configuration that will be applied to a
       container. Some fields are present in both SecurityContext and
       PodSecurityContext.  When both are set, the values in SecurityContext take
       precedence.
 
       **parameters**
 
       * **allowPrivilegeEscalation** ``Optional[bool]`` - AllowPrivilegeEscalation controls whether a process can gain more privileges
@@ -4953,15 +4953,15 @@
     seLinuxOptions: 'Optional[SELinuxOptions]' = None
     seccompProfile: 'Optional[SeccompProfile]' = None
     windowsOptions: 'Optional[WindowsSecurityContextOptions]' = None
 
 
 @dataclass
 class Service(DictMixin):
-    """Service is a named abstraction of software service (for example, mysql)
+    r"""Service is a named abstraction of software service (for example, mysql)
       consisting of local port (for example 3306) that the proxy listens on, and the
       selector that determines which pods will answer requests sent through the
       proxy.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
@@ -4985,15 +4985,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[ServiceSpec]' = None
     status: 'Optional[ServiceStatus]' = None
 
 
 @dataclass
 class ServiceAccount(DictMixin):
-    """ServiceAccount binds together: * a name, understood by users, and perhaps by
+    r"""ServiceAccount binds together: * a name, understood by users, and perhaps by
       peripheral systems, for an identity * a principal that can be authenticated
       and authorized * a set of secrets
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -5028,15 +5028,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     secrets: 'Optional[List[ObjectReference]]' = None
 
 
 @dataclass
 class ServiceAccountList(DictMixin):
-    """ServiceAccountList is a list of ServiceAccount objects
+    r"""ServiceAccountList is a list of ServiceAccount objects
 
       **parameters**
 
       * **items** ``List[ServiceAccount]`` - List of ServiceAccounts. More info:
         https://kubernetes.io/docs/tasks/configure-pod-container/configure-service-account/
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -5053,15 +5053,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ServiceAccountTokenProjection(DictMixin):
-    """ServiceAccountTokenProjection represents a projected service account token
+    r"""ServiceAccountTokenProjection represents a projected service account token
       volume. This projection can be used to insert a service account token into the
       pods runtime filesystem for use against APIs (Kubernetes API Server or
       otherwise).
 
       **parameters**
 
       * **path** ``str`` - path is the path relative to the mount point of the file to project the token
@@ -5080,15 +5080,15 @@
     path: 'str'
     audience: 'Optional[str]' = None
     expirationSeconds: 'Optional[int]' = None
 
 
 @dataclass
 class ServiceList(DictMixin):
-    """ServiceList holds a list of services.
+    r"""ServiceList holds a list of services.
 
       **parameters**
 
       * **items** ``List[Service]`` - List of services
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -5104,15 +5104,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ServicePort(DictMixin):
-    """ServicePort contains information on service's port.
+    r"""ServicePort contains information on service's port.
 
       **parameters**
 
       * **port** ``int`` - The port that will be exposed by this service.
       * **appProtocol** ``Optional[str]`` - The application protocol for this port. This is used as a hint for
         implementations to offer richer behavior for protocols that they understand.
         This field follows standard Kubernetes label syntax. Valid values are either:
@@ -5157,15 +5157,15 @@
     nodePort: 'Optional[int]' = None
     protocol: 'Optional[str]' = None
     targetPort: 'Optional[util_intstr.IntOrString]' = None
 
 
 @dataclass
 class ServiceSpec(DictMixin):
-    """ServiceSpec describes the attributes that a user creates on a service.
+    r"""ServiceSpec describes the attributes that a user creates on a service.
 
       **parameters**
 
       * **allocateLoadBalancerNodePorts** ``Optional[bool]`` - allocateLoadBalancerNodePorts defines if NodePorts will be automatically
         allocated for services with type LoadBalancer.  Default is "true". It may be
         set to "false" if the cluster load-balancer does not rely on NodePorts.  If
         the caller requests specific NodePorts (by specifying a value), those requests
@@ -5356,51 +5356,51 @@
     sessionAffinityConfig: 'Optional[SessionAffinityConfig]' = None
     trafficDistribution: 'Optional[str]' = None
     type: 'Optional[str]' = None
 
 
 @dataclass
 class ServiceStatus(DictMixin):
-    """ServiceStatus represents the current status of a service.
+    r"""ServiceStatus represents the current status of a service.
 
       **parameters**
 
       * **conditions** ``Optional[List[meta_v1.Condition]]`` - Current service state
       * **loadBalancer** ``Optional[LoadBalancerStatus]`` - LoadBalancer contains the current status of the load-balancer, if one is
         present.
     """
     conditions: 'Optional[List[meta_v1.Condition]]' = None
     loadBalancer: 'Optional[LoadBalancerStatus]' = None
 
 
 @dataclass
 class SessionAffinityConfig(DictMixin):
-    """SessionAffinityConfig represents the configurations of session affinity.
+    r"""SessionAffinityConfig represents the configurations of session affinity.
 
       **parameters**
 
       * **clientIP** ``Optional[ClientIPConfig]`` - clientIP contains the configurations of Client IP based session affinity.
     """
     clientIP: 'Optional[ClientIPConfig]' = None
 
 
 @dataclass
 class SleepAction(DictMixin):
-    """SleepAction describes a "sleep" action.
+    r"""SleepAction describes a "sleep" action.
 
       **parameters**
 
       * **seconds** ``int`` - Seconds is the number of seconds to sleep.
     """
     seconds: 'int'
 
 
 @dataclass
 class StorageOSPersistentVolumeSource(DictMixin):
-    """Represents a StorageOS persistent volume resource.
+    r"""Represents a StorageOS persistent volume resource.
 
       **parameters**
 
       * **fsType** ``Optional[str]`` - fsType is the filesystem type to mount. Must be a filesystem type supported by
         the host operating system. Ex. "ext4", "xfs", "ntfs". Implicitly inferred to
         be "ext4" if unspecified.
       * **readOnly** ``Optional[bool]`` - readOnly defaults to false (read/write). ReadOnly here will force the ReadOnly
@@ -5421,15 +5421,15 @@
     secretRef: 'Optional[ObjectReference]' = None
     volumeName: 'Optional[str]' = None
     volumeNamespace: 'Optional[str]' = None
 
 
 @dataclass
 class StorageOSVolumeSource(DictMixin):
-    """Represents a StorageOS persistent volume resource.
+    r"""Represents a StorageOS persistent volume resource.
 
       **parameters**
 
       * **fsType** ``Optional[str]`` - fsType is the filesystem type to mount. Must be a filesystem type supported by
         the host operating system. Ex. "ext4", "xfs", "ntfs". Implicitly inferred to
         be "ext4" if unspecified.
       * **readOnly** ``Optional[bool]`` - readOnly defaults to false (read/write). ReadOnly here will force the ReadOnly
@@ -5450,42 +5450,42 @@
     secretRef: 'Optional[LocalObjectReference]' = None
     volumeName: 'Optional[str]' = None
     volumeNamespace: 'Optional[str]' = None
 
 
 @dataclass
 class Sysctl(DictMixin):
-    """Sysctl defines a kernel parameter to be set
+    r"""Sysctl defines a kernel parameter to be set
 
       **parameters**
 
       * **name** ``str`` - Name of a property to set
       * **value** ``str`` - Value of a property to set
     """
     name: 'str'
     value: 'str'
 
 
 @dataclass
 class TCPSocketAction(DictMixin):
-    """TCPSocketAction describes an action based on opening a socket
+    r"""TCPSocketAction describes an action based on opening a socket
 
       **parameters**
 
       * **port** ``util_intstr.IntOrString`` - Number or name of the port to access on the container. Number must be in the
         range 1 to 65535. Name must be an IANA_SVC_NAME.
       * **host** ``Optional[str]`` - Optional: Host name to connect to, defaults to the pod IP.
     """
     port: 'util_intstr.IntOrString'
     host: 'Optional[str]' = None
 
 
 @dataclass
 class Taint(DictMixin):
-    """The node this Taint is attached to has the "effect" on any pod that does not
+    r"""The node this Taint is attached to has the "effect" on any pod that does not
       tolerate the Taint.
 
       **parameters**
 
       * **effect** ``str`` - Required. The effect of the taint on pods that do not tolerate the taint.
         Valid effects are NoSchedule, PreferNoSchedule and NoExecute.
       * **key** ``str`` - Required. The taint key to be applied to a node.
@@ -5497,15 +5497,15 @@
     key: 'str'
     timeAdded: 'Optional[meta_v1.Time]' = None
     value: 'Optional[str]' = None
 
 
 @dataclass
 class Toleration(DictMixin):
-    """The pod this Toleration is attached to tolerates any taint that matches the
+    r"""The pod this Toleration is attached to tolerates any taint that matches the
       triple <key,value,effect> using the matching operator <operator>.
 
       **parameters**
 
       * **effect** ``Optional[str]`` - Effect indicates the taint effect to match. Empty means match all taint
         effects. When specified, allowed values are NoSchedule, PreferNoSchedule and
         NoExecute.
@@ -5528,44 +5528,44 @@
     operator: 'Optional[str]' = None
     tolerationSeconds: 'Optional[int]' = None
     value: 'Optional[str]' = None
 
 
 @dataclass
 class TopologySelectorLabelRequirement(DictMixin):
-    """A topology selector requirement is a selector that matches given label. This
+    r"""A topology selector requirement is a selector that matches given label. This
       is an alpha feature and may change in the future.
 
       **parameters**
 
       * **key** ``str`` - The label key that the selector applies to.
       * **values** ``List[str]`` - An array of string values. One value must match the label to be selected. Each
         entry in Values is ORed.
     """
     key: 'str'
     values: 'List[str]'
 
 
 @dataclass
 class TopologySelectorTerm(DictMixin):
-    """A topology selector term represents the result of label queries. A null or
+    r"""A topology selector term represents the result of label queries. A null or
       empty topology selector term matches no objects. The requirements of them are
       ANDed. It provides a subset of functionality as NodeSelectorTerm. This is an
       alpha feature and may change in the future.
 
       **parameters**
 
       * **matchLabelExpressions** ``Optional[List[TopologySelectorLabelRequirement]]`` - A list of topology selector requirements by labels.
     """
     matchLabelExpressions: 'Optional[List[TopologySelectorLabelRequirement]]' = None
 
 
 @dataclass
 class TopologySpreadConstraint(DictMixin):
-    """TopologySpreadConstraint specifies how to spread matching pods among the given
+    r"""TopologySpreadConstraint specifies how to spread matching pods among the given
       topology.
 
       **parameters**
 
       * **maxSkew** ``int`` - MaxSkew describes the degree to which pods may be unevenly distributed. When
         `whenUnsatisfiable=DoNotSchedule`, it is the maximum permitted difference
         between the number of matching pods in the target topology and the global
@@ -5657,15 +5657,15 @@
     minDomains: 'Optional[int]' = None
     nodeAffinityPolicy: 'Optional[str]' = None
     nodeTaintsPolicy: 'Optional[str]' = None
 
 
 @dataclass
 class TypedLocalObjectReference(DictMixin):
-    """TypedLocalObjectReference contains enough information to let you locate the
+    r"""TypedLocalObjectReference contains enough information to let you locate the
       typed referenced object inside the same namespace.
 
       **parameters**
 
       * **kind** ``str`` - Kind is the type of resource being referenced
       * **name** ``str`` - Name is the name of resource being referenced
       * **apiGroup** ``Optional[str]`` - APIGroup is the group for the resource being referenced. If APIGroup is not
@@ -5675,15 +5675,15 @@
     kind: 'str'
     name: 'str'
     apiGroup: 'Optional[str]' = None
 
 
 @dataclass
 class TypedObjectReference(DictMixin):
-    """
+    r"""
 
       **parameters**
 
       * **kind** ``str`` - Kind is the type of resource being referenced
       * **name** ``str`` - Name is the name of resource being referenced
       * **apiGroup** ``Optional[str]`` - APIGroup is the group for the resource being referenced. If APIGroup is not
         specified, the specified Kind must be in the core API group. For any other
@@ -5698,15 +5698,15 @@
     name: 'str'
     apiGroup: 'Optional[str]' = None
     namespace: 'Optional[str]' = None
 
 
 @dataclass
 class Volume(DictMixin):
-    """Volume represents a named volume in a pod that may be accessed by any
+    r"""Volume represents a named volume in a pod that may be accessed by any
       container in the pod.
 
       **parameters**
 
       * **name** ``str`` - name of the volume. Must be a DNS_LABEL and unique within the pod. More info:
         https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names
       * **awsElasticBlockStore** ``Optional[AWSElasticBlockStoreVolumeSource]`` - awsElasticBlockStore represents an AWS Disk resource that is attached to a
@@ -5818,29 +5818,29 @@
     secret: 'Optional[SecretVolumeSource]' = None
     storageos: 'Optional[StorageOSVolumeSource]' = None
     vsphereVolume: 'Optional[VsphereVirtualDiskVolumeSource]' = None
 
 
 @dataclass
 class VolumeDevice(DictMixin):
-    """volumeDevice describes a mapping of a raw block device within a container.
+    r"""volumeDevice describes a mapping of a raw block device within a container.
 
       **parameters**
 
       * **devicePath** ``str`` - devicePath is the path inside of the container that the device will be mapped
         to.
       * **name** ``str`` - name must match the name of a persistentVolumeClaim in the pod
     """
     devicePath: 'str'
     name: 'str'
 
 
 @dataclass
 class VolumeMount(DictMixin):
-    """VolumeMount describes a mounting of a Volume within a container.
+    r"""VolumeMount describes a mounting of a Volume within a container.
 
       **parameters**
 
       * **mountPath** ``str`` - Path within the container at which the volume should be mounted.  Must not
         contain ':'.
       * **name** ``str`` - This must match the Name of a Volume.
       * **mountPropagation** ``Optional[str]`` - mountPropagation determines how mounts are propagated from the host to
@@ -5876,15 +5876,15 @@
     recursiveReadOnly: 'Optional[str]' = None
     subPath: 'Optional[str]' = None
     subPathExpr: 'Optional[str]' = None
 
 
 @dataclass
 class VolumeMountStatus(DictMixin):
-    """VolumeMountStatus shows status of volume mounts.
+    r"""VolumeMountStatus shows status of volume mounts.
 
       **parameters**
 
       * **mountPath** ``str`` - MountPath corresponds to the original VolumeMount.
       * **name** ``str`` - Name corresponds to the name of the original VolumeMount.
       * **readOnly** ``Optional[bool]`` - ReadOnly corresponds to the original VolumeMount.
       * **recursiveReadOnly** ``Optional[str]`` - RecursiveReadOnly must be set to Disabled, Enabled, or unspecified (for
@@ -5895,27 +5895,27 @@
     name: 'str'
     readOnly: 'Optional[bool]' = None
     recursiveReadOnly: 'Optional[str]' = None
 
 
 @dataclass
 class VolumeNodeAffinity(DictMixin):
-    """VolumeNodeAffinity defines constraints that limit what nodes this volume can
+    r"""VolumeNodeAffinity defines constraints that limit what nodes this volume can
       be accessed from.
 
       **parameters**
 
       * **required** ``Optional[NodeSelector]`` - required specifies hard node constraints that must be met.
     """
     required: 'Optional[NodeSelector]' = None
 
 
 @dataclass
 class VolumeProjection(DictMixin):
-    """Projection that may be projected along with other supported volume types
+    r"""Projection that may be projected along with other supported volume types
 
       **parameters**
 
       * **clusterTrustBundle** ``Optional[ClusterTrustBundleProjection]`` - ClusterTrustBundle allows a pod to access the `.spec.trustBundle` field of
         ClusterTrustBundle objects in an auto-updating file.
         Alpha, gated by the ClusterTrustBundleProjection feature gate.
         ClusterTrustBundle objects can either be selected by name, or by the
@@ -5936,15 +5936,15 @@
     downwardAPI: 'Optional[DownwardAPIProjection]' = None
     secret: 'Optional[SecretProjection]' = None
     serviceAccountToken: 'Optional[ServiceAccountTokenProjection]' = None
 
 
 @dataclass
 class VolumeResourceRequirements(DictMixin):
-    """VolumeResourceRequirements describes the storage resource requirements for a
+    r"""VolumeResourceRequirements describes the storage resource requirements for a
       volume.
 
       **parameters**
 
       * **limits** ``Optional[dict]`` - Limits describes the maximum amount of compute resources allowed. More info:
         https://kubernetes.io/docs/concepts/configuration/manage-resources-containers/
       * **requests** ``Optional[dict]`` - Requests describes the minimum amount of compute resources required. If
@@ -5955,15 +5955,15 @@
     """
     limits: 'Optional[dict]' = None
     requests: 'Optional[dict]' = None
 
 
 @dataclass
 class VsphereVirtualDiskVolumeSource(DictMixin):
-    """Represents a vSphere volume resource.
+    r"""Represents a vSphere volume resource.
 
       **parameters**
 
       * **volumePath** ``str`` - volumePath is the path that identifies vSphere volume vmdk
       * **fsType** ``Optional[str]`` - fsType is filesystem type to mount. Must be a filesystem type supported by the
         host operating system. Ex. "ext4", "xfs", "ntfs". Implicitly inferred to be
         "ext4" if unspecified.
@@ -5975,30 +5975,30 @@
     fsType: 'Optional[str]' = None
     storagePolicyID: 'Optional[str]' = None
     storagePolicyName: 'Optional[str]' = None
 
 
 @dataclass
 class WeightedPodAffinityTerm(DictMixin):
-    """The weights of all of the matched WeightedPodAffinityTerm fields are added
+    r"""The weights of all of the matched WeightedPodAffinityTerm fields are added
       per-node to find the most preferred node(s)
 
       **parameters**
 
       * **podAffinityTerm** ``PodAffinityTerm`` - Required. A pod affinity term, associated with the corresponding weight.
       * **weight** ``int`` - weight associated with matching the corresponding podAffinityTerm, in the
         range 1-100.
     """
     podAffinityTerm: 'PodAffinityTerm'
     weight: 'int'
 
 
 @dataclass
 class WindowsSecurityContextOptions(DictMixin):
-    """WindowsSecurityContextOptions contain Windows-specific options and
+    r"""WindowsSecurityContextOptions contain Windows-specific options and
       credentials.
 
       **parameters**
 
       * **gmsaCredentialSpec** ``Optional[str]`` - GMSACredentialSpec is where the GMSA admission webhook
         (https://github.com/kubernetes-sigs/windows-gmsa) inlines the contents of the
         GMSA credential spec named by the GMSACredentialSpecName field.
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/discovery_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/discovery_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from . import core_v1
 from . import meta_v1
+from . import core_v1
 
 
 @dataclass
 class Endpoint(DictMixin):
-    """Endpoint represents a single logical "backend" implementing a service.
+    r"""Endpoint represents a single logical "backend" implementing a service.
 
       **parameters**
 
       * **addresses** ``List[str]`` - addresses of this endpoint. The contents of this field are interpreted
         according to the corresponding EndpointSlice addressType field. Consumers must
         handle different types of addresses in the context of their own capabilities.
         This must contain at least one address but no more than 100. These are all
@@ -47,15 +47,15 @@
     nodeName: 'Optional[str]' = None
     targetRef: 'Optional[core_v1.ObjectReference]' = None
     zone: 'Optional[str]' = None
 
 
 @dataclass
 class EndpointConditions(DictMixin):
-    """EndpointConditions represents the current condition of an endpoint.
+    r"""EndpointConditions represents the current condition of an endpoint.
 
       **parameters**
 
       * **ready** ``Optional[bool]`` - ready indicates that this endpoint is prepared to receive traffic, according
         to whatever system is managing the endpoint. A nil value indicates an unknown
         state. In most cases consumers should interpret this unknown state as ready.
         For compatibility reasons, ready should never be "true" for terminating
@@ -73,27 +73,27 @@
     ready: 'Optional[bool]' = None
     serving: 'Optional[bool]' = None
     terminating: 'Optional[bool]' = None
 
 
 @dataclass
 class EndpointHints(DictMixin):
-    """EndpointHints provides hints describing how an endpoint should be consumed.
+    r"""EndpointHints provides hints describing how an endpoint should be consumed.
 
       **parameters**
 
       * **forZones** ``Optional[List[ForZone]]`` - forZones indicates the zone(s) this endpoint should be consumed by to enable
         topology aware routing.
     """
     forZones: 'Optional[List[ForZone]]' = None
 
 
 @dataclass
 class EndpointPort(DictMixin):
-    """EndpointPort represents a Port used by an EndpointSlice
+    r"""EndpointPort represents a Port used by an EndpointSlice
 
       **parameters**
 
       * **appProtocol** ``Optional[str]`` - The application protocol for this port. This is used as a hint for
         implementations to offer richer behavior for protocols that they understand.
         This field follows standard Kubernetes label syntax. Valid values are either:
         * Un-prefixed protocol names - reserved for IANA standard service names (as
@@ -124,15 +124,15 @@
     name: 'Optional[str]' = None
     port: 'Optional[int]' = None
     protocol: 'Optional[str]' = None
 
 
 @dataclass
 class EndpointSlice(DictMixin):
-    """EndpointSlice represents a subset of the endpoints that implement a service.
+    r"""EndpointSlice represents a subset of the endpoints that implement a service.
       For a given service there may be multiple EndpointSlice objects, selected by
       labels, which must be joined to produce the full set of endpoints.
 
       **parameters**
 
       * **addressType** ``str`` - addressType specifies the type of address carried by this EndpointSlice. All
         addresses in this slice must be the same type. This field is immutable after
@@ -161,15 +161,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     ports: 'Optional[List[EndpointPort]]' = None
 
 
 @dataclass
 class EndpointSliceList(DictMixin):
-    """EndpointSliceList represents a list of endpoint slices
+    r"""EndpointSliceList represents a list of endpoint slices
 
       **parameters**
 
       * **items** ``List[EndpointSlice]`` - items is the list of endpoint slices
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -184,15 +184,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ForZone(DictMixin):
-    """ForZone provides information about which zones should consume this endpoint.
+    r"""ForZone provides information about which zones should consume this endpoint.
 
       **parameters**
 
       * **name** ``str`` - name represents the name of the zone.
     """
     name: 'str'
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/events_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/events_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from . import core_v1
 from . import meta_v1
+from . import core_v1
 
 
 @dataclass
 class Event(DictMixin):
-    """Event is a report of an event somewhere in the cluster. It generally denotes
+    r"""Event is a report of an event somewhere in the cluster. It generally denotes
       some state change in the system. Events have a limited retention time and
       triggers and messages may evolve with time.  Event consumers should not rely
       on the timing of an event with a given Reason reflecting a consistent
       underlying trigger, or the continued existence of events with that Reason.
       Events should be treated as informative, best-effort, supplemental data.
 
       **parameters**
@@ -81,15 +81,15 @@
     reportingInstance: 'Optional[str]' = None
     series: 'Optional[EventSeries]' = None
     type: 'Optional[str]' = None
 
 
 @dataclass
 class EventList(DictMixin):
-    """EventList is a list of Event objects.
+    r"""EventList is a list of Event objects.
 
       **parameters**
 
       * **items** ``List[Event]`` - items is a list of schema objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -105,15 +105,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class EventSeries(DictMixin):
-    """EventSeries contain information on series of events, i.e. thing that was/is
+    r"""EventSeries contain information on series of events, i.e. thing that was/is
       happening continuously for some time. How often to update the EventSeries is
       up to the event reporters. The default event reporter in
       "k8s.io/client-go/tools/events/event_broadcaster.go" shows how this struct is
       updated on heartbeats and can guide customized reporter implementations.
 
       **parameters**
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/flowcontrol_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/flowcontrol_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class ExemptPriorityLevelConfiguration(DictMixin):
-    """ExemptPriorityLevelConfiguration describes the configurable aspects of the
+    r"""ExemptPriorityLevelConfiguration describes the configurable aspects of the
       handling of exempt requests. In the mandatory exempt configuration object the
       values in the fields here can be modified by authorized users, unlike the rest
       of the `spec`.
 
       **parameters**
 
       * **lendablePercent** ``Optional[int]`` - `lendablePercent` prescribes the fraction of the level's NominalCL that can be
@@ -38,27 +38,27 @@
     """
     lendablePercent: 'Optional[int]' = None
     nominalConcurrencyShares: 'Optional[int]' = None
 
 
 @dataclass
 class FlowDistinguisherMethod(DictMixin):
-    """FlowDistinguisherMethod specifies the method of a flow distinguisher.
+    r"""FlowDistinguisherMethod specifies the method of a flow distinguisher.
 
       **parameters**
 
       * **type** ``str`` - `type` is the type of flow distinguisher method The supported types are
         "ByUser" and "ByNamespace". Required.
     """
     type: 'str'
 
 
 @dataclass
 class FlowSchema(DictMixin):
-    """FlowSchema defines the schema of a group of flows. Note that a flow is made up
+    r"""FlowSchema defines the schema of a group of flows. Note that a flow is made up
       of a set of inbound API requests with similar attributes and is identified by
       a pair of strings: the name of the FlowSchema and a "flow distinguisher".
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -81,15 +81,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[FlowSchemaSpec]' = None
     status: 'Optional[FlowSchemaStatus]' = None
 
 
 @dataclass
 class FlowSchemaCondition(DictMixin):
-    """FlowSchemaCondition describes conditions for a FlowSchema.
+    r"""FlowSchemaCondition describes conditions for a FlowSchema.
 
       **parameters**
 
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - `lastTransitionTime` is the last time the condition transitioned from one
         status to another.
       * **message** ``Optional[str]`` - `message` is a human-readable message indicating details about last
         transition.
@@ -104,15 +104,15 @@
     reason: 'Optional[str]' = None
     status: 'Optional[str]' = None
     type: 'Optional[str]' = None
 
 
 @dataclass
 class FlowSchemaList(DictMixin):
-    """FlowSchemaList is a list of FlowSchema objects.
+    r"""FlowSchemaList is a list of FlowSchema objects.
 
       **parameters**
 
       * **items** ``List[FlowSchema]`` - `items` is a list of FlowSchemas.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -128,15 +128,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class FlowSchemaSpec(DictMixin):
-    """FlowSchemaSpec describes how the FlowSchema's specification looks like.
+    r"""FlowSchemaSpec describes how the FlowSchema's specification looks like.
 
       **parameters**
 
       * **priorityLevelConfiguration** ``PriorityLevelConfigurationReference`` - `priorityLevelConfiguration` should reference a PriorityLevelConfiguration in
         the cluster. If the reference cannot be resolved, the FlowSchema will be
         ignored and marked as invalid in its status. Required.
       * **distinguisherMethod** ``Optional[FlowDistinguisherMethod]`` - `distinguisherMethod` defines how to compute the flow distinguisher for
@@ -156,39 +156,39 @@
     distinguisherMethod: 'Optional[FlowDistinguisherMethod]' = None
     matchingPrecedence: 'Optional[int]' = None
     rules: 'Optional[List[PolicyRulesWithSubjects]]' = None
 
 
 @dataclass
 class FlowSchemaStatus(DictMixin):
-    """FlowSchemaStatus represents the current state of a FlowSchema.
+    r"""FlowSchemaStatus represents the current state of a FlowSchema.
 
       **parameters**
 
       * **conditions** ``Optional[List[FlowSchemaCondition]]`` - `conditions` is a list of the current states of FlowSchema.
     """
     conditions: 'Optional[List[FlowSchemaCondition]]' = None
 
 
 @dataclass
 class GroupSubject(DictMixin):
-    """GroupSubject holds detailed information for group-kind subject.
+    r"""GroupSubject holds detailed information for group-kind subject.
 
       **parameters**
 
       * **name** ``str`` - name is the user group that matches, or "*" to match all user groups. See
         https://github.com/kubernetes/apiserver/blob/master/pkg/authentication/user/user.go
         for some well-known group names. Required.
     """
     name: 'str'
 
 
 @dataclass
 class LimitResponse(DictMixin):
-    """LimitResponse defines how to handle requests that can not be executed right
+    r"""LimitResponse defines how to handle requests that can not be executed right
       now.
 
       **parameters**
 
       * **type** ``str`` - `type` is "Queue" or "Reject". "Queue" means that requests that can not be
         executed upon arrival are held in a queue until they can be executed or a
         queuing limit is reached. "Reject" means that requests that can not be
@@ -198,15 +198,15 @@
     """
     type: 'str'
     queuing: 'Optional[QueuingConfiguration]' = None
 
 
 @dataclass
 class LimitedPriorityLevelConfiguration(DictMixin):
-    """LimitedPriorityLevelConfiguration specifies how to handle requests that are
+    r"""LimitedPriorityLevelConfiguration specifies how to handle requests that are
       subject to limits. It addresses two issues:
         - How are requests for this priority level limited?
         - What should be done with requests that exceed the limit?
 
       **parameters**
 
       * **borrowingLimitPercent** ``Optional[int]`` - `borrowingLimitPercent`, if present, configures a limit on how many seats this
@@ -248,15 +248,15 @@
     lendablePercent: 'Optional[int]' = None
     limitResponse: 'Optional[LimitResponse]' = None
     nominalConcurrencyShares: 'Optional[int]' = None
 
 
 @dataclass
 class NonResourcePolicyRule(DictMixin):
-    """NonResourcePolicyRule is a predicate that matches non-resource requests
+    r"""NonResourcePolicyRule is a predicate that matches non-resource requests
       according to their verb and the target non-resource URL. A
       NonResourcePolicyRule matches a request if and only if both (a) at least one
       member of verbs matches the request and (b) at least one member of
       nonResourceURLs matches the request.
 
       **parameters**
 
@@ -274,15 +274,15 @@
     """
     nonResourceURLs: 'List[str]'
     verbs: 'List[str]'
 
 
 @dataclass
 class PolicyRulesWithSubjects(DictMixin):
-    """PolicyRulesWithSubjects prescribes a test that applies to a request to an
+    r"""PolicyRulesWithSubjects prescribes a test that applies to a request to an
       apiserver. The test considers the subject making the request, the verb being
       requested, and the resource to be acted upon. This PolicyRulesWithSubjects
       matches a request if and only if both (a) at least one member of subjects
       matches the request and (b) at least one member of resourceRules or
       nonResourceRules matches the request.
 
       **parameters**
@@ -300,15 +300,15 @@
     subjects: 'List[Subject]'
     nonResourceRules: 'Optional[List[NonResourcePolicyRule]]' = None
     resourceRules: 'Optional[List[ResourcePolicyRule]]' = None
 
 
 @dataclass
 class PriorityLevelConfiguration(DictMixin):
-    """PriorityLevelConfiguration represents the configuration of a priority level.
+    r"""PriorityLevelConfiguration represents the configuration of a priority level.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -329,15 +329,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[PriorityLevelConfigurationSpec]' = None
     status: 'Optional[PriorityLevelConfigurationStatus]' = None
 
 
 @dataclass
 class PriorityLevelConfigurationCondition(DictMixin):
-    """PriorityLevelConfigurationCondition defines the condition of priority level.
+    r"""PriorityLevelConfigurationCondition defines the condition of priority level.
 
       **parameters**
 
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - `lastTransitionTime` is the last time the condition transitioned from one
         status to another.
       * **message** ``Optional[str]`` - `message` is a human-readable message indicating details about last
         transition.
@@ -352,15 +352,15 @@
     reason: 'Optional[str]' = None
     status: 'Optional[str]' = None
     type: 'Optional[str]' = None
 
 
 @dataclass
 class PriorityLevelConfigurationList(DictMixin):
-    """PriorityLevelConfigurationList is a list of PriorityLevelConfiguration
+    r"""PriorityLevelConfigurationList is a list of PriorityLevelConfiguration
       objects.
 
       **parameters**
 
       * **items** ``List[PriorityLevelConfiguration]`` - `items` is a list of request-priorities.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -377,28 +377,28 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class PriorityLevelConfigurationReference(DictMixin):
-    """PriorityLevelConfigurationReference contains information that points to the
+    r"""PriorityLevelConfigurationReference contains information that points to the
       "request-priority" being used.
 
       **parameters**
 
       * **name** ``str`` - `name` is the name of the priority level configuration being referenced
         Required.
     """
     name: 'str'
 
 
 @dataclass
 class PriorityLevelConfigurationSpec(DictMixin):
-    """PriorityLevelConfigurationSpec specifies the configuration of a priority
+    r"""PriorityLevelConfigurationSpec specifies the configuration of a priority
       level.
 
       **parameters**
 
       * **type** ``str`` - `type` indicates whether this priority level is subject to limitation on
         request execution.  A value of `"Exempt"` means that requests of this priority
         level are not subject to a limit (and thus are never queued) and do not
@@ -416,27 +416,27 @@
     type: 'str'
     exempt: 'Optional[ExemptPriorityLevelConfiguration]' = None
     limited: 'Optional[LimitedPriorityLevelConfiguration]' = None
 
 
 @dataclass
 class PriorityLevelConfigurationStatus(DictMixin):
-    """PriorityLevelConfigurationStatus represents the current state of a
+    r"""PriorityLevelConfigurationStatus represents the current state of a
       "request-priority".
 
       **parameters**
 
       * **conditions** ``Optional[List[PriorityLevelConfigurationCondition]]`` - `conditions` is the current state of "request-priority".
     """
     conditions: 'Optional[List[PriorityLevelConfigurationCondition]]' = None
 
 
 @dataclass
 class QueuingConfiguration(DictMixin):
-    """QueuingConfiguration holds the configuration parameters for queuing
+    r"""QueuingConfiguration holds the configuration parameters for queuing
 
       **parameters**
 
       * **handSize** ``Optional[int]`` - `handSize` is a small positive number that configures the shuffle sharding of
         requests into queues.  When enqueuing a request at this priority level the
         request's flow identifier (a string pair) is hashed and the hash value is used
         to shuffle the list of queues and deal a hand of the size specified here.  The
@@ -456,15 +456,15 @@
     handSize: 'Optional[int]' = None
     queueLengthLimit: 'Optional[int]' = None
     queues: 'Optional[int]' = None
 
 
 @dataclass
 class ResourcePolicyRule(DictMixin):
-    """ResourcePolicyRule is a predicate that matches some resource requests, testing
+    r"""ResourcePolicyRule is a predicate that matches some resource requests, testing
       the request's verb and the target resource. A ResourcePolicyRule matches a
       resource request if and only if: (a) at least one member of verbs matches the
       request, (b) at least one member of apiGroups matches the request, (c) at
       least one member of resources matches the request, and (d) either (d1) the
       request does not specify a namespace (i.e., `Namespace==""`) and clusterScope
       is true or (d2) the request specifies a namespace and least one member of
       namespaces matches the request's namespace.
@@ -495,30 +495,30 @@
     verbs: 'List[str]'
     clusterScope: 'Optional[bool]' = None
     namespaces: 'Optional[List[str]]' = None
 
 
 @dataclass
 class ServiceAccountSubject(DictMixin):
-    """ServiceAccountSubject holds detailed information for service-account-kind
+    r"""ServiceAccountSubject holds detailed information for service-account-kind
       subject.
 
       **parameters**
 
       * **name** ``str`` - `name` is the name of matching ServiceAccount objects, or "*" to match
         regardless of name. Required.
       * **namespace** ``str`` - `namespace` is the namespace of matching ServiceAccount objects. Required.
     """
     name: 'str'
     namespace: 'str'
 
 
 @dataclass
 class Subject(DictMixin):
-    """Subject matches the originator of a request, as identified by the request
+    r"""Subject matches the originator of a request, as identified by the request
       authentication system. There are three ways of matching an originator; by
       user, group, or service account.
 
       **parameters**
 
       * **kind** ``str`` - `kind` indicates which one of the other fields is non-empty. Required
       * **group** ``Optional[GroupSubject]`` - `group` matches based on user group name.
@@ -529,15 +529,15 @@
     group: 'Optional[GroupSubject]' = None
     serviceAccount: 'Optional[ServiceAccountSubject]' = None
     user: 'Optional[UserSubject]' = None
 
 
 @dataclass
 class UserSubject(DictMixin):
-    """UserSubject holds detailed information for user-kind subject.
+    r"""UserSubject holds detailed information for user-kind subject.
 
       **parameters**
 
       * **name** ``str`` - `name` is the username that matches, or "*" to match all usernames. Required.
     """
     name: 'str'
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/flowcontrol_v1beta3.py` & `lightkube-models-1.30.0.8/lightkube/models/flowcontrol_v1beta3.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class ExemptPriorityLevelConfiguration(DictMixin):
-    """ExemptPriorityLevelConfiguration describes the configurable aspects of the
+    r"""ExemptPriorityLevelConfiguration describes the configurable aspects of the
       handling of exempt requests. In the mandatory exempt configuration object the
       values in the fields here can be modified by authorized users, unlike the rest
       of the `spec`.
 
       **parameters**
 
       * **lendablePercent** ``Optional[int]`` - `lendablePercent` prescribes the fraction of the level's NominalCL that can be
@@ -38,27 +38,27 @@
     """
     lendablePercent: 'Optional[int]' = None
     nominalConcurrencyShares: 'Optional[int]' = None
 
 
 @dataclass
 class FlowDistinguisherMethod(DictMixin):
-    """FlowDistinguisherMethod specifies the method of a flow distinguisher.
+    r"""FlowDistinguisherMethod specifies the method of a flow distinguisher.
 
       **parameters**
 
       * **type** ``str`` - `type` is the type of flow distinguisher method The supported types are
         "ByUser" and "ByNamespace". Required.
     """
     type: 'str'
 
 
 @dataclass
 class FlowSchema(DictMixin):
-    """FlowSchema defines the schema of a group of flows. Note that a flow is made up
+    r"""FlowSchema defines the schema of a group of flows. Note that a flow is made up
       of a set of inbound API requests with similar attributes and is identified by
       a pair of strings: the name of the FlowSchema and a "flow distinguisher".
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -81,15 +81,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[FlowSchemaSpec]' = None
     status: 'Optional[FlowSchemaStatus]' = None
 
 
 @dataclass
 class FlowSchemaCondition(DictMixin):
-    """FlowSchemaCondition describes conditions for a FlowSchema.
+    r"""FlowSchemaCondition describes conditions for a FlowSchema.
 
       **parameters**
 
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - `lastTransitionTime` is the last time the condition transitioned from one
         status to another.
       * **message** ``Optional[str]`` - `message` is a human-readable message indicating details about last
         transition.
@@ -104,15 +104,15 @@
     reason: 'Optional[str]' = None
     status: 'Optional[str]' = None
     type: 'Optional[str]' = None
 
 
 @dataclass
 class FlowSchemaList(DictMixin):
-    """FlowSchemaList is a list of FlowSchema objects.
+    r"""FlowSchemaList is a list of FlowSchema objects.
 
       **parameters**
 
       * **items** ``List[FlowSchema]`` - `items` is a list of FlowSchemas.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -128,15 +128,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class FlowSchemaSpec(DictMixin):
-    """FlowSchemaSpec describes how the FlowSchema's specification looks like.
+    r"""FlowSchemaSpec describes how the FlowSchema's specification looks like.
 
       **parameters**
 
       * **priorityLevelConfiguration** ``PriorityLevelConfigurationReference`` - `priorityLevelConfiguration` should reference a PriorityLevelConfiguration in
         the cluster. If the reference cannot be resolved, the FlowSchema will be
         ignored and marked as invalid in its status. Required.
       * **distinguisherMethod** ``Optional[FlowDistinguisherMethod]`` - `distinguisherMethod` defines how to compute the flow distinguisher for
@@ -156,39 +156,39 @@
     distinguisherMethod: 'Optional[FlowDistinguisherMethod]' = None
     matchingPrecedence: 'Optional[int]' = None
     rules: 'Optional[List[PolicyRulesWithSubjects]]' = None
 
 
 @dataclass
 class FlowSchemaStatus(DictMixin):
-    """FlowSchemaStatus represents the current state of a FlowSchema.
+    r"""FlowSchemaStatus represents the current state of a FlowSchema.
 
       **parameters**
 
       * **conditions** ``Optional[List[FlowSchemaCondition]]`` - `conditions` is a list of the current states of FlowSchema.
     """
     conditions: 'Optional[List[FlowSchemaCondition]]' = None
 
 
 @dataclass
 class GroupSubject(DictMixin):
-    """GroupSubject holds detailed information for group-kind subject.
+    r"""GroupSubject holds detailed information for group-kind subject.
 
       **parameters**
 
       * **name** ``str`` - name is the user group that matches, or "*" to match all user groups. See
         https://github.com/kubernetes/apiserver/blob/master/pkg/authentication/user/user.go
         for some well-known group names. Required.
     """
     name: 'str'
 
 
 @dataclass
 class LimitResponse(DictMixin):
-    """LimitResponse defines how to handle requests that can not be executed right
+    r"""LimitResponse defines how to handle requests that can not be executed right
       now.
 
       **parameters**
 
       * **type** ``str`` - `type` is "Queue" or "Reject". "Queue" means that requests that can not be
         executed upon arrival are held in a queue until they can be executed or a
         queuing limit is reached. "Reject" means that requests that can not be
@@ -198,15 +198,15 @@
     """
     type: 'str'
     queuing: 'Optional[QueuingConfiguration]' = None
 
 
 @dataclass
 class LimitedPriorityLevelConfiguration(DictMixin):
-    """LimitedPriorityLevelConfiguration specifies how to handle requests that are
+    r"""LimitedPriorityLevelConfiguration specifies how to handle requests that are
       subject to limits. It addresses two issues:
         - How are requests for this priority level limited?
         - What should be done with requests that exceed the limit?
 
       **parameters**
 
       * **borrowingLimitPercent** ``Optional[int]`` - `borrowingLimitPercent`, if present, configures a limit on how many seats this
@@ -245,15 +245,15 @@
     lendablePercent: 'Optional[int]' = None
     limitResponse: 'Optional[LimitResponse]' = None
     nominalConcurrencyShares: 'Optional[int]' = None
 
 
 @dataclass
 class NonResourcePolicyRule(DictMixin):
-    """NonResourcePolicyRule is a predicate that matches non-resource requests
+    r"""NonResourcePolicyRule is a predicate that matches non-resource requests
       according to their verb and the target non-resource URL. A
       NonResourcePolicyRule matches a request if and only if both (a) at least one
       member of verbs matches the request and (b) at least one member of
       nonResourceURLs matches the request.
 
       **parameters**
 
@@ -271,15 +271,15 @@
     """
     nonResourceURLs: 'List[str]'
     verbs: 'List[str]'
 
 
 @dataclass
 class PolicyRulesWithSubjects(DictMixin):
-    """PolicyRulesWithSubjects prescribes a test that applies to a request to an
+    r"""PolicyRulesWithSubjects prescribes a test that applies to a request to an
       apiserver. The test considers the subject making the request, the verb being
       requested, and the resource to be acted upon. This PolicyRulesWithSubjects
       matches a request if and only if both (a) at least one member of subjects
       matches the request and (b) at least one member of resourceRules or
       nonResourceRules matches the request.
 
       **parameters**
@@ -297,15 +297,15 @@
     subjects: 'List[Subject]'
     nonResourceRules: 'Optional[List[NonResourcePolicyRule]]' = None
     resourceRules: 'Optional[List[ResourcePolicyRule]]' = None
 
 
 @dataclass
 class PriorityLevelConfiguration(DictMixin):
-    """PriorityLevelConfiguration represents the configuration of a priority level.
+    r"""PriorityLevelConfiguration represents the configuration of a priority level.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -326,15 +326,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[PriorityLevelConfigurationSpec]' = None
     status: 'Optional[PriorityLevelConfigurationStatus]' = None
 
 
 @dataclass
 class PriorityLevelConfigurationCondition(DictMixin):
-    """PriorityLevelConfigurationCondition defines the condition of priority level.
+    r"""PriorityLevelConfigurationCondition defines the condition of priority level.
 
       **parameters**
 
       * **lastTransitionTime** ``Optional[meta_v1.Time]`` - `lastTransitionTime` is the last time the condition transitioned from one
         status to another.
       * **message** ``Optional[str]`` - `message` is a human-readable message indicating details about last
         transition.
@@ -349,15 +349,15 @@
     reason: 'Optional[str]' = None
     status: 'Optional[str]' = None
     type: 'Optional[str]' = None
 
 
 @dataclass
 class PriorityLevelConfigurationList(DictMixin):
-    """PriorityLevelConfigurationList is a list of PriorityLevelConfiguration
+    r"""PriorityLevelConfigurationList is a list of PriorityLevelConfiguration
       objects.
 
       **parameters**
 
       * **items** ``List[PriorityLevelConfiguration]`` - `items` is a list of request-priorities.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -374,28 +374,28 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class PriorityLevelConfigurationReference(DictMixin):
-    """PriorityLevelConfigurationReference contains information that points to the
+    r"""PriorityLevelConfigurationReference contains information that points to the
       "request-priority" being used.
 
       **parameters**
 
       * **name** ``str`` - `name` is the name of the priority level configuration being referenced
         Required.
     """
     name: 'str'
 
 
 @dataclass
 class PriorityLevelConfigurationSpec(DictMixin):
-    """PriorityLevelConfigurationSpec specifies the configuration of a priority
+    r"""PriorityLevelConfigurationSpec specifies the configuration of a priority
       level.
 
       **parameters**
 
       * **type** ``str`` - `type` indicates whether this priority level is subject to limitation on
         request execution.  A value of `"Exempt"` means that requests of this priority
         level are not subject to a limit (and thus are never queued) and do not
@@ -413,27 +413,27 @@
     type: 'str'
     exempt: 'Optional[ExemptPriorityLevelConfiguration]' = None
     limited: 'Optional[LimitedPriorityLevelConfiguration]' = None
 
 
 @dataclass
 class PriorityLevelConfigurationStatus(DictMixin):
-    """PriorityLevelConfigurationStatus represents the current state of a
+    r"""PriorityLevelConfigurationStatus represents the current state of a
       "request-priority".
 
       **parameters**
 
       * **conditions** ``Optional[List[PriorityLevelConfigurationCondition]]`` - `conditions` is the current state of "request-priority".
     """
     conditions: 'Optional[List[PriorityLevelConfigurationCondition]]' = None
 
 
 @dataclass
 class QueuingConfiguration(DictMixin):
-    """QueuingConfiguration holds the configuration parameters for queuing
+    r"""QueuingConfiguration holds the configuration parameters for queuing
 
       **parameters**
 
       * **handSize** ``Optional[int]`` - `handSize` is a small positive number that configures the shuffle sharding of
         requests into queues.  When enqueuing a request at this priority level the
         request's flow identifier (a string pair) is hashed and the hash value is used
         to shuffle the list of queues and deal a hand of the size specified here.  The
@@ -453,15 +453,15 @@
     handSize: 'Optional[int]' = None
     queueLengthLimit: 'Optional[int]' = None
     queues: 'Optional[int]' = None
 
 
 @dataclass
 class ResourcePolicyRule(DictMixin):
-    """ResourcePolicyRule is a predicate that matches some resource requests, testing
+    r"""ResourcePolicyRule is a predicate that matches some resource requests, testing
       the request's verb and the target resource. A ResourcePolicyRule matches a
       resource request if and only if: (a) at least one member of verbs matches the
       request, (b) at least one member of apiGroups matches the request, (c) at
       least one member of resources matches the request, and (d) either (d1) the
       request does not specify a namespace (i.e., `Namespace==""`) and clusterScope
       is true or (d2) the request specifies a namespace and least one member of
       namespaces matches the request's namespace.
@@ -492,30 +492,30 @@
     verbs: 'List[str]'
     clusterScope: 'Optional[bool]' = None
     namespaces: 'Optional[List[str]]' = None
 
 
 @dataclass
 class ServiceAccountSubject(DictMixin):
-    """ServiceAccountSubject holds detailed information for service-account-kind
+    r"""ServiceAccountSubject holds detailed information for service-account-kind
       subject.
 
       **parameters**
 
       * **name** ``str`` - `name` is the name of matching ServiceAccount objects, or "*" to match
         regardless of name. Required.
       * **namespace** ``str`` - `namespace` is the namespace of matching ServiceAccount objects. Required.
     """
     name: 'str'
     namespace: 'str'
 
 
 @dataclass
 class Subject(DictMixin):
-    """Subject matches the originator of a request, as identified by the request
+    r"""Subject matches the originator of a request, as identified by the request
       authentication system. There are three ways of matching an originator; by
       user, group, or service account.
 
       **parameters**
 
       * **kind** ``str`` - `kind` indicates which one of the other fields is non-empty. Required
       * **group** ``Optional[GroupSubject]`` - `group` matches based on user group name.
@@ -526,15 +526,15 @@
     group: 'Optional[GroupSubject]' = None
     serviceAccount: 'Optional[ServiceAccountSubject]' = None
     user: 'Optional[UserSubject]' = None
 
 
 @dataclass
 class UserSubject(DictMixin):
-    """UserSubject holds detailed information for user-kind subject.
+    r"""UserSubject holds detailed information for user-kind subject.
 
       **parameters**
 
       * **name** ``str`` - `name` is the username that matches, or "*" to match all usernames. Required.
     """
     name: 'str'
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/meta_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/meta_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
 from . import runtime
-from typing import Dict
 from datetime import datetime
+from typing import Dict
 
 
 @dataclass
 class APIGroup(DictMixin):
-    """APIGroup contains the name, the supported versions, and the preferred version
+    r"""APIGroup contains the name, the supported versions, and the preferred version
       of a group.
 
       **parameters**
 
       * **name** ``str`` - name is the name of the group.
       * **versions** ``List[GroupVersionForDiscovery]`` - versions are the versions supported in this group.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
@@ -46,15 +46,15 @@
     kind: 'Optional[str]' = None
     preferredVersion: 'Optional[GroupVersionForDiscovery]' = None
     serverAddressByClientCIDRs: 'Optional[List[ServerAddressByClientCIDR]]' = None
 
 
 @dataclass
 class APIGroupList(DictMixin):
-    """APIGroupList is a list of APIGroup, to allow clients to discover the API at
+    r"""APIGroupList is a list of APIGroup, to allow clients to discover the API at
       /apis.
 
       **parameters**
 
       * **groups** ``List[APIGroup]`` - groups is a list of APIGroup.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -68,15 +68,15 @@
     groups: 'List[APIGroup]'
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
 
 
 @dataclass
 class APIResource(DictMixin):
-    """APIResource specifies the name of a resource and whether it is namespaced.
+    r"""APIResource specifies the name of a resource and whether it is namespaced.
 
       **parameters**
 
       * **kind** ``str`` - kind is the kind for the resource (e.g. 'Foo' is the kind for a resource
         'foo')
       * **name** ``str`` - name is the plural name of the resource.
       * **namespaced** ``bool`` - namespaced indicates if a resource is namespaced or not.
@@ -113,15 +113,15 @@
     shortNames: 'Optional[List[str]]' = None
     storageVersionHash: 'Optional[str]' = None
     version: 'Optional[str]' = None
 
 
 @dataclass
 class APIResourceList(DictMixin):
-    """APIResourceList is a list of APIResource, it is used to expose the name of the
+    r"""APIResourceList is a list of APIResource, it is used to expose the name of the
       resources supported in a specific group and version, and if the resource is
       namespaced.
 
       **parameters**
 
       * **groupVersion** ``str`` - groupVersion is the group and version this APIResourceList is for.
       * **resources** ``List[APIResource]`` - resources contains the name of the resources and if they are namespaced.
@@ -138,15 +138,15 @@
     resources: 'List[APIResource]'
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
 
 
 @dataclass
 class APIVersions(DictMixin):
-    """APIVersions lists the versions that are available, to allow clients to
+    r"""APIVersions lists the versions that are available, to allow clients to
       discover the API at /api, which is the root path of the legacy v1 API.
 
       **parameters**
 
       * **serverAddressByClientCIDRs** ``List[ServerAddressByClientCIDR]`` - a map of client CIDR to server address that is serving this group. This is to
         help clients reach servers in the most network-efficient way possible. Clients
         can use the appropriate server address as per the CIDR that they match. In
@@ -170,15 +170,15 @@
     versions: 'List[str]'
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
 
 
 @dataclass
 class Condition(DictMixin):
-    """Condition contains details for one aspect of the current state of this API
+    r"""Condition contains details for one aspect of the current state of this API
       Resource.
 
       **parameters**
 
       * **lastTransitionTime** ``Time`` - lastTransitionTime is the last time the condition transitioned from one status
         to another. This should be when the underlying condition changed.  If that is
         not known, then using the time when the API field changed is acceptable.
@@ -202,15 +202,15 @@
     status: 'str'
     type: 'str'
     observedGeneration: 'Optional[int]' = None
 
 
 @dataclass
 class DeleteOptions(DictMixin):
-    """DeleteOptions may be provided when deleting an API object.
+    r"""DeleteOptions may be provided when deleting an API object.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -251,30 +251,30 @@
 
 
 FieldsV1 = Dict
 
 
 @dataclass
 class GroupVersionForDiscovery(DictMixin):
-    """GroupVersion contains the "group/version" and "version" string of a version.
+    r"""GroupVersion contains the "group/version" and "version" string of a version.
       It is made a struct to keep extensibility.
 
       **parameters**
 
       * **groupVersion** ``str`` - groupVersion specifies the API group and version in the form "group/version"
       * **version** ``str`` - version specifies the version in the form of "version". This is to save the
         clients the trouble of splitting the GroupVersion.
     """
     groupVersion: 'str'
     version: 'str'
 
 
 @dataclass
 class LabelSelector(DictMixin):
-    """A label selector is a label query over a set of resources. The result of
+    r"""A label selector is a label query over a set of resources. The result of
       matchLabels and matchExpressions are ANDed. An empty label selector matches
       all objects. A null label selector matches no objects.
 
       **parameters**
 
       * **matchExpressions** ``Optional[List[LabelSelectorRequirement]]`` - matchExpressions is a list of label selector requirements. The requirements
         are ANDed.
@@ -285,15 +285,15 @@
     """
     matchExpressions: 'Optional[List[LabelSelectorRequirement]]' = None
     matchLabels: 'Optional[dict]' = None
 
 
 @dataclass
 class LabelSelectorRequirement(DictMixin):
-    """A label selector requirement is a selector that contains values, a key, and an
+    r"""A label selector requirement is a selector that contains values, a key, and an
       operator that relates the key and values.
 
       **parameters**
 
       * **key** ``str`` - key is the label key that the selector applies to.
       * **operator** ``str`` - operator represents a key's relationship to a set of values. Valid operators
         are In, NotIn, Exists and DoesNotExist.
@@ -305,15 +305,15 @@
     key: 'str'
     operator: 'str'
     values: 'Optional[List[str]]' = None
 
 
 @dataclass
 class ListMeta(DictMixin):
-    """ListMeta describes metadata that synthetic resources must have, including
+    r"""ListMeta describes metadata that synthetic resources must have, including
       lists and various status objects. A resource may have only one of {ObjectMeta,
       ListMeta}.
 
       **parameters**
 
       * **continue_** ``Optional[str]`` - continue may be set if the user set a limit on the number of items returned,
         and indicates that the server has more data available. The value is opaque and
@@ -344,15 +344,15 @@
     remainingItemCount: 'Optional[int]' = None
     resourceVersion: 'Optional[str]' = None
     selfLink: 'Optional[str]' = None
 
 
 @dataclass
 class ManagedFieldsEntry(DictMixin):
-    """ManagedFieldsEntry is a workflow-id, a FieldSet and the group version of the
+    r"""ManagedFieldsEntry is a workflow-id, a FieldSet and the group version of the
       resource that the fieldset applies to.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the version of this resource that this field set applies
         to. The format is "group/version" just like the top-level APIVersion field. It
         is necessary to track the version of a field set because it cannot be
@@ -386,15 +386,15 @@
 
 
 MicroTime = datetime
 
 
 @dataclass
 class ObjectMeta(DictMixin):
-    """ObjectMeta is metadata that all persisted resources must have, which includes
+    r"""ObjectMeta is metadata that all persisted resources must have, which includes
       all objects users must create.
 
       **parameters**
 
       * **annotations** ``Optional[dict]`` - Annotations is an unstructured key value map stored with a resource that may
         be set by external tools to store and retrieve arbitrary metadata. They are
         not queryable and should be preserved when modifying objects. More info:
@@ -510,15 +510,15 @@
     resourceVersion: 'Optional[str]' = None
     selfLink: 'Optional[str]' = None
     uid: 'Optional[str]' = None
 
 
 @dataclass
 class OwnerReference(DictMixin):
-    """OwnerReference contains enough information to let you identify an owning
+    r"""OwnerReference contains enough information to let you identify an owning
       object. An owning object must be in the same namespace as the dependent, or be
       cluster-scoped, so there is no namespace field.
 
       **parameters**
 
       * **apiVersion** ``str`` - API version of the referent.
       * **kind** ``str`` - Kind of the referent. More info:
@@ -546,29 +546,29 @@
 
 
 Patch = Dict
 
 
 @dataclass
 class Preconditions(DictMixin):
-    """Preconditions must be fulfilled before an operation (update, delete, etc.) is
+    r"""Preconditions must be fulfilled before an operation (update, delete, etc.) is
       carried out.
 
       **parameters**
 
       * **resourceVersion** ``Optional[str]`` - Specifies the target ResourceVersion
       * **uid** ``Optional[str]`` - Specifies the target UID.
     """
     resourceVersion: 'Optional[str]' = None
     uid: 'Optional[str]' = None
 
 
 @dataclass
 class ServerAddressByClientCIDR(DictMixin):
-    """ServerAddressByClientCIDR helps the client to determine the server address
+    r"""ServerAddressByClientCIDR helps the client to determine the server address
       that they should use, depending on the clientCIDR that they match.
 
       **parameters**
 
       * **clientCIDR** ``str`` - The CIDR with which clients can match their IP to figure out the server
         address that they should use.
       * **serverAddress** ``str`` - Address of this server, suitable for a client that matches the above CIDR.
@@ -576,15 +576,15 @@
     """
     clientCIDR: 'str'
     serverAddress: 'str'
 
 
 @dataclass
 class Status(DictMixin):
-    """Status is a return value for calls that don't return other objects.
+    r"""Status is a return value for calls that don't return other objects.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -613,15 +613,15 @@
     metadata: 'Optional[ListMeta]' = None
     reason: 'Optional[str]' = None
     status: 'Optional[str]' = None
 
 
 @dataclass
 class StatusCause(DictMixin):
-    """StatusCause provides more information about an api.Status failure, including
+    r"""StatusCause provides more information about an api.Status failure, including
       cases when multiple errors are encountered.
 
       **parameters**
 
       * **field** ``Optional[str]`` - The field of the resource that has caused this error, as named by its JSON
         serialization. May include dot and postfix notation for nested attributes.
         Arrays are zero-indexed.  Fields may appear more than once in an array of
@@ -637,15 +637,15 @@
     field: 'Optional[str]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class StatusDetails(DictMixin):
-    """StatusDetails is a set of additional properties that MAY be set by the server
+    r"""StatusDetails is a set of additional properties that MAY be set by the server
       to provide additional information about a response. The Reason field of a
       Status object defines what attributes will be set. Clients must ignore fields
       that do not match the defined type of each attribute, and should assume that
       any attribute may be empty, invalid, or under defined.
 
       **parameters**
 
@@ -674,15 +674,15 @@
 
 
 Time = datetime
 
 
 @dataclass
 class WatchEvent(DictMixin):
-    """Event represents a single event to a watched resource.
+    r"""Event represents a single event to a watched resource.
 
       **parameters**
 
       * **object** ``runtime.RawExtension`` - Object is:
          * If Type is Added or Modified: the new state of the object.
          * If Type is Deleted: the state of the object immediately before deletion.
          * If Type is Error: *Status is recommended; other types may make sense
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/networking_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/networking_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
+from . import meta_v1
 from . import core_v1
 from . import util_intstr
-from . import meta_v1
 
 
 @dataclass
 class HTTPIngressPath(DictMixin):
-    """HTTPIngressPath associates a path with a backend. Incoming urls matching the
+    r"""HTTPIngressPath associates a path with a backend. Incoming urls matching the
       path are forwarded to the backend.
 
       **parameters**
 
       * **backend** ``IngressBackend`` - backend defines the referenced service endpoint to which the traffic will be
         forwarded to.
       * **pathType** ``str`` - pathType determines the interpretation of the path matching. PathType can be
@@ -41,29 +41,29 @@
     backend: 'IngressBackend'
     pathType: 'str'
     path: 'Optional[str]' = None
 
 
 @dataclass
 class HTTPIngressRuleValue(DictMixin):
-    """HTTPIngressRuleValue is a list of http selectors pointing to backends. In the
+    r"""HTTPIngressRuleValue is a list of http selectors pointing to backends. In the
       example: http://<host>/<path>?<searchpart> -> backend where where parts of the
       url correspond to RFC 3986, this resource will be used to match against
       everything after the last '/' and before the first '?' or '#'.
 
       **parameters**
 
       * **paths** ``List[HTTPIngressPath]`` - paths is a collection of paths that map requests to backends.
     """
     paths: 'List[HTTPIngressPath]'
 
 
 @dataclass
 class IPBlock(DictMixin):
-    """IPBlock describes a particular CIDR (Ex. "192.168.1.0/24","2001:db8::/64")
+    r"""IPBlock describes a particular CIDR (Ex. "192.168.1.0/24","2001:db8::/64")
       that is allowed to the pods matched by a NetworkPolicySpec's podSelector. The
       except entry describes CIDRs that should not be included within this rule.
 
       **parameters**
 
       * **cidr** ``str`` - cidr is a string representing the IPBlock Valid examples are "192.168.1.0/24"
         or "2001:db8::/64"
@@ -73,15 +73,15 @@
     """
     cidr: 'str'
     except_: 'Optional[List[str]]' = field(metadata={"json": "except"}, default=None)
 
 
 @dataclass
 class Ingress(DictMixin):
-    """Ingress is a collection of rules that allow inbound connections to reach the
+    r"""Ingress is a collection of rules that allow inbound connections to reach the
       endpoints defined by a backend. An Ingress can be configured to give services
       externally-reachable urls, load balance traffic, terminate SSL, offer name
       based virtual hosting etc.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
@@ -104,15 +104,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[IngressSpec]' = None
     status: 'Optional[IngressStatus]' = None
 
 
 @dataclass
 class IngressBackend(DictMixin):
-    """IngressBackend describes all endpoints for a given service and port.
+    r"""IngressBackend describes all endpoints for a given service and port.
 
       **parameters**
 
       * **resource** ``Optional[core_v1.TypedLocalObjectReference]`` - resource is an ObjectRef to another Kubernetes resource in the namespace of
         the Ingress object. If resource is specified, a service.Name and service.Port
         must not be specified. This is a mutually exclusive setting with "Service".
       * **service** ``Optional[IngressServiceBackend]`` - service references a service as a backend. This is a mutually exclusive
@@ -120,15 +120,15 @@
     """
     resource: 'Optional[core_v1.TypedLocalObjectReference]' = None
     service: 'Optional[IngressServiceBackend]' = None
 
 
 @dataclass
 class IngressClass(DictMixin):
-    """IngressClass represents the class of the Ingress, referenced by the Ingress
+    r"""IngressClass represents the class of the Ingress, referenced by the Ingress
       Spec. The `ingressclass.kubernetes.io/is-default-class` annotation can be used
       to indicate that an IngressClass should be considered default. When a single
       IngressClass resource has this annotation set to true, new Ingress resources
       without a class specified will be assigned this default class.
 
       **parameters**
 
@@ -149,15 +149,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[IngressClassSpec]' = None
 
 
 @dataclass
 class IngressClassList(DictMixin):
-    """IngressClassList is a collection of IngressClasses.
+    r"""IngressClassList is a collection of IngressClasses.
 
       **parameters**
 
       * **items** ``List[IngressClass]`` - items is the list of IngressClasses.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -172,15 +172,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class IngressClassParametersReference(DictMixin):
-    """IngressClassParametersReference identifies an API object. This can be used to
+    r"""IngressClassParametersReference identifies an API object. This can be used to
       specify a cluster or namespace-scoped resource.
 
       **parameters**
 
       * **kind** ``str`` - kind is the type of resource being referenced.
       * **name** ``str`` - name is the name of resource being referenced.
       * **apiGroup** ``Optional[str]`` - apiGroup is the group for the resource being referenced. If APIGroup is not
@@ -197,15 +197,15 @@
     apiGroup: 'Optional[str]' = None
     namespace: 'Optional[str]' = None
     scope: 'Optional[str]' = None
 
 
 @dataclass
 class IngressClassSpec(DictMixin):
-    """IngressClassSpec provides information about the class of an Ingress.
+    r"""IngressClassSpec provides information about the class of an Ingress.
 
       **parameters**
 
       * **controller** ``Optional[str]`` - controller refers to the name of the controller that should handle this class.
         This allows for different "flavors" that are controlled by the same
         controller. For example, you may have different parameters for the same
         implementing controller. This should be specified as a domain-prefixed path no
@@ -217,15 +217,15 @@
     """
     controller: 'Optional[str]' = None
     parameters: 'Optional[IngressClassParametersReference]' = None
 
 
 @dataclass
 class IngressList(DictMixin):
-    """IngressList is a collection of Ingress.
+    r"""IngressList is a collection of Ingress.
 
       **parameters**
 
       * **items** ``List[Ingress]`` - items is the list of Ingress.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -241,15 +241,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class IngressLoadBalancerIngress(DictMixin):
-    """IngressLoadBalancerIngress represents the status of a load-balancer ingress
+    r"""IngressLoadBalancerIngress represents the status of a load-balancer ingress
       point.
 
       **parameters**
 
       * **hostname** ``Optional[str]`` - hostname is set for load-balancer ingress points that are DNS based.
       * **ip** ``Optional[str]`` - ip is set for load-balancer ingress points that are IP based.
       * **ports** ``Optional[List[IngressPortStatus]]`` - ports provides information about the ports exposed by this LoadBalancer.
@@ -257,26 +257,26 @@
     hostname: 'Optional[str]' = None
     ip: 'Optional[str]' = None
     ports: 'Optional[List[IngressPortStatus]]' = None
 
 
 @dataclass
 class IngressLoadBalancerStatus(DictMixin):
-    """IngressLoadBalancerStatus represents the status of a load-balancer.
+    r"""IngressLoadBalancerStatus represents the status of a load-balancer.
 
       **parameters**
 
       * **ingress** ``Optional[List[IngressLoadBalancerIngress]]`` - ingress is a list containing ingress points for the load-balancer.
     """
     ingress: 'Optional[List[IngressLoadBalancerIngress]]' = None
 
 
 @dataclass
 class IngressPortStatus(DictMixin):
-    """IngressPortStatus represents the error condition of a service port
+    r"""IngressPortStatus represents the error condition of a service port
 
       **parameters**
 
       * **port** ``int`` - port is the port number of the ingress port.
       * **protocol** ``str`` - protocol is the protocol of the ingress port. The supported values are: "TCP",
         "UDP", "SCTP"
       * **error** ``Optional[str]`` - error is to record the problem with the service port The format of the error
@@ -289,15 +289,15 @@
     port: 'int'
     protocol: 'str'
     error: 'Optional[str]' = None
 
 
 @dataclass
 class IngressRule(DictMixin):
-    """IngressRule represents the rules mapping the paths under a specified host to
+    r"""IngressRule represents the rules mapping the paths under a specified host to
       the related backend services. Incoming requests are first evaluated for a host
       match, then routed to the backend associated with the matching
       IngressRuleValue.
 
       **parameters**
 
       * **host** ``Optional[str]`` - host is the fully qualified domain name of a network host, as defined by RFC
@@ -325,30 +325,30 @@
     """
     host: 'Optional[str]' = None
     http: 'Optional[HTTPIngressRuleValue]' = None
 
 
 @dataclass
 class IngressServiceBackend(DictMixin):
-    """IngressServiceBackend references a Kubernetes Service as a Backend.
+    r"""IngressServiceBackend references a Kubernetes Service as a Backend.
 
       **parameters**
 
       * **name** ``str`` - name is the referenced service. The service must exist in the same namespace
         as the Ingress object.
       * **port** ``Optional[ServiceBackendPort]`` - port of the referenced service. A port name or port number is required for a
         IngressServiceBackend.
     """
     name: 'str'
     port: 'Optional[ServiceBackendPort]' = None
 
 
 @dataclass
 class IngressSpec(DictMixin):
-    """IngressSpec describes the Ingress the user wishes to exist.
+    r"""IngressSpec describes the Ingress the user wishes to exist.
 
       **parameters**
 
       * **defaultBackend** ``Optional[IngressBackend]`` - defaultBackend is the backend that should handle requests that don't match any
         rule. If Rules are not specified, DefaultBackend must be specified. If
         DefaultBackend is not set, the handling of requests that do not match any of
         the rules will be up to the Ingress controller.
@@ -374,26 +374,26 @@
     ingressClassName: 'Optional[str]' = None
     rules: 'Optional[List[IngressRule]]' = None
     tls: 'Optional[List[IngressTLS]]' = None
 
 
 @dataclass
 class IngressStatus(DictMixin):
-    """IngressStatus describe the current state of the Ingress.
+    r"""IngressStatus describe the current state of the Ingress.
 
       **parameters**
 
       * **loadBalancer** ``Optional[IngressLoadBalancerStatus]`` - loadBalancer contains the current status of the load-balancer.
     """
     loadBalancer: 'Optional[IngressLoadBalancerStatus]' = None
 
 
 @dataclass
 class IngressTLS(DictMixin):
-    """IngressTLS describes the transport layer security associated with an ingress.
+    r"""IngressTLS describes the transport layer security associated with an ingress.
 
       **parameters**
 
       * **hosts** ``Optional[List[str]]`` - hosts is a list of hosts included in the TLS certificate. The values in this
         list must match the name/s used in the tlsSecret. Defaults to the wildcard
         host setting for the loadbalancer controller fulfilling this Ingress, if left
         unspecified.
@@ -405,15 +405,15 @@
     """
     hosts: 'Optional[List[str]]' = None
     secretName: 'Optional[str]' = None
 
 
 @dataclass
 class NetworkPolicy(DictMixin):
-    """NetworkPolicy describes what network traffic is allowed for a set of Pods
+    r"""NetworkPolicy describes what network traffic is allowed for a set of Pods
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
         https://git.k8s.io/community/contributors/devel/sig-architecture/api-conventions.md#resources
@@ -430,15 +430,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[NetworkPolicySpec]' = None
 
 
 @dataclass
 class NetworkPolicyEgressRule(DictMixin):
-    """NetworkPolicyEgressRule describes a particular set of traffic that is allowed
+    r"""NetworkPolicyEgressRule describes a particular set of traffic that is allowed
       out of pods matched by a NetworkPolicySpec's podSelector. The traffic must
       match both ports and to. This type is beta-level in 1.8
 
       **parameters**
 
       * **ports** ``Optional[List[NetworkPolicyPort]]`` - ports is a list of destination ports for outgoing traffic. Each item in this
         list is combined using a logical OR. If this field is empty or missing, this
@@ -454,15 +454,15 @@
     """
     ports: 'Optional[List[NetworkPolicyPort]]' = None
     to: 'Optional[List[NetworkPolicyPeer]]' = None
 
 
 @dataclass
 class NetworkPolicyIngressRule(DictMixin):
-    """NetworkPolicyIngressRule describes a particular set of traffic that is allowed
+    r"""NetworkPolicyIngressRule describes a particular set of traffic that is allowed
       to the pods matched by a NetworkPolicySpec's podSelector. The traffic must
       match both ports and from.
 
       **parameters**
 
       * **from_** ``Optional[List[NetworkPolicyPeer]]`` - from is a list of sources which should be able to access the pods selected for
         this rule. Items in this list are combined using a logical OR operation. If
@@ -478,15 +478,15 @@
     """
     from_: 'Optional[List[NetworkPolicyPeer]]' = field(metadata={"json": "from"}, default=None)
     ports: 'Optional[List[NetworkPolicyPort]]' = None
 
 
 @dataclass
 class NetworkPolicyList(DictMixin):
-    """NetworkPolicyList is a list of NetworkPolicy objects.
+    r"""NetworkPolicyList is a list of NetworkPolicy objects.
 
       **parameters**
 
       * **items** ``List[NetworkPolicy]`` - items is a list of schema objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -502,15 +502,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class NetworkPolicyPeer(DictMixin):
-    """NetworkPolicyPeer describes a peer to allow traffic to/from. Only certain
+    r"""NetworkPolicyPeer describes a peer to allow traffic to/from. Only certain
       combinations of fields are allowed
 
       **parameters**
 
       * **ipBlock** ``Optional[IPBlock]`` - ipBlock defines policy on a particular IPBlock. If this field is set then
         neither of the other fields can be.
       * **namespaceSelector** ``Optional[meta_v1.LabelSelector]`` - namespaceSelector selects namespaces using cluster-scoped labels. This field
@@ -529,15 +529,15 @@
     ipBlock: 'Optional[IPBlock]' = None
     namespaceSelector: 'Optional[meta_v1.LabelSelector]' = None
     podSelector: 'Optional[meta_v1.LabelSelector]' = None
 
 
 @dataclass
 class NetworkPolicyPort(DictMixin):
-    """NetworkPolicyPort describes a port to allow traffic on
+    r"""NetworkPolicyPort describes a port to allow traffic on
 
       **parameters**
 
       * **endPort** ``Optional[int]`` - endPort indicates that the range of ports from port to endPort if set,
         inclusive, should be allowed by the policy. This field cannot be defined if
         the port field is not defined or if the port field is defined as a named
         (string) port. The endPort must be equal or greater than port.
@@ -551,15 +551,15 @@
     endPort: 'Optional[int]' = None
     port: 'Optional[util_intstr.IntOrString]' = None
     protocol: 'Optional[str]' = None
 
 
 @dataclass
 class NetworkPolicySpec(DictMixin):
-    """NetworkPolicySpec provides the specification of a NetworkPolicy
+    r"""NetworkPolicySpec provides the specification of a NetworkPolicy
 
       **parameters**
 
       * **podSelector** ``meta_v1.LabelSelector`` - podSelector selects the pods to which this NetworkPolicy object applies. The
         array of ingress rules is applied to any pods selected by this field. Multiple
         network policies can select the same set of pods. In this case, the ingress
         rules for each are combined additively. This field is NOT optional and follows
@@ -595,15 +595,15 @@
     egress: 'Optional[List[NetworkPolicyEgressRule]]' = None
     ingress: 'Optional[List[NetworkPolicyIngressRule]]' = None
     policyTypes: 'Optional[List[str]]' = None
 
 
 @dataclass
 class ServiceBackendPort(DictMixin):
-    """ServiceBackendPort is the service port being referenced.
+    r"""ServiceBackendPort is the service port being referenced.
 
       **parameters**
 
       * **name** ``Optional[str]`` - name is the name of the port on the Service. This is a mutually exclusive
         setting with "Number".
       * **number** ``Optional[int]`` - number is the numerical port number (e.g. 80) on the Service. This is a
         mutually exclusive setting with "Name".
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/networking_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/models/networking_v1alpha1.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class IPAddress(DictMixin):
-    """IPAddress represents a single IP of a single IP Family. The object is designed
+    r"""IPAddress represents a single IP of a single IP Family. The object is designed
       to be used by APIs that operate on IP addresses. The object is used by the
       Service core API for allocation of IP addresses. An IP address can be
       represented in different formats, to guarantee the uniqueness of the IP, the
       name of the object is the IP address in canonical format, four decimal digits
       separated by dots suppressing leading zeros for IPv4 and the representation
       defined by RFC 5952 for IPv6. Valid: 192.168.1.5 or 2001:db8::1 or
       2001:db8:aaaa:bbbb:cccc:dddd:eeee:1 Invalid: 10.01.2.3 or 2001:db8:0:0:0::1
@@ -39,15 +39,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[IPAddressSpec]' = None
 
 
 @dataclass
 class IPAddressList(DictMixin):
-    """IPAddressList contains a list of IPAddress.
+    r"""IPAddressList contains a list of IPAddress.
 
       **parameters**
 
       * **items** ``List[IPAddress]`` - items is the list of IPAddresses.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -63,27 +63,27 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class IPAddressSpec(DictMixin):
-    """IPAddressSpec describe the attributes in an IP Address.
+    r"""IPAddressSpec describe the attributes in an IP Address.
 
       **parameters**
 
       * **parentRef** ``ParentReference`` - ParentRef references the resource that an IPAddress is attached to. An
         IPAddress must reference a parent object.
     """
     parentRef: 'ParentReference'
 
 
 @dataclass
 class ParentReference(DictMixin):
-    """ParentReference describes a reference to a parent object.
+    r"""ParentReference describes a reference to a parent object.
 
       **parameters**
 
       * **name** ``str`` - Name is the name of the object being referenced.
       * **resource** ``str`` - Resource is the resource of the object being referenced.
       * **group** ``Optional[str]`` - Group is the group of the object being referenced.
       * **namespace** ``Optional[str]`` - Namespace is the namespace of the object being referenced.
@@ -92,15 +92,15 @@
     resource: 'str'
     group: 'Optional[str]' = None
     namespace: 'Optional[str]' = None
 
 
 @dataclass
 class ServiceCIDR(DictMixin):
-    """ServiceCIDR defines a range of IP addresses using CIDR format (e.g.
+    r"""ServiceCIDR defines a range of IP addresses using CIDR format (e.g.
       192.168.0.0/24 or 2001:db2::/64). This range is used to allocate ClusterIPs to
       Service objects.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -122,15 +122,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[ServiceCIDRSpec]' = None
     status: 'Optional[ServiceCIDRStatus]' = None
 
 
 @dataclass
 class ServiceCIDRList(DictMixin):
-    """ServiceCIDRList contains a list of ServiceCIDR objects.
+    r"""ServiceCIDRList contains a list of ServiceCIDR objects.
 
       **parameters**
 
       * **items** ``List[ServiceCIDR]`` - items is the list of ServiceCIDRs.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -146,29 +146,29 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ServiceCIDRSpec(DictMixin):
-    """ServiceCIDRSpec define the CIDRs the user wants to use for allocating
+    r"""ServiceCIDRSpec define the CIDRs the user wants to use for allocating
       ClusterIPs for Services.
 
       **parameters**
 
       * **cidrs** ``Optional[List[str]]`` - CIDRs defines the IP blocks in CIDR notation (e.g. "192.168.0.0/24" or
         "2001:db8::/64") from which to assign service cluster IPs. Max of two CIDRs is
         allowed, one of each IP family. This field is immutable.
     """
     cidrs: 'Optional[List[str]]' = None
 
 
 @dataclass
 class ServiceCIDRStatus(DictMixin):
-    """ServiceCIDRStatus describes the current state of the ServiceCIDR.
+    r"""ServiceCIDRStatus describes the current state of the ServiceCIDR.
 
       **parameters**
 
       * **conditions** ``Optional[List[meta_v1.Condition]]`` - conditions holds an array of metav1.Condition that describe the state of the
         ServiceCIDR. Current service state
     """
     conditions: 'Optional[List[meta_v1.Condition]]' = None
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/node_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/node_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from . import core_v1
 from . import meta_v1
+from . import core_v1
 
 
 @dataclass
 class Overhead(DictMixin):
-    """Overhead structure represents the resource overhead associated with running a
+    r"""Overhead structure represents the resource overhead associated with running a
       pod.
 
       **parameters**
 
       * **podFixed** ``Optional[dict]`` - podFixed represents the fixed resource overhead associated with running a pod.
     """
     podFixed: 'Optional[dict]' = None
 
 
 @dataclass
 class RuntimeClass(DictMixin):
-    """RuntimeClass defines a class of container runtime supported in the cluster.
+    r"""RuntimeClass defines a class of container runtime supported in the cluster.
       The RuntimeClass is used to determine which container runtime is used to run
       all containers in a pod. RuntimeClasses are manually defined by a user or
       cluster provisioner, and referenced in the PodSpec. The Kubelet is responsible
       for resolving the RuntimeClassName reference before running the pod.  For more
       details, see https://kubernetes.io/docs/concepts/containers/runtime-class/
 
       **parameters**
@@ -64,15 +64,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     overhead: 'Optional[Overhead]' = None
     scheduling: 'Optional[Scheduling]' = None
 
 
 @dataclass
 class RuntimeClassList(DictMixin):
-    """RuntimeClassList is a list of RuntimeClass objects.
+    r"""RuntimeClassList is a list of RuntimeClass objects.
 
       **parameters**
 
       * **items** ``List[RuntimeClass]`` - items is a list of schema objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -88,15 +88,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class Scheduling(DictMixin):
-    """Scheduling specifies the scheduling constraints for nodes supporting a
+    r"""Scheduling specifies the scheduling constraints for nodes supporting a
       RuntimeClass.
 
       **parameters**
 
       * **nodeSelector** ``Optional[dict]`` - nodeSelector lists labels that must be present on nodes that support this
         RuntimeClass. Pods using this RuntimeClass can only be scheduled to a node
         matched by this selector. The RuntimeClass nodeSelector is merged with a pod's
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/policy_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/policy_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from . import util_intstr
 from . import meta_v1
+from . import util_intstr
 
 
 @dataclass
 class Eviction(DictMixin):
-    """Eviction evicts a pod from its node subject to certain policies and safety
+    r"""Eviction evicts a pod from its node subject to certain policies and safety
       constraints. This is a subresource of Pod.  A request to cause such an
       eviction is created by POSTing to .../pods/<pod name>/evictions.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
@@ -33,15 +33,15 @@
     deleteOptions: 'Optional[meta_v1.DeleteOptions]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
 class PodDisruptionBudget(DictMixin):
-    """PodDisruptionBudget is an object to define the max disruption that can be
+    r"""PodDisruptionBudget is an object to define the max disruption that can be
       caused to a collection of pods
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -60,15 +60,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[PodDisruptionBudgetSpec]' = None
     status: 'Optional[PodDisruptionBudgetStatus]' = None
 
 
 @dataclass
 class PodDisruptionBudgetList(DictMixin):
-    """PodDisruptionBudgetList is a collection of PodDisruptionBudgets.
+    r"""PodDisruptionBudgetList is a collection of PodDisruptionBudgets.
 
       **parameters**
 
       * **items** ``List[PodDisruptionBudget]`` - Items is a list of PodDisruptionBudgets
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -84,15 +84,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class PodDisruptionBudgetSpec(DictMixin):
-    """PodDisruptionBudgetSpec is a description of a PodDisruptionBudget.
+    r"""PodDisruptionBudgetSpec is a description of a PodDisruptionBudget.
 
       **parameters**
 
       * **maxUnavailable** ``Optional[util_intstr.IntOrString]`` - An eviction is allowed if at most "maxUnavailable" pods selected by "selector"
         are unavailable after the eviction, i.e. even in absence of the evicted pod.
         For example, one can prevent all voluntary evictions by specifying 0. This is
         a mutually exclusive setting with "minAvailable".
@@ -128,15 +128,15 @@
     minAvailable: 'Optional[util_intstr.IntOrString]' = None
     selector: 'Optional[meta_v1.LabelSelector]' = None
     unhealthyPodEvictionPolicy: 'Optional[str]' = None
 
 
 @dataclass
 class PodDisruptionBudgetStatus(DictMixin):
-    """PodDisruptionBudgetStatus represents information about the status of a
+    r"""PodDisruptionBudgetStatus represents information about the status of a
       PodDisruptionBudget. Status may trail the actual state of a system.
 
       **parameters**
 
       * **currentHealthy** ``int`` - current number of healthy pods
       * **desiredHealthy** ``int`` - minimum desired number of healthy pods
       * **disruptionsAllowed** ``int`` - Number of pod disruptions that are currently allowed.
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/rbac_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/rbac_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,29 +7,29 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class AggregationRule(DictMixin):
-    """AggregationRule describes how to locate ClusterRoles to aggregate into the
+    r"""AggregationRule describes how to locate ClusterRoles to aggregate into the
       ClusterRole
 
       **parameters**
 
       * **clusterRoleSelectors** ``Optional[List[meta_v1.LabelSelector]]`` - ClusterRoleSelectors holds a list of selectors which will be used to find
         ClusterRoles and create the rules. If any of the selectors match, then the
         ClusterRole's permissions will be added
     """
     clusterRoleSelectors: 'Optional[List[meta_v1.LabelSelector]]' = None
 
 
 @dataclass
 class ClusterRole(DictMixin):
-    """ClusterRole is a cluster level, logical grouping of PolicyRules that can be
+    r"""ClusterRole is a cluster level, logical grouping of PolicyRules that can be
       referenced as a unit by a RoleBinding or ClusterRoleBinding.
 
       **parameters**
 
       * **aggregationRule** ``Optional[AggregationRule]`` - AggregationRule is an optional field that describes how to build the Rules for
         this ClusterRole. If AggregationRule is set, then the Rules are controller
         managed and direct changes to Rules will be stomped by the controller.
@@ -49,15 +49,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     rules: 'Optional[List[PolicyRule]]' = None
 
 
 @dataclass
 class ClusterRoleBinding(DictMixin):
-    """ClusterRoleBinding references a ClusterRole, but not contain it.  It can
+    r"""ClusterRoleBinding references a ClusterRole, but not contain it.  It can
       reference a ClusterRole in the global namespace, and adds who information via
       Subject.
 
       **parameters**
 
       * **roleRef** ``RoleRef`` - RoleRef can only reference a ClusterRole in the global namespace. If the
         RoleRef cannot be resolved, the Authorizer must return an error. This field is
@@ -78,15 +78,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     subjects: 'Optional[List[Subject]]' = None
 
 
 @dataclass
 class ClusterRoleBindingList(DictMixin):
-    """ClusterRoleBindingList is a collection of ClusterRoleBindings
+    r"""ClusterRoleBindingList is a collection of ClusterRoleBindings
 
       **parameters**
 
       * **items** ``List[ClusterRoleBinding]`` - Items is a list of ClusterRoleBindings
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -101,15 +101,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ClusterRoleList(DictMixin):
-    """ClusterRoleList is a collection of ClusterRoles
+    r"""ClusterRoleList is a collection of ClusterRoles
 
       **parameters**
 
       * **items** ``List[ClusterRole]`` - Items is a list of ClusterRoles
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -124,15 +124,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class PolicyRule(DictMixin):
-    """PolicyRule holds information that describes a policy rule, but does not
+    r"""PolicyRule holds information that describes a policy rule, but does not
       contain information about who the rule applies to or which namespace the rule
       applies to.
 
       **parameters**
 
       * **verbs** ``List[str]`` - Verbs is a list of Verbs that apply to ALL the ResourceKinds contained in this
         rule. '*' represents all verbs.
@@ -156,15 +156,15 @@
     nonResourceURLs: 'Optional[List[str]]' = None
     resourceNames: 'Optional[List[str]]' = None
     resources: 'Optional[List[str]]' = None
 
 
 @dataclass
 class Role(DictMixin):
-    """Role is a namespaced, logical grouping of PolicyRules that can be referenced
+    r"""Role is a namespaced, logical grouping of PolicyRules that can be referenced
       as a unit by a RoleBinding.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -180,15 +180,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     rules: 'Optional[List[PolicyRule]]' = None
 
 
 @dataclass
 class RoleBinding(DictMixin):
-    """RoleBinding references a role, but does not contain it.  It can reference a
+    r"""RoleBinding references a role, but does not contain it.  It can reference a
       Role in the same namespace or a ClusterRole in the global namespace. It adds
       who information via Subjects and namespace information by which namespace it
       exists in.  RoleBindings in a given namespace only have effect in that
       namespace.
 
       **parameters**
 
@@ -211,15 +211,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     subjects: 'Optional[List[Subject]]' = None
 
 
 @dataclass
 class RoleBindingList(DictMixin):
-    """RoleBindingList is a collection of RoleBindings
+    r"""RoleBindingList is a collection of RoleBindings
 
       **parameters**
 
       * **items** ``List[RoleBinding]`` - Items is a list of RoleBindings
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -234,15 +234,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class RoleList(DictMixin):
-    """RoleList is a collection of Roles
+    r"""RoleList is a collection of Roles
 
       **parameters**
 
       * **items** ``List[Role]`` - Items is a list of Roles
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -257,30 +257,30 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class RoleRef(DictMixin):
-    """RoleRef contains information that points to the role being used
+    r"""RoleRef contains information that points to the role being used
 
       **parameters**
 
       * **apiGroup** ``str`` - APIGroup is the group for the resource being referenced
       * **kind** ``str`` - Kind is the type of resource being referenced
       * **name** ``str`` - Name is the name of resource being referenced
     """
     apiGroup: 'str'
     kind: 'str'
     name: 'str'
 
 
 @dataclass
 class Subject(DictMixin):
-    """Subject contains a reference to the object or user identities a role binding
+    r"""Subject contains a reference to the object or user identities a role binding
       applies to.  This can either hold a direct API object reference, or a value
       for non-objects such as user and group names.
 
       **parameters**
 
       * **kind** ``str`` - Kind of object being referenced. Values defined by this API group are "User",
         "Group", and "ServiceAccount". If the Authorizer does not recognized the kind
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/resource_v1alpha2.py` & `lightkube-models-1.30.0.8/lightkube/models/resource_v1alpha2.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
-from . import core_v1
 from . import runtime
+from . import core_v1
 from . import meta_v1
 from . import resource
 
 
 @dataclass
 class AllocationResult(DictMixin):
-    """AllocationResult contains attributes of an allocated resource.
+    r"""AllocationResult contains attributes of an allocated resource.
 
       **parameters**
 
       * **availableOnNodes** ``Optional[core_v1.NodeSelector]`` - This field will get set by the resource driver after it has allocated the
         resource to inform the scheduler where it can schedule Pods using the
         ResourceClaim.
         Setting this field is optional. If null, the resource is available everywhere.
@@ -39,15 +39,15 @@
     availableOnNodes: 'Optional[core_v1.NodeSelector]' = None
     resourceHandles: 'Optional[List[ResourceHandle]]' = None
     shareable: 'Optional[bool]' = None
 
 
 @dataclass
 class DriverAllocationResult(DictMixin):
-    """DriverAllocationResult contains vendor parameters and the allocation result
+    r"""DriverAllocationResult contains vendor parameters and the allocation result
       for one request.
 
       **parameters**
 
       * **namedResources** ``Optional[NamedResourcesAllocationResult]`` - NamedResources describes the allocation result when using the named resources
         model.
       * **vendorRequestParameters** ``Optional[runtime.RawExtension]`` - VendorRequestParameters are the per-request configuration parameters from the
@@ -55,15 +55,15 @@
     """
     namedResources: 'Optional[NamedResourcesAllocationResult]' = None
     vendorRequestParameters: 'Optional[runtime.RawExtension]' = None
 
 
 @dataclass
 class DriverRequests(DictMixin):
-    """DriverRequests describes all resources that are needed from one particular
+    r"""DriverRequests describes all resources that are needed from one particular
       driver.
 
       **parameters**
 
       * **driverName** ``Optional[str]`` - DriverName is the name used by the DRA driver kubelet plugin.
       * **requests** ``Optional[List[ResourceRequest]]`` - Requests describes all resources that are needed from the driver.
       * **vendorParameters** ``Optional[runtime.RawExtension]`` - VendorParameters are arbitrary setup parameters for all requests of the claim.
@@ -72,26 +72,26 @@
     driverName: 'Optional[str]' = None
     requests: 'Optional[List[ResourceRequest]]' = None
     vendorParameters: 'Optional[runtime.RawExtension]' = None
 
 
 @dataclass
 class NamedResourcesAllocationResult(DictMixin):
-    """NamedResourcesAllocationResult is used in AllocationResultModel.
+    r"""NamedResourcesAllocationResult is used in AllocationResultModel.
 
       **parameters**
 
       * **name** ``str`` - Name is the name of the selected resource instance.
     """
     name: 'str'
 
 
 @dataclass
 class NamedResourcesAttribute(DictMixin):
-    """NamedResourcesAttribute is a combination of an attribute name and its value.
+    r"""NamedResourcesAttribute is a combination of an attribute name and its value.
 
       **parameters**
 
       * **name** ``str`` - Name is unique identifier among all resource instances managed by the driver
         on the node. It must be a DNS subdomain.
       * **bool** ``Optional[bool]`` - BoolValue is a true/false value.
       * **int** ``Optional[int]`` - IntValue is a 64-bit integer.
@@ -109,15 +109,15 @@
     string: 'Optional[str]' = None
     stringSlice: 'Optional[NamedResourcesStringSlice]' = None
     version: 'Optional[str]' = None
 
 
 @dataclass
 class NamedResourcesFilter(DictMixin):
-    """NamedResourcesFilter is used in ResourceFilterModel.
+    r"""NamedResourcesFilter is used in ResourceFilterModel.
 
       **parameters**
 
       * **selector** ``str`` - Selector is a CEL expression which must evaluate to true if a resource
         instance is suitable. The language is as defined in
         https://kubernetes.io/docs/reference/using-api/cel/
         In addition, for each type NamedResourcesin AttributeValue there is a map that
@@ -127,15 +127,15 @@
            attributes.stringslice["b"].isSorted()
     """
     selector: 'str'
 
 
 @dataclass
 class NamedResourcesInstance(DictMixin):
-    """NamedResourcesInstance represents one individual hardware instance that can be
+    r"""NamedResourcesInstance represents one individual hardware instance that can be
       selected based on its attributes.
 
       **parameters**
 
       * **name** ``str`` - Name is unique identifier among all resource instances managed by the driver
         on the node. It must be a DNS subdomain.
       * **attributes** ``Optional[List[NamedResourcesAttribute]]`` - Attributes defines the attributes of this resource instance. The name of each
@@ -143,26 +143,26 @@
     """
     name: 'str'
     attributes: 'Optional[List[NamedResourcesAttribute]]' = None
 
 
 @dataclass
 class NamedResourcesIntSlice(DictMixin):
-    """NamedResourcesIntSlice contains a slice of 64-bit integers.
+    r"""NamedResourcesIntSlice contains a slice of 64-bit integers.
 
       **parameters**
 
       * **ints** ``List[int]`` - Ints is the slice of 64-bit integers.
     """
     ints: 'List[int]'
 
 
 @dataclass
 class NamedResourcesRequest(DictMixin):
-    """NamedResourcesRequest is used in ResourceRequestModel.
+    r"""NamedResourcesRequest is used in ResourceRequestModel.
 
       **parameters**
 
       * **selector** ``str`` - Selector is a CEL expression which must evaluate to true if a resource
         instance is suitable. The language is as defined in
         https://kubernetes.io/docs/reference/using-api/cel/
         In addition, for each type NamedResourcesin AttributeValue there is a map that
@@ -172,37 +172,37 @@
            attributes.stringslice["b"].isSorted()
     """
     selector: 'str'
 
 
 @dataclass
 class NamedResourcesResources(DictMixin):
-    """NamedResourcesResources is used in ResourceModel.
+    r"""NamedResourcesResources is used in ResourceModel.
 
       **parameters**
 
       * **instances** ``List[NamedResourcesInstance]`` - The list of all individual resources instances currently available.
     """
     instances: 'List[NamedResourcesInstance]'
 
 
 @dataclass
 class NamedResourcesStringSlice(DictMixin):
-    """NamedResourcesStringSlice contains a slice of strings.
+    r"""NamedResourcesStringSlice contains a slice of strings.
 
       **parameters**
 
       * **strings** ``List[str]`` - Strings is the slice of strings.
     """
     strings: 'List[str]'
 
 
 @dataclass
 class PodSchedulingContext(DictMixin):
-    """PodSchedulingContext objects hold information that is needed to schedule a Pod
+    r"""PodSchedulingContext objects hold information that is needed to schedule a Pod
       with ResourceClaims that use "WaitForFirstConsumer" allocation mode.
       
       This is an alpha type and requires enabling the DynamicResourceAllocation
       feature gate.
 
       **parameters**
 
@@ -223,15 +223,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[PodSchedulingContextStatus]' = None
 
 
 @dataclass
 class PodSchedulingContextList(DictMixin):
-    """PodSchedulingContextList is a collection of Pod scheduling objects.
+    r"""PodSchedulingContextList is a collection of Pod scheduling objects.
 
       **parameters**
 
       * **items** ``List[PodSchedulingContext]`` - Items is the list of PodSchedulingContext objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -246,15 +246,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class PodSchedulingContextSpec(DictMixin):
-    """PodSchedulingContextSpec describes where resources for the Pod are needed.
+    r"""PodSchedulingContextSpec describes where resources for the Pod are needed.
 
       **parameters**
 
       * **potentialNodes** ``Optional[List[str]]`` - PotentialNodes lists nodes where the Pod might be able to run.
         The size of this field is limited to 128. This is large enough for many
         clusters. Larger clusters may need more attempts to find a node that suits all
         pending resources. This may get increased in the future, but not reduced.
@@ -264,29 +264,29 @@
     """
     potentialNodes: 'Optional[List[str]]' = None
     selectedNode: 'Optional[str]' = None
 
 
 @dataclass
 class PodSchedulingContextStatus(DictMixin):
-    """PodSchedulingContextStatus describes where resources for the Pod can be
+    r"""PodSchedulingContextStatus describes where resources for the Pod can be
       allocated.
 
       **parameters**
 
       * **resourceClaims** ``Optional[List[ResourceClaimSchedulingStatus]]`` - ResourceClaims describes resource availability for each pod.spec.resourceClaim
         entry where the corresponding ResourceClaim uses "WaitForFirstConsumer"
         allocation mode.
     """
     resourceClaims: 'Optional[List[ResourceClaimSchedulingStatus]]' = None
 
 
 @dataclass
 class ResourceClaim(DictMixin):
-    """ResourceClaim describes which resources are needed by a resource consumer. Its
+    r"""ResourceClaim describes which resources are needed by a resource consumer. Its
       status tracks whether the resource has been allocated and what the resulting
       attributes are.
       
       This is an alpha type and requires enabling the DynamicResourceAllocation
       feature gate.
 
       **parameters**
@@ -309,15 +309,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[ResourceClaimStatus]' = None
 
 
 @dataclass
 class ResourceClaimConsumerReference(DictMixin):
-    """ResourceClaimConsumerReference contains enough information to let you locate
+    r"""ResourceClaimConsumerReference contains enough information to let you locate
       the consumer of a ResourceClaim. The user must be a resource in the same
       namespace as the ResourceClaim.
 
       **parameters**
 
       * **name** ``str`` - Name is the name of resource being referenced.
       * **resource** ``str`` - Resource is the type of resource being referenced, for example "pods".
@@ -330,15 +330,15 @@
     resource: 'str'
     uid: 'str'
     apiGroup: 'Optional[str]' = None
 
 
 @dataclass
 class ResourceClaimList(DictMixin):
-    """ResourceClaimList is a collection of claims.
+    r"""ResourceClaimList is a collection of claims.
 
       **parameters**
 
       * **items** ``List[ResourceClaim]`` - Items is the list of resource claims.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -353,15 +353,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ResourceClaimParameters(DictMixin):
-    """ResourceClaimParameters defines resource requests for a ResourceClaim in an
+    r"""ResourceClaimParameters defines resource requests for a ResourceClaim in an
       in-tree format understood by Kubernetes.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -389,15 +389,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     shareable: 'Optional[bool]' = None
 
 
 @dataclass
 class ResourceClaimParametersList(DictMixin):
-    """ResourceClaimParametersList is a collection of ResourceClaimParameters.
+    r"""ResourceClaimParametersList is a collection of ResourceClaimParameters.
 
       **parameters**
 
       * **items** ``List[ResourceClaimParameters]`` - Items is the list of node resource capacity objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -412,15 +412,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ResourceClaimParametersReference(DictMixin):
-    """ResourceClaimParametersReference contains enough information to let you locate
+    r"""ResourceClaimParametersReference contains enough information to let you locate
       the parameters for a ResourceClaim. The object must be in the same namespace
       as the ResourceClaim.
 
       **parameters**
 
       * **kind** ``str`` - Kind is the type of resource being referenced. This is the same value as in
         the parameter object's metadata, for example "ConfigMap".
@@ -432,15 +432,15 @@
     kind: 'str'
     name: 'str'
     apiGroup: 'Optional[str]' = None
 
 
 @dataclass
 class ResourceClaimSchedulingStatus(DictMixin):
-    """ResourceClaimSchedulingStatus contains information about one particular
+    r"""ResourceClaimSchedulingStatus contains information about one particular
       ResourceClaim with "WaitForFirstConsumer" allocation mode.
 
       **parameters**
 
       * **name** ``Optional[str]`` - Name matches the pod.spec.resourceClaims[*].Name field.
       * **unsuitableNodes** ``Optional[List[str]]`` - UnsuitableNodes lists nodes that the ResourceClaim cannot be allocated for.
         The size of this field is limited to 128, the same as for
@@ -449,15 +449,15 @@
     """
     name: 'Optional[str]' = None
     unsuitableNodes: 'Optional[List[str]]' = None
 
 
 @dataclass
 class ResourceClaimSpec(DictMixin):
-    """ResourceClaimSpec defines how a resource is to be allocated.
+    r"""ResourceClaimSpec defines how a resource is to be allocated.
 
       **parameters**
 
       * **resourceClassName** ``str`` - ResourceClassName references the driver and additional parameters via the name
         of a ResourceClass that was created as part of the driver deployment.
       * **allocationMode** ``Optional[str]`` - Allocation can start immediately or when a Pod wants to use the resource.
         "WaitForFirstConsumer" is the default.
@@ -468,15 +468,15 @@
     resourceClassName: 'str'
     allocationMode: 'Optional[str]' = None
     parametersRef: 'Optional[ResourceClaimParametersReference]' = None
 
 
 @dataclass
 class ResourceClaimStatus(DictMixin):
-    """ResourceClaimStatus tracks whether the resource has been allocated and what
+    r"""ResourceClaimStatus tracks whether the resource has been allocated and what
       the resulting attributes are.
 
       **parameters**
 
       * **allocation** ``Optional[AllocationResult]`` - Allocation is set by the resource driver once a resource or set of resources
         has been allocated successfully. If this is not specified, the resources have
         not been allocated yet.
@@ -497,15 +497,15 @@
     deallocationRequested: 'Optional[bool]' = None
     driverName: 'Optional[str]' = None
     reservedFor: 'Optional[List[ResourceClaimConsumerReference]]' = None
 
 
 @dataclass
 class ResourceClaimTemplate(DictMixin):
-    """ResourceClaimTemplate is used to produce ResourceClaim objects.
+    r"""ResourceClaimTemplate is used to produce ResourceClaim objects.
 
       **parameters**
 
       * **spec** ``ResourceClaimTemplateSpec`` - Describes the ResourceClaim that is to be generated.
         This field is immutable. A ResourceClaim will get created by the control plane
         for a Pod when needed and then not get updated anymore.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
@@ -522,15 +522,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
 class ResourceClaimTemplateList(DictMixin):
-    """ResourceClaimTemplateList is a collection of claim templates.
+    r"""ResourceClaimTemplateList is a collection of claim templates.
 
       **parameters**
 
       * **items** ``List[ResourceClaimTemplate]`` - Items is the list of resource claim templates.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -545,15 +545,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ResourceClaimTemplateSpec(DictMixin):
-    """ResourceClaimTemplateSpec contains the metadata and fields for a
+    r"""ResourceClaimTemplateSpec contains the metadata and fields for a
       ResourceClaim.
 
       **parameters**
 
       * **spec** ``ResourceClaimSpec`` - Spec for the ResourceClaim. The entire content is copied unchanged into the
         ResourceClaim that gets created from this template. The same fields as in a
         ResourceClaim are also valid here.
@@ -563,15 +563,15 @@
     """
     spec: 'ResourceClaimSpec'
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
 class ResourceClass(DictMixin):
-    """ResourceClass is used by administrators to influence how resources are
+    r"""ResourceClass is used by administrators to influence how resources are
       allocated.
       
       This is an alpha type and requires enabling the DynamicResourceAllocation
       feature gate.
 
       **parameters**
 
@@ -606,15 +606,15 @@
     parametersRef: 'Optional[ResourceClassParametersReference]' = None
     structuredParameters: 'Optional[bool]' = None
     suitableNodes: 'Optional[core_v1.NodeSelector]' = None
 
 
 @dataclass
 class ResourceClassList(DictMixin):
-    """ResourceClassList is a collection of classes.
+    r"""ResourceClassList is a collection of classes.
 
       **parameters**
 
       * **items** ``List[ResourceClass]`` - Items is the list of resource classes.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -629,15 +629,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ResourceClassParameters(DictMixin):
-    """ResourceClassParameters defines resource requests for a ResourceClass in an
+    r"""ResourceClassParameters defines resource requests for a ResourceClass in an
       in-tree format understood by Kubernetes.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -662,15 +662,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     vendorParameters: 'Optional[List[VendorParameters]]' = None
 
 
 @dataclass
 class ResourceClassParametersList(DictMixin):
-    """ResourceClassParametersList is a collection of ResourceClassParameters.
+    r"""ResourceClassParametersList is a collection of ResourceClassParameters.
 
       **parameters**
 
       * **items** ``List[ResourceClassParameters]`` - Items is the list of node resource capacity objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -685,15 +685,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class ResourceClassParametersReference(DictMixin):
-    """ResourceClassParametersReference contains enough information to let you locate
+    r"""ResourceClassParametersReference contains enough information to let you locate
       the parameters for a ResourceClass.
 
       **parameters**
 
       * **kind** ``str`` - Kind is the type of resource being referenced. This is the same value as in
         the parameter object's metadata.
       * **name** ``str`` - Name is the name of resource being referenced.
@@ -707,28 +707,28 @@
     name: 'str'
     apiGroup: 'Optional[str]' = None
     namespace: 'Optional[str]' = None
 
 
 @dataclass
 class ResourceFilter(DictMixin):
-    """ResourceFilter is a filter for resources from one particular driver.
+    r"""ResourceFilter is a filter for resources from one particular driver.
 
       **parameters**
 
       * **driverName** ``Optional[str]`` - DriverName is the name used by the DRA driver kubelet plugin.
       * **namedResources** ``Optional[NamedResourcesFilter]`` - NamedResources describes a resource filter using the named resources model.
     """
     driverName: 'Optional[str]' = None
     namedResources: 'Optional[NamedResourcesFilter]' = None
 
 
 @dataclass
 class ResourceHandle(DictMixin):
-    """ResourceHandle holds opaque resource data for processing by a specific kubelet
+    r"""ResourceHandle holds opaque resource data for processing by a specific kubelet
       plugin.
 
       **parameters**
 
       * **data** ``Optional[str]`` - Data contains the opaque data associated with this ResourceHandle. It is set
         by the controller component of the resource driver whose name matches the
         DriverName set in the ResourceClaimStatus this ResourceHandle is embedded in.
@@ -745,30 +745,30 @@
     data: 'Optional[str]' = None
     driverName: 'Optional[str]' = None
     structuredData: 'Optional[StructuredResourceHandle]' = None
 
 
 @dataclass
 class ResourceRequest(DictMixin):
-    """ResourceRequest is a request for resources from one particular driver.
+    r"""ResourceRequest is a request for resources from one particular driver.
 
       **parameters**
 
       * **namedResources** ``Optional[NamedResourcesRequest]`` - NamedResources describes a request for resources with the named resources
         model.
       * **vendorParameters** ``Optional[runtime.RawExtension]`` - VendorParameters are arbitrary setup parameters for the requested resource.
         They are ignored while allocating a claim.
     """
     namedResources: 'Optional[NamedResourcesRequest]' = None
     vendorParameters: 'Optional[runtime.RawExtension]' = None
 
 
 @dataclass
 class ResourceSlice(DictMixin):
-    """ResourceSlice provides information about available resources on individual
+    r"""ResourceSlice provides information about available resources on individual
       nodes.
 
       **parameters**
 
       * **driverName** ``str`` - DriverName identifies the DRA driver providing the capacity information. A
         field selector can be used to list only ResourceSlice objects with a certain
         driver name.
@@ -793,15 +793,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     namedResources: 'Optional[NamedResourcesResources]' = None
     nodeName: 'Optional[str]' = None
 
 
 @dataclass
 class ResourceSliceList(DictMixin):
-    """ResourceSliceList is a collection of ResourceSlices.
+    r"""ResourceSliceList is a collection of ResourceSlices.
 
       **parameters**
 
       * **items** ``List[ResourceSlice]`` - Items is the list of node resource capacity objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -816,15 +816,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class StructuredResourceHandle(DictMixin):
-    """StructuredResourceHandle is the in-tree representation of the allocation
+    r"""StructuredResourceHandle is the in-tree representation of the allocation
       result.
 
       **parameters**
 
       * **results** ``List[DriverAllocationResult]`` - Results lists all allocated driver resources.
       * **nodeName** ``Optional[str]`` - NodeName is the name of the node providing the necessary resources if the
         resources are local to a node.
@@ -837,15 +837,15 @@
     nodeName: 'Optional[str]' = None
     vendorClaimParameters: 'Optional[runtime.RawExtension]' = None
     vendorClassParameters: 'Optional[runtime.RawExtension]' = None
 
 
 @dataclass
 class VendorParameters(DictMixin):
-    """VendorParameters are opaque parameters for one particular driver.
+    r"""VendorParameters are opaque parameters for one particular driver.
 
       **parameters**
 
       * **driverName** ``Optional[str]`` - DriverName is the name used by the DRA driver kubelet plugin.
       * **parameters** ``Optional[runtime.RawExtension]`` - Parameters can be arbitrary setup parameters. They are ignored while
         allocating a claim.
     """
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/scheduling_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/scheduling_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class PriorityClass(DictMixin):
-    """PriorityClass defines mapping from a priority class name to the priority
+    r"""PriorityClass defines mapping from a priority class name to the priority
       integer value. The value can be any valid integer.
 
       **parameters**
 
       * **value** ``int`` - value represents the integer value of this priority class. This is the actual
         priority that pods receive when they have the name of this class in their pod
         spec.
@@ -47,15 +47,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     preemptionPolicy: 'Optional[str]' = None
 
 
 @dataclass
 class PriorityClassList(DictMixin):
-    """PriorityClassList is a collection of priority classes.
+    r"""PriorityClassList is a collection of priority classes.
 
       **parameters**
 
       * **items** ``List[PriorityClass]`` - items is the list of PriorityClasses
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/storage_v1.py` & `lightkube-models-1.30.0.8/lightkube/models/storage_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from typing import List, Optional, TYPE_CHECKING
 
 from ._schema import dataclass, field, DictMixin
 
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
+from . import meta_v1
 from . import resource
 from . import core_v1
-from . import meta_v1
 
 
 @dataclass
 class CSIDriver(DictMixin):
-    """CSIDriver captures information about a Container Storage Interface (CSI)
+    r"""CSIDriver captures information about a Container Storage Interface (CSI)
       volume driver deployed on the cluster. Kubernetes attach detach controller
       uses this object to determine whether attach is required. Kubelet uses this
       object to determine whether pod information needs to be passed on mount.
       CSIDriver objects are non-namespaced.
 
       **parameters**
 
@@ -41,15 +41,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
 class CSIDriverList(DictMixin):
-    """CSIDriverList is a collection of CSIDriver objects.
+    r"""CSIDriverList is a collection of CSIDriver objects.
 
       **parameters**
 
       * **items** ``List[CSIDriver]`` - items is the list of CSIDriver
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -65,15 +65,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class CSIDriverSpec(DictMixin):
-    """CSIDriverSpec is the specification of a CSIDriver.
+    r"""CSIDriverSpec is the specification of a CSIDriver.
 
       **parameters**
 
       * **attachRequired** ``Optional[bool]`` - attachRequired indicates this CSI volume driver requires an attach operation
         (because it implements the CSI ControllerPublishVolume() method), and that the
         Kubernetes attach detach controller should call the attach volume interface
         which checks the volumeattachment status and waits until the volume is
@@ -179,15 +179,15 @@
     storageCapacity: 'Optional[bool]' = None
     tokenRequests: 'Optional[List[TokenRequest]]' = None
     volumeLifecycleModes: 'Optional[List[str]]' = None
 
 
 @dataclass
 class CSINode(DictMixin):
-    """CSINode holds information about all CSI drivers installed on a node. CSI
+    r"""CSINode holds information about all CSI drivers installed on a node. CSI
       drivers do not need to create the CSINode object directly. As long as they use
       the node-driver-registrar sidecar container, the kubelet will automatically
       populate the CSINode object for the CSI driver as part of kubelet plugin
       registration. CSINode has the same name as a node. If the object is missing,
       it means either there are no CSI Drivers available on the node, or the Kubelet
       version is low enough that it doesn't create this object. CSINode has an
       OwnerReference that points to the corresponding node object.
@@ -209,15 +209,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
 
 
 @dataclass
 class CSINodeDriver(DictMixin):
-    """CSINodeDriver holds information about the specification of one CSI driver
+    r"""CSINodeDriver holds information about the specification of one CSI driver
       installed on a node
 
       **parameters**
 
       * **name** ``str`` - name represents the name of the CSI driver that this object refers to. This
         MUST be the same name returned by the CSI GetPluginName() call for that
         driver.
@@ -245,15 +245,15 @@
     nodeID: 'str'
     allocatable: 'Optional[VolumeNodeResources]' = None
     topologyKeys: 'Optional[List[str]]' = None
 
 
 @dataclass
 class CSINodeList(DictMixin):
-    """CSINodeList is a collection of CSINode objects.
+    r"""CSINodeList is a collection of CSINode objects.
 
       **parameters**
 
       * **items** ``List[CSINode]`` - items is the list of CSINode
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -269,28 +269,28 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class CSINodeSpec(DictMixin):
-    """CSINodeSpec holds information about the specification of all CSI drivers
+    r"""CSINodeSpec holds information about the specification of all CSI drivers
       installed on a node
 
       **parameters**
 
       * **drivers** ``List[CSINodeDriver]`` - drivers is a list of information of all CSI Drivers existing on a node. If all
         drivers in the list are uninstalled, this can become empty.
     """
     drivers: 'List[CSINodeDriver]'
 
 
 @dataclass
 class CSIStorageCapacity(DictMixin):
-    """CSIStorageCapacity stores the result of one CSI GetCapacity call. For a given
+    r"""CSIStorageCapacity stores the result of one CSI GetCapacity call. For a given
       StorageClass, this describes the available capacity in a particular topology
       segment.  This can be used when considering where to instantiate new
       PersistentVolumes.
       
       For example this can express things like: - StorageClass "standard" has "1234
       GiB" available in "topology.kubernetes.io/zone=us-east1" - StorageClass
       "localssd" has "10 GiB" available in "kubernetes.io/hostname=knode-abc123"
@@ -358,15 +358,15 @@
     maximumVolumeSize: 'Optional[resource.Quantity]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     nodeTopology: 'Optional[meta_v1.LabelSelector]' = None
 
 
 @dataclass
 class CSIStorageCapacityList(DictMixin):
-    """CSIStorageCapacityList is a collection of CSIStorageCapacity objects.
+    r"""CSIStorageCapacityList is a collection of CSIStorageCapacity objects.
 
       **parameters**
 
       * **items** ``List[CSIStorageCapacity]`` - items is the list of CSIStorageCapacity objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -382,15 +382,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class StorageClass(DictMixin):
-    """StorageClass describes the parameters for a class of storage for which
+    r"""StorageClass describes the parameters for a class of storage for which
       PersistentVolumes can be dynamically provisioned.
       
       StorageClasses are non-namespaced; the name of the storage class according to
       etcd is in ObjectMeta.Name.
 
       **parameters**
 
@@ -432,15 +432,15 @@
     parameters: 'Optional[dict]' = None
     reclaimPolicy: 'Optional[str]' = None
     volumeBindingMode: 'Optional[str]' = None
 
 
 @dataclass
 class StorageClassList(DictMixin):
-    """StorageClassList is a collection of storage classes.
+    r"""StorageClassList is a collection of storage classes.
 
       **parameters**
 
       * **items** ``List[StorageClass]`` - items is the list of StorageClasses
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -456,15 +456,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class TokenRequest(DictMixin):
-    """TokenRequest contains parameters of a service account token.
+    r"""TokenRequest contains parameters of a service account token.
 
       **parameters**
 
       * **audience** ``str`` - audience is the intended audience of the token in "TokenRequestSpec". It will
         default to the audiences of kube apiserver.
       * **expirationSeconds** ``Optional[int]`` - expirationSeconds is the duration of validity of the token in
         "TokenRequestSpec". It has the same default value of "ExpirationSeconds" in
@@ -472,15 +472,15 @@
     """
     audience: 'str'
     expirationSeconds: 'Optional[int]' = None
 
 
 @dataclass
 class VolumeAttachment(DictMixin):
-    """VolumeAttachment captures the intent to attach or detach the specified volume
+    r"""VolumeAttachment captures the intent to attach or detach the specified volume
       to/from the specified node.
       
       VolumeAttachment objects are non-namespaced.
 
       **parameters**
 
       * **spec** ``VolumeAttachmentSpec`` - spec represents specification of the desired attach/detach volume behavior.
@@ -503,15 +503,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     status: 'Optional[VolumeAttachmentStatus]' = None
 
 
 @dataclass
 class VolumeAttachmentList(DictMixin):
-    """VolumeAttachmentList is a collection of VolumeAttachment objects.
+    r"""VolumeAttachmentList is a collection of VolumeAttachment objects.
 
       **parameters**
 
       * **items** ``List[VolumeAttachment]`` - items is the list of VolumeAttachments
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -527,15 +527,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class VolumeAttachmentSource(DictMixin):
-    """VolumeAttachmentSource represents a volume that should be attached. Right now
+    r"""VolumeAttachmentSource represents a volume that should be attached. Right now
       only PersistenVolumes can be attached via external attacher, in future we may
       allow also inline volumes in pods. Exactly one member can be set.
 
       **parameters**
 
       * **inlineVolumeSpec** ``Optional[core_v1.PersistentVolumeSpec]`` - inlineVolumeSpec contains all the information necessary to attach a persistent
         volume defined by a pod's inline VolumeSource. This field is populated only
@@ -546,15 +546,15 @@
     """
     inlineVolumeSpec: 'Optional[core_v1.PersistentVolumeSpec]' = None
     persistentVolumeName: 'Optional[str]' = None
 
 
 @dataclass
 class VolumeAttachmentSpec(DictMixin):
-    """VolumeAttachmentSpec is the specification of a VolumeAttachment request.
+    r"""VolumeAttachmentSpec is the specification of a VolumeAttachment request.
 
       **parameters**
 
       * **attacher** ``str`` - attacher indicates the name of the volume driver that MUST handle this
         request. This is the name returned by GetPluginName().
       * **nodeName** ``str`` - nodeName represents the node that the volume should be attached to.
       * **source** ``VolumeAttachmentSource`` - source represents the volume that should be attached.
@@ -562,15 +562,15 @@
     attacher: 'str'
     nodeName: 'str'
     source: 'VolumeAttachmentSource'
 
 
 @dataclass
 class VolumeAttachmentStatus(DictMixin):
-    """VolumeAttachmentStatus is the status of a VolumeAttachment request.
+    r"""VolumeAttachmentStatus is the status of a VolumeAttachment request.
 
       **parameters**
 
       * **attached** ``bool`` - attached indicates the volume is successfully attached. This field must only
         be set by the entity completing the attach operation, i.e. the
         external-attacher.
       * **attachError** ``Optional[VolumeError]`` - attachError represents the last error encountered during attach operation, if
@@ -588,29 +588,29 @@
     attachError: 'Optional[VolumeError]' = None
     attachmentMetadata: 'Optional[dict]' = None
     detachError: 'Optional[VolumeError]' = None
 
 
 @dataclass
 class VolumeError(DictMixin):
-    """VolumeError captures an error encountered during a volume operation.
+    r"""VolumeError captures an error encountered during a volume operation.
 
       **parameters**
 
       * **message** ``Optional[str]`` - message represents the error encountered during Attach or Detach operation.
         This string may be logged, so it should not contain sensitive information.
       * **time** ``Optional[meta_v1.Time]`` - time represents the time the error was encountered.
     """
     message: 'Optional[str]' = None
     time: 'Optional[meta_v1.Time]' = None
 
 
 @dataclass
 class VolumeNodeResources(DictMixin):
-    """VolumeNodeResources is a set of resource limits for scheduling of volumes.
+    r"""VolumeNodeResources is a set of resource limits for scheduling of volumes.
 
       **parameters**
 
       * **count** ``Optional[int]`` - count indicates the maximum number of unique volumes managed by the CSI driver
         that can be used on a node. A volume that is both attached and mounted on a
         node is considered to be used once, not twice. The same rule applies for a
         unique volume that is shared among multiple pods on the same node. If this
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/storage_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/models/storage_v1alpha1.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class VolumeAttributesClass(DictMixin):
-    """VolumeAttributesClass represents a specification of mutable volume attributes
+    r"""VolumeAttributesClass represents a specification of mutable volume attributes
       defined by the CSI driver. The class can be specified during dynamic
       provisioning of PersistentVolumeClaims, and changed in the
       PersistentVolumeClaim spec after provisioning.
 
       **parameters**
 
       * **driverName** ``str`` - Name of the CSI driver This field is immutable.
@@ -47,15 +47,15 @@
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     parameters: 'Optional[dict]' = None
 
 
 @dataclass
 class VolumeAttributesClassList(DictMixin):
-    """VolumeAttributesClassList is a collection of VolumeAttributesClass objects.
+    r"""VolumeAttributesClassList is a collection of VolumeAttributesClass objects.
 
       **parameters**
 
       * **items** ``List[VolumeAttributesClass]`` - items is the list of VolumeAttributesClass objects.
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/storagemigration_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/models/storagemigration_v1alpha1.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
     from dataclasses import dataclass, field
 
 from . import meta_v1
 
 
 @dataclass
 class GroupVersionResource(DictMixin):
-    """The names of the group, the version, and the resource.
+    r"""The names of the group, the version, and the resource.
 
       **parameters**
 
       * **group** ``Optional[str]`` - The name of the group.
       * **resource** ``Optional[str]`` - The name of the resource.
       * **version** ``Optional[str]`` - The name of the version.
     """
     group: 'Optional[str]' = None
     resource: 'Optional[str]' = None
     version: 'Optional[str]' = None
 
 
 @dataclass
 class MigrationCondition(DictMixin):
-    """Describes the state of a migration at a certain point.
+    r"""Describes the state of a migration at a certain point.
 
       **parameters**
 
       * **status** ``str`` - Status of the condition, one of True, False, Unknown.
       * **type** ``str`` - Type of the condition.
       * **lastUpdateTime** ``Optional[meta_v1.Time]`` - The last time this condition was updated.
       * **message** ``Optional[str]`` - A human readable message indicating details about the transition.
@@ -41,15 +41,15 @@
     lastUpdateTime: 'Optional[meta_v1.Time]' = None
     message: 'Optional[str]' = None
     reason: 'Optional[str]' = None
 
 
 @dataclass
 class StorageVersionMigration(DictMixin):
-    """StorageVersionMigration represents a migration of stored data to the latest
+    r"""StorageVersionMigration represents a migration of stored data to the latest
       storage version.
 
       **parameters**
 
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -68,15 +68,15 @@
     metadata: 'Optional[meta_v1.ObjectMeta]' = None
     spec: 'Optional[StorageVersionMigrationSpec]' = None
     status: 'Optional[StorageVersionMigrationStatus]' = None
 
 
 @dataclass
 class StorageVersionMigrationList(DictMixin):
-    """StorageVersionMigrationList is a collection of storage version migrations.
+    r"""StorageVersionMigrationList is a collection of storage version migrations.
 
       **parameters**
 
       * **items** ``List[StorageVersionMigration]`` - Items is the list of StorageVersionMigration
       * **apiVersion** ``Optional[str]`` - APIVersion defines the versioned schema of this representation of an object.
         Servers should convert recognized schemas to the latest internal value, and
         may reject unrecognized values. More info:
@@ -92,15 +92,15 @@
     apiVersion: 'Optional[str]' = None
     kind: 'Optional[str]' = None
     metadata: 'Optional[meta_v1.ListMeta]' = None
 
 
 @dataclass
 class StorageVersionMigrationSpec(DictMixin):
-    """Spec of the storage version migration.
+    r"""Spec of the storage version migration.
 
       **parameters**
 
       * **resource** ``GroupVersionResource`` - The resource that is being migrated. The migrator sends requests to the
         endpoint serving the resource. Immutable.
       * **continueToken** ``Optional[str]`` - The token used in the list options to get the next chunk of objects to
         migrate. When the .status.conditions indicates the migration is "Running",
@@ -108,15 +108,15 @@
     """
     resource: 'GroupVersionResource'
     continueToken: 'Optional[str]' = None
 
 
 @dataclass
 class StorageVersionMigrationStatus(DictMixin):
-    """Status of the storage version migration.
+    r"""Status of the storage version migration.
 
       **parameters**
 
       * **conditions** ``Optional[List[MigrationCondition]]`` - The latest available observations of the migration's current state.
       * **resourceVersion** ``Optional[str]`` - ResourceVersion to compare with the GC cache for performing the migration.
         This is the current resource version of given group, version and resource when
         kube-controller-manager first observes this StorageVersionMigration resource.
```

### Comparing `lightkube-models-1.30.0.7/lightkube/models/version.py` & `lightkube-models-1.30.0.8/lightkube/models/version.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 if TYPE_CHECKING:   # Fix for pycharm autocompletion https://youtrack.jetbrains.com/issue/PY-54560
     from dataclasses import dataclass, field
 
 
 
 @dataclass
 class Info(DictMixin):
-    """Info contains versioning information. how we'll want to distribute that
+    r"""Info contains versioning information. how we'll want to distribute that
       information.
 
       **parameters**
 
       * **buildDate** ``str`` - 
       * **compiler** ``str`` - 
       * **gitCommit** ``str`` -
```

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/admissionregistration_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/admissionregistration_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/admissionregistration_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/resources/admissionregistration_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/admissionregistration_v1beta1.py` & `lightkube-models-1.30.0.8/lightkube/resources/admissionregistration_v1beta1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/apiextensions_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/apiextensions_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/apiregistration_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/apiregistration_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/apps_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/apps_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/authentication_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/authentication_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/authentication_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/resources/authentication_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/authentication_v1beta1.py` & `lightkube-models-1.30.0.8/lightkube/resources/authentication_v1beta1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/authorization_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/authorization_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/autoscaling_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/autoscaling_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/autoscaling_v2.py` & `lightkube-models-1.30.0.8/lightkube/resources/autoscaling_v2.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/batch_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/batch_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/certificates_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/certificates_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/certificates_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/resources/certificates_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/coordination_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/coordination_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/core_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/core_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/discovery_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/discovery_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/events_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/events_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/flowcontrol_apiserver_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/flowcontrol_apiserver_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/flowcontrol_apiserver_v1beta3.py` & `lightkube-models-1.30.0.8/lightkube/resources/flowcontrol_apiserver_v1beta3.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/internal_apiserver_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/resources/internal_apiserver_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/networking_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/networking_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/networking_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/resources/networking_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/node_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/node_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/policy_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/policy_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/rbac_authorization_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/rbac_authorization_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/resource_v1alpha2.py` & `lightkube-models-1.30.0.8/lightkube/resources/resource_v1alpha2.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/scheduling_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/scheduling_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/storage_v1.py` & `lightkube-models-1.30.0.8/lightkube/resources/storage_v1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/storage_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/resources/storage_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube/resources/storagemigration_v1alpha1.py` & `lightkube-models-1.30.0.8/lightkube/resources/storagemigration_v1alpha1.py`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/lightkube_models.egg-info/PKG-INFO` & `lightkube-models-1.30.0.8/lightkube_models.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightkube-models
-Version: 1.30.0.7
+Version: 1.30.0.8
 Summary: Models and Resources for lightkube module
 Home-page: https://github.com/gtsystem/lightkube-models
 Author: Giuseppe Tribulato
 Author-email: gtsystem@gmail.com
 License: Apache Software License
 Description: # lightkube-models
```

### Comparing `lightkube-models-1.30.0.7/lightkube_models.egg-info/SOURCES.txt` & `lightkube-models-1.30.0.8/lightkube_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightkube-models-1.30.0.7/setup.py` & `lightkube-models-1.30.0.8/setup.py`

 * *Files identical despite different names*

