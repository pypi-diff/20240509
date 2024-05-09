# Comparing `tmp/vonage_utils-1.1.1.tar.gz` & `tmp/vonage_utils-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vonage_utils-1.1.1.tar", last modified: Mon Apr 29 01:52:07 2024, max compression
+gzip compressed data, was "vonage_utils-1.1.2.tar", last modified: Thu May  9 15:01:58 2024, max compression
```

## Comparing `vonage_utils-1.1.1.tar` & `vonage_utils-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.637698 vonage_utils-1.1.1/
--rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-04-29 01:52:07.636161 vonage_utils-1.1.1/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      974 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/README.md
--rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/backend_shim.py
--rw-r--r--   0 mkahan     (503) staff       (20)      834 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/pyproject.toml
--rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-04-29 01:52:07.637780 vonage_utils-1.1.1/setup.cfg
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.621942 vonage_utils-1.1.1/src/
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.628138 vonage_utils-1.1.1/src/vonage_utils/
--rw-r--r--   0 mkahan     (503) staff       (20)      210 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/src/vonage_utils/__init__.py
--rw-r--r--   0 mkahan     (503) staff       (20)      325 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/src/vonage_utils/errors.py
--rw-r--r--   0 mkahan     (503) staff       (20)       70 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/src/vonage_utils/models.py
--rw-r--r--   0 mkahan     (503) staff       (20)      262 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/src/vonage_utils/types.py
--rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-04-29 01:52:06.000000 vonage_utils-1.1.1/src/vonage_utils/utils.py
-drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-04-29 01:52:07.634440 vonage_utils-1.1.1/src/vonage_utils.egg-info/
--rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-04-29 01:52:07.000000 vonage_utils-1.1.1/src/vonage_utils.egg-info/PKG-INFO
--rw-r--r--   0 mkahan     (503) staff       (20)      374 2024-04-29 01:52:07.000000 vonage_utils-1.1.1/src/vonage_utils.egg-info/SOURCES.txt
--rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-04-29 01:52:07.000000 vonage_utils-1.1.1/src/vonage_utils.egg-info/dependency_links.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       41 2024-04-29 01:52:07.000000 vonage_utils-1.1.1/src/vonage_utils.egg-info/requires.txt
--rw-r--r--   0 mkahan     (503) staff       (20)       13 2024-04-29 01:52:07.000000 vonage_utils-1.1.1/src/vonage_utils.egg-info/top_level.txt
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:58.774925 vonage_utils-1.1.2/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-05-09 15:01:58.773737 vonage_utils-1.1.2/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      974 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/README.md
+-rw-r--r--   0 mkahan     (503) staff       (20)      751 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/backend_shim.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      834 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/pyproject.toml
+-rw-r--r--   0 mkahan     (503) staff       (20)       38 2024-05-09 15:01:58.775230 vonage_utils-1.1.2/setup.cfg
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:58.763544 vonage_utils-1.1.2/src/
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:58.768099 vonage_utils-1.1.2/src/vonage_utils/
+-rw-r--r--   0 mkahan     (503) staff       (20)      210 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/src/vonage_utils/__init__.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      325 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/src/vonage_utils/errors.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      320 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/src/vonage_utils/models.py
+-rw-r--r--   0 mkahan     (503) staff       (20)      262 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/src/vonage_utils/types.py
+-rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/src/vonage_utils/utils.py
+drwxr-xr-x   0 mkahan     (503) staff       (20)        0 2024-05-09 15:01:58.772802 vonage_utils-1.1.2/src/vonage_utils.egg-info/
+-rw-r--r--   0 mkahan     (503) staff       (20)     1748 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/src/vonage_utils.egg-info/PKG-INFO
+-rw-r--r--   0 mkahan     (503) staff       (20)      374 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/src/vonage_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)        1 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/src/vonage_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       41 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/src/vonage_utils.egg-info/requires.txt
+-rw-r--r--   0 mkahan     (503) staff       (20)       13 2024-05-09 15:01:58.000000 vonage_utils-1.1.2/src/vonage_utils.egg-info/top_level.txt
```

### Comparing `vonage_utils-1.1.1/PKG-INFO` & `vonage_utils-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vonage-utils
-Version: 1.1.1
+Version: 1.1.2
 Summary: Utils package containing objects for use with Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: Homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vonage_utils-1.1.1/README.md` & `vonage_utils-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vonage_utils-1.1.1/backend_shim.py` & `vonage_utils-1.1.2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `vonage_utils-1.1.1/pyproject.toml` & `vonage_utils-1.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'vonage-utils'
-version = '1.1.1'
+version = '1.1.2'
 description = 'Utils package containing objects for use with Vonage APIs'
 readme = "README.md"
 authors = [{ name = "Vonage", email = "devrel@vonage.com" }]
 dependencies = ["typing_extensions>=4.9.0", "pydantic>=2.7.1"]
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python",
```

### Comparing `vonage_utils-1.1.1/src/vonage_utils/utils.py` & `vonage_utils-1.1.2/src/vonage_utils/utils.py`

 * *Files identical despite different names*

### Comparing `vonage_utils-1.1.1/src/vonage_utils.egg-info/PKG-INFO` & `vonage_utils-1.1.2/src/vonage_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vonage-utils
-Version: 1.1.1
+Version: 1.1.2
 Summary: Utils package containing objects for use with Vonage APIs
 Author-email: Vonage <devrel@vonage.com>
 Project-URL: Homepage, https://github.com/Vonage/vonage-python-sdk
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

