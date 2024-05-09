# Comparing `tmp/ape-polygon-zkevm-0.7.1.tar.gz` & `tmp/ape-polygon-zkevm-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-polygon-zkevm-0.7.1.tar", last modified: Tue Jan 23 19:28:23 2024, max compression
+gzip compressed data, was "ape-polygon-zkevm-0.7.2.tar", last modified: Thu May  9 01:18:31 2024, max compression
```

## Comparing `ape-polygon-zkevm-0.7.1.tar` & `ape-polygon-zkevm-0.7.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:28:23.598038 ape-polygon-zkevm-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:28:23.594038 ape-polygon-zkevm-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:28:23.594038 ape-polygon-zkevm-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:28:23.594038 ape-polygon-zkevm-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-01-23 19:28:23.598038 ape-polygon-zkevm-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:28:23.594038 ape-polygon-zkevm-0.7.1/ape_polygon_zkevm/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/ape_polygon_zkevm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/ape_polygon_zkevm/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/ape_polygon_zkevm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-23 19:28:23.000000 ape-polygon-zkevm-0.7.1/ape_polygon_zkevm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:28:23.598038 ape-polygon-zkevm-0.7.1/ape_polygon_zkevm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-01-23 19:28:23.000000 ape-polygon-zkevm-0.7.1/ape_polygon_zkevm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-01-23 19:28:23.000000 ape-polygon-zkevm-0.7.1/ape_polygon_zkevm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 19:28:23.000000 ape-polygon-zkevm-0.7.1/ape_polygon_zkevm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 19:28:23.000000 ape-polygon-zkevm-0.7.1/ape_polygon_zkevm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-23 19:28:23.000000 ape-polygon-zkevm-0.7.1/ape_polygon_zkevm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-23 19:28:23.000000 ape-polygon-zkevm-0.7.1/ape_polygon_zkevm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-23 19:28:23.598038 ape-polygon-zkevm-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:28:23.598038 ape-polygon-zkevm-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/tests/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-23 19:27:27.000000 ape-polygon-zkevm-0.7.1/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.293650 ape-polygon-zkevm-0.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.289650 ape-polygon-zkevm-0.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.289650 ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.289650 ape-polygon-zkevm-0.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-09 01:18:31.293650 ape-polygon-zkevm-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.289650 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.289650 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-09 01:18:31.293650 ape-polygon-zkevm-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.293650 ape-polygon-zkevm-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/tests/test_provider.py
```

### Comparing `ape-polygon-zkevm-0.7.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.1/.github/release-drafter.yml` & `ape-polygon-zkevm-0.7.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.1/.github/workflows/codeql.yaml` & `ape-polygon-zkevm-0.7.2/.github/workflows/codeql.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       security-events: write
 
     strategy:
       fail-fast: false
 
     steps:
     - name: Checkout repository
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     - name: Initialize CodeQL
       uses: github/codeql-action/init@v2
       with:
         languages: python
 
     - name: Autobuild
```

### Comparing `ape-polygon-zkevm-0.7.1/.github/workflows/commitlint.yaml` & `ape-polygon-zkevm-0.7.2/.github/workflows/commitlint.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # NOTE: Skip check on PR so as not to confuse contributors
 # NOTE: Also install a PR title checker so we don't mess up merges
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
           with:
               fetch-depth: 0
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check commit history
```

### Comparing `ape-polygon-zkevm-0.7.1/.github/workflows/prtitle.yaml` & `ape-polygon-zkevm-0.7.2/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
       - synchronize
 
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
```

### Comparing `ape-polygon-zkevm-0.7.1/.github/workflows/publish.yaml` & `ape-polygon-zkevm-0.7.2/.github/workflows/publish.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
```

### Comparing `ape-polygon-zkevm-0.7.1/.github/workflows/test.yaml` & `ape-polygon-zkevm-0.7.2/.github/workflows/test.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -10,18 +10,18 @@
   cancel-in-progress: true
 
 jobs:
     linting:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
@@ -38,18 +38,18 @@
         - name: Run mdformat
           run: mdformat . --check
 
     type-check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
@@ -58,22 +58,24 @@
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11"]
+                # TODO: Replace with macos-latest when works again.
+                #   https://github.com/actions/setup-python/issues/808
+                os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
+                python-version: [3.8, 3.9, "3.10", "3.11", "3.12"]
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[test]
@@ -85,18 +87,18 @@
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
 #
 #        steps:
-#        - uses: actions/checkout@v3
+#        - uses: actions/checkout@v4
 #
 #        - name: Setup Python
-#          uses: actions/setup-python@v4
+#          uses: actions/setup-python@v5
 #          with:
 #              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
```

### Comparing `ape-polygon-zkevm-0.7.1/.gitignore` & `ape-polygon-zkevm-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.1/.pre-commit-config.yaml` & `ape-polygon-zkevm-0.7.2/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: check-yaml
 
--   repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.10.1
+-   repo: https://github.com/PyCQA/isort
+    rev: 5.13.2
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 23.12.1
+    rev: 24.4.2
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
     rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.10.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
```

### Comparing `ape-polygon-zkevm-0.7.1/CONTRIBUTING.md` & `ape-polygon-zkevm-0.7.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.1/LICENSE` & `ape-polygon-zkevm-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.1/PKG-INFO` & `ape-polygon-zkevm-0.7.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-polygon-zkevm
-Version: 0.7.1
+Version: 0.7.2
 Summary: ape-polygon-zkevm: Ecosystem plugin for Polygon ZkEVM
 Home-page: https://github.com/ApeWorX/ape-polygon-zkevm
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,29 +14,30 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ecosystem Plugin for Polygon ZkEVM support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -55,15 +56,15 @@
 ```
 
 ## Quick Usage
 
 Installing this plugin adds support for the Polygon ZkEVM ecosystem:
 
 ```
-ape console --network polygon-zkevm:goerli 
+ape console --network polygon-zkevm:cardona
 ```
 
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-polygon-zkevm-0.7.1/README.md` & `ape-polygon-zkevm-0.7.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ecosystem Plugin for Polygon ZkEVM support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -27,15 +27,15 @@
 ```
 
 ## Quick Usage
 
 Installing this plugin adds support for the Polygon ZkEVM ecosystem:
 
 ```
-ape console --network polygon-zkevm:goerli 
+ape console --network polygon-zkevm:cardona
 ```
 
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-polygon-zkevm-0.7.1/ape_polygon_zkevm/__init__.py` & `ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.1/ape_polygon_zkevm/ecosystem.py` & `ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/ecosystem.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     NetworkConfig,
     create_network_config,
 )
 
 NETWORKS = {
     # chain_id, network_id
     "mainnet": (1101, 1101),
-    "goerli": (1442, 1442),
+    "cardona": (2442, 2442),
 }
 
 
 class PolygonZkEVMConfig(BaseEthereumConfig):
     mainnet: NetworkConfig = create_network_config(block_time=2, required_confirmations=1)
-    goerli: NetworkConfig = create_network_config(block_time=2, required_confirmations=1)
+    cardona: NetworkConfig = create_network_config(block_time=2, required_confirmations=1)
 
 
 class PolygonZkEVM(Ethereum):
     @property
     def config(self) -> PolygonZkEVMConfig:  # type: ignore
         return cast(PolygonZkEVMConfig, self.config_manager.get_config("polygon-zkevm"))
```

### Comparing `ape-polygon-zkevm-0.7.1/ape_polygon_zkevm.egg-info/PKG-INFO` & `ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-polygon-zkevm
-Version: 0.7.1
+Version: 0.7.2
 Summary: ape-polygon-zkevm: Ecosystem plugin for Polygon ZkEVM
 Home-page: https://github.com/ApeWorX/ape-polygon-zkevm
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,29 +14,30 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ecosystem Plugin for Polygon ZkEVM support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -55,15 +56,15 @@
 ```
 
 ## Quick Usage
 
 Installing this plugin adds support for the Polygon ZkEVM ecosystem:
 
 ```
-ape console --network polygon-zkevm:goerli 
+ape console --network polygon-zkevm:cardona
 ```
 
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-polygon-zkevm-0.7.1/ape_polygon_zkevm.egg-info/SOURCES.txt` & `ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.1/ape_polygon_zkevm.egg-info/requires.txt` & `ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -2,42 +2,42 @@
 ethpm-types
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
-black<24,>=23.12.1
-mypy<2,>=1.8.0
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
 flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 setuptools
 wheel
 twine
 commitizen
 pre-commit
 pytest-watch
 IPython
 ipdb
 
 [lint]
-black<24,>=23.12.1
-mypy<2,>=1.8.0
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
 flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 
 [release]
 setuptools
```

### Comparing `ape-polygon-zkevm-0.7.1/pyproject.toml` & `ape-polygon-zkevm-0.7.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-polygon-zkevm-0.7.1/setup.py` & `ape-polygon-zkevm-0.7.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=23.12.1,<24",  # Auto-formatter and linter
-        "mypy>=1.8.0,<2",  # Static type analyzer
+        "black>=24.4.2,<25",  # Auto-formatter and linter
+        "mypy>=1.10.0,<2",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
         "flake8>=7.0.0,<8",  # Style linter
         "flake8-breakpoint>=1.1.0,<2",  # Detect breakpoints left in code
         "flake8-print>=5.0.0,<6",  # Detect print statements left in code
-        "isort>=5.10.1,<6",  # Import sorting linter
+        "isort>=5.13.2,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
@@ -79,9 +79,10 @@
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `ape-polygon-zkevm-0.7.1/tests/conftest.py` & `ape-polygon-zkevm-0.7.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.1/tests/test_config.py` & `ape-polygon-zkevm-0.7.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.1/tests/test_ecosystem.py` & `ape-polygon-zkevm-0.7.2/tests/test_ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.1/tests/test_integration.py` & `ape-polygon-zkevm-0.7.2/tests/test_integration.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ape._cli import cli as ape_cli
 from click.testing import CliRunner
 
 EXPECTED_OUTPUT = """
 polygon-zkevm
 ├── mainnet
 │   └── geth  (default)
-├── goerli
+├── cardona
 │   └── geth  (default)
 └── local  (default)
     └── test  (default)
 """.strip()
 
 
 @pytest.fixture
@@ -43,11 +43,11 @@
     for expected_line in expected_lines:
         assert expected_line in actual_lines
 
 
 def test_networks(runner, cli, polygon_zkevm):
     # Do this in case local env changed it.
     polygon_zkevm.mainnet.set_default_provider("geth")
-    polygon_zkevm.goerli.set_default_provider("geth")
+    polygon_zkevm.cardona.set_default_provider("geth")
 
     result = runner.invoke(cli, ["networks", "list"])
     assert_rich_text(result.output, EXPECTED_OUTPUT)
```

