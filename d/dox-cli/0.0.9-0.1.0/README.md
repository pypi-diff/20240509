# Comparing `tmp/dox-cli-0.0.9.tar.gz` & `tmp/dox_cli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dox-cli-0.0.9.tar", last modified: Sun Jan 28 02:16:59 2024, max compression
+gzip compressed data, was "dox_cli-0.1.0.tar", last modified: Thu May  9 04:30:16 2024, max compression
```

## Comparing `dox-cli-0.0.9.tar` & `dox_cli-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:16:59.887238 dox-cli-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-28 02:16:48.000000 dox-cli-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 02:16:48.000000 dox-cli-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-01-28 02:16:59.887238 dox-cli-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-01-28 02:16:48.000000 dox-cli-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:16:59.883238 dox-cli-0.0.9/dox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:16:59.883238 dox-cli-0.0.9/dox/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/cmd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:16:59.883238 dox-cli-0.0.9/dox/cmd/check/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/cmd/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/cmd/check/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/cmd/check/ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/cmd/check/network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:16:59.883238 dox-cli-0.0.9/dox/cmd/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/cmd/gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/cmd/gitlab/create_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/cmd/gitlab/list_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:16:59.883238 dox-cli-0.0.9/dox/cmd/zero/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/cmd/zero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:16:59.883238 dox-cli-0.0.9/dox/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/utils/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-01-28 02:16:48.000000 dox-cli-0.0.9/dox/utils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 02:16:59.887238 dox-cli-0.0.9/dox_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-01-28 02:16:59.000000 dox-cli-0.0.9/dox_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-28 02:16:59.000000 dox-cli-0.0.9/dox_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 02:16:59.000000 dox-cli-0.0.9/dox_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-28 02:16:59.000000 dox-cli-0.0.9/dox_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-28 02:16:59.000000 dox-cli-0.0.9/dox_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-28 02:16:59.000000 dox-cli-0.0.9/dox_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 02:16:59.887238 dox-cli-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-28 02:16:48.000000 dox-cli-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:30:16.762651 dox_cli-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-09 04:30:13.000000 dox_cli-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:30:13.000000 dox_cli-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-09 04:30:16.762651 dox_cli-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4795 2024-05-09 04:30:13.000000 dox_cli-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:30:16.758651 dox_cli-0.1.0/dox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:30:16.758651 dox_cli-0.1.0/dox/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/cmd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:30:16.762651 dox_cli-0.1.0/dox/cmd/check/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/cmd/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/cmd/check/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/cmd/check/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/cmd/check/network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:30:16.762651 dox_cli-0.1.0/dox/cmd/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/cmd/gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/cmd/gitlab/create_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/cmd/gitlab/list_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:30:16.762651 dox_cli-0.1.0/dox/cmd/zero/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/cmd/zero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:30:16.762651 dox_cli-0.1.0/dox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/utils/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-09 04:30:13.000000 dox_cli-0.1.0/dox/utils/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:30:16.762651 dox_cli-0.1.0/dox_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-05-09 04:30:16.000000 dox_cli-0.1.0/dox_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 04:30:16.000000 dox_cli-0.1.0/dox_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:30:16.000000 dox_cli-0.1.0/dox_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 04:30:16.000000 dox_cli-0.1.0/dox_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-09 04:30:16.000000 dox_cli-0.1.0/dox_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-09 04:30:16.000000 dox_cli-0.1.0/dox_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 04:30:16.762651 dox_cli-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-09 04:30:13.000000 dox_cli-0.1.0/setup.py
```

### Comparing `dox-cli-0.0.9/LICENSE` & `dox_cli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dox-cli-0.0.9/PKG-INFO` & `dox_cli-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dox-cli
-Version: 0.0.9
+Version: 0.1.0
 Summary: Make all DevOps experience better
 Home-page: https://github.com/kaonmir/dox-cli
 Author: kaonmir
 Author-email: sonjeff@naver.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dox-cli-0.0.9/README.md` & `dox_cli-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dox-cli-0.0.9/dox/cmd/check/hardware.py` & `dox_cli-0.1.0/dox/cmd/check/hardware.py`

 * *Files identical despite different names*

### Comparing `dox-cli-0.0.9/dox/cmd/gitlab/list_project.py` & `dox_cli-0.1.0/dox/cmd/gitlab/list_project.py`

 * *Files identical despite different names*

### Comparing `dox-cli-0.0.9/dox/utils/gitlab.py` & `dox_cli-0.1.0/dox/utils/gitlab.py`

 * *Files identical despite different names*

### Comparing `dox-cli-0.0.9/dox/utils/helpers.py` & `dox_cli-0.1.0/dox/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dox-cli-0.0.9/dox_cli.egg-info/PKG-INFO` & `dox_cli-0.1.0/dox_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dox-cli
-Version: 0.0.9
+Version: 0.1.0
 Summary: Make all DevOps experience better
 Home-page: https://github.com/kaonmir/dox-cli
 Author: kaonmir
 Author-email: sonjeff@naver.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dox-cli-0.0.9/dox_cli.egg-info/SOURCES.txt` & `dox_cli-0.1.0/dox_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dox-cli-0.0.9/setup.py` & `dox_cli-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="dox-cli",
-    version="0.0.9",  # TODO: 태그 걸면 배포되도록 수정
+    version="0.1.0",  # TODO: 태그 걸면 배포되도록 수정
     license="MIT",
     author="kaonmir",
     author_email="sonjeff@naver.com",
     description="Make all DevOps experience better",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kaonmir/dox-cli",
```

