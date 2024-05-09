# Comparing `tmp/decomp2dbg-3.9.0.tar.gz` & `tmp/decomp2dbg-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decomp2dbg-3.9.0.tar", last modified: Mon Mar  4 19:35:07 2024, max compression
+gzip compressed data, was "decomp2dbg-3.9.1.tar", last modified: Thu May  9 04:03:02 2024, max compression
```

## Comparing `decomp2dbg-3.9.0.tar` & `decomp2dbg-3.9.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:35:07.264931 decomp2dbg-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-03-04 19:35:07.264931 decomp2dbg-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/d2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:35:07.260931 decomp2dbg-3.9.0/decomp2dbg/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:35:07.260931 decomp2dbg-3.9.0/decomp2dbg/clients/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/clients/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:35:07.260931 decomp2dbg-3.9.0/decomp2dbg/clients/gdb/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/clients/gdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/clients/gdb/decompiler_pane.py
--rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/clients/gdb/gdb_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/clients/gdb/gef_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/clients/gdb/pwndbg_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/clients/gdb/symbol_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/clients/gdb/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decomp2dbg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:35:07.264931 decomp2dbg-3.9.0/decomp2dbg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-03-04 19:35:07.000000 decomp2dbg-3.9.0/decomp2dbg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-04 19:35:07.000000 decomp2dbg-3.9.0/decomp2dbg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 19:35:07.000000 decomp2dbg-3.9.0/decomp2dbg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-04 19:35:07.000000 decomp2dbg-3.9.0/decomp2dbg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-04 19:35:07.000000 decomp2dbg-3.9.0/decomp2dbg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-04 19:35:07.000000 decomp2dbg-3.9.0/decomp2dbg.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:35:07.260931 decomp2dbg-3.9.0/decompilers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:35:07.260931 decomp2dbg-3.9.0/decompilers/d2d_angr/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decompilers/d2d_angr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decompilers/d2d_angr/d2d_angr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decompilers/d2d_angr/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:35:07.264931 decomp2dbg-3.9.0/decompilers/d2d_binja/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decompilers/d2d_binja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decompilers/d2d_binja/d2d_binja.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decompilers/d2d_binja/plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decompilers/d2d_binja/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:35:07.264931 decomp2dbg-3.9.0/decompilers/d2d_ida/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 19:35:07.264931 decomp2dbg-3.9.0/decompilers/d2d_ida/d2d_ida/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decompilers/d2d_ida/d2d_ida/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decompilers/d2d_ida/d2d_ida/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decompilers/d2d_ida/d2d_ida/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decompilers/d2d_ida/d2d_ida.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/decompilers/server_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-04 19:35:07.264931 decomp2dbg-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-03-04 19:35:02.000000 decomp2dbg-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/d2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.493087 decomp2dbg-3.9.1/decomp2dbg/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.493087 decomp2dbg-3.9.1/decomp2dbg/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/decompiler_pane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11095 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/gdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/gef_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/pwndbg_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/symbol_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/clients/gdb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decomp2dbg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decomp2dbg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-09 04:03:02.000000 decomp2dbg-3.9.1/decomp2dbg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-09 04:03:02.000000 decomp2dbg-3.9.1/decomp2dbg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:03:02.000000 decomp2dbg-3.9.1/decomp2dbg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 04:03:02.000000 decomp2dbg-3.9.1/decomp2dbg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-09 04:03:02.000000 decomp2dbg-3.9.1/decomp2dbg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-09 04:03:02.000000 decomp2dbg-3.9.1/decomp2dbg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decompilers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decompilers/d2d_angr/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_angr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_angr/d2d_angr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_angr/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decompilers/d2d_binja/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_binja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_binja/d2d_binja.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_binja/plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_binja/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decompilers/d2d_ida/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/decompilers/server_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-09 04:03:02.497087 decomp2dbg-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-09 04:02:58.000000 decomp2dbg-3.9.1/setup.py
```

### Comparing `decomp2dbg-3.9.0/LICENSE` & `decomp2dbg-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/PKG-INFO` & `decomp2dbg-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decomp2dbg
-Version: 3.9.0
+Version: 3.9.1
 Summary: Symbol syncing framework for decompilers and debuggers
 Home-page: https://github.com/mahaloz/decomp2dbg
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.5
```

### Comparing `decomp2dbg-3.9.0/README.md` & `decomp2dbg-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/d2d.py` & `decomp2dbg-3.9.1/d2d.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decomp2dbg/__main__.py` & `decomp2dbg-3.9.1/decomp2dbg/__main__.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decomp2dbg/clients/client.py` & `decomp2dbg-3.9.1/decomp2dbg/clients/client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decomp2dbg/clients/gdb/decompiler_pane.py` & `decomp2dbg-3.9.1/decomp2dbg/clients/gdb/decompiler_pane.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decomp2dbg/clients/gdb/gdb_client.py` & `decomp2dbg-3.9.1/decomp2dbg/clients/gdb/gdb_client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decomp2dbg/clients/gdb/gef_client.py` & `decomp2dbg-3.9.1/decomp2dbg/clients/gdb/gef_client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decomp2dbg/clients/gdb/pwndbg_client.py` & `decomp2dbg-3.9.1/decomp2dbg/clients/gdb/pwndbg_client.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decomp2dbg/clients/gdb/symbol_mapper.py` & `decomp2dbg-3.9.1/decomp2dbg/clients/gdb/symbol_mapper.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decomp2dbg/clients/gdb/utils.py` & `decomp2dbg-3.9.1/decomp2dbg/clients/gdb/utils.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decomp2dbg/installer.py` & `decomp2dbg-3.9.1/decomp2dbg/installer.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decomp2dbg/utils.py` & `decomp2dbg-3.9.1/decomp2dbg/utils.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decomp2dbg.egg-info/PKG-INFO` & `decomp2dbg-3.9.1/decomp2dbg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decomp2dbg
-Version: 3.9.0
+Version: 3.9.1
 Summary: Symbol syncing framework for decompilers and debuggers
 Home-page: https://github.com/mahaloz/decomp2dbg
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.5
```

### Comparing `decomp2dbg-3.9.0/decomp2dbg.egg-info/SOURCES.txt` & `decomp2dbg-3.9.1/decomp2dbg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decompilers/d2d_angr/d2d_angr.py` & `decomp2dbg-3.9.1/decompilers/d2d_angr/d2d_angr.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decompilers/d2d_angr/server.py` & `decomp2dbg-3.9.1/decompilers/d2d_angr/server.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decompilers/d2d_binja/d2d_binja.py` & `decomp2dbg-3.9.1/decompilers/d2d_binja/d2d_binja.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decompilers/d2d_binja/plugin.json` & `decomp2dbg-3.9.1/decompilers/d2d_binja/plugin.json`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decompilers/d2d_binja/server.py` & `decomp2dbg-3.9.1/decompilers/d2d_binja/server.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decompilers/d2d_ida/d2d_ida/plugin.py` & `decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida/plugin.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decompilers/d2d_ida/d2d_ida/server.py` & `decomp2dbg-3.9.1/decompilers/d2d_ida/d2d_ida/server.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/decompilers/server_template.py` & `decomp2dbg-3.9.1/decompilers/server_template.py`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/setup.cfg` & `decomp2dbg-3.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `decomp2dbg-3.9.0/setup.py` & `decomp2dbg-3.9.1/setup.py`

 * *Files identical despite different names*

