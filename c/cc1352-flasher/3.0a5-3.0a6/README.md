# Comparing `tmp/cc1352_flasher-3.0a5.tar.gz` & `tmp/cc1352_flasher-3.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc1352_flasher-3.0a5.tar", last modified: Thu Jan  4 18:58:06 2024, max compression
+gzip compressed data, was "cc1352_flasher-3.0a6.tar", last modified: Thu May  9 16:54:56 2024, max compression
```

## Comparing `cc1352_flasher-3.0a5.tar` & `cc1352_flasher-3.0a6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 18:58:06.190880 cc1352_flasher-3.0a5/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-01-04 18:57:58.000000 cc1352_flasher-3.0a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-01-04 18:58:06.190880 cc1352_flasher-3.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-01-04 18:57:58.000000 cc1352_flasher-3.0a5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-04 18:57:58.000000 cc1352_flasher-3.0a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-04 18:58:06.190880 cc1352_flasher-3.0a5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 18:58:06.190880 cc1352_flasher-3.0a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 18:58:06.190880 cc1352_flasher-3.0a5/src/cc1352_flasher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-04 18:57:58.000000 cc1352_flasher-3.0a5/src/cc1352_flasher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-04 18:57:58.000000 cc1352_flasher-3.0a5/src/cc1352_flasher/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    57047 2024-01-04 18:57:58.000000 cc1352_flasher-3.0a5/src/cc1352_flasher/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 18:58:06.190880 cc1352_flasher-3.0a5/src/cc1352_flasher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-01-04 18:58:06.000000 cc1352_flasher-3.0a5/src/cc1352_flasher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-01-04 18:58:06.000000 cc1352_flasher-3.0a5/src/cc1352_flasher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 18:58:06.000000 cc1352_flasher-3.0a5/src/cc1352_flasher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-04 18:58:06.000000 cc1352_flasher-3.0a5/src/cc1352_flasher.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-04 18:58:06.000000 cc1352_flasher-3.0a5/src/cc1352_flasher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-04 18:58:06.000000 cc1352_flasher-3.0a5/src/cc1352_flasher.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 18:58:06.190880 cc1352_flasher-3.0a5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-01-04 18:57:58.000000 cc1352_flasher-3.0a5/tests/test_cc1352-flasher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:54:56.897069 cc1352_flasher-3.0a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-09 16:54:52.000000 cc1352_flasher-3.0a6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-05-09 16:54:56.897069 cc1352_flasher-3.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-09 16:54:52.000000 cc1352_flasher-3.0a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-09 16:54:52.000000 cc1352_flasher-3.0a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 16:54:56.897069 cc1352_flasher-3.0a6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:54:56.897069 cc1352_flasher-3.0a6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:54:56.897069 cc1352_flasher-3.0a6/src/cc1352_flasher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:54:52.000000 cc1352_flasher-3.0a6/src/cc1352_flasher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-09 16:54:52.000000 cc1352_flasher-3.0a6/src/cc1352_flasher/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    57164 2024-05-09 16:54:52.000000 cc1352_flasher-3.0a6/src/cc1352_flasher/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:54:56.897069 cc1352_flasher-3.0a6/src/cc1352_flasher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-05-09 16:54:56.000000 cc1352_flasher-3.0a6/src/cc1352_flasher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-09 16:54:56.000000 cc1352_flasher-3.0a6/src/cc1352_flasher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:54:56.000000 cc1352_flasher-3.0a6/src/cc1352_flasher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 16:54:56.000000 cc1352_flasher-3.0a6/src/cc1352_flasher.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-09 16:54:56.000000 cc1352_flasher-3.0a6/src/cc1352_flasher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 16:54:56.000000 cc1352_flasher-3.0a6/src/cc1352_flasher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:54:56.897069 cc1352_flasher-3.0a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-09 16:54:52.000000 cc1352_flasher-3.0a6/tests/test_cc1352-flasher.py
```

### Comparing `cc1352_flasher-3.0a5/LICENSE.md` & `cc1352_flasher-3.0a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cc1352_flasher-3.0a5/PKG-INFO` & `cc1352_flasher-3.0a6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc1352_flasher
-Version: 3.0a5
+Version: 3.0a6
 Summary: Script flash CC1352 on BeaglePlay or BeagleConnect Freedom
 Author-email: Jason Kridner <jkridner@beagleboard.org>, Jelmer Tiete <jelmer@tiete.be>
 License: BSD 3-Clause License
         
         Copyright (c) 2014, Jelmer Tiete <jelmer@tiete.be>.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `cc1352_flasher-3.0a5/README.md` & `cc1352_flasher-3.0a6/README.md`

 * *Files identical despite different names*

### Comparing `cc1352_flasher-3.0a5/pyproject.toml` & `cc1352_flasher-3.0a6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="cc1352_flasher"
-version="3.0a5"
+version="3.0a6"
 description="Script flash CC1352 on BeaglePlay or BeagleConnect Freedom"
 readme="README.md"
 authors=[
   { name = "Jason Kridner", email = "jkridner@beagleboard.org" },
   { name = "Jelmer Tiete", email = "jelmer@tiete.be" }
 ]
 license = { file = "LICENSE.md" }
```

### Comparing `cc1352_flasher-3.0a5/src/cc1352_flasher/cli.py` & `cc1352_flasher-3.0a6/src/cc1352_flasher/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     # >>> dir(gpiod.line_request)
     # ['DIRECTION_AS_IS', 'DIRECTION_INPUT', 'DIRECTION_OUTPUT', 'EVENT_BOTH_EDGES', 'EVENT_FALLING_EDGE', 'EVENT_RISING_EDGE', 'FLAG_ACTIVE_LOW', 'FLAG_BIAS_DISABLE', 'FLAG_BIAS_PULL_DOWN', 'FLAG_BIAS_PULL_UP', 'FLAG_OPEN_DRAIN', 'FLAG_OPEN_SOURCE', '__class__', '__delattr__', '__dict__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__le__', '__lt__', '__module__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', '__weakref__']
     have_gpiod = True
 except ImportError:
     have_gpiod = False
 
 # version
-__version__ = "3.0a5"
+__version__ = "3.0a6"
 
 # Verbose level
 QUIET = 5
 
 try:
     import serial
 except ImportError:
@@ -1172,14 +1172,21 @@
 Examples:
     ./%s -e -w -v example/main.bin
     ./%s -e -w -v --ieee-address 00:12:4b:aa:bb:cc:dd:ee example/main.bin
 
     """ % (sys.argv[0], sys.argv[0], sys.argv[0]))
 
 
+def should_append(p):
+    if os.path.isdir(p):
+        return "/zephyr/zephyr.bin"
+    else:
+        return ""
+
+
 def main():
     conf = {
             'port': 'auto',
             'baud': 500000,
             'force_speed': 0,
             'address': None,
             'force': 0,
@@ -1269,23 +1276,23 @@
             conf['disable-bootloader'] = 1
         elif o == '-E' or o == '--erase-page':
             conf['erase_page'] = str(a)
         elif o == '--bcf':
             conf['erase'] = 1
             conf['write'] = 1
             conf['verify'] = 1
-            conf['append'] = '/zephyr/zephyr.bin'
+            conf['append'] = should_append(args[0])
             conf['bootloader_send_break'] = True
         elif o == '--play':
             conf['erase'] = 1
             conf['write'] = 1
             conf['verify'] = 1
             conf['bootloader_gpio'] = 'auto'
             conf['port'] = '/dev/play/cc1352/uart'
-            conf['append'] = '/zephyr/zephyr.bin'
+            conf['append'] = should_append(args[0])
         elif o == '--version':
             print_version()
             sys.exit(0)
         else:
             assert False, "Unhandled option"
 
     try:
```

### Comparing `cc1352_flasher-3.0a5/src/cc1352_flasher.egg-info/PKG-INFO` & `cc1352_flasher-3.0a6/src/cc1352_flasher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc1352_flasher
-Version: 3.0a5
+Version: 3.0a6
 Summary: Script flash CC1352 on BeaglePlay or BeagleConnect Freedom
 Author-email: Jason Kridner <jkridner@beagleboard.org>, Jelmer Tiete <jelmer@tiete.be>
 License: BSD 3-Clause License
         
         Copyright (c) 2014, Jelmer Tiete <jelmer@tiete.be>.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `cc1352_flasher-3.0a5/tests/test_cc1352-flasher.py` & `cc1352_flasher-3.0a6/tests/test_cc1352-flasher.py`

 * *Files identical despite different names*

