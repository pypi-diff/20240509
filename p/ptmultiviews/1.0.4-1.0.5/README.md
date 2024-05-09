# Comparing `tmp/ptmultiviews-1.0.4.tar.gz` & `tmp/ptmultiviews-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptmultiviews-1.0.4.tar", last modified: Thu May  9 11:09:49 2024, max compression
+gzip compressed data, was "ptmultiviews-1.0.5.tar", last modified: Thu May  9 16:57:38 2024, max compression
```

## Comparing `ptmultiviews-1.0.4.tar` & `ptmultiviews-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 11:09:49.890662 ptmultiviews-1.0.4/
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2024-04-29 08:26:15.000000 ptmultiviews-1.0.4/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-09 11:09:49.890662 ptmultiviews-1.0.4/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     3596 2024-05-09 09:38:41.000000 ptmultiviews-1.0.4/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 11:09:49.890662 ptmultiviews-1.0.4/ptmultiviews/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:15.000000 ptmultiviews-1.0.4/ptmultiviews/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-09 11:04:18.000000 ptmultiviews-1.0.4/ptmultiviews/_version.py
--rw-r--r--   0 kali      (1000) kali      (1000)    15483 2024-05-09 09:38:41.000000 ptmultiviews-1.0.4/ptmultiviews/ptmultiviews.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 11:09:49.890662 ptmultiviews-1.0.4/ptmultiviews.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-09 11:09:49.000000 ptmultiviews-1.0.4/ptmultiviews.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      323 2024-05-09 11:09:49.000000 ptmultiviews-1.0.4/ptmultiviews.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 11:09:49.000000 ptmultiviews-1.0.4/ptmultiviews.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       64 2024-05-09 11:09:49.000000 ptmultiviews-1.0.4/ptmultiviews.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-09 11:09:49.000000 ptmultiviews-1.0.4/ptmultiviews.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2024-05-09 11:09:49.000000 ptmultiviews-1.0.4/ptmultiviews.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 11:09:49.890662 ptmultiviews-1.0.4/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1254 2024-05-09 10:21:25.000000 ptmultiviews-1.0.4/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 16:57:38.348249 ptmultiviews-1.0.5/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2024-04-29 08:26:15.000000 ptmultiviews-1.0.5/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-09 16:57:38.348249 ptmultiviews-1.0.5/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     3596 2024-05-09 09:38:41.000000 ptmultiviews-1.0.5/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 16:57:38.348249 ptmultiviews-1.0.5/ptmultiviews/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:15.000000 ptmultiviews-1.0.5/ptmultiviews/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-09 16:54:35.000000 ptmultiviews-1.0.5/ptmultiviews/_version.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    15528 2024-05-09 16:52:51.000000 ptmultiviews-1.0.5/ptmultiviews/ptmultiviews.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 16:57:38.348249 ptmultiviews-1.0.5/ptmultiviews.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     4462 2024-05-09 16:57:38.000000 ptmultiviews-1.0.5/ptmultiviews.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      323 2024-05-09 16:57:38.000000 ptmultiviews-1.0.5/ptmultiviews.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 16:57:38.000000 ptmultiviews-1.0.5/ptmultiviews.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       64 2024-05-09 16:57:38.000000 ptmultiviews-1.0.5/ptmultiviews.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-09 16:57:38.000000 ptmultiviews-1.0.5/ptmultiviews.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2024-05-09 16:57:38.000000 ptmultiviews-1.0.5/ptmultiviews.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 16:57:38.348249 ptmultiviews-1.0.5/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1254 2024-05-09 10:21:25.000000 ptmultiviews-1.0.5/setup.py
```

### Comparing `ptmultiviews-1.0.4/LICENSE` & `ptmultiviews-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ptmultiviews-1.0.4/PKG-INFO` & `ptmultiviews-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptmultiviews
-Version: 1.0.4
+Version: 1.0.5
 Summary: Apache Multiviews Detection & Enumeration Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptmultiviews
```

### Comparing `ptmultiviews-1.0.4/README.md` & `ptmultiviews-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ptmultiviews-1.0.4/ptmultiviews/ptmultiviews.py` & `ptmultiviews-1.0.5/ptmultiviews/ptmultiviews.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,16 @@
         elif self.domain_file_test:
             # Domains from file
             ptprinthelper.ptprint("Vulnerable domains:", "TITLE", not self.use_json, newline_above=True, colortext=True)
             self.ptthreads.threads(self.url_list, self._is_vulnerable, args.threads)
 
         ptprinthelper.ptprint('\n'.join(sorted(self.result_path_list)), "", not self.use_json)
 
-        if not self.result_path_list:
-            ptprinthelper.ptprint("No alternatives to enumerate")
+        if not self.result_path_list and not self.use_json:
+            ptprinthelper.ptprint("No alternatives to enumerate", "", not self.use_json)
 
         if self.output_file:
             self._write_output_to_file(args.output)
 
         self.ptjsonlib.set_status("finished")
         ptprinthelper.ptprint(self.ptjsonlib.get_result_json(), condition=self.use_json)
```

### Comparing `ptmultiviews-1.0.4/ptmultiviews.egg-info/PKG-INFO` & `ptmultiviews-1.0.5/ptmultiviews.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptmultiviews
-Version: 1.0.4
+Version: 1.0.5
 Summary: Apache Multiviews Detection & Enumeration Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptmultiviews
```

### Comparing `ptmultiviews-1.0.4/setup.py` & `ptmultiviews-1.0.5/setup.py`

 * *Files identical despite different names*

