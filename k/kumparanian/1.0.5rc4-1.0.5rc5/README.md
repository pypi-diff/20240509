# Comparing `tmp/kumparanian-1.0.5rc4.tar.gz` & `tmp/kumparanian-1.0.5rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kumparanian-1.0.5rc4.tar", max compression
+gzip compressed data, was "kumparanian-1.0.5rc5.tar", max compression
```

## Comparing `kumparanian-1.0.5rc4.tar` & `kumparanian-1.0.5rc5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1486 2024-05-07 14:10:12.509016 kumparanian-1.0.5rc4/LICENSE
--rw-r--r--   0        0        0     2626 2024-05-07 14:10:12.509300 kumparanian-1.0.5rc4/README.md
--rw-r--r--   0        0        0        0 2024-05-07 14:10:12.509834 kumparanian-1.0.5rc4/kumparanian/__init__.py
--rw-r--r--   0        0        0       30 2024-05-09 08:24:12.247895 kumparanian-1.0.5rc4/kumparanian/__main__.py
--rw-r--r--   0        0        0     3251 2024-05-09 09:04:31.086800 kumparanian-1.0.5rc4/kumparanian/cli.py
--rw-r--r--   0        0        0      666 2024-05-07 14:10:12.510450 kumparanian-1.0.5rc4/kumparanian/de/__init__.py
--rw-r--r--   0        0        0     2396 2024-05-07 14:10:12.510586 kumparanian-1.0.5rc4/kumparanian/de/dataset.py
--rw-r--r--   0        0        0     1480 2024-05-07 14:10:12.510724 kumparanian-1.0.5rc4/kumparanian/de/help_text.py
--rw-r--r--   0        0        0     5471 2024-05-07 14:10:12.510872 kumparanian-1.0.5rc4/kumparanian/de/submission.py
--rw-r--r--   0        0        0      435 2024-05-07 14:10:12.511045 kumparanian-1.0.5rc4/kumparanian/ds/__init__.py
--rw-r--r--   0        0        0      647 2024-05-07 14:10:12.511170 kumparanian-1.0.5rc4/kumparanian/ds/help_text.py
--rw-r--r--   0        0        0     2319 2024-05-07 14:10:12.511319 kumparanian-1.0.5rc4/kumparanian/ds/model.py
--rw-r--r--   0        0        0      619 2024-05-09 09:07:07.125257 kumparanian-1.0.5rc4/pyproject.toml
--rw-r--r--   0        0        0     3255 1970-01-01 00:00:00.000000 kumparanian-1.0.5rc4/PKG-INFO
+-rw-r--r--   0        0        0     1486 2024-05-07 14:10:12.509016 kumparanian-1.0.5rc5/LICENSE
+-rw-r--r--   0        0        0     2626 2024-05-07 14:10:12.509300 kumparanian-1.0.5rc5/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 14:10:12.509834 kumparanian-1.0.5rc5/kumparanian/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-09 08:24:12.247895 kumparanian-1.0.5rc5/kumparanian/__main__.py
+-rw-r--r--   0        0        0     3445 2024-05-09 09:25:49.458497 kumparanian-1.0.5rc5/kumparanian/cli.py
+-rw-r--r--   0        0        0      666 2024-05-07 14:10:12.510450 kumparanian-1.0.5rc5/kumparanian/de/__init__.py
+-rw-r--r--   0        0        0     2396 2024-05-07 14:10:12.510586 kumparanian-1.0.5rc5/kumparanian/de/dataset.py
+-rw-r--r--   0        0        0     1480 2024-05-07 14:10:12.510724 kumparanian-1.0.5rc5/kumparanian/de/help_text.py
+-rw-r--r--   0        0        0     5471 2024-05-07 14:10:12.510872 kumparanian-1.0.5rc5/kumparanian/de/submission.py
+-rw-r--r--   0        0        0      435 2024-05-07 14:10:12.511045 kumparanian-1.0.5rc5/kumparanian/ds/__init__.py
+-rw-r--r--   0        0        0      647 2024-05-07 14:10:12.511170 kumparanian-1.0.5rc5/kumparanian/ds/help_text.py
+-rw-r--r--   0        0        0     2319 2024-05-07 14:10:12.511319 kumparanian-1.0.5rc5/kumparanian/ds/model.py
+-rw-r--r--   0        0        0      619 2024-05-09 09:26:56.781469 kumparanian-1.0.5rc5/pyproject.toml
+-rw-r--r--   0        0        0     3255 1970-01-01 00:00:00.000000 kumparanian-1.0.5rc5/PKG-INFO
```

### Comparing `kumparanian-1.0.5rc4/LICENSE` & `kumparanian-1.0.5rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc4/README.md` & `kumparanian-1.0.5rc5/README.md`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc4/kumparanian/cli.py` & `kumparanian-1.0.5rc5/kumparanian/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import click
+import multiprocessing
 
 import kumparanian.ds as ds
 import kumparanian.de as de
 
 # Help texts
 epilog = ("If you found any issues, feel free report it at: "
           "https://github.com/kumparan/kumparanian/issues")
@@ -98,9 +99,13 @@
 def evaluate_submission(submission_dir, solution_dir):
     de.submission.evaluate(submission_dir, solution_dir)
 
 
 def main():
     cli()
 
+
 if __name__ == '__main__':
-    cli()
+    # handle "Error: No such option: --multiprocessing-fork"
+    # read more https://github.com/pyinstaller/pyinstaller/issues/2023
+    multiprocessing.freeze_support()
+    cli()
```

### Comparing `kumparanian-1.0.5rc4/kumparanian/de/__init__.py` & `kumparanian-1.0.5rc5/kumparanian/de/__init__.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc4/kumparanian/de/dataset.py` & `kumparanian-1.0.5rc5/kumparanian/de/dataset.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc4/kumparanian/de/help_text.py` & `kumparanian-1.0.5rc5/kumparanian/de/help_text.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc4/kumparanian/de/submission.py` & `kumparanian-1.0.5rc5/kumparanian/de/submission.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc4/kumparanian/ds/help_text.py` & `kumparanian-1.0.5rc5/kumparanian/ds/help_text.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc4/kumparanian/ds/model.py` & `kumparanian-1.0.5rc5/kumparanian/ds/model.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc4/pyproject.toml` & `kumparanian-1.0.5rc5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kumparanian"
-version = "1.0.5rc4"
+version = "1.0.5rc5"
 description = ""
 authors = ["Zavli Juwantara <zavli.juwantara@kumparan.com>"]
 license = "kumparan"
 readme = "README.md"
 packages = [
     { include = "kumparanian" },
     { include = "kumparanian/de" },
```

### Comparing `kumparanian-1.0.5rc4/PKG-INFO` & `kumparanian-1.0.5rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kumparanian
-Version: 1.0.5rc4
+Version: 1.0.5rc5
 Summary: 
 License: kumparan
 Author: Zavli Juwantara
 Author-email: zavli.juwantara@kumparan.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

