# Comparing `tmp/golink-0.5.6.tar.gz` & `tmp/golink-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golink-0.5.6.tar", max compression
+gzip compressed data, was "golink-0.5.7.tar", max compression
```

## Comparing `golink-0.5.6.tar` & `golink-0.5.7.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2024-04-29 04:04:28.448306 golink-0.5.6/LICENSE
--rw-r--r--   0        0        0     2858 2024-05-09 20:17:16.306197 golink-0.5.6/README.md
--rw-r--r--   0        0        0      100 2024-05-09 20:26:37.020179 golink-0.5.6/golink/__init__.py
--rw-r--r--   0        0        0     7928 2024-05-06 18:41:37.701305 golink-0.5.6/golink/cli.py
--rw-r--r--   0        0        0     1988 2024-04-29 04:04:28.448306 golink-0.5.6/golink/script.js
--rw-r--r--   0        0        0     3361 2024-04-29 04:04:28.448306 golink-0.5.6/golink/style.css
--rw-r--r--   0        0        0     7729 2024-04-29 04:04:28.448306 golink-0.5.6/golink/utils.py
--rw-r--r--   0        0        0      793 2024-05-09 20:42:37.522871 golink-0.5.6/pyproject.toml
--rw-r--r--   0        0        0     3555 1970-01-01 00:00:00.000000 golink-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-29 04:04:28.448306 golink-0.5.7/LICENSE
+-rw-r--r--   0        0        0     2858 2024-05-09 20:17:16.306197 golink-0.5.7/README.md
+-rw-r--r--   0        0        0      100 2024-05-09 20:26:37.020179 golink-0.5.7/golink/__init__.py
+-rw-r--r--   0        0        0     7928 2024-05-06 18:41:37.701305 golink-0.5.7/golink/cli.py
+-rw-r--r--   0        0        0     1988 2024-04-29 04:04:28.448306 golink-0.5.7/golink/script.js
+-rw-r--r--   0        0        0     3361 2024-04-29 04:04:28.448306 golink-0.5.7/golink/style.css
+-rw-r--r--   0        0        0     7729 2024-04-29 04:04:28.448306 golink-0.5.7/golink/utils.py
+-rw-r--r--   0        0        0      815 2024-05-09 20:45:47.646617 golink-0.5.7/pyproject.toml
+-rw-r--r--   0        0        0     3598 1970-01-01 00:00:00.000000 golink-0.5.7/PKG-INFO
```

### Comparing `golink-0.5.6/LICENSE` & `golink-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `golink-0.5.6/README.md` & `golink-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `golink-0.5.6/golink/cli.py` & `golink-0.5.7/golink/cli.py`

 * *Files identical despite different names*

### Comparing `golink-0.5.6/golink/script.js` & `golink-0.5.7/golink/script.js`

 * *Files identical despite different names*

### Comparing `golink-0.5.6/golink/style.css` & `golink-0.5.7/golink/style.css`

 * *Files identical despite different names*

### Comparing `golink-0.5.6/golink/utils.py` & `golink-0.5.7/golink/utils.py`

 * *Files identical despite different names*

### Comparing `golink-0.5.6/pyproject.toml` & `golink-0.5.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -10,29 +10,30 @@
 
 # [project.scripts]
 # golink = "golink.cli:main"
 
 
 [tool.poetry]
 name = "golink"
-version = "0.5.6"
+version = "0.5.7"
 license = "GPLv3"
 description = "A simple URL shortener"
 authors = ["Max Vogel", "Logan Engstrom"]
 readme = "README.md"
 repository = "https://github.com/Mehvix/golink"
 
 packages = [{ include = "golink", from = "." }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 tqdm = "^4.66.4"
 tabulate = "^0.9.0"
 requests = "^2.31.0"
 pandas = "^2.2.2"
+gitpython = "^3.1.43"
 
 [tool.setuptools]
 include-package-data = true
 package-data = { "" = ["script.js", "style.css"] }
 zip-safe = false
 
 [tool.poetry.scripts]
```

### Comparing `golink-0.5.6/PKG-INFO` & `golink-0.5.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: golink
-Version: 0.5.6
+Version: 0.5.7
 Summary: A simple URL shortener
 Home-page: https://github.com/Mehvix/golink
 License: GPLv3
 Author: Max Vogel
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: gitpython (>=3.1.43,<4.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Project-URL: Repository, https://github.com/Mehvix/golink
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: golink Version: 0.5.6 Summary: A simple URL
+Metadata-Version: 2.1 Name: golink Version: 0.5.7 Summary: A simple URL
 shortener Home-page: https://github.com/Mehvix/golink License: GPLv3 Author:
 Max Vogel Requires-Python: >=3.9,<4.0 Classifier: License :: Other/Proprietary
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: pandas
-(>=2.2.2,<3.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist:
-tabulate (>=0.9.0,<0.10.0) Requires-Dist: tqdm (>=4.66.4,<5.0.0) Project-URL:
-Repository, https://github.com/Mehvix/golink Description-Content-Type: text/
-markdown # `golink` - git powered go-links
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: gitpython
+(>=3.1.43,<4.0.0) Requires-Dist: pandas (>=2.2.2,<3.0.0) Requires-Dist:
+requests (>=2.31.0,<3.0.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-
+Dist: tqdm (>=4.66.4,<5.0.0) Project-URL: Repository, https://github.com/
+Mehvix/golink Description-Content-Type: text/markdown # `golink` - git powered
+go-links
               Host your own "_g_o_-_l_i_n_k_s" via git and _g_i_t_h_u_b_ _p_a_g_e_s
                               pip install golink
                                [static/demo.gif]
 **What:** `golink` is a command line tool that maps custom shortlinks to URLs
 via [Git](https://git-scm.com) and [GitHub Pages](https://pages.github.com).
 This free software is licensed under GPLv3 and is a fork of [gitlink](https://
 github.com/lengstrom/gitlinks). **How:** `golink` works by [storing state on
```

