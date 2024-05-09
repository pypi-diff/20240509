# Comparing `tmp/telicent_label_builder-0.0.0.tar.gz` & `tmp/telicent_label_builder-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telicent_label_builder-0.0.0.tar", last modified: Thu May  9 07:51:08 2024, max compression
+gzip compressed data, was "telicent_label_builder-0.1.0.tar", last modified: Thu May  9 08:25:15 2024, max compression
```

## Comparing `telicent_label_builder-0.0.0.tar` & `telicent_label_builder-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:51:08.344917 telicent_label_builder-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-09 07:50:59.000000 telicent_label_builder-0.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-09 07:50:59.000000 telicent_label_builder-0.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-05-09 07:51:08.344917 telicent_label_builder-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-09 07:50:59.000000 telicent_label_builder-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-09 07:50:59.000000 telicent_label_builder-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 07:51:08.344917 telicent_label_builder-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:51:08.344917 telicent_label_builder-0.0.0/telicent_label_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-05-09 07:51:08.000000 telicent_label_builder-0.0.0/telicent_label_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-09 07:51:08.000000 telicent_label_builder-0.0.0/telicent_label_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:51:08.000000 telicent_label_builder-0.0.0/telicent_label_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 07:51:08.000000 telicent_label_builder-0.0.0/telicent_label_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 07:51:08.000000 telicent_label_builder-0.0.0/telicent_label_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:51:08.344917 telicent_label_builder-0.0.0/telicent_labels/
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 07:50:59.000000 telicent_label_builder-0.0.0/telicent_labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-09 07:50:59.000000 telicent_label_builder-0.0.0/telicent_labels/security_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-09 07:50:59.000000 telicent_label_builder-0.0.0/telicent_labels/telicent_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-09 07:50:59.000000 telicent_label_builder-0.0.0/telicent_labels/telicentv1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-09 07:50:59.000000 telicent_label_builder-0.0.0/telicent_labels/telicentv2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:51:08.344917 telicent_label_builder-0.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-09 07:50:59.000000 telicent_label_builder-0.0.0/test/test_security_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-09 07:50:59.000000 telicent_label_builder-0.0.0/test/test_security_labels_edhv1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:25:15.083534 telicent_label_builder-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-09 08:25:09.000000 telicent_label_builder-0.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-09 08:25:09.000000 telicent_label_builder-0.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-05-09 08:25:15.083534 telicent_label_builder-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-09 08:25:09.000000 telicent_label_builder-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-09 08:25:09.000000 telicent_label_builder-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:25:15.087534 telicent_label_builder-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:25:15.083534 telicent_label_builder-0.1.0/telicent_label_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2024-05-09 08:25:15.000000 telicent_label_builder-0.1.0/telicent_label_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-09 08:25:15.000000 telicent_label_builder-0.1.0/telicent_label_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:25:15.000000 telicent_label_builder-0.1.0/telicent_label_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 08:25:15.000000 telicent_label_builder-0.1.0/telicent_label_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 08:25:15.000000 telicent_label_builder-0.1.0/telicent_label_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:25:15.083534 telicent_label_builder-0.1.0/telicent_labels/
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 08:25:09.000000 telicent_label_builder-0.1.0/telicent_labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-09 08:25:09.000000 telicent_label_builder-0.1.0/telicent_labels/security_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-09 08:25:09.000000 telicent_label_builder-0.1.0/telicent_labels/telicent_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-09 08:25:09.000000 telicent_label_builder-0.1.0/telicent_labels/telicentv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-09 08:25:09.000000 telicent_label_builder-0.1.0/telicent_labels/telicentv2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:25:15.083534 telicent_label_builder-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-09 08:25:09.000000 telicent_label_builder-0.1.0/test/test_security_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-09 08:25:09.000000 telicent_label_builder-0.1.0/test/test_security_labels_edhv1.py
```

### Comparing `telicent_label_builder-0.0.0/LICENSE.md` & `telicent_label_builder-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `telicent_label_builder-0.0.0/PKG-INFO` & `telicent_label_builder-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telicent-label-builder
-Version: 0.0.0
+Version: 0.1.0
 Summary: A helper package for creating and building security labels for telicent-lib
 Author-email: Telicent Ltd <admin@telicent.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `telicent_label_builder-0.0.0/pyproject.toml` & `telicent_label_builder-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2.0", "wheel==0.41.3", "pip-tools==7.3.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "telicent-label-builder"
-version = "0.0.0"
+version = "0.1.0"
 authors = [{name = "Telicent Ltd", email = "admin@telicent.io"}]
 description = "A helper package for creating and building security labels for telicent-lib"
 requires-python = ">=3.10"
 license = {file = "LICENSE.md"}
 readme = "README.md"
 dependencies = [
     "pydantic"
```

### Comparing `telicent_label_builder-0.0.0/telicent_label_builder.egg-info/PKG-INFO` & `telicent_label_builder-0.1.0/telicent_label_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telicent-label-builder
-Version: 0.0.0
+Version: 0.1.0
 Summary: A helper package for creating and building security labels for telicent-lib
 Author-email: Telicent Ltd <admin@telicent.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `telicent_label_builder-0.0.0/telicent_labels/__init__.py` & `telicent_label_builder-0.1.0/telicent_labels/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_label_builder-0.0.0/telicent_labels/security_labels.py` & `telicent_label_builder-0.1.0/telicent_labels/security_labels.py`

 * *Files identical despite different names*

### Comparing `telicent_label_builder-0.0.0/telicent_labels/telicent_model.py` & `telicent_label_builder-0.1.0/telicent_labels/telicent_model.py`

 * *Files identical despite different names*

### Comparing `telicent_label_builder-0.0.0/telicent_labels/telicentv1.py` & `telicent_label_builder-0.1.0/telicent_labels/telicentv1.py`

 * *Files identical despite different names*

### Comparing `telicent_label_builder-0.0.0/telicent_labels/telicentv2.py` & `telicent_label_builder-0.1.0/telicent_labels/telicentv2.py`

 * *Files identical despite different names*

### Comparing `telicent_label_builder-0.0.0/test/test_security_labels.py` & `telicent_label_builder-0.1.0/test/test_security_labels.py`

 * *Files identical despite different names*

### Comparing `telicent_label_builder-0.0.0/test/test_security_labels_edhv1.py` & `telicent_label_builder-0.1.0/test/test_security_labels_edhv1.py`

 * *Files identical despite different names*

