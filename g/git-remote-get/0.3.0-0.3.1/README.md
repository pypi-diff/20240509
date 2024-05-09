# Comparing `tmp/git_remote_get-0.3.0.tar.gz` & `tmp/git_remote_get-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_remote_get-0.3.0.tar", max compression
+gzip compressed data, was "git_remote_get-0.3.1.tar", max compression
```

## Comparing `git_remote_get-0.3.0.tar` & `git_remote_get-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1056 2024-03-14 08:22:01.722802 git_remote_get-0.3.0/LICENSE
--rw-r--r--   0        0        0     4040 2024-03-14 08:22:01.722802 git_remote_get-0.3.0/README.md
--rw-r--r--   0        0        0       68 2024-03-14 08:22:01.722802 git_remote_get-0.3.0/gget/__init__.py
--rw-r--r--   0        0        0       59 2024-03-14 08:22:01.722802 git_remote_get-0.3.0/gget/__main__.py
--rw-r--r--   0        0        0     1001 2024-03-14 08:22:01.722802 git_remote_get-0.3.0/gget/_get_remote_file.py
--rw-r--r--   0        0        0     2529 2024-03-14 08:22:01.722802 git_remote_get-0.3.0/gget/cli.py
--rw-r--r--   0        0        0      185 2024-03-14 08:22:01.726801 git_remote_get-0.3.0/gget/platform/__init__.py
--rw-r--r--   0        0        0      504 2024-03-14 08:22:01.726801 git_remote_get-0.3.0/gget/platform/_dirent.py
--rw-r--r--   0        0        0      399 2024-03-14 08:22:01.726801 git_remote_get-0.3.0/gget/platform/_get_provider.py
--rw-r--r--   0        0        0      203 2024-03-14 08:22:01.726801 git_remote_get-0.3.0/gget/platform/_provider.py
--rw-r--r--   0        0        0      196 2024-03-14 08:22:01.726801 git_remote_get-0.3.0/gget/platform/_repository.py
--rw-r--r--   0        0        0      165 2024-03-14 08:22:01.726801 git_remote_get-0.3.0/gget/platform/github/__init__.py
--rw-r--r--   0        0        0     2659 2024-03-14 08:22:01.726801 git_remote_get-0.3.0/gget/platform/github/_dirent.py
--rw-r--r--   0        0        0      599 2024-03-14 08:22:01.726801 git_remote_get-0.3.0/gget/platform/github/_provider.py
--rw-r--r--   0        0        0     1163 2024-03-14 08:22:01.726801 git_remote_get-0.3.0/gget/platform/github/_repository.py
--rw-r--r--   0        0        0       56 2024-03-14 08:22:01.726801 git_remote_get-0.3.0/gget/writer/__init__.py
--rw-r--r--   0        0        0     1048 2024-03-14 08:22:01.726801 git_remote_get-0.3.0/gget/writer/_writer.py
--rw-r--r--   0        0        0     1963 2024-03-14 08:22:01.726801 git_remote_get-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5367 1970-01-01 00:00:00.000000 git_remote_get-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4040 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/README.md
+-rw-r--r--   0        0        0       68 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/__main__.py
+-rw-r--r--   0        0        0     1001 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/_get_remote_file.py
+-rw-r--r--   0        0        0     2529 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/cli.py
+-rw-r--r--   0        0        0      185 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/platform/__init__.py
+-rw-r--r--   0        0        0      504 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/platform/_dirent.py
+-rw-r--r--   0        0        0      399 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/platform/_get_provider.py
+-rw-r--r--   0        0        0      203 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/platform/_provider.py
+-rw-r--r--   0        0        0      196 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/platform/_repository.py
+-rw-r--r--   0        0        0      165 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/platform/github/__init__.py
+-rw-r--r--   0        0        0     2659 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/platform/github/_dirent.py
+-rw-r--r--   0        0        0      575 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/platform/github/_provider.py
+-rw-r--r--   0        0        0     1163 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/platform/github/_repository.py
+-rw-r--r--   0        0        0       56 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/writer/__init__.py
+-rw-r--r--   0        0        0     1048 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/gget/writer/_writer.py
+-rw-r--r--   0        0        0     1963 2024-05-09 15:36:09.618472 git_remote_get-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5367 1970-01-01 00:00:00.000000 git_remote_get-0.3.1/PKG-INFO
```

### Comparing `git_remote_get-0.3.0/LICENSE` & `git_remote_get-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git_remote_get-0.3.0/README.md` & `git_remote_get-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `git_remote_get-0.3.0/gget/_get_remote_file.py` & `git_remote_get-0.3.1/gget/_get_remote_file.py`

 * *Files identical despite different names*

### Comparing `git_remote_get-0.3.0/gget/cli.py` & `git_remote_get-0.3.1/gget/cli.py`

 * *Files identical despite different names*

### Comparing `git_remote_get-0.3.0/gget/platform/github/_dirent.py` & `git_remote_get-0.3.1/gget/platform/github/_dirent.py`

 * *Files identical despite different names*

### Comparing `git_remote_get-0.3.0/gget/platform/github/_repository.py` & `git_remote_get-0.3.1/gget/platform/github/_repository.py`

 * *Files identical despite different names*

### Comparing `git_remote_get-0.3.0/gget/writer/_writer.py` & `git_remote_get-0.3.1/gget/writer/_writer.py`

 * *Files identical despite different names*

### Comparing `git_remote_get-0.3.0/pyproject.toml` & `git_remote_get-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "git-remote-get"
-version = "0.3.0"
+version = "0.3.1"
 description = "Download single files or directories from a git remote repository without cloning its entire contents."
 authors = ["01Joseph-Hwang10 <joseph95501@gmail.com>"]
 classifiers = [
   'Development Status :: 5 - Production/Stable',
   'Intended Audience :: Developers',
   'Natural Language :: English',
   'Topic :: Software Development',
```

### Comparing `git_remote_get-0.3.0/PKG-INFO` & `git_remote_get-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-remote-get
-Version: 0.3.0
+Version: 0.3.1
 Summary: Download single files or directories from a git remote repository without cloning its entire contents.
 License: MIT
 Author: 01Joseph-Hwang10
 Author-email: joseph95501@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

