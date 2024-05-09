# Comparing `tmp/bap_elk_backends-0.5.2rc1.tar.gz` & `tmp/bap_elk_backends-0.5.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bap_elk_backends-0.5.2rc1.tar", max compression
+gzip compressed data, was "bap_elk_backends-0.5.3rc1.tar", max compression
```

## Comparing `bap_elk_backends-0.5.2rc1.tar` & `bap_elk_backends-0.5.3rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       86 2024-04-16 08:21:20.845715 bap_elk_backends-0.5.2rc1/AUTHORS
--rw-r--r--   0        0        0    35149 2024-04-16 08:21:20.845715 bap_elk_backends-0.5.2rc1/LICENSE
--rw-r--r--   0        0        0     3630 2024-04-16 08:21:20.845715 bap_elk_backends-0.5.2rc1/NEWS
--rw-r--r--   0        0        0     3060 2024-04-16 08:21:20.845715 bap_elk_backends-0.5.2rc1/README.md
--rw-r--r--   0        0        0        0 2024-04-16 08:21:20.845715 bap_elk_backends-0.5.2rc1/bap_elk_backends/__init__.py
--rw-r--r--   0        0        0       91 2024-04-16 08:21:20.845715 bap_elk_backends-0.5.2rc1/bap_elk_backends/_version.py
--rw-r--r--   0        0        0        0 2024-04-16 08:21:20.845715 bap_elk_backends-0.5.2rc1/bap_elk_backends/enriched/__init__.py
--rw-r--r--   0        0        0     8240 2024-04-16 08:21:20.845715 bap_elk_backends-0.5.2rc1/bap_elk_backends/enriched/pontoon.py
--rw-r--r--   0        0        0      925 2024-04-16 08:21:20.845715 bap_elk_backends-0.5.2rc1/bap_elk_backends/enriched/public_inbox.py
--rw-r--r--   0        0        0     4465 2024-04-16 08:21:20.845715 bap_elk_backends-0.5.2rc1/bap_elk_backends/enriched/topicbox.py
--rw-r--r--   0        0        0        0 2024-04-16 08:21:20.845715 bap_elk_backends-0.5.2rc1/bap_elk_backends/raw/__init__.py
--rw-r--r--   0        0        0     2251 2024-04-16 08:21:20.849716 bap_elk_backends-0.5.2rc1/bap_elk_backends/raw/pontoon.py
--rw-r--r--   0        0        0     2200 2024-04-16 08:21:20.849716 bap_elk_backends-0.5.2rc1/bap_elk_backends/raw/public_inbox.py
--rw-r--r--   0        0        0     1713 2024-04-16 08:21:20.849716 bap_elk_backends-0.5.2rc1/bap_elk_backends/raw/topicbox.py
--rw-r--r--   0        0        0     1552 2024-04-16 08:21:20.849716 bap_elk_backends-0.5.2rc1/bap_elk_backends/utils.py
--rw-r--r--   0        0        0     1678 2024-04-16 08:21:20.849716 bap_elk_backends-0.5.2rc1/pyproject.toml
--rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 bap_elk_backends-0.5.2rc1/PKG-INFO
+-rw-r--r--   0        0        0       86 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/AUTHORS
+-rw-r--r--   0        0        0    35149 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/LICENSE
+-rw-r--r--   0        0        0     3718 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/NEWS
+-rw-r--r--   0        0        0     3060 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/bap_elk_backends/__init__.py
+-rw-r--r--   0        0        0       91 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/bap_elk_backends/_version.py
+-rw-r--r--   0        0        0        0 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/bap_elk_backends/enriched/__init__.py
+-rw-r--r--   0        0        0     8240 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/bap_elk_backends/enriched/pontoon.py
+-rw-r--r--   0        0        0      925 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/bap_elk_backends/enriched/public_inbox.py
+-rw-r--r--   0        0        0     4465 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/bap_elk_backends/enriched/topicbox.py
+-rw-r--r--   0        0        0        0 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/bap_elk_backends/raw/__init__.py
+-rw-r--r--   0        0        0     2251 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/bap_elk_backends/raw/pontoon.py
+-rw-r--r--   0        0        0     2200 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/bap_elk_backends/raw/public_inbox.py
+-rw-r--r--   0        0        0     1713 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/bap_elk_backends/raw/topicbox.py
+-rw-r--r--   0        0        0     1552 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/bap_elk_backends/utils.py
+-rw-r--r--   0        0        0     1678 2024-05-09 12:44:28.378424 bap_elk_backends-0.5.3rc1/pyproject.toml
+-rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 bap_elk_backends-0.5.3rc1/PKG-INFO
```

### Comparing `bap_elk_backends-0.5.2rc1/LICENSE` & `bap_elk_backends-0.5.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `bap_elk_backends-0.5.2rc1/NEWS` & `bap_elk_backends-0.5.3rc1/NEWS`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Releases
 
+  ## bap-elk-backends 0.5.2 - (2024-04-16)
+  
+  * Update Poetry's package dependencies
+
   ## bap-elk-backends 0.5.1 - (2024-04-01)
   
   * Update Poetry's package dependencies
 
 ## bap-elk-backends 0.5.0 - (2024-03-12)
 
 **New features:**
```

### Comparing `bap_elk_backends-0.5.2rc1/README.md` & `bap_elk_backends-0.5.3rc1/README.md`

 * *Files identical despite different names*

### Comparing `bap_elk_backends-0.5.2rc1/bap_elk_backends/enriched/pontoon.py` & `bap_elk_backends-0.5.3rc1/bap_elk_backends/enriched/pontoon.py`

 * *Files identical despite different names*

### Comparing `bap_elk_backends-0.5.2rc1/bap_elk_backends/enriched/public_inbox.py` & `bap_elk_backends-0.5.3rc1/bap_elk_backends/enriched/public_inbox.py`

 * *Files identical despite different names*

### Comparing `bap_elk_backends-0.5.2rc1/bap_elk_backends/enriched/topicbox.py` & `bap_elk_backends-0.5.3rc1/bap_elk_backends/enriched/topicbox.py`

 * *Files identical despite different names*

### Comparing `bap_elk_backends-0.5.2rc1/bap_elk_backends/raw/pontoon.py` & `bap_elk_backends-0.5.3rc1/bap_elk_backends/raw/pontoon.py`

 * *Files identical despite different names*

### Comparing `bap_elk_backends-0.5.2rc1/bap_elk_backends/raw/public_inbox.py` & `bap_elk_backends-0.5.3rc1/bap_elk_backends/raw/public_inbox.py`

 * *Files identical despite different names*

### Comparing `bap_elk_backends-0.5.2rc1/bap_elk_backends/raw/topicbox.py` & `bap_elk_backends-0.5.3rc1/bap_elk_backends/raw/topicbox.py`

 * *Files identical despite different names*

### Comparing `bap_elk_backends-0.5.2rc1/bap_elk_backends/utils.py` & `bap_elk_backends-0.5.3rc1/bap_elk_backends/utils.py`

 * *Files identical despite different names*

### Comparing `bap_elk_backends-0.5.2rc1/pyproject.toml` & `bap_elk_backends-0.5.3rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bap-elk-backends"
-version = "0.5.2-rc.1"
+version = "0.5.3-rc.1"
 description = "GrimoireELK plugic for public-inbox."
 authors = [
     "Bitergia Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `bap_elk_backends-0.5.2rc1/PKG-INFO` & `bap_elk_backends-0.5.3rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bap-elk-backends
-Version: 0.5.2rc1
+Version: 0.5.3rc1
 Summary: GrimoireELK plugic for public-inbox.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: Bitergia Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

