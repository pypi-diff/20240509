# Comparing `tmp/ptcrossd-1.0.2.tar.gz` & `tmp/ptcrossd-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptcrossd-1.0.2.tar", last modified: Fri Aug  4 11:22:59 2023, max compression
+gzip compressed data, was "ptcrossd-1.0.3.tar", last modified: Thu May  9 10:57:07 2024, max compression
```

## Comparing `ptcrossd-1.0.2.tar` & `ptcrossd-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:22:59.458378 ptcrossd-1.0.2/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35823 2023-07-27 11:42:59.000000 ptcrossd-1.0.2/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3151 2023-08-04 11:22:59.458378 ptcrossd-1.0.2/PKG-INFO
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     2666 2023-08-03 16:40:19.000000 ptcrossd-1.0.2/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:22:59.458378 ptcrossd-1.0.2/ptcrossd/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-27 11:42:59.000000 ptcrossd-1.0.2/ptcrossd/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-08-03 16:41:44.000000 ptcrossd-1.0.2/ptcrossd/_version.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    12589 2023-08-03 17:50:01.000000 ptcrossd-1.0.2/ptcrossd/ptcrossd.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:22:59.458378 ptcrossd-1.0.2/ptcrossd.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3151 2023-08-04 11:22:59.000000 ptcrossd-1.0.2/ptcrossd.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      283 2023-08-04 11:22:59.000000 ptcrossd-1.0.2/ptcrossd.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-08-04 11:22:59.000000 ptcrossd-1.0.2/ptcrossd.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       52 2023-08-04 11:22:59.000000 ptcrossd-1.0.2/ptcrossd.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       33 2023-08-04 11:22:59.000000 ptcrossd-1.0.2/ptcrossd.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        9 2023-08-04 11:22:59.000000 ptcrossd-1.0.2/ptcrossd.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-08-04 11:22:59.458378 ptcrossd-1.0.2/setup.cfg
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     1036 2023-07-27 11:42:59.000000 ptcrossd-1.0.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 10:57:07.230878 ptcrossd-1.0.3/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:26:45.000000 ptcrossd-1.0.3/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3532 2024-05-09 10:57:07.230878 ptcrossd-1.0.3/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2684 2024-04-29 08:26:45.000000 ptcrossd-1.0.3/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 10:57:07.230878 ptcrossd-1.0.3/ptcrossd/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:45.000000 ptcrossd-1.0.3/ptcrossd/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       21 2024-04-29 08:26:45.000000 ptcrossd-1.0.3/ptcrossd/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    13651 2024-05-09 09:06:31.000000 ptcrossd-1.0.3/ptcrossd/ptcrossd.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 10:57:07.230878 ptcrossd-1.0.3/ptcrossd.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3532 2024-05-09 10:57:07.000000 ptcrossd-1.0.3/ptcrossd.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      283 2024-05-09 10:57:07.000000 ptcrossd-1.0.3/ptcrossd.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 10:57:07.000000 ptcrossd-1.0.3/ptcrossd.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       52 2024-05-09 10:57:07.000000 ptcrossd-1.0.3/ptcrossd.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       28 2024-05-09 10:57:07.000000 ptcrossd-1.0.3/ptcrossd.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        9 2024-05-09 10:57:07.000000 ptcrossd-1.0.3/ptcrossd.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 10:57:07.230878 ptcrossd-1.0.3/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1293 2024-04-29 08:26:45.000000 ptcrossd-1.0.3/setup.py
```

### Comparing `ptcrossd-1.0.2/LICENSE` & `ptcrossd-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ptcrossd-1.0.2/PKG-INFO` & `ptcrossd-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,99 @@
 Metadata-Version: 2.1
 Name: ptcrossd
-Version: 1.0.2
-Summary: crossdomain.xml misconfigurations testing tool
+Version: 1.0.3
+Summary: Crossdomain.xml Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
-License: GPLv3+
+License: GPLv3
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptcrossd
+Project-URL: tracker, https://github.com/penterep/ptcrossd/issues
+Project-URL: changelog, https://github.com/penterep/ptcrossd/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.6
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ptlibs<2,>=1.0.7
+Requires-Dist: defusedxml
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
-
-# PTCROSSD
-
-> crossdomain.xml misconfigurations testing tool
+## PTCROSSD - Crossdomain.xml Testing Tool
 
 ## Installation
+
 ```
 pip install ptcrossd
 ```
 
-## Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+## Adding to PATH
+If you're unable to invoke the script from your terminal, it's likely because it's not included in your PATH. You can resolve this issue by executing the following commands, depending on the shell you're using:
 
-> Add to PATH for Bash
+For Bash Users
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
-> Add to PATH for ZSH
+For ZSH Users
 ```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
-source ~/.zshhrc
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
+source ~/.zshrc
 ```
 
-
 ## Usage examples
 ```
 ptcrossd -u https://www.example.com/crossdomain.xml
 ptcrossd -u https://www.example.com/
 ```
 
 ## Options
-
 ```
--u   --url         <url>           Connect to URL
--p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--T   --timeout     <timeout>       Set timeout (default to 10)
--c   --cookie      <cookie>        Set cookie
--ua  --user-agent  <user-agent>    Set User-Agent header
--H   --headers     <header:value>  Set custom header(s)
--C   --cache                       Cache requests (load from tmp in future)
--v   --version                     Show script version and exit
--h   --help                        Show this help message and exit
--j   --json                        Output in JSON format
+-u   --url                  <url>           Connect to URL
+-cf  --cross-domain-file                    Test crossdomain.xml file
+-ch  --cross-origin-header                  Test Access-Control-Allow-Origin header
+-p   --proxy                <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T   --timeout              <timeout>       Set timeout (default to 10)
+-c   --cookie               <cookie>        Set cookie
+-a   --user-agent           <user-agent>    Set User-Agent header
+-H   --headers              <header:value>  Set custom header(s)
+-C   --cache                                Cache requests (load from tmp in future)
+-v   --version                              Show script version and exit
+-h   --help                                 Show this help message and exit
+-j   --json                                 Output in JSON format
 ```
 
 ## Dependencies
 ```
-defusedxml
-requests
 ptlibs
+defusedxml
 ```
 
-## Version History
-```
-1.0.2
-    - Full script rework
-1.0.1
-    - Fix urllib3 error
-1.0.0
-    - updated for ptlibs 1.0.0
-    - code refactorization
-0.0.1 - 0.0.2
-    - Alpha releases
-```
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
-
-ptcrossd is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+Copyright (c) 2024 Penterep Security s.r.o.
 
-ptcrossd is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ptcrossd is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+ptcrossd is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
 
-You should have received a copy of the GNU General Public License along with ptcrossd. If not, see https://www.gnu.org/licenses/.
+You should have received a copy of the GNU General Public License
+along with ptcrossd.  If not, see <https://www.gnu.org/licenses/>.
 
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
```

### Comparing `ptcrossd-1.0.2/README.md` & `ptcrossd-1.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,85 +1,77 @@
-[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
-
-
-# PTCROSSD
-
-> crossdomain.xml misconfigurations testing tool
-
-## Installation
-```
-pip install ptcrossd
-```
-
-## Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
-
-> Add to PATH for Bash
-```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
-source ~/.bashrc
-```
-
-> Add to PATH for ZSH
-```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
-source ~/.zshhrc
-```
-
-
-## Usage examples
-```
-ptcrossd -u https://www.example.com/crossdomain.xml
-ptcrossd -u https://www.example.com/
-```
-
-## Options
-
-```
--u   --url         <url>           Connect to URL
--p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--T   --timeout     <timeout>       Set timeout (default to 10)
--c   --cookie      <cookie>        Set cookie
--ua  --user-agent  <user-agent>    Set User-Agent header
--H   --headers     <header:value>  Set custom header(s)
--C   --cache                       Cache requests (load from tmp in future)
--v   --version                     Show script version and exit
--h   --help                        Show this help message and exit
--j   --json                        Output in JSON format
-```
-
-## Dependencies
-```
-defusedxml
-requests
-ptlibs
-```
-
-## Version History
-```
-1.0.2
-    - Full script rework
-1.0.1
-    - Fix urllib3 error
-1.0.0
-    - updated for ptlibs 1.0.0
-    - code refactorization
-0.0.1 - 0.0.2
-    - Alpha releases
-```
-## License
-
-Copyright (c) 2023 Penterep Security s.r.o.
-
-ptcrossd is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
-
-ptcrossd is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with ptcrossd. If not, see https://www.gnu.org/licenses/.
-
-## Warning
-
-You are only allowed to run the tool against the websites which
-you have been given permission to pentest. We do not accept any
-responsibility for any damage/harm that this application causes to your
-computer, or your network. Penterep is not responsible for any illegal
-or malicious use of this code. Be Ethical!
+[![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
+
+## PTCROSSD - Crossdomain.xml Testing Tool
+
+## Installation
+
+```
+pip install ptcrossd
+```
+
+## Adding to PATH
+If you're unable to invoke the script from your terminal, it's likely because it's not included in your PATH. You can resolve this issue by executing the following commands, depending on the shell you're using:
+
+For Bash Users
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
+source ~/.bashrc
+```
+
+For ZSH Users
+```bash
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
+source ~/.zshrc
+```
+
+## Usage examples
+```
+ptcrossd -u https://www.example.com/crossdomain.xml
+ptcrossd -u https://www.example.com/
+```
+
+## Options
+```
+-u   --url                  <url>           Connect to URL
+-cf  --cross-domain-file                    Test crossdomain.xml file
+-ch  --cross-origin-header                  Test Access-Control-Allow-Origin header
+-p   --proxy                <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T   --timeout              <timeout>       Set timeout (default to 10)
+-c   --cookie               <cookie>        Set cookie
+-a   --user-agent           <user-agent>    Set User-Agent header
+-H   --headers              <header:value>  Set custom header(s)
+-C   --cache                                Cache requests (load from tmp in future)
+-v   --version                              Show script version and exit
+-h   --help                                 Show this help message and exit
+-j   --json                                 Output in JSON format
+```
+
+## Dependencies
+```
+ptlibs
+defusedxml
+```
+
+## License
+
+Copyright (c) 2024 Penterep Security s.r.o.
+
+ptcrossd is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+ptcrossd is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with ptcrossd.  If not, see <https://www.gnu.org/licenses/>.
+
+## Warning
+
+You are only allowed to run the tool against the websites which
+you have been given permission to pentest. We do not accept any
+responsibility for any damage/harm that this application causes to your
+computer, or your network. Penterep is not responsible for any illegal
+or malicious use of this code. Be Ethical!
```

### Comparing `ptcrossd-1.0.2/ptcrossd/ptcrossd.py` & `ptcrossd-1.0.3/ptcrossd/ptcrossd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/python3
 """
-    Copyright (c) 2023 Penterep Security s.r.o.
+    Copyright (c) 2024 Penterep Security s.r.o.
 
-    ptcrossd - crossdomain.xml misconfigurations testing tool
+    ptcrossd - Crossdomain.xml Testing Tool
 
     ptcrossd is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     ptcrossd is distributed in the hope that it will be useful,
@@ -35,71 +35,90 @@
     def __init__(self, args):
         self.ptjsonlib   = ptjsonlib.PtJsonLib()
         self.headers     = ptnethelper.get_request_headers(args)
         self.use_json    = args.json
         self.timeout     = args.timeout
         self.cache       = args.cache
         self.proxies     = {"http": args.proxy, "https": args.proxy}
+        self.file_test   = args.cross_domain_file
+        self.header_test = args.cross_origin_header
         self._validate_url(args.url)
-        self._set_tests(args)
+        if not any([args.cross_domain_file, args.cross_origin_header]):
+            self.file_test = self.header_test = True
 
     def run(self, args) -> None:
         if self.use_json:
             if self.file_test:
                 url_path, url = self._adjust_url(args.url)
-                self._test_url(url, url_path)
+                self._test_crossdomain(url, url_path)
             if self.header_test:
-                self._test_headers_only(args.url)
-            self.ptjsonlib.set_status("ok")
+                self._test_headers(args.url)
+            self.ptjsonlib.set_status("finished")
             ptprinthelper.ptprint(self.ptjsonlib.get_result_json())
-
         else:
             if self.file_test:
-                urls = self._get_paths_for_crossdomain(args.url)
-                for index, url in enumerate(urls):
-                    if index != 0: ptprinthelper.ptprint(" ", "", not self.use_json)
-                    self._test_url(url)
-            if not self.file_test and self.header_test:
-                self._test_headers_only(args.url)
+                url_list = self._get_paths_for_crossdomain(args.url)
+                for url in url_list:
+                    if url != url_list[-1]: ptprinthelper.ptprint(" ", "", not self.use_json)
+                    if self._test_crossdomain(url):
+                        args.url = url
+                        break
+            if self.header_test:
+                self._test_headers(args.url)
+
+    def _test_crlf(self, url, header_name) -> None:
+        headers = self.headers.copy()
+        headers.update({header_name: "test%0D%0Atestcrlf:crlf"})
+        r, r_dump = self._get_response(url)
+
+        if r.headers.get("testcrlf"):
+            ptprinthelper.ptprint(f"Header {header_name} is vulnerable to CRLF injection", "VULN", not self.use_json)
+            self.ptjsonlib.add_vulnerability(f"PTV-WEB-INJECT-CORS{header_name.capitalize()[0]}CSRF")
+
+    def _test_headers(self, url) -> None:
+        ptprinthelper.ptprint(f"Testing: Access-Control-Allow-Origin header", "TITLE", not self.use_json, colortext=True, newline_above=False)
+        headers = self.headers.copy()
+        headers.update({"Referer": "https://test-cors-referer.com", "Origin": "https://test-cors-origin.com"})
+        response, response_dump = self._get_response(url, headers=headers)
 
-    def _test_headers_only(self, url) -> None:
-        ptprinthelper.ptprint(f"Testing: {url}", "TITLE", not self.use_json, colortext=True)
-        response, response_dump = self._get_response(url)
         if response.headers.get("Access-Control-Allow-Origin"):
             if response.headers.get("Access-Control-Allow-Origin") == "*":
                 ptprinthelper.ptprint("Open CORS vulnerability detected in Access-Control-Allow-Origin header", "VULN", not self.use_json)
-                self.ptjsonlib.add_vulnerability("PTWV-OPEN-CORS-HEADER", request=response_dump["request"], response=response_dump["response"])
+                self.ptjsonlib.add_vulnerability("PTV-WEB-HTTP-CORSS", vuln_request=response_dump["request"], vuln_response=response_dump["response"])
+
+            if response.headers.get("Access-Control-Allow-Origin") == "https://test-cors-referer.com":
+                ptprinthelper.ptprint("Reflecting Referer header to Access-Control-Allow-Origin header", "VULN", not self.use_json)
+                self.ptjsonlib.add_vulnerability("PTV-WEB-HTTP-CORSR", vuln_request=response_dump["request"], vuln_response=response_dump["response"])
+                self._test_crlf(url, header_name="Referer")
+
+            if response.headers.get("Access-Control-Allow-Origin") == "https://test-cors-origin.com":
+                ptprinthelper.ptprint("Reflecting Origin header to Access-Control-Allow-Origin header", "VULN", not self.use_json)
+                self.ptjsonlib.add_vulnerability("PTV-WEB-HTTP-CORSO", vuln_request=response_dump["request"], vuln_response=response_dump["response"])
+                self._test_crlf(url, header_name="Origin")
+
         else:
             ptprinthelper.ptprint(f'Header Access-Control-Allow-Origin is not present', "INFO", not self.use_json)
 
-    def _test_url(self, url, url_path=None) -> None:
+    def _test_crossdomain(self, url, url_path=None) -> bool:
         ptprinthelper.ptprint(f"Testing: {url}", "TITLE", not self.use_json, colortext=True)
         response, response_dump = self._get_response(url)
-
-        ptprinthelper.ptprint(f"Returned Content-Type: '{response.headers.get('Content-Type')}'", "INFO", not self.use_json)
-        if self.header_test and not self.use_json:
-            if response.headers.get("Access-Control-Allow-Origin"):
-                ptprinthelper.ptprint(f'Access-Control-Allow-Origin: {response.headers.get("Access-Control-Allow-Origin")}', "INFO", not self.use_json)
-            else:
-                ptprinthelper.ptprint(f'Header Access-Control-Allow-Origin is not present', "INFO", not self.use_json)
+        ptprinthelper.ptprint(f"Returned Status Code: {response.status_code}", "INFO", not self.use_json)
 
         if response.status_code == 200:
+            self._process_crossdomain(response, response_dump)
             if self.use_json:
-                self.ptjsonlib.add_node(self.ptjsonlib.create_node_object("webpage", properties={"url": url, "name": url_path, "WebPageType": "crossdomain.xml"}))
-            self._process_crossdomain_xml(response, response_dump)
+                self.ptjsonlib.add_node(self.ptjsonlib.create_node_object("webSource", properties={"url": url, "name": url_path, "webSourceType": "crossdomain.xml"}))
+            return True
         else:
+            ptprinthelper.ptprint(f"crossdomain.xml not found", "INFO", not self.use_json, end="\n\n")
             self.ptjsonlib.set_message("crossdomain.xml not found")
-            ptprinthelper.ptprint(f"crossdomain.xml not found", "INFO", not self.use_json)
+            return False
 
-        if self.header_test and not self.use_json:
-            if response.headers.get("Access-Control-Allow-Origin"):
-                if response.headers.get("Access-Control-Allow-Origin") == "*":
-                    ptprinthelper.ptprint("Open CORS vulnerability detected in Access-Control-Allow-Origin header", "VULN", not self.use_json)
 
-    def _process_crossdomain_xml(self, response, response_dump) -> None:
+    def _process_crossdomain(self, response, response_dump) -> None:
         try:
             tree = DEFUSED_ET.fromstring(response.text)
         except DEFUSED_ET.ParseError:
             ptprinthelper.ptprint(f"Error parsing provided XML file", "ERROR", not self.use_json)
             self.ptjsonlib.set_message("Error parsing provided XML file")
             return
         except DEFUSED_ET.EntitiesForbidden:
@@ -124,34 +143,35 @@
             for acf_element in acf_elements:
                 if "domain" in acf_element.keys() and acf_element.attrib["domain"] == "*":
                     is_open_cors = True
                 if "secure" in acf_element.keys() and not acf_element.attrib["secure"]:
                     http_allowed = True
             if is_open_cors:
                 ptprinthelper.ptprint("Open CORS vulnerability detected in crossdomain.xml file", "VULN", not self.use_json)
-                self.ptjsonlib.add_vulnerability("PTWV-OPEN-CORS-FILE", request=response_dump["request"], response=response_dump["response"])
+                self.ptjsonlib.add_vulnerability("PTV-WEB-HTTP-CROSSD", vuln_request=response_dump["request"], vuln_response=response_dump["response"])
             if http_allowed:
                 ptprinthelper.ptprint("Non-secure communication detected in crossdomain.xml file", "VULN", not self.use_json)
 
         if not is_open_cors:
             self.ptjsonlib.set_message(response.text)
 
     def _adjust_url(self, url: str) -> tuple[str, str]:
+        """Adjusts a given URL to ensure it points to a 'crossdomain.xml' file."""
         parsed_url = urllib.parse.urlparse(url)
         if not parsed_url.path.endswith("/crossdomain.xml"):
-            if parsed_url.path in ["/", ""]:
+            if parsed_url.path in ["", "/"]:
                 parsed_url = parsed_url._replace(path="/crossdomain.xml")
             else:
                 directories = [d for d in parsed_url.path.split("/") if d]
-                if "." in directories[-1]:
-                    directories.pop()
+                if "." in directories[-1]: directories.pop()
                 parsed_url = parsed_url._replace(path='/'.join(directories) + "/crossdomain.xml")
         return (parsed_url.path if not parsed_url.path.startswith("/") else parsed_url.path[1:], urllib.parse.urlunparse((parsed_url.scheme, parsed_url.netloc, parsed_url.path, "", "", "")))
 
     def _get_paths_for_crossdomain(self, url) -> list:
+        """Generates a list of URLs pointing to potential 'crossdomain.xml' locations based on the given URL."""
         parsed_url = urllib.parse.urlparse(url)
         result = []
         if parsed_url.path not in ["/", ""]:
             directories = [d for d in parsed_url.path.split("/") if d]
             if "." in directories[-1]:
                 directories.pop()
             while directories:
@@ -164,62 +184,56 @@
     def _validate_url(self, url: str) -> None:
         parsed_url = urllib.parse.urlparse(url)
         if not re.match("https?$", parsed_url.scheme):
             self.ptjsonlib.end_error("Missing or wrong scheme, only HTTP(s) schemas are supported", self.use_json)
         if not parsed_url.netloc:
             self.ptjsonlib.end_error("Provided URL is not valid", self.use_json)
 
-    def _set_tests(self, args) -> None:
-        if not args.cross_domain_file and not args.cross_origin_header:
-            self.header_test = True
-            self.file_test = True
-        else:
-            self.file_test = args.cross_domain_file
-            self.header_test = args.cross_origin_header
-
-    def _get_response(self, url: str):
+    def _get_response(self, url: str, headers: dict|None = None):
+        if not headers:
+            headers = self.headers
         try:
-            response, response_dump = ptmisclib.load_url_from_web_or_temp(url, method="GET", headers=self.headers, proxies=self.proxies, timeout=self.timeout, redirects=False, verify=False, cache=self.cache, dump_response=True)
+            response, response_dump = ptmisclib.load_url_from_web_or_temp(url, method="GET", headers=headers, proxies=self.proxies, timeout=self.timeout, redirects=True, verify=False, cache=self.cache, dump_response=True)
             return response, response_dump
         except requests.RequestException:
             self.ptjsonlib.end_error(f"Cannot connect to server", self.use_json)
 
 
 def get_help():
     return [
-        {"description": ["crossdomain.xml misconfigurations testing tool"]},
+        {"description": ["Crossdomain.xml Testing Tool"]},
         {"usage": ["ptcrossd <options>"]},
         {"usage_example": [
             "ptcrossd -u https://www.example.com/crossdomain.xml",
             "ptcrossd -u https://www.example.com/",
 
         ]},
         {"options": [
             ["-u",  "--url",                    "<url>",            "Connect to URL"],
             ["-cf",  "--cross-domain-file",     "",                 "Test crossdomain.xml file"],
             ["-ch", "--cross-origin-header",    "",                 "Test Access-Control-Allow-Origin header"],
             ["-p",  "--proxy",                  "<proxy>",          "Set proxy (e.g. http://127.0.0.1:8080)"],
             ["-T",  "--timeout",                "<timeout>",        "Set timeout (default to 10)"],
             ["-c",  "--cookie",                 "<cookie>",         "Set cookie"],
-            ["-ua", "--user-agent",             "<user-agent>",     "Set User-Agent header"],
+            ["-a", "--user-agent",              "<user-agent>",     "Set User-Agent header"],
             ["-H",  "--headers",                "<header:value>",   "Set custom header(s)"],
             ["-C",  "--cache",                  "",                 "Cache requests (load from tmp in future)"],
             ["-v",  "--version",                "",                 "Show script version and exit"],
             ["-h",  "--help",                   "",                 "Show this help message and exit"],
             ["-j",  "--json",                   "",                 "Output in JSON format"],
         ]
         }]
 
 
 def parse_args():
     parser = argparse.ArgumentParser(add_help="False")
     parser.add_argument("-u",   "--url",                 type=str, required=True)
     parser.add_argument("-p",   "--proxy",               type=str)
     parser.add_argument("-c",   "--cookie",              type=str)
-    parser.add_argument("-ua",  "--user-agent",          type=str, default="Penterep Tools")
+    parser.add_argument("-a",  "--user-agent",           type=str, default="Penterep Tools")
     parser.add_argument("-T",   "--timeout",             type=int, default=10)
     parser.add_argument("-H",   "--headers",             type=ptmisclib.pairs, nargs="+")
     parser.add_argument("-cf",  "--cross-domain-file",   action="store_true")
     parser.add_argument("-ch",  "--cross-origin-header", action="store_true")
     parser.add_argument("-j",   "--json",                action="store_true")
     parser.add_argument("-C",   "--cache",               action="store_true")
     parser.add_argument("-v",   "--version",             action="version", version=f"{SCRIPTNAME} {__version__}")
```

### Comparing `ptcrossd-1.0.2/ptcrossd.egg-info/PKG-INFO` & `ptcrossd-1.0.3/ptcrossd.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,99 @@
 Metadata-Version: 2.1
 Name: ptcrossd
-Version: 1.0.2
-Summary: crossdomain.xml misconfigurations testing tool
+Version: 1.0.3
+Summary: Crossdomain.xml Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
-License: GPLv3+
+License: GPLv3
+Project-URL: homepage, https://www.penterep.com/
+Project-URL: repository, https://github.com/penterep/ptcrossd
+Project-URL: tracker, https://github.com/penterep/ptcrossd/issues
+Project-URL: changelog, https://github.com/penterep/ptcrossd/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Topic :: Security
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Requires-Python: >=3.6
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ptlibs<2,>=1.0.7
+Requires-Dist: defusedxml
 
 [![penterepTools](https://www.penterep.com/external/penterepToolsLogo.png)](https://www.penterep.com/)
 
-
-# PTCROSSD
-
-> crossdomain.xml misconfigurations testing tool
+## PTCROSSD - Crossdomain.xml Testing Tool
 
 ## Installation
+
 ```
 pip install ptcrossd
 ```
 
-## Add to PATH
-If you cannot invoke the script in your terminal, its probably because its not in your PATH. Fix it by running commands below.
+## Adding to PATH
+If you're unable to invoke the script from your terminal, it's likely because it's not included in your PATH. You can resolve this issue by executing the following commands, depending on the shell you're using:
 
-> Add to PATH for Bash
+For Bash Users
 ```bash
 echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.bashrc
 source ~/.bashrc
 ```
 
-> Add to PATH for ZSH
+For ZSH Users
 ```bash
-echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshhrc
-source ~/.zshhrc
+echo "export PATH=\"`python3 -m site --user-base`/bin:\$PATH\"" >> ~/.zshrc
+source ~/.zshrc
 ```
 
-
 ## Usage examples
 ```
 ptcrossd -u https://www.example.com/crossdomain.xml
 ptcrossd -u https://www.example.com/
 ```
 
 ## Options
-
 ```
--u   --url         <url>           Connect to URL
--p   --proxy       <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
--T   --timeout     <timeout>       Set timeout (default to 10)
--c   --cookie      <cookie>        Set cookie
--ua  --user-agent  <user-agent>    Set User-Agent header
--H   --headers     <header:value>  Set custom header(s)
--C   --cache                       Cache requests (load from tmp in future)
--v   --version                     Show script version and exit
--h   --help                        Show this help message and exit
--j   --json                        Output in JSON format
+-u   --url                  <url>           Connect to URL
+-cf  --cross-domain-file                    Test crossdomain.xml file
+-ch  --cross-origin-header                  Test Access-Control-Allow-Origin header
+-p   --proxy                <proxy>         Set proxy (e.g. http://127.0.0.1:8080)
+-T   --timeout              <timeout>       Set timeout (default to 10)
+-c   --cookie               <cookie>        Set cookie
+-a   --user-agent           <user-agent>    Set User-Agent header
+-H   --headers              <header:value>  Set custom header(s)
+-C   --cache                                Cache requests (load from tmp in future)
+-v   --version                              Show script version and exit
+-h   --help                                 Show this help message and exit
+-j   --json                                 Output in JSON format
 ```
 
 ## Dependencies
 ```
-defusedxml
-requests
 ptlibs
+defusedxml
 ```
 
-## Version History
-```
-1.0.2
-    - Full script rework
-1.0.1
-    - Fix urllib3 error
-1.0.0
-    - updated for ptlibs 1.0.0
-    - code refactorization
-0.0.1 - 0.0.2
-    - Alpha releases
-```
 ## License
 
-Copyright (c) 2023 Penterep Security s.r.o.
-
-ptcrossd is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+Copyright (c) 2024 Penterep Security s.r.o.
 
-ptcrossd is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ptcrossd is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+ptcrossd is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
 
-You should have received a copy of the GNU General Public License along with ptcrossd. If not, see https://www.gnu.org/licenses/.
+You should have received a copy of the GNU General Public License
+along with ptcrossd.  If not, see <https://www.gnu.org/licenses/>.
 
 ## Warning
 
 You are only allowed to run the tool against the websites which
 you have been given permission to pentest. We do not accept any
 responsibility for any damage/harm that this application causes to your
 computer, or your network. Penterep is not responsible for any illegal
```

