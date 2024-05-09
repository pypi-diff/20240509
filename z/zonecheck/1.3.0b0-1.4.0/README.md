# Comparing `tmp/zonecheck-1.3.0b0.tar.gz` & `tmp/zonecheck-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zonecheck-1.3.0b0.tar", last modified: Fri Oct 22 22:56:04 2021, max compression
+gzip compressed data, was "zonecheck-1.4.0.tar", last modified: Thu May  9 12:41:20 2024, max compression
```

## Comparing `zonecheck-1.3.0b0.tar` & `zonecheck-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mauricio.vergara (451454889) staff       (20)        0 2021-10-22 22:56:04.026036 zonecheck-1.3.0b0/
--rw-r--r--   0 mauricio.vergara (451454889) staff       (20)    11357 2021-10-19 22:31:22.000000 zonecheck-1.3.0b0/LICENSE
--rw-r--r--   0 mauricio.vergara (451454889) staff       (20)     2619 2021-10-22 22:56:04.026265 zonecheck-1.3.0b0/PKG-INFO
--rw-r--r--   0 mauricio.vergara (451454889) staff       (20)     1222 2021-10-22 00:50:18.000000 zonecheck-1.3.0b0/README.md
-drwxr-xr-x   0 mauricio.vergara (451454889) staff       (20)        0 2021-10-22 22:56:04.023229 zonecheck-1.3.0b0/bin/
--rwxr-xr-x   0 mauricio.vergara (451454889) staff       (20)     2637 2021-10-22 17:26:01.000000 zonecheck-1.3.0b0/bin/axfrcheck
--rwxr-xr-x   0 mauricio.vergara (451454889) staff       (20)     5796 2021-10-22 17:32:58.000000 zonecheck-1.3.0b0/bin/zonecheck
--rwxr-xr-x   0 mauricio.vergara (451454889) staff       (20)     4123 2021-10-22 17:26:40.000000 zonecheck-1.3.0b0/bin/zonechecklite
--rw-r--r--   0 mauricio.vergara (451454889) staff       (20)       96 2021-10-22 01:21:49.000000 zonecheck-1.3.0b0/pyproject.toml
--rw-r--r--   0 mauricio.vergara (451454889) staff       (20)     1475 2021-10-22 22:56:04.027177 zonecheck-1.3.0b0/setup.cfg
--rw-r--r--   0 mauricio.vergara (451454889) staff       (20)       69 2021-10-22 01:22:08.000000 zonecheck-1.3.0b0/setup.py
-drwxr-xr-x   0 mauricio.vergara (451454889) staff       (20)        0 2021-10-22 22:56:04.023692 zonecheck-1.3.0b0/zonecheck/
--rwxr-xr-x   0 mauricio.vergara (451454889) staff       (20)    10630 2021-10-22 18:12:06.000000 zonecheck-1.3.0b0/zonecheck/__init__.py
-drwxr-xr-x   0 mauricio.vergara (451454889) staff       (20)        0 2021-10-22 22:56:04.025704 zonecheck-1.3.0b0/zonecheck.egg-info/
--rw-r--r--   0 mauricio.vergara (451454889) staff       (20)     2619 2021-10-22 22:56:04.000000 zonecheck-1.3.0b0/zonecheck.egg-info/PKG-INFO
--rw-r--r--   0 mauricio.vergara (451454889) staff       (20)      283 2021-10-22 22:56:04.000000 zonecheck-1.3.0b0/zonecheck.egg-info/SOURCES.txt
--rw-r--r--   0 mauricio.vergara (451454889) staff       (20)        1 2021-10-22 22:56:04.000000 zonecheck-1.3.0b0/zonecheck.egg-info/dependency_links.txt
--rw-r--r--   0 mauricio.vergara (451454889) staff       (20)      107 2021-10-22 22:56:04.000000 zonecheck-1.3.0b0/zonecheck.egg-info/requires.txt
--rw-r--r--   0 mauricio.vergara (451454889) staff       (20)       10 2021-10-22 22:56:04.000000 zonecheck-1.3.0b0/zonecheck.egg-info/top_level.txt
+drwxr-xr-x   0 john.bond (979230392) ICANN\Domain Users (1205227579)        0 2024-05-09 12:41:20.125291 zonecheck-1.4.0/
+-rw-r--r--   0 john.bond (979230392) ICANN\Domain Users (1205227579)    11357 2024-03-12 11:25:53.000000 zonecheck-1.4.0/LICENSE
+-rw-r--r--   0 john.bond (979230392) ICANN\Domain Users (1205227579)     2758 2024-05-09 12:41:20.124838 zonecheck-1.4.0/PKG-INFO
+-rw-r--r--   0 john.bond (979230392) ICANN\Domain Users (1205227579)     1222 2023-12-15 16:14:44.000000 zonecheck-1.4.0/README.md
+drwxr-xr-x   0 john.bond (979230392) ICANN\Domain Users (1205227579)        0 2024-05-09 12:41:20.116946 zonecheck-1.4.0/bin/
+-rwxr-xr-x   0 john.bond (979230392) ICANN\Domain Users (1205227579)     2637 2023-12-15 16:14:44.000000 zonecheck-1.4.0/bin/axfrcheck
+-rwxr-xr-x   0 john.bond (979230392) ICANN\Domain Users (1205227579)     5757 2024-03-12 14:43:11.000000 zonecheck-1.4.0/bin/zonecheck
+-rwxr-xr-x   0 john.bond (979230392) ICANN\Domain Users (1205227579)     4116 2024-03-12 14:43:11.000000 zonecheck-1.4.0/bin/zonechecklite
+-rw-r--r--   0 john.bond (979230392) ICANN\Domain Users (1205227579)       96 2023-12-15 16:14:44.000000 zonecheck-1.4.0/pyproject.toml
+-rw-r--r--   0 john.bond (979230392) ICANN\Domain Users (1205227579)     1469 2024-05-09 12:41:20.126546 zonecheck-1.4.0/setup.cfg
+-rw-r--r--   0 john.bond (979230392) ICANN\Domain Users (1205227579)       69 2023-12-15 16:14:44.000000 zonecheck-1.4.0/setup.py
+drwxr-xr-x   0 john.bond (979230392) ICANN\Domain Users (1205227579)        0 2024-05-09 12:41:20.117467 zonecheck-1.4.0/zonecheck/
+-rwxr-xr-x   0 john.bond (979230392) ICANN\Domain Users (1205227579)    10630 2023-12-15 16:14:44.000000 zonecheck-1.4.0/zonecheck/__init__.py
+drwxr-xr-x   0 john.bond (979230392) ICANN\Domain Users (1205227579)        0 2024-05-09 12:41:20.123480 zonecheck-1.4.0/zonecheck.egg-info/
+-rw-r--r--   0 john.bond (979230392) ICANN\Domain Users (1205227579)     2758 2024-05-09 12:41:20.000000 zonecheck-1.4.0/zonecheck.egg-info/PKG-INFO
+-rw-r--r--   0 john.bond (979230392) ICANN\Domain Users (1205227579)      283 2024-05-09 12:41:20.000000 zonecheck-1.4.0/zonecheck.egg-info/SOURCES.txt
+-rw-r--r--   0 john.bond (979230392) ICANN\Domain Users (1205227579)        1 2024-05-09 12:41:20.000000 zonecheck-1.4.0/zonecheck.egg-info/dependency_links.txt
+-rw-r--r--   0 john.bond (979230392) ICANN\Domain Users (1205227579)      107 2024-05-09 12:41:20.000000 zonecheck-1.4.0/zonecheck.egg-info/requires.txt
+-rw-r--r--   0 john.bond (979230392) ICANN\Domain Users (1205227579)       10 2024-05-09 12:41:20.000000 zonecheck-1.4.0/zonecheck.egg-info/top_level.txt
```

### Comparing `zonecheck-1.3.0b0/LICENSE` & `zonecheck-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zonecheck-1.3.0b0/PKG-INFO` & `zonecheck-1.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: zonecheck
-Version: 1.3.0b0
+Version: 1.4.0
 Summary: Helper libraries to check if DNS zonefiles configured on a server are the same as DNS master servers.
 Home-page: https://github.com/icann-dns/zonecheck
 Author: John Bond
 Author-email: pypi@johnbond.org
 License: License :: OSI Approved :: Apache Software License 2.0 (Apache-2.0)
 Project-URL: Bug Tracker, https://github.com/icann-dns/zonecheck/issues
 Keywords: dns,puppet
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -25,14 +24,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: Name Service (DNS)
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dnspython>=2.0.0; python_version >= "3.6"
+Requires-Dist: dnspython>=1.15; python_version < "3.0"
+Requires-Dist: pyyaml>=5.2
+Requires-Dist: future
 
 # Zonecheck
 Homepage: https://github.com/icann-dns/zonecheck
 
 ![GitHub issues](https://img.shields.io/github/issues/icann-dns/zonecheck?style=plastic)
 ![GitHub contributors](https://img.shields.io/github/contributors/icann-dns/zonecheck)
 ![GitHub](https://img.shields.io/github/license/icann-dns/zonecheck)
@@ -58,9 +61,7 @@
                         alert if the serial is behind by this value or more
   --log LOG             location of error file
   --puppet-facts
   --puppet-facts-dir PUPPET_FACTS_DIR
   --config CONFIG       comma seperated list of zones
   -v, --verbose
 ```
-
-
```

### Comparing `zonecheck-1.3.0b0/README.md` & `zonecheck-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `zonecheck-1.3.0b0/bin/axfrcheck` & `zonecheck-1.4.0/bin/axfrcheck`

 * *Files identical despite different names*

### Comparing `zonecheck-1.3.0b0/bin/zonecheck` & `zonecheck-1.4.0/bin/zonecheck`

 * *Files 9% similar despite different names*

```diff
@@ -92,19 +92,19 @@
 def get_facts_file(facts_dir, logger):
     possible_paths = [
             '/etc/puppetlabs/facter/facts.d',
             '/var/puppet/facts']
     if facts_dir == 'guess':
         for path in possible_paths:
             if os.path.exists(path):
-                return open(os.path.join(path, 'zone_status.txt'), 'w')
+                return open(os.path.join(path, 'zone_status.yaml'), 'w')
         logger.error('unable to guess facts dir')
         exit(1)
     elif os.path.exists(facts_dir):
-        return open(os.path.join(facts_dir, 'zone_status.txt'), 'w')
+        return open(os.path.join(facts_dir, 'zone_status.yaml'), 'w')
     else:
         loggin.error('invalid facts_dir: {}'.format(facts_dir))
         exit(1)
 
 def main():
     args = get_args()
     set_log_level(args.verbose)
@@ -144,15 +144,15 @@
     logger.error('errors:{}'.format(yaml.dump(errors)))
 
     if args.puppet_facts:
         # this is a safety so we dont disable all nodes if there is
         # a problem with the distribution layer
         if master_soa_error:
             facter_error = False
-        facts = 'zone_status_errors={}\n'.format(str(facter_error).lower())
-        logger.debug('puppet facts = {}'.format(facts))
+        facts = {'zone_status_errors': facter_error}
+        logger.debug(facts)
         facts_file = get_facts_file(args.puppet_facts_dir, logger)
-        facts_file.write(facts)
+        yaml.safe_dump(facts, facts_file)
         facts_file.close()
 
 if __name__ == '__main__':
     main()
```

### Comparing `zonecheck-1.3.0b0/bin/zonechecklite` & `zonecheck-1.4.0/bin/zonechecklite`

 * *Files 3% similar despite different names*

```diff
@@ -60,21 +60,21 @@
 def get_facts_file(facts_dir, logger):
     possible_paths = [
             '/etc/puppetlabs/facter/facts.d',
             '/var/puppet/facts']
     if facts_dir == 'guess':
         for path in possible_paths:
             if os.path.exists(path):
-                return open(os.path.join(path, 'zone_status.txt'), 'w')
+                return open(os.path.join(path, 'zone_status.yaml'), 'w')
         logger.error('unable to guess facts dir')
         exit(1)
     elif os.path.exists(facts_dir):
-        return open(os.path.join(facts_dir, 'zone_status.txt'), 'w')
+        return open(os.path.join(facts_dir, 'zone_status.yaml'), 'w')
     else:
-        loggin.error('invalid facts_dir: {}'.format(facts_dir))
+        logger.error('invalid facts_dir: {}'.format(facts_dir))
         exit(1)
 
 def main():
     args = get_args()
     set_log_level(args.verbose)
     logger = get_log_file(args.log)
     try:
@@ -102,15 +102,16 @@
     logger.error('errors:{}'.format(yaml.dump(errors)))
 
     if args.puppet_facts:
         # this is a safety so we dont disable all nodes if there is
         # a problem with the distribution layer
         if master_soa_error:
             facter_error = False
-        facts = 'zone_status_errors={}\n'.format(str(facter_error).lower())
-        logger.debug('puppet facts = {}'.format(facts))
+        facts = {'zone_status_errors': facter_error}
+        logger.debug(facts)
         facts_file = get_facts_file(args.puppet_facts_dir, logger)
+        yaml.safe_dump(facts, facts_file)
         facts_file.write(facts)
         facts_file.close()
 
 if __name__ == '__main__':
     main()
```

### Comparing `zonecheck-1.3.0b0/setup.cfg` & `zonecheck-1.4.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = zonecheck
-version = 1.3.0-beta0
+version = 1.4.0
 author = John Bond
 author_email = pypi@johnbond.org
 description = Helper libraries to check if DNS zonefiles configured on a server are the same as DNS master servers.
 keywords = 
 	dns
 	puppet
 license = License :: OSI Approved :: Apache Software License 2.0 (Apache-2.0)
```

### Comparing `zonecheck-1.3.0b0/zonecheck/__init__.py` & `zonecheck-1.4.0/zonecheck/__init__.py`

 * *Files identical despite different names*

### Comparing `zonecheck-1.3.0b0/zonecheck.egg-info/PKG-INFO` & `zonecheck-1.4.0/zonecheck.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: zonecheck
-Version: 1.3.0b0
+Version: 1.4.0
 Summary: Helper libraries to check if DNS zonefiles configured on a server are the same as DNS master servers.
 Home-page: https://github.com/icann-dns/zonecheck
 Author: John Bond
 Author-email: pypi@johnbond.org
 License: License :: OSI Approved :: Apache Software License 2.0 (Apache-2.0)
 Project-URL: Bug Tracker, https://github.com/icann-dns/zonecheck/issues
 Keywords: dns,puppet
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
@@ -25,14 +24,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: Name Service (DNS)
 Classifier: Topic :: System :: Networking :: Monitoring
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dnspython>=2.0.0; python_version >= "3.6"
+Requires-Dist: dnspython>=1.15; python_version < "3.0"
+Requires-Dist: pyyaml>=5.2
+Requires-Dist: future
 
 # Zonecheck
 Homepage: https://github.com/icann-dns/zonecheck
 
 ![GitHub issues](https://img.shields.io/github/issues/icann-dns/zonecheck?style=plastic)
 ![GitHub contributors](https://img.shields.io/github/contributors/icann-dns/zonecheck)
 ![GitHub](https://img.shields.io/github/license/icann-dns/zonecheck)
@@ -58,9 +61,7 @@
                         alert if the serial is behind by this value or more
   --log LOG             location of error file
   --puppet-facts
   --puppet-facts-dir PUPPET_FACTS_DIR
   --config CONFIG       comma seperated list of zones
   -v, --verbose
 ```
-
-
```

