# Comparing `tmp/ifstate-1.8.5.tar.gz` & `tmp/ifstate-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifstate-1.8.5.tar", last modified: Sat Jul  1 17:05:43 2023, max compression
+gzip compressed data, was "ifstate-1.9.0.tar", last modified: Thu Sep 14 18:31:15 2023, max compression
```

## Comparing `ifstate-1.8.5.tar` & `ifstate-1.9.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-01 17:05:32.000000 ifstate-1.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-01 17:05:43.761737 ifstate-1.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-01 17:05:32.000000 ifstate-1.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/ifstate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:32.000000 ifstate-1.8.5/ifstate/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7289 2023-07-01 17:05:32.000000 ifstate-1.8.5/ifstate/ifstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-01 17:05:32.000000 ifstate-1.8.5/ifstate/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/ifstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-01 17:05:43.000000 ifstate-1.8.5/ifstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-01 17:05:43.000000 ifstate-1.8.5/ifstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 17:05:43.000000 ifstate-1.8.5/ifstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-01 17:05:43.000000 ifstate-1.8.5/ifstate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-01 17:05:43.000000 ifstate-1.8.5/ifstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-01 17:05:43.000000 ifstate-1.8.5/ifstate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/libifstate/
--rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/libifstate/address/
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/address/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/libifstate/bpf/
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/bpf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/bpf/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/bpf/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/libifstate/brport/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/brport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/link/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22757 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/link/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/link/physical.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/link/tun.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/link/veth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/neighbour/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/neighbour/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/parser/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/routing/
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/routing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/sysctl/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/sysctl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/tc/
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/wireguard/
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/wireguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.761737 ifstate-1.8.5/libifstate/xdp/
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-01 17:05:32.000000 ifstate-1.8.5/libifstate/xdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 17:05:43.757737 ifstate-1.8.5/schema/
--rw-r--r--   0 runner    (1001) docker     (123)   178382 2023-07-01 17:05:32.000000 ifstate-1.8.5/schema/ifstate.conf.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 17:05:43.761737 ifstate-1.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-01 17:05:32.000000 ifstate-1.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.928499 ifstate-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-09-14 18:31:03.000000 ifstate-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2023-09-14 18:31:15.928499 ifstate-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2023-09-14 18:31:03.000000 ifstate-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.920499 ifstate-1.9.0/ifstate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:03.000000 ifstate-1.9.0/ifstate/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7533 2023-09-14 18:31:03.000000 ifstate-1.9.0/ifstate/ifstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2023-09-14 18:31:03.000000 ifstate-1.9.0/ifstate/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.920499 ifstate-1.9.0/ifstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2023-09-14 18:31:15.000000 ifstate-1.9.0/ifstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2023-09-14 18:31:15.000000 ifstate-1.9.0/ifstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 18:31:15.000000 ifstate-1.9.0/ifstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2023-09-14 18:31:15.000000 ifstate-1.9.0/ifstate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-09-14 18:31:15.000000 ifstate-1.9.0/ifstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-09-14 18:31:15.000000 ifstate-1.9.0/ifstate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.924499 ifstate-1.9.0/libifstate/
+-rw-r--r--   0 runner    (1001) docker     (127)    27197 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.924499 ifstate-1.9.0/libifstate/address/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/address/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.924499 ifstate-1.9.0/libifstate/bpf/
+-rw-r--r--   0 runner    (1001) docker     (127)     7699 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/bpf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/bpf/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/bpf/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.924499 ifstate-1.9.0/libifstate/brport/
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/brport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.924499 ifstate-1.9.0/libifstate/link/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26758 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/link/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/link/physical.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/link/tun.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/link/veth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.924499 ifstate-1.9.0/libifstate/neighbour/
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/neighbour/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.924499 ifstate-1.9.0/libifstate/netns/
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/netns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.928499 ifstate-1.9.0/libifstate/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/parser/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.928499 ifstate-1.9.0/libifstate/routing/
+-rw-r--r--   0 runner    (1001) docker     (127)    16831 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/routing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.928499 ifstate-1.9.0/libifstate/sysctl/
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/sysctl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.928499 ifstate-1.9.0/libifstate/tc/
+-rw-r--r--   0 runner    (1001) docker     (127)    11211 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.928499 ifstate-1.9.0/libifstate/wireguard/
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/wireguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.928499 ifstate-1.9.0/libifstate/xdp/
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2023-09-14 18:31:03.000000 ifstate-1.9.0/libifstate/xdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:31:15.924499 ifstate-1.9.0/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)   188621 2023-09-14 18:31:03.000000 ifstate-1.9.0/schema/ifstate.conf.schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-14 18:31:15.928499 ifstate-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-09-14 18:31:03.000000 ifstate-1.9.0/setup.py
```

### Comparing `ifstate-1.8.5/LICENSE` & `ifstate-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.5/PKG-INFO` & `ifstate-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifstate
-Version: 1.8.5
+Version: 1.9.0
 Summary: Manage host interface settings in a declarative manner
 Home-page: https://ifstate.net/
 Author: Thomas Liske
 Author-email: thomas@fiasko-nw.net
 License: GPL3+
 Description-Content-Type: text/markdown
 Provides-Extra: shell
```

### Comparing `ifstate-1.8.5/README.md` & `ifstate-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.5/ifstate/ifstate.py` & `ifstate-1.9.0/ifstate/ifstate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 from libifstate.parser import YamlParser
 from libifstate import __version__, IfState
-from libifstate.exception import FeatureMissingError, LinkNoConfigFound, ParserValidationError, ParserOpenError, ParserParseError, ParserIncludeError
+from libifstate.exception import FeatureMissingError, LinkNoConfigFound, LinkCircularLinked, ParserValidationError, ParserOpenError, ParserParseError, ParserIncludeError
 from libifstate.util import logger, IfStateLogging
 from collections import namedtuple
 from copy import deepcopy
 from setproctitle import setproctitle
 
 import argparse
 import logging
@@ -161,14 +161,17 @@
             exit(ex.exit_code())
 
         if args.action == Actions.CHECK:
             try:
                 ifs_config.ifs.check()
             except LinkNoConfigFound:
                 pass
+            except LinkCircularLinked as ex:
+                ifslog.quit()
+                exit(ex.exit_code())
         elif args.action == Actions.VRRP_FIFO:
             signal.signal(signal.SIGHUP, ifs_config.sighup_handler)
             signal.signal(signal.SIGPIPE, signal.SIG_IGN)
             signal.signal(signal.SIGTERM, signal.SIG_IGN)
 
             status_pattern = re.compile(
                 r'(group|instance) "([^"]+)" (unknown|fault|backup|master)( \d+)?$', re.IGNORECASE)
@@ -191,13 +194,16 @@
                 if args.action == Actions.APPLY:
                     ifs_config.ifs.apply()
                 elif args.action == Actions.VRRP:
                     ifs_config.ifs.apply(
                         args.type, args.name, args.state)
             except LinkNoConfigFound:
                 pass
+            except LinkCircularLinked as ex:
+                ifslog.quit()
+                exit(ex.exit_code())
 
         ifslog.quit()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ifstate-1.8.5/ifstate/shell.py` & `ifstate-1.9.0/ifstate/shell.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import rlcompleter
 import atexit
 import code
 import os
 import readline
 
 import pprint
-from libifstate.util import ipr
+from libifstate.netns import NetNameSpace
 
 has_pygments = False
 try:
     from pygments import highlight
     from pygments.lexers import PythonLexer
     from pygments.formatters import TerminalFormatter
 
@@ -29,14 +29,16 @@
                  histfile=os.path.expanduser("~/.ifstate_history")):
 
         # use pygments for print() if available
         print_func = pprint.pprint
         if has_pygments:
             print_func = pygments_print
 
+        ipr = NetNameSpace(None).ipr
+
         print("Links:")
         for link in ipr.get_links():
             print("  {:2}: {}".format(
                 link.get('index'), link.get_attr('IFLA_IFNAME')))
         print("")
```

### Comparing `ifstate-1.8.5/ifstate.egg-info/PKG-INFO` & `ifstate-1.9.0/ifstate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifstate
-Version: 1.8.5
+Version: 1.9.0
 Summary: Manage host interface settings in a declarative manner
 Home-page: https://ifstate.net/
 Author: Thomas Liske
 Author-email: thomas@fiasko-nw.net
 License: GPL3+
 Description-Content-Type: text/markdown
 Provides-Extra: shell
```

### Comparing `ifstate-1.8.5/ifstate.egg-info/SOURCES.txt` & `ifstate-1.9.0/ifstate.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 libifstate/brport/__init__.py
 libifstate/link/__init__.py
 libifstate/link/base.py
 libifstate/link/physical.py
 libifstate/link/tun.py
 libifstate/link/veth.py
 libifstate/neighbour/__init__.py
+libifstate/netns/__init__.py
 libifstate/parser/__init__.py
 libifstate/parser/base.py
 libifstate/parser/yaml.py
 libifstate/routing/__init__.py
 libifstate/sysctl/__init__.py
 libifstate/tc/__init__.py
 libifstate/wireguard/__init__.py
```

### Comparing `ifstate-1.8.5/libifstate/__init__.py` & `ifstate-1.9.0/libifstate/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from libifstate.exception import LinkDuplicate
 from libifstate.link.base import ethtool_path, Link
 from libifstate.address import Addresses
 from libifstate.neighbour import Neighbours
 from libifstate.routing import Tables, Rules, RTLookups
-from libifstate.sysctl import Sysctl
 from libifstate.parser import Parser
 from libifstate.tc import TC
 from libifstate.exception import netlinkerror_classes
 
 from pyroute2.netlink.rtnl.ifaddrmsg import IFA_F_PERMANENT
 try:
     from libifstate.wireguard import WireGuard
@@ -27,48 +26,38 @@
     except ModuleNotFoundError:
         # ignore missing plugin
         pass
 except ModuleNotFoundError:
     # ignore missing plugin
     pass
 
-from libifstate.util import logger, ipr, IfStateLogging
+from libifstate.netns import NetNameSpace, prepare_netns, get_netns_instances, LinkRegistry
+from libifstate.util import logger, IfStateLogging, LinkDependency
 from libifstate.exception import FeatureMissingError, LinkCircularLinked, LinkNoConfigFound, ParserValidationError
 from ipaddress import ip_network, ip_interface
 from jsonschema import validate, ValidationError, FormatChecker
 from copy import deepcopy
 import os
 import pkgutil
 import re
 import json
 import errno
 import logging
 
-__version__ = "1.8.5"
+__version__ = "1.9.0"
 
 
 class IfState():
     def __init__(self):
         logger.debug('IfState {}'.format(__version__))
-        self.links = {}
-        self.addresses = {}
-        self.bpf_progs = None
-        self.neighbours = {}
+
+        self.namespaces = None
+        self.root_netns = NetNameSpace(None)
+        self.defaults = []
         self.ignore = {}
-        self.vrrp = {
-            'links': [],
-            'group': {},
-            'instance': {},
-        }
-        self.tables = None
-        self.rules = None
-        self.sysctl = Sysctl()
-        self.tc = {}
-        self.wireguard = {}
-        self.xdp = {}
         self.features = {
             'brport': True,
             'link': True,
             'sysctl': os.access('/proc/sys/net', os.R_OK),
             'ethtool': not ethtool_path is None,
             'tc': True,
             'wireguard': not globals().get("WireGuard") is None,
@@ -104,81 +93,117 @@
             else:
                 detail = ex.message
             if soft_schema:
                 logger.error("Config validation failed for {}".format(detail))
             else:
                 raise ParserValidationError(detail)
 
+        # add interface defaults
+        if 'defaults' in ifstates:
+            self.defaults = ifstates['defaults']
+
+        # add ignore list items
+        self.ignore.update(ifstates['ignore'])
+        self.ipaddr_ignore = set()
+        for ip in self.ignore.get('ipaddr', []):
+            self.ipaddr_ignore.add(ip_network(ip))
+
+        # save cshaper profiles
+        self.cshaper_profiles = ifstates['cshaper']
+
+        # build link registry over all named netns
+        self.link_registry = LinkRegistry(
+            self.ignore.get('ifname', []),
+            self.root_netns,
+            *get_netns_instances())
+
+        self._update(self.root_netns, ifstates)
+        if 'namespaces' in ifstates:
+            self.namespaces = {}
+            for netns_name, netns_ifstates in ifstates['namespaces'].items():
+                self.namespaces[netns_name] = NetNameSpace(netns_name)
+                self._update(self.namespaces[netns_name], netns_ifstates)
+
+    def _update(self, netns, ifstates):
         # parse options
         if 'options' in ifstates:
             # parse global sysctl settings
             if 'sysctl' in ifstates['options']:
                 for iface in ['all', 'default']:
                     if iface in ifstates['options']['sysctl']:
-                        self.sysctl.add(
+                        netns.sysctl.add(
                             iface, ifstates['options']['sysctl'][iface])
 
         # load BPF programs
         if 'bpf' in ifstates:
             if not self.features['bpf']:
                 raise FeatureMissingError("bpf")
 
-            if self.bpf_progs is None:
-                self.bpf_progs = BPF()
+            if netns.bpf_progs is None:
+                netns.bpf_progs = BPF(netns)
             for name, config in ifstates['bpf'].items():
-                self.bpf_progs.add(name, config)
+                netns.bpf_progs.add(name, config)
 
         # add interfaces from config
         for ifstate in ifstates['interfaces']:
+            defaults = self.get_defaults(
+                ifname=ifstate['name'],
+                kind=ifstate['link']['kind'])
+
             name = ifstate['name']
-            if name in self.links:
+            if name in netns.links:
                 raise LinkDuplicate()
+            link = {}
+            if 'link' in defaults:
+                link.update(defaults['link'])
             if 'link' in ifstate:
-                self.links[name] = Link(
-                    name, ifstate['link'], ifstate.get('ethtool'), ifstate.get('vrrp'), ifstate.get('brport'))
+                link.update(ifstate['link'])
+            if link:
+                netns.links[name] = Link(self,
+                    netns, name, link, ifstate.get('ethtool'), ifstate.get('vrrp'), ifstate.get('brport'))
             else:
-                self.links[name] = None
+                netns.links[name] = None
 
             if 'addresses' in ifstate:
-                self.addresses[name] = Addresses(name, ifstate['addresses'])
-            else:
-                self.addresses[name] = None
+                netns.addresses[name] = Addresses(netns, name, ifstate['addresses'])
+            elif defaults.get('clear_addresses', False):
+                netns.addresses[name] = Addresses(netns, name, [])
 
             if 'neighbours' in ifstate:
-                self.neighbours[name] = Neighbours(name, ifstate['neighbours'])
-            else:
-                self.neighbours[name] = None
+                netns.neighbours[name] = Neighbours(netns, name, ifstate['neighbours'])
+            elif defaults.get('clear_neighbours', False):
+                netns.neighbours[name] = Neighbours(netns, name, [])
 
             if 'vrrp' in ifstate:
                 ktype = ifstate['vrrp']['type']
                 kname = ifstate['vrrp']['name']
                 kstates = ifstate['vrrp']['states']
-                if not kname in self.vrrp[ktype]:
-                    self.vrrp[ktype][kname] = {}
+                if not kname in netns.vrrp[ktype]:
+                    netns.vrrp[ktype][kname] = {}
                 for kstate in kstates:
-                    if not kstate in self.vrrp[ktype][kname]:
-                        self.vrrp[ktype][kname][kstate] = []
-                    self.vrrp[ktype][kname][kstate].append(name)
-                self.vrrp['links'].append(name)
+                    if not kstate in netns.vrrp[ktype][kname]:
+                        netns.vrrp[ktype][kname][kstate] = []
+                    netns.vrrp[ktype][kname][kstate].append(name)
+                netns.vrrp['links'].append(name)
 
             if 'sysctl' in ifstate:
-                self.sysctl.add(name, ifstate['sysctl'])
+                netns.sysctl.add(name, ifstate['sysctl'])
 
             if 'cshaper' in ifstate:
                 profile_name = ifstate['cshaper'].get(
                     'profile', 'default')
                 logger.debug('cshaper profile {} enabled'.format(profile_name),
-                             extra={'iface': name})
-                cshaper_profile = ifstates['cshaper'][profile_name]
+                             extra={'iface': name, 'netns': netns})
+                cshaper_profile = deepcopy(self.cshaper_profiles[profile_name])
 
                 # ingress
                 ifb_name = re.sub(
                     cshaper_profile['ingress_ifname']['search'], cshaper_profile['ingress_ifname']['replace'], name)
                 logger.debug('cshaper ifb name {}'.format(ifb_name),
-                             extra={'iface': name})
+                             extra={'iface': name, 'netns': netns})
 
                 ifb_state = {
                     'name': ifb_name,
                     'link': {
                         'state': 'up',
                         'kind': 'ifb',
                     },
@@ -190,15 +215,15 @@
                     'ingress', 'unlimited')
 
                 ifstates['interfaces'].append(ifb_state)
 
                 # egress
                 if 'tc' in ifstate:
                     logger.warning(
-                        'cshaper settings replaces tc settings', extra={'iface': name})
+                        'cshaper settings replaces tc settings', extra={'iface': name, 'netns': netns})
 
                 ifstate['tc'] = {
                     'ingress': True,
                     'qdisc': cshaper_profile['egress_qdisc'],
                     'filter': [
                         {
                             'kind': 'matchall',
@@ -218,288 +243,351 @@
 
                 ifstate['tc']['qdisc']['bandwidth'] = ifstate['cshaper'].get(
                     'egress', 'unlimited')
 
                 del ifstate['cshaper']
 
             if 'tc' in ifstate:
-                self.tc[name] = TC(
-                    name, ifstate['tc'])
+                netns.tc[name] = TC(
+                    netns, name, ifstate['tc'])
 
             if 'wireguard' in ifstate:
                 if not self.features['wireguard']:
                     raise FeatureMissingError("wireguard")
 
-                self.wireguard[name] = WireGuard(name, ifstate['wireguard'])
+                netns.wireguard[name] = WireGuard(netns, name, ifstate['wireguard'])
 
             if 'xdp' in ifstate:
                 if not self.features['xdp']:
                     raise FeatureMissingError("xdp")
 
-                self.xdp[name] = XDP(name, ifstate['xdp'])
+                netns.xdp[name] = XDP(netns, name, ifstate['xdp'])
 
         # add routing from config
         if 'routing' in ifstates:
             if 'routes' in ifstates['routing']:
-                if self.tables is None:
-                    self.tables = Tables()
+                if netns.tables is None:
+                    netns.tables = Tables(netns)
                 for route in ifstates['routing']['routes']:
-                    self.tables.add(route)
+                    netns.tables.add(route)
 
             if 'rules' in ifstates['routing']:
-                if self.rules is None:
-                    self.rules = Rules()
+                if netns.rules is None:
+                    netns.rules = Rules(netns)
                 for rule in ifstates['routing']['rules']:
-                    self.rules.add(rule)
-
-        # add ignore list items
-        self.ignore.update(ifstates['ignore'])
+                    netns.rules.add(rule)
 
     def apply(self, vrrp_type=None, vrrp_name=None, vrrp_state=None):
         self._apply(True, vrrp_type, vrrp_name, vrrp_state)
 
     def check(self, vrrp_type=None, vrrp_name=None, vrrp_state=None):
         self._apply(False, vrrp_type, vrrp_name, vrrp_state)
 
-    def _apply(self, do_apply, vrrp_type, vrrp_name, vrrp_state):
-        vrrp_ignore = []
-        vrrp_disable = []
+    def free_registry_item(self, do_apply, item):
+        ifname = item.attributes['ifname']
+
+        log_str = ifname
+        if item.netns.netns is not None:
+            log_str += "[netns={}]".format(item.netns.netns)
+
+        if item.attributes['kind'] != 'physical':
+            # remove virtual interface
+            logger.log_del(log_str)
+            if do_apply:
+                try:
+                    item.netns.ipr.link('set', index=item.attributes['index'], state='down')
+                    item.netns.ipr.link('del', index=item.attributes['index'])
+                except Exception as err:
+                    if not isinstance(err, netlinkerror_classes):
+                        raise
+                    logger.warning('removing link {} failed: {}'.format(
+                        ifname, err.args[1]), extra={'netns': item.netns})
+            return True
+        else:
+            # shutdown physical interfaces
+            logger.log_del(log_str, 'orphan')
+            if do_apply:
+                try:
+                    item.netns.ipr.link('set', index=item.attributes['index'], state='down')
+                except Exception as err:
+                    if not isinstance(err, netlinkerror_classes):
+                        raise
+                    logger.warning('updating link {} failed: {}'.format(
+                        ifname, err.args[1]), extra={'netns': item.netns})
+            return False
+
+    def _dependencies(self, netns):
+        deps = {}
+        for ifname, link in netns.links.items():
+            deps[LinkDependency(ifname, netns.netns)] = link.depends()
+
+        for ifname, tc in netns.tc.items():
+            for fltr in tc.tc.get('filter', []):
+                for action in fltr.get('action', []):
+                    if 'dev' in action:
+                        link = LinkDependency(ifname, netns.netns)
+                        dep = LinkDependency(action['dev'], netns.netns)
+                        if link in deps:
+                            deps[link].append(dep)
+                        else:
+                            deps[link] = [dep]
+
+        return deps
 
+    def _stages(self, continue_on_circualar):
+        def dep(arg):
+            '''
+                Dependency resolver
+
+            "arg" is a dependency dictionary in which
+            the values are the dependencies of their respective keys.
+            '''
+            d=dict((k, set(arg[k])) for k in arg)
+            r=[]
+            while d:
+                # values not in keys (items without dep)
+                t=set(i for v in d.values() for i in v)-set(d.keys())
+                # and keys without value (items without dep)
+                t.update(k for k, v in d.items() if not v)
+
+                if len(t) == 0:
+                    logger.error("Circualar link dependency detected: ")
+                    for k, v in d.items():
+                        logger.error('  {} => {}'.format(k, ", ".join(map(str, v))))
+                    logger.error("")
+
+                    if continue_on_circualar:
+                        # remaining link deps cannot be resolved, drop them
+                        # if we shall continue
+                        return r
+                    else:
+                        raise LinkCircularLinked()
+
+                # can be done right away
+                r.append(t)
+                # and cleaned up
+                d=dict(((k, v-t) for k, v in d.items() if v))
+            return r
+
+        dependencies = self._dependencies(self.root_netns)
+        if self.namespaces is not None:
+            for netns in self.namespaces.values():
+                dependencies.update(self._dependencies(netns))
+
+        if logger.getEffectiveLevel() <= logging.DEBUG:
+            logger.debug('dependencies dump:')
+            for ifname, deps in dependencies.items():
+                logger.debug('  %s => %s', ifname, ", ".join(map(str, deps)))
+
+        stages = dep(dependencies)
+
+        if logger.getEffectiveLevel() <= logging.DEBUG:
+            logger.debug('stages dump:')
+            i = 1
+            for stage in stages:
+                logger.debug('  #%d => %s', i, ", ".join(map(str, stage)))
+                i += 1
+
+        return stages
+
+    def _apply(self, do_apply, vrrp_type=None, vrrp_name=None, vrrp_state=None):
+        # check if called from vrrp hook and ignore non-vrrp interfaces
         by_vrrp = not None in [
             vrrp_type, vrrp_name, vrrp_state]
-
         if by_vrrp:
-            logger.info("vrrp state change: {} {} => {}".format(vrrp_type, vrrp_name, vrrp_state))
+            logger.info("triggered by vrrp state change")
+            logger.log_change("{} {}".format(vrrp_type, vrrp_name), vrrp_state)
+            logger.info("")
 
             # ifstate schema requires lower case keywords
             vrrp_type = vrrp_type.lower()
             vrrp_state = vrrp_state.lower()
 
-        # check which links to remove or ignore:
-        #   remove: vrrp type & name matches, but vrrp state not
-        #   ignore: vrrp type & name does not match
-        for ifname, link in self.links.items():
-            if ifname in self.vrrp['links']:
-                if not by_vrrp:
-                    vrrp_ignore.append(ifname)
-                else:
-                    if not link.match_vrrp_select(vrrp_type, vrrp_name):
-                        vrrp_ignore.append(ifname)
-                    elif not vrrp_name in self.vrrp[vrrp_type] or not vrrp_state in self.vrrp[vrrp_type][vrrp_name] or not ifname in self.vrrp[vrrp_type][vrrp_name][vrrp_state]:
-                        vrrp_disable.append(ifname)
-            elif by_vrrp:
-                vrrp_ignore.append(ifname)
-        logger.debug("vrrp links to be disabled: {}".format(", ".join(vrrp_disable)))
-        logger.debug("vrrp links to be ignored: {}".format(", ".join(vrrp_ignore)))
-
-        self.ipaddr_ignore = set()
-        for ip in self.ignore.get('ipaddr', []):
-            self.ipaddr_ignore.add(ip_network(ip))
-
-        if not any(not x is None for x in self.links.values()):
-            logger.error("DANGER: Not a single link config has been found!")
-            raise LinkNoConfigFound()
-
-        for iface in ['all', 'default']:
-            if self.sysctl.has_settings(iface):
-                logger.info("\nconfiguring {} interface sysctl".format(iface))
-                self.sysctl.apply(iface, do_apply)
-
-        if not self.bpf_progs is None:
-            self.bpf_progs.apply(do_apply)
-
-        for stage in range(2):
-            if stage == 0:
-                logger.info("\nconfiguring interface links")
-
-                for ifname in vrrp_disable:
-                    logger.debug('to be disabled due to vrrp constraint',
-                                 extra={'iface': ifname})
-                    self.links[ifname].settings['state'] = 'down'
-            else:
-                logger.info("\nconfiguring interface links (stage 2)")
-
-            retry = False
-            applied = []
-            while len(applied) + len(vrrp_ignore) < len(self.links):
-                last = len(applied)
-                for name, link in self.links.items():
-                    if name in applied:
-                        continue
-
-                    if name in vrrp_ignore:
-                        logger.debug('skipped due to vrrp constraint',
-                                     extra={'iface': name})
-                        continue
-
-                    if link is None:
-                        logger.debug('skipped due to no link settings',
-                                     extra={'iface': name})
-                        applied.append(name)
-                    else:
-                        deps = link.depends()
-                        if all(x in applied+vrrp_ignore for x in deps):
-                            excpts = link.apply(do_apply, self.sysctl)
-                            if excpts.has_errno(errno.EEXIST):
-                                retry = True
-                            applied.append(name)
-                if last == len(applied):
-                    raise LinkCircularLinked()
-
-            for link in ipr.get_links():
-                name = link.get_attr('IFLA_IFNAME')
-                # skip links on ignore list
-                if not name in self.links and not any(re.match(regex, name) for regex in self.ignore.get('ifname', [])):
-                    info = link.get_attr('IFLA_LINKINFO')
-                    # remove virtual interface
-                    if info is not None:
-                        kind = info.get_attr('IFLA_INFO_KIND')
-                        logger.info(
-                            'del', extra={'iface': name, 'style': IfStateLogging.STYLE_DEL})
-                        if do_apply:
-                            try:
-                                ipr.link('set', index=link.get(
-                                    'index'), state='down')
-                                ipr.link('del', index=link.get('index'))
-                            except Exception as err:
-                                if not isinstance(err, netlinkerror_classes):
-                                    raise
-                                logger.warning('removing link {} failed: {}'.format(
-                                    name, err.args[1]))
-                    # shutdown physical interfaces
-                    else:
-                        if name in vrrp_ignore:
-                            logger.warning('vrrp', extra={
-                                'iface': name, 'style': IfStateLogging.STYLE_OK})
-                        if link.get('state') == 'down':
-                            logger.warning('orphan', extra={
-                                'iface': name, 'style': IfStateLogging.STYLE_OK})
+        # create and destroy namespaces to match config
+        if not by_vrrp and self.namespaces is not None:
+            prepare_netns(do_apply, self.namespaces.keys())
+            logger.info("")
+
+        # get link dependency tree
+        stages = self._stages(do_apply)
+
+        # remove any orphan (non-ignored) links
+        if not by_vrrp:
+            had_cleanup = False
+            cleanup_items = []
+            for item in self.link_registry.registry:
+                ifname = item.attributes['ifname']
+                # items without a link are orphan - keep them if they match the ignore regex list...
+                if item.link is None and not any(re.match(regex, ifname) for regex in self.ignore.get('ifname', [])):
+                    # ...or are in a netns namespace while the config has no `namespaces` setting
+                    if self.namespaces is not None or item.netns.netns is None:
+                        if not had_cleanup:
+                            logger.info("cleanup orphan interfaces...")
+                            had_cleanup = True
+                        if self.free_registry_item(do_apply, item):
+                            cleanup_items.append(item)
                         else:
-                            logger.warning('orphan', extra={
-                                'iface': name, 'style': IfStateLogging.STYLE_CHG})
-                            if do_apply:
-                                try:
-                                    ipr.link('set', index=link.get(
-                                        'index'), state='down')
-                                except Exception as err:
-                                    if not isinstance(err, netlinkerror_classes):
-                                        raise
-                                    logger.warning('updating link {} failed: {}'.format(
-                                        name, err.args[1]))
-            if not retry:
-                break
-
-        if any(not x is None for x in self.tc.values()):
-            logger.info("\nconfiguring interface traffic control...")
-
-            for name, tc in self.tc.items():
-                if name in vrrp_ignore:
-                    logger.debug('skipped due to vrrp constraint',
-                                 extra={'iface': name})
-                elif tc is None:
-                    logger.debug('skipped due to no tc settings', extra={
-                                 'iface': name})
-                else:
-                    tc.apply(do_apply)
-
-        if any(not x is None for x in self.xdp.values()):
-            logger.info("\nconfiguring eXpress Data Path...")
-
-            for name, xdp in self.xdp.items():
-                if name in vrrp_ignore:
-                    logger.debug('skipped due to vrrp constraint',
-                                 extra={'iface': name})
-                elif xdp is None:
-                    logger.debug('skipped due to no xdp settings', extra={
-                                 'iface': name})
-                else:
-                    xdp.apply(do_apply, self.bpf_progs)
+                            item.attributes['orphan'] = True
 
-        if any(not x is None for x in self.addresses.values()):
-            logger.info("\nconfiguring interface ip addresses...")
-            # add empty objects for unhandled interfaces
-            for link in ipr.get_links():
-                name = link.get_attr('IFLA_IFNAME')
-                # skip links on ignore list
-                if not name in self.addresses and not any(re.match(regex, name) for regex in self.ignore.get('ifname', [])):
-                    self.addresses[name] = Addresses(name, [])
-
-            for name, addresses in self.addresses.items():
-                if name in vrrp_ignore:
-                    logger.debug('skipped due to vrrp constraint',
-                                 extra={'iface': name})
-                elif addresses is None:
-                    logger.debug('skipped due to no address settings', extra={
-                                 'iface': name})
+            if cleanup_items:
+                for item in cleanup_items:
+                    self.link_registry.registry.remove(item)
+
+            if had_cleanup:
+                logger.info("")
+
+        # dump link registry in verbose mode
+        if logger.getEffectiveLevel() <= logging.DEBUG:
+            self.link_registry.debug_dump()
+
+        if not by_vrrp:
+            # apply bpf settings
+            had_bpf = self._apply_bpf(do_apply, self.root_netns)
+            if self.namespaces is not None:
+                for name, netns in self.namespaces.items():
+                    had_bpf = self._apply_bpf(do_apply, netns, had_bpf)
+            if had_bpf:
+                logger.info("")
+
+            # apply sysctl settings
+            had_sysctl = self._apply_sysctl(do_apply, self.root_netns)
+            if self.namespaces is not None:
+                for name, netns in self.namespaces.items():
+                    had_sysctl = self._apply_sysctl(do_apply, netns, had_sysctl)
+            if had_sysctl:
+                logger.info("")
+
+        # create/modify links in order of dependencies
+        logger.info("configure interfaces...")
+        for stage in stages:
+            for link_dep in sorted(stage):
+                logger.info(" {}".format(link_dep))
+                if link_dep.netns is None:
+                    self._apply_iface(do_apply, self.root_netns, link_dep.ifname, by_vrrp, vrrp_type, vrrp_name, vrrp_state)
                 else:
-                    addresses.apply(self.ipaddr_ignore, self.ignore.get(
-                        'ipaddr_dynamic', True), do_apply)
-        else:
-            logger.debug("\nno interface ip addressing to be applied")
+                    self._apply_iface(do_apply, self.namespaces[link_dep.netns], link_dep.ifname, by_vrrp, vrrp_type, vrrp_name, vrrp_state)
 
-        if any(not x is None for x in self.neighbours.values()):
-            logger.info("\nconfiguring interface neighbours...")
-            # add empty objects for unhandled interfaces
-            for link in ipr.get_links():
-                name = link.get_attr('IFLA_IFNAME')
-                # skip links on ignore list
-                if not name in self.neighbours and not any(re.match(regex, name) for regex in self.ignore.get('ifname', [])):
-                    self.neighbours[name] = Neighbours(name, [])
-
-            for name, neighbours in self.neighbours.items():
-                if name in vrrp_ignore:
-                    logger.debug('skipped due to vrrp constraint',
-                                 extra={'iface': name})
-                elif neighbours is None:
-                    logger.debug('skipped due to no address settings', extra={
-                                 'iface': name})
-                else:
-                    neighbours.apply(do_apply)
-        else:
-            logger.debug("\nno interface neighbours to be applied")
+        # configure routing
+        logger.info("")
+        logger.info("configure routing...")
+        self._apply_routing(do_apply, self.root_netns)
+        if self.namespaces is not None:
+            for name, netns in self.namespaces.items():
+                self._apply_routing(do_apply, netns)
+
+    def _apply_bpf(self, do_apply, netns, had_bpf=False):
+        if not netns.bpf_progs is None:
+            if not had_bpf:
+                logger.info("load BPF programs...")
+                had_bpf = True
+            netns.bpf_progs.apply(do_apply)
 
-        if not self.tables is None:
-            self.tables.apply(self.ignore.get('routes', []), do_apply)
+        return had_bpf
 
-        if not self.rules is None:
-            self.rules.apply(self.ignore.get('rules', []), do_apply)
+    def _apply_sysctl(self, do_apply, netns, had_sysctl=False):
+        for iface in ['all', 'default']:
+            if netns.sysctl.has_settings(iface):
+                if not had_sysctl:
+                    logger.info("configure sysctl settings...")
+                    had_sysctl = True
+                netns.sysctl.apply(iface, do_apply)
+        return had_sysctl
+
+    def _apply_iface(self, do_apply, netns, ifname, by_vrrp, vrrp_type, vrrp_name, vrrp_state):
+        if ifname in netns.links:
+            link = netns.links[ifname]
+
+        # check for vrrp mode:
+        #   disable: vrrp type & name matches, but vrrp state not
+        #   ignore : vrrp type & name does not match
+        if ifname in netns.vrrp['links']:
+            # this is a vrrp link but not running in a vrrp action
+            if not by_vrrp:
+                return
+            else:
+                # skip if another vrrp type & name is addressed
+                if not link.match_vrrp_select(vrrp_type, vrrp_name):
+                    logger.log_ok("other vrrp")
+                    return
+                # vrrp type & name does match, but the state does not => disable this interface
+                elif not vrrp_name in netns.vrrp[vrrp_type] or not vrrp_state in netns.vrrp[vrrp_type][vrrp_name] or not ifname in netns.vrrp[vrrp_type][vrrp_name][vrrp_state]:
+                    if ifname in netns.links:
+                        logger.debug('to be disabled due to vrrp constraint',
+                                    extra={'iface': ifname})
+                        link.settings['state'] = 'down'
+        # ignore if this link is not vrrp aware at all
+        elif by_vrrp:
+            logger.log_ok("no vrrp")
+            return
+
+        if ifname in netns.links:
+            excpts = link.apply(do_apply, netns.sysctl)
+            if excpts.has_errno(errno.EEXIST):
+                retry = True
+
+        if ifname in netns.tc:
+            netns.tc[ifname].apply(do_apply)
+
+        if ifname in netns.xdp:
+            netns.xdp[ifname].apply(do_apply, netns.bpf_progs)
+
+        if ifname in netns.addresses and netns.addresses[ifname]:
+            netns.addresses[ifname].apply(self.ipaddr_ignore, self.ignore.get(
+                'ipaddr_dynamic', True), do_apply)
+
+        if ifname in netns.neighbours:
+            netns.neighbours[ifname].apply(do_apply)
+
+        if ifname in netns.wireguard:
+            netns.wireguard[ifname].apply(do_apply)
+
+    def _apply_routing(self, do_apply, netns):
+        if not netns.tables is None:
+            netns.tables.apply(self.ignore.get('routes', []), do_apply)
 
-        if len(self.wireguard):
-            logger.info("\nconfiguring WireGuard...")
-            for iface, wireguard in self.wireguard.items():
-                if iface in vrrp_ignore:
-                    logger.debug('skipped due to vrrp constraint',
-                                 extra={'iface': name})
-                    continue
-                wireguard.apply(do_apply)
+        if not netns.rules is None:
+            netns.rules.apply(self.ignore.get('rules', []), do_apply)
 
     def show(self, showall=False):
         if showall:
             defaults = deepcopy(Parser._default_ifstates)
         else:
             defaults = {}
 
         ipaddr_ignore = []
         for ip in Parser._default_ifstates['ignore']['ipaddr_builtin']:
             ipaddr_ignore.append(ip_network(ip))
 
+        root_config = self._show_netns(self.root_netns, showall, ipaddr_ignore)
+        netns_instances = get_netns_instances()
+        if len(netns_instances) > 0:
+            netns_configs = {}
+            for netns in netns_instances:
+                netns_configs[netns.netns] = self._show_netns(netns, showall, ipaddr_ignore)
+
+            return {**defaults, **root_config, 'namespaces': netns_configs}
+
+
+        return {**defaults, **root_config}
+
+    def _show_netns(self, netns, showall, ipaddr_ignore):
         ifs_links = []
-        for ipr_link in ipr.get_links():
+        for ipr_link in netns.ipr.get_links():
             name = ipr_link.get_attr('IFLA_IFNAME')
             # skip links on ignore list
             if not any(re.match(regex, name) for regex in Parser._default_ifstates['ignore']['ifname_builtin']):
                 ifs_link = {
                     'name': name,
                     'addresses': [],
                     'link': {
                         'state': ipr_link['state'],
                     },
                 }
 
-                for addr in ipr.get_addr(index=ipr_link['index']):
+                for addr in netns.ipr.get_addr(index=ipr_link['index']):
                     if addr['flags'] & IFA_F_PERMANENT == IFA_F_PERMANENT:
                         ip = ip_interface(addr.get_attr(
                             'IFA_ADDRESS') + '/' + str(addr['prefixlen']))
                         if not any(ip in net for net in ipaddr_ignore):
                             ifs_link['addresses'].append(ip.with_prefixlen)
 
                 info = ipr_link.get_attr('IFLA_LINKINFO')
@@ -524,49 +612,66 @@
                                 else:
                                     ifs_link['link'][attr] = v
                 else:
                     ifs_link['link']['kind'] = 'physical'
                     addr = ipr_link.get_attr('IFLA_ADDRESS')
                     if not addr is None:
                         ifs_link['link']['address'] = addr
-                    permaddr = ipr.get_permaddr(name)
+                    permaddr = netns.ipr.get_permaddr(name)
                     if not permaddr is None:
                         if addr is None:
                             ifs_link['link']['addr'] = permaddr
                         elif addr != permaddr:
                             ifs_link['link']['permaddr'] = permaddr
-                    businfo = ipr.get_businfo(name)
+                    businfo = netns.ipr.get_businfo(name)
                     if not businfo is None:
                         ifs_link['link']['businfo'] = businfo
 
                 # add device group if not 0
                 group = ipr_link.get_attr('IFLA_GROUP')
                 if not group is None and group != 0:
                     ifs_link['link']['group'] = RTLookups.group.lookup_str(group)
 
                 for attr in ['link', 'master', 'gre_link', 'ip6gre_link', 'vxlan_link', 'xfrm_link']:
                     ref = ipr_link.get_attr('IFLA_{}'.format(attr.upper()))
                     if ref is not None:
                         try:
-                            ifs_link['link'][attr] = ipr.get_ifname_by_index(
+                            ifs_link['link'][attr] = netns.ipr.get_ifname_by_index(
                                 ref)
                         except Exception as err:
                             if not isinstance(err, netlinkerror_classes):
                                 raise
                             logger.warning('lookup {} failed: {}'.format(
-                                attr, err.args[1]), extra={'iface': name})
+                                attr, err.args[1]), extra={'iface': name, 'netns': netns})
                             ifs_link['link'][attr] = ref
 
                 mtu = ipr_link.get_attr('IFLA_MTU')
                 if not mtu is None and not mtu in [1500, 65536]:
                     ifs_link['link']['mtu'] = mtu
 
-                brport.BRPort.show(showall, ipr_link['index'], ifs_link)
+                brport.BRPort.show(netns.ipr, showall, ipr_link['index'], ifs_link)
 
                 ifs_links.append(ifs_link)
 
         routing = {
-            'routes': Tables().show_routes(Parser._default_ifstates['ignore']['routes_builtin']),
-            'rules': Rules().show_rules(Parser._default_ifstates['ignore']['rules_builtin']),
+            'routes': Tables(netns).show_routes(Parser._default_ifstates['ignore']['routes_builtin']),
+            'rules': Rules(netns).show_rules(Parser._default_ifstates['ignore']['rules_builtin']),
         }
 
-        return {**defaults, **{'interfaces': ifs_links, 'routing': routing}}
+        return {**{'interfaces': ifs_links, 'routing': routing}}
+
+
+    def get_defaults(self, **kwargs):
+        for default in self.defaults:
+            for match in default['match']:
+                matching = True
+
+                for option, regex in match.items():
+                    if not option in kwargs:
+                        matching = False
+                    elif not re.match(regex, kwargs[option]):
+                        matching = False
+
+                if matching:
+                    return default
+
+        return {}
```

### Comparing `ifstate-1.8.5/libifstate/address/__init__.py` & `ifstate-1.9.0/libifstate/address/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,64 @@
-from libifstate.util import logger, ipr, IfStateLogging
+from libifstate.util import logger, IfStateLogging
 from libifstate.exception import netlinkerror_classes
 from ipaddress import ip_interface
 from pyroute2.netlink.rtnl.ifaddrmsg import IFA_F_PERMANENT
 
 
 class Addresses():
-    def __init__(self, iface, addresses):
+    def __init__(self, netns, iface, addresses):
+        self.netns = netns
         self.iface = iface
         self.addresses = []
         for address in addresses:
             self.addresses.append(ip_interface(address))
 
     def apply(self, ignore, ign_dynamic, do_apply):
-        logger.debug('getting addresses', extra={'iface': self.iface})
+        logger.debug('getting addresses', extra={'iface': self.iface, 'netns': self.netns})
 
         # get ifindex
-        idx = next(iter(ipr.link_lookup(ifname=self.iface)), None)
+        idx = next(iter(self.netns.ipr.link_lookup(ifname=self.iface)), None)
 
         if idx == None:
-            logger.warning('link missing', extra={'iface': self.iface})
+            logger.warning('link missing', extra={'iface': self.iface, 'netns': self.netns})
             return
 
         # get active ip addresses
         ipr_addr = {}
         addr_add = []
-        for addr in ipr.get_addr(index=idx):
+        for addr in self.netns.ipr.get_addr(index=idx):
             ip = ip_interface(addr.get_attr('IFA_ADDRESS') +
                               '/' + str(addr['prefixlen']))
             ipr_addr[ip] = addr
 
         for addr in self.addresses:
             if addr in ipr_addr:
-                logger.info(' %s', addr.with_prefixlen, extra={
-                            'iface': self.iface, 'style': IfStateLogging.STYLE_OK})
+                logger.log_ok('addresses', '= {}'.format(addr.with_prefixlen))
                 del ipr_addr[addr]
             else:
                 addr_add.append(addr)
 
         for ip, addr in ipr_addr.items():
             if not any(ip in net for net in ignore):
                 if not ign_dynamic or ipr_addr[ip]['flags'] & IFA_F_PERMANENT == IFA_F_PERMANENT:
-                    logger.info(
-                        '-%s', ip.with_prefixlen, extra={'iface': self.iface, 'style': IfStateLogging.STYLE_DEL})
+                    logger.log_del('addresses', '- {}'.format(ip.with_prefixlen))
                     try:
                         if do_apply:
-                            ipr.addr("del", index=idx, address=str(
+                            self.netns.ipr.addr("del", index=idx, address=str(
                                 ip.ip), mask=ip.network.prefixlen)
                     except Exception as err:
                         if not isinstance(err, netlinkerror_classes):
                             raise
                         logger.warning('removing ip {}/{} failed: {}'.format(
                             str(ip.ip), ip.network.prefixlen, err.args[1]))
 
         for addr in addr_add:
-            logger.info('+%s', addr.with_prefixlen,
-                        extra={'iface': self.iface, 'style': IfStateLogging.STYLE_CHG})
+            logger.log_change('addresses', '+ {}'.format(addr.with_prefixlen))
             if do_apply:
                 try:
-                    ipr.addr("add", index=idx, address=str(
+                    self.netns.ipr.addr("add", index=idx, address=str(
                         addr.ip), mask=addr.network.prefixlen)
                 except Exception as err:
                     if not isinstance(err, netlinkerror_classes):
                         raise
                     logger.warning('adding ip {}/{} failed: {}'.format(
                         str(addr.ip), addr.network.prefixlen, err.args[1]))
```

### Comparing `ifstate-1.8.5/libifstate/bpf/__init__.py` & `ifstate-1.9.0/libifstate/bpf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,181 +1,193 @@
 from libifstate.util import logger, IfStateLogging
 from libifstate.bpf.map import BPF_Map
 from libifstate.bpf.ctypes import *
 import os
+import pyroute2.netns
 import shutil
 
 
 BPF_PROG_TYPE_XDP = 6
 
 bpfs_ifstate_dir = '/sys/fs/bpf/ifstate'
 
 
 class BPF():
-    def __init__(self):
+    def __init__(self, netns):
+        self.netns = netns
         self.bpf_fds = {}
         self.bpf_progs = {}
         self.bpf_tags = {}
 
     def add(self, name, config):
         self.bpf_progs[name] = config
 
     def apply(self, do_apply):
-        logger.info('\nloading BPF programs...')
-
         # prepare pinning directories
-        progs_pin_dir = "{}/progs".format(bpfs_ifstate_dir)
-        maps_pin_dir = "{}/maps".format(bpfs_ifstate_dir)
+        if self.netns.netns is None:
+            progs_pin_dir = "{}/progs".format(bpfs_ifstate_dir)
+            maps_pin_dir = "{}/maps".format(bpfs_ifstate_dir)
+        else:
+            progs_pin_dir = "{}/netns/{}/progs".format(bpfs_ifstate_dir, self.netns.netns)
+            maps_pin_dir = "{}/netns/{}/maps".format(bpfs_ifstate_dir, self.netns.netns)
+
         pinning = False
         if os.path.ismount('/sys/fs/bpf'):
             logger.debug('bpfs is mounted, enable pinning')
             pinning = True
 
             if do_apply:
                 os.makedirs(progs_pin_dir, exist_ok=True)
                 os.makedirs(maps_pin_dir, exist_ok=True)
         else:
             logger.debug('bpfs is not mounted, skipping pinning')
 
-        # load (and pin) bpf programs
-        for name, config in self.bpf_progs.items():
-            current_prog_tag = None
-            current_prog_fd = -1
-            self.bpf_tags[name] = None
-            self.bpf_fds[name] = -1
-
-            prog_pin_filename = "{}/{}".format(progs_pin_dir, name)
-            if os.path.isfile(prog_pin_filename):
-                current_prog_fd = libbpf.bpf_obj_get(
-                    os.fsencode(prog_pin_filename))
-
-                if current_prog_fd < 0:
-                    logger.warning('could not get current BPF obj fd for {}: {}'.format(
-                        name, os.strerror(-current_prog_fd)))
-                else:
-                    self.bpf_fds[name] = current_prog_fd
+        if self.netns.netns is not None:
+            pyroute2.netns.pushns(self.netns.netns)
 
-                    current_prog_info = struct_bpf_prog_info()
-                    current_prog_size = ctypes.c_uint(
-                        ctypes.sizeof(current_prog_info))
-                    rc = libbpf.bpf_obj_get_info_by_fd(current_prog_fd, ctypes.byref(
-                        current_prog_info), ctypes.byref(current_prog_size))
-                    if rc == 0:
-                        current_prog_tag = bytes(current_prog_info.tag).hex()
-                        self.bpf_tags[name] = current_prog_tag
+        try:
+            # load (and pin) bpf programs
+            for name, config in self.bpf_progs.items():
+                log_str = name
+                if self.netns.netns is not None:
+                    log_str += "[netns={}]".format(self.netns.netns)
+
+                current_prog_tag = None
+                current_prog_fd = -1
+                self.bpf_tags[name] = None
+                self.bpf_fds[name] = -1
+
+                prog_pin_filename = "{}/{}".format(progs_pin_dir, name)
+                if os.path.isfile(prog_pin_filename):
+                    current_prog_fd = libbpf.bpf_obj_get(
+                        os.fsencode(prog_pin_filename))
 
-                        logger.debug('current prog tag: {}'.format(current_prog_tag), extra={
-                            'iface': name})
+                    if current_prog_fd < 0:
+                        logger.warning('could not get current BPF obj fd for {}: {}'.format(
+                            log_str, os.strerror(-current_prog_fd)))
                     else:
-                        logger.warning('could not get current BPF obj info for {}: {}'.format(
-                            name, os.strerror(-rc)))
+                        self.bpf_fds[name] = current_prog_fd
 
-            # load new BPF prog
-            new_prog_tag = None
-            new_prog_fd = None
-
-            new_obj = libbpf.bpf_object__open_file(
-                os.fsencode(config["object"]),
-                None,
-            )
-            if not new_obj:
-                logger.warning('BPF open on {} failed: {}'.format(
-                    name, os.strerror(ctypes.get_errno())))
-                continue
-
-            logger.debug('loaded object: {}'.format(libbpf.bpf_object__name(new_obj).decode('ascii')), extra={
-                'iface': name})
-
-            rc = libbpf.bpf_object__load(new_obj)
-            if rc < 0:
-                logger.warning('BPF load on {} failed: {}'.format(
-                    name, os.strerror(-rc)))
-                continue
-
-            new_prog = libbpf.bpf_object__next_program(new_obj, None)
-            while new_prog:
-                section = libbpf.bpf_program__section_name(
-                    new_prog).decode('ascii')
-
-                logger.debug('  section: {}'.format(section), extra={
-                    'iface': name})
-
-                if section == config['section']:
-                    break
-                prog = libbpf.bpf_object__next_program(new_obj, new_prog)
-
-            if not new_prog:
-                logger.warning('BPF section {} on {} not found'.format(
-                    config['section'], name))
-                continue
-
-            # get prog fd
-            new_prog_fd = libbpf.bpf_program__fd(new_prog)
-            if not new_prog_fd:
-                logger.warning('BPF failed to get prog fd on {}'.format(
-                    name))
-                continue
-
-            # get new prog tag
-            info = struct_bpf_prog_info()
-            sz = ctypes.c_uint(ctypes.sizeof(info))
-            rc = libbpf.bpf_obj_get_info_by_fd(
-                new_prog_fd, ctypes.byref(info), ctypes.byref(sz))
-            if rc == 0:
-                new_prog_tag = bytes(info.tag).hex()
-
-                logger.debug('new prog tag: {}'.format(new_prog_tag), extra={
-                    'iface': name})
-
-                if current_prog_tag != new_prog_tag:
-                    self.bpf_fds[name] = new_prog_fd
-                    self.bpf_tags[name] = new_prog_tag
-
-                    if os.path.isfile(prog_pin_filename):
-                        os.unlink(prog_pin_filename)
-                    libbpf.bpf_program__pin(
-                        new_prog,
-                        os.fsencode(prog_pin_filename))
+                        current_prog_info = struct_bpf_prog_info()
+                        current_prog_size = ctypes.c_uint(
+                            ctypes.sizeof(current_prog_info))
+                        rc = libbpf.bpf_obj_get_info_by_fd(current_prog_fd, ctypes.byref(
+                            current_prog_info), ctypes.byref(current_prog_size))
+                        if rc == 0:
+                            current_prog_tag = bytes(current_prog_info.tag).hex()
+                            self.bpf_tags[name] = current_prog_tag
+
+                            logger.debug('current prog tag: {}'.format(current_prog_tag), extra={
+                                'iface': log_str})
+                        else:
+                            logger.warning('could not get current BPF obj info for {}: {}'.format(
+                                log_str, os.strerror(-rc)))
+
+                # load new BPF prog
+                new_prog_tag = None
+                new_prog_fd = None
+
+                new_obj = libbpf.bpf_object__open_file(
+                    os.fsencode(config["object"]),
+                    None,
+                )
+                if not new_obj:
+                    logger.warning('BPF open on {} failed: {}'.format(
+                        log_str, os.strerror(ctypes.get_errno())))
+                    continue
+
+                logger.debug('loaded object: {}'.format(libbpf.bpf_object__name(new_obj).decode('ascii')), extra={
+                    'iface': log_str})
+
+                rc = libbpf.bpf_object__load(new_obj)
+                if rc < 0:
+                    logger.warning('BPF load on {} failed: {}'.format(
+                        log_str, os.strerror(-rc)))
+                    continue
+
+                new_prog = libbpf.bpf_object__next_program(new_obj, None)
+                while new_prog:
+                    section = libbpf.bpf_program__section_name(
+                        new_prog).decode('ascii')
+
+                    logger.debug('  section: {}'.format(section), extra={
+                        'iface': log_str})
+
+                    if section == config['section']:
+                        break
+                    prog = libbpf.bpf_object__next_program(new_obj, new_prog)
+
+                if not new_prog:
+                    logger.warning('BPF section {} on {} not found'.format(
+                        config['section'], log_str))
+                    continue
+
+                # get prog fd
+                new_prog_fd = libbpf.bpf_program__fd(new_prog)
+                if not new_prog_fd:
+                    logger.warning('BPF failed to get prog fd on {}'.format(
+                        log_str))
+                    continue
+
+                # get new prog tag
+                info = struct_bpf_prog_info()
+                sz = ctypes.c_uint(ctypes.sizeof(info))
+                rc = libbpf.bpf_obj_get_info_by_fd(
+                    new_prog_fd, ctypes.byref(info), ctypes.byref(sz))
+                if rc == 0:
+                    new_prog_tag = bytes(info.tag).hex()
+
+                    logger.debug('new prog tag: {}'.format(new_prog_tag), extra={
+                        'iface': log_str})
+
+                    if current_prog_tag != new_prog_tag:
+                        self.bpf_fds[name] = new_prog_fd
+                        self.bpf_tags[name] = new_prog_tag
+
+                        if os.path.isfile(prog_pin_filename):
+                            os.unlink(prog_pin_filename)
+                        libbpf.bpf_program__pin(
+                            new_prog,
+                            os.fsencode(prog_pin_filename))
+
+                        maps_path = "{}/{}".format(maps_pin_dir, name)
+
+                        # unbind any orphan maps
+                        if os.path.isdir(maps_path):
+                            shutil.rmtree(maps_path)
+
+                        # create a new maps directory
+                        os.makedirs(maps_path, exist_ok=True)
+
+                        # pin  maps
+                        logger.debug('pin maps at: {}'.format(maps_path), extra={
+                            'iface': log_str})
+                        libbpf.bpf_object__pin_maps(
+                            new_obj,
+                            os.fsencode(maps_path))
+
+                        logger.log_change(log_str)
+                    else:
+                        logger.log_ok(log_str)
 
-                    maps_path = "{}/{}".format(maps_pin_dir, name)
+                    # update maps if appropriate
+                    if config.get('maps'):
+                        for map_name, map_entries in config['maps'].items():
+                            map_filename = "{}/{}/{}".format(maps_pin_dir, name, map_name)
+
+                            try:
+                                map_instance = BPF_Map(map_filename)
+                            except OSError as ex:
+                                logger.warning(
+                                    "opening bpf map {} failed: {}".format(map_name, ex))
+                                continue
 
-                    # unbind any orphan maps
-                    if os.path.isdir(maps_path):
-                        shutil.rmtree(maps_path)
-
-                    # create a new maps directory
-                    os.makedirs(maps_path, exist_ok=True)
-
-                    # pin  maps
-                    logger.debug('pin maps at: {}'.format(maps_path), extra={
-                        'iface': name})
-                    libbpf.bpf_object__pin_maps(
-                        new_obj,
-                        os.fsencode(maps_path))
-
-                    logger.info(
-                        'change',
-                        extra={'iface': name, 'style': IfStateLogging.STYLE_CHG})
+                            # TODO: support to manage map entries
                 else:
-                    logger.info(
-                        'ok',
-                        extra={'iface': name, 'style': IfStateLogging.STYLE_OK})
-
-                # update maps if appropriate
-                if config.get('maps'):
-                    for map_name, map_entries in config['maps'].items():
-                        map_filename = "{}/{}/{}".format(maps_pin_dir, name, map_name)
-
-                        try:
-                            map_instance = BPF_Map(map_filename)
-                        except OSError as ex:
-                            logger.warning(
-                                "opening bpf map {} failed: {}".format(map_name, ex))
-                            continue
-
-                        # TODO: support to manage map entries
-            else:
-                logger.warning(
-                    'BPF failed to get prog info on {}'.format(name))
+                    logger.warning(
+                        'BPF failed to get prog info on {}'.format(log_str))
+        finally:
+            if self.netns.netns is not None:
+                pyroute2.netns.popns()
 
     def get_bpf(self, name):
         return (self.bpf_fds.get(name, -1), self.bpf_tags.get(name))
```

### Comparing `ifstate-1.8.5/libifstate/bpf/ctypes.py` & `ifstate-1.9.0/libifstate/bpf/ctypes.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.5/libifstate/bpf/map.py` & `ifstate-1.9.0/libifstate/bpf/map.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.5/libifstate/brport/__init__.py` & `ifstate-1.9.0/libifstate/brport/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from libifstate.util import logger, ipr, IfStateLogging, filter_ifla_dump
+from libifstate.util import logger, IfStateLogging, filter_ifla_dump, LinkDependency
 from libifstate.exception import netlinkerror_classes
 
-
 class BRPort():
     ILFA_DEFAULTS = {
         "priority": 32,
         "guard": 0,
         "mode": 0,
         "fast_leave": 0,
         "protect": 0,
@@ -18,33 +17,35 @@
         "proxyarp_wifi": 0,
         "neigh_suppress": 0,
         "vlan_tunnel": 0,
         "backup_port": None,
         "isolated": 0,
     }
 
-    def __init__(self, iface, brport):
+    def __init__(self, netns, iface, brport):
+        self.netns = netns
         self.iface = iface
         self.brport = brport
 
     def depends(self):
         '''get link dependencies (i.e. backup port)'''
 
         backup_port = self.brport.get('backup_port')
 
         if backup_port:
-            return (backup_port,)
+            ns = self.settings.get("backup_port_netns", self.netns.netns)
+            return (LinkDependency(backup_port, ns),)
         else:
             return ()
 
     def has_changes(self, idx):
         logger.debug('checking brport', extra={'iface': self.iface})
 
         has_changes = False
-        brport_state = next(iter(ipr.brport('dump', index=idx)), None)
+        brport_state = next(iter(self.netns.ipr.brport('dump', index=idx)), None)
 
         # no a bridge port
         if brport_state is None:
             logger.debug('  not a bridge port', extra={'iface': self.iface})
             return True
 
         for setting in self.brport.keys():
@@ -55,35 +56,34 @@
             logger.debug('  %s: %s => %s', setting, current_value, self.brport[setting], extra={
                          'iface': self.iface})
             has_changes |= current_value != self.brport[setting]
 
         return has_changes
 
     def apply(self, do_apply, idx, excpts):
-        brport_state = ipr.brport('dump', index=idx)
+        brport_state = self.netns.ipr.brport('dump', index=idx)
         if brport_state == None:
             logger.warning('link is not a bridge port',
                            extra={'iface': self.iface})
             return
 
-        logger.info(
-            'change (brport)', extra={'iface': self.iface, 'style': IfStateLogging.STYLE_CHG})
+        logger.log_change('brport')
 
         logger.debug("bridge link set: {}".format(
             " ".join("{}={}".format(k, v) for k, v in self.brport.items())))
 
         if do_apply:
             try:
-                ipr.brport('set', index=idx, **(self.brport))
+                self.netns.ipr.brport('set', index=idx, **(self.brport))
             except Exception as err:
                 if not isinstance(err, netlinkerror_classes):
                     raise
                 excpts.add('brport', err, **(self.brport))
 
-    def show(showall, idx, config):
+    def show(ipr, showall, idx, config):
         brport_state = next(iter(ipr.brport('dump', index=idx)), None)
 
         if not brport_state:
             return
 
         proinfo = next(iter(brport_state.get_attrs('IFLA_PROTINFO')))
```

### Comparing `ifstate-1.8.5/libifstate/exception.py` & `ifstate-1.9.0/libifstate/exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,18 +66,17 @@
 class LinkTypeUnknown(Exception):
     pass
 
 
 class LinkDuplicate(Exception):
     pass
 
-
 class LinkCircularLinked(Exception):
-    pass
-
+    def exit_code(self):
+        return 5
 
 class LinkNoConfigFound(Exception):
     pass
 
 class ParserValidationError(Exception):
     def __init__(self, detail):
         self.detail = detail
```

### Comparing `ifstate-1.8.5/libifstate/link/base.py` & `ifstate-1.9.0/libifstate/link/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from libifstate.util import logger, ipr, IfStateLogging
+from libifstate.util import logger, IfStateLogging, LinkDependency
 from libifstate.exception import ExceptionCollector, LinkTypeUnknown, netlinkerror_classes
 from libifstate.brport import BRPort
 from libifstate.routing import RTLookups
 from abc import ABC, abstractmethod
 import os
 import subprocess
 import yaml
 import shutil
 import copy
+import pyroute2.netns
 
 ethtool_path = shutil.which("ethtool") or '/usr/sbin/ethtool'
 
-
 class Link(ABC):
     _nla_prefix = 'IFLA_'
     _classes = {}
     attr_value_maps = {
         # === bond ===
         'bond_mode': {
             0: 'balance-rr',
@@ -80,69 +80,112 @@
     attr_value_lookup = {
         'group': RTLookups.group,
     }
 
     def __new__(cls, *args, **kwargs):
         cname = cls.__name__
         if cname == Link.__name__:
-            cname = "{}Link".format(args[1]['kind'].lower().capitalize())
+            cname = "{}Link".format(args[3]['kind'].lower().capitalize())
 
         for c in Link.__subclasses__():
             if c.__name__ == cname:
                 return super().__new__(c)
 
         return super().__new__(GenericLink)
         #raise LinkTypeUnknown()
 
-    def __init__(self, name, link, ethtool, vrrp, brport):
+    def __init__(self, ifstate, netns, name, link, ethtool, vrrp, brport):
+        self.ifstate = ifstate
+        self.netns = netns
         self.cap_create = True
         self.cap_ethtool = False
         self.settings = {
             'ifname': name,
         }
         self.settings.update(link)
         self.ethtool = None
         self.vrrp = vrrp
         if brport:
-            self.brport = BRPort(name, brport)
+            self.brport = BRPort(netns, name, brport)
         else:
             self.brport = None
         self.attr_map = {
             'kind': ['IFLA_LINKINFO', 'IFLA_INFO_KIND'],
         }
         self.attr_idx = ['link', 'master', 'gre_link',
                          'ip6gre_link', 'vxlan_link', 'xfrm_link']
         self.idx = None
+        self.link_registry_search_args = []
+        self.link_ref = LinkDependency(name, self.netns.netns)
 
-        if 'address' in self.settings and self.settings['kind'] == 'physical':
-            self.settings['address'] = self.settings['address'].lower()
-            self.idx = next(iter(ipr.link_lookup(
-                address=self.settings['address'])), None)
-        if 'permaddr' in self.settings:
-            self.settings['permaddr'] = self.settings['permaddr'].lower()
-            self.idx = ipr.get_iface_by_permaddr(self.settings['permaddr'])
+        # prepare link registry search filters
         if 'businfo' in self.settings:
             self.settings['businfo'] = self.settings['businfo'].lower()
-            self.idx = ipr.get_iface_by_businfo(self.settings['businfo'])
+            self.link_registry_search_args.append({
+                'kind': self.settings['kind'],
+                'businfo': self.settings['businfo'],
+            })
+
+        if 'permaddr' in self.settings:
+            self.settings['permaddr'] = self.settings['permaddr'].lower()
+            self.link_registry_search_args.append({
+                'kind': self.settings['kind'],
+                'permaddr': self.settings['permaddr'],
+            })
+
+        if 'address' in self.settings and self.settings['kind'] == 'physical':
+            self.settings['address'] = self.settings['address'].lower()
+            self.link_registry_search_args.append({
+                'kind': self.settings['kind'],
+                'address': self.settings['address'],
+                'netns': netns.netns,
+            })
+
+        self.link_registry_search_args.append({
+            'kind': self.settings['kind'],
+            'ifname': name,
+            'netns': netns.netns,
+        })
+
+        if self.settings['kind'] == 'physical':
+            self.link_registry_search_args.append({
+                'kind': 'physical',
+                'ifname': name,
+                'orphan': True,
+            })
+
+        self.search_link_registry()
 
         for attr, mappings in self.attr_value_maps.items():
             if attr in self.settings and type(self.settings[attr]) != int:
                 self.settings[attr] = next((k for k, v in mappings.items(
                 ) if v == self.settings[attr]), self.settings[attr])
 
         for attr, lookup in self.attr_value_lookup.items():
             if attr in self.settings and type(self.settings[attr]) != int:
                 try:
                     self.settings[attr] = lookup.lookup_id(self.settings[attr])
                 except KeyError as err:
                     # mapping not available - catch exception and skip it
                     logger.warning('ignoring unknown group "%s"', self.settings[attr],
-                                   extra={'iface': self.settings['ifname']})
+                                   extra={'iface': self.settings['ifname'], 'netns': self.netns})
                     del(self.settings[attr])
 
+    def search_link_registry(self):
+        for args in self.link_registry_search_args:
+            item = self.ifstate.link_registry.get_link(**args)
+            if item is not None:
+                item.link = self
+                return item
+
+        logger.debug('no link found: %s', self.link_registry_search_args,
+                     extra={'iface': self.settings['ifname'], 'netns': self.netns})
+
+        return None
+
     def _drill_attr(self, data, keys):
         key = keys[0]
         d = data.get_attr(key)
 
         if d is not None:
             if len(keys) > 1:
                 return self._drill_attr(d, keys[1:])
@@ -177,26 +220,39 @@
                 ret = info.get_attr(nla)
                 if not ret is None:
                     return ret
 
         return None
 
     def get_ethtool_fn(self, setting):
-        return "/run/ifstate-ethtool:{}_{}.state".format(self.idx, setting)
+        try:
+            os.makedirs("/run/ifstate/ethtool", exist_ok=True)
+        except:
+            pass
+
+        # try to create a unique netns independent filename
+        name = ('bi', self.iface.get('businfo'))
+        if None in name:
+            name = ('pa', self.iface.get('permaddr'))
+        if None in name:
+            name = ('id', str(self.idx))
+        name = "__".join(name)
+
+        return "/run/ifstate/ethtool/{}__{}.state".format(name, setting)
 
     def get_ethtool_state(self, settings):
         ethtool = {}
 
         for setting in settings:
             ethtool[setting] = {}
             fn = self.get_ethtool_fn(setting)
 
             if not os.path.isfile(fn):
                 logger.debug('no prior ethtool %s state available', setting,
-                             extra={'iface': self.settings['ifname']})
+                             extra={'iface': self.settings['ifname'], 'netns': self.netns})
                 continue
 
             try:
                 with open(fn) as fh:
                     obj = yaml.load(fh, Loader=yaml.SafeLoader)
                     if type(obj) == dict:
                         ethtool[setting] = obj
@@ -218,16 +274,15 @@
 
         return [str(value)]
 
     def set_ethtool_state(self, ifname, settings, do_apply):
         if len(settings) == 0:
             return
 
-        logger.info(
-            'change (ethtool)', extra={'iface': self.settings['ifname'], 'style': IfStateLogging.STYLE_CHG})
+        logger.log_change('ethtool')
 
         if not do_apply:
             return
 
         for setting in settings:
             cmd = [ethtool_path]
             if setting in ['coalesce', 'features', 'pause', 'rxfh']:
@@ -236,24 +291,31 @@
                 cmd.append("--config-{}".format(setting))
             else:
                 cmd.append("--set-{}".format(setting))
             cmd.append(ifname)
             for option, value in self.ethtool[setting].items():
                 cmd.extend([option] + self.fmt_ethtool_opt(value))
             logger.debug("{}".format(" ".join(cmd)))
+
+            if self.netns.netns is not None:
+                pyroute2.netns.pushns(self.netns.netns)
             try:
-                res = subprocess.run(cmd)
-                if res.returncode != 0:
-                    logger.warning(
-                        '`{}` has failed'.format(" ".join(cmd[0:3])))
+                try:
+                    res = subprocess.run(cmd)
+                    if res.returncode != 0:
+                        logger.warning(
+                            '`{}` has failed'.format(" ".join(cmd[0:3])))
+                        return
+                except Exception as err:
+                    logger.warning('failed to run `{}`: {}'.format(
+                        " ".join(cmd[0:3]), err.args[1]))
                     return
-            except Exception as err:
-                logger.warning('failed to run `{}`: {}'.format(
-                    " ".join(cmd[0:3]), err.args[1]))
-                return
+            finally:
+                if self.netns.netns is not None:
+                    pyroute2.netns.popns()
 
             fn = self.get_ethtool_fn(setting)
             try:
                 with open(fn, 'w') as fh:
                     yaml.dump(self.ethtool[setting], fh)
             except Exception as err:
                 logger.warning('failed write `{}`: {}'.format(fn, err.args[1]))
@@ -270,37 +332,78 @@
     def apply(self, do_apply, sysctl):
         excpts = ExceptionCollector(self.settings['ifname'])
         osettings = copy.deepcopy(self.settings)
 
         # lookup for attributes requiring a interface index
         for attr in self.attr_idx:
             if attr in self.settings:
-                self.settings[attr] = next(iter(ipr.link_lookup(
-                    ifname=self.settings[attr])), self.settings[attr])
+                netns_attr = "{}_netns".format(attr)
+                netnsid_attr = "{}_netnsid".format(attr)
+                if netns_attr in self.settings:
+                    # ToDo: throw exception for unknown netns
+                    (peer_ipr, peer_nsid) = self.netns.get_netnsid(self.settings[netns_attr])
+                    self.settings[netnsid_attr] = peer_nsid
+                    idx = next(iter(peer_ipr.link_lookup(
+                        ifname=self.settings[attr])), None)
+
+                    del(self.settings[netns_attr])
+                else:
+                    idx = next(iter(self.netns.ipr.link_lookup(
+                        ifname=self.settings[attr])), None)
+
+                if idx is not None:
+                    self.settings[attr] = idx
+                else:
+                    logger.warning('could not find %s "%s"', attr,
+                        self.settings[attr],
+                        extra={
+                            'iface': self.settings['ifname'],
+                            'netns': self.netns})
+                    self.settings['state'] = 'down'
+                    if netnsid_attr in self.settings:
+                        del(self.settings[netnsid_attr])
+                    del(self.settings[attr])
 
-        if self.idx is None:
-            self.idx = next(iter(ipr.link_lookup(
-                ifname=self.settings['ifname'])), None)
+        # get interface from registry
+        item = self.search_link_registry()
+
+        # move interface into netns if required
+        if item is not None and item.netns.netns != self.netns.netns:
+            logger.log_change('netns')
+
+            if do_apply:
+                try:
+                    # move link into target netns
+                    item.update_netns(self.netns)
+                except Exception as err:
+                    if not isinstance(err, netlinkerror_classes):
+                        raise
+                    item.netns.ipr.link('set', index=item.attributes['index'], state='down')
+                    excpts.add('set', err, netns=self.netns.netns)
+                    return excpts
+
+        if item is not None:
+            self.idx = item.attributes['index']
 
         if self.idx is not None:
-            self.iface = next(iter(ipr.get_links(self.idx)), None)
-            permaddr = ipr.get_permaddr(self.iface.get_attr('IFLA_IFNAME'))
+            self.iface = next(iter(item.netns.ipr.get_links(self.idx)), None)
+            permaddr = item.netns.ipr.get_permaddr(self.iface.get_attr('IFLA_IFNAME'))
             if not permaddr is None:
                 self.iface['permaddr'] = permaddr
-            businfo = ipr.get_businfo(self.iface.get_attr('IFLA_IFNAME'))
+            businfo = item.netns.ipr.get_businfo(self.iface.get_attr('IFLA_IFNAME'))
             if not businfo is None:
                 self.iface['businfo'] = businfo
 
             # check for ifname collisions
-            idx = next(iter(ipr.link_lookup(
+            idx = next(iter(self.netns.ipr.link_lookup(
                 ifname=self.settings['ifname'])), None)
             if idx is not None and idx != self.idx and do_apply:
                 try:
-                    ipr.link('set', index=idx, state='down')
-                    ipr.link('set', index=idx, ifname='{}!'.format(
+                    self.netns.ipr.link('set', index=idx, state='down')
+                    self.netns.ipr.link('set', index=idx, ifname='{}!'.format(
                         self.settings['ifname']))
                 except Exception as err:
                     if not isinstance(err, netlinkerror_classes):
                         raise
                     excpts.add('set', err, state='down', ifname='{}!')
 
             if self.cap_create and self.get_if_attr('kind') != self.settings['kind']:
@@ -314,45 +417,44 @@
         else:
             self.create(do_apply, sysctl, excpts)
 
         self.settings = osettings
         return excpts
 
     def create(self, do_apply, sysctl, excpts, oper="add"):
-        logger.info(
-            oper, extra={'iface': self.settings['ifname'], 'style': IfStateLogging.STYLE_CHG})
+        logger.log_add('link')
 
         logger.debug("ip link add: {}".format(
             " ".join("{}={}".format(k, v) for k, v in self.settings.items())))
         if do_apply:
             try:
                 # set state later
                 state = self.settings.pop('state', None)
 
                 # prevent altname conflict
                 self.prevent_altname_conflict()
 
                 # add link
-                ipr.link('add', **(self.settings))
-                self.idx = next(iter(ipr.link_lookup(
+                self.netns.ipr.link('add', **(self.settings))
+                self.idx = next(iter(self.netns.ipr.link_lookup(
                     ifname=self.settings['ifname'])), None)
 
                 if self.idx is not None:
                     # set sysctl settings if required
                     sysctl.apply(self.settings['ifname'], do_apply)
 
                     # set brport settings if required
                     if self.brport:
                         if self.brport.has_changes(self.idx):
                             self.brport.apply(do_apply, self.idx, excpts)
 
                     # set state if required
                     if state is not None and not excpts.has_op('brport'):
                         try:
-                            ipr.link('set', index=self.idx, state=state)
+                            self.netns.ipr.link('set', index=self.idx, state=state)
                         except Exception as err:
                             if not isinstance(err, netlinkerror_classes):
                                 raise
                             excpts.add('set', err, state=state)
             except Exception as err:
                 if not isinstance(err, netlinkerror_classes):
                     raise
@@ -361,34 +463,34 @@
         if not self.ethtool is None:
             logger.debug("ethtool: {}".format(self.ethtool))
             self.set_ethtool_state(
                 self.settings['ifname'], self.ethtool.keys(), do_apply)
 
     def recreate(self, do_apply, sysctl, excpts):
         logger.debug('has wrong link kind %s, removing', self.settings['kind'], extra={
-                     'iface': self.settings['ifname']})
+                     'iface': self.settings['ifname'], 'netns': self.netns})
         if do_apply:
             try:
-                ipr.link('del', index=self.idx)
+                self.netns.ipr.link('del', index=self.idx)
             except Exception as err:
                 if not isinstance(err, netlinkerror_classes):
                     raise
                 excpts.add('del', err)
         self.idx = None
         self.create(do_apply, sysctl, excpts, "replace")
 
     def update(self, do_apply, sysctl, excpts):
-        logger.debug('checking link', extra={'iface': self.settings['ifname']})
+        logger.debug('checking link', extra={'iface': self.settings['ifname'], 'netns': self.netns})
 
         old_state = self.iface['state']
         has_link_changes = False
         has_state_changes = False
         for setting in self.settings.keys():
             logger.debug('  %s: %s => %s', setting, self.get_if_attr(
-                setting), self.settings[setting], extra={'iface': self.settings['ifname']})
+                setting), self.settings[setting], extra={'iface': self.settings['ifname'], 'netns': self.netns})
             if setting == "state":
                 has_state_changes = self.get_if_attr(
                     setting) != self.settings[setting]
             else:
                 if setting != 'kind' or self.cap_create:
                     has_link_changes |= self.get_if_attr(
                         setting) != self.settings[setting]
@@ -413,21 +515,21 @@
 
         has_brport_changes = False
         if self.brport:
             has_brport_changes = self.brport.has_changes(self.idx)
 
         if has_link_changes:
             logger.debug('needs to be configured', extra={
-                         'iface': self.settings['ifname']})
+                         'iface': self.settings['ifname'], 'netns': self.netns})
             if old_state != 'down':
                 logger.debug('shutting down', extra={
-                             'iface': self.settings['ifname']})
+                             'iface': self.settings['ifname'], 'netns': self.netns})
                 if do_apply:
                     try:
-                        ipr.link('set', index=self.idx, state='down')
+                        self.netns.ipr.link('set', index=self.idx, state='down')
                     except Exception as err:
                         if not isinstance(err, netlinkerror_classes):
                             raise
                         excpts.add('set', err, state='down')
 
                 if not 'state' in self.settings:
                     self.settings['state'] = 'up'
@@ -438,61 +540,59 @@
 
             self.set_ethtool_state(self.get_if_attr(
                 'ifname'), has_ethtool_changes, do_apply)
 
             has_ifname_change = self.get_if_attr(
                 'ifname') != self.settings['ifname']
             if has_ifname_change:
-                logger.info('change (was {})'.format(self.get_if_attr('ifname')), extra={
-                            'iface': self.settings['ifname'], 'style': IfStateLogging.STYLE_CHG})
-            else:
-                logger.info('change', extra={
-                            'iface': self.settings['ifname'], 'style': IfStateLogging.STYLE_CHG})
+                logger.log_change('ifname')
+            logger.log_change('link')
 
             logger.debug("ip link set: {}".format(
                 " ".join("{}={}".format(k, v) for k, v in self.settings.items())))
             if do_apply:
                 # temp. remove special settings
-                state = self.settings.pop('state', None)
-                peer = self.settings.pop('peer', None)
+                skipped_settings = {}
+                for setting in ['state', 'peer', 'kind', 'businfo', 'permaddr']:
+                    if setting in self.settings:
+                        skipped_settings[setting] = self.settings.pop(setting)
 
                 if has_ifname_change:
                     self.prevent_altname_conflict()
 
                 try:
-                    ipr.link('set', index=self.idx, **(self.settings))
+                    self.netns.ipr.link('set', index=self.idx, **(self.settings))
+                    self.iface = next(iter(self.netns.ipr.get_links(self.idx)), None)
 
                     for setting in self.settings.keys():
-                        if self.get_if_attr(setting) != self.settings[setting]:
-                            if self.cap_create:
-                                logger.debug('  %s: setting could not be changed', setting, extra={'iface': self.settings['ifname']})
-                                excpts.add('set', Exception('ip link set'), **{setting: self.settings[setting]})
-                            else:
-                                logger.warning('%s setting could not be changed', setting,
-                                               extra={'iface': self.settings['ifname']})
+                        if not setting.endswith('_netns') or not setting[:-6] in self.attr_idx:
+                            if self.get_if_attr(setting) != self.settings[setting]:
+                                if self.cap_create:
+                                    logger.debug('  %s: setting could not be changed', setting, extra={'iface': self.settings['ifname']})
+                                    excpts.add('set', Exception('ip link set'), **{setting: self.settings[setting]})
+                                else:
+                                    logger.warning('%s setting could not be changed', setting,
+                                                   extra={'iface': self.settings['ifname']})
                 except Exception as err:
                     if not isinstance(err, netlinkerror_classes):
                         raise
                     excpts.add('set', err, **(self.settings))
 
                 # restore settings
-                if state is not None:
-                    self.settings['state'] = state
-                if peer is not None:
-                    self.settings['peer'] = peer
+                for setting, value in skipped_settings.items():
+                    self.settings[setting] = value
 
                 try:
-                    if not state is None:
+                    if 'state' in self.settings:
                         # restore state setting for recreate
-                        self.settings['state'] = state
-                        ipr.link('set', index=self.idx, state=state)
+                        self.netns.ipr.link('set', index=self.idx, state=self.settings['state'])
                 except Exception as err:
                     if not isinstance(err, netlinkerror_classes):
                         raise
-                    excpts.add('set', err, state=state)
+                    excpts.add('set', err, state=self.settings['state'])
 
             if has_brport_changes:
                 self.brport.apply(do_apply, self.idx, excpts)
         else:
             # set sysctl settings
             sysctl.apply(self.get_if_attr(
                 'ifname'), do_apply)
@@ -502,47 +602,46 @@
 
             if has_brport_changes:
                 if old_state:
                     logger.debug('shutting down', extra={
                                  'iface': self.settings['ifname']})
                     if do_apply:
                         try:
-                            ipr.link('set', index=self.idx, state='down')
+                            self.netns.ipr.link('set', index=self.idx, state='down')
                         except Exception as err:
                             if not isinstance(err, netlinkerror_classes):
                                 raise
                             excpts.add('set', err, state='down')
                     if not 'state' in self.settings:
                         self.settings['state'] = 'up'
 
                     has_state_changes = self.settings['state'] == 'up'
 
                 self.brport.apply(do_apply, self.idx, excpts)
 
             if has_state_changes:
                 if do_apply:
                     try:
-                        ipr.link('set', index=self.idx,
+                        self.netns.ipr.link('set', index=self.idx,
                                  state=self.settings["state"])
                     except Exception as err:
                         if not isinstance(err, netlinkerror_classes):
                             raise
-                        excpts.add('set', err, state=state)
-                logger.info('change', extra={
-                            'iface': self.settings['ifname'], 'style': IfStateLogging.STYLE_CHG})
-
+                        excpts.add('set', err, state=self.settings['state'])
+                logger.log_change('link')
             else:
-                logger.info(
-                    'ok', extra={'iface': self.settings['ifname'], 'style': IfStateLogging.STYLE_OK})
+                logger.log_ok('link')
 
     def depends(self):
         deps = []
+
         for attr in self.attr_idx:
             if attr in self.settings:
-                deps.append(self.settings[attr])
+                ns = self.settings.get("{}_netns".format(attr), self.netns.netns)
+                deps.append(LinkDependency(self.settings[attr], ns))
 
         if self.brport:
             deps.extend(self.brport.depends())
 
         return deps
 
     def prevent_altname_conflict(self):
@@ -550,33 +649,33 @@
         When renaming interfaces a interface name conflict could
         happen on the IFLA_ALT_IFNAME property (Linux 5.5+). Remove
         the altname from the other interface in such case, it may be
         the same interface if it is renamed to one of it's altnames.
         '''
 
         logger.debug('checking altname conflict', extra={
-                     'iface': self.settings['ifname']})
+                     'iface': self.settings['ifname'], 'netns': self.netns})
 
         # get link candidate having the ifname as altname
         try:
             link = next(
-                iter(ipr.link('get', altname=self.settings['ifname'])), None)
+                iter(self.netns.ipr.link('get', altname=self.settings['ifname'])), None)
         except Exception as err:
             if not isinstance(err, netlinkerror_classes):
                 raise
             return
 
         # pyroute2 may return the interface having ifname rather than
         # altname set - only remove altname if it is set
         properties = link.get_attr('IFLA_PROP_LIST')
         if properties is not None and self.settings['ifname'] in properties.get_attrs('IFLA_ALT_IFNAME'):
             logger.debug('  found: %s (%d)', link.get_attr(
-                'IFLA_IFNAME'), link['index'], extra={'iface': self.settings['ifname']})
+                'IFLA_IFNAME'), link['index'], extra={'iface': self.settings['ifname'], 'netns': self.netns})
             try:
-                ipr.link('property_del',
+                self.netns.ipr.link('property_del',
                          index=link['index'], altname=self.settings['ifname'])
             except Exception as err:
                 if not isinstance(err, netlinkerror_classes):
                     raise
 
     @classmethod
     def name2nla(self, name):
@@ -590,9 +689,9 @@
         name = name.upper()
         if name.find(self._nla_prefix) == -1:
             name = "%s%s" % (self._nla_prefix, name)
         return name
 
 
 class GenericLink(Link):
-    def __init__(self, name, link, ethtool, vrrp, brport):
-        super().__init__(name, link, ethtool, vrrp, brport)
+    def __init__(self, ifstate, netns, name, link, ethtool, vrrp, brport):
+        super().__init__(ifstate, netns, name, link, ethtool, vrrp, brport)
```

### Comparing `ifstate-1.8.5/libifstate/link/physical.py` & `ifstate-1.9.0/libifstate/link/physical.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from libifstate.util import logger
 from libifstate.link.base import Link
 from libifstate.exception import LinkCannotAdd
 
 class PhysicalLink(Link):
-    def __init__(self, name, link, ethtool, vrrp, brport):
-        super().__init__(name, link, ethtool, vrrp, brport)
+    def __init__(self, ifstate, netns, name, link, ethtool, vrrp, brport):
+        super().__init__(ifstate, netns, name, link, ethtool, vrrp, brport)
         self.cap_create = False
         self.cap_ethtool = True
         self.ethtool = ethtool
  
     def create(self, do_apply, sysctl, excpts, oper="add"):
         logger.warning('Unable to create missing physical link: {}'.format(self.settings.get('ifname')))
```

### Comparing `ifstate-1.8.5/libifstate/link/tun.py` & `ifstate-1.9.0/libifstate/link/tun.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from libifstate.link.base import Link
 from libifstate.exception import LinkCannotAdd
 
 from pwd import getpwnam
 from grp import getgrnam
 
 class TunLink(Link):
-    def __init__(self, name, link, ethtool, vrrp, brport):
+    def __init__(self, ifstate, netns, name, link, ethtool, vrrp, brport):
         if 'tun_owner' in link and isinstance(link['tun_owner'], str):
             link['tun_owner'] = getpwnam(link['tun_owner'])[2]
 
         if 'tun_group' in link and isinstance(link['tun_group'], str):
             link['tun_group'] = getgrnam(link['tun_group'])[2]
 
-        super().__init__(name, link, ethtool, vrrp, brport)
+        super().__init__(ifstate, netns, name, link, ethtool, vrrp, brport)
         self.cap_create = bool(link.get('tun_persist'))
  
     def create(self, do_apply, sysctl, excpts, oper="add"):
         if not self.cap_create:
             logger.warning('Unable to create missing non-persistent tuntap link: {}'.format(self.settings.get('ifname')))
         else:
             super().create(do_apply, sysctl, excpts, oper)
```

### Comparing `ifstate-1.8.5/libifstate/link/veth.py` & `ifstate-1.9.0/libifstate/link/veth.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from libifstate.util import logger, ipr
+from libifstate.util import logger
 from libifstate.link.base import Link
 from libifstate.exception import LinkCannotAdd
 
 class VethLink(Link):
-    def __init__(self, name, link, ethtool, vrrp, brport):
-        super().__init__(name, link, ethtool, vrrp, brport)
+    def __init__(self, ifstate, netns, name, link, ethtool, vrrp, brport):
+        super().__init__(ifstate, netns, name, link, ethtool, vrrp, brport)
 
     # quirk to handle peer attribute
     def get_if_attr(self, key):
         if key != "peer":
             return super().get_if_attr(key)
 
         peer = super().get_if_attr("link")
 
         if peer is None:
             return None
 
-        lnk = next(iter(ipr.get_links(peer)), None)
+        lnk = next(iter(self.netns.ipr.get_links(peer)), None)
         return lnk.get_attr("IFLA_IFNAME")
```

### Comparing `ifstate-1.8.5/libifstate/log.py` & `ifstate-1.9.0/libifstate/log.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,37 @@
 from logging.handlers import QueueHandler, QueueListener
 import os
 import queue
 import sys
 
 logger = logging.getLogger('ifstate')
 logger.propagate = False
+logger.log_add = lambda option, oper='add': logger.info(oper, extra={'option': option, 'style': IfStateLogging.STYLE_CHG})
+logger.log_change = lambda option, oper='change': logger.info(oper, extra={'option': option, 'style': IfStateLogging.STYLE_CHG})
+logger.log_ok = lambda option, oper='ok': logger.info(oper, extra={'option': option, 'style': IfStateLogging.STYLE_OK})
+logger.log_del = lambda option, oper='del': logger.info(oper, extra={'option': option, 'style': IfStateLogging.STYLE_DEL})
 
 formatter = logging.Formatter('%(bol)s%(prefix)s%(style)s%(message)s%(eol)s')
 
 class IfStateLogFilter(logging.Filter):
     def __init__(self, is_terminal):
         super().__init__()
         self.is_terminal = is_terminal
 
     def filter(self, record):
         record.levelshort = record.levelname[:1]
 
         if hasattr(record, 'iface'):
-            record.prefix = " {:15} ".format(record.iface)
+            record.prefix = " {:35} ".format(record.iface)
         else:
             record.prefix = ''
 
+        if hasattr(record, 'option'):
+            record.prefix = "   {:33} ".format(record.option)
+
         if self.is_terminal and record.levelno >= logging.WARNING:
             if record.levelno >= logging.ERROR:
                 record.bol = IfStateLogging.ANSI_RED
             else:
                 record.bol = IfStateLogging.ANSI_MAGENTA
             record.eol = IfStateLogging.ANSI_RESET
         else:
```

### Comparing `ifstate-1.8.5/libifstate/neighbour/__init__.py` & `ifstate-1.9.0/libifstate/neighbour/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,68 +1,66 @@
-from libifstate.util import logger, ipr, IfStateLogging
+from libifstate.util import logger, IfStateLogging
 from libifstate.exception import netlinkerror_classes
 from ipaddress import ip_address
 
 
 class Neighbours():
-    def __init__(self, iface, neighbours):
+    def __init__(self, netns, iface, neighbours):
+        self.netns = netns
         self.iface = iface
         self.neighbours = {}
         for neigh in neighbours:
             self.neighbours[ip_address(neigh['dst'])] = neigh.get('lladdr')
 
     def apply(self, do_apply):
         logger.debug('getting neighbours', extra={'iface': self.iface})
 
         # get ifindex
-        idx = next(iter(ipr.link_lookup(ifname=self.iface)), None)
+        idx = next(iter(self.netns.ipr.link_lookup(ifname=self.iface)), None)
 
         if idx == None:
             logger.warning('link missing', extra={'iface': self.iface})
             return
 
         # get neighbour entries (only NUD_PERMANENT)
         ipr_neigh = {}
         neigh_add = {}
-        for neigh in ipr.get_neighbours(ifindex=idx, state=128):
+        for neigh in self.netns.ipr.get_neighbours(ifindex=idx, state=128):
             ip = ip_address(neigh.get_attr('NDA_DST'))
             ipr_neigh[ip] = neigh.get_attr('NDA_LLADDR')
 
         for ip, lladdr in self.neighbours.items():
             if ip in ipr_neigh and lladdr == ipr_neigh[ip]:
-                logger.info(' %s', ip, extra={
-                            'iface': self.iface, 'style': IfStateLogging.STYLE_OK})
+                logger.log_ok('neighbours', '= {}'.format(ip))
                 del ipr_neigh[ip]
             else:
                 neigh_add[ip] = lladdr
 
         for ip, lladdr in ipr_neigh.items():
-            logger.info(
-                '-%s', str(ip), extra={'iface': self.iface, 'style': IfStateLogging.STYLE_DEL})
+            logger.log_del('neighbours', '- {}'.format(str(ip)))
             try:
                 if do_apply:
-                    ipr.neigh("del", ifindex=idx, dst=str(
+                    self.netns.ipr.neigh("del", ifindex=idx, dst=str(
                         ip))
             except Exception as err:
                 if not isinstance(err, netlinkerror_classes):
                     raise
                 logger.warning('removing neighbour {} failed: {}'.format(
                     str(ip), err.args[1]))
 
         for ip, lladdr in neigh_add.items():
-            logger.info('+%s', str(ip),
-                        extra={'iface': self.iface, 'style': IfStateLogging.STYLE_CHG})
+            logger.log_add('neighbours', '+ {}'.format(str(ip)))
             if do_apply:
                 try:
                     opts = {
                         'ifindex': idx,
                         'dst': str(ip),
                         'lladdr': lladdr,
                         'state': 128
                     }
 
-                    ipr.neigh('replace', **opts)
+                    self.netns.ipr.neigh('replace', **opts)
                 except Exception as err:
                     if not isinstance(err, netlinkerror_classes):
                         raise
                     logger.warning('adding neighbour {} failed: {}'.format(
                         str(ip), err.args[1]))
```

### Comparing `ifstate-1.8.5/libifstate/parser/base.py` & `ifstate-1.9.0/libifstate/parser/base.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.5/libifstate/parser/yaml.py` & `ifstate-1.9.0/libifstate/parser/yaml.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.5/libifstate/routing/__init__.py` & `ifstate-1.9.0/libifstate/routing/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from libifstate.util import logger, ipr, IfStateLogging
+from libifstate.util import logger, IfStateLogging
 from libifstate.exception import RouteDupblicate, netlinkerror_classes
 from ipaddress import ip_address, ip_network, IPv6Network
 from pyroute2.netlink.rtnl.fibmsg import FR_ACT_VALUES
 from pyroute2.netlink.rtnl import rt_type
 import collections.abc
 from glob import glob
 import os
@@ -85,15 +85,16 @@
     'scope': 0,
     'proto': 3,
     'realm': 0,
     'tos': 0,
 }
 
 class Tables(collections.abc.Mapping):
-    def __init__(self):
+    def __init__(self, netns):
+        self.netns = netns
         self.tables = {
             254: [],
         }
 
     def __getitem__(self, key):
         if not key in self.tables:
             raise KeyError()
@@ -116,15 +117,15 @@
         for key, lookup in RT_LOOKUPS_DICT.items():
             try:
                 rt[key] = route.get(key, RT_LOOKUPS_DEFAULTS[key])
                 rt[key] = lookup.lookup_id(rt[key])
             except KeyError as err:
                 # mapping not available - catch exception and skip it
                 logger.warning('ignoring unknown %s "%s"', key, rt[key],
-                               extra={'iface': rt['dst']})
+                               extra={'iface': rt['dst'], 'netns': self.netns})
                 rt[key] = RT_LOOKUPS_DEFAULTS[key]
 
         if type(rt['type']) == str:
             rt['type'] = rt_type[rt['type']]
 
         if 'dev' in route:
             rt['oif'] = route['dev']
@@ -144,15 +145,15 @@
 
         if not rt['table'] in self.tables:
             self.tables[rt['table']] = []
         self.tables[rt['table']].append(rt)
 
     def show_routes(self, ignores):
         routes = []
-        for route in ipr.get_routes(family=AF_INET) + ipr.get_routes(family=AF_INET6):
+        for route in self.netns.ipr.get_routes(family=AF_INET) + self.netns.ipr.get_routes(family=AF_INET6):
             # skip routes from local table
             table = route.get_attr('RTA_TABLE')
             if table == 255:
                 continue
 
             # skip ignored routes
             ignore = False
@@ -176,15 +177,15 @@
             }
 
             if table != 254:
                 rt['table'] = RTLookups.tables.lookup_str(table),
 
             dev = route.get_attr('RTA_OIF')
             if dev:
-                link = next(iter(ipr.get_links(dev)), None)
+                link = next(iter(self.netns.ipr.get_links(dev)), None)
                 if link:
                     rt['dev'] = link.get_attr('IFLA_IFNAME', dev)
                 else:
                     rt['dev'] = dev
 
             via = route.get_attr('RTA_GATEWAY')
             if via:
@@ -217,15 +218,15 @@
 
             routes.append(rt)
 
         return routes
 
     def kernel_routes(self, table):
         routes = []
-        for route in ipr.get_routes(table=table, family=AF_INET) + ipr.get_routes(table=table, family=AF_INET6):
+        for route in self.netns.ipr.get_routes(table=table, family=AF_INET) + self.netns.ipr.get_routes(table=table, family=AF_INET6):
             # ignore RTM_F_CLONED routes
             if route['flags'] & 512:
                 continue
 
             if route['dst_len'] > 0:
                 dst = ip_network(
                     '{}/{}'.format(route.get_attr('RTA_DST'), route['dst_len'])).with_prefixlen
@@ -267,49 +268,47 @@
                 rt['priority'] = priority
 
             routes.append(rt)
         return routes
 
     def apply(self, ignores, do_apply):
         for table, croutes in self.tables.items():
-            pfx = RTLookups.tables.lookup_str(table)
-            logger.info('\nconfiguring routing table {}...'.format(pfx))
+            log_str = RTLookups.tables.lookup_str(table)
+            if self.netns.netns != None:
+                log_str += "[netns={}]".format(self.netns.netns)
 
             kroutes = self.kernel_routes(table)
 
             for route in croutes:
                 if 'oif' in route and type(route['oif']) == str:
                     route['oif'] = next(
-                        iter(ipr.link_lookup(ifname=route['oif'])), None)
+                        iter(self.netns.ipr.link_lookup(ifname=route['oif'])), None)
                 found = False
                 identical = False
                 for i, kroute in enumerate(kroutes):
                     if route_matches(route, kroute):
                         del kroutes[i]
                         found = True
                         if route_matches(route, kroute, route.keys(), indent=route['dst']):
                             identical = True
                             break
 
                 if identical:
-                    logger.info(
-                        'ok', extra={'iface': route['dst'], 'style': IfStateLogging.STYLE_OK})
+                    logger.log_ok(log_str, "= {}".format(route['dst']))
                 else:
                     if found:
-                        logger.info('change', extra={
-                                    'iface': route['dst'], 'style': IfStateLogging.STYLE_CHG})
+                        logger.log_change(log_str, "~ {}".format(route['dst']))
                     else:
-                        logger.info(
-                            'add', extra={'iface': route['dst'], 'style': IfStateLogging.STYLE_CHG})
+                        logger.log_add(log_str, "+ {}".format(route['dst']))
 
                     logger.debug("ip route replace: {}".format(
                         " ".join("{}={}".format(k, v) for k, v in route.items())))
                     try:
                         if do_apply:
-                            ipr.route('replace', **route)
+                            self.netns.ipr.route('replace', **route)
                     except Exception as err:
                         if not isinstance(err, netlinkerror_classes):
                             raise
                         logger.warning('route setup {} failed: {}'.format(
                             route['dst'], err.args[1]))
 
             for route in kroutes:
@@ -317,28 +316,28 @@
                 for iroute in ignores:
                     if route_matches(route, iroute, iroute.keys()):
                         ignore = True
                         break
                 if ignore:
                     continue
 
-                logger.info(
-                    'del', extra={'iface': route['dst'], 'style': IfStateLogging.STYLE_DEL})
+                logger.log_del(log_str, "- {}".format(route['dst']))
                 try:
                     if do_apply:
-                        ipr.route('del', **route)
+                        self.netns.ipr.route('del', **route)
                 except Exception as err:
                     if not isinstance(err, netlinkerror_classes):
                         raise
                     logger.warning('removing route {} failed: {}'.format(
                         route['dst'], err.args[1]))
 
 
 class Rules():
-    def __init__(self):
+    def __init__(self, netns):
+        self.netns = netns
         self.rules = []
 
     def add(self, rule):
         ru = {
             'table': RTLookups.tables.lookup_id(rule.get('table', 254)),
             'protocol': RTLookups.protos.lookup_id(rule.get('proto', 0)),
             'tos': rule.get('tos', 0),
@@ -382,15 +381,15 @@
         if 'priority' in rule:
             ru['priority'] = rule['priority']
 
         self.rules.append(ru)
 
     def kernel_rules(self):
         rules = []
-        for rule in ipr.get_rules(family=AF_INET) + ipr.get_rules(family=AF_INET6):
+        for rule in self.netns.ipr.get_rules(family=AF_INET) + self.netns.ipr.get_rules(family=AF_INET6):
             ru = {
                 'action': FR_ACT_VALUES.get(rule['action']),
                 'table': rule.get_attr('FRA_TABLE'),
                 'protocol': rule.get_attr('FRA_PROTOCOL'),
                 'priority': rule.get_attr('FRA_PRIORITY', 0),
                 'family': rule['family'],
                 'tos': rule['tos'],
@@ -452,36 +451,37 @@
                     del rule[key]
 
             rules.append(rule)
 
         return rules
 
     def apply(self, ignores, do_apply):
-        logger.info('\nconfiguring routing rules...')
         krules = self.kernel_rules()
         for rule in self.rules:
+            log_str = '#{}'.format(rule['priority'])
+            if self.netns.netns != None:
+                log_str += "[netns={}]".format(self.netns.netns)
+
             found = False
             for i, krule in enumerate(krules):
                 if rule_matches(rule, krule, rule.keys()):
                     del krules[i]
                     found = True
                     break
 
             if found:
-                logger.info(
-                    'ok', extra={'iface': '#{}'.format(rule['priority']), 'style': IfStateLogging.STYLE_OK})
+                logger.log_ok(log_str)
             else:
-                logger.info(
-                    'add', extra={'iface': '#{}'.format(rule['priority']), 'style': IfStateLogging.STYLE_CHG})
+                logger.log_add(log_str)
 
                 logger.debug("ip rule add: {}".format(
                     " ".join("{}={}".format(k, v) for k, v in rule.items())))
                 try:
                     if do_apply:
-                        ipr.rule('add', **rule)
+                        self.netns.ipr.rule('add', **rule)
                 except Exception as err:
                     if not isinstance(err, netlinkerror_classes):
                         raise
                     logger.warning('rule setup failed: {}'.format(err.args[1]))
 
         for rule in krules:
             ignore = False
@@ -491,16 +491,15 @@
                     del irule['proto']
                 if rule_matches(rule, irule, irule.keys()):
                     ignore = True
                     break
             if ignore:
                 continue
 
-            logger.info(
-                'del', extra={'iface': '#{}'.format(rule['priority']), 'style': IfStateLogging.STYLE_DEL})
+            logger.log_del(log_str)
             try:
                 if do_apply:
-                    ipr.rule('del', **rule)
+                    self.netns.ipr.rule('del', **rule)
             except Exception as err:
                 if not isinstance(err, netlinkerror_classes):
                     raise
                 logger.warning('removing rule failed: {}'.format(err.args[1]))
```

### Comparing `ifstate-1.8.5/libifstate/sysctl/__init__.py` & `ifstate-1.9.0/libifstate/sysctl/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 from libifstate.util import logger, IfStateLogging
+import pyroute2.netns
 
 import os
 
 
 class Sysctl():
-    def __init__(self):
+    def __init__(self, netns):
         self.sysctls = {}
+        self.netns = netns
 
     def add(self, iface, sysctl):
         self.sysctls[iface] = sysctl
 
     def set_sysctl(self, iface_current, iface_config, family, key, val, do_apply):
-        fn = '/proc/sys/net/{}/conf/{}/{}'.format(family, iface_current, key)
+        if self.netns.netns is not None:
+            pyroute2.netns.pushns(self.netns.netns)
+
+        log_str = "{}/{}".format(family, key)
+        if self.netns.netns is not None:
+            log_str += "[netns={}]".format(self.netns.netns)
+
         try:
-            with open(fn) as fh:
-                current = fh.readline().rstrip()
-        except OSError as err:
-            logger.warning('reading sysctl {}/{} failed: {}'.format(
-                family, key, err.args[1]))
-            return
-        if current == str(val):
-            logger.debug('  %s/%s: %s == %s', family, key, current, val, extra={'iface': iface_config})
-            return False
-        else:
-            logger.debug('  %s/%s: %s => %s', family, key, current, val, extra={'iface': iface_config})
-            if do_apply:
-                try:
-                    with open(fn, 'w') as fh:
-                        fh.writelines([str(val)])
-                except OSError as err:
-                    logger.warning('updating sysctl {}/{} failed: {}'.format(
-                        family, key, err.args[1]))
-            return True
+            fn = '/proc/sys/net/{}/conf/{}/{}'.format(family, iface_current, key)
+            try:
+                with open(fn) as fh:
+                    current = fh.readline().rstrip()
+            except OSError as err:
+                logger.warning('reading sysctl {}/{} failed: {}'.format(
+                    family, key, err.args[1]))
+                return
+            if current == str(val):
+                logger.debug('  %s/%s: %s == %s', family, key, current, val, extra={'iface': iface_config, 'netns': self.netns})
+                logger.log_ok(log_str)
+                return False
+            else:
+                logger.debug('  %s/%s: %s => %s', family, key, current, val, extra={'iface': iface_config, 'netns': self.netns})
+                if do_apply:
+                    try:
+                        with open(fn, 'w') as fh:
+                            fh.writelines([str(val)])
+                    except OSError as err:
+                        logger.warning('updating sysctl {}/{} failed: {}'.format(
+                            family, key, err.args[1]))
+                logger.log_change(log_str)
+                return True
+        finally:
+            if self.netns.netns is not None:
+                pyroute2.netns.popns()
 
     def apply(self, iface_current, do_apply, iface_config=None):
         # if None the interface has already the final name..
         if iface_config is None:
             iface_config = iface_current
 
         if not iface_config in self.sysctls:
@@ -45,13 +60,9 @@
         logger.debug('checking sysctl', extra={'iface': iface_config})
 
         changes = False
         for family in self.sysctls[iface_config].keys():
             for key, val in self.sysctls[iface_config][family].items():
                 changes = changes or self.set_sysctl(iface_current, iface_config, family, key, val, do_apply)
 
-        if changes:
-            logger.info(
-                'change (sysctl)', extra={'iface': iface_config, 'style': IfStateLogging.STYLE_CHG})
-
     def has_settings(self, iface):
         return iface in self.sysctls
```

### Comparing `ifstate-1.8.5/libifstate/tc/__init__.py` & `ifstate-1.9.0/libifstate/tc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from libifstate.util import logger, ipr, IfStateLogging
+from libifstate.util import logger, IfStateLogging
 from libifstate.exception import ExceptionCollector, netlinkerror_classes
 
 
 class TC():
     ROOT_HANDLE = 0xFFFFFFFF
     INGRESS_HANDLE = 0xFFFF0000
     INGRESS_PARENT = 0xFFFFFFF1
@@ -29,40 +29,41 @@
 
         l = s.split(':')
         if l[1] == "":
             l[1] = "0"
 
         return int(l[0], 16) << 16 | int(l[1], 16)
 
-    def __init__(self, iface, tc):
+    def __init__(self, netns, iface, tc):
+        self.netns = netns
         self.iface = iface
         self.idx = None
         self.tc = tc
 
-    def get_qdisc(self, ipr_qdiscs, parent):
-        for qdisc in ipr_qdiscs:
+    def get_qdisc(self, netns_qdiscs, parent):
+        for qdisc in netns_qdiscs:
             if qdisc['parent'] == parent:
                 return qdisc
 
-    def get_qchild(self, ipr_qdiscs, parent, slot):
-        for qdisc in ipr_qdiscs:
+    def get_qchild(self, netns_qdiscs, parent, slot):
+        for qdisc in netns_qdiscs:
             if qdisc['parent'] == parent | slot:
                 return qdisc
 
     def apply_ingress(self, ingress, qdisc, excpts, do_apply):
         logger.debug('checking ingress qdisc', extra={'iface': self.iface})
         if not ingress:
             if qdisc:
                 if do_apply:
                     opts = {
                         "index": self.idx,
                         "parent": TC.INGRESS_PARENT,
                     }
                     try:
-                        ipr.tc("del", **opts)
+                        self.netns.ipr.tc("del", **opts)
                     except Exception as err:
                         if not isinstance(err, netlinkerror_classes):
                             raise
                         logger.warning('removing ingress qdisc on {} failed: {}'.format(
                             self.iface, err.args[1]))
                         excpts.add('del', err, **opts)
                 return True
@@ -70,15 +71,15 @@
             if not qdisc:
                 if do_apply:
                     opts = {
                         "index": self.idx,
                         "kind": "ingress",
                     }
                     try:
-                        ipr.tc("add", **opts)
+                        self.netns.ipr.tc("add", **opts)
                     except Exception as err:
                         if not isinstance(err, netlinkerror_classes):
                             raise
                         logger.warning('adding ingress qdisc on {} failed: {}'.format(
                             self.iface, err.args[1]))
                         excpts.add('add', err, **opts)
                 return True
@@ -99,40 +100,40 @@
                     TC.int2handle(qdisc["handle"]), tc["handle"]), extra={'iface': self.iface})
                 if TC.handle2int(tc["handle"]) != qdisc["handle"]:
                     recreate = True
 
         if recreate and do_apply:
             if qdisc is not None:
                 try:
-                    ipr.tc("del", index=self.idx, parent=qdisc["parent"])
+                    self.netns.ipr.tc("del", index=self.idx, parent=qdisc["parent"])
                 except:
                     pass
 
         opts = {
             "index": self.idx,
             "parent": TC.int2handle(parent),
         }
         for k, v in tc.items():
             if k != "children":
                 opts[k] = v
 
         if do_apply:
             if recreate:
                 try:
-                    ipr.tc("add", **opts)
+                    self.netns.ipr.tc("add", **opts)
                 except Exception as err:
                     if not isinstance(err, netlinkerror_classes):
                         raise
                     logger.warning('adding qdisc {} on {} failed: {}'.format(
                         opts.get("handle"), self.iface, err.args[1]))
                     excpts.add('add', err, **opts)
             else:
                 # soft update for TCA_OPTIONS
                 try:
-                    ipr.tc("change", **opts)
+                    self.netns.ipr.tc("change", **opts)
                 except Exception as err:
                     if not isinstance(err, netlinkerror_classes):
                         raise
                     logger.warning('updating qdisc {} on {} failed: {}'.format(
                         opts.get("handle"), self.iface, err.args[1]))
                     excpts.add('change', err, **opts)
 
@@ -175,15 +176,15 @@
                 if do_apply:
                     opts = {
                         "index": self.idx,
                         "info": ipr_filter["info"],
                         "parent": parent,
                     }
                     try:
-                        ipr.del_filter_by_info(**opts)
+                        self.netns.ipr.del_filter_by_info(**opts)
                     except Exception as err:
                         if not isinstance(err, netlinkerror_classes):
                             raise
                         logger.warning('deleting filter #{} on {} failed: {}'.format(
                             prio, self.iface, err.args[1]))
                         excpts.add('del', err, **opts)
 
@@ -192,103 +193,99 @@
                 for tc_filter in tc_filters[parent].values():
                     tc_filter['index'] = self.idx
                     if "action" in tc_filter:
                         for action in tc_filter["action"]:
                             if action["kind"] == "mirred":
                                 # get ifindex
                                 action["ifindex"] = next(
-                                    iter(ipr.link_lookup(ifname=action["dev"])), None)
+                                    iter(self.netns.ipr.link_lookup(ifname=action["dev"])), None)
 
                                 if self.idx == None:
                                     logger.warning("filter #{} references unknown interface {}".format(
                                         tc_filter["prio"], action["dev"]), extra={'iface': self.iface})
                                     continue
                     if "parent" in tc_filter:
                         tc_filter["parent"] = TC.handle2int(tc_filter["parent"])
                     try:
                         try:
-                            ipr.tc("replace-filter", **tc_filter)
+                            self.netns.ipr.tc("replace-filter", **tc_filter)
                             # replace seems only to work if there is no filter
                             # => something has changed
                             changes = True
                         except Exception as err:
                             if not isinstance(err, netlinkerror_classes):
                                 raise
                             # replace does not work, supress changes result
                             # for now
                             #changes = True
                             opts = {
                                 "index": self.idx,
                                 "info": tc_filter["prio"] << 16,
                                 "parent": parent,
                             }
-                            ipr.del_filter_by_info(**opts)
-                            ipr.tc("add-filter", **tc_filter)
+                            self.netns.ipr.del_filter_by_info(**opts)
+                            self.netns.ipr.tc("add-filter", **tc_filter)
 
                     except Exception as err:
                         if not isinstance(err, netlinkerror_classes):
                             raise
                         logger.warning('replace filter #{} on {} failed: {}'.format(
                             tc_filter['prio'], self.iface, err.args[1]))
                         excpts.add('replace', err, **tc_filter)
 
         return changes
 
     def apply(self, do_apply):
         excpts = ExceptionCollector(ifname=self.iface)
 
         # get ifindex
-        self.idx = next(iter(ipr.link_lookup(ifname=self.iface)), None)
+        self.idx = next(iter(self.netns.ipr.link_lookup(ifname=self.iface)), None)
 
         if self.idx == None:
             logger.warning('link missing', extra={'iface': self.iface})
             return
 
         changes = []
         ipr_qdiscs = None
 
         # apply ingress qdics
         if "ingress" in self.tc:
-            ipr_qdiscs = ipr.get_qdiscs(index=self.idx)
+            ipr_qdiscs = self.netns.ipr.get_qdiscs(index=self.idx)
             if self.apply_ingress(self.tc["ingress"],
                                   self.get_qdisc(
                                       ipr_qdiscs, TC.INGRESS_PARENT),
                                   excpts,
                                   do_apply):
                 changes.append("ingress")
 
         # apply qdisc tree
         if "qdisc" in self.tc:
             if ipr_qdiscs is None:
-                ipr_qdiscs = ipr.get_qdiscs(index=self.idx)
+                ipr_qdiscs = self.netns.ipr.get_qdiscs(index=self.idx)
             logger.debug('checking qdisc tree', extra={'iface': self.iface})
             if self.apply_qtree(
                     self.tc["qdisc"],
                     self.get_qdisc(ipr_qdiscs, TC.ROOT_HANDLE),
                     ipr_qdiscs,
                     TC.ROOT_HANDLE,
                     excpts,
                     do_apply):
                 changes.append("qdisc")
 
         # apply filters
         if "filter" in self.tc:
-            ipr_filters = ipr.get_filters(
-                index=self.idx) + ipr.get_filters(index=self.idx, parent=TC.INGRESS_HANDLE)
+            ipr_filters = self.netns.ipr.get_filters(
+                index=self.idx) + self.netns.ipr.get_filters(index=self.idx, parent=TC.INGRESS_HANDLE)
             logger.debug('checking filters', extra={'iface': self.iface})
             if self.apply_filter(
                     self.tc["filter"],
                     ipr_filters,
                     excpts,
                     do_apply):
                 changes.append("filter")
 
         if len(changes) > 0:
-            logger.info(
-                'change ({})'.format(", ".join(changes)),
-                extra={'iface': self.iface, 'style': IfStateLogging.STYLE_CHG})
+            logger.log_change('tc', 'change ({})'.format(", ".join(changes)))
         else:
-            logger.info(
-                'ok',
-                extra={'iface': self.iface, 'style': IfStateLogging.STYLE_OK})
+            logger.log_ok('tc')
 
         return excpts
```

### Comparing `ifstate-1.8.5/libifstate/wireguard/__init__.py` & `ifstate-1.9.0/libifstate/wireguard/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,61 +1,67 @@
 from libifstate.util import logger, IfStateLogging
-from libifstate.exception import netlinkerror_classes
+from libifstate.exception import netlinkerror_classes, FeatureMissingError
 from wgnlpy import WireGuard as WG
 from ipaddress import ip_network
 import collections
-
-wg = WG()
-
+import pyroute2.netns
 
 class WireGuard():
-    def __init__(self, iface, wireguard):
+    def __init__(self, netns, iface, wireguard):
+        self.netns = netns
         self.iface = iface
         self.wireguard = wireguard
 
+        if self.netns.netns is not None:
+            pyroute2.netns.pushns(self.netns.netns)
+
+        try:
+            self.wg = WG()
+        finally:
+            if self.netns.netns is not None:
+                pyroute2.netns.popns()
+
         # convert allowedips peers settings into IPv[46]Network objects
         # and remove duplicates
         if 'peers' in self.wireguard:
             for i, peer in enumerate(self.wireguard['peers']):
                 if 'allowedips' in peer:
                     self.wireguard['peers'][i]['allowedips'] = set(
                         [ip_network(x) for x in self.wireguard['peers'][i]['allowedips']])
 
     def apply(self, do_apply):
         # get kernel's wireguard settings for the interface
         try:
-            state = wg.get_interface(
+            state = self.wg.get_interface(
                 self.iface, spill_private_key=True, spill_preshared_keys=True)
         except Exception as err:
             logger.warning('WireGuard on {} failed: {}'.format(
                 self.iface, err.args[1]))
             return
 
         # check base settings (not the peers, yet)
         has_changes = False
         for setting in [x for x in self.wireguard.keys() if x != 'peers']:
             logger.debug('  %s: %s => %s', setting, getattr(
                 state, setting), self.wireguard[setting], extra={'iface': self.iface})
             has_changes |= self.wireguard[setting] != getattr(state, setting)
 
         if has_changes:
-            logger.info('change [iface]', extra={
-                        'iface': self.iface, 'style': IfStateLogging.STYLE_CHG})
+            logger.log_change('wireguard')
             if do_apply:
                 try:
-                    wg.set_interface(
+                    self.wg.set_interface(
                         self.iface, **{k: v for k, v in self.wireguard.items() if k != "peers"})
                 except Exception as err:
                     if not isinstance(err, netlinkerror_classes):
                         raise
                     logger.warning('updating iface {} failed: {}'.format(
                         self.iface, err.args[1]))
         else:
-            logger.info('ok [iface]', extra={
-                        'iface': self.iface, 'style': IfStateLogging.STYLE_OK})
+            logger.log_ok('wireguard')
 
         # check peers list if provided
         if 'peers' in self.wireguard:
             peers = getattr(state, 'peers')
             has_pchanges = False
 
             avail = []
@@ -63,15 +69,15 @@
                 avail.append(peer['public_key'])
                 pubkey = next(
                     iter([x for x in peers.keys() if x == peer['public_key']]), None)
                 if pubkey is None:
                     has_pchanges = True
                     if do_apply:
                         try:
-                            wg.set_peer(self.iface, **peer)
+                            self.wg.set_peer(self.iface, **peer)
                         except Exception as err:
                             if not isinstance(err, netlinkerror_classes):
                                 raise
                             logger.warning('add peer to {} failed: {}'.format(
                                 self.iface, err.args[1]))
                 else:
                     pchange = False
@@ -87,31 +93,29 @@
                             pchange |= str(peer[setting]) != str(getattr(
                                 peers[pubkey], setting))
 
                     if pchange:
                         has_pchanges = True
                         if do_apply:
                             try:
-                                wg.set_peer(self.iface, **peer)
+                                self.wg.set_peer(self.iface, **peer)
                             except Exception as err:
                                 if not isinstance(err, netlinkerror_classes):
                                     raise
                                 logger.warning('change peer at {} failed: {}'.format(
                                     self.iface, err.args[1]))
 
             for peer in peers:
                 if not peer in avail:
                     has_pchanges = True
                     if do_apply:
                         try:
-                            wg.remove_peers(self.iface, peer)
+                            self.wg.remove_peers(self.iface, peer)
                         except Exception as err:
                             if not isinstance(err, netlinkerror_classes):
                                 raise
                             logger.warning('remove peer from {} failed: {}'.format(
                                 self.iface, err.args[1]))
             if has_pchanges:
-                logger.info('change [peers]', extra={
-                            'iface': self.iface, 'style': IfStateLogging.STYLE_CHG})
+                logger.log_change('wg.peers')
             else:
-                logger.info('ok [peers]', extra={
-                            'iface': self.iface, 'style': IfStateLogging.STYLE_OK})
+                logger.log_ok('wg.peers')
```

### Comparing `ifstate-1.8.5/libifstate/xdp/__init__.py` & `ifstate-1.9.0/libifstate/xdp/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,161 +1,170 @@
-from libifstate.util import logger, ipr, IfStateLogging
+from libifstate.util import logger, IfStateLogging
 from libifstate.exception import netlinkerror_classes
 from libifstate.bpf import libbpf, struct_bpf_prog_info, bpfs_ifstate_dir
 
+from pyroute2 import IPRoute
+
 from pyroute2.netlink.rtnl.ifinfmsg import XDP_FLAGS_SKB_MODE
 from pyroute2.netlink.rtnl.ifinfmsg import XDP_FLAGS_DRV_MODE
 from pyroute2.netlink.rtnl.ifinfmsg import XDP_FLAGS_HW_MODE
 
 import ctypes
 import os
+import pyroute2.netns
 import shutil
 
 class XDP():
-    def __init__(self, iface, xdp):
+    def __init__(self, netns, iface, xdp):
+        self.netns = netns
         self.iface = iface
         self.xdp = xdp
 
     def apply(self, do_apply, bpf_progs):
-        self.link = next(iter(ipr.get_links(ifname=self.iface)), None)
+        self.link = next(iter(self.netns.ipr.get_links(ifname=self.iface)), None)
 
         if self.link == None:
             logger.warning('link missing', extra={'iface': self.iface})
             return
 
-        # get ifindex
-        self.idx = self.link['index']
+        if self.netns.netns is not None:
+            pyroute2.netns.pushns(self.netns.netns)
 
-        # new BPF instance (from pinned, bpf or xdp settings)
-        new_prog_tag = None
-        new_prog_fd = None
-
-        # get current BPF tag, if any
-        current_prog_tag = None
-        current_prog_id = None
-        current_attached = None
-        ifla_xdp = self.link.get_attr('IFLA_XDP')
-        if ifla_xdp is not None:
-            current_prog_id = ifla_xdp.get_attr('IFLA_XDP_PROG_ID')
-            current_attached = ifla_xdp.get_attr('IFLA_XDP_ATTACHED')
-
-        if current_prog_id:
-            current_prog_fd = libbpf.bpf_prog_get_fd_by_id(current_prog_id)
-            if current_prog_fd < 0:
-                logger.warning('could not get current XDP prog fd for {}: {}'.format(
-                    self.iface, os.strerror(-current_prog_fd)))
+        try:
+            # get ifindex
+            self.idx = self.link['index']
+
+            # new BPF instance (from pinned, bpf or xdp settings)
+            new_prog_tag = None
+            new_prog_fd = None
+
+            # get current BPF tag, if any
+            current_prog_tag = None
+            current_prog_id = None
+            current_attached = None
+            ifla_xdp = self.link.get_attr('IFLA_XDP')
+            if ifla_xdp is not None:
+                current_prog_id = ifla_xdp.get_attr('IFLA_XDP_PROG_ID')
+                current_attached = ifla_xdp.get_attr('IFLA_XDP_ATTACHED')
+
+            if current_prog_id:
+                current_prog_fd = libbpf.bpf_prog_get_fd_by_id(current_prog_id)
+                if current_prog_fd < 0:
+                    logger.warning('could not get current XDP prog fd for {}: {}'.format(
+                        self.iface, os.strerror(-current_prog_fd)))
+                else:
+                    current_prog_info = struct_bpf_prog_info()
+                    current_prog_size = ctypes.c_uint(ctypes.sizeof(current_prog_info))
+                    rc = libbpf.bpf_obj_get_info_by_fd(current_prog_fd, ctypes.byref(current_prog_info), ctypes.byref(current_prog_size))
+                    if rc == 0:
+                        current_prog_tag = bytes(current_prog_info.tag).hex()
+
+                        logger.debug('current prog tag: {}'.format(current_prog_tag), extra={
+                                    'iface': self.iface})
+                    else:
+                        logger.warning('could not get current XDP obj info for {}: {}'.format(
+                            self.iface, os.strerror(-rc)))
+
+            logger.debug('current attached: {}'.format(current_attached), extra={
+                'iface': self.iface})
+
+            # load new BPF prog
+            new_obj = None
+            if not self.xdp:
+                new_prog_fd = -1
+            elif 'pinned' in self.xdp:
+                new_prog_fd = libbpf.bpf_obj_get( os.fsencode(self.xdp["pinned"]) )
+
+                if new_prog_fd < 0:
+                    logger.warning("pinned BPF object '{}' cannot be opened: {}".format(
+                        self.xdp["pinned"], os.strerror(-new_prog_fd)))
+            elif 'bpf' in self.xdp:
+                if bpf_progs is not None:
+                    (new_prog_fd, new_prog_tag) = bpf_progs.get_bpf(self.xdp["bpf"])
+
+                if new_prog_fd == -1 or new_prog_fd is None:
+                    logger.warning("BPF program '{}' not loaded for {}".format(
+                        self.xdp["bpf"], self.iface))
+                else:
+                    logger.debug('new prog tag: {}'.format(new_prog_tag), extra={
+                                'iface': self.iface})
             else:
-                current_prog_info = struct_bpf_prog_info()
-                current_prog_size = ctypes.c_uint(ctypes.sizeof(current_prog_info))
-                rc = libbpf.bpf_obj_get_info_by_fd(current_prog_fd, ctypes.byref(current_prog_info), ctypes.byref(current_prog_size))
+                assert False, "unhandled XDP settings"
+
+            # get new prog tag
+            if new_prog_fd != -1 and new_prog_fd != None and new_prog_tag == None:
+                info = struct_bpf_prog_info()
+                sz = ctypes.c_uint(ctypes.sizeof(info))
+                rc = libbpf.bpf_obj_get_info_by_fd(new_prog_fd, ctypes.byref(info), ctypes.byref(sz))
                 if rc == 0:
-                    current_prog_tag = bytes(current_prog_info.tag).hex()
+                    new_prog_tag = bytes(info.tag).hex()
 
-                    logger.debug('current prog tag: {}'.format(current_prog_tag), extra={
+                    logger.debug('new prog tag: {}'.format(new_prog_tag), extra={
                                 'iface': self.iface})
                 else:
-                    logger.warning('could not get current XDP obj info for {}: {}'.format(
-                        self.iface, os.strerror(-rc)))
-
-        logger.debug('current attached: {}'.format(current_attached), extra={
-            'iface': self.iface})
-
-        # load new BPF prog
-        new_obj = None
-        if not self.xdp:
-            new_prog_fd = -1
-        elif 'pinned' in self.xdp:
-            new_prog_fd = libbpf.bpf_obj_get( os.fsencode(self.xdp["pinned"]) )
-
-            if new_prog_fd < 0:
-                logger.warning("pinned BPF object '{}' cannot be opened: {}".format(
-                    self.xdp["pinned"], os.strerror(-new_prog_fd)))
-        elif 'bpf' in self.xdp:
-            if bpf_progs is not None:
-                (new_prog_fd, new_prog_tag) = bpf_progs.get_bpf(self.xdp["bpf"])
-
-            if new_prog_fd == -1:
-                logger.warning("BPF program '{}' not loaded for {}".format(
-                    self.xdp["bpf"], self.iface))
-            else:
-                logger.debug('new prog tag: {}'.format(new_prog_tag), extra={
-                            'iface': self.iface})
-        else:
-            assert False, "unhandled XDP settings"
-
-        # get new prog tag
-        if new_prog_fd != -1 and new_prog_tag == None:
-            info = struct_bpf_prog_info()
-            sz = ctypes.c_uint(ctypes.sizeof(info))
-            rc = libbpf.bpf_obj_get_info_by_fd(new_prog_fd, ctypes.byref(info), ctypes.byref(sz))
-            if rc == 0:
-                new_prog_tag = bytes(info.tag).hex()
+                    logger.warning('XDP failed to get prog info on {}'.format(
+                        self.iface))
 
-                logger.debug('new prog tag: {}'.format(new_prog_tag), extra={
-                            'iface': self.iface})
+            # get attach mode flags
+            new_attached = self.xdp.get("mode", "auto")
+            if type(new_attached) != list:
+                new_attached = [new_attached]
+
+            new_flags = 0
+            if "auto" in new_attached:
+                new_attached = ["xdp", "xdpgeneric", "xdpoffload"]
             else:
-                logger.warning('XDP failed to get prog info on {}'.format(
-                    self.iface))
-
-        # get attach mode flags
-        new_attached = self.xdp.get("mode", "auto")
-        if type(new_attached) != list:
-            new_attached = [new_attached]
-
-        new_flags = 0
-        if "auto" in new_attached:
-            new_attached = ["xdp", "xdpgeneric", "xdpoffload"]
-        else:
-            if "xdp" in new_attached:
-                new_flags = new_flags | XDP_FLAGS_DRV_MODE
-            if "xdpgeneric" in new_attached:
-                new_flags = new_flags | XDP_FLAGS_SKB_MODE
-            if "xdpoffload" in new_attached:
-                new_flags = new_flags | XDP_FLAGS_HW_MODE
-
-        logger.debug('new attached: {}'.format(", ".join(new_attached)), extra={
-            'iface': self.iface})
-
-        logger.debug('new flags: {}'.format(new_flags), extra={
-            'iface': self.iface})
-
-        # set new XDP prog if tag or attach mode has changed
-        if current_prog_tag != new_prog_tag or not current_attached in new_attached:
-            if do_apply:
-                attach_ok = False
-                try:
-                    ipr.link('set', index=self.idx, xdp_fd=new_prog_fd, xdp_flags=new_flags)
-                    attach_ok = True
-                except Exception as err:
-                    if not isinstance(err, netlinkerror_classes):
-                        raise
-
-                    # try again: detaching XDP first
+                if "xdp" in new_attached:
+                    new_flags = new_flags | XDP_FLAGS_DRV_MODE
+                if "xdpgeneric" in new_attached:
+                    new_flags = new_flags | XDP_FLAGS_SKB_MODE
+                if "xdpoffload" in new_attached:
+                    new_flags = new_flags | XDP_FLAGS_HW_MODE
+
+            logger.debug('new attached: {}'.format(", ".join(new_attached)), extra={
+                'iface': self.iface})
+
+            logger.debug('new flags: {}'.format(new_flags), extra={
+                'iface': self.iface})
+
+            # set new XDP prog if tag or attach mode has changed
+            if current_prog_tag != new_prog_tag or not current_attached in new_attached:
+                if do_apply:
+                    ipr = IPRoute()
+                    attach_ok = False
                     try:
-                        ipr.link('set', index=self.idx, xdp_fd=-1)
-
                         ipr.link('set', index=self.idx, xdp_fd=new_prog_fd, xdp_flags=new_flags)
                         attach_ok = True
                     except Exception as err:
                         if not isinstance(err, netlinkerror_classes):
                             raise
 
-                        logger.warning('attaching XDP program on {} failed: {}'.format(
-                            self.iface, err.args[1]))
+                        # try again: detaching XDP first
+                        try:
+                            ipr.link('set', index=self.idx, xdp_fd=-1)
+
+                            ipr.link('set', index=self.idx, xdp_fd=new_prog_fd, xdp_flags=new_flags)
+                            attach_ok = True
+                        except Exception as err:
+                            if not isinstance(err, netlinkerror_classes):
+                                raise
 
-            if new_prog_fd == -1:
-                logger.info('detach', extra={
-                            'iface': self.iface, 'style': IfStateLogging.STYLE_DEL})
+                            logger.warning('attaching XDP program on {} failed: {}'.format(
+                                self.iface, err.args[1]))
+
+                if new_prog_fd == -1:
+                    logger.log_del('xdp', 'detach')
+                else:
+                    logger.log_change('xdp')
             else:
-                logger.info('change', extra={
-                            'iface': self.iface, 'style': IfStateLogging.STYLE_CHG})
-        else:
-            logger.info(
-                'ok',
-                extra={'iface': self.iface, 'style': IfStateLogging.STYLE_OK})
+                logger.log_ok('xdp')
+
+        finally:
+            if self.netns.netns is not None:
+                pyroute2.netns.popns()
 
 try:
     libbpf.bpf_obj_get_info_by_fd
     libbpf.bpf_object__name
     libbpf.bpf_object__next_program
     libbpf.bpf_object__load
     libbpf.bpf_object__open_file
```

### Comparing `ifstate-1.8.5/schema/ifstate.conf.schema.json` & `ifstate-1.9.0/schema/ifstate.conf.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9822362836041337%*

 * *Differences: {"'$defs'": "{'iface-link_link-netns': OrderedDict([('type', ['string', 'null']), ('description', "*

 * *            '"specifies the parent\'s netns name")]), \'iface-link_master-netns\': '*

 * *            'OrderedDict([(\'type\', [\'string\', \'null\']), (\'description\', "specifies the '*

 * *            'master\'s netns name")])}',*

 * * "'properties'": "{'ignore': {'properties': {'netns': OrderedDict([('description', 'netns "*

 * *                 "namespaces matching this list of regex will be ignored'), ('type', 'array'), "*

 * * […]*

```diff
@@ -31,21 +31,35 @@
         "iface-link_link": {
             "description": "specifies a parent device name or index",
             "type": [
                 "integer",
                 "string"
             ]
         },
+        "iface-link_link-netns": {
+            "description": "specifies the parent's netns name",
+            "type": [
+                "string",
+                "null"
+            ]
+        },
         "iface-link_master": {
             "description": "specifies a master device name or index",
             "type": [
                 "integer",
                 "string"
             ]
         },
+        "iface-link_master-netns": {
+            "description": "specifies the master's netns name",
+            "type": [
+                "string",
+                "null"
+            ]
+        },
         "iface-link_mtu": {
             "description": "change the mtu of the device",
             "maximum": 65536,
             "minimum": 68,
             "type": "integer"
         },
         "iface-link_state": {
@@ -1004,14 +1018,98 @@
                 }
             },
             "required": [
                 "default"
             ],
             "type": "object"
         },
+        "defaults": {
+            "description": "default settings for configured interfaces",
+            "items": {
+                "additionalProperties": false,
+                "description": "first matching entry will be used, settings will be overriden by explicit configured interface settings",
+                "properties": {
+                    "clear_addresses": {
+                        "default": false,
+                        "description": "implicit remove all ip addresses",
+                        "type": "boolean"
+                    },
+                    "clear_neighbours": {
+                        "default": false,
+                        "description": "implicit remove all permanent ip neighbours",
+                        "type": "boolean"
+                    },
+                    "link": {
+                        "additionalProperties": false,
+                        "description": "implicit link settings for matching interfaces",
+                        "properties": {
+                            "group": {
+                                "$ref": "#/$defs/iface-link_group"
+                            },
+                            "ifalias": {
+                                "$ref": "#/$defs/iface-link_ifalias"
+                            },
+                            "link": {
+                                "$ref": "#/$defs/iface-link_link"
+                            },
+                            "link_netns": {
+                                "$ref": "#/$defs/iface-link_link-netns"
+                            },
+                            "master": {
+                                "$ref": "#/$defs/iface-link_master"
+                            },
+                            "master_netns": {
+                                "$ref": "#/$defs/iface-link_master-netns"
+                            },
+                            "mtu": {
+                                "$ref": "#/$defs/iface-link_mtu"
+                            },
+                            "state": {
+                                "$ref": "#/$defs/iface-link_state"
+                            },
+                            "txqlen": {
+                                "$ref": "#/$defs/iface-link_txqlen"
+                            }
+                        },
+                        "type": "object"
+                    },
+                    "match": {
+                        "description": "apply default settings for interfaces  matching any list item (OR)",
+                        "items": {
+                            "additionalProperties": false,
+                            "description": "all conditions that must match (AND)",
+                            "properties": {
+                                "ifname": {
+                                    "description": "regex to match interface name",
+                                    "examples": [
+                                        "^eth\\d+$"
+                                    ],
+                                    "type": "string"
+                                },
+                                "kind": {
+                                    "description": "regex to match link type",
+                                    "examples": [
+                                        "^physical$",
+                                        "^(physical|vlan)$"
+                                    ],
+                                    "type": "string"
+                                }
+                            },
+                            "type": "object"
+                        },
+                        "type": "array"
+                    }
+                },
+                "required": [
+                    "match"
+                ],
+                "type": "object"
+            },
+            "type": "array"
+        },
         "ignore": {
             "additionalProperties": false,
             "description": "ignore patterns to skip interface, ip address or routing objects",
             "properties": {
                 "ifname": {
                     "$ref": "#/$defs/ignore-ifname"
                 },
@@ -1025,14 +1123,25 @@
                     "$ref": "#/$defs/ignore-ipaddr"
                 },
                 "ipaddr_dynamic": {
                     "default": true,
                     "description": "ignore dynamic assigned ip addresses",
                     "type": "boolean"
                 },
+                "netns": {
+                    "description": "netns namespaces matching this list of regex will be ignored",
+                    "items": {
+                        "description": "regex to match interface name",
+                        "examples": [
+                            "^tenant-\\d+"
+                        ],
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
                 "routes": {
                     "$ref": "#/$defs/ignore-routes"
                 },
                 "routes_builtin": {
                     "$ref": "#/$defs/ignore-routes"
                 },
                 "rules": {
@@ -1650,14 +1759,17 @@
                                     "kind": {
                                         "const": "ifb",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -1683,14 +1795,17 @@
                                     "kind": {
                                         "const": "ip6tnl",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -1716,14 +1831,17 @@
                                     "kind": {
                                         "const": "ipoib",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -1749,14 +1867,17 @@
                                     "kind": {
                                         "const": "ipvlan",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -1782,14 +1903,17 @@
                                     "kind": {
                                         "const": "macvlan",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -1815,14 +1939,17 @@
                                     "kind": {
                                         "const": "macvtap",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -1848,14 +1975,17 @@
                                     "kind": {
                                         "const": "team",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -1882,14 +2012,17 @@
                                     "kind": {
                                         "const": "tun",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "tun_group": {
@@ -1992,14 +2125,17 @@
                                     "kind": {
                                         "const": "vrf",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2025,14 +2161,17 @@
                                     "kind": {
                                         "const": "vti",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2058,14 +2197,17 @@
                                     "kind": {
                                         "const": "vti6",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2286,14 +2428,17 @@
                                     "kind": {
                                         "const": "bond",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2335,14 +2480,17 @@
                                     "kind": {
                                         "const": "bridge",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2377,14 +2525,17 @@
                                             "physical"
                                         ],
                                         "type": "string"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "permaddr": {
                                         "$ref": "#/$defs/iface-link_address",
                                         "description": "select interface by permanent address [ethtool -P]"
                                     },
@@ -2418,14 +2569,17 @@
                                             "dummy"
                                         ],
                                         "type": "string"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2456,14 +2610,17 @@
                                             "vxcan"
                                         ],
                                         "type": "string"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "peer": {
                                         "$ref": "#/$defs/iface-link_link"
                                     },
                                     "state": {
@@ -2494,17 +2651,23 @@
                                     "kind": {
                                         "const": "vlan",
                                         "description": "link type"
                                     },
                                     "link": {
                                         "$ref": "#/$defs/iface-link_link"
                                     },
+                                    "link_netns": {
+                                        "$ref": "#/$defs/iface-link_link-netns"
+                                    },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2551,14 +2714,17 @@
                                     "kind": {
                                         "const": "vxlan",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2604,14 +2770,17 @@
                                     "kind": {
                                         "const": "ipip",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2640,14 +2809,17 @@
                                     "kind": {
                                         "const": "sit",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "sit_local": {
                                         "$ref": "#/$defs/iface-link_tun-local4"
                                     },
                                     "sit_remote": {
@@ -2695,14 +2867,17 @@
                                             "gretap"
                                         ],
                                         "type": "string"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2744,14 +2919,17 @@
                                             "ip6gretap"
                                         ],
                                         "type": "string"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2791,14 +2969,17 @@
                                     "kind": {
                                         "const": "geneve",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2838,14 +3019,17 @@
                                     "kind": {
                                         "const": "geneve",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2874,14 +3058,17 @@
                                     "kind": {
                                         "const": "wireguard",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -2908,14 +3095,17 @@
                                     "kind": {
                                         "const": "xfrm",
                                         "description": "link type"
                                     },
                                     "master": {
                                         "$ref": "#/$defs/iface-link_master"
                                     },
+                                    "master_netns": {
+                                        "$ref": "#/$defs/iface-link_master-netns"
+                                    },
                                     "mtu": {
                                         "$ref": "#/$defs/iface-link_mtu"
                                     },
                                     "state": {
                                         "$ref": "#/$defs/iface-link_state"
                                     },
                                     "txqlen": {
@@ -3406,14 +3596,41 @@
                 "required": [
                     "name"
                 ],
                 "type": "object"
             },
             "type": "array"
         },
+        "namespaces": {
+            "additionalProperties": false,
+            "patternProperties": {
+                ".+": {
+                    "additionalProperties": false,
+                    "properties": {
+                        "bpf": {
+                            "$ref": "#/properties/bpf"
+                        },
+                        "interfaces": {
+                            "$ref": "#/properties/interfaces"
+                        },
+                        "options": {
+                            "$ref": "#/properties/options"
+                        },
+                        "routing": {
+                            "$ref": "#/properties/routing"
+                        }
+                    },
+                    "required": [
+                        "interfaces"
+                    ],
+                    "type": "object"
+                }
+            },
+            "type": "object"
+        },
         "options": {
             "additionalProperties": false,
             "description": "global configuration settings",
             "properties": {
                 "sysctl": {
                     "properties": {
                         "all": {
```

### Comparing `ifstate-1.8.5/setup.py` & `ifstate-1.9.0/setup.py`

 * *Files identical despite different names*

