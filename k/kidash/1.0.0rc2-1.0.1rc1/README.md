# Comparing `tmp/kidash-1.0.0rc2.tar.gz` & `tmp/kidash-1.0.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kidash-1.0.0rc2.tar", max compression
+gzip compressed data, was "kidash-1.0.1rc1.tar", max compression
```

## Comparing `kidash-1.0.0rc2.tar` & `kidash-1.0.1rc1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      340 2024-04-11 10:41:52.886116 kidash-1.0.0rc2/AUTHORS
--rw-r--r--   0        0        0    35147 2024-04-11 10:41:52.886116 kidash-1.0.0rc2/LICENSE
--rw-r--r--   0        0        0     2768 2024-04-11 10:41:52.886116 kidash-1.0.0rc2/NEWS
--rw-r--r--   0        0        0     2525 2024-04-11 10:41:52.886116 kidash-1.0.0rc2/README.md
--rw-r--r--   0        0        0      894 2024-04-11 10:41:52.886116 kidash-1.0.0rc2/kidash/__init__.py
--rw-r--r--   0        0        0       91 2024-04-11 10:41:52.886116 kidash-1.0.0rc2/kidash/_version.py
--rwxr-xr-x   0        0        0     4355 2024-04-11 10:41:52.886116 kidash-1.0.0rc2/kidash/bin/kidash.py
--rwxr-xr-x   0        0        0    59366 2024-04-11 10:41:52.886116 kidash-1.0.0rc2/kidash/kidash.py
--rw-r--r--   0        0        0     1307 2024-04-11 10:41:52.886116 kidash-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0    54328 2024-04-11 10:41:52.890117 kidash-1.0.0rc2/tests/data/overview-with-index-patterns.json
--rwxr-xr-x   0        0        0     1166 2024-04-11 10:41:52.890117 kidash-1.0.0rc2/tests/run_tests.py
--rw-r--r--   0        0        0     2131 2024-04-11 10:41:52.890117 kidash-1.0.0rc2/tests/test_export.py
--rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 kidash-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      340 2024-05-09 06:58:47.848566 kidash-1.0.1rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2024-05-09 06:58:47.848566 kidash-1.0.1rc1/LICENSE
+-rw-r--r--   0        0        0     2918 2024-05-09 06:58:47.848566 kidash-1.0.1rc1/NEWS
+-rw-r--r--   0        0        0     2525 2024-05-09 06:58:47.848566 kidash-1.0.1rc1/README.md
+-rw-r--r--   0        0        0      894 2024-05-09 06:58:47.848566 kidash-1.0.1rc1/kidash/__init__.py
+-rw-r--r--   0        0        0       91 2024-05-09 06:58:47.848566 kidash-1.0.1rc1/kidash/_version.py
+-rwxr-xr-x   0        0        0     4355 2024-05-09 06:58:47.848566 kidash-1.0.1rc1/kidash/bin/kidash.py
+-rwxr-xr-x   0        0        0    59366 2024-05-09 06:58:47.848566 kidash-1.0.1rc1/kidash/kidash.py
+-rw-r--r--   0        0        0     1307 2024-05-09 06:58:47.848566 kidash-1.0.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    54328 2024-05-09 06:58:47.852566 kidash-1.0.1rc1/tests/data/overview-with-index-patterns.json
+-rwxr-xr-x   0        0        0     1166 2024-05-09 06:58:47.852566 kidash-1.0.1rc1/tests/run_tests.py
+-rw-r--r--   0        0        0     2131 2024-05-09 06:58:47.852566 kidash-1.0.1rc1/tests/test_export.py
+-rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 kidash-1.0.1rc1/PKG-INFO
```

### Comparing `kidash-1.0.0rc2/LICENSE` & `kidash-1.0.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kidash-1.0.0rc2/NEWS` & `kidash-1.0.1rc1/NEWS`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Releases
 
+## kidash 1.0.0 - (2024-04-13)
+
+**New features:**
+
+ * First major release\
+   GrimoireLab reached a stable status. This is our first major release.
+
+
   ## kidash 0.6.9 - (2024-03-27)
   
   * Update Poetry's package dependencies
 
   ## kidash 0.6.8 - (2024-03-12)
   
   * Update Poetry's package dependencies
```

### Comparing `kidash-1.0.0rc2/README.md` & `kidash-1.0.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `kidash-1.0.0rc2/kidash/__init__.py` & `kidash-1.0.1rc1/kidash/__init__.py`

 * *Files identical despite different names*

### Comparing `kidash-1.0.0rc2/kidash/bin/kidash.py` & `kidash-1.0.1rc1/kidash/bin/kidash.py`

 * *Files identical despite different names*

### Comparing `kidash-1.0.0rc2/kidash/kidash.py` & `kidash-1.0.1rc1/kidash/kidash.py`

 * *Files identical despite different names*

### Comparing `kidash-1.0.0rc2/pyproject.toml` & `kidash-1.0.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kidash"
-version = "1.0.0-rc.2"
+version = "1.0.1-rc.1"
 description = "GrimoireLab script to manage Kibana dashboards from the command line"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `kidash-1.0.0rc2/tests/data/overview-with-index-patterns.json` & `kidash-1.0.1rc1/tests/data/overview-with-index-patterns.json`

 * *Files identical despite different names*

### Comparing `kidash-1.0.0rc2/tests/run_tests.py` & `kidash-1.0.1rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `kidash-1.0.0rc2/tests/test_export.py` & `kidash-1.0.1rc1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `kidash-1.0.0rc2/PKG-INFO` & `kidash-1.0.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kidash
-Version: 1.0.0rc2
+Version: 1.0.1rc1
 Summary: GrimoireLab script to manage Kibana dashboards from the command line
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

