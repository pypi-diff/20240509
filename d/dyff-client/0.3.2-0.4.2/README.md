# Comparing `tmp/dyff_client-0.3.2.tar.gz` & `tmp/dyff_client-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_client-0.3.2.tar", last modified: Wed Apr 24 22:17:29 2024, max compression
+gzip compressed data, was "dyff_client-0.4.2.tar", last modified: Thu May  9 00:38:48 2024, max compression
```

## Comparing `dyff_client-0.3.2.tar` & `dyff_client-0.4.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.630480 dyff_client-0.3.2/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-24 22:17:23.000000 dyff_client-0.3.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1777 2024-04-24 22:17:23.000000 dyff_client-0.3.2/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-24 22:17:23.000000 dyff_client-0.3.2/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-24 22:17:23.000000 dyff_client-0.3.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-04-24 22:17:23.000000 dyff_client-0.3.2/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     3478 2024-04-24 22:17:23.000000 dyff_client-0.3.2/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-04-24 22:17:23.000000 dyff_client-0.3.2/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-24 22:17:23.000000 dyff_client-0.3.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-24 22:17:23.000000 dyff_client-0.3.2/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4008 2024-04-24 22:17:29.630480 dyff_client-0.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2781 2024-04-24 22:17:23.000000 dyff_client-0.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.617647 dyff_client-0.3.2/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.623147 dyff_client-0.3.2/dyff/client/
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.624064 dyff_client-0.3.2/dyff/client/_generated/
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7058 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      752 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)    80932 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.624980 dyff_client-0.3.2/dyff/client/_generated/aio/
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7226 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.625897 dyff_client-0.3.2/dyff/client/_generated/aio/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   770253 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/aio/operations/_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.627730 dyff_client-0.3.2/dyff/client/_generated/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   821959 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/operations/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/_generated/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    82266 2024-04-24 22:17:23.000000 dyff_client-0.3.2/dyff/client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.629564 dyff_client-0.3.2/dyff_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4008 2024-04-24 22:17:29.000000 dyff_client-0.3.2/dyff_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1464 2024-04-24 22:17:29.000000 dyff_client-0.3.2/dyff_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 22:17:29.000000 dyff_client-0.3.2/dyff_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2024-04-24 22:17:29.000000 dyff_client-0.3.2/dyff_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-24 22:17:29.000000 dyff_client-0.3.2/dyff_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1084 2024-04-24 22:17:23.000000 dyff_client-0.3.2/makefile
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-24 22:17:23.000000 dyff_client-0.3.2/package-lock.json
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-04-24 22:17:23.000000 dyff_client-0.3.2/package.json
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-24 22:17:23.000000 dyff_client-0.3.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.618564 dyff_client-0.3.2/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.628647 dyff_client-0.3.2/scripts/inferenceservices/
--rw-rw-rw-   0 root         (0) root         (0)     2529 2024-04-24 22:17:23.000000 dyff_client-0.3.2/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
--rw-rw-rw-   0 root         (0) root         (0)     2537 2024-04-24 22:17:23.000000 dyff_client-0.3.2/scripts/inferenceservices/tiiuae--falcon-7b--default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.629564 dyff_client-0.3.2/scripts/models/
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-24 22:17:23.000000 dyff_client-0.3.2/scripts/models/databricks--dolly-v2-3b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1374 2024-04-24 22:17:23.000000 dyff_client-0.3.2/scripts/models/databricks--dolly-v2-3b.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-04-24 22:17:23.000000 dyff_client-0.3.2/scripts/models/tiiuae--falcon-7b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1356 2024-04-24 22:17:23.000000 dyff_client-0.3.2/scripts/models/tiiuae--falcon-7b.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 22:17:29.630480 dyff_client-0.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 22:17:29.629564 dyff_client-0.3.2/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-04-24 22:17:23.000000 dyff_client-0.3.2/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.573569 dyff_client-0.4.2/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-09 00:38:42.000000 dyff_client-0.4.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2024-05-09 00:38:42.000000 dyff_client-0.4.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-05-09 00:38:42.000000 dyff_client-0.4.2/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-09 00:38:42.000000 dyff_client-0.4.2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-05-09 00:38:42.000000 dyff_client-0.4.2/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     3478 2024-05-09 00:38:42.000000 dyff_client-0.4.2/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-09 00:38:42.000000 dyff_client-0.4.2/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-09 00:38:42.000000 dyff_client-0.4.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-05-09 00:38:42.000000 dyff_client-0.4.2/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-05-09 00:38:48.573569 dyff_client-0.4.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2024-05-09 00:38:42.000000 dyff_client-0.4.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.559569 dyff_client-0.4.2/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.564569 dyff_client-0.4.2/dyff/client/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.566569 dyff_client-0.4.2/dyff/client/_generated/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6489 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      752 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    80932 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.567569 dyff_client-0.4.2/dyff/client/_generated/aio/
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6649 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.569569 dyff_client-0.4.2/dyff/client/_generated/aio/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   821473 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/aio/operations/_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.570569 dyff_client-0.4.2/dyff/client/_generated/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   877754 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/operations/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/_generated/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    77153 2024-05-09 00:38:42.000000 dyff_client-0.4.2/dyff/client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.572569 dyff_client-0.4.2/dyff_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4008 2024-05-09 00:38:48.000000 dyff_client-0.4.2/dyff_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-05-09 00:38:48.000000 dyff_client-0.4.2/dyff_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 00:38:48.000000 dyff_client-0.4.2/dyff_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-05-09 00:38:48.000000 dyff_client-0.4.2/dyff_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-09 00:38:48.000000 dyff_client-0.4.2/dyff_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2024-05-09 00:38:42.000000 dyff_client-0.4.2/makefile
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-09 00:38:42.000000 dyff_client-0.4.2/package-lock.json
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-05-09 00:38:42.000000 dyff_client-0.4.2/package.json
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-05-09 00:38:42.000000 dyff_client-0.4.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.560569 dyff_client-0.4.2/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.571569 dyff_client-0.4.2/scripts/inferenceservices/
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2024-05-09 00:38:42.000000 dyff_client-0.4.2/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2024-05-09 00:38:42.000000 dyff_client-0.4.2/scripts/inferenceservices/tiiuae--falcon-7b--default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.572569 dyff_client-0.4.2/scripts/models/
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-09 00:38:42.000000 dyff_client-0.4.2/scripts/models/databricks--dolly-v2-3b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2024-05-09 00:38:42.000000 dyff_client-0.4.2/scripts/models/databricks--dolly-v2-3b.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-09 00:38:42.000000 dyff_client-0.4.2/scripts/models/tiiuae--falcon-7b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2024-05-09 00:38:42.000000 dyff_client-0.4.2/scripts/models/tiiuae--falcon-7b.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 00:38:48.573569 dyff_client-0.4.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 00:38:48.572569 dyff_client-0.4.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-09 00:38:42.000000 dyff_client-0.4.2/tests/test_import.py
```

### Comparing `dyff_client-0.3.2/.gitlab-ci.yml` & `dyff_client-0.4.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/.licenserc.yaml` & `dyff_client-0.4.2/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/.pre-commit-config.yaml` & `dyff_client-0.4.2/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
         args: ["--maxkb=600"]
       - id: check-merge-conflict
       - id: end-of-file-fixer
       - id: fix-byte-order-marker
       - id: trailing-whitespace
@@ -20,15 +20,15 @@
           - "--in-place"
           - "--expand-star-imports"
           - "--remove-duplicate-keys"
           - "--remove-unused-variables"
           - "--remove-all-unused-imports"
 
   - repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 24.4.2
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/isort
     rev: "5.13.2"
     hooks:
       - id: isort
@@ -37,31 +37,31 @@
     rev: v1.7.5
     hooks:
       - id: docformatter
         additional_dependencies: [tomli]
         args: ["--in-place", "--black", "--config", "./pyproject.toml"]
 
   - repo: https://gitlab.com/buildgarden/pipelines/skywalking-eyes
-    rev: "0.2.0"
+    rev: "0.2.1"
     hooks:
       - id: license-eye-header-fix
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
 
   - repo: https://gitlab.com/buildgarden/tools/badgie
-    rev: "0.11.2"
+    rev: "0.12.0"
     hooks:
       - id: badgie
 
   - repo: https://gitlab.com/buildgarden/tools/cici-tools
     rev: "0.7.0"
     hooks:
       - id: cici-update
 
   - repo: https://github.com/yelp/detect-secrets
-    rev: v1.4.0
+    rev: v1.5.0
     hooks:
       - id: detect-secrets
         args: ["--baseline", ".secrets.baseline"]
```

### Comparing `dyff_client-0.3.2/.secrets.baseline` & `dyff_client-0.4.2/.secrets.baseline`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'version'": "'1.5.0'"}*

```diff
@@ -141,9 +141,9 @@
                 "hashed_secret": "2b19de86010e0cae466e3a22f41b01c784884395",
                 "is_verified": false,
                 "line_number": 32,
                 "type": "Hex High Entropy String"
             }
         ]
     },
-    "version": "1.4.0"
+    "version": "1.5.0"
 }
```

### Comparing `dyff_client-0.3.2/CODE_OF_CONDUCT.md` & `dyff_client-0.4.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/LICENSE` & `dyff_client-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/PKG-INFO` & `dyff_client-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.3.2
+Version: 0.4.2
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_client-0.3.2/README.md` & `dyff_client-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/dyff/client/_generated/__init__.py` & `dyff_client-0.4.2/dyff/client/_generated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.16)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._client import DyffV0API
 
 try:
     from ._patch import *  # pylint: disable=unused-wildcard-import
```

### Comparing `dyff_client-0.3.2/dyff/client/_generated/_client.py` & `dyff_client-0.4.2/dyff/client/_generated/_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.16)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any
 
 from azure.core import PipelineClient
 from azure.core.pipeline import policies
 from azure.core.rest import HttpRequest, HttpResponse
 
 from ._configuration import DyffV0APIConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
-    AuditproceduresOperations,
-    AuditsOperations,
     DatasetsOperations,
     EvaluationsOperations,
     InferenceservicesOperations,
     InferencesessionsOperations,
     MeasurementsOperations,
     MethodsOperations,
     ModelsOperations,
@@ -28,26 +26,22 @@
     SafetycasesOperations,
 )
 
 
 class DyffV0API:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """DyffV0API.
 
-    :ivar audits: AuditsOperations operations :vartype audits:
-    _generated.operations.AuditsOperations :ivar auditprocedures:
-    AuditproceduresOperations operations :vartype auditprocedures:
-    _generated.operations.AuditproceduresOperations :ivar datasets: DatasetsOperations
-    operations :vartype datasets: _generated.operations.DatasetsOperations :ivar
-    evaluations: EvaluationsOperations operations :vartype evaluations:
-    _generated.operations.EvaluationsOperations :ivar inferenceservices:
-    InferenceservicesOperations operations :vartype inferenceservices:
-    _generated.operations.InferenceservicesOperations :ivar inferencesessions:
-    InferencesessionsOperations operations :vartype inferencesessions:
-    _generated.operations.InferencesessionsOperations :ivar measurements:
-    MeasurementsOperations operations :vartype measurements:
+    :ivar datasets: DatasetsOperations operations :vartype datasets:
+    _generated.operations.DatasetsOperations :ivar evaluations: EvaluationsOperations
+    operations :vartype evaluations: _generated.operations.EvaluationsOperations :ivar
+    inferenceservices: InferenceservicesOperations operations :vartype
+    inferenceservices: _generated.operations.InferenceservicesOperations :ivar
+    inferencesessions: InferencesessionsOperations operations :vartype
+    inferencesessions: _generated.operations.InferencesessionsOperations :ivar
+    measurements: MeasurementsOperations operations :vartype measurements:
     _generated.operations.MeasurementsOperations :ivar methods: MethodsOperations
     operations :vartype methods: _generated.operations.MethodsOperations :ivar models:
     ModelsOperations operations :vartype models: _generated.operations.ModelsOperations
     :ivar modules: ModulesOperations operations :vartype modules:
     _generated.operations.ModulesOperations :ivar reports: ReportsOperations operations
     :vartype reports: _generated.operations.ReportsOperations :ivar safetycases:
     SafetycasesOperations operations :vartype safetycases:
@@ -84,20 +78,14 @@
         self._client: PipelineClient = PipelineClient(
             base_url=endpoint, policies=_policies, **kwargs
         )
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
-        self.audits = AuditsOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
-        self.auditprocedures = AuditproceduresOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
         self.datasets = DatasetsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.evaluations = EvaluationsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.inferenceservices = InferenceservicesOperations(
```

### Comparing `dyff_client-0.3.2/dyff/client/_generated/_configuration.py` & `dyff_client-0.4.2/dyff/client/_generated/aio/_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.16)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.pipeline import policies
 
@@ -37,12 +37,14 @@
         ) or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get(
             "http_logging_policy"
         ) or policies.HttpLoggingPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get(
             "custom_hook_policy"
         ) or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(
+        self.redirect_policy = kwargs.get(
+            "redirect_policy"
+        ) or policies.AsyncRedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(
             **kwargs
         )
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
```

### Comparing `dyff_client-0.3.2/dyff/client/_generated/_patch.py` & `dyff_client-0.4.2/dyff/client/_generated/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/dyff/client/_generated/_serialization.py` & `dyff_client-0.4.2/dyff/client/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/dyff/client/_generated/_vendor.py` & `dyff_client-0.4.2/dyff/client/_generated/_vendor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.16)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 
 def raise_if_not_implemented(cls, abstract_methods):
     not_implemented = [
         f for f in abstract_methods if not callable(getattr(cls, f, None))
```

### Comparing `dyff_client-0.3.2/dyff/client/_generated/aio/__init__.py` & `dyff_client-0.4.2/dyff/client/_generated/aio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.16)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._client import DyffV0API
 
 try:
     from ._patch import *  # pylint: disable=unused-wildcard-import
```

### Comparing `dyff_client-0.3.2/dyff/client/_generated/aio/_client.py` & `dyff_client-0.4.2/dyff/client/_generated/aio/_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.16)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable
 
 from azure.core import AsyncPipelineClient
 from azure.core.pipeline import policies
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 
 from .._serialization import Deserializer, Serializer
 from ._configuration import DyffV0APIConfiguration
 from .operations import (
-    AuditproceduresOperations,
-    AuditsOperations,
     DatasetsOperations,
     EvaluationsOperations,
     InferenceservicesOperations,
     InferencesessionsOperations,
     MeasurementsOperations,
     MethodsOperations,
     ModelsOperations,
@@ -28,18 +26,14 @@
     SafetycasesOperations,
 )
 
 
 class DyffV0API:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """DyffV0API.
 
-    :ivar audits: AuditsOperations operations
-    :vartype audits: _generated.aio.operations.AuditsOperations
-    :ivar auditprocedures: AuditproceduresOperations operations
-    :vartype auditprocedures: _generated.aio.operations.AuditproceduresOperations
     :ivar datasets: DatasetsOperations operations
     :vartype datasets: _generated.aio.operations.DatasetsOperations
     :ivar evaluations: EvaluationsOperations operations
     :vartype evaluations: _generated.aio.operations.EvaluationsOperations
     :ivar inferenceservices: InferenceservicesOperations operations
     :vartype inferenceservices: _generated.aio.operations.InferenceservicesOperations
     :ivar inferencesessions: InferencesessionsOperations operations
@@ -88,20 +82,14 @@
         self._client: AsyncPipelineClient = AsyncPipelineClient(
             base_url=endpoint, policies=_policies, **kwargs
         )
 
         self._serialize = Serializer()
         self._deserialize = Deserializer()
         self._serialize.client_side_validation = False
-        self.audits = AuditsOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
-        self.auditprocedures = AuditproceduresOperations(
-            self._client, self._config, self._serialize, self._deserialize
-        )
         self.datasets = DatasetsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.evaluations = EvaluationsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.inferenceservices = InferenceservicesOperations(
```

### Comparing `dyff_client-0.3.2/dyff/client/_generated/aio/_configuration.py` & `dyff_client-0.4.2/dyff/client/_generated/_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.16)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.pipeline import policies
 
@@ -37,14 +37,12 @@
         ) or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get(
             "http_logging_policy"
         ) or policies.HttpLoggingPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get(
             "custom_hook_policy"
         ) or policies.CustomHookPolicy(**kwargs)
-        self.redirect_policy = kwargs.get(
-            "redirect_policy"
-        ) or policies.AsyncRedirectPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(
+        self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(
             **kwargs
         )
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
```

### Comparing `dyff_client-0.3.2/dyff/client/_generated/aio/_patch.py` & `dyff_client-0.4.2/dyff/client/_generated/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/dyff/client/_generated/aio/_vendor.py` & `dyff_client-0.4.2/dyff/client/_generated/aio/_vendor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.16)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 
 def raise_if_not_implemented(cls, abstract_methods):
     not_implemented = [
         f for f in abstract_methods if not callable(getattr(cls, f, None))
```

### Comparing `dyff_client-0.3.2/dyff/client/_generated/aio/operations/__init__.py` & `dyff_client-0.4.2/dyff/client/_generated/aio/operations/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.16)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import (
-    AuditproceduresOperations,
-    AuditsOperations,
     DatasetsOperations,
     EvaluationsOperations,
     InferenceservicesOperations,
     InferencesessionsOperations,
     MeasurementsOperations,
     MethodsOperations,
     ModelsOperations,
@@ -19,16 +17,14 @@
     SafetycasesOperations,
 )
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import __all__ as _patch_all
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "AuditsOperations",
-    "AuditproceduresOperations",
     "DatasetsOperations",
     "EvaluationsOperations",
     "InferenceservicesOperations",
     "InferencesessionsOperations",
     "MeasurementsOperations",
     "MethodsOperations",
     "ModelsOperations",
```

### Comparing `dyff_client-0.3.2/dyff/client/_generated/aio/operations/_operations.py` & `dyff_client-0.4.2/dyff/client/_generated/aio/operations/_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.16)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import sys
 from io import IOBase
 from typing import (
     IO,
     Any,
@@ -31,791 +31,102 @@
 )
 from azure.core.pipeline import PipelineResponse
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.utils import case_insensitive_dict
 
 from ...operations._operations import (
-    build_auditprocedures_download_request,
-    build_audits_delete_request,
-    build_audits_get_request,
-    build_audits_label_request,
-    build_audits_query_request,
     build_datasets_create_request,
     build_datasets_data_request,
     build_datasets_delete_request,
+    build_datasets_documentation_request,
+    build_datasets_edit_documentation_request,
     build_datasets_finalize_request,
     build_datasets_get_request,
     build_datasets_label_request,
     build_datasets_query_request,
     build_datasets_strata_request,
     build_datasets_upload_request,
     build_evaluations_create_request,
     build_evaluations_delete_request,
     build_evaluations_get_request,
     build_evaluations_label_request,
     build_evaluations_query_request,
     build_inferenceservices_create_request,
     build_inferenceservices_delete_request,
+    build_inferenceservices_documentation_request,
+    build_inferenceservices_edit_documentation_request,
     build_inferenceservices_get_request,
     build_inferenceservices_label_request,
     build_inferenceservices_query_request,
     build_inferencesessions_create_request,
     build_inferencesessions_delete_request,
     build_inferencesessions_get_request,
     build_inferencesessions_infer_request,
     build_inferencesessions_label_request,
     build_inferencesessions_query_request,
     build_inferencesessions_ready_request,
     build_inferencesessions_terminate_request,
     build_inferencesessions_token_request,
     build_measurements_create_request,
     build_measurements_delete_request,
+    build_measurements_downlinks_request,
     build_measurements_get_request,
     build_measurements_label_request,
     build_measurements_query_request,
     build_methods_create_request,
     build_methods_delete_request,
+    build_methods_documentation_request,
+    build_methods_edit_documentation_request,
     build_methods_get_request,
     build_methods_label_request,
     build_methods_query_request,
     build_models_create_request,
     build_models_delete_request,
+    build_models_documentation_request,
+    build_models_edit_documentation_request,
     build_models_get_request,
     build_models_label_request,
     build_models_query_request,
     build_modules_create_request,
     build_modules_delete_request,
+    build_modules_documentation_request,
+    build_modules_edit_documentation_request,
     build_modules_finalize_request,
     build_modules_get_request,
     build_modules_label_request,
     build_modules_query_request,
     build_modules_upload_request,
     build_reports_create_request,
     build_reports_data_request,
     build_reports_delete_request,
     build_reports_get_request,
     build_reports_label_request,
     build_reports_query_request,
     build_safetycases_create_request,
     build_safetycases_delete_request,
+    build_safetycases_downlinks_request,
     build_safetycases_get_request,
     build_safetycases_label_request,
     build_safetycases_query_request,
 )
-from .._vendor import raise_if_not_implemented
 
 if sys.version_info >= (3, 9):
     from collections.abc import MutableMapping
 else:
     from typing import (
         MutableMapping,  # type: ignore  # pylint: disable=ungrouped-imports
     )
 JSON = MutableMapping[str, Any]  # pylint: disable=unsubscriptable-object
 T = TypeVar("T")
 ClsType = Optional[
     Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]
 ]
 
 
-class AuditsOperations:  # pylint: disable=abstract-class-instantiated
-    """
-    .. warning::
-        **DO NOT** instantiate this class directly.
-
-        Instead, you should access the following operations through
-        :class:`~_generated.aio.DyffV0API`'s
-        :attr:`audits` attribute.
-    """
-
-    def __init__(self, *args, **kwargs) -> None:
-        input_args = list(args)
-        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
-        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
-        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
-        self._deserialize = (
-            input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        )
-
-        raise_if_not_implemented(
-            self.__class__,
-            [
-                "upload",
-            ],
-        )
-
-    @overload
-    async def label(
-        self,
-        audit_id: str,
-        body: JSON,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any,
-    ) -> Union[Any, JSON]:
-        # pylint: disable=line-too-long
-        """Update labels for an existing Audit.
-
-        Update labels for an existing Audit.
-
-        :param audit_id: Required.
-        :type audit_id: str
-        :param body: Required.
-        :type body: JSON
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: any or JSON object
-        :rtype: any or JSON
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # JSON input template you can fill out and use as your body input.
-                body = {
-                    "labels": {
-                        "str": "str"  # Optional. A set of key-value labels for the resource.
-                          Used to specify identifying attributes of resources that are meaningful to
-                          users but do not imply semantics in the dyff system.  The keys are DNS labels
-                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
-                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
-                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
-                          follow the kubernetes label conventions closely. See:
-                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
-                }
-
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-
-    @overload
-    async def label(
-        self,
-        audit_id: str,
-        body: IO[bytes],
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any,
-    ) -> Union[Any, JSON]:
-        """Update labels for an existing Audit.
-
-        Update labels for an existing Audit.
-
-        :param audit_id: Required.
-        :type audit_id: str
-        :param body: Required.
-        :type body: IO[bytes]
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: any or JSON object
-        :rtype: any or JSON
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-
-    @distributed_trace_async
-    async def label(
-        self, audit_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
-    ) -> Union[Any, JSON]:
-        # pylint: disable=line-too-long
-        """Update labels for an existing Audit.
-
-        Update labels for an existing Audit.
-
-        :param audit_id: Required.
-        :type audit_id: str
-        :param body: Is either a JSON type or a IO[bytes] type. Required.
-        :type body: JSON or IO[bytes]
-        :return: any or JSON object
-        :rtype: any or JSON
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # JSON input template you can fill out and use as your body input.
-                body = {
-                    "labels": {
-                        "str": "str"  # Optional. A set of key-value labels for the resource.
-                          Used to specify identifying attributes of resources that are meaningful to
-                          users but do not imply semantics in the dyff system.  The keys are DNS labels
-                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
-                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
-                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
-                          follow the kubernetes label conventions closely. See:
-                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
-                }
-
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-        error_map: MutableMapping[int, Type[HttpResponseError]] = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = kwargs.pop("params", {}) or {}
-
-        content_type: Optional[str] = kwargs.pop(
-            "content_type", _headers.pop("Content-Type", None)
-        )
-        cls: ClsType[Union[Any, JSON]] = kwargs.pop("cls", None)
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(body, (IOBase, bytes)):
-            _content = body
-        else:
-            _json = body
-
-        _request = build_audits_label_request(
-            audit_id=audit_id,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            headers=_headers,
-            params=_params,
-        )
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = (
-            await self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 422]:
-            if _stream:
-                await response.read()  # Load the body in memory and close the socket
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
-
-        if response.status_code == 200:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if response.status_code == 422:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if cls:
-            return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
-
-        return cast(Union[Any, JSON], deserialized)  # type: ignore
-
-    @distributed_trace_async
-    async def query(
-        self,
-        *,
-        id: Optional[str] = None,
-        account: Optional[str] = None,
-        status: Optional[str] = None,
-        reason: Optional[str] = None,
-        labels: Optional[str] = None,
-        name: Optional[str] = None,
-        **kwargs: Any,
-    ) -> Union[List[JSON], JSON]:
-        # pylint: disable=line-too-long
-        """Get all Audits matching a query.
-
-        Get all Audits matching a query. The query is a set of equality
-        constraints specified as key-value pairs.
-
-        :keyword id: Default value is None.
-        :paramtype id: str
-        :keyword account: Default value is None.
-        :paramtype account: str
-        :keyword status: Default value is None.
-        :paramtype status: str
-        :keyword reason: Default value is None.
-        :paramtype reason: str
-        :keyword labels: Default value is None.
-        :paramtype labels: str
-        :keyword name: Default value is None.
-        :paramtype name: str
-        :return: list of JSON object or JSON object
-        :rtype: list[JSON] or JSON
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # response body for status code(s): 200
-                response == [
-                    {
-                        "account": "str",  # Account that owns the entity. Required.
-                        "auditProcedure": "str",  # The AuditProcedure to run. Required.
-                        "id": "str",  # Unique identifier of the entity. Required.
-                        "inferenceService": "str",  # The InferenceService to audit.
-                          Required.
-                        "annotations": [
-                            {
-                                "key": "str",  # The annotation key. A DNS label with
-                                  an optional DNS domain prefix. For example: 'my-key',
-                                  'your.com/key_0'. Names prefixed with 'dyff.io/',
-                                  'subdomain.dyff.io/', etc. are reserved.  See
-                                  https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
-                                  for detailed naming rules. Required.
-                                "value": "str"  # The annotation value. An arbitrary
-                                  string. Required.
-                            }
-                        ],
-                        "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation
-                          time (assigned by system).
-                        "kind": "Audit",  # Optional. Default value is "Audit". Kind. "Audit"
-                        "labels": {
-                            "str": "str"  # Optional. A set of key-value labels for the
-                              resource. Used to specify identifying attributes of resources that are
-                              meaningful to users but do not imply semantics in the dyff system.  The
-                              keys are DNS labels with an optional DNS domain prefix. For example:
-                              'my-key', 'your.com/key_0'. Keys prefixed with 'dyff.io/',
-                              'subdomain.dyff.io/', etc. are reserved.  The label values are
-                              alphanumeric characters separated by '.', '-', or '_'.  We follow the
-                              kubernetes label conventions closely. See:
-                              https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                        },
-                        "reason": "str",  # Optional. Reason for current status (assigned by
-                          system).
-                        "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
-                          schema version. "0.1"
-                        "status": "str"  # Optional. Top-level resource status (assigned by
-                          system).
-                    }
-                ]
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-        error_map: MutableMapping[int, Type[HttpResponseError]] = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = kwargs.pop("params", {}) or {}
-
-        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
-
-        _request = build_audits_query_request(
-            id=id,
-            account=account,
-            status=status,
-            reason=reason,
-            labels=labels,
-            name=name,
-            headers=_headers,
-            params=_params,
-        )
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = (
-            await self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 422]:
-            if _stream:
-                await response.read()  # Load the body in memory and close the socket
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
-
-        if response.status_code == 200:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if response.status_code == 422:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if cls:
-            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
-
-        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
-
-    @distributed_trace_async
-    async def get(self, audit_id: str, **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
-        """Get an Audit by its key.
-
-        Get an Audit by its key. Raises a 404 error if no entity exists with that key.
-
-        :param audit_id: Required.
-        :type audit_id: str
-        :return: JSON object
-        :rtype: JSON
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # response body for status code(s): 200
-                response == {
-                    "account": "str",  # Account that owns the entity. Required.
-                    "auditProcedure": "str",  # The AuditProcedure to run. Required.
-                    "id": "str",  # Unique identifier of the entity. Required.
-                    "inferenceService": "str",  # The InferenceService to audit. Required.
-                    "annotations": [
-                        {
-                            "key": "str",  # The annotation key. A DNS label with an
-                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
-                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
-                              See
-                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
-                              for detailed naming rules. Required.
-                            "value": "str"  # The annotation value. An arbitrary string.
-                              Required.
-                        }
-                    ],
-                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
-                      (assigned by system).
-                    "kind": "Audit",  # Optional. Default value is "Audit". Kind. "Audit"
-                    "labels": {
-                        "str": "str"  # Optional. A set of key-value labels for the resource.
-                          Used to specify identifying attributes of resources that are meaningful to
-                          users but do not imply semantics in the dyff system.  The keys are DNS labels
-                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
-                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
-                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
-                          follow the kubernetes label conventions closely. See:
-                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    },
-                    "reason": "str",  # Optional. Reason for current status (assigned by system).
-                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
-                      version. "0.1"
-                    "status": "str"  # Optional. Top-level resource status (assigned by system).
-                }
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-        error_map: MutableMapping[int, Type[HttpResponseError]] = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = kwargs.pop("params", {}) or {}
-
-        cls: ClsType[JSON] = kwargs.pop("cls", None)
-
-        _request = build_audits_get_request(
-            audit_id=audit_id,
-            headers=_headers,
-            params=_params,
-        )
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = (
-            await self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 422]:
-            if _stream:
-                await response.read()  # Load the body in memory and close the socket
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
-
-        if response.status_code == 200:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if response.status_code == 422:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
-
-        return cast(JSON, deserialized)  # type: ignore
-
-    @distributed_trace_async
-    async def delete(self, audit_id: str, **kwargs: Any) -> JSON:
-        """Mark an Audit for deletion.
-
-        Mark an Audit for deletion.
-
-        :param audit_id: Required.
-        :type audit_id: str
-        :return: JSON object
-        :rtype: JSON
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # response body for status code(s): 200
-                response == {
-                    "reason": "str",  # Optional. Reason for current status (assigned by system).
-                    "status": "str"  # Optional. Top-level resource status (assigned by system).
-                }
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-        error_map: MutableMapping[int, Type[HttpResponseError]] = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = kwargs.pop("params", {}) or {}
-
-        cls: ClsType[JSON] = kwargs.pop("cls", None)
-
-        _request = build_audits_delete_request(
-            audit_id=audit_id,
-            headers=_headers,
-            params=_params,
-        )
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = (
-            await self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 422]:
-            if _stream:
-                await response.read()  # Load the body in memory and close the socket
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
-
-        if response.status_code == 200:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if response.status_code == 422:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
-
-        return cast(JSON, deserialized)  # type: ignore
-
-
-class AuditproceduresOperations:
-    """
-    .. warning::
-        **DO NOT** instantiate this class directly.
-
-        Instead, you should access the following operations through
-        :class:`~_generated.aio.DyffV0API`'s
-        :attr:`auditprocedures` attribute.
-    """
-
-    def __init__(self, *args, **kwargs) -> None:
-        input_args = list(args)
-        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
-        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
-        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
-        self._deserialize = (
-            input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        )
-
-    @distributed_trace_async
-    async def download(
-        self, path: str, **kwargs: Any
-    ) -> Union[AsyncIterator[bytes], JSON]:
-        """Download the source code of an AuditProcedure.
-
-        Download the source code of an AuditProcedure.
-
-        :param path: Required.
-        :type path: str
-        :return: AsyncIterator[bytes] or JSON object or None
-        :rtype: AsyncIterator[bytes] or JSON or None
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-        error_map: MutableMapping[int, Type[HttpResponseError]] = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = kwargs.pop("params", {}) or {}
-
-        cls: ClsType[Union[AsyncIterator[bytes], JSON]] = kwargs.pop("cls", None)
-
-        _request = build_auditprocedures_download_request(
-            path=path,
-            headers=_headers,
-            params=_params,
-        )
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = True
-        pipeline_response: PipelineResponse = (
-            await self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 404, 422]:
-            if _stream:
-                await response.read()  # Load the body in memory and close the socket
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
-
-        deserialized = None
-        if response.status_code == 200:
-            deserialized = response.iter_bytes()
-
-        if response.status_code == 422:
-            deserialized = response.iter_bytes()
-
-        if cls:
-            return cls(pipeline_response, deserialized, {})  # type: ignore
-
-        return deserialized  # type: ignore
-
-
 class DatasetsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~_generated.aio.DyffV0API`'s
@@ -1082,20 +393,21 @@
 
                 # response body for status code(s): 200
                 response == [
                     {
                         "account": "str",  # Account that owns the entity. Required.
                         "artifacts": [
                             {
+                                "path": "str",  # The relative path of the artifact
+                                  within the tree. Required.
                                 "digest": {
-                                    "md5": "str"  # Optional. Md5.
+                                    "md5": "str"  # Optional. md5 digest of
+                                      artifact data.
                                 },
-                                "kind": "str",  # The kind of artifact. Required.
-                                "path": "str"  # The relative path of the artifact
-                                  within the dataset. Required.
+                                "kind": "str"  # Optional. The kind of artifact.
                             }
                         ],
                         "id": "str",  # Unique identifier of the entity. Required.
                         "name": "str",  # The name of the Dataset. Required.
                         "schema": {
                             "arrowSchema": "str",  # The schema in Arrow format, encoded
                               with dyff.schema.arrow.encode_schema(). This is required, but can be
@@ -1273,20 +585,21 @@
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "name": "str",  # The name of the Dataset. Required.
                     "schema": {
                         "arrowSchema": "str",  # The schema in Arrow format, encoded with
                           dyff.schema.arrow.encode_schema(). This is required, but can be populated
                           from a DyffDataSchema. Required.
@@ -1336,20 +649,21 @@
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Dataset. Required.
                     "schema": {
                         "arrowSchema": "str",  # The schema in Arrow format, encoded with
                           dyff.schema.arrow.encode_schema(). This is required, but can be populated
@@ -1461,20 +775,21 @@
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Dataset. Required.
                     "schema": {
                         "arrowSchema": "str",  # The schema in Arrow format, encoded with
                           dyff.schema.arrow.encode_schema(). This is required, but can be populated
@@ -1581,20 +896,21 @@
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "name": "str",  # The name of the Dataset. Required.
                     "schema": {
                         "arrowSchema": "str",  # The schema in Arrow format, encoded with
                           dyff.schema.arrow.encode_schema(). This is required, but can be populated
                           from a DyffDataSchema. Required.
@@ -1644,20 +960,21 @@
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Dataset. Required.
                     "schema": {
                         "arrowSchema": "str",  # The schema in Arrow format, encoded with
                           dyff.schema.arrow.encode_schema(). This is required, but can be populated
@@ -1830,20 +1147,21 @@
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Dataset. Required.
                     "schema": {
                         "arrowSchema": "str",  # The schema in Arrow format, encoded with
                           dyff.schema.arrow.encode_schema(). This is required, but can be populated
@@ -2405,14 +1723,348 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
+    @distributed_trace_async
+    async def documentation(self, dataset_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get the documentation associated with a Dataset.
+
+        Get the documentation associated with a Dataset. Raises a 404
+        error if no entity exists with that key.
+
+        :param dataset_id: Required.
+        :type dataset_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_datasets_documentation_request(
+            dataset_id=dataset_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @overload
+    async def edit_documentation(
+        self,
+        dataset_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Dataset.
+
+        Edit the documentation associated with a Dataset. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param dataset_id: Required.
+        :type dataset_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    async def edit_documentation(
+        self,
+        dataset_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Dataset.
+
+        Edit the documentation associated with a Dataset. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param dataset_id: Required.
+        :type dataset_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace_async
+    async def edit_documentation(
+        self, dataset_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Dataset.
+
+        Edit the documentation associated with a Dataset. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param dataset_id: Required.
+        :type dataset_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_datasets_edit_documentation_request(
+            dataset_id=dataset_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
 
 class EvaluationsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -5856,14 +5508,348 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
+    @distributed_trace_async
+    async def documentation(self, service_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get the documentation associated with an InferenceService.
+
+        Get the documentation associated with an InferenceService. Raises a 404
+        error if no entity exists with that key.
+
+        :param service_id: Required.
+        :type service_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_inferenceservices_documentation_request(
+            service_id=service_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @overload
+    async def edit_documentation(
+        self,
+        service_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with an InferenceService.
+
+        Edit the documentation associated with an InferenceService. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param service_id: Required.
+        :type service_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    async def edit_documentation(
+        self,
+        service_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with an InferenceService.
+
+        Edit the documentation associated with an InferenceService. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param service_id: Required.
+        :type service_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace_async
+    async def edit_documentation(
+        self, service_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with an InferenceService.
+
+        Edit the documentation associated with an InferenceService. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param service_id: Required.
+        :type service_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_inferenceservices_edit_documentation_request(
+            service_id=service_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
 
 class InferencesessionsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -8304,20 +8290,14 @@
                                 ],
                                 "schemaVersion": "0.1"  # Optional. Default value is
                                   "0.1". The dyff schema version. "0.1"
                             },
                             "jsonSchema": {}  # Optional. The schema in JSON Schema
                               format.
                         },
-                        "scope": {
-                            "dataset": "str",  # Optional. Dataset.
-                            "evaluation": "str",  # Optional. Evaluation.
-                            "inferenceService": "str",  # Optional. Inferenceservice.
-                            "model": "str"  # Optional. Model.
-                        },
                         "annotations": [
                             {
                                 "key": "str",  # The annotation key. A DNS label with
                                   an optional DNS domain prefix. For example: 'my-key',
                                   'your.com/key_0'. Names prefixed with 'dyff.io/',
                                   'subdomain.dyff.io/', etc. are reserved.  See
                                   https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -8360,14 +8340,24 @@
                               kubernetes label conventions closely. See:
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                         },
                         "reason": "str",  # Optional. Reason for current status (assigned by
                           system).
                         "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
                           schema version. "0.1"
+                        "scope": {
+                            "dataset": "str",  # Optional. The Dataset to which the
+                              analysis applies.
+                            "evaluation": "str",  # Optional. The Evaluation to which the
+                              analysis applies.
+                            "inferenceService": "str",  # Optional. The InferenceService
+                              to which the analysis applies.
+                            "model": "str"  # Optional. The Model to which the analysis
+                              applies.
+                        },
                         "status": "str"  # Optional. Top-level resource status (assigned by
                           system).
                     }
                 ]
                 # response body for status code(s): 422
                 response == {
                     "detail": [
@@ -8464,20 +8454,14 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "method": "str",  # Method ID. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "arguments": [
                         {
                             "keyword": "str",  # The 'keyword' of the corresponding
                               ModelParameter. Required.
                             "value": "str"  # The value of of the argument. Always a
                               string; implementations are responsible for parsing. Required.
                         }
@@ -8486,16 +8470,25 @@
                         {
                             "entity": "str",  # The ID of the entity whose data should be
                               made available as 'keyword'. Required.
                             "keyword": "str"  # The 'keyword' specified for this input in
                               the MethodSpec. Required.
                         }
                     ],
-                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    }
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "id": "str",  # Unique identifier of the entity. Required.
                     "level": "str",  # Measurement level. Required. Known values are: "Dataset"
@@ -8596,20 +8589,14 @@
                                   schema is the composition of these component schemas. Required.
                             ],
                             "schemaVersion": "0.1"  # Optional. Default value is "0.1".
                               The dyff schema version. "0.1"
                         },
                         "jsonSchema": {}  # Optional. The schema in JSON Schema format.
                     },
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -8649,14 +8636,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -8792,20 +8788,14 @@
                                   schema is the composition of these component schemas. Required.
                             ],
                             "schemaVersion": "0.1"  # Optional. Default value is "0.1".
                               The dyff schema version. "0.1"
                         },
                         "jsonSchema": {}  # Optional. The schema in JSON Schema format.
                     },
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -8845,14 +8835,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -8881,20 +8880,14 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "method": "str",  # Method ID. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "arguments": [
                         {
                             "keyword": "str",  # The 'keyword' of the corresponding
                               ModelParameter. Required.
                             "value": "str"  # The value of of the argument. Always a
                               string; implementations are responsible for parsing. Required.
                         }
@@ -8903,16 +8896,25 @@
                         {
                             "entity": "str",  # The ID of the entity whose data should be
                               made available as 'keyword'. Required.
                             "keyword": "str"  # The 'keyword' specified for this input in
                               the MethodSpec. Required.
                         }
                     ],
-                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    }
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "id": "str",  # Unique identifier of the entity. Required.
                     "level": "str",  # Measurement level. Required. Known values are: "Dataset"
@@ -9013,20 +9015,14 @@
                                   schema is the composition of these component schemas. Required.
                             ],
                             "schemaVersion": "0.1"  # Optional. Default value is "0.1".
                               The dyff schema version. "0.1"
                         },
                         "jsonSchema": {}  # Optional. The schema in JSON Schema format.
                     },
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -9066,14 +9062,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -9270,20 +9275,14 @@
                                   schema is the composition of these component schemas. Required.
                             ],
                             "schemaVersion": "0.1"  # Optional. Default value is "0.1".
                               The dyff schema version. "0.1"
                         },
                         "jsonSchema": {}  # Optional. The schema in JSON Schema format.
                     },
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -9323,14 +9322,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -9479,14 +9487,122 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
+    @distributed_trace_async
+    async def downlinks(
+        self, measurement_id: str, **kwargs: Any
+    ) -> Union[List[JSON], JSON]:
+        """Get a list of signed GET URLs from which measurement artifacts can be
+        downloaded.
+
+        Get a list of signed GET URLs from which measurement artifacts can be downloaded.
+
+        :param measurement_id: Required.
+        :type measurement_id: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "artifact": {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
+                            "digest": {
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
+                            },
+                            "kind": "str"  # Optional. The kind of artifact.
+                        },
+                        "signedURL": {
+                            "method": "str",  # The HTTP method applicable to the URL.
+                              Required.
+                            "url": "str",  # The signed URL. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Mandatory headers that must
+                                  be passed with the request.
+                            }
+                        }
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_measurements_downlinks_request(
+            measurement_id=measurement_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
+
 
 class MethodsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -10905,14 +11021,348 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
+    @distributed_trace_async
+    async def documentation(self, method_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get the documentation associated with a Method.
+
+        Get the documentation associated with a Method. Raises a 404
+        error if no entity exists with that key.
+
+        :param method_id: Required.
+        :type method_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_methods_documentation_request(
+            method_id=method_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @overload
+    async def edit_documentation(
+        self,
+        method_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Method.
+
+        Edit the documentation associated with a Method. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param method_id: Required.
+        :type method_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    async def edit_documentation(
+        self,
+        method_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Method.
+
+        Edit the documentation associated with a Method. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param method_id: Required.
+        :type method_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace_async
+    async def edit_documentation(
+        self, method_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Method.
+
+        Edit the documentation associated with a Method. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param method_id: Required.
+        :type method_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_methods_edit_documentation_request(
+            method_id=method_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
 
 class ModelsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -12199,14 +12649,348 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
+    @distributed_trace_async
+    async def documentation(self, model_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get the documentation associated with a Model.
+
+        Get the documentation associated with a Model. Raises a 404
+        error if no entity exists with that key.
+
+        :param model_id: Required.
+        :type model_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_models_documentation_request(
+            model_id=model_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @overload
+    async def edit_documentation(
+        self,
+        model_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Model.
+
+        Edit the documentation associated with a Model. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param model_id: Required.
+        :type model_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    async def edit_documentation(
+        self,
+        model_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Model.
+
+        Edit the documentation associated with a Model. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param model_id: Required.
+        :type model_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace_async
+    async def edit_documentation(
+        self, model_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Model.
+
+        Edit the documentation associated with a Model. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param model_id: Required.
+        :type model_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_models_edit_documentation_request(
+            model_id=model_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
 
 class ModulesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -12474,20 +13258,21 @@
 
                 # response body for status code(s): 200
                 response == [
                     {
                         "account": "str",  # Account that owns the entity. Required.
                         "artifacts": [
                             {
+                                "path": "str",  # The relative path of the artifact
+                                  within the tree. Required.
                                 "digest": {
-                                    "md5": "str"  # Optional. Md5.
+                                    "md5": "str"  # Optional. md5 digest of
+                                      artifact data.
                                 },
-                                "kind": "str",  # The kind of artifact. Required.
-                                "path": "str"  # The relative path of the artifact
-                                  within the dataset. Required.
+                                "kind": "str"  # Optional. The kind of artifact.
                             }
                         ],
                         "id": "str",  # Unique identifier of the entity. Required.
                         "name": "str",  # The name of the Module. Required.
                         "annotations": [
                             {
                                 "key": "str",  # The annotation key. A DNS label with
@@ -12617,38 +13402,40 @@
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "name": "str",  # The name of the Module. Required.
                     "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Module. Required.
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
@@ -12715,20 +13502,21 @@
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Module. Required.
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
@@ -12790,38 +13578,40 @@
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "name": "str",  # The name of the Module. Required.
                     "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Module. Required.
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
@@ -12949,20 +13739,21 @@
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Module. Required.
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
@@ -13319,14 +14110,348 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
+    @distributed_trace_async
+    async def documentation(self, module_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get the documentation associated with a Module.
+
+        Get the documentation associated with a Module. Raises a 404
+        error if no entity exists with that key.
+
+        :param module_id: Required.
+        :type module_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_modules_documentation_request(
+            module_id=module_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @overload
+    async def edit_documentation(
+        self,
+        module_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Module.
+
+        Edit the documentation associated with a Module. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param module_id: Required.
+        :type module_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    async def edit_documentation(
+        self,
+        module_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Module.
+
+        Edit the documentation associated with a Module. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param module_id: Required.
+        :type module_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace_async
+    async def edit_documentation(
+        self, module_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Module.
+
+        Edit the documentation associated with a Module. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param module_id: Required.
+        :type module_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_modules_edit_documentation_request(
+            module_id=module_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
 
 class ReportsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -15031,20 +16156,14 @@
                                       implementation. Required.
                                     "description": "str"  # Optional. Long-form
                                       description, interpreted as Markdown.
                                 }
                             ]
                         },
                         "name": "str",  # Descriptive name of the SafetyCase. Required.
-                        "scope": {
-                            "dataset": "str",  # Optional. Dataset.
-                            "evaluation": "str",  # Optional. Evaluation.
-                            "inferenceService": "str",  # Optional. Inferenceservice.
-                            "model": "str"  # Optional. Model.
-                        },
                         "annotations": [
                             {
                                 "key": "str",  # The annotation key. A DNS label with
                                   an optional DNS domain prefix. For example: 'my-key',
                                   'your.com/key_0'. Names prefixed with 'dyff.io/',
                                   'subdomain.dyff.io/', etc. are reserved.  See
                                   https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -15087,14 +16206,24 @@
                               kubernetes label conventions closely. See:
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                         },
                         "reason": "str",  # Optional. Reason for current status (assigned by
                           system).
                         "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
                           schema version. "0.1"
+                        "scope": {
+                            "dataset": "str",  # Optional. The Dataset to which the
+                              analysis applies.
+                            "evaluation": "str",  # Optional. The Evaluation to which the
+                              analysis applies.
+                            "inferenceService": "str",  # Optional. The InferenceService
+                              to which the analysis applies.
+                            "model": "str"  # Optional. The Model to which the analysis
+                              applies.
+                        },
                         "status": "str"  # Optional. Top-level resource status (assigned by
                           system).
                     }
                 ]
                 # response body for status code(s): 422
                 response == {
                     "detail": [
@@ -15191,20 +16320,14 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "method": "str",  # Method ID. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "arguments": [
                         {
                             "keyword": "str",  # The 'keyword' of the corresponding
                               ModelParameter. Required.
                             "value": "str"  # The value of of the argument. Always a
                               string; implementations are responsible for parsing. Required.
                         }
@@ -15213,16 +16336,25 @@
                         {
                             "entity": "str",  # The ID of the entity whose data should be
                               made available as 'keyword'. Required.
                             "keyword": "str"  # The 'keyword' specified for this input in
                               the MethodSpec. Required.
                         }
                     ],
-                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    }
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "id": "str",  # Unique identifier of the entity. Required.
                     "method": {
@@ -15307,20 +16439,14 @@
                                   'keyword' in the context of the method implementation. Required.
                                 "description": "str"  # Optional. Long-form
                                   description, interpreted as Markdown.
                             }
                         ]
                     },
                     "name": "str",  # Descriptive name of the SafetyCase. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -15360,14 +16486,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -15487,20 +16622,14 @@
                                   'keyword' in the context of the method implementation. Required.
                                 "description": "str"  # Optional. Long-form
                                   description, interpreted as Markdown.
                             }
                         ]
                     },
                     "name": "str",  # Descriptive name of the SafetyCase. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -15540,14 +16669,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -15576,20 +16714,14 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "method": "str",  # Method ID. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "arguments": [
                         {
                             "keyword": "str",  # The 'keyword' of the corresponding
                               ModelParameter. Required.
                             "value": "str"  # The value of of the argument. Always a
                               string; implementations are responsible for parsing. Required.
                         }
@@ -15598,16 +16730,25 @@
                         {
                             "entity": "str",  # The ID of the entity whose data should be
                               made available as 'keyword'. Required.
                             "keyword": "str"  # The 'keyword' specified for this input in
                               the MethodSpec. Required.
                         }
                     ],
-                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    }
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "id": "str",  # Unique identifier of the entity. Required.
                     "method": {
@@ -15692,20 +16833,14 @@
                                   'keyword' in the context of the method implementation. Required.
                                 "description": "str"  # Optional. Long-form
                                   description, interpreted as Markdown.
                             }
                         ]
                     },
                     "name": "str",  # Descriptive name of the SafetyCase. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -15745,14 +16880,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -15933,20 +17077,14 @@
                                   'keyword' in the context of the method implementation. Required.
                                 "description": "str"  # Optional. Long-form
                                   description, interpreted as Markdown.
                             }
                         ]
                     },
                     "name": "str",  # Descriptive name of the SafetyCase. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -15986,14 +17124,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -16141,7 +17288,115 @@
             else:
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace_async
+    async def downlinks(
+        self, safetycase_id: str, **kwargs: Any
+    ) -> Union[List[JSON], JSON]:
+        """Get a list of signed GET URLs from which safety case artifacts can be
+        downloaded.
+
+        Get a list of signed GET URLs from which safety case artifacts can be downloaded.
+
+        :param safetycase_id: Required.
+        :type safetycase_id: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "artifact": {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
+                            "digest": {
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
+                            },
+                            "kind": "str"  # Optional. The kind of artifact.
+                        },
+                        "signedURL": {
+                            "method": "str",  # The HTTP method applicable to the URL.
+                              Required.
+                            "url": "str",  # The signed URL. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Mandatory headers that must
+                                  be passed with the request.
+                            }
+                        }
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_safetycases_downlinks_request(
+            safetycase_id=safetycase_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                await response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
```

### Comparing `dyff_client-0.3.2/dyff/client/_generated/aio/operations/_patch.py` & `dyff_client-0.4.2/dyff/client/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/dyff/client/_generated/operations/__init__.py` & `dyff_client-0.4.2/dyff/client/_generated/operations/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.16)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import (
-    AuditproceduresOperations,
-    AuditsOperations,
     DatasetsOperations,
     EvaluationsOperations,
     InferenceservicesOperations,
     InferencesessionsOperations,
     MeasurementsOperations,
     MethodsOperations,
     ModelsOperations,
@@ -19,16 +17,14 @@
     SafetycasesOperations,
 )
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import __all__ as _patch_all
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
-    "AuditsOperations",
-    "AuditproceduresOperations",
     "DatasetsOperations",
     "EvaluationsOperations",
     "InferenceservicesOperations",
     "InferencesessionsOperations",
     "MeasurementsOperations",
     "MethodsOperations",
     "ModelsOperations",
```

### Comparing `dyff_client-0.3.2/dyff/client/_generated/operations/_operations.py` & `dyff_client-0.4.2/dyff/client/_generated/operations/_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.12)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.10.2, generator: @autorest/python@6.13.16)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import sys
 from io import IOBase
 from typing import (
     IO,
     Any,
@@ -31,15 +31,14 @@
 )
 from azure.core.pipeline import PipelineResponse
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 
 from .._serialization import Serializer
-from .._vendor import raise_if_not_implemented
 
 if sys.version_info >= (3, 9):
     from collections.abc import MutableMapping
 else:
     from typing import (
         MutableMapping,  # type: ignore  # pylint: disable=ungrouped-imports
     )
@@ -49,137 +48,14 @@
     Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]
 ]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_audits_label_request(audit_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    content_type: Optional[str] = kwargs.pop(
-        "content_type", _headers.pop("Content-Type", None)
-    )
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/audits/{audit_id}/labels"
-    path_format_arguments = {
-        "audit_id": _SERIALIZER.url("audit_id", audit_id, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header(
-            "content_type", content_type, "str"
-        )
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
-
-
-def build_audits_query_request(
-    *,
-    id: Optional[str] = None,
-    account: Optional[str] = None,
-    status: Optional[str] = None,
-    reason: Optional[str] = None,
-    labels: Optional[str] = None,
-    name: Optional[str] = None,
-    **kwargs: Any,
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/audits"
-
-    # Construct parameters
-    if id is not None:
-        _params["id"] = _SERIALIZER.query("id", id, "str")
-    if account is not None:
-        _params["account"] = _SERIALIZER.query("account", account, "str")
-    if status is not None:
-        _params["status"] = _SERIALIZER.query("status", status, "str")
-    if reason is not None:
-        _params["reason"] = _SERIALIZER.query("reason", reason, "str")
-    if labels is not None:
-        _params["labels"] = _SERIALIZER.query("labels", labels, "str")
-    if name is not None:
-        _params["name"] = _SERIALIZER.query("name", name, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(
-        method="GET", url=_url, params=_params, headers=_headers, **kwargs
-    )
-
-
-def build_audits_get_request(audit_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/audits/{audit_id}"
-    path_format_arguments = {
-        "audit_id": _SERIALIZER.url("audit_id", audit_id, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
-
-
-def build_audits_delete_request(audit_id: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/audits/{audit_id}/delete"
-    path_format_arguments = {
-        "audit_id": _SERIALIZER.url("audit_id", audit_id, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
-
-
-def build_auditprocedures_download_request(path: str, **kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/auditprocedures/{path}/download"
-    path_format_arguments = {
-        "path": _SERIALIZER.url("path", path, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
-
-
 def build_datasets_label_request(dataset_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
     )
     accept = _headers.pop("Accept", "application/json")
@@ -376,14 +252,61 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
+def build_datasets_documentation_request(dataset_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/datasets/{dataset_id}/documentation"
+    path_format_arguments = {
+        "dataset_id": _SERIALIZER.url("dataset_id", dataset_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_datasets_edit_documentation_request(  # pylint: disable=name-too-long
+    dataset_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop(
+        "content_type", _headers.pop("Content-Type", None)
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/datasets/{dataset_id}/documentation"
+    path_format_arguments = {
+        "dataset_id": _SERIALIZER.url("dataset_id", dataset_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header(
+            "content_type", content_type, "str"
+        )
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
+
+
 def build_evaluations_label_request(evaluation_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
     )
     accept = _headers.pop("Accept", "application/json")
@@ -652,14 +575,63 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
 
 
+def build_inferenceservices_documentation_request(  # pylint: disable=name-too-long
+    service_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/inferenceservices/{service_id}/documentation"
+    path_format_arguments = {
+        "service_id": _SERIALIZER.url("service_id", service_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_inferenceservices_edit_documentation_request(  # pylint: disable=name-too-long
+    service_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop(
+        "content_type", _headers.pop("Content-Type", None)
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/inferenceservices/{service_id}/documentation"
+    path_format_arguments = {
+        "service_id": _SERIALIZER.url("service_id", service_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header(
+            "content_type", content_type, "str"
+        )
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
+
+
 def build_inferencesessions_label_request(
     session_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
@@ -1022,14 +994,35 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
 
 
+def build_measurements_downlinks_request(
+    measurement_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/measurements/{measurement_id}/downlinks"
+    path_format_arguments = {
+        "measurement_id": _SERIALIZER.url("measurement_id", measurement_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
 def build_methods_label_request(method_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
     )
     accept = _headers.pop("Accept", "application/json")
@@ -1150,14 +1143,61 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
 
 
+def build_methods_documentation_request(method_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/methods/{method_id}/documentation"
+    path_format_arguments = {
+        "method_id": _SERIALIZER.url("method_id", method_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_methods_edit_documentation_request(
+    method_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop(
+        "content_type", _headers.pop("Content-Type", None)
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/methods/{method_id}/documentation"
+    path_format_arguments = {
+        "method_id": _SERIALIZER.url("method_id", method_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header(
+            "content_type", content_type, "str"
+        )
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
+
+
 def build_models_label_request(model_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
     )
     accept = _headers.pop("Accept", "application/json")
@@ -1275,14 +1315,61 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
 
 
+def build_models_documentation_request(model_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/models/{model_id}/documentation"
+    path_format_arguments = {
+        "model_id": _SERIALIZER.url("model_id", model_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_models_edit_documentation_request(
+    model_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop(
+        "content_type", _headers.pop("Content-Type", None)
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/models/{model_id}/documentation"
+    path_format_arguments = {
+        "model_id": _SERIALIZER.url("model_id", model_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header(
+            "content_type", content_type, "str"
+        )
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
+
+
 def build_modules_label_request(module_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
     )
     accept = _headers.pop("Accept", "application/json")
@@ -1441,14 +1528,61 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="POST", url=_url, headers=_headers, **kwargs)
 
 
+def build_modules_documentation_request(module_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/modules/{module_id}/documentation"
+    path_format_arguments = {
+        "module_id": _SERIALIZER.url("module_id", module_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
+
+
+def build_modules_edit_documentation_request(
+    module_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+
+    content_type: Optional[str] = kwargs.pop(
+        "content_type", _headers.pop("Content-Type", None)
+    )
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = "/modules/{module_id}/documentation"
+    path_format_arguments = {
+        "module_id": _SERIALIZER.url("module_id", module_id, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct headers
+    if content_type is not None:
+        _headers["Content-Type"] = _SERIALIZER.header(
+            "content_type", content_type, "str"
+        )
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="PATCH", url=_url, headers=_headers, **kwargs)
+
+
 def build_reports_label_request(report_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
     content_type: Optional[str] = kwargs.pop(
         "content_type", _headers.pop("Content-Type", None)
     )
     accept = _headers.pop("Accept", "application/json")
@@ -1735,705 +1869,33 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="PUT", url=_url, headers=_headers, **kwargs)
 
 
-class AuditsOperations:  # pylint: disable=abstract-class-instantiated
-    """
-    .. warning::
-        **DO NOT** instantiate this class directly.
-
-        Instead, you should access the following operations through
-        :class:`~_generated.DyffV0API`'s
-        :attr:`audits` attribute.
-    """
-
-    def __init__(self, *args, **kwargs):
-        input_args = list(args)
-        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
-        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
-        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
-        self._deserialize = (
-            input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        )
-
-        raise_if_not_implemented(
-            self.__class__,
-            [
-                "upload",
-            ],
-        )
-
-    @overload
-    def label(
-        self,
-        audit_id: str,
-        body: JSON,
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any,
-    ) -> Union[Any, JSON]:
-        # pylint: disable=line-too-long
-        """Update labels for an existing Audit.
-
-        Update labels for an existing Audit.
-
-        :param audit_id: Required.
-        :type audit_id: str
-        :param body: Required.
-        :type body: JSON
-        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: any or JSON object
-        :rtype: any or JSON
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # JSON input template you can fill out and use as your body input.
-                body = {
-                    "labels": {
-                        "str": "str"  # Optional. A set of key-value labels for the resource.
-                          Used to specify identifying attributes of resources that are meaningful to
-                          users but do not imply semantics in the dyff system.  The keys are DNS labels
-                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
-                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
-                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
-                          follow the kubernetes label conventions closely. See:
-                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
-                }
-
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-
-    @overload
-    def label(
-        self,
-        audit_id: str,
-        body: IO[bytes],
-        *,
-        content_type: str = "application/json",
-        **kwargs: Any,
-    ) -> Union[Any, JSON]:
-        """Update labels for an existing Audit.
-
-        Update labels for an existing Audit.
-
-        :param audit_id: Required.
-        :type audit_id: str
-        :param body: Required.
-        :type body: IO[bytes]
-        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
-         Default value is "application/json".
-        :paramtype content_type: str
-        :return: any or JSON object
-        :rtype: any or JSON
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-
-    @distributed_trace
-    def label(
-        self, audit_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
-    ) -> Union[Any, JSON]:
-        # pylint: disable=line-too-long
-        """Update labels for an existing Audit.
-
-        Update labels for an existing Audit.
-
-        :param audit_id: Required.
-        :type audit_id: str
-        :param body: Is either a JSON type or a IO[bytes] type. Required.
-        :type body: JSON or IO[bytes]
-        :return: any or JSON object
-        :rtype: any or JSON
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # JSON input template you can fill out and use as your body input.
-                body = {
-                    "labels": {
-                        "str": "str"  # Optional. A set of key-value labels for the resource.
-                          Used to specify identifying attributes of resources that are meaningful to
-                          users but do not imply semantics in the dyff system.  The keys are DNS labels
-                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
-                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
-                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
-                          follow the kubernetes label conventions closely. See:
-                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    }
-                }
-
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-        error_map: MutableMapping[int, Type[HttpResponseError]] = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = kwargs.pop("params", {}) or {}
-
-        content_type: Optional[str] = kwargs.pop(
-            "content_type", _headers.pop("Content-Type", None)
-        )
-        cls: ClsType[Union[Any, JSON]] = kwargs.pop("cls", None)
-
-        content_type = content_type or "application/json"
-        _json = None
-        _content = None
-        if isinstance(body, (IOBase, bytes)):
-            _content = body
-        else:
-            _json = body
-
-        _request = build_audits_label_request(
-            audit_id=audit_id,
-            content_type=content_type,
-            json=_json,
-            content=_content,
-            headers=_headers,
-            params=_params,
-        )
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = (
-            self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 422]:
-            if _stream:
-                response.read()  # Load the body in memory and close the socket
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
-
-        if response.status_code == 200:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if response.status_code == 422:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if cls:
-            return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
-
-        return cast(Union[Any, JSON], deserialized)  # type: ignore
-
-    @distributed_trace
-    def query(
-        self,
-        *,
-        id: Optional[str] = None,
-        account: Optional[str] = None,
-        status: Optional[str] = None,
-        reason: Optional[str] = None,
-        labels: Optional[str] = None,
-        name: Optional[str] = None,
-        **kwargs: Any,
-    ) -> Union[List[JSON], JSON]:
-        # pylint: disable=line-too-long
-        """Get all Audits matching a query.
-
-        Get all Audits matching a query. The query is a set of equality
-        constraints specified as key-value pairs.
-
-        :keyword id: Default value is None.
-        :paramtype id: str
-        :keyword account: Default value is None.
-        :paramtype account: str
-        :keyword status: Default value is None.
-        :paramtype status: str
-        :keyword reason: Default value is None.
-        :paramtype reason: str
-        :keyword labels: Default value is None.
-        :paramtype labels: str
-        :keyword name: Default value is None.
-        :paramtype name: str
-        :return: list of JSON object or JSON object
-        :rtype: list[JSON] or JSON
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # response body for status code(s): 200
-                response == [
-                    {
-                        "account": "str",  # Account that owns the entity. Required.
-                        "auditProcedure": "str",  # The AuditProcedure to run. Required.
-                        "id": "str",  # Unique identifier of the entity. Required.
-                        "inferenceService": "str",  # The InferenceService to audit.
-                          Required.
-                        "annotations": [
-                            {
-                                "key": "str",  # The annotation key. A DNS label with
-                                  an optional DNS domain prefix. For example: 'my-key',
-                                  'your.com/key_0'. Names prefixed with 'dyff.io/',
-                                  'subdomain.dyff.io/', etc. are reserved.  See
-                                  https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
-                                  for detailed naming rules. Required.
-                                "value": "str"  # The annotation value. An arbitrary
-                                  string. Required.
-                            }
-                        ],
-                        "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation
-                          time (assigned by system).
-                        "kind": "Audit",  # Optional. Default value is "Audit". Kind. "Audit"
-                        "labels": {
-                            "str": "str"  # Optional. A set of key-value labels for the
-                              resource. Used to specify identifying attributes of resources that are
-                              meaningful to users but do not imply semantics in the dyff system.  The
-                              keys are DNS labels with an optional DNS domain prefix. For example:
-                              'my-key', 'your.com/key_0'. Keys prefixed with 'dyff.io/',
-                              'subdomain.dyff.io/', etc. are reserved.  The label values are
-                              alphanumeric characters separated by '.', '-', or '_'.  We follow the
-                              kubernetes label conventions closely. See:
-                              https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                        },
-                        "reason": "str",  # Optional. Reason for current status (assigned by
-                          system).
-                        "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
-                          schema version. "0.1"
-                        "status": "str"  # Optional. Top-level resource status (assigned by
-                          system).
-                    }
-                ]
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-        error_map: MutableMapping[int, Type[HttpResponseError]] = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = kwargs.pop("params", {}) or {}
-
-        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
-
-        _request = build_audits_query_request(
-            id=id,
-            account=account,
-            status=status,
-            reason=reason,
-            labels=labels,
-            name=name,
-            headers=_headers,
-            params=_params,
-        )
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = (
-            self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 422]:
-            if _stream:
-                response.read()  # Load the body in memory and close the socket
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
-
-        if response.status_code == 200:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if response.status_code == 422:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if cls:
-            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
-
-        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
-
-    @distributed_trace
-    def get(self, audit_id: str, **kwargs: Any) -> JSON:
-        # pylint: disable=line-too-long
-        """Get an Audit by its key.
-
-        Get an Audit by its key. Raises a 404 error if no entity exists with that key.
-
-        :param audit_id: Required.
-        :type audit_id: str
-        :return: JSON object
-        :rtype: JSON
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # response body for status code(s): 200
-                response == {
-                    "account": "str",  # Account that owns the entity. Required.
-                    "auditProcedure": "str",  # The AuditProcedure to run. Required.
-                    "id": "str",  # Unique identifier of the entity. Required.
-                    "inferenceService": "str",  # The InferenceService to audit. Required.
-                    "annotations": [
-                        {
-                            "key": "str",  # The annotation key. A DNS label with an
-                              optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
-                              Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
-                              See
-                              https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
-                              for detailed naming rules. Required.
-                            "value": "str"  # The annotation value. An arbitrary string.
-                              Required.
-                        }
-                    ],
-                    "creationTime": "2020-02-20 00:00:00",  # Optional. Resource creation time
-                      (assigned by system).
-                    "kind": "Audit",  # Optional. Default value is "Audit". Kind. "Audit"
-                    "labels": {
-                        "str": "str"  # Optional. A set of key-value labels for the resource.
-                          Used to specify identifying attributes of resources that are meaningful to
-                          users but do not imply semantics in the dyff system.  The keys are DNS labels
-                          with an optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
-                          Keys prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.  The
-                          label values are alphanumeric characters separated by '.', '-', or '_'.  We
-                          follow the kubernetes label conventions closely. See:
-                          https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
-                    },
-                    "reason": "str",  # Optional. Reason for current status (assigned by system).
-                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
-                      version. "0.1"
-                    "status": "str"  # Optional. Top-level resource status (assigned by system).
-                }
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-        error_map: MutableMapping[int, Type[HttpResponseError]] = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = kwargs.pop("params", {}) or {}
-
-        cls: ClsType[JSON] = kwargs.pop("cls", None)
-
-        _request = build_audits_get_request(
-            audit_id=audit_id,
-            headers=_headers,
-            params=_params,
-        )
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = (
-            self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 422]:
-            if _stream:
-                response.read()  # Load the body in memory and close the socket
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
-
-        if response.status_code == 200:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if response.status_code == 422:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
-
-        return cast(JSON, deserialized)  # type: ignore
-
-    @distributed_trace
-    def delete(self, audit_id: str, **kwargs: Any) -> JSON:
-        """Mark an Audit for deletion.
-
-        Mark an Audit for deletion.
-
-        :param audit_id: Required.
-        :type audit_id: str
-        :return: JSON object
-        :rtype: JSON
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # response body for status code(s): 200
-                response == {
-                    "reason": "str",  # Optional. Reason for current status (assigned by system).
-                    "status": "str"  # Optional. Top-level resource status (assigned by system).
-                }
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-        error_map: MutableMapping[int, Type[HttpResponseError]] = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = kwargs.pop("params", {}) or {}
-
-        cls: ClsType[JSON] = kwargs.pop("cls", None)
-
-        _request = build_audits_delete_request(
-            audit_id=audit_id,
-            headers=_headers,
-            params=_params,
-        )
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = False
-        pipeline_response: PipelineResponse = (
-            self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-        )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 422]:
-            if _stream:
-                response.read()  # Load the body in memory and close the socket
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
-
-        if response.status_code == 200:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if response.status_code == 422:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-
-        if cls:
-            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
-
-        return cast(JSON, deserialized)  # type: ignore
-
-
-class AuditproceduresOperations:
-    """
-    .. warning::
-        **DO NOT** instantiate this class directly.
-
-        Instead, you should access the following operations through
-        :class:`~_generated.DyffV0API`'s
-        :attr:`auditprocedures` attribute.
-    """
-
-    def __init__(self, *args, **kwargs):
-        input_args = list(args)
-        self._client = input_args.pop(0) if input_args else kwargs.pop("client")
-        self._config = input_args.pop(0) if input_args else kwargs.pop("config")
-        self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
-        self._deserialize = (
-            input_args.pop(0) if input_args else kwargs.pop("deserializer")
-        )
-
-    @distributed_trace
-    def download(self, path: str, **kwargs: Any) -> Union[Iterator[bytes], JSON]:
-        """Download the source code of an AuditProcedure.
-
-        Download the source code of an AuditProcedure.
-
-        :param path: Required.
-        :type path: str
-        :return: Iterator[bytes] or JSON object or None
-        :rtype: Iterator[bytes] or JSON or None
-        :raises ~azure.core.exceptions.HttpResponseError:
-
-        Example:
-            .. code-block:: python
-
-                # response body for status code(s): 422
-                response == {
-                    "detail": [
-                        {
-                            "loc": [
-                                {}
-                            ],
-                            "msg": "str",  # Message. Required.
-                            "type": "str"  # Error Type. Required.
-                        }
-                    ]
-                }
-        """
-        error_map: MutableMapping[int, Type[HttpResponseError]] = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = kwargs.pop("headers", {}) or {}
-        _params = kwargs.pop("params", {}) or {}
-
-        cls: ClsType[Union[Iterator[bytes], JSON]] = kwargs.pop("cls", None)
-
-        _request = build_auditprocedures_download_request(
-            path=path,
-            headers=_headers,
-            params=_params,
-        )
-        _request.url = self._client.format_url(_request.url)
-
-        _stream = True
-        pipeline_response: PipelineResponse = (
-            self._client._pipeline.run(  # pylint: disable=protected-access
-                _request, stream=_stream, **kwargs
-            )
-        )
-
-        response = pipeline_response.http_response
+def build_safetycases_downlinks_request(
+    safetycase_id: str, **kwargs: Any
+) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
 
-        if response.status_code not in [200, 404, 422]:
-            if _stream:
-                response.read()  # Load the body in memory and close the socket
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
+    accept = _headers.pop("Accept", "application/json")
 
-        deserialized = None
-        if response.status_code == 200:
-            deserialized = response.iter_bytes()
+    # Construct URL
+    _url = "/safetycases/{safetycase_id}/downlinks"
+    path_format_arguments = {
+        "safetycase_id": _SERIALIZER.url("safetycase_id", safetycase_id, "str"),
+    }
 
-        if response.status_code == 422:
-            deserialized = response.iter_bytes()
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
 
-        if cls:
-            return cls(pipeline_response, deserialized, {})  # type: ignore
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
-        return deserialized  # type: ignore
+    return HttpRequest(method="GET", url=_url, headers=_headers, **kwargs)
 
 
 class DatasetsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
@@ -2702,20 +2164,21 @@
 
                 # response body for status code(s): 200
                 response == [
                     {
                         "account": "str",  # Account that owns the entity. Required.
                         "artifacts": [
                             {
+                                "path": "str",  # The relative path of the artifact
+                                  within the tree. Required.
                                 "digest": {
-                                    "md5": "str"  # Optional. Md5.
+                                    "md5": "str"  # Optional. md5 digest of
+                                      artifact data.
                                 },
-                                "kind": "str",  # The kind of artifact. Required.
-                                "path": "str"  # The relative path of the artifact
-                                  within the dataset. Required.
+                                "kind": "str"  # Optional. The kind of artifact.
                             }
                         ],
                         "id": "str",  # Unique identifier of the entity. Required.
                         "name": "str",  # The name of the Dataset. Required.
                         "schema": {
                             "arrowSchema": "str",  # The schema in Arrow format, encoded
                               with dyff.schema.arrow.encode_schema(). This is required, but can be
@@ -2893,20 +2356,21 @@
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "name": "str",  # The name of the Dataset. Required.
                     "schema": {
                         "arrowSchema": "str",  # The schema in Arrow format, encoded with
                           dyff.schema.arrow.encode_schema(). This is required, but can be populated
                           from a DyffDataSchema. Required.
@@ -2956,20 +2420,21 @@
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Dataset. Required.
                     "schema": {
                         "arrowSchema": "str",  # The schema in Arrow format, encoded with
                           dyff.schema.arrow.encode_schema(). This is required, but can be populated
@@ -3081,20 +2546,21 @@
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Dataset. Required.
                     "schema": {
                         "arrowSchema": "str",  # The schema in Arrow format, encoded with
                           dyff.schema.arrow.encode_schema(). This is required, but can be populated
@@ -3201,20 +2667,21 @@
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "name": "str",  # The name of the Dataset. Required.
                     "schema": {
                         "arrowSchema": "str",  # The schema in Arrow format, encoded with
                           dyff.schema.arrow.encode_schema(). This is required, but can be populated
                           from a DyffDataSchema. Required.
@@ -3264,20 +2731,21 @@
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Dataset. Required.
                     "schema": {
                         "arrowSchema": "str",  # The schema in Arrow format, encoded with
                           dyff.schema.arrow.encode_schema(). This is required, but can be populated
@@ -3450,20 +2918,21 @@
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Dataset. Required.
                     "schema": {
                         "arrowSchema": "str",  # The schema in Arrow format, encoded with
                           dyff.schema.arrow.encode_schema(). This is required, but can be populated
@@ -4021,14 +3490,348 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
+    @distributed_trace
+    def documentation(self, dataset_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get the documentation associated with a Dataset.
+
+        Get the documentation associated with a Dataset. Raises a 404
+        error if no entity exists with that key.
+
+        :param dataset_id: Required.
+        :type dataset_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_datasets_documentation_request(
+            dataset_id=dataset_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @overload
+    def edit_documentation(
+        self,
+        dataset_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Dataset.
+
+        Edit the documentation associated with a Dataset. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param dataset_id: Required.
+        :type dataset_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    def edit_documentation(
+        self,
+        dataset_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Dataset.
+
+        Edit the documentation associated with a Dataset. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param dataset_id: Required.
+        :type dataset_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace
+    def edit_documentation(
+        self, dataset_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Dataset.
+
+        Edit the documentation associated with a Dataset. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param dataset_id: Required.
+        :type dataset_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_datasets_edit_documentation_request(
+            dataset_id=dataset_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
 
 class EvaluationsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -7472,14 +7275,348 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
+    @distributed_trace
+    def documentation(self, service_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get the documentation associated with an InferenceService.
+
+        Get the documentation associated with an InferenceService. Raises a 404
+        error if no entity exists with that key.
+
+        :param service_id: Required.
+        :type service_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_inferenceservices_documentation_request(
+            service_id=service_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @overload
+    def edit_documentation(
+        self,
+        service_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with an InferenceService.
+
+        Edit the documentation associated with an InferenceService. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param service_id: Required.
+        :type service_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    def edit_documentation(
+        self,
+        service_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with an InferenceService.
+
+        Edit the documentation associated with an InferenceService. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param service_id: Required.
+        :type service_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace
+    def edit_documentation(
+        self, service_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with an InferenceService.
+
+        Edit the documentation associated with an InferenceService. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param service_id: Required.
+        :type service_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_inferenceservices_edit_documentation_request(
+            service_id=service_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
 
 class InferencesessionsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -9920,20 +10057,14 @@
                                 ],
                                 "schemaVersion": "0.1"  # Optional. Default value is
                                   "0.1". The dyff schema version. "0.1"
                             },
                             "jsonSchema": {}  # Optional. The schema in JSON Schema
                               format.
                         },
-                        "scope": {
-                            "dataset": "str",  # Optional. Dataset.
-                            "evaluation": "str",  # Optional. Evaluation.
-                            "inferenceService": "str",  # Optional. Inferenceservice.
-                            "model": "str"  # Optional. Model.
-                        },
                         "annotations": [
                             {
                                 "key": "str",  # The annotation key. A DNS label with
                                   an optional DNS domain prefix. For example: 'my-key',
                                   'your.com/key_0'. Names prefixed with 'dyff.io/',
                                   'subdomain.dyff.io/', etc. are reserved.  See
                                   https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -9976,14 +10107,24 @@
                               kubernetes label conventions closely. See:
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                         },
                         "reason": "str",  # Optional. Reason for current status (assigned by
                           system).
                         "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
                           schema version. "0.1"
+                        "scope": {
+                            "dataset": "str",  # Optional. The Dataset to which the
+                              analysis applies.
+                            "evaluation": "str",  # Optional. The Evaluation to which the
+                              analysis applies.
+                            "inferenceService": "str",  # Optional. The InferenceService
+                              to which the analysis applies.
+                            "model": "str"  # Optional. The Model to which the analysis
+                              applies.
+                        },
                         "status": "str"  # Optional. Top-level resource status (assigned by
                           system).
                     }
                 ]
                 # response body for status code(s): 422
                 response == {
                     "detail": [
@@ -10080,20 +10221,14 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "method": "str",  # Method ID. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "arguments": [
                         {
                             "keyword": "str",  # The 'keyword' of the corresponding
                               ModelParameter. Required.
                             "value": "str"  # The value of of the argument. Always a
                               string; implementations are responsible for parsing. Required.
                         }
@@ -10102,16 +10237,25 @@
                         {
                             "entity": "str",  # The ID of the entity whose data should be
                               made available as 'keyword'. Required.
                             "keyword": "str"  # The 'keyword' specified for this input in
                               the MethodSpec. Required.
                         }
                     ],
-                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    }
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "id": "str",  # Unique identifier of the entity. Required.
                     "level": "str",  # Measurement level. Required. Known values are: "Dataset"
@@ -10212,20 +10356,14 @@
                                   schema is the composition of these component schemas. Required.
                             ],
                             "schemaVersion": "0.1"  # Optional. Default value is "0.1".
                               The dyff schema version. "0.1"
                         },
                         "jsonSchema": {}  # Optional. The schema in JSON Schema format.
                     },
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -10265,14 +10403,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -10408,20 +10555,14 @@
                                   schema is the composition of these component schemas. Required.
                             ],
                             "schemaVersion": "0.1"  # Optional. Default value is "0.1".
                               The dyff schema version. "0.1"
                         },
                         "jsonSchema": {}  # Optional. The schema in JSON Schema format.
                     },
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -10461,14 +10602,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -10497,20 +10647,14 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "method": "str",  # Method ID. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "arguments": [
                         {
                             "keyword": "str",  # The 'keyword' of the corresponding
                               ModelParameter. Required.
                             "value": "str"  # The value of of the argument. Always a
                               string; implementations are responsible for parsing. Required.
                         }
@@ -10519,16 +10663,25 @@
                         {
                             "entity": "str",  # The ID of the entity whose data should be
                               made available as 'keyword'. Required.
                             "keyword": "str"  # The 'keyword' specified for this input in
                               the MethodSpec. Required.
                         }
                     ],
-                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    }
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "id": "str",  # Unique identifier of the entity. Required.
                     "level": "str",  # Measurement level. Required. Known values are: "Dataset"
@@ -10629,20 +10782,14 @@
                                   schema is the composition of these component schemas. Required.
                             ],
                             "schemaVersion": "0.1"  # Optional. Default value is "0.1".
                               The dyff schema version. "0.1"
                         },
                         "jsonSchema": {}  # Optional. The schema in JSON Schema format.
                     },
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -10682,14 +10829,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -10886,20 +11042,14 @@
                                   schema is the composition of these component schemas. Required.
                             ],
                             "schemaVersion": "0.1"  # Optional. Default value is "0.1".
                               The dyff schema version. "0.1"
                         },
                         "jsonSchema": {}  # Optional. The schema in JSON Schema format.
                     },
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -10939,14 +11089,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -11095,14 +11254,120 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
+    @distributed_trace
+    def downlinks(self, measurement_id: str, **kwargs: Any) -> Union[List[JSON], JSON]:
+        """Get a list of signed GET URLs from which measurement artifacts can be
+        downloaded.
+
+        Get a list of signed GET URLs from which measurement artifacts can be downloaded.
+
+        :param measurement_id: Required.
+        :type measurement_id: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "artifact": {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
+                            "digest": {
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
+                            },
+                            "kind": "str"  # Optional. The kind of artifact.
+                        },
+                        "signedURL": {
+                            "method": "str",  # The HTTP method applicable to the URL.
+                              Required.
+                            "url": "str",  # The signed URL. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Mandatory headers that must
+                                  be passed with the request.
+                            }
+                        }
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_measurements_downlinks_request(
+            measurement_id=measurement_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
+
 
 class MethodsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -12521,14 +12786,348 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
+    @distributed_trace
+    def documentation(self, method_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get the documentation associated with a Method.
+
+        Get the documentation associated with a Method. Raises a 404
+        error if no entity exists with that key.
+
+        :param method_id: Required.
+        :type method_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_methods_documentation_request(
+            method_id=method_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @overload
+    def edit_documentation(
+        self,
+        method_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Method.
+
+        Edit the documentation associated with a Method. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param method_id: Required.
+        :type method_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    def edit_documentation(
+        self,
+        method_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Method.
+
+        Edit the documentation associated with a Method. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param method_id: Required.
+        :type method_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace
+    def edit_documentation(
+        self, method_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Method.
+
+        Edit the documentation associated with a Method. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param method_id: Required.
+        :type method_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_methods_edit_documentation_request(
+            method_id=method_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
 
 class ModelsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -13815,14 +14414,348 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
 
+    @distributed_trace
+    def documentation(self, model_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get the documentation associated with a Model.
+
+        Get the documentation associated with a Model. Raises a 404
+        error if no entity exists with that key.
+
+        :param model_id: Required.
+        :type model_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_models_documentation_request(
+            model_id=model_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @overload
+    def edit_documentation(
+        self,
+        model_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Model.
+
+        Edit the documentation associated with a Model. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param model_id: Required.
+        :type model_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    def edit_documentation(
+        self,
+        model_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Model.
+
+        Edit the documentation associated with a Model. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param model_id: Required.
+        :type model_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace
+    def edit_documentation(
+        self, model_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Model.
+
+        Edit the documentation associated with a Model. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param model_id: Required.
+        :type model_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_models_edit_documentation_request(
+            model_id=model_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
 
 class ModulesOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -14090,20 +15023,21 @@
 
                 # response body for status code(s): 200
                 response == [
                     {
                         "account": "str",  # Account that owns the entity. Required.
                         "artifacts": [
                             {
+                                "path": "str",  # The relative path of the artifact
+                                  within the tree. Required.
                                 "digest": {
-                                    "md5": "str"  # Optional. Md5.
+                                    "md5": "str"  # Optional. md5 digest of
+                                      artifact data.
                                 },
-                                "kind": "str",  # The kind of artifact. Required.
-                                "path": "str"  # The relative path of the artifact
-                                  within the dataset. Required.
+                                "kind": "str"  # Optional. The kind of artifact.
                             }
                         ],
                         "id": "str",  # Unique identifier of the entity. Required.
                         "name": "str",  # The name of the Module. Required.
                         "annotations": [
                             {
                                 "key": "str",  # The annotation key. A DNS label with
@@ -14233,38 +15167,40 @@
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "name": "str",  # The name of the Module. Required.
                     "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Module. Required.
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
@@ -14331,20 +15267,21 @@
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Module. Required.
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
@@ -14406,38 +15343,40 @@
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "name": "str",  # The name of the Module. Required.
                     "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
                       version. "0.1"
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Module. Required.
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
@@ -14565,20 +15504,21 @@
             .. code-block:: python
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "artifacts": [
                         {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
                             "digest": {
-                                "md5": "str"  # Optional. Md5.
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
                             },
-                            "kind": "str",  # The kind of artifact. Required.
-                            "path": "str"  # The relative path of the artifact within the
-                              dataset. Required.
+                            "kind": "str"  # Optional. The kind of artifact.
                         }
                     ],
                     "id": "str",  # Unique identifier of the entity. Required.
                     "name": "str",  # The name of the Module. Required.
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
@@ -14935,14 +15875,348 @@
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(Union[Any, JSON], deserialized), {})  # type: ignore
 
         return cast(Union[Any, JSON], deserialized)  # type: ignore
 
+    @distributed_trace
+    def documentation(self, module_id: str, **kwargs: Any) -> JSON:
+        # pylint: disable=line-too-long
+        """Get the documentation associated with a Module.
+
+        Get the documentation associated with a Module. Raises a 404
+        error if no entity exists with that key.
+
+        :param module_id: Required.
+        :type module_id: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        _request = build_modules_documentation_request(
+            module_id=module_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
+    @overload
+    def edit_documentation(
+        self,
+        module_id: str,
+        body: JSON,
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Module.
+
+        Edit the documentation associated with a Module. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param module_id: Required.
+        :type module_id: str
+        :param body: Required.
+        :type body: JSON
+        :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @overload
+    def edit_documentation(
+        self,
+        module_id: str,
+        body: IO[bytes],
+        *,
+        content_type: str = "application/json",
+        **kwargs: Any,
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Module.
+
+        Edit the documentation associated with a Module. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param module_id: Required.
+        :type module_id: str
+        :param body: Required.
+        :type body: IO[bytes]
+        :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
+         Default value is "application/json".
+        :paramtype content_type: str
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+
+    @distributed_trace
+    def edit_documentation(
+        self, module_id: str, body: Union[JSON, IO[bytes]], **kwargs: Any
+    ) -> JSON:
+        # pylint: disable=line-too-long
+        """Edit the documentation associated with a Module.
+
+        Edit the documentation associated with a Module. Raises a 404
+        error if no entity exists with that key. Returns the modified Documentation.
+
+        :param module_id: Required.
+        :type module_id: str
+        :param body: Is either a JSON type or a IO[bytes] type. Required.
+        :type body: JSON or IO[bytes]
+        :return: JSON object
+        :rtype: JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # JSON input template you can fill out and use as your body input.
+                body = {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+
+                # response body for status code(s): 200
+                response == {
+                    "fullPage": "str",  # Optional. Long-form documentation. Interpreted as
+                      Markdown. There are no length constraints, but be reasonable.
+                    "summary": "str",  # Optional. A brief summary, suitable for display in small
+                      UI elements. Interpreted as Markdown. Excessively long summaries may be truncated
+                      in the UI, especially on small displays.
+                    "title": "str"  # Optional. A short plain string suitable as a title or
+                      "headline".
+                }
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+        _params = kwargs.pop("params", {}) or {}
+
+        content_type: Optional[str] = kwargs.pop(
+            "content_type", _headers.pop("Content-Type", None)
+        )
+        cls: ClsType[JSON] = kwargs.pop("cls", None)
+
+        content_type = content_type or "application/json"
+        _json = None
+        _content = None
+        if isinstance(body, (IOBase, bytes)):
+            _content = body
+        else:
+            _json = body
+
+        _request = build_modules_edit_documentation_request(
+            module_id=module_id,
+            content_type=content_type,
+            json=_json,
+            content=_content,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
+
+        return cast(JSON, deserialized)  # type: ignore
+
 
 class ReportsOperations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
@@ -16645,20 +17919,14 @@
                                       implementation. Required.
                                     "description": "str"  # Optional. Long-form
                                       description, interpreted as Markdown.
                                 }
                             ]
                         },
                         "name": "str",  # Descriptive name of the SafetyCase. Required.
-                        "scope": {
-                            "dataset": "str",  # Optional. Dataset.
-                            "evaluation": "str",  # Optional. Evaluation.
-                            "inferenceService": "str",  # Optional. Inferenceservice.
-                            "model": "str"  # Optional. Model.
-                        },
                         "annotations": [
                             {
                                 "key": "str",  # The annotation key. A DNS label with
                                   an optional DNS domain prefix. For example: 'my-key',
                                   'your.com/key_0'. Names prefixed with 'dyff.io/',
                                   'subdomain.dyff.io/', etc. are reserved.  See
                                   https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -16701,14 +17969,24 @@
                               kubernetes label conventions closely. See:
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                         },
                         "reason": "str",  # Optional. Reason for current status (assigned by
                           system).
                         "schemaVersion": "0.1",  # Optional. Default value is "0.1". The
                           schema version. "0.1"
+                        "scope": {
+                            "dataset": "str",  # Optional. The Dataset to which the
+                              analysis applies.
+                            "evaluation": "str",  # Optional. The Evaluation to which the
+                              analysis applies.
+                            "inferenceService": "str",  # Optional. The InferenceService
+                              to which the analysis applies.
+                            "model": "str"  # Optional. The Model to which the analysis
+                              applies.
+                        },
                         "status": "str"  # Optional. Top-level resource status (assigned by
                           system).
                     }
                 ]
                 # response body for status code(s): 422
                 response == {
                     "detail": [
@@ -16805,20 +18083,14 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "method": "str",  # Method ID. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "arguments": [
                         {
                             "keyword": "str",  # The 'keyword' of the corresponding
                               ModelParameter. Required.
                             "value": "str"  # The value of of the argument. Always a
                               string; implementations are responsible for parsing. Required.
                         }
@@ -16827,16 +18099,25 @@
                         {
                             "entity": "str",  # The ID of the entity whose data should be
                               made available as 'keyword'. Required.
                             "keyword": "str"  # The 'keyword' specified for this input in
                               the MethodSpec. Required.
                         }
                     ],
-                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    }
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "id": "str",  # Unique identifier of the entity. Required.
                     "method": {
@@ -16921,20 +18202,14 @@
                                   'keyword' in the context of the method implementation. Required.
                                 "description": "str"  # Optional. Long-form
                                   description, interpreted as Markdown.
                             }
                         ]
                     },
                     "name": "str",  # Descriptive name of the SafetyCase. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -16974,14 +18249,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -17101,20 +18385,14 @@
                                   'keyword' in the context of the method implementation. Required.
                                 "description": "str"  # Optional. Long-form
                                   description, interpreted as Markdown.
                             }
                         ]
                     },
                     "name": "str",  # Descriptive name of the SafetyCase. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -17154,14 +18432,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -17190,20 +18477,14 @@
         Example:
             .. code-block:: python
 
                 # JSON input template you can fill out and use as your body input.
                 body = {
                     "account": "str",  # Account that owns the entity. Required.
                     "method": "str",  # Method ID. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "arguments": [
                         {
                             "keyword": "str",  # The 'keyword' of the corresponding
                               ModelParameter. Required.
                             "value": "str"  # The value of of the argument. Always a
                               string; implementations are responsible for parsing. Required.
                         }
@@ -17212,16 +18493,25 @@
                         {
                             "entity": "str",  # The ID of the entity whose data should be
                               made available as 'keyword'. Required.
                             "keyword": "str"  # The 'keyword' specified for this input in
                               the MethodSpec. Required.
                         }
                     ],
-                    "schemaVersion": "0.1"  # Optional. Default value is "0.1". The schema
+                    "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    }
                 }
 
                 # response body for status code(s): 200
                 response == {
                     "account": "str",  # Account that owns the entity. Required.
                     "id": "str",  # Unique identifier of the entity. Required.
                     "method": {
@@ -17306,20 +18596,14 @@
                                   'keyword' in the context of the method implementation. Required.
                                 "description": "str"  # Optional. Long-form
                                   description, interpreted as Markdown.
                             }
                         ]
                     },
                     "name": "str",  # Descriptive name of the SafetyCase. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -17359,14 +18643,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -17547,20 +18840,14 @@
                                   'keyword' in the context of the method implementation. Required.
                                 "description": "str"  # Optional. Long-form
                                   description, interpreted as Markdown.
                             }
                         ]
                     },
                     "name": "str",  # Descriptive name of the SafetyCase. Required.
-                    "scope": {
-                        "dataset": "str",  # Optional. Dataset.
-                        "evaluation": "str",  # Optional. Evaluation.
-                        "inferenceService": "str",  # Optional. Inferenceservice.
-                        "model": "str"  # Optional. Model.
-                    },
                     "annotations": [
                         {
                             "key": "str",  # The annotation key. A DNS label with an
                               optional DNS domain prefix. For example: 'my-key', 'your.com/key_0'.
                               Names prefixed with 'dyff.io/', 'subdomain.dyff.io/', etc. are reserved.
                               See
                               https://kubernetes.io/docs/concepts/overview/working-with-objects/annotations
@@ -17600,14 +18887,23 @@
                           label values are alphanumeric characters separated by '.', '-', or '_'.  We
                           follow the kubernetes label conventions closely. See:
                           https://kubernetes.io/docs/concepts/overview/working-with-objects/labels.
                     },
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "schemaVersion": "0.1",  # Optional. Default value is "0.1". The schema
                       version. "0.1"
+                    "scope": {
+                        "dataset": "str",  # Optional. The Dataset to which the analysis
+                          applies.
+                        "evaluation": "str",  # Optional. The Evaluation to which the
+                          analysis applies.
+                        "inferenceService": "str",  # Optional. The InferenceService to which
+                          the analysis applies.
+                        "model": "str"  # Optional. The Model to which the analysis applies.
+                    },
                     "status": "str"  # Optional. Top-level resource status (assigned by system).
                 }
                 # response body for status code(s): 422
                 response == {
                     "detail": [
                         {
                             "loc": [
@@ -17755,7 +19051,113 @@
             else:
                 deserialized = None
 
         if cls:
             return cls(pipeline_response, cast(JSON, deserialized), {})  # type: ignore
 
         return cast(JSON, deserialized)  # type: ignore
+
+    @distributed_trace
+    def downlinks(self, safetycase_id: str, **kwargs: Any) -> Union[List[JSON], JSON]:
+        """Get a list of signed GET URLs from which safety case artifacts can be
+        downloaded.
+
+        Get a list of signed GET URLs from which safety case artifacts can be downloaded.
+
+        :param safetycase_id: Required.
+        :type safetycase_id: str
+        :return: list of JSON object or JSON object
+        :rtype: list[JSON] or JSON
+        :raises ~azure.core.exceptions.HttpResponseError:
+
+        Example:
+            .. code-block:: python
+
+                # response body for status code(s): 200
+                response == [
+                    {
+                        "artifact": {
+                            "path": "str",  # The relative path of the artifact within
+                              the tree. Required.
+                            "digest": {
+                                "md5": "str"  # Optional. md5 digest of artifact
+                                  data.
+                            },
+                            "kind": "str"  # Optional. The kind of artifact.
+                        },
+                        "signedURL": {
+                            "method": "str",  # The HTTP method applicable to the URL.
+                              Required.
+                            "url": "str",  # The signed URL. Required.
+                            "headers": {
+                                "str": "str"  # Optional. Mandatory headers that must
+                                  be passed with the request.
+                            }
+                        }
+                    }
+                ]
+                # response body for status code(s): 422
+                response == {
+                    "detail": [
+                        {
+                            "loc": [
+                                {}
+                            ],
+                            "msg": "str",  # Message. Required.
+                            "type": "str"  # Error Type. Required.
+                        }
+                    ]
+                }
+        """
+        error_map: MutableMapping[int, Type[HttpResponseError]] = {
+            401: ClientAuthenticationError,
+            404: ResourceNotFoundError,
+            409: ResourceExistsError,
+            304: ResourceNotModifiedError,
+        }
+        error_map.update(kwargs.pop("error_map", {}) or {})
+
+        _headers = kwargs.pop("headers", {}) or {}
+        _params = kwargs.pop("params", {}) or {}
+
+        cls: ClsType[Union[List[JSON], JSON]] = kwargs.pop("cls", None)
+
+        _request = build_safetycases_downlinks_request(
+            safetycase_id=safetycase_id,
+            headers=_headers,
+            params=_params,
+        )
+        _request.url = self._client.format_url(_request.url)
+
+        _stream = False
+        pipeline_response: PipelineResponse = (
+            self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
+            )
+        )
+
+        response = pipeline_response.http_response
+
+        if response.status_code not in [200, 422]:
+            if _stream:
+                response.read()  # Load the body in memory and close the socket
+            map_error(
+                status_code=response.status_code, response=response, error_map=error_map
+            )
+            raise HttpResponseError(response=response)
+
+        if response.status_code == 200:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if response.status_code == 422:
+            if response.content:
+                deserialized = response.json()
+            else:
+                deserialized = None
+
+        if cls:
+            return cls(pipeline_response, cast(Union[List[JSON], JSON], deserialized), {})  # type: ignore
+
+        return cast(Union[List[JSON], JSON], deserialized)  # type: ignore
```

### Comparing `dyff_client-0.3.2/dyff/client/_generated/operations/_patch.py` & `dyff_client-0.4.2/dyff/client/_generated/operations/_patch.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,25 +7,17 @@
 # ------------------------------------
 """Customize generated code here.
 
 Follow our quickstart for examples: https://aka.ms/azsdk/python/dpcodegen/python/customize
 """
 from typing import List
 
-from ._operations import AuditsOperations as _AuditsOperationsGenerated
-
-
-class AuditsOperations(_AuditsOperationsGenerated):
-    def upload(self, *args, **kwargs):
-        raise NotImplementedError()
-
-
-__all__: List[str] = [
-    "AuditsOperations"
-]  # Add all objects you want publicly available to users at this package level
+__all__: List[str] = (
+    []
+)  # Add all objects you want publicly available to users at this package level
 
 
 def patch_sdk():
     """Do not remove from this file.
 
     `patch_sdk` is a last resort escape hatch that allows you to do customizations
     you can't accomplish using the techniques described in
```

### Comparing `dyff_client-0.3.2/dyff/client/client.py` & `dyff_client-0.4.2/dyff/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,46 +5,38 @@
 from __future__ import annotations
 
 import json
 import pathlib
 import sys
 import time
 from io import BytesIO
-from typing import Any, BinaryIO, Callable, Optional, TypeVar
+from typing import Any, Callable, Optional, TypeVar
 from warnings import warn
 
 import httpx
 import pandas
 import pyarrow.dataset
 from azure.core.credentials import AccessToken, TokenCredential
 
 # We bring this into our namespace so that people can catch it without being
 # confused by having to import 'azure.core'
-from azure.core.exceptions import (
-    ClientAuthenticationError,
-    HttpResponseError,
-    ResourceExistsError,
-    ResourceNotFoundError,
-    ResourceNotModifiedError,
-    map_error,
-)
+from azure.core.exceptions import HttpResponseError
 from azure.core.pipeline import PipelineResponse
 from azure.core.pipeline.policies import BearerTokenCredentialPolicy
 from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
-from azure.core.utils import case_insensitive_dict
 
 from dyff.schema.adapters import Adapter, create_pipeline
 from dyff.schema.dataset import arrow, binary
 from dyff.schema.platform import (
     Artifact,
-    Audit,
     DataSchema,
     Dataset,
     Digest,
+    Documentation,
     DyffEntity,
     Evaluation,
     InferenceInterface,
     InferenceService,
     InferenceSession,
     InferenceSessionAndToken,
     Label,
@@ -56,36 +48,27 @@
     SafetyCase,
     Status,
     StorageSignedURL,
 )
 from dyff.schema.requests import (
     AnalysisCreateRequest,
     DatasetCreateRequest,
+    DocumentationEditRequest,
     EvaluationCreateRequest,
     InferenceServiceCreateRequest,
     InferenceSessionCreateRequest,
     LabelUpdateRequest,
     MethodCreateRequest,
     ModelCreateRequest,
     ModuleCreateRequest,
     ReportCreateRequest,
 )
 
 from ._generated import DyffV0API as RawClient
 from ._generated._serialization import Serializer
-
-# from ._generated.operations._operations import (
-#     AnalysesOperations as AnalysesOperationsGenerated,
-# )
-from ._generated.operations._operations import (
-    AuditproceduresOperations as AuditproceduresOperationsGenerated,
-)
-from ._generated.operations._operations import (
-    AuditsOperations as AuditsOperationsGenerated,
-)
 from ._generated.operations._operations import (
     DatasetsOperations as DatasetsOperationsGenerated,
 )
 from ._generated.operations._operations import (
     EvaluationsOperations as EvaluationsOperationsGenerated,
 )
 from ._generated.operations._operations import (
@@ -178,54 +161,14 @@
                     retries += 1
                 else:
                     raise
 
     return _impl
 
 
-def build_audits_upload_request(
-    audit_id: str, *, file: BinaryIO, **kwargs: Any
-) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-
-    # Note: Do not set the content type manually. Azure will figure out that
-    # it's multipart/form-data and generate the '; boundary=...' part.
-    content_type: Optional[str] = kwargs.pop(
-        "content_type", _headers.pop("Content-Type", None)
-    )
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = "/audits/{audit_id}/upload"
-    path_format_arguments = {
-        "audit_id": _SERIALIZER.url("audit_id", audit_id, "str"),
-    }
-
-    _url = _url.format(**path_format_arguments)
-
-    # Construct headers
-    if content_type is not None:
-        _headers["Content-Type"] = _SERIALIZER.header(
-            "content_type", content_type, "str"
-        )
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    # Note: The key is the name of the parameter in FastAPI
-    # It's not obvious from the documentation of HttpRequest, but the file has
-    # to be a file-like object. Even though HttpRequest will accept the file
-    # data instead, this will not get encoded/decoded correctly for FastAPI
-    # to work with it.
-    # See: azure.core.utils._pipeline_transport_rest_shared._format_data_helper()
-    # The error if you provide the data instead:
-    # {'detail': [{'loc': ['body', 'file'], 'msg': "Expected UploadFile, received: <class 'str'>", 'type': 'value_error'}]}
-    files = {"file": file}
-    # Note: The annotated type of 'files' might not be accurate
-    return HttpRequest(method="POST", url=_url, headers=_headers, files=files, **kwargs)  # type: ignore
-
-
 class InferenceSessionClient:
     """A client used for making inference requests to a running
     :class:`~dyff.schema.platform.InferenceSession`.
 
     .. note::
 
       Do not instantiate this class. Create an instance using
@@ -296,300 +239,14 @@
             response.read()
             json_response = once(response.json())
             if self._output_adapter is not None:
                 json_response = self._output_adapter(json_response)
         return list(json_response)
 
 
-# class AnalysesOperations:
-#     """Operations on :class:`~dyff.schema.platform.Analysis` entities.
-
-#     .. note::
-
-#       Do not instantiate this class. Access it through the
-#       ``.analyses`` attribute of :class:`~dyff.client.Client`.
-#     """
-
-#     def __init__(self, _raw_ops: AnalysesOperationsGenerated):
-#         self._raw_ops = _raw_ops
-
-#     def get(self, analysis_id: str) -> Analysis:
-#         """Get an Analysis by its key.
-
-#         :param analysis_id: The analysis id
-#         :type analysis_id: str
-#         :return: The Analysis with the given ID.
-#         """
-#         return Analysis.parse_obj(self._raw_ops.get(analysis_id))
-
-#     def delete(self, analysis_id: str) -> Status:
-#         """Mark an Analysis for deletion.
-
-#         :param analysis_id: The analysis id
-#         :type analysis_id: str
-#         :return: The resulting status of the entity
-#         :rtype: dyff.schema.platform.Status
-#         """
-#         return Status.parse_obj(self._raw_ops.delete(analysis_id))
-
-#     def query(
-#         self,
-#         *,
-#         id: Optional[str] = None,
-#         account: Optional[str] = None,
-#         status: Optional[str] = None,
-#         reason: Optional[str] = None,
-#         labels: Optional[dict[str, str]] = None,
-#         method: Optional[str] = None,
-#         method_name: Optional[str] = None,
-#         method_output_kind: Optional[str] = None,
-#     ) -> list[Analysis]:
-#         """Get all Analysis entities matching a query. The query is a set of equality constraints
-#         specified as key-value pairs.
-
-#         :keyword id: Default value is None.
-#         :paramtype id: str
-#         :keyword account: Default value is None.
-#         :paramtype account: str
-#         :keyword status: Default value is None.
-#         :paramtype status: str
-#         :keyword reason: Default value is None.
-#         :paramtype reason: str
-#         :keyword labels: Default value is None.
-#         :paramtype labels: dict[str, str]
-#         :keyword method: Default value is None.
-#         :paramtype method: str
-#         :keyword method_name: Default value is None.
-#         :paramtype method_name: str
-#         :keyword method_output_kind: Default value is None.
-#         :paramtype method_output_kind: str
-#         :return: list of Analysis entities matching the query
-#         :rtype: list[Analysis]
-#         :raises ~azure.core.exceptions.HttpResponseError:
-#         """
-#         return [
-#             Analysis.parse_obj(obj)
-#             for obj in self._raw_ops.query(
-#                 id=id,
-#                 account=account,
-#                 status=status,
-#                 reason=reason,
-#                 labels=_encode_labels(labels),
-#                 method=method,
-#                 method_name=method_name,
-#                 method_output_kind=method_output_kind,
-#             )
-#         ]
-
-#     def label(self, analysis_id: str, labels: dict[str, Optional[str]]) -> None:
-#         """Label the specified Analysis with key-value pairs (stored in the ``.labels``
-#         field of the resource).
-
-#         Providing ``None`` for the value deletes the label.
-
-#         See :class:`~dyff.schema.platform.Label` for a description of the
-#         constraints on label keys and values.
-
-#         :param analysis_id: The ID of the Analysis to label.
-#         :type analysis_id: str
-#         :param labels: The label keys and values.
-#         :type labels: dict[str, Optional[str]]
-#         """
-#         if not labels:
-#             return
-#         labels = LabelUpdateRequest(labels=labels).dict()
-#         self._raw_ops.label(analysis_id, labels)
-
-#     def create(self, analysis_request: AnalysisCreateRequest) -> Analysis:
-#         """Create an Analysis.
-
-#         .. note::
-#             This operation will incur compute costs.
-
-#         :param analysis_request: The Analysis specification.
-#         :type analysis_request: AnalysisCreateRequest
-#         :return: A full Analysis entity with .id and other properties set.
-#         """
-#         return Analysis.parse_obj(self._raw_ops.create(analysis_request.dict()))
-
-
-class AuditsOperations:
-    """Operations on :class:`~dyff.schema.platform.Audit` entities.
-
-    .. note::
-
-      Do not instantiate this class. Access it through the
-      ``.audits`` attribute of :class:`~dyff.client.Client`.
-    """
-
-    def __init__(self, _raw_ops: AuditsOperationsGenerated):
-        self._raw_ops = _raw_ops
-
-    def get(self, audit_id: str) -> Audit:
-        """Get an Audit by its key.
-
-        :param audit_id: The audit id
-        :type audit_id: str
-        :return: The Audit with the given key.
-        """
-        return Audit.parse_obj(self._raw_ops.get(audit_id))
-
-    def delete(self, audit_id: str) -> Status:
-        """Mark an Audit for deletion.
-
-        :param audit_id: The audit key
-        :type audit_id: str
-        :return: The resulting status of the entity
-        :rtype: dyff.schema.platform.Status
-        """
-        return Status.parse_obj(self._raw_ops.delete(audit_id))
-
-    def query(
-        self,
-        *,
-        id: Optional[str] = None,
-        account: Optional[str] = None,
-        status: Optional[str] = None,
-        reason: Optional[str] = None,
-        labels: Optional[dict[str, str]] = None,
-        name: Optional[str] = None,
-    ) -> list[Audit]:
-        """Get all Audits matching a query. The query is a set of equality constraints
-        specified as key-value pairs.
-
-        :keyword id:
-        :paramtype id: str
-        :keyword account:
-        :paramtype account: str
-        :keyword status:
-        :paramtype status: str
-        :keyword reason:
-        :paramtype reason: str
-        :keyword labels:
-        :paramtype labels: dict[str, str]
-        :keyword name: Default value is None.
-        :paramtype name: str
-        :return: list of ``Audit`` resources satisfying the query.
-        :rtype: list[Audit]
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        return [
-            Audit.parse_obj(obj)
-            for obj in self._raw_ops.query(
-                id=id,
-                account=account,
-                status=status,
-                reason=reason,
-                labels=_encode_labels(labels),
-                name=name,
-            )
-        ]
-
-    def label(self, audit_id: str, labels: dict[str, Optional[str]]) -> None:
-        """Label the specified Audit with key-value pairs (stored in the ``.labels``
-        field of the resource).
-
-        Providing ``None`` for the value deletes the label.
-
-        See :class:`~dyff.schema.platform.Label` for a description of the
-        constraints on label keys and values.
-
-        :param audit_id: The ID of the Audit to label.
-        :type audit_id: str
-        :param labels: The label keys and values.
-        :type labels: dict[str, Optional[str]]
-        """
-        if not labels:
-            return
-        labels = LabelUpdateRequest(labels=labels).dict()
-        self._raw_ops.label(audit_id, labels)
-
-    def upload(self, audit_id: str, file_path: str, **kwargs) -> None:
-        """Upload an Audit report.
-
-        Raises a 404 error if no entity exists with that key.
-
-        :param audit_id: The Audit id.
-        :type audit_id: str
-        :param file_path: The path to the audit report data on the local file
-            system. The report data must be packages as a ``.tar.gz`` archive.
-        :type file_path: str
-        :raises ~azure.core.exceptions.HttpResponseError:
-        """
-        error_map = {
-            401: ClientAuthenticationError,
-            404: ResourceNotFoundError,
-            409: ResourceExistsError,
-            304: ResourceNotModifiedError,
-        }
-        error_map.update(kwargs.pop("error_map", {}) or {})
-
-        _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-        _params = kwargs.pop("params", {}) or {}
-
-        with open(file_path, "rb") as fin:
-            request = build_audits_upload_request(
-                audit_id=audit_id,
-                file=fin,
-                headers=_headers,
-                params=_params,
-            )
-            request.url = self._raw_ops._client.format_url(request.url)
-
-            _stream = False
-            pipeline_response: PipelineResponse = (
-                self._raw_ops._client._pipeline.run(  # pylint: disable=protected-access
-                    request, stream=_stream, **kwargs
-                )
-            )
-
-        response = pipeline_response.http_response
-
-        if response.status_code not in [200, 422]:
-            map_error(
-                status_code=response.status_code, response=response, error_map=error_map
-            )
-            raise HttpResponseError(response=response)
-
-        if response.status_code == 422:
-            if response.content:
-                deserialized = response.json()
-            else:
-                deserialized = None
-            raise ValueError(f"Unprocessable entity: {deserialized}")
-
-
-class AuditproceduresOperations:
-    """Operations on :class:`~dyff.schema.platform.AuditProcedure` entities.
-
-    .. note::
-
-      Do not instantiate this class. Access it through the
-      ``.auditprocedures`` attribute of :class:`~dyff.client.Client`.
-    """
-
-    def __init__(self, _raw_ops: AuditproceduresOperationsGenerated):
-        self._raw_ops = _raw_ops
-
-    def download(self, path: str) -> BytesIO:
-        """Fetch the source code of an audit procedure.
-
-        The data is returned as an in-memory ``.tar.gz`` archive.
-
-        :param path: The relative path to the source code in the git repository.
-        :type path: str
-        :return: The audit procedure source code as an in-memory ``.tar.gz`` archive.
-        """
-        stream = self._raw_ops.download(path)
-        blob = bytearray()
-        for chunk in stream:
-            blob.extend(chunk)  # type: ignore
-        return BytesIO(blob)
-
-
 class DatasetsOperations:
     """Operations on :class:`~dyff.schema.platform.Dataset` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
       ``.datasets`` attribute of :class:`~dyff.client.Client`.
@@ -832,14 +489,50 @@
                     content=fin,
                     headers=headers,
                     verify=not self._insecure,
                 )
                 response.raise_for_status()
         _retry_not_found(self._raw_ops.finalize)(dataset.id)
 
+    def documentation(self, dataset_id: str) -> Documentation:
+        """Get the documentation associated with a Dataset.
+
+        Get the documentation associated with a Dataset. Raises a 404 error if no entity
+        exists with that key.
+
+        :param dataset_id: The ID of the Dataset.
+        :type dataset_id: str
+        :return: The documentation associated with the Dataset.
+        :rtype: Documentation :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return Documentation.parse_obj(self._raw_ops.documentation(dataset_id))
+
+    def edit_documentation(
+        self, dataset_id: str, edit_request: DocumentationEditRequest
+    ) -> Documentation:
+        """Edit the documentation associated with a Dataset.
+
+        Edit the documentation associated with a Dataset. Raises a 404 error if no
+        entity exists with that key. Returns the modified Documentation.
+
+        :param dataset_id: The ID of the Dataset.
+        :type dataset_id: str
+        :param edit_request: Object containing the edits to make.
+        :type edit_request: DocumentationEditRequest
+        :return: The modified documentation.
+        :rtype: Documentation :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return Documentation.parse_obj(
+            # exclude_unset: Users can explicitly set a field to None, but we
+            # don't want to overwrite with None implicitly
+            self._raw_ops.edit_documentation(
+                dataset_id, edit_request.dict(exclude_unset=True)
+            )
+        )
+
 
 class EvaluationsOperations:
     """Operations on :class:`~dyff.schema.platform.Evaluation` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
@@ -1070,14 +763,50 @@
         :return: A full InferenceService entity with .id and other properties set.
         """
         inferenceservice = _retry_not_found(self._raw_ops.create)(
             inference_service_request.dict()
         )
         return InferenceService.parse_obj(inferenceservice)
 
+    def documentation(self, service_id: str) -> Documentation:
+        """Get the documentation associated with an InferenceService.
+
+        Get the documentation associated with a InferenceService. Raises a 404 error if
+        no entity exists with that key.
+
+        :param service_id: The ID of the InferenceService.
+        :type service_id: str
+        :return: The documentation associated with the InferenceService.
+        :rtype: Documentation :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return Documentation.parse_obj(self._raw_ops.documentation(service_id))
+
+    def edit_documentation(
+        self, service_id: str, edit_request: DocumentationEditRequest
+    ) -> Documentation:
+        """Edit the documentation associated with an InferenceService.
+
+        Edit the documentation associated with an InferenceService. Raises a 404 error
+        if no entity exists with that key. Returns the modified Documentation.
+
+        :param service_id: The ID of the InferenceService.
+        :type service_id: str
+        :param edit_request: Object containing the edits to make.
+        :type edit_request: DocumentationEditRequest
+        :return: The modified documentation.
+        :rtype: Documentation :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return Documentation.parse_obj(
+            # exclude_unset: Users can explicitly set a field to None, but we
+            # don't want to overwrite with None implicitly
+            self._raw_ops.edit_documentation(
+                service_id, edit_request.dict(exclude_unset=True)
+            )
+        )
+
 
 class InferencesessionsOperations:
     """Operations on :class:`~dyff.schema.platform.Inferencesession` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
@@ -1541,14 +1270,50 @@
         :param method_request: The Method specification.
         :type method_request: MethodCreateRequest
         :return: A full Method entity with .id and other properties set.
         """
         method = _retry_not_found(self._raw_ops.create)(method_request.dict())
         return Method.parse_obj(method)
 
+    def documentation(self, method_id: str) -> Documentation:
+        """Get the documentation associated with a Method.
+
+        Get the documentation associated with a Method. Raises a 404 error if no entity
+        exists with that key.
+
+        :param method_id: The ID of the Method.
+        :type method_id: str
+        :return: The documentation associated with the Method.
+        :rtype: Documentation :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return Documentation.parse_obj(self._raw_ops.documentation(method_id))
+
+    def edit_documentation(
+        self, method_id: str, edit_request: DocumentationEditRequest
+    ) -> Documentation:
+        """Edit the documentation associated with a Method.
+
+        Edit the documentation associated with a Method. Raises a 404 error if no entity
+        exists with that key. Returns the modified Documentation.
+
+        :param method_id: The ID of the Method.
+        :type method_id: str
+        :param edit_request: Object containing the edits to make.
+        :type edit_request: DocumentationEditRequest
+        :return: The modified documentation.
+        :rtype: Documentation :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return Documentation.parse_obj(
+            # exclude_unset: Users can explicitly set a field to None, but we
+            # don't want to overwrite with None implicitly
+            self._raw_ops.edit_documentation(
+                method_id, edit_request.dict(exclude_unset=True)
+            )
+        )
+
 
 class ModelsOperations:
     """Operations on :class:`~dyff.schema.platform.Model` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
@@ -1646,14 +1411,50 @@
         :param model_request: The model specification.
         :type model: Model
         :return: A full Model entity with .id and other properties set.
         """
         model = _retry_not_found(self._raw_ops.create)(model_request.dict())
         return Model.parse_obj(model)
 
+    def documentation(self, model_id: str) -> Documentation:
+        """Get the documentation associated with a Model.
+
+        Get the documentation associated with a Model. Raises a 404 error if no entity
+        exists with that key.
+
+        :param model_id: The ID of the Model.
+        :type model_id: str
+        :return: The documentation associated with the Model.
+        :rtype: Documentation :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return Documentation.parse_obj(self._raw_ops.documentation(model_id))
+
+    def edit_documentation(
+        self, model_id: str, edit_request: DocumentationEditRequest
+    ) -> Documentation:
+        """Edit the documentation associated with a Model.
+
+        Edit the documentation associated with a Method. Raises a 404 error if no entity
+        exists with that key. Returns the modified Documentation.
+
+        :param model_id: The ID of the Model.
+        :type model_id: str
+        :param edit_request: Object containing the edits to make.
+        :type edit_request: DocumentationEditRequest
+        :return: The modified documentation.
+        :rtype: Documentation :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return Documentation.parse_obj(
+            # exclude_unset: Users can explicitly set a field to None, but we
+            # don't want to overwrite with None implicitly
+            self._raw_ops.edit_documentation(
+                model_id, edit_request.dict(exclude_unset=True)
+            )
+        )
+
 
 class ModulesOperations:
     """Operations on :class:`~dyff.schema.platform.Module` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
@@ -1858,14 +1659,50 @@
                     content=fin,
                     headers=headers,
                     verify=not self._insecure,
                 )
                 response.raise_for_status()
         _retry_not_found(self._raw_ops.finalize)(module.id)
 
+    def documentation(self, module_id: str) -> Documentation:
+        """Get the documentation associated with a Module.
+
+        Get the documentation associated with a Module. Raises a 404 error if no entity
+        exists with that key.
+
+        :param module_id: The ID of the Module.
+        :type module_id: str
+        :return: The documentation associated with the Module.
+        :rtype: Documentation :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return Documentation.parse_obj(self._raw_ops.documentation(module_id))
+
+    def edit_documentation(
+        self, module_id: str, edit_request: DocumentationEditRequest
+    ) -> Documentation:
+        """Edit the documentation associated with a Module.
+
+        Edit the documentation associated with a Method. Raises a 404 error if no entity
+        exists with that key. Returns the modified Documentation.
+
+        :param module_id: The ID of the Module.
+        :type module_id: str
+        :param edit_request: Object containing the edits to make.
+        :type edit_request: DocumentationEditRequest
+        :return: The modified documentation.
+        :rtype: Documentation :raises ~azure.core.exceptions.HttpResponseError:
+        """
+        return Documentation.parse_obj(
+            # exclude_unset: Users can explicitly set a field to None, but we
+            # don't want to overwrite with None implicitly
+            self._raw_ops.edit_documentation(
+                module_id, edit_request.dict(exclude_unset=True)
+            )
+        )
+
 
 class ReportsOperations:
     """Operations on :class:`~dyff.schema.platform.Report` entities.
 
     .. note::
 
       Do not instantiate this class. Access it through the
@@ -2210,17 +2047,14 @@
         # False
         # >> print(self._pipeline._transport.connection_config.verify)
         # True
         self._raw._client._pipeline._transport.connection_config.verify = (  # type: ignore
             not insecure
         )
 
-        # self._analyses = AnalysesOperations(self._raw.analyses)
-        self._audits = AuditsOperations(self._raw.audits)
-        self._auditprocedures = AuditproceduresOperations(self._raw.auditprocedures)
         self._datasets = DatasetsOperations(self._raw.datasets, insecure=insecure)
         self._evaluations = EvaluationsOperations(self._raw.evaluations)
         self._inferenceservices = InferenceservicesOperations(
             self._raw.inferenceservices
         )
         self._inferencesessions = InferencesessionsOperations(
             self._raw.inferencesessions,
@@ -2237,29 +2071,14 @@
         self._safetycases = SafetycasesOperations(self._raw.safetycases)
 
     @property
     def raw(self) -> RawClient:
         """The "raw" API client, which can be used to send JSON requests directly."""
         return self._raw
 
-    # @property
-    # def analyses(self) -> AnalysesOperations:
-    #     """Operations on :class:`~dyff.schema.platform.Analysis` entities."""
-    #     return self._analyses
-
-    @property
-    def audits(self) -> AuditsOperations:
-        """Operations on :class:`~dyff.schema.platform.Audit` entities."""
-        return self._audits
-
-    @property
-    def auditprocedures(self) -> AuditproceduresOperations:
-        """Operations on :class:`~dyff.schema.platform.AuditProcedure` entities."""
-        return self._auditprocedures
-
     @property
     def datasets(self) -> DatasetsOperations:
         """Operations on :class:`~dyff.schema.platform.Dataset` entities."""
         return self._datasets
 
     @property
     def evaluations(self) -> EvaluationsOperations:
```

### Comparing `dyff_client-0.3.2/dyff_client.egg-info/PKG-INFO` & `dyff_client-0.4.2/dyff_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-client
-Version: 0.3.2
+Version: 0.4.2
 Summary: Python client for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-client
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-client/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff_client-0.3.2/dyff_client.egg-info/SOURCES.txt` & `dyff_client-0.4.2/dyff_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/makefile` & `dyff_client-0.4.2/makefile`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/pyproject.toml` & `dyff_client-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/scripts/inferenceservices/databricks--dolly-v2-3b--default.py` & `dyff_client-0.4.2/scripts/inferenceservices/databricks--dolly-v2-3b--default.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/scripts/inferenceservices/tiiuae--falcon-7b--default.py` & `dyff_client-0.4.2/scripts/inferenceservices/tiiuae--falcon-7b--default.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/scripts/models/databricks--dolly-v2-3b.py` & `dyff_client-0.4.2/scripts/models/databricks--dolly-v2-3b.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/scripts/models/tiiuae--falcon-7b.py` & `dyff_client-0.4.2/scripts/models/tiiuae--falcon-7b.py`

 * *Files identical despite different names*

### Comparing `dyff_client-0.3.2/tests/test_import.py` & `dyff_client-0.4.2/tests/test_import.py`

 * *Files identical despite different names*

