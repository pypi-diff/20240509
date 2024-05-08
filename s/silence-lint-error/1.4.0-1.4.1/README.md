# Comparing `tmp/silence_lint_error-1.4.0.tar.gz` & `tmp/silence_lint_error-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silence_lint_error-1.4.0.tar", last modified: Thu Apr 11 09:48:15 2024, max compression
+gzip compressed data, was "silence_lint_error-1.4.1.tar", last modified: Wed May  8 23:32:59 2024, max compression
```

## Comparing `silence_lint_error-1.4.0.tar` & `silence_lint_error-1.4.1.tar`

### file list

```diff
@@ -1,31 +1,18 @@
-drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2024-04-11 09:48:15.656846 silence_lint_error-1.4.0/
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1078 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/LICENSE
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     3196 2024-04-11 09:48:15.656731 silence_lint_error-1.4.0/PKG-INFO
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     2573 2024-04-11 09:47:00.000000 silence_lint_error-1.4.0/README.md
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1420 2024-04-11 09:48:15.657194 silence_lint_error-1.4.0/setup.cfg
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)       74 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/setup.py
-drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2024-04-11 09:48:15.653324 silence_lint_error-1.4.0/silence_lint_error/
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        0 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/silence_lint_error/__init__.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     3996 2023-12-15 23:41:05.000000 silence_lint_error-1.4.0/silence_lint_error/comments.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     4866 2023-12-15 23:41:05.000000 silence_lint_error-1.4.0/silence_lint_error/fix_silenced_error.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)    11052 2024-04-11 09:47:00.000000 silence_lint_error-1.4.0/silence_lint_error/silence_lint_error.py
-drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2024-04-11 09:48:15.656385 silence_lint_error-1.4.0/silence_lint_error.egg-info/
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     3196 2024-04-11 09:48:15.000000 silence_lint_error-1.4.0/silence_lint_error.egg-info/PKG-INFO
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)      784 2024-04-11 09:48:15.000000 silence_lint_error-1.4.0/silence_lint_error.egg-info/SOURCES.txt
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        1 2024-04-11 09:48:15.000000 silence_lint_error-1.4.0/silence_lint_error.egg-info/dependency_links.txt
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)      146 2024-04-11 09:48:15.000000 silence_lint_error-1.4.0/silence_lint_error.egg-info/entry_points.txt
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)       18 2024-04-11 09:48:15.000000 silence_lint_error-1.4.0/silence_lint_error.egg-info/requires.txt
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)       25 2024-04-11 09:48:15.000000 silence_lint_error-1.4.0/silence_lint_error.egg-info/top_level.txt
-drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2024-04-11 09:48:15.654441 silence_lint_error-1.4.0/tests/
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        0 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/tests/__init__.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     4095 2023-12-15 23:41:05.000000 silence_lint_error-1.4.0/tests/comments_test.py
-drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2024-04-11 09:48:15.654877 silence_lint_error-1.4.0/tests/fix_silenced_error/
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        0 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/tests/fix_silenced_error/__init__.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1725 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/tests/fix_silenced_error/fixit_test.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1308 2023-12-15 23:41:05.000000 silence_lint_error-1.4.0/tests/fix_silenced_error/ruff_test.py
-drwxr-xr-x   0 sam.searles-bryant   (501) staff       (20)        0 2024-04-11 09:48:15.655771 silence_lint_error-1.4.0/tests/silence_lint_error/
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)        0 2023-11-17 18:45:42.000000 silence_lint_error-1.4.0/tests/silence_lint_error/__init__.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     6387 2023-12-11 17:21:55.000000 silence_lint_error-1.4.0/tests/silence_lint_error/fixit_test.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     2065 2023-11-24 18:42:18.000000 silence_lint_error-1.4.0/tests/silence_lint_error/flake8_test.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     1898 2023-11-24 18:42:18.000000 silence_lint_error-1.4.0/tests/silence_lint_error/ruff_test.py
--rw-r--r--   0 sam.searles-bryant   (501) staff       (20)     2347 2024-04-11 09:47:00.000000 silence_lint_error-1.4.0/tests/silence_lint_error/semgrep_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:59.335232 silence_lint_error-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-08 23:32:56.000000 silence_lint_error-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-08 23:32:59.335232 silence_lint_error-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-08 23:32:56.000000 silence_lint_error-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-08 23:32:59.335232 silence_lint_error-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 23:32:56.000000 silence_lint_error-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:59.331232 silence_lint_error-1.4.1/silence_lint_error/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:56.000000 silence_lint_error-1.4.1/silence_lint_error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-08 23:32:56.000000 silence_lint_error-1.4.1/silence_lint_error/comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-08 23:32:56.000000 silence_lint_error-1.4.1/silence_lint_error/fix_silenced_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11052 2024-05-08 23:32:56.000000 silence_lint_error-1.4.1/silence_lint_error/silence_lint_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 23:32:59.335232 silence_lint_error-1.4.1/silence_lint_error.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-08 23:32:59.000000 silence_lint_error-1.4.1/silence_lint_error.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-08 23:32:59.000000 silence_lint_error-1.4.1/silence_lint_error.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 23:32:59.000000 silence_lint_error-1.4.1/silence_lint_error.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-08 23:32:59.000000 silence_lint_error-1.4.1/silence_lint_error.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-08 23:32:59.000000 silence_lint_error-1.4.1/silence_lint_error.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 23:32:59.000000 silence_lint_error-1.4.1/silence_lint_error.egg-info/top_level.txt
```

### Comparing `silence_lint_error-1.4.0/LICENSE` & `silence_lint_error-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `silence_lint_error-1.4.0/PKG-INFO` & `silence_lint_error-1.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silence_lint_error
-Version: 1.4.0
+Version: 1.4.1
 Summary: silence linting errors by adding ignore/fixme comments
 Home-page: https://github.com/samueljsb/silence-lint-error
 Author: Samuel Searles-Bryant
 Author-email: sam@samueljsb.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -66,14 +66,16 @@
 run:
 
 ```shell
 SEMGREP_RULES=r/python silence-lint-error semgrep python.lang.best-practice.sleep.arbitrary-sleep path/to/files/ path/to/more/files/
 ```
 
 N.B. The rules must be configured in an environment variable.
+For more information about configuring semgrep rules,
+see the `--config` entry in the [`semgrep` documentation](https://semgrep.dev/docs/cli-reference-oss/)
 
 ### fix silenced errors
 
 If there is an auto-fix for a linting error, you can remove the `ignore` or
 `fixme` comments and apply the auto-fix.
 
 For example, to remove all `lint-fixme: CollapseIsinstanceChecks` comments and
```

### Comparing `silence_lint_error-1.4.0/README.md` & `silence_lint_error-1.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 run:
 
 ```shell
 SEMGREP_RULES=r/python silence-lint-error semgrep python.lang.best-practice.sleep.arbitrary-sleep path/to/files/ path/to/more/files/
 ```
 
 N.B. The rules must be configured in an environment variable.
+For more information about configuring semgrep rules,
+see the `--config` entry in the [`semgrep` documentation](https://semgrep.dev/docs/cli-reference-oss/)
 
 ### fix silenced errors
 
 If there is an auto-fix for a linting error, you can remove the `ignore` or
 `fixme` comments and apply the auto-fix.
 
 For example, to remove all `lint-fixme: CollapseIsinstanceChecks` comments and
```

### Comparing `silence_lint_error-1.4.0/setup.cfg` & `silence_lint_error-1.4.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = silence_lint_error
-version = 1.4.0
+version = 1.4.1
 description = silence linting errors by adding ignore/fixme comments
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/samueljsb/silence-lint-error
 author = Samuel Searles-Bryant
 author_email = sam@samueljsb.co.uk
 license = MIT
@@ -12,16 +12,14 @@
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
-packages = 
-	find:
 install_requires = 
 	attrs
 	tokenize-rt
 python_requires = >=3.9
 
 [options.entry_points]
 console_scripts =
```

### Comparing `silence_lint_error-1.4.0/silence_lint_error/comments.py` & `silence_lint_error-1.4.1/silence_lint_error/comments.py`

 * *Files identical despite different names*

### Comparing `silence_lint_error-1.4.0/silence_lint_error/fix_silenced_error.py` & `silence_lint_error-1.4.1/silence_lint_error/fix_silenced_error.py`

 * *Files identical despite different names*

### Comparing `silence_lint_error-1.4.0/silence_lint_error/silence_lint_error.py` & `silence_lint_error-1.4.1/silence_lint_error/silence_lint_error.py`

 * *Files identical despite different names*

### Comparing `silence_lint_error-1.4.0/silence_lint_error.egg-info/PKG-INFO` & `silence_lint_error-1.4.1/silence_lint_error.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silence_lint_error
-Version: 1.4.0
+Version: 1.4.1
 Summary: silence linting errors by adding ignore/fixme comments
 Home-page: https://github.com/samueljsb/silence-lint-error
 Author: Samuel Searles-Bryant
 Author-email: sam@samueljsb.co.uk
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -66,14 +66,16 @@
 run:
 
 ```shell
 SEMGREP_RULES=r/python silence-lint-error semgrep python.lang.best-practice.sleep.arbitrary-sleep path/to/files/ path/to/more/files/
 ```
 
 N.B. The rules must be configured in an environment variable.
+For more information about configuring semgrep rules,
+see the `--config` entry in the [`semgrep` documentation](https://semgrep.dev/docs/cli-reference-oss/)
 
 ### fix silenced errors
 
 If there is an auto-fix for a linting error, you can remove the `ignore` or
 `fixme` comments and apply the auto-fix.
 
 For example, to remove all `lint-fixme: CollapseIsinstanceChecks` comments and
```

