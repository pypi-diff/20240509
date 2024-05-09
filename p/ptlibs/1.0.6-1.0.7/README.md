# Comparing `tmp/ptlibs-1.0.6.tar.gz` & `tmp/ptlibs-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptlibs-1.0.6.tar", last modified: Thu Feb 22 23:44:34 2024, max compression
+gzip compressed data, was "ptlibs-1.0.7.tar", last modified: Thu May  9 13:54:34 2024, max compression
```

## Comparing `ptlibs-1.0.6.tar` & `ptlibs-1.0.7.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-02-22 23:44:34.052611 ptlibs-1.0.6/
--rw-rw-rw-   0        0        0    35149 2024-02-18 18:15:26.000000 ptlibs-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     3117 2024-02-22 23:44:34.052611 ptlibs-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2404 2024-02-22 23:41:49.000000 ptlibs-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-02-22 23:44:33.958425 ptlibs-1.0.6/ptlibs/
--rw-rw-rw-   0        0        0       21 2024-02-22 23:26:55.000000 ptlibs-1.0.6/ptlibs/__init__.py
--rw-rw-rw-   0        0        0      343 2024-02-18 18:15:26.000000 ptlibs-1.0.6/ptlibs/cli.py
--rw-rw-rw-   0        0        0     1115 2024-02-18 18:15:26.000000 ptlibs-1.0.6/ptlibs/ptcharsethelper.py
--rw-rw-rw-   0        0        0      753 2024-02-18 18:15:26.000000 ptlibs-1.0.6/ptlibs/ptdefs.py
--rw-rw-rw-   0        0        0     5190 2024-02-22 17:07:22.000000 ptlibs-1.0.6/ptlibs/ptjsonlib.py
--rw-rw-rw-   0        0        0     6542 2024-02-18 18:15:26.000000 ptlibs-1.0.6/ptlibs/ptmisclib.py
--rw-rw-rw-   0        0        0     2096 2024-02-18 18:15:26.000000 ptlibs-1.0.6/ptlibs/ptnethelper.py
--rw-rw-rw-   0        0        0     7512 2024-02-21 22:25:12.000000 ptlibs-1.0.6/ptlibs/ptpathtypedetector.py
--rw-rw-rw-   0        0        0     5881 2024-02-22 00:44:54.000000 ptlibs-1.0.6/ptlibs/ptprinthelper.py
-drwxrwxrwx   0        0        0        0 2024-02-22 23:44:34.052611 ptlibs-1.0.6/ptlibs/threads/
--rw-rw-rw-   0        0        0        0 2024-02-18 18:15:26.000000 ptlibs-1.0.6/ptlibs/threads/__init__.py
--rw-rw-rw-   0        0        0     1040 2024-02-18 18:15:26.000000 ptlibs-1.0.6/ptlibs/threads/arraylock.py
--rw-rw-rw-   0        0        0     1316 2024-02-18 18:15:26.000000 ptlibs-1.0.6/ptlibs/threads/printlock.py
--rw-rw-rw-   0        0        0     2014 2024-02-18 18:15:26.000000 ptlibs-1.0.6/ptlibs/threads/ptthreads.py
--rw-rw-rw-   0        0        0     3562 2024-02-18 18:15:26.000000 ptlibs-1.0.6/ptlibs/tldparser.py
-drwxrwxrwx   0        0        0        0 2024-02-22 23:44:34.052611 ptlibs-1.0.6/ptlibs.egg-info/
--rw-rw-rw-   0        0        0     3117 2024-02-22 23:44:33.000000 ptlibs-1.0.6/ptlibs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2024-02-22 23:44:33.000000 ptlibs-1.0.6/ptlibs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-22 23:44:33.000000 ptlibs-1.0.6/ptlibs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-02-22 23:44:33.000000 ptlibs-1.0.6/ptlibs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2024-02-22 23:44:33.000000 ptlibs-1.0.6/ptlibs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-22 23:44:33.000000 ptlibs-1.0.6/ptlibs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-22 23:44:34.052611 ptlibs-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      944 2024-02-18 18:15:26.000000 ptlibs-1.0.6/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:54:34.055226 ptlibs-1.0.7/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2024-04-27 19:41:20.000000 ptlibs-1.0.7/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     1565 2024-05-09 13:54:34.055226 ptlibs-1.0.7/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      849 2024-05-09 10:18:42.000000 ptlibs-1.0.7/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:54:34.055226 ptlibs-1.0.7/ptlibs/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-05-06 09:15:32.000000 ptlibs-1.0.7/ptlibs/_version.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      352 2024-05-09 10:18:42.000000 ptlibs-1.0.7/ptlibs/cli.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1115 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/ptcharsethelper.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      753 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/ptdefs.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6590 2024-05-09 10:18:42.000000 ptlibs-1.0.7/ptlibs/ptjsonlib.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7360 2024-05-09 10:18:42.000000 ptlibs-1.0.7/ptlibs/ptmisclib.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2096 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/ptnethelper.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7550 2024-05-09 10:18:37.000000 ptlibs-1.0.7/ptlibs/ptpathtypedetector.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5881 2024-05-06 15:00:46.000000 ptlibs-1.0.7/ptlibs/ptprinthelper.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:54:34.055226 ptlibs-1.0.7/ptlibs/threads/
+-rw-r--r--   0 kali      (1000) kali      (1000)        0 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/threads/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1040 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/threads/arraylock.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1316 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/threads/printlock.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2014 2024-04-27 19:41:20.000000 ptlibs-1.0.7/ptlibs/threads/ptthreads.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4092 2024-05-09 10:18:42.000000 ptlibs-1.0.7/ptlibs/tldparser.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 13:54:34.055226 ptlibs-1.0.7/ptlibs.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1565 2024-05-09 13:54:34.000000 ptlibs-1.0.7/ptlibs.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      549 2024-05-09 13:54:34.000000 ptlibs-1.0.7/ptlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 13:54:34.000000 ptlibs-1.0.7/ptlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       43 2024-05-09 13:54:34.000000 ptlibs-1.0.7/ptlibs.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       27 2024-05-09 13:54:34.000000 ptlibs-1.0.7/ptlibs.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        7 2024-05-09 13:54:34.000000 ptlibs-1.0.7/ptlibs.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 13:54:34.055226 ptlibs-1.0.7/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1073 2024-05-09 13:54:08.000000 ptlibs-1.0.7/setup.py
```

### Comparing `ptlibs-1.0.6/LICENSE` & `ptlibs-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.6/ptlibs/ptcharsethelper.py` & `ptlibs-1.0.7/ptlibs/ptcharsethelper.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.6/ptlibs/ptdefs.py` & `ptlibs-1.0.7/ptlibs/ptdefs.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.6/ptlibs/ptjsonlib.py` & `ptlibs-1.0.7/ptlibs/ptjsonlib.py`

 * *Files 26% similar despite different names*

```diff
@@ -31,26 +31,27 @@
 
     def add_nodes(self, nodes: list) -> None:
         """Adds nodes to json_object"""
         assert type(nodes) is list
         for node in nodes:
             self.add_node(node)
 
-    def parse_url2nodes(self, url: str, nodes: list = []) -> list[dict]:
+    def parse_url2nodes(self, url: str, nodes: list = None) -> list[dict]:
         """Parses url to node object"""
+        nodes = nodes if nodes else []
         base_url = self.get_base_url(url)
         parent = None
         paths = self.get_paths(url)
         for index, path in enumerate(paths):
             url = f"{base_url}/{'/'.join(paths[0:index+1])}"
             page_type = self.PtPathTypeDetector.get_type(path)
             parent_type = "webRootDirectory" if index == 0 else None
-            properties = {"name": path, "url": url, "webPageType": page_type}
+            properties = {"name": path, "url": url, "webSourceType": page_type}
             node_object = self.create_node_object("webSource", parent_type, parent, properties, nodes)
-            if type(node_object) is not str: #check whether node already exists
+            if type(node_object) is not str: # check whether node already exists
                 parent = node_object["key"]
                 nodes.append(node_object)
             else:
                 parent = node_object
         return nodes
 
     def get_base_url(self, url: str) -> str:
@@ -62,51 +63,77 @@
         base_address = address.split("/")[0]
         return f"{schema + schema_separator if schema else ''}{base_address}"
 
     def get_paths(self, url: str) -> list[str]:
         """Returns paths from url"""
         return url.strip("/").split("/")[2:][1:]
 
-    def create_node_object(self, node_type: str, parent_type=None, parent=None, properties: dict = {}, nodes: list=[]) -> dict:
+    def create_node_object(self, node_type: str, parent_type=None, parent=None, properties: dict = None, nodes: list = None, vulnerabilities: list = None) -> dict:
         """Creates node object"""
-        assert type(properties) is dict
+        properties = properties or {}
+        nodes = nodes or []
+        vulnerabilities = vulnerabilities or []
+        assert isinstance(properties, dict)
+        assert isinstance(nodes, list)
+        assert isinstance(vulnerabilities, list)
+
         ident = self.node_duplicity_check(parent_type, properties, nodes)
         if ident:
             return ident
-        return {"type": node_type, "key": self.create_guid(), "parent": parent, "parentType": parent_type, "properties": properties, "vulnerabilities": [] }
+        return {"type": node_type, "key": self.create_guid(), "parent": parent, "parentType": parent_type, "properties": properties, "vulnerabilities": vulnerabilities }
 
     def node_duplicity_check(self, parent_type, properties: dict, nodes: list) -> str | None:
         """Returns node ident if node already exists in json_object else returns None"""
         for node in nodes:
             if node["parentType"] == parent_type:
                 if node["properties"] == properties:
                     return node["key"]
         return None
 
     def create_guid(self) -> str:
         """Creates random guid"""
         return str(uuid.uuid4())
 
+    def to_camel_case(self, snake_str):
+        components = snake_str.split('_')
+        return components[0] + ''.join(x.title() for x in components[1:])
+
+    def convert_keys_to_camel_case(self, original_dict: dict, keys_to_convert: list):
+        """Create a new dictionary with camelCase keys"""
+        camel_case_dict = {}
+        for key, value in original_dict.items():
+            if key in keys_to_convert:
+                camel_case_key = self.to_camel_case(key)
+                camel_case_dict[camel_case_key] = value
+            else:
+                camel_case_dict[key] = value
+        return camel_case_dict
+
     def add_property(self, name: str, value: str) -> None:
         self.json_object["results"]["properties"].update({"name": name, "value": value})
 
-    def add_vulnerability(self, code: str, request: str=None, response: str=None, description: str=None, score: str=None, note: str=None, node_key: str=None) -> None:
+    def add_vulnerability(self, vuln_code: str, vuln_request: str=None, vuln_response: str=None, description: str=None, score: str=None, note: str=None, node_key: str=None) -> None:
         """Add vulnerability code to the json result, if <node_key> parameter is provided, vulnerability will be added to the specified node instead."""
-        vuln_dict = {k:v for k, v in locals().items() if v is not None}
-        vuln_dict.pop("self", None)
+        vulnerability_dict = {k:v for k, v in locals().items() if v is not None}; vulnerability_dict.pop("self", None)
+        vulnerability_dict = self.convert_keys_to_camel_case(vulnerability_dict, keys_to_convert=["vuln_code", "vuln_request", "vuln_response"])
 
         if node_key:
-            vuln_dict.pop("node_key")
+            vulnerability_dict.pop("node_key")
             for d in self.json_object["results"]["nodes"]:
                 if d["key"] == node_key:
-                    d["vulnerabilities"].append(vuln_dict)
+                    if not self.vuln_code_in_vulnerabilities(vuln_code):
+                        d["vulnerabilities"].append(vulnerability_dict)
                     break
         else:
-            self.json_object["results"]["vulnerabilities"].append(vuln_dict)
+            self.json_object["results"]["vulnerabilities"].append(vulnerability_dict)
 
+    def vuln_code_in_vulnerabilities(self, code: str) -> bool:
+        for obj in self.json_object["results"]["vulnerabilities"]:
+            if obj.get("code") == code:
+                return True
 
     def set_status(self, status: str, message: str = "") -> None:
         self.json_object["status"] = status
         if message:
             self.json_object["message"] = message
 
     def set_message(self, message: str) -> None:
@@ -121,8 +148,8 @@
         ptprint( out_if(self.get_result_json(), None, condition) )
         sys.exit(1)
 
     def end_ok(self, message, condition, bullet_type="ERROR"):
         ptprint( out_ifnot(message, bullet_type, condition) )
         self.set_status("ok", message)
         ptprint( out_if(self.get_result_json(), None, condition) )
-        sys.exit(0)
+        sys.exit(0)
```

### Comparing `ptlibs-1.0.6/ptlibs/ptmisclib.py` & `ptlibs-1.0.7/ptlibs/ptmisclib.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from hashlib import sha256
-import datetime
 from http.cookies import SimpleCookie
+import datetime
 import os
 import pickle
 import signal
 import sys
 import tempfile
 import typing
 import re
@@ -12,20 +12,26 @@
 import requests
 from requests_toolbelt.utils import dump
 
 from ptlibs import ptdefs
 from ptlibs.ptprinthelper import out_if, ptprint
 
 
+
 def signal_handler(sig, frame):
     ptprint(f"\r", clear_to_eol=True)
-    ptprint( out_if(f"{ptdefs.colors['ERROR']}Script terminated{ptdefs.colors['TEXT']}", "ERROR"), clear_to_eol=True)
-    sys.exit(0)
-signal.signal(signal.SIGINT, signal_handler)
+    ptprint( out_if(f"{ptdefs.colors['ERROR']}Script terminating. Press CTRL+C again to force.{ptdefs.colors['TEXT']}", "ERROR"), clear_to_eol=True)
 
+    #with open(os.devnull, "w") as devnull:
+    #    sys.stdout = devnull
+        #sys.stderr = devnull
+    sys.exit(1)
+
+# Register the signal handler for SIGINT
+signal.signal(signal.SIGINT, signal_handler)
 
 def read_file(file: str) -> list[str]:
     with open(file, "r") as f:
         domain_list = [line.strip("\n") for line in f]
         return domain_list
 
 
@@ -117,15 +123,15 @@
         raise error
     return response
 
 
 def _get_cookies_from_headers(headers: dict) -> dict | None:
     if "Cookie" not in headers:
         return None
-    
+
     cookies_object = SimpleCookie()
     cookies_object.load(headers["Cookie"])
     cookies = {key: morsel.value for key, morsel in cookies_object.items()}
     return cookies
 
 
 def load_url_from_web_or_temp(url: str, method: str, headers: dict, proxies: dict = {}, data: dict = None, timeout: int = None, redirects: bool = False, verify: bool = False, cache: bool = False, dump_response: bool = False, auth: tuple[str, str] = None) -> requests.Response:
@@ -164,7 +170,27 @@
             response = _get_response(url, method, headers, proxies, data, timeout, redirects, verify, auth)
             response_dump = get_response_data_dump(response)
             save_object({"response": response, "response_dump": response_dump}, filename)
             return response if not dump_response else (response, response_dump)
     else:
         response = _get_response(url, method, headers, proxies, data, timeout, redirects, verify, auth)
         return response if not dump_response else (response, get_response_data_dump(response))
+
+
+def clean_html(input_html):
+    """
+    Removes all HTML tags from the input string, replacing <br>, <br/> and </p> tags with newlines.
+
+    Parameters:
+    input_html (str): A string containing HTML content.
+
+    Returns:
+    str: The cleaned string with no HTML tags and certain tags replaced by newline characters.
+    """
+    # Replace <br>, <br/>, and </p> tags with \n
+    patterns_to_newline = re.compile(r'(<br\s*/?>|</p>)', re.IGNORECASE)
+    text_with_newlines = re.sub(patterns_to_newline, '\n', input_html)
+
+    # Remove all other HTML tags
+    clean_text = re.sub(r'<.*?>', '', text_with_newlines)
+
+    return clean_text.rstrip()
```

### Comparing `ptlibs-1.0.6/ptlibs/ptnethelper.py` & `ptlibs-1.0.7/ptlibs/ptnethelper.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.6/ptlibs/ptpathtypedetector.py` & `ptlibs-1.0.7/ptlibs/ptpathtypedetector.py`

 * *Files 9% similar despite different names*

```diff
@@ -122,51 +122,51 @@
             A string representing the file type.
         """
 
         self.path = path
         self.resource_name, self.extension = os.path.splitext(path)
 
         if self.is_directory():
-            return "webPageTypeDirectory"
+            return "webSourceTypeDirectory"
         elif self.is_html():
-            return "webPageTypeHtml"
+            return "webSourceTypeHtml"
         elif self.is_robots_file():
-            return "webPageTypeRobotsTxt"
+            return "webSourceTypeRobotsTxt"
         elif self.is_sitemap_file():
-            return "webPageTypeSitemap"
+            return "webSourceTypeSitemap"
         elif self.is_security_file():
-            return "webPageTypeSecurityTxt"
+            return "webSourceTypeSecurityTxt"
         elif self.is_document():
-            return 'webPageTypeDocument'
+            return 'webSourceTypeDocument'
         elif self.is_image():
-            return 'webPageTypeImage'
+            return 'webSourceTypeImage'
         elif self.is_config():
-            return 'webPageTypeConfiguration'
+            return 'webSourceTypeConfiguration'
         elif self.is_backup():
-            return 'webPageTypeBackup'
+            return 'webSourceTypeBackup'
         elif self.is_json():
-            return 'webPageTypeJson'
+            return 'webSourceTypeJson'
         elif self.is_xml():
-            return 'webPageTypeXml'
+            return 'webSourceTypeXml'
         elif self.is_db():
-            return 'webPageTypeDatabase'
+            return 'webSourceTypeDatabase'
         elif self.is_javascript():
-            return 'webPageTypeJavaScript'
+            return 'webSourceTypeJavaScript'
         elif self.is_css():
-            return 'webPageTypeCss'
+            return 'webSourceTypeCss'
         elif self.is_rss():
-            return 'webPageTypeRss'
+            return 'webSourceTypeRss'
         elif self.is_binary():
-            return 'webPageTypeBinary'
+            return 'webSourceTypeBinary'
         elif self.is_archive():
-            return 'webPageTypeArchive'
+            return 'webSourceTypeArchive'
         elif self.is_crossdomain_file():
-            return 'webPageTypeCrossDomainXml'
+            return 'webSourceTypeCrossDomainXml'
         else:
-            return "webPageTypeOther"
+            return "webSourceTypeOther"
 
 
     def is_directory(self):
         """Determine if the path is a directory."""
         return self.extension == ""
 
     def is_html(self):
```

### Comparing `ptlibs-1.0.6/ptlibs/ptprinthelper.py` & `ptlibs-1.0.7/ptlibs/ptprinthelper.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.6/ptlibs/threads/arraylock.py` & `ptlibs-1.0.7/ptlibs/threads/arraylock.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.6/ptlibs/threads/printlock.py` & `ptlibs-1.0.7/ptlibs/threads/printlock.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.6/ptlibs/threads/ptthreads.py` & `ptlibs-1.0.7/ptlibs/threads/ptthreads.py`

 * *Files identical despite different names*

### Comparing `ptlibs-1.0.6/ptlibs.egg-info/SOURCES.txt` & `ptlibs-1.0.7/ptlibs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 ptlibs/__init__.py
+ptlibs/_version.py
 ptlibs/cli.py
 ptlibs/ptcharsethelper.py
 ptlibs/ptdefs.py
 ptlibs/ptjsonlib.py
 ptlibs/ptmisclib.py
 ptlibs/ptnethelper.py
 ptlibs/ptpathtypedetector.py
```

### Comparing `ptlibs-1.0.6/setup.py` & `ptlibs-1.0.7/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import setuptools
 
-from ptlibs import __version__
+from ptlibs._version import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ptlibs",
     description="Support library for penterepTools",
     author="Penterep",
     author_email="info@penterep.com",
     url="https://www.penterep.com/",
     version=__version__,
-    license="GPLv3+",
+    license="GPLv3",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
     ],
     entry_points = {'console_scripts': ['ptlibs = ptlibs.cli:main']},
-    python_requires = '>=3.6',
+    python_requires = '>=3.9',
     install_requires=["requests", "requests-toolbelt"],
     long_description=long_description,
-    long_description_content_type="text/markdown"
+    long_description_content_type="text/markdown",
+    project_urls = {
+    "homepage":   "https://www.penterep.com/",
+    "repository": "https://github.com/penterep/ptlibs",
+    }
 )
```

