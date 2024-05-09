# Comparing `tmp/dsi_cocoa-0.1.9.tar.gz` & `tmp/dsi_cocoa-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsi_cocoa-0.1.9.tar", last modified: Wed May  8 16:13:41 2024, max compression
+gzip compressed data, was "dsi_cocoa-0.2.0.tar", last modified: Thu May  9 20:51:07 2024, max compression
```

## Comparing `dsi_cocoa-0.1.9.tar` & `dsi_cocoa-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:41.268186 dsi_cocoa-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:41.264186 dsi_cocoa-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:41.264186 dsi_cocoa-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/.github/workflows/main.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/.github/workflows/publish.workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-08 16:13:41.268186 dsi_cocoa-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/eval-repo.sh
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-08 16:13:41.268186 dsi_cocoa-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:41.264186 dsi_cocoa-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:41.268186 dsi_cocoa-0.1.9/src/cocoa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/evaluate_repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-08 16:13:36.000000 dsi_cocoa-0.1.9/src/cocoa/spring2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:13:41.268186 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-08 16:13:41.000000 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-08 16:13:41.000000 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:13:41.000000 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 16:13:41.000000 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-08 16:13:41.000000 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 16:13:41.000000 dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:07.755569 dsi_cocoa-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:07.747569 dsi_cocoa-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:07.751569 dsi_cocoa-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/.github/workflows/main.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/.github/workflows/publish.workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-09 20:51:07.755569 dsi_cocoa-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/eval-repo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-09 20:51:07.755569 dsi_cocoa-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:07.751569 dsi_cocoa-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:07.751569 dsi_cocoa-0.2.0/src/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6559 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/evaluate_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-09 20:51:03.000000 dsi_cocoa-0.2.0/src/cocoa/spring2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 20:51:07.755569 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-09 20:51:07.000000 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-09 20:51:07.000000 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 20:51:07.000000 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-09 20:51:07.000000 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-09 20:51:07.000000 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 20:51:07.000000 dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/top_level.txt
```

### Comparing `dsi_cocoa-0.1.9/.github/workflows/main.workflow.yml` & `dsi_cocoa-0.2.0/.github/workflows/main.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.9/.github/workflows/publish.workflow.yml` & `dsi_cocoa-0.2.0/.github/workflows/publish.workflow.yml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.9/.gitignore` & `dsi_cocoa-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.9/.pre-commit-config.yaml` & `dsi_cocoa-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.9/PKG-INFO` & `dsi_cocoa-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.1.9
+Version: 0.2.0
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -23,15 +23,15 @@
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
 ```pip install dsi-cocoa```
 
-To install the package from the local files, run the following command from the root of the repository:
+To install the package locally, run the following command from the root of the repository:
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
 
 This package contains a module `evaluate_repo` which runs code testing libraries against a repository. There are multiple ways that we want to be able to run this repo:
@@ -63,26 +63,34 @@
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
-If you want to do linting on Python files, then you can add the argument "--lint" to the command:
+If you want to turn on linting, add the argument "--lint":
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
 
 ```bash
 cocoa /path/to/repo --verbose
 ```
 
+To report remote branch information, use the `--branchinfo` option.
+
+To run cocoa on files changed after a certain date, use the `--date` option with a date formatted as below.
+```bash
+cocoa /path/to/repo --date YYYY-MM-DD
+```
+
+
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
 1. WARNING: Most likely this needs to be fixed. 
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
```

### Comparing `dsi_cocoa-0.1.9/README.md` & `dsi_cocoa-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
 ```pip install dsi-cocoa```
 
-To install the package from the local files, run the following command from the root of the repository:
+To install the package locally, run the following command from the root of the repository:
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
 
 This package contains a module `evaluate_repo` which runs code testing libraries against a repository. There are multiple ways that we want to be able to run this repo:
@@ -44,26 +44,34 @@
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
-If you want to do linting on Python files, then you can add the argument "--lint" to the command:
+If you want to turn on linting, add the argument "--lint":
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
 
 ```bash
 cocoa /path/to/repo --verbose
 ```
 
+To report remote branch information, use the `--branchinfo` option.
+
+To run cocoa on files changed after a certain date, use the `--date` option with a date formatted as below.
+```bash
+cocoa /path/to/repo --date YYYY-MM-DD
+```
+
+
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
 1. WARNING: Most likely this needs to be fixed. 
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
```

### Comparing `dsi_cocoa-0.1.9/pyproject.toml` & `dsi_cocoa-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.9/src/cocoa/evaluate_repo.py` & `dsi_cocoa-0.2.0/src/cocoa/evaluate_repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -141,26 +141,29 @@
             print(f"\t{tool_name} found {len(results)} issues:")
             for result in results[:5]:
                 print(f"\t  {result}")
             if len(results) > 5:
                 print(f"\t  ...and {len(results) - 5} more issues.")
 
 
-def evaluate_repo(path_or_url, lint_flag, start_date=None, verbose=False):
+def evaluate_repo(
+    path_or_url, lint_flag, start_date=None, verbose=False, branchinfo=False
+):
     """
     This is the entry point to running the automated code review.
     """
 
     if os.path.isdir(path_or_url):
         if not is_git_repo(path_or_url):
             print(f"Error: {path_or_url} is not a Git repository.")
             exit(1)
 
         check_branch_names(path_or_url)
-        get_remote_branches_info(path_or_url)
+        if branchinfo:
+            get_remote_branches_info(path_or_url)
         walk_and_process(
             path_or_url,
             None,
             lint_flag=lint_flag,
             start_date=start_date,
             verbose=verbose,
         )
@@ -188,20 +191,24 @@
     )
     parser.add_argument(
         "--date",
         default=None,
         help="Start date in YYYY-MM-DD format to filter files by commit date",
         type=str,
     )
+    parser.add_argument(
+        "--branchinfo", help="Report branch information", action="store_true"
+    )
 
     args = parser.parse_args()
 
     dir_path = args.repo
     lint_flag = args.lint
     start_date = args.date
     verbose = args.verbose
+    branchinfo = args.branchinfo
 
-    evaluate_repo(dir_path, lint_flag, start_date, verbose)
+    evaluate_repo(dir_path, lint_flag, start_date, verbose, branchinfo)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dsi_cocoa-0.1.9/src/cocoa/linting.py` & `dsi_cocoa-0.2.0/src/cocoa/linting.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.9/src/cocoa/notebooks.py` & `dsi_cocoa-0.2.0/src/cocoa/notebooks.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.9/src/cocoa/repo.py` & `dsi_cocoa-0.2.0/src/cocoa/repo.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.9/src/cocoa/spring2024.py` & `dsi_cocoa-0.2.0/src/cocoa/spring2024.py`

 * *Files identical despite different names*

### Comparing `dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/PKG-INFO` & `dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsi-cocoa
-Version: 0.1.9
+Version: 0.2.0
 Summary: Clinic Opinionated Codebase Oversight and Analysis
 Author-email: Nick Ross <tspread@uchicago.edu>, Trevor Spreadbury <tspread@uchicago.edu>
 Maintainer: Nick Ross, Trevor Spreadbury
 Keywords: codebase analysis,uchicago dsi
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -23,15 +23,15 @@
 
 The goals of this codebase is to provide a quick and easy way to review code and to alert contributors where their code may be failing.
 
 ## Installation
 
 ```pip install dsi-cocoa```
 
-To install the package from the local files, run the following command from the root of the repository:
+To install the package locally, run the following command from the root of the repository:
 ```bash
 python3 -m pip install .
 ```
 
 ## cocoa
 
 This package contains a module `evaluate_repo` which runs code testing libraries against a repository. There are multiple ways that we want to be able to run this repo:
@@ -63,26 +63,34 @@
 A few important notes:
 
 1. Make sure to `git pull` _before_ running this code.
 1. This will get branch information for all branches.
 1. This will only run the analysis (`pyflakes` on python files) for the code _in the current branch_. So if you run this while your current branch is `main` it will run on `main`.
 
 #### Options
-If you want to do linting on Python files, then you can add the argument "--lint" to the command:
+If you want to turn on linting, add the argument "--lint":
 
 ```bash
 cocoa /path/to/repo --lint
 ```
 
 Results are truncated by default. To print all results, use the verbose option:
 
 ```bash
 cocoa /path/to/repo --verbose
 ```
 
+To report remote branch information, use the `--branchinfo` option.
+
+To run cocoa on files changed after a certain date, use the `--date` option with a date formatted as below.
+```bash
+cocoa /path/to/repo --date YYYY-MM-DD
+```
+
+
 ### Checks
 
 The code run multiple checks on each repo. For each check run there are three possibilities:
 
 1. WARNING: Most likely this needs to be fixed. 
 1. INFO: Log information for additional context.
 1. ERROR: A critical issue that needs to be addressed.
```

### Comparing `dsi_cocoa-0.1.9/src/dsi_cocoa.egg-info/SOURCES.txt` & `dsi_cocoa-0.2.0/src/dsi_cocoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

