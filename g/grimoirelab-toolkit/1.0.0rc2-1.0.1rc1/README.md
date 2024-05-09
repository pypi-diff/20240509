# Comparing `tmp/grimoirelab_toolkit-1.0.0rc2.tar.gz` & `tmp/grimoirelab_toolkit-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimoirelab_toolkit-1.0.0rc2.tar", max compression
+gzip compressed data, was "grimoirelab_toolkit-1.0.1rc1.tar", max compression
```

## Comparing `grimoirelab_toolkit-1.0.0rc2.tar` & `grimoirelab_toolkit-1.0.1rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      278 2024-04-09 16:06:54.514809 grimoirelab_toolkit-1.0.0rc2/AUTHORS
--rw-r--r--   0        0        0    35147 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0     2196 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/NEWS
--rw-r--r--   0        0        0     2091 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/README.md
--rw-r--r--   0        0        0     1011 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/grimoirelab_toolkit/__init__.py
--rw-r--r--   0        0        0       91 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/grimoirelab_toolkit/_version.py
--rw-r--r--   0        0        0     5606 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/grimoirelab_toolkit/datetime.py
--rw-r--r--   0        0        0     3846 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/grimoirelab_toolkit/introspect.py
--rw-r--r--   0        0        0     1383 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/grimoirelab_toolkit/uris.py
--rw-r--r--   0        0        0     1132 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/pyproject.toml
--rwxr-xr-x   0        0        0     1063 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/tests/run_tests.py
--rw-r--r--   0        0        0    10186 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/tests/test_datetime.py
--rw-r--r--   0        0        0     7078 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/tests/test_introspect.py
--rw-r--r--   0        0        0     2678 2024-04-09 16:06:54.518809 grimoirelab_toolkit-1.0.0rc2/tests/test_uris.py
--rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 grimoirelab_toolkit-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      278 2024-05-09 07:53:38.669771 grimoirelab_toolkit-1.0.1rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-05-09 07:53:38.669771 grimoirelab_toolkit-1.0.1rc1/LICENSE
+-rw-r--r--   0        0        0     2359 2024-05-09 07:53:38.669771 grimoirelab_toolkit-1.0.1rc1/NEWS
+-rw-r--r--   0        0        0     2091 2024-05-09 07:53:38.669771 grimoirelab_toolkit-1.0.1rc1/README.md
+-rw-r--r--   0        0        0     1011 2024-05-09 07:53:38.669771 grimoirelab_toolkit-1.0.1rc1/grimoirelab_toolkit/__init__.py
+-rw-r--r--   0        0        0       91 2024-05-09 07:53:38.669771 grimoirelab_toolkit-1.0.1rc1/grimoirelab_toolkit/_version.py
+-rw-r--r--   0        0        0     5606 2024-05-09 07:53:38.673771 grimoirelab_toolkit-1.0.1rc1/grimoirelab_toolkit/datetime.py
+-rw-r--r--   0        0        0     3846 2024-05-09 07:53:38.673771 grimoirelab_toolkit-1.0.1rc1/grimoirelab_toolkit/introspect.py
+-rw-r--r--   0        0        0     1383 2024-05-09 07:53:38.673771 grimoirelab_toolkit-1.0.1rc1/grimoirelab_toolkit/uris.py
+-rw-r--r--   0        0        0     1132 2024-05-09 07:53:38.673771 grimoirelab_toolkit-1.0.1rc1/pyproject.toml
+-rwxr-xr-x   0        0        0     1063 2024-05-09 07:53:38.673771 grimoirelab_toolkit-1.0.1rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    10186 2024-05-09 07:53:38.673771 grimoirelab_toolkit-1.0.1rc1/tests/test_datetime.py
+-rw-r--r--   0        0        0     7078 2024-05-09 07:53:38.673771 grimoirelab_toolkit-1.0.1rc1/tests/test_introspect.py
+-rw-r--r--   0        0        0     2678 2024-05-09 07:53:38.673771 grimoirelab_toolkit-1.0.1rc1/tests/test_uris.py
+-rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 grimoirelab_toolkit-1.0.1rc1/PKG-INFO
```

### Comparing `grimoirelab_toolkit-1.0.0rc2/LICENSE` & `grimoirelab_toolkit-1.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-1.0.0rc2/NEWS` & `grimoirelab_toolkit-1.0.1rc1/NEWS`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Releases
 
+## grimoirelab-toolkit 1.0.0 - (2024-04-13)
+
+**New features:**
+
+ * First major release\
+   GrimoireLab reached a stable status. This is our first major release.
+
+
 ## grimoirelab-toolkit 1.0.0-rc.1 - (2024-04-09)
 
 **New features:**
 
  * First major release\
    GrimoireLab reached a stable status. This is our first major release.
```

### Comparing `grimoirelab_toolkit-1.0.0rc2/README.md` & `grimoirelab_toolkit-1.0.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-1.0.0rc2/grimoirelab_toolkit/__init__.py` & `grimoirelab_toolkit-1.0.1rc1/grimoirelab_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-1.0.0rc2/grimoirelab_toolkit/datetime.py` & `grimoirelab_toolkit-1.0.1rc1/grimoirelab_toolkit/datetime.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-1.0.0rc2/grimoirelab_toolkit/introspect.py` & `grimoirelab_toolkit-1.0.1rc1/grimoirelab_toolkit/introspect.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-1.0.0rc2/grimoirelab_toolkit/uris.py` & `grimoirelab_toolkit-1.0.1rc1/grimoirelab_toolkit/uris.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-1.0.0rc2/pyproject.toml` & `grimoirelab_toolkit-1.0.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grimoirelab-toolkit"
-version = "1.0.0-rc.2"
+version = "1.0.1-rc.1"
 description = "Toolkit of common functions used across GrimoireLab"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `grimoirelab_toolkit-1.0.0rc2/tests/run_tests.py` & `grimoirelab_toolkit-1.0.1rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-1.0.0rc2/tests/test_datetime.py` & `grimoirelab_toolkit-1.0.1rc1/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-1.0.0rc2/tests/test_introspect.py` & `grimoirelab_toolkit-1.0.1rc1/tests/test_introspect.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-1.0.0rc2/tests/test_uris.py` & `grimoirelab_toolkit-1.0.1rc1/tests/test_uris.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-1.0.0rc2/PKG-INFO` & `grimoirelab_toolkit-1.0.1rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoirelab-toolkit
-Version: 1.0.0rc2
+Version: 1.0.1rc1
 Summary: Toolkit of common functions used across GrimoireLab
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

