# Comparing `tmp/domaintools_api_v2-2.0.0.tar.gz` & `tmp/domaintools_api_v2-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domaintools_api_v2-2.0.0.tar", last modified: Mon Apr 29 18:15:06 2024, max compression
+gzip compressed data, was "domaintools_api_v2-2.0.1.tar", last modified: Thu May  9 16:27:06 2024, max compression
```

## Comparing `domaintools_api_v2-2.0.0.tar` & `domaintools_api_v2-2.0.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-04-29 18:15:06.483635 domaintools_api_v2-2.0.0/
--rw-r--r--   0 bluza      (502) staff       (20)     1078 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.0/LICENSE
--rw-r--r--   0 bluza      (502) staff       (20)     9691 2024-04-29 18:15:06.483449 domaintools_api_v2-2.0.0/PKG-INFO
--rw-r--r--   0 bluza      (502) staff       (20)     7230 2024-03-04 18:03:36.000000 domaintools_api_v2-2.0.0/README.md
--rw-r--r--   0 bluza      (502) staff       (20)        5 2024-04-16 18:45:50.000000 domaintools_api_v2-2.0.0/VERSION
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-04-29 18:15:06.473934 domaintools_api_v2-2.0.0/domaintools/
--rw-r--r--   0 bluza      (502) staff       (20)      135 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.0/domaintools/__init__.py
--rw-r--r--   0 bluza      (502) staff       (20)     1181 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.0/domaintools/_version.py
--rw-r--r--   0 bluza      (502) staff       (20)    40580 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.0/domaintools/api.py
--rw-r--r--   0 bluza      (502) staff       (20)     8893 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.0/domaintools/base_results.py
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-04-29 18:15:06.475716 domaintools_api_v2-2.0.0/domaintools/cli/
--rw-r--r--   0 bluza      (502) staff       (20)      141 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.0/domaintools/cli/__init__.py
--rw-r--r--   0 bluza      (502) staff       (20)     7819 2024-04-18 16:48:06.000000 domaintools_api_v2-2.0.0/domaintools/cli/api.py
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-04-29 18:15:06.478341 domaintools_api_v2-2.0.0/domaintools/cli/commands/
--rw-r--r--   0 bluza      (502) staff       (20)      133 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.0/domaintools/cli/commands/__init__.py
--rw-r--r--   0 bluza      (502) staff       (20)     2823 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.0/domaintools/cli/commands/accounts.py
--rw-r--r--   0 bluza      (502) staff       (20)    18505 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.0/domaintools/cli/commands/detects.py
--rw-r--r--   0 bluza      (502) staff       (20)    23368 2024-04-29 16:18:47.000000 domaintools_api_v2-2.0.0/domaintools/cli/commands/domains.py
--rw-r--r--   0 bluza      (502) staff       (20)     6835 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.0/domaintools/cli/commands/ips.py
--rw-r--r--   0 bluza      (502) staff       (20)     6452 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.0/domaintools/cli/commands/iris.py
--rw-r--r--   0 bluza      (502) staff       (20)     3315 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.0/domaintools/cli/commands/phisheye.py
--rw-r--r--   0 bluza      (502) staff       (20)     1266 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.0/domaintools/cli/constants.py
--rw-r--r--   0 bluza      (502) staff       (20)      519 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.0/domaintools/cli/main.py
--rw-r--r--   0 bluza      (502) staff       (20)     6050 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.0/domaintools/cli/utils.py
--rw-r--r--   0 bluza      (502) staff       (20)      687 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.0/domaintools/exceptions.py
--rw-r--r--   0 bluza      (502) staff       (20)     3674 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.0/domaintools/results.py
--rw-r--r--   0 bluza      (502) staff       (20)     5619 2024-04-29 17:05:33.000000 domaintools_api_v2-2.0.0/domaintools/utils.py
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-04-29 18:15:06.482750 domaintools_api_v2-2.0.0/domaintools_api_v2.egg-info/
--rw-r--r--   0 bluza      (502) staff       (20)     9691 2024-04-29 18:15:06.000000 domaintools_api_v2-2.0.0/domaintools_api_v2.egg-info/PKG-INFO
--rw-r--r--   0 bluza      (502) staff       (20)      961 2024-04-29 18:15:06.000000 domaintools_api_v2-2.0.0/domaintools_api_v2.egg-info/SOURCES.txt
--rw-r--r--   0 bluza      (502) staff       (20)        1 2024-04-29 18:15:06.000000 domaintools_api_v2-2.0.0/domaintools_api_v2.egg-info/dependency_links.txt
--rw-r--r--   0 bluza      (502) staff       (20)       52 2024-04-29 18:15:06.000000 domaintools_api_v2-2.0.0/domaintools_api_v2.egg-info/entry_points.txt
--rw-r--r--   0 bluza      (502) staff       (20)       37 2024-04-29 18:15:06.000000 domaintools_api_v2-2.0.0/domaintools_api_v2.egg-info/requires.txt
--rw-r--r--   0 bluza      (502) staff       (20)       30 2024-04-29 18:15:06.000000 domaintools_api_v2-2.0.0/domaintools_api_v2.egg-info/top_level.txt
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-04-29 18:15:06.480412 domaintools_api_v2-2.0.0/domaintools_async/
--rw-r--r--   0 bluza      (502) staff       (20)     3015 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.0/domaintools_async/__init__.py
--rw-r--r--   0 bluza      (502) staff       (20)     1453 2024-04-29 18:14:49.000000 domaintools_api_v2-2.0.0/pyproject.toml
--rw-r--r--   0 bluza      (502) staff       (20)      172 2024-04-29 18:15:06.483957 domaintools_api_v2-2.0.0/setup.cfg
--rwxr-xr-x   0 bluza      (502) staff       (20)     1541 2024-04-11 04:41:30.000000 domaintools_api_v2-2.0.0/setup.py
-drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-04-29 18:15:06.481770 domaintools_api_v2-2.0.0/tests/
--rw-r--r--   0 bluza      (502) staff       (20)    15279 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.0/tests/test_api.py
--rw-r--r--   0 bluza      (502) staff       (20)     1760 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.0/tests/test_async.py
--rw-r--r--   0 bluza      (502) staff       (20)     1045 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.0/tests/test_cli.py
--rw-r--r--   0 bluza      (502) staff       (20)     4055 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.547258 domaintools_api_v2-2.0.1/
+-rw-r--r--   0 bluza      (502) staff       (20)     1078 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/LICENSE
+-rw-r--r--   0 bluza      (502) staff       (20)     9691 2024-05-09 16:27:06.547105 domaintools_api_v2-2.0.1/PKG-INFO
+-rw-r--r--   0 bluza      (502) staff       (20)     7230 2024-03-04 18:03:36.000000 domaintools_api_v2-2.0.1/README.md
+-rw-r--r--   0 bluza      (502) staff       (20)        5 2024-05-09 16:24:56.000000 domaintools_api_v2-2.0.1/VERSION
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.536625 domaintools_api_v2-2.0.1/domaintools/
+-rw-r--r--   0 bluza      (502) staff       (20)      135 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1181 2024-05-09 16:26:19.000000 domaintools_api_v2-2.0.1/domaintools/_version.py
+-rw-r--r--   0 bluza      (502) staff       (20)    43189 2024-05-07 11:17:06.000000 domaintools_api_v2-2.0.1/domaintools/api.py
+-rw-r--r--   0 bluza      (502) staff       (20)     8893 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/domaintools/base_results.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.538453 domaintools_api_v2-2.0.1/domaintools/cli/
+-rw-r--r--   0 bluza      (502) staff       (20)      141 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     7819 2024-05-02 12:32:44.000000 domaintools_api_v2-2.0.1/domaintools/cli/api.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.541683 domaintools_api_v2-2.0.1/domaintools/cli/commands/
+-rw-r--r--   0 bluza      (502) staff       (20)      133 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     2823 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/accounts.py
+-rw-r--r--   0 bluza      (502) staff       (20)    18505 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/detects.py
+-rw-r--r--   0 bluza      (502) staff       (20)    23368 2024-04-29 16:18:47.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/domains.py
+-rw-r--r--   0 bluza      (502) staff       (20)     6835 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/ips.py
+-rw-r--r--   0 bluza      (502) staff       (20)     6452 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/iris.py
+-rw-r--r--   0 bluza      (502) staff       (20)     3315 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/commands/phisheye.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1266 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/constants.py
+-rw-r--r--   0 bluza      (502) staff       (20)      519 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/domaintools/cli/main.py
+-rw-r--r--   0 bluza      (502) staff       (20)     6050 2024-04-16 17:13:01.000000 domaintools_api_v2-2.0.1/domaintools/cli/utils.py
+-rw-r--r--   0 bluza      (502) staff       (20)      687 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/domaintools/exceptions.py
+-rw-r--r--   0 bluza      (502) staff       (20)     5216 2024-05-07 12:07:39.000000 domaintools_api_v2-2.0.1/domaintools/filters.py
+-rw-r--r--   0 bluza      (502) staff       (20)     3674 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/domaintools/results.py
+-rw-r--r--   0 bluza      (502) staff       (20)     5811 2024-05-03 13:55:31.000000 domaintools_api_v2-2.0.1/domaintools/utils.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.546645 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/
+-rw-r--r--   0 bluza      (502) staff       (20)     9691 2024-05-09 16:27:06.000000 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/PKG-INFO
+-rw-r--r--   0 bluza      (502) staff       (20)     1006 2024-05-09 16:27:06.000000 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 bluza      (502) staff       (20)        1 2024-05-09 16:27:06.000000 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 bluza      (502) staff       (20)       52 2024-05-09 16:27:06.000000 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/entry_points.txt
+-rw-r--r--   0 bluza      (502) staff       (20)       37 2024-05-09 16:27:06.000000 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/requires.txt
+-rw-r--r--   0 bluza      (502) staff       (20)       30 2024-05-09 16:27:06.000000 domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/top_level.txt
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.542822 domaintools_api_v2-2.0.1/domaintools_async/
+-rw-r--r--   0 bluza      (502) staff       (20)     3015 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/domaintools_async/__init__.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1453 2024-05-02 12:32:47.000000 domaintools_api_v2-2.0.1/pyproject.toml
+-rw-r--r--   0 bluza      (502) staff       (20)      172 2024-05-09 16:27:06.547521 domaintools_api_v2-2.0.1/setup.cfg
+-rwxr-xr-x   0 bluza      (502) staff       (20)     1541 2024-04-11 04:41:30.000000 domaintools_api_v2-2.0.1/setup.py
+drwxr-xr-x   0 bluza      (502) staff       (20)        0 2024-05-09 16:27:06.545570 domaintools_api_v2-2.0.1/tests/
+-rw-r--r--   0 bluza      (502) staff       (20)    15279 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/tests/test_api.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1760 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/tests/test_async.py
+-rw-r--r--   0 bluza      (502) staff       (20)     1045 2024-04-15 09:28:25.000000 domaintools_api_v2-2.0.1/tests/test_cli.py
+-rw-r--r--   0 bluza      (502) staff       (20)     3004 2024-05-07 12:07:01.000000 domaintools_api_v2-2.0.1/tests/test_filters.py
+-rw-r--r--   0 bluza      (502) staff       (20)     4055 2024-02-26 14:17:41.000000 domaintools_api_v2-2.0.1/tests/test_utils.py
```

### Comparing `domaintools_api_v2-2.0.0/LICENSE` & `domaintools_api_v2-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/PKG-INFO` & `domaintools_api_v2-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domaintools_api_v2
-Version: 2.0.0
+Version: 2.0.1
 Summary: DomainTools Official Python API
 Author-email: DomainTools <integrations@domaintools.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 DomainTools
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: domaintools_api_v2 Version: 2.0.0 Summary:
+Metadata-Version: 2.1 Name: domaintools_api_v2 Version: 2.0.1 Summary:
 DomainTools Official Python API Author-email: DomainTools
 domaintools.com> License: The MIT License (MIT) Copyright (c) 2016 DomainTools
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `domaintools_api_v2-2.0.0/README.md` & `domaintools_api_v2-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/_version.py` & `domaintools_api_v2-2.0.1/domaintools/_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
 CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 """
 
-current = "2.0.0"
+current = "2.0.1"
```

### Comparing `domaintools_api_v2-2.0.0/domaintools/api.py` & `domaintools_api_v2-2.0.1/domaintools/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 from hashlib import sha1, sha256, md5
 from hmac import new as hmac
 from types import MethodType
 import re
 
 from domaintools._version import current as version
 from domaintools.results import GroupedIterable, ParsedWhois, Reputation, Results
+from domaintools.filters import (
+    filter_by_riskscore,
+    filter_by_expire_date,
+    filter_by_date_updated_after,
+    filter_by_field,
+    DTResultFilter,
+)
 
 AVAILABLE_KEY_SIGN_HASHES = ["sha1", "sha256", "md5"]
 
 
 def delimited(items, character="|"):
     """Returns a character delimited version of the provided list as a Python string"""
     return character.join(items) if type(items) in (list, tuple, set) else items
@@ -545,23 +552,55 @@
             raise ValueError("One or more domains to enrich must be provided")
 
         domains = ",".join(domains)
         data_updated_after = kwargs.get("data_updated_after", None)
         if hasattr(data_updated_after, "strftime"):
             data_updated_after = data_updated_after.strftime("%Y-%m-%d")
 
-        return self._results(
+        results = self._results(
             "iris-enrich",
             "/v1/iris-enrich/",
             domain=domains,
             data_updated_after=data_updated_after,
             items_path=("results",),
             **kwargs,
         )
 
+        risk_score = kwargs.pop("risk_score", {}) or None
+        younger_than_date = kwargs.pop("younger_than_date", {}) or None
+        older_than_date = kwargs.pop("older_than_date", {}) or None
+        updated_after = kwargs.pop("updated_after", {}) or None
+        include_domains_with_missing_field = (
+            kwargs.pop("include_domains_with_missing_field", {}) or None
+        )
+        exclude_domains_with_missing_field = (
+            kwargs.pop("exclude_domains_with_missing_field", {}) or None
+        )
+
+        filtered_results = DTResultFilter(result_set=results).by(
+            [
+                filter_by_riskscore(threshold=risk_score),
+                filter_by_expire_date(date=younger_than_date, lookup_type="before"),
+                filter_by_expire_date(date=older_than_date, lookup_type="after"),
+                filter_by_date_updated_after(date=updated_after),
+                filter_by_field(
+                    field=include_domains_with_missing_field, filter_type="include"
+                ),
+                filter_by_field(
+                    field=exclude_domains_with_missing_field, filter_type="exclude"
+                ),
+            ]
+        )
+
+        results["results"] = filtered_results
+        results["results_count"] = len(filtered_results)
+        results["total_count"] = len(filtered_results)
+
+        return results
+
     def iris_enrich_cli(self, domains=None, **kwargs):
         """Returns back enriched data related to the specified domains using our Iris Enrich service.
          This is a CLI version of the iris_enrich method to help maintain backwards compatibility.
 
         api.iris_enrich(['domaintools.com', 'google.com'])
 
         api.iris_enrich(DOMAIN_LIST)['results_count'] Returns the number of results
@@ -597,14 +636,20 @@
         self,
         domains=None,
         data_updated_after=None,
         expiration_date=None,
         create_date=None,
         active=None,
         search_hash=None,
+        risk_score=None,
+        younger_than_date=None,
+        older_than_date=None,
+        updated_after=None,
+        include_domains_with_missing_field=None,
+        exclude_domains_with_missing_field=None,
         **kwargs,
     ):
         """Returns back a list of domains based on the provided filters.
         The following filters are available beyond what is parameterized as kwargs:
 
             - ip: Search for domains having this IP.
             - email: Search for domains with this email in their data.
@@ -658,25 +703,46 @@
         if hasattr(expiration_date, "strftime"):
             expiration_date = expiration_date.strftime("%Y-%m-%d")
         if hasattr(create_date, "strftime"):
             create_date = create_date.strftime("%Y-%m-%d")
         if isinstance(active, bool):
             kwargs["active"] = str(active).lower()
 
-        return self._results(
+        results = self._results(
             "iris-investigate",
             "/v1/iris-investigate/",
             domain=domains,
             data_updated_after=data_updated_after,
             expiration_date=expiration_date,
             create_date=create_date,
             items_path=("results",),
             **kwargs,
         )
 
+        filtered_results = DTResultFilter(result_set=results).by(
+            [
+                filter_by_riskscore(threshold=risk_score),
+                filter_by_expire_date(date=younger_than_date, lookup_type="before"),
+                filter_by_expire_date(date=older_than_date, lookup_type="after"),
+                filter_by_date_updated_after(date=updated_after),
+                filter_by_field(
+                    field=include_domains_with_missing_field, filter_type="include"
+                ),
+                filter_by_field(
+                    field=exclude_domains_with_missing_field, filter_type="exclude"
+                ),
+            ]
+        )
+
+        results["results"] = filtered_results
+        results["results_count"] = len(filtered_results)
+        results["total_count"] = len(filtered_results)
+
+        return results
+
     def iris_detect_monitors(
         self,
         include_counts=False,
         datetime_counts_since=None,
         sort=None,
         order="desc",
         offset=0,
```

### Comparing `domaintools_api_v2-2.0.0/domaintools/base_results.py` & `domaintools_api_v2-2.0.1/domaintools/base_results.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/cli/api.py` & `domaintools_api_v2-2.0.1/domaintools/cli/api.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/cli/commands/accounts.py` & `domaintools_api_v2-2.0.1/domaintools/cli/commands/accounts.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/cli/commands/detects.py` & `domaintools_api_v2-2.0.1/domaintools/cli/commands/detects.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/cli/commands/domains.py` & `domaintools_api_v2-2.0.1/domaintools/cli/commands/domains.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/cli/commands/ips.py` & `domaintools_api_v2-2.0.1/domaintools/cli/commands/ips.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/cli/commands/iris.py` & `domaintools_api_v2-2.0.1/domaintools/cli/commands/iris.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/cli/commands/phisheye.py` & `domaintools_api_v2-2.0.1/domaintools/cli/commands/phisheye.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/cli/constants.py` & `domaintools_api_v2-2.0.1/domaintools/cli/constants.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/cli/main.py` & `domaintools_api_v2-2.0.1/domaintools/cli/main.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/cli/utils.py` & `domaintools_api_v2-2.0.1/domaintools/cli/utils.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/exceptions.py` & `domaintools_api_v2-2.0.1/domaintools/exceptions.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/results.py` & `domaintools_api_v2-2.0.1/domaintools/results.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/domaintools/utils.py` & `domaintools_api_v2-2.0.1/domaintools/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from datetime import datetime
+
+from typing import Optional
+
 import re
 
 
 def get_domain_age(create_date):
     """
     Finds how many days old a domain is given a start date.
     Args:
@@ -166,7 +169,13 @@
                 elif isinstance(temp_data, tuple):
                     return_data.append([name[1:].upper().replace("_", " "), temp_data])
     count -= 1
     if count:
         return
     else:
         return return_data
+
+
+def convert_str_to_dateobj(
+    string_date: str, date_format: Optional[str] = "%Y-%m-%d"
+) -> datetime:
+    return datetime.strptime(string_date, date_format)
```

### Comparing `domaintools_api_v2-2.0.0/domaintools_api_v2.egg-info/PKG-INFO` & `domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domaintools_api_v2
-Version: 2.0.0
+Version: 2.0.1
 Summary: DomainTools Official Python API
 Author-email: DomainTools <integrations@domaintools.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 DomainTools
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: domaintools_api_v2 Version: 2.0.0 Summary:
+Metadata-Version: 2.1 Name: domaintools_api_v2 Version: 2.0.1 Summary:
 DomainTools Official Python API Author-email: DomainTools
 domaintools.com> License: The MIT License (MIT) Copyright (c) 2016 DomainTools
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `domaintools_api_v2-2.0.0/domaintools_api_v2.egg-info/SOURCES.txt` & `domaintools_api_v2-2.0.1/domaintools_api_v2.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 setup.py
 domaintools/__init__.py
 domaintools/_version.py
 domaintools/api.py
 domaintools/base_results.py
 domaintools/exceptions.py
+domaintools/filters.py
 domaintools/results.py
 domaintools/utils.py
 domaintools/cli/__init__.py
 domaintools/cli/api.py
 domaintools/cli/constants.py
 domaintools/cli/main.py
 domaintools/cli/utils.py
@@ -29,8 +30,9 @@
 domaintools_api_v2.egg-info/entry_points.txt
 domaintools_api_v2.egg-info/requires.txt
 domaintools_api_v2.egg-info/top_level.txt
 domaintools_async/__init__.py
 tests/test_api.py
 tests/test_async.py
 tests/test_cli.py
+tests/test_filters.py
 tests/test_utils.py
```

### Comparing `domaintools_api_v2-2.0.0/domaintools_async/__init__.py` & `domaintools_api_v2-2.0.1/domaintools_async/__init__.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/pyproject.toml` & `domaintools_api_v2-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/setup.py` & `domaintools_api_v2-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/tests/test_api.py` & `domaintools_api_v2-2.0.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/tests/test_async.py` & `domaintools_api_v2-2.0.1/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/tests/test_cli.py` & `domaintools_api_v2-2.0.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `domaintools_api_v2-2.0.0/tests/test_utils.py` & `domaintools_api_v2-2.0.1/tests/test_utils.py`

 * *Files identical despite different names*

