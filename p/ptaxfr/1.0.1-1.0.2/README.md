# Comparing `tmp/ptaxfr-1.0.1.tar.gz` & `tmp/ptaxfr-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptaxfr-1.0.1.tar", last modified: Tue May  7 11:55:33 2024, max compression
+gzip compressed data, was "ptaxfr-1.0.2.tar", last modified: Thu May  9 17:22:20 2024, max compression
```

## Comparing `ptaxfr-1.0.1.tar` & `ptaxfr-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-07 11:55:33.500927 ptaxfr-1.0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:26:26.000000 ptaxfr-1.0.1/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3539 2024-05-07 11:55:33.500927 ptaxfr-1.0.1/PKG-INFO
--rwxr-xr-x   0 kali      (1000) kali      (1000)     2766 2024-05-07 11:51:11.000000 ptaxfr-1.0.1/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-07 11:55:33.500927 ptaxfr-1.0.1/ptaxfr/
--rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:26.000000 ptaxfr-1.0.1/ptaxfr/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)       23 2024-04-29 08:26:26.000000 ptaxfr-1.0.1/ptaxfr/_version.py
--rwxr-xr-x   0 kali      (1000) kali      (1000)    14239 2024-04-30 09:55:08.000000 ptaxfr-1.0.1/ptaxfr/ptaxfr.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-07 11:55:33.500927 ptaxfr-1.0.1/ptaxfr.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3539 2024-05-07 11:55:33.000000 ptaxfr-1.0.1/ptaxfr.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      263 2024-05-07 11:55:33.000000 ptaxfr-1.0.1/ptaxfr.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-07 11:55:33.000000 ptaxfr-1.0.1/ptaxfr.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       46 2024-05-07 11:55:33.000000 ptaxfr-1.0.1/ptaxfr.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       32 2024-05-07 11:55:33.000000 ptaxfr-1.0.1/ptaxfr.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        7 2024-05-07 11:55:33.000000 ptaxfr-1.0.1/ptaxfr.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-07 11:55:33.500927 ptaxfr-1.0.1/setup.cfg
--rwxr-xr-x   0 kali      (1000) kali      (1000)     1289 2024-05-07 11:50:53.000000 ptaxfr-1.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:22:20.746229 ptaxfr-1.0.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35823 2024-04-29 08:26:26.000000 ptaxfr-1.0.2/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3539 2024-05-09 17:22:20.746229 ptaxfr-1.0.2/PKG-INFO
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     2766 2024-05-07 11:51:11.000000 ptaxfr-1.0.2/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:22:20.746229 ptaxfr-1.0.2/ptaxfr/
+-rwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-29 08:26:26.000000 ptaxfr-1.0.2/ptaxfr/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       23 2024-05-09 17:18:37.000000 ptaxfr-1.0.2/ptaxfr/_version.py
+-rwxr-xr-x   0 kali      (1000) kali      (1000)    14421 2024-05-09 17:17:20.000000 ptaxfr-1.0.2/ptaxfr/ptaxfr.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-05-09 17:22:20.746229 ptaxfr-1.0.2/ptaxfr.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3539 2024-05-09 17:22:20.000000 ptaxfr-1.0.2/ptaxfr.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      263 2024-05-09 17:22:20.000000 ptaxfr-1.0.2/ptaxfr.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-05-09 17:22:20.000000 ptaxfr-1.0.2/ptaxfr.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       46 2024-05-09 17:22:20.000000 ptaxfr-1.0.2/ptaxfr.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       32 2024-05-09 17:22:20.000000 ptaxfr-1.0.2/ptaxfr.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        7 2024-05-09 17:22:20.000000 ptaxfr-1.0.2/ptaxfr.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-05-09 17:22:20.746229 ptaxfr-1.0.2/setup.cfg
+-rwxr-xr-x   0 kali      (1000) kali      (1000)     1289 2024-05-07 11:50:53.000000 ptaxfr-1.0.2/setup.py
```

### Comparing `ptaxfr-1.0.1/LICENSE` & `ptaxfr-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptaxfr-1.0.1/PKG-INFO` & `ptaxfr-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptaxfr
-Version: 1.0.1
+Version: 1.0.2
 Summary: DNS Zone Transfer Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptaxfr
```

### Comparing `ptaxfr-1.0.1/README.md` & `ptaxfr-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ptaxfr-1.0.1/ptaxfr/ptaxfr.py` & `ptaxfr-1.0.2/ptaxfr/ptaxfr.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     def run(self, args):
         """Main method"""
         if self.print_vulnerable_domains and not (self.print_records or self.print_subdomains):
             ptmisclib.ptprint("Vulnerable domains:", "TITLE", condition=self.use_json or not self.silent)
 
         self.ptthreads.threads(self.domains, self.ns_check, args.threads)
 
-        self.ptjsonlib.set_status("ok")
+        self.ptjsonlib.set_status("finished")
         ptprinthelper.ptprint(self.ptjsonlib.get_result_json(), "", self.use_json)
 
     def ns_check(self, domain: str) -> None:
         """Finds and tests all nameservers of <domain> for zone transfer"""
         printlock_instance  = printlock.PrintLock()
         resolver            = dns.resolver.Resolver()
         is_vulnerable       = False
@@ -93,19 +93,20 @@
             nameserver_ip = [str(ip) for ip in resolver.resolve(nameserver, "A")][0]
             nameserver_list.append({"nameserver": nameserver, "ns_ip": nameserver_ip, "vulnerable": "null", "dns_records": [], "subdomains": []})
             printlock_instance.add_string_to_output(ptprinthelper.out_ifnot(f"Nameserver: {nameserver}", "INFO", self.use_json or self.print_vulnerable_domains), silent=self.silent)
             printlock_instance.add_string_to_output(ptprinthelper.out_ifnot(f"IP: {nameserver_ip}", "INFO", self.use_json or self.print_vulnerable_domains), silent=self.silent)
             try:
                 zone = dns.zone.from_xfr(dns.query.xfr(nameserver_ip, domain, lifetime=5.0))
                 is_vulnerable = True
-                dns_records_data = self._extract_dns_records(zone)
-                subdomains_data =  self._extract_subdomains(zone)
+                dns_records_data = self._extract_dns_records(zone) if self.print_records else []
+                subdomains_data =  self._extract_subdomains(zone) if self.print_subdomains else []
                 nameserver_list[-1].update({"vulnerable": True, "zone": zone, "dns_records": dns_records_data, "subdomains": subdomains_data})
-                self.ptjsonlib.add_vulnerability(vuln_code="PTV-WEB-INFO-AXFR", vuln_request=f"nslookup -q=AXFR {nameserver}", vuln_response=dns_records_data)
                 printlock_instance.add_string_to_output(ptprinthelper.out_ifnot(f"Vulnerable: True", "VULN", self.use_json or self.print_vulnerable_domains, colortext=True), silent=self.silent, end="\n")
+                if self.use_json:
+                    self.ptjsonlib.add_vulnerability(vuln_code="PTV-WEB-INFO-AXFR", vuln_request=f"nslookup -q=AXFR {nameserver}", vuln_response=dns_records_data if self.print_records else [])
             except dns.exception.Timeout:
                 nameserver_list[-1].update({"vulnerable": False})
                 printlock_instance.add_string_to_output(ptprinthelper.out_ifnot(f"Timeout error", "ERROR", self.use_json or self.print_vulnerable_domains), silent=self.silent)
             except dns.exception.DNSException:
                 nameserver_list[-1].update({"vulnerable": False})
                 printlock_instance.add_string_to_output(ptprinthelper.out_ifnot(f"Vulnerable: False", "NOTVULN", self.use_json or self.print_vulnerable_domains, colortext=True), silent=self.silent, end="\n")
             except Exception as e:
@@ -149,15 +150,15 @@
         if self.unique:
             if self.print_records:
                 printlock_instance.add_string_to_output(ptprinthelper.out_ifnot('\n'.join(sorted(merged_dns_records)), "", self.use_json))
             if self.print_subdomains:
                 printlock_instance.add_string_to_output(ptprinthelper.out_ifnot('\n'.join(sorted(merged_subdomains)), "", self.use_json))
 
         for subdomain in sorted(merged_subdomains):
-            if subdomain != "*":
+            if subdomain != "*" and self.print_subdomains and self.use_json:
                 self.ptjsonlib.add_node(self.ptjsonlib.create_node_object('domain', properties={'name': subdomain}))
         if not self.use_json:
             printlock_instance.lock_print_output(end="\n" if not self.silent else "")
 
     def _extract_dns_records(self, zone):
         output_list = []
         data = []
```

### Comparing `ptaxfr-1.0.1/ptaxfr.egg-info/PKG-INFO` & `ptaxfr-1.0.2/ptaxfr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptaxfr
-Version: 1.0.1
+Version: 1.0.2
 Summary: DNS Zone Transfer Testing Tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3
 Project-URL: homepage, https://www.penterep.com/
 Project-URL: repository, https://github.com/penterep/ptaxfr
```

### Comparing `ptaxfr-1.0.1/setup.py` & `ptaxfr-1.0.2/setup.py`

 * *Files identical despite different names*

