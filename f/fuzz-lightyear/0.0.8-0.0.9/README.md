# Comparing `tmp/fuzz_lightyear-0.0.8.tar.gz` & `tmp/fuzz_lightyear-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuzz_lightyear-0.0.8.tar", last modified: Mon Aug 17 17:30:09 2020, max compression
+gzip compressed data, was "dist/fuzz_lightyear-0.0.9.tar", last modified: Wed Aug 19 21:54:03 2020, max compression
```

## Comparing `fuzz_lightyear-0.0.8.tar` & `fuzz_lightyear-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 vzhou     (4633) users      (100)        0 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/
--rw-r--r--   0 vzhou     (4633) users      (100)     1693 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/setup.py
--rw-r--r--   0 vzhou     (4633) users      (100)    10739 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.8/README.md
--rw-r--r--   0 vzhou     (4633) users      (100)       38 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/setup.cfg
--rw-r--r--   0 vzhou     (4633) users      (100)      757 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/PKG-INFO
-drwxr-xr-x   0 vzhou     (4633) users      (100)        0 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/
--rw-r--r--   0 vzhou     (4633) users      (100)     4470 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/main.py
--rw-r--r--   0 vzhou     (4633) users      (100)       18 2020-08-17 17:28:24.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/version.py
--rw-r--r--   0 vzhou     (4633) users      (100)      571 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/result.py
--rw-r--r--   0 vzhou     (4633) users      (100)      671 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/util.py
-drwxr-xr-x   0 vzhou     (4633) users      (100)        0 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/
--rw-r--r--   0 vzhou     (4633) users      (100)     3767 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/exclude.py
--rw-r--r--   0 vzhou     (4633) users      (100)      584 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/setup.py
--rw-r--r--   0 vzhou     (4633) users      (100)     1113 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/auth.py
--rw-r--r--   0 vzhou     (4633) users      (100)      516 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/request.py
--rw-r--r--   0 vzhou     (4633) users      (100)      564 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/include.py
--rw-r--r--   0 vzhou     (4633) users      (100)      788 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/hooks.py
--rw-r--r--   0 vzhou     (4633) users      (100)     2951 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/factory.py
--rw-r--r--   0 vzhou     (4633) users      (100)        0 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/__init__.py
--rw-r--r--   0 vzhou     (4633) users      (100)     1583 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/abstraction.py
--rw-r--r--   0 vzhou     (4633) users      (100)    11974 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/request.py
--rw-r--r--   0 vzhou     (4633) users      (100)     1385 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/response.py
--rw-r--r--   0 vzhou     (4633) users      (100)      679 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/exceptions.py
--rw-r--r--   0 vzhou     (4633) users      (100)      621 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/settings.py
-drwxr-xr-x   0 vzhou     (4633) users      (100)        0 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/plugins/
--rw-r--r--   0 vzhou     (4633) users      (100)     1716 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/plugins/idor.py
--rw-r--r--   0 vzhou     (4633) users      (100)      621 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/plugins/__init__.py
--rw-r--r--   0 vzhou     (4633) users      (100)      485 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/plugins/base.py
--rw-r--r--   0 vzhou     (4633) users      (100)     6653 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/generator.py
--rw-r--r--   0 vzhou     (4633) users      (100)     7216 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/fuzzer.py
--rw-r--r--   0 vzhou     (4633) users      (100)     4174 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/usage.py
--rw-r--r--   0 vzhou     (4633) users      (100)       63 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/__main__.py
--rw-r--r--   0 vzhou     (4633) users      (100)     1531 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/runner.py
--rw-r--r--   0 vzhou     (4633) users      (100)      621 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/__init__.py
--rw-r--r--   0 vzhou     (4633) users      (100)     6894 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/datastore.py
--rw-r--r--   0 vzhou     (4633) users      (100)     1049 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/discovery.py
-drwxr-xr-x   0 vzhou     (4633) users      (100)        0 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/output/
--rw-r--r--   0 vzhou     (4633) users      (100)     2606 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/output/logging.py
--rw-r--r--   0 vzhou     (4633) users      (100)      448 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/output/util.py
--rw-r--r--   0 vzhou     (4633) users      (100)     5685 2020-08-17 16:54:26.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/output/formatter.py
--rw-r--r--   0 vzhou     (4633) users      (100)      463 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/output/color.py
--rw-r--r--   0 vzhou     (4633) users      (100)        0 2020-01-09 19:45:28.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/output/__init__.py
--rw-r--r--   0 vzhou     (4633) users      (100)     3496 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.8/fuzz_lightyear/output/interface.py
-drwxr-xr-x   0 vzhou     (4633) users      (100)        0 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/fuzz_lightyear.egg-info/
--rw-r--r--   0 vzhou     (4633) users      (100)       61 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/fuzz_lightyear.egg-info/entry_points.txt
--rw-r--r--   0 vzhou     (4633) users      (100)     1301 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/fuzz_lightyear.egg-info/SOURCES.txt
--rw-r--r--   0 vzhou     (4633) users      (100)      757 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/fuzz_lightyear.egg-info/PKG-INFO
--rw-r--r--   0 vzhou     (4633) users      (100)       50 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/fuzz_lightyear.egg-info/requires.txt
--rw-r--r--   0 vzhou     (4633) users      (100)       15 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/fuzz_lightyear.egg-info/top_level.txt
--rw-r--r--   0 vzhou     (4633) users      (100)        1 2020-08-17 17:30:09.000000 fuzz_lightyear-0.0.8/fuzz_lightyear.egg-info/dependency_links.txt
+drwxr-xr-x   0 vzhou     (4633) users      (100)        0 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/
+-rw-r--r--   0 vzhou     (4633) users      (100)     1693 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/setup.py
+-rw-r--r--   0 vzhou     (4633) users      (100)    10739 2020-07-29 17:10:39.000000 fuzz_lightyear-0.0.9/README.md
+-rw-r--r--   0 vzhou     (4633) users      (100)       38 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/setup.cfg
+-rw-r--r--   0 vzhou     (4633) users      (100)      757 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/PKG-INFO
+drwxr-xr-x   0 vzhou     (4633) users      (100)        0 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/
+-rw-r--r--   0 vzhou     (4633) users      (100)     4470 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/main.py
+-rw-r--r--   0 vzhou     (4633) users      (100)       18 2020-08-19 21:51:58.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/version.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      571 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/result.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      671 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/util.py
+drwxr-xr-x   0 vzhou     (4633) users      (100)        0 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/
+-rw-r--r--   0 vzhou     (4633) users      (100)     3767 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/exclude.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      584 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/setup.py
+-rw-r--r--   0 vzhou     (4633) users      (100)     1113 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/auth.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      516 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/request.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      564 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/include.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      788 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/hooks.py
+-rw-r--r--   0 vzhou     (4633) users      (100)     2951 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/factory.py
+-rw-r--r--   0 vzhou     (4633) users      (100)        0 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/__init__.py
+-rw-r--r--   0 vzhou     (4633) users      (100)     1583 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/abstraction.py
+-rw-r--r--   0 vzhou     (4633) users      (100)    11975 2020-08-19 17:27:55.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/request.py
+-rw-r--r--   0 vzhou     (4633) users      (100)     1385 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/response.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      679 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/exceptions.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      621 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/settings.py
+drwxr-xr-x   0 vzhou     (4633) users      (100)        0 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/plugins/
+-rw-r--r--   0 vzhou     (4633) users      (100)     1716 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/plugins/idor.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      621 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/plugins/__init__.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      485 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/plugins/base.py
+-rw-r--r--   0 vzhou     (4633) users      (100)     6653 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/generator.py
+-rw-r--r--   0 vzhou     (4633) users      (100)     7216 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/fuzzer.py
+-rw-r--r--   0 vzhou     (4633) users      (100)     4174 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/usage.py
+-rw-r--r--   0 vzhou     (4633) users      (100)       63 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/__main__.py
+-rw-r--r--   0 vzhou     (4633) users      (100)     1531 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/runner.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      621 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/__init__.py
+-rw-r--r--   0 vzhou     (4633) users      (100)     6894 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/datastore.py
+-rw-r--r--   0 vzhou     (4633) users      (100)     1049 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/discovery.py
+drwxr-xr-x   0 vzhou     (4633) users      (100)        0 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/output/
+-rw-r--r--   0 vzhou     (4633) users      (100)     2606 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/output/logging.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      448 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/output/util.py
+-rw-r--r--   0 vzhou     (4633) users      (100)     5685 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/output/formatter.py
+-rw-r--r--   0 vzhou     (4633) users      (100)      463 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/output/color.py
+-rw-r--r--   0 vzhou     (4633) users      (100)        0 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/output/__init__.py
+-rw-r--r--   0 vzhou     (4633) users      (100)     3496 2020-08-19 17:27:38.000000 fuzz_lightyear-0.0.9/fuzz_lightyear/output/interface.py
+drwxr-xr-x   0 vzhou     (4633) users      (100)        0 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/fuzz_lightyear.egg-info/
+-rw-r--r--   0 vzhou     (4633) users      (100)       61 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/fuzz_lightyear.egg-info/entry_points.txt
+-rw-r--r--   0 vzhou     (4633) users      (100)     1301 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/fuzz_lightyear.egg-info/SOURCES.txt
+-rw-r--r--   0 vzhou     (4633) users      (100)      757 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/fuzz_lightyear.egg-info/PKG-INFO
+-rw-r--r--   0 vzhou     (4633) users      (100)       50 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/fuzz_lightyear.egg-info/requires.txt
+-rw-r--r--   0 vzhou     (4633) users      (100)       15 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/fuzz_lightyear.egg-info/top_level.txt
+-rw-r--r--   0 vzhou     (4633) users      (100)        1 2020-08-19 21:54:03.000000 fuzz_lightyear-0.0.9/fuzz_lightyear.egg-info/dependency_links.txt
```

### Comparing `fuzz_lightyear-0.0.8/setup.py` & `fuzz_lightyear-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/README.md` & `fuzz_lightyear-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/PKG-INFO` & `fuzz_lightyear-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fuzz_lightyear
-Version: 0.0.8
+Version: 0.0.9
 Summary: Vulnerability Discovery through Stateful Swagger Fuzzing
 Home-page: UNKNOWN
 Author: Aaron Loo <aaronloo@yelp.com>, Joey Lee <joeylee@yelp.com>, Victor Zhou <vzhou@yelp.com>
 Author-email: UNKNOWN
 License: Copyright Yelp, Inc. 2019
 Description: UNKNOWN
 Keywords: fuzzer,security,swagger
```

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/main.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/main.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/result.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/result.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/util.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/util.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/exclude.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/exclude.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/setup.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/setup.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/auth.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/auth.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/request.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/request.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/include.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/include.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/hooks.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/hooks.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/factory.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/factory.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/supplements/abstraction.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/supplements/abstraction.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/request.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+import json
 from collections import defaultdict
 from functools import lru_cache
 from typing import Any
 from typing import Callable
 from typing import cast
 from typing import Dict
 from typing import List
 from typing import Optional
 from urllib.parse import quote_plus
 from urllib.parse import urlencode
-import json
 
 from bravado.client import CallableOperation
 from bravado_core.param import get_param_type_spec      # type: ignore
 from cached_property import cached_property             # type: ignore
 from hypothesis.strategies import SearchStrategy
 
 from .datastore import get_post_fuzz_hooks
@@ -134,15 +134,15 @@
         # it should not matter the specific session that we use).
         headers = data.get('header', {})
         headers.update(
             get_victim_session_factory()().get(
                 '_request_options', {},
             ).get(
                 'headers', {},
-            )
+            ),
         )
         for key, value in headers.items():
             args.append(f'-H \'{key}: {value}\'')
 
         return f'curl -X {data["method"]} {url} {" ".join(args)}'.rstrip()
 
     def send(
```

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/response.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/response.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/exceptions.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/exceptions.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/settings.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/settings.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/plugins/idor.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/plugins/idor.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/plugins/__init__.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/generator.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/generator.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/fuzzer.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/fuzzer.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/usage.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/usage.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/runner.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/runner.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/__init__.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/__init__.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/datastore.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/datastore.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/discovery.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/discovery.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/output/logging.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/output/logging.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/output/formatter.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/output/formatter.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear/output/interface.py` & `fuzz_lightyear-0.0.9/fuzz_lightyear/output/interface.py`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear.egg-info/SOURCES.txt` & `fuzz_lightyear-0.0.9/fuzz_lightyear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuzz_lightyear-0.0.8/fuzz_lightyear.egg-info/PKG-INFO` & `fuzz_lightyear-0.0.9/fuzz_lightyear.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: fuzz-lightyear
-Version: 0.0.8
+Version: 0.0.9
 Summary: Vulnerability Discovery through Stateful Swagger Fuzzing
 Home-page: UNKNOWN
 Author: Aaron Loo <aaronloo@yelp.com>, Joey Lee <joeylee@yelp.com>, Victor Zhou <vzhou@yelp.com>
 Author-email: UNKNOWN
 License: Copyright Yelp, Inc. 2019
 Description: UNKNOWN
 Keywords: fuzzer,security,swagger
```

