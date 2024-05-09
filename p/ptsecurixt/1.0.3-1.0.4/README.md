# Comparing `tmp/ptsecurixt-1.0.3.tar.gz` & `tmp/ptsecurixt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptsecurixt-1.0.3.tar", last modified: Mon May  6 16:54:52 2024, max compression
+gzip compressed data, was "ptsecurixt-1.0.4.tar", last modified: Thu May  9 11:13:24 2024, max compression
```

## Comparing `ptsecurixt-1.0.3.tar` & `ptsecurixt-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 16:54:52.122424 ptsecurixt-1.0.3/
--rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:25:17.000000 ptsecurixt-1.0.3/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3378 2024-05-06 16:54:52.122424 ptsecurixt-1.0.3/PKG-INFO
--rwxr-xr-x   0 kali      (1000) kali      (1000)     2616 2024-05-06 16:33:40.000000 ptsecurixt-1.0.3/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 16:54:52.122424 ptsecurixt-1.0.3/ptsecurixt/
--rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:25:17.000000 ptsecurixt-1.0.3/ptsecurixt/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-06 16:46:51.000000 ptsecurixt-1.0.3/ptsecurixt/_version.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)     6887 2024-05-06 16:33:44.000000 ptsecurixt-1.0.3/ptsecurixt/ptsecurixt.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-06 16:54:52.122424 ptsecurixt-1.0.3/ptsecurixt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3378 2024-05-06 16:54:52.000000 ptsecurixt-1.0.3/ptsecurixt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      303 2024-05-06 16:54:52.000000 ptsecurixt-1.0.3/ptsecurixt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-06 16:54:52.000000 ptsecurixt-1.0.3/ptsecurixt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       58 2024-05-06 16:54:52.000000 ptsecurixt-1.0.3/ptsecurixt.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-06 16:54:52.000000 ptsecurixt-1.0.3/ptsecurixt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       11 2024-05-06 16:54:52.000000 ptsecurixt-1.0.3/ptsecurixt.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-06 16:54:52.122424 ptsecurixt-1.0.3/setup.cfg
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1274 2024-05-06 16:47:02.000000 ptsecurixt-1.0.3/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 11:13:24.250596 ptsecurixt-1.0.4/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:25:17.000000 ptsecurixt-1.0.4/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3379 2024-05-09 11:13:24.250596 ptsecurixt-1.0.4/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2617 2024-05-09 09:47:09.000000 ptsecurixt-1.0.4/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 11:13:24.250596 ptsecurixt-1.0.4/ptsecurixt/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:25:17.000000 ptsecurixt-1.0.4/ptsecurixt/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-09 11:12:23.000000 ptsecurixt-1.0.4/ptsecurixt/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     6891 2024-05-09 09:46:57.000000 ptsecurixt-1.0.4/ptsecurixt/ptsecurixt.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 11:13:24.250596 ptsecurixt-1.0.4/ptsecurixt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3379 2024-05-09 11:13:24.000000 ptsecurixt-1.0.4/ptsecurixt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      303 2024-05-09 11:13:24.000000 ptsecurixt-1.0.4/ptsecurixt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 11:13:24.000000 ptsecurixt-1.0.4/ptsecurixt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       58 2024-05-09 11:13:24.000000 ptsecurixt-1.0.4/ptsecurixt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2024-05-09 11:13:24.000000 ptsecurixt-1.0.4/ptsecurixt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       11 2024-05-09 11:13:24.000000 ptsecurixt-1.0.4/ptsecurixt.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 11:13:24.250596 ptsecurixt-1.0.4/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1274 2024-05-09 09:46:57.000000 ptsecurixt-1.0.4/setup.py
```

### Comparing `ptsecurixt-1.0.3/LICENSE` & `ptsecurixt-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ptsecurixt-1.0.3/PKG-INFO` & `ptsecurixt-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptsecurixt
-Version: 1.0.3
+Version: 1.0.4
 Summary: security.txt finder
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptsecurixt
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ptlibs<2,>=1.0.7
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTSECURIXT - security.txt finder
+## PTSECURIXT - security.txt finder
 
 ptsecurixt is an automated tool that efficiently locates 'security.txt' files in their known locations.
 
 ## Installation
 
 ```
 pip install ptsecurixt
```

### Comparing `ptsecurixt-1.0.3/README.md` & `ptsecurixt-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTSECURIXT - security.txt finder
+## PTSECURIXT - security.txt finder
 
 ptsecurixt is an automated tool that efficiently locates 'security.txt' files in their known locations.
 
 ## Installation
 
 ```
 pip install ptsecurixt
```

### Comparing `ptsecurixt-1.0.3/ptsecurixt/ptsecurixt.py` & `ptsecurixt-1.0.4/ptsecurixt/ptsecurixt.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         if response.status_code == 200 and "text/plain" in response.headers["content-type"]:
             self._break_carriage_return()
             ptprinthelper.ptprint(f"Found security.txt file", "OK", not self.use_json)
             ptprinthelper.ptprint(f"File contents:", "TITLE", not self.use_json)
             file_contents = response.text.encode('ascii', 'ignore').decode()
             ptprinthelper.ptprint(file_contents, "", not self.use_json, newline_above=True)
             if self.use_json:
-                self.ptjsonlib.add_node(self.ptjsonlib.create_node_object("webpage", properties={"url": url, "name": os.path.split(response.url)[-1], "WebPageType": "security_txt"}))
+                self.ptjsonlib.add_node(self.ptjsonlib.create_node_object("webSource", properties={"url": url, "name": os.path.split(response.url)[-1], "WebSourceType": "security_txt"}))
             return True
 
     def _adjust_url(self, url: str) -> str:
         o = urllib.parse.urlparse(url)
         if not re.match("https?$", o.scheme):
             self.ptjsonlib.end_error("Missing or wrong scheme - only HTTP/HTTPS schemas are supported", self.use_json)
         if not o.netloc:
```

### Comparing `ptsecurixt-1.0.3/ptsecurixt.egg-info/PKG-INFO` & `ptsecurixt-1.0.4/ptsecurixt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptsecurixt
-Version: 1.0.3
+Version: 1.0.4
 Summary: security.txt finder
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptsecurixt
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ptlibs<2,>=1.0.7
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
 
-# PTSECURIXT - security.txt finder
+## PTSECURIXT - security.txt finder
 
 ptsecurixt is an automated tool that efficiently locates 'security.txt' files in their known locations.
 
 ## Installation
 
 ```
 pip install ptsecurixt
```

### Comparing `ptsecurixt-1.0.3/setup.py` & `ptsecurixt-1.0.4/setup.py`

 * *Files identical despite different names*

