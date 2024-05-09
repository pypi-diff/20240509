# Comparing `tmp/coherent_build-0.5.0.tar.gz` & `tmp/coherent_build-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherent_build-0.5.0.tar", last modified: Wed May  8 12:58:36 2024, max compression
+gzip compressed data, was "coherent_build-0.6.0.tar", last modified: Thu May  9 19:59:35 2024, max compression
```

## Comparing `coherent_build-0.5.0.tar` & `coherent_build-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-08 12:58:34.967964 coherent_build-0.5.0/
--rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.5.0/README.md
--rw-r--r--   0 jaraco     (501) staff       (20)     5574 2024-05-08 12:57:14.008323 coherent_build-0.5.0/__init__.py
--rw-r--r--   0 jaraco     (501) staff       (20)     8550 2024-05-07 20:37:24.092828 coherent_build-0.5.0/__init__.py.orig
--rw-r--r--   0 jaraco     (501) staff       (20)      492 2024-05-08 12:56:54.105638 coherent_build-0.5.0/__main__.py
--rw-r--r--   0 jaraco     (501) staff       (20)     3232 2024-05-08 12:36:43.178900 coherent_build-0.5.0/discovery.py
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-08 12:58:34.968043 coherent_build-0.5.0/pyproject.toml
--rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.5.0/system.toml
--rw-r--r--   0        0        0      509 2024-05-08 12:58:36.669853 coherent_build-0.5.0/PKG-INFO
+drwxr-xr-x   0 jaraco     (501) staff       (20)        0 2024-05-09 19:59:33.401990 coherent_build-0.6.0/
+-rw-r--r--   0 jaraco     (501) staff       (20)       84 2024-05-05 14:27:21.911766 coherent_build-0.6.0/README.md
+-rw-r--r--   0 jaraco     (501) staff       (20)     5660 2024-05-09 19:51:56.014871 coherent_build-0.6.0/__init__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     8550 2024-05-07 20:37:24.092828 coherent_build-0.6.0/__init__.py.orig
+-rw-r--r--   0 jaraco     (501) staff       (20)      492 2024-05-09 19:24:41.199168 coherent_build-0.6.0/__main__.py
+-rw-r--r--   0 jaraco     (501) staff       (20)     4238 2024-05-09 19:58:21.109403 coherent_build-0.6.0/discovery.py
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-09 19:59:33.402047 coherent_build-0.6.0/pyproject.toml
+-rw-r--r--   0 jaraco     (501) staff       (20)       78 2024-05-02 15:12:07.306572 coherent_build-0.6.0/system.toml
+-rw-r--r--   0        0        0      611 2024-05-09 19:59:35.832361 coherent_build-0.6.0/PKG-INFO
```

### Comparing `coherent_build-0.5.0/__init__.py` & `coherent_build-0.6.0/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     'pip-run',
     'setuptools_scm',
     'build',
     'git-fame',
     'jaraco.context',
     'requests',
     'packaging',
+    'jaraco.functools',
 ]
 
 import functools
 import importlib.metadata
 import io
 import os
 import pathlib
@@ -163,21 +164,22 @@
         >>> md = Metadata.discover()
         """
         return cls(cls._discover_fields())
 
     @staticmethod
     def _discover_fields():
         yield 'Metadata-Version', '2.3'
-        yield 'Name', discovery.name_from_path()
+        yield 'Name', discovery.best_name()
         yield 'Version', discovery.version_from_vcs()
         yield 'Author-Email', discovery.author_from_vcs()
         yield 'Summary', discovery.summary_from_github()
         yield 'Requires-Python', discovery.python_requires_supported()
         for dep in discovery.read_deps():
             yield 'Requires-Dist', dep
+        yield 'Project-URL', f'Homepage, {discovery.source_url()}'
         yield from discovery.description_from_readme()
 
     @classmethod
     def from_sdist(cls):
         sdist_metadata = importlib.metadata.PathDistribution(pathlib.Path()).metadata
         return (sdist_metadata or None) and cls(sdist_metadata)
```

### Comparing `coherent_build-0.5.0/__init__.py.orig` & `coherent_build-0.6.0/__init__.py.orig`

 * *Files identical despite different names*

### Comparing `coherent_build-0.5.0/discovery.py` & `coherent_build-0.6.0/discovery.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,99 @@
 import contextlib
+import functools
 import json
 import pathlib
 import subprocess
 import types
 import mimetypes
+from collections.abc import Mapping
 
+import jaraco.functools
 import requests
 import setuptools_scm
 from jaraco.context import suppress
 from pip_run import scripts
 
 
 mimetypes.add_type('text/plain', '', strict=True)
 mimetypes.add_type('text/markdown', '.md', strict=True)
 mimetypes.add_type('text/x-rst', '.rst', strict=True)
 
 
+@suppress(subprocess.CalledProcessError)
+def name_from_vcs():
+    """
+    >>> name_from_vcs()
+    'coherent.build'
+    """
+    url = subprocess.check_output(
+        ['git', 'remote', 'get-url', 'origin'],
+        text=True,
+        encoding='utf-8',
+    )
+    _, _, tail = url.strip().rpartition('/')
+    return tail
+
+
 def name_from_path():
+    """
+    >>> name_from_vcs()
+    'coherent.build'
+    """
     return pathlib.Path('.').absolute().name
 
 
+def best_name():
+    """
+    Name is important, so if the name can't be inferred from the VCS,
+    use the path.
+    """
+    return name_from_vcs() or name_from_path()
+
+
 def version_from_vcs():
     return setuptools_scm.get_version()
 
 
+def none_as(replacement):
+    return lambda val: replacement if val is None else val
+
+
+@functools.lru_cache
+@jaraco.functools.apply(none_as({}))
 @suppress(subprocess.CalledProcessError)
+def repo_info() -> Mapping:
+    data = json.loads(
+        subprocess.check_output(
+            ['gh', 'repo', 'view', '--json', 'description,url'],
+            text=True,
+            encoding='utf-8',
+        )
+    )
+    return {k: v for k, v in data.items() if v}
+
+
 def summary_from_github():
     """
     Load the summary from GitHub.
 
     >>> summary_from_github()
     'A zero-config Python project build backend'
     """
-    return (
-        json.loads(
-            subprocess.check_output(
-                ['gh', 'repo', 'view', '--json', 'description'],
-                text=True,
-                encoding='utf-8',
-            )
-        )['description']
-        or None
-    )
+    return repo_info().get('description')
+
+
+def source_url():
+    """
+    Load the repo URL from GitHub.
+
+    >>> source_url()
+    'https://github.com/coherent-oss/coherent.build'
+    """
+    return repo_info().get('url')
 
 
 def python_requires_supported():
     """
     >>> python_requires_supported()
     '>= 3...'
     """
```

