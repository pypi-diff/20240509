# Comparing `tmp/kumparanian-1.0.5rc1.tar.gz` & `tmp/kumparanian-1.0.5rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kumparanian-1.0.5rc1.tar", max compression
+gzip compressed data, was "kumparanian-1.0.5rc2.tar", max compression
```

## Comparing `kumparanian-1.0.5rc1.tar` & `kumparanian-1.0.5rc2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1486 2024-05-07 14:10:12.509016 kumparanian-1.0.5rc1/LICENSE
--rw-r--r--   0        0        0     2626 2024-05-07 14:10:12.509300 kumparanian-1.0.5rc1/README.md
--rw-r--r--   0        0        0        0 2024-05-07 14:10:12.509834 kumparanian-1.0.5rc1/kumparanian/__init__.py
--rw-r--r--   0        0        0       30 2024-05-07 14:10:12.510074 kumparanian-1.0.5rc1/kumparanian/__main__.py
--rw-r--r--   0        0        0     3214 2024-05-07 14:10:12.510227 kumparanian-1.0.5rc1/kumparanian/cli.py
--rw-r--r--   0        0        0      666 2024-05-07 14:10:12.510450 kumparanian-1.0.5rc1/kumparanian/de/__init__.py
--rw-r--r--   0        0        0     2396 2024-05-07 14:10:12.510586 kumparanian-1.0.5rc1/kumparanian/de/dataset.py
--rw-r--r--   0        0        0     1480 2024-05-07 14:10:12.510724 kumparanian-1.0.5rc1/kumparanian/de/help_text.py
--rw-r--r--   0        0        0     5471 2024-05-07 14:10:12.510872 kumparanian-1.0.5rc1/kumparanian/de/submission.py
--rw-r--r--   0        0        0      435 2024-05-07 14:10:12.511045 kumparanian-1.0.5rc1/kumparanian/ds/__init__.py
--rw-r--r--   0        0        0      647 2024-05-07 14:10:12.511170 kumparanian-1.0.5rc1/kumparanian/ds/help_text.py
--rw-r--r--   0        0        0     2319 2024-05-07 14:10:12.511319 kumparanian-1.0.5rc1/kumparanian/ds/model.py
--rw-r--r--   0        0        0      505 2024-05-08 08:43:45.573993 kumparanian-1.0.5rc1/pyproject.toml
--rw-r--r--   0        0        0     3255 1970-01-01 00:00:00.000000 kumparanian-1.0.5rc1/PKG-INFO
+-rw-r--r--   0        0        0     1486 2024-05-07 14:10:12.509016 kumparanian-1.0.5rc2/LICENSE
+-rw-r--r--   0        0        0     2626 2024-05-07 14:10:12.509300 kumparanian-1.0.5rc2/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 14:10:12.509834 kumparanian-1.0.5rc2/kumparanian/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-07 14:10:12.510074 kumparanian-1.0.5rc2/kumparanian/__main__.py
+-rw-r--r--   0        0        0     3214 2024-05-07 14:10:12.510227 kumparanian-1.0.5rc2/kumparanian/cli.py
+-rw-r--r--   0        0        0      666 2024-05-07 14:10:12.510450 kumparanian-1.0.5rc2/kumparanian/de/__init__.py
+-rw-r--r--   0        0        0     2396 2024-05-07 14:10:12.510586 kumparanian-1.0.5rc2/kumparanian/de/dataset.py
+-rw-r--r--   0        0        0     1480 2024-05-07 14:10:12.510724 kumparanian-1.0.5rc2/kumparanian/de/help_text.py
+-rw-r--r--   0        0        0     5471 2024-05-07 14:10:12.510872 kumparanian-1.0.5rc2/kumparanian/de/submission.py
+-rw-r--r--   0        0        0      435 2024-05-07 14:10:12.511045 kumparanian-1.0.5rc2/kumparanian/ds/__init__.py
+-rw-r--r--   0        0        0      647 2024-05-07 14:10:12.511170 kumparanian-1.0.5rc2/kumparanian/ds/help_text.py
+-rw-r--r--   0        0        0     2319 2024-05-07 14:10:12.511319 kumparanian-1.0.5rc2/kumparanian/ds/model.py
+-rw-r--r--   0        0        0      504 2024-05-09 04:33:54.172361 kumparanian-1.0.5rc2/pyproject.toml
+-rw-r--r--   0        0        0     3255 1970-01-01 00:00:00.000000 kumparanian-1.0.5rc2/PKG-INFO
```

### Comparing `kumparanian-1.0.5rc1/LICENSE` & `kumparanian-1.0.5rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc1/README.md` & `kumparanian-1.0.5rc2/README.md`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc1/kumparanian/cli.py` & `kumparanian-1.0.5rc2/kumparanian/cli.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc1/kumparanian/de/__init__.py` & `kumparanian-1.0.5rc2/kumparanian/de/__init__.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc1/kumparanian/de/dataset.py` & `kumparanian-1.0.5rc2/kumparanian/de/dataset.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc1/kumparanian/de/help_text.py` & `kumparanian-1.0.5rc2/kumparanian/de/help_text.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc1/kumparanian/de/submission.py` & `kumparanian-1.0.5rc2/kumparanian/de/submission.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc1/kumparanian/ds/help_text.py` & `kumparanian-1.0.5rc2/kumparanian/ds/help_text.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc1/kumparanian/ds/model.py` & `kumparanian-1.0.5rc2/kumparanian/ds/model.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc1/PKG-INFO` & `kumparanian-1.0.5rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kumparanian
-Version: 1.0.5rc1
+Version: 1.0.5rc2
 Summary: 
 License: kumparan
 Author: Zavli Juwantara
 Author-email: zavli.juwantara@kumparan.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

