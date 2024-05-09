# Comparing `tmp/ptsamesite-1.0.1.tar.gz` & `tmp/ptsamesite-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptsamesite-1.0.1.tar", last modified: Mon May  6 17:10:16 2024, max compression
+gzip compressed data, was "ptsamesite-1.0.2.tar", last modified: Thu May  9 16:50:59 2024, max compression
```

## Comparing `ptsamesite-1.0.1.tar` & `ptsamesite-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 17:10:16.712427 ptsamesite-1.0.1/
--rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:24:58.000000 ptsamesite-1.0.1/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3681 2024-05-06 17:10:16.712427 ptsamesite-1.0.1/PKG-INFO
--rwxr-xr-x   0 kali      (1000) kali      (1000)     2883 2024-04-29 08:24:58.000000 ptsamesite-1.0.1/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 17:10:16.712427 ptsamesite-1.0.1/ptsamesite/
--rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:24:58.000000 ptsamesite-1.0.1/ptsamesite/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-04-29 08:24:58.000000 ptsamesite-1.0.1/ptsamesite/_version.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     7297 2024-05-06 13:47:15.000000 ptsamesite-1.0.1/ptsamesite/ptsamesite.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 17:10:16.712427 ptsamesite-1.0.1/ptsamesite.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3681 2024-05-06 17:10:16.000000 ptsamesite-1.0.1/ptsamesite.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      303 2024-05-06 17:10:16.000000 ptsamesite-1.0.1/ptsamesite.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-06 17:10:16.000000 ptsamesite-1.0.1/ptsamesite.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       58 2024-05-06 17:10:16.000000 ptsamesite-1.0.1/ptsamesite.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       32 2024-05-06 17:10:16.000000 ptsamesite-1.0.1/ptsamesite.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       11 2024-05-06 17:10:16.000000 ptsamesite-1.0.1/ptsamesite.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-06 17:10:16.712427 ptsamesite-1.0.1/setup.cfg
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1309 2024-05-06 17:02:21.000000 ptsamesite-1.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 16:50:59.458358 ptsamesite-1.0.2/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:24:58.000000 ptsamesite-1.0.2/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3682 2024-05-09 16:50:59.458358 ptsamesite-1.0.2/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2884 2024-05-07 11:36:10.000000 ptsamesite-1.0.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 16:50:59.458358 ptsamesite-1.0.2/ptsamesite/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:24:58.000000 ptsamesite-1.0.2/ptsamesite/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-09 16:49:51.000000 ptsamesite-1.0.2/ptsamesite/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     7305 2024-05-09 16:49:39.000000 ptsamesite-1.0.2/ptsamesite/ptsamesite.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 16:50:59.458358 ptsamesite-1.0.2/ptsamesite.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3682 2024-05-09 16:50:59.000000 ptsamesite-1.0.2/ptsamesite.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      303 2024-05-09 16:50:59.000000 ptsamesite-1.0.2/ptsamesite.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 16:50:59.000000 ptsamesite-1.0.2/ptsamesite.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       58 2024-05-09 16:50:59.000000 ptsamesite-1.0.2/ptsamesite.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       32 2024-05-09 16:50:59.000000 ptsamesite-1.0.2/ptsamesite.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       11 2024-05-09 16:50:59.000000 ptsamesite-1.0.2/ptsamesite.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 16:50:59.458358 ptsamesite-1.0.2/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1309 2024-05-06 17:02:21.000000 ptsamesite-1.0.2/setup.py
```

### Comparing `ptsamesite-1.0.1/LICENSE` & `ptsamesite-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptsamesite-1.0.1/PKG-INFO` & `ptsamesite-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptsamesite
-Version: 1.0.1
+Version: 1.0.2
 Summary: Same Site Scripting Detection Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptsamesite
@@ -20,15 +20,15 @@
 License-File: LICENSE
 Requires-Dist: ptlibs<2,>=1.0.7
 Requires-Dist: dnspython>=2.1
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTSAMESITE - Same Site Scripting Detection Tool
+## PTSAMESITE - Same Site Scripting Detection Tool
 
 ptsamesite is a tool designed to detect same-site scripting vulnerabilities across various domains.
 
 ## Installation
 
 ```
 pip install ptsamesite
```

### Comparing `ptsamesite-1.0.1/README.md` & `ptsamesite-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTSAMESITE - Same Site Scripting Detection Tool
+## PTSAMESITE - Same Site Scripting Detection Tool
 
 ptsamesite is a tool designed to detect same-site scripting vulnerabilities across various domains.
 
 ## Installation
 
 ```
 pip install ptsamesite
```

### Comparing `ptsamesite-1.0.1/ptsamesite/ptsamesite.py` & `ptsamesite-1.0.2/ptsamesite/ptsamesite.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,16 @@
         if len(self.domain_list) > 1 and self.use_json:
             self.ptjsonlib.end_error("Cannot test more than 1 domain while --json parameter is present", self.use_json)
 
     def run(self, args) -> None:
         """Main method"""
         ptprinthelper.ptprint("Vulnerable domains:", "TITLE", not self.use_json and self.vulnerable)
         self.ptthreads.threads(self.domain_list, self._test_domain, args.threads)
-        self.ptjsonlib.set_status("ok")
+
+        self.ptjsonlib.set_status("finished")
         ptprinthelper.ptprint(self.ptjsonlib.get_result_json(), "", self.use_json)
 
 
     def _test_domain(self, domain_list: list):
         printlock_ = printlock.PrintLock()
         subdomains = self._prepare_subdomains_for_test(domain_list)
         for subdomain in subdomains:
```

### Comparing `ptsamesite-1.0.1/ptsamesite.egg-info/PKG-INFO` & `ptsamesite-1.0.2/ptsamesite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptsamesite
-Version: 1.0.1
+Version: 1.0.2
 Summary: Same Site Scripting Detection Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptsamesite
@@ -20,15 +20,15 @@
 License-File: LICENSE
 Requires-Dist: ptlibs<2,>=1.0.7
 Requires-Dist: dnspython>=2.1
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTSAMESITE - Same Site Scripting Detection Tool
+## PTSAMESITE - Same Site Scripting Detection Tool
 
 ptsamesite is a tool designed to detect same-site scripting vulnerabilities across various domains.
 
 ## Installation
 
 ```
 pip install ptsamesite
```

### Comparing `ptsamesite-1.0.1/setup.py` & `ptsamesite-1.0.2/setup.py`

 * *Files identical despite different names*

