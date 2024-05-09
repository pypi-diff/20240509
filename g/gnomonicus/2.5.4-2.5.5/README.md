# Comparing `tmp/gnomonicus-2.5.4.tar.gz` & `tmp/gnomonicus-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gnomonicus-2.5.4.tar", last modified: Thu May  9 07:41:49 2024, max compression
+gzip compressed data, was "gnomonicus-2.5.5.tar", last modified: Thu May  9 09:34:18 2024, max compression
```

## Comparing `gnomonicus-2.5.4.tar` & `gnomonicus-2.5.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:41:49.859773 gnomonicus-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-09 07:41:49.859773 gnomonicus-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:41:49.855774 gnomonicus-2.5.4/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/bin/gbkToPkl
--rwxr-xr-x   0 runner    (1001) docker     (127)    10910 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/bin/gnomonicus
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/bin/gnomonicus-table-update
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:41:49.859773 gnomonicus-2.5.4/gnomonicus/
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/gnomonicus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79237 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/gnomonicus/gnomonicus_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:41:49.859773 gnomonicus-2.5.4/gnomonicus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-09 07:41:49.000000 gnomonicus-2.5.4/gnomonicus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-09 07:41:49.000000 gnomonicus-2.5.4/gnomonicus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:41:49.000000 gnomonicus-2.5.4/gnomonicus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:41:09.000000 gnomonicus-2.5.4/gnomonicus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 07:41:49.000000 gnomonicus-2.5.4/gnomonicus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 07:41:49.000000 gnomonicus-2.5.4/gnomonicus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-09 07:41:05.000000 gnomonicus-2.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-09 07:41:49.859773 gnomonicus-2.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:34:18.826356 gnomonicus-2.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-09 09:33:33.000000 gnomonicus-2.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-09 09:34:18.822356 gnomonicus-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-09 09:33:33.000000 gnomonicus-2.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:34:18.822356 gnomonicus-2.5.5/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-09 09:33:33.000000 gnomonicus-2.5.5/bin/gbkToPkl
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10910 2024-05-09 09:33:33.000000 gnomonicus-2.5.5/bin/gnomonicus
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-09 09:33:33.000000 gnomonicus-2.5.5/bin/gnomonicus-table-update
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:34:18.822356 gnomonicus-2.5.5/gnomonicus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-09 09:33:33.000000 gnomonicus-2.5.5/gnomonicus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79237 2024-05-09 09:33:33.000000 gnomonicus-2.5.5/gnomonicus/gnomonicus_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:34:18.822356 gnomonicus-2.5.5/gnomonicus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2024-05-09 09:34:18.000000 gnomonicus-2.5.5/gnomonicus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-09 09:34:18.000000 gnomonicus-2.5.5/gnomonicus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:34:18.000000 gnomonicus-2.5.5/gnomonicus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:33:38.000000 gnomonicus-2.5.5/gnomonicus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 09:34:18.000000 gnomonicus-2.5.5/gnomonicus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 09:34:18.000000 gnomonicus-2.5.5/gnomonicus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-09 09:33:33.000000 gnomonicus-2.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-09 09:34:18.826356 gnomonicus-2.5.5/setup.cfg
```

### Comparing `gnomonicus-2.5.4/LICENSE` & `gnomonicus-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.4/PKG-INFO` & `gnomonicus-2.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnomonicus
-Version: 2.5.4
+Version: 2.5.5
 Summary: Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
 Home-page: https://github.com/oxfordmmm/gnomonicus
 Author: Philip W Fowler, Jeremy Westhead
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford License, see LICENSE
 Keywords: gnomonicus,piezo,lodestone,clockwork,TB
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gnomonicus-2.5.4/README.md` & `gnomonicus-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.4/bin/gbkToPkl` & `gnomonicus-2.5.5/bin/gbkToPkl`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.4/bin/gnomonicus` & `gnomonicus-2.5.5/bin/gnomonicus`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.4/bin/gnomonicus-table-update` & `gnomonicus-2.5.5/bin/gnomonicus-table-update`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.4/gnomonicus/__init__.py` & `gnomonicus-2.5.5/gnomonicus/__init__.py`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.4/gnomonicus/gnomonicus_lib.py` & `gnomonicus-2.5.5/gnomonicus/gnomonicus_lib.py`

 * *Files identical despite different names*

### Comparing `gnomonicus-2.5.4/gnomonicus.egg-info/PKG-INFO` & `gnomonicus-2.5.5/gnomonicus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gnomonicus
-Version: 2.5.4
+Version: 2.5.5
 Summary: Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
 Home-page: https://github.com/oxfordmmm/gnomonicus
 Author: Philip W Fowler, Jeremy Westhead
 Author-email: philip.fowler@ndm.ox.ac.uk
 License: University of Oxford License, see LICENSE
 Keywords: gnomonicus,piezo,lodestone,clockwork,TB
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gnomonicus-2.5.4/setup.cfg` & `gnomonicus-2.5.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gnomonicus
-version = 2.5.4
+version = 2.5.5
 author = Philip W Fowler, Jeremy Westhead
 author_email = philip.fowler@ndm.ox.ac.uk
 description = Python code to integrate results of tb-pipeline and provide an antibiogram, mutations and variants
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/oxfordmmm/gnomonicus
 keywords = gnomonicus, piezo, lodestone, clockwork, TB
```

