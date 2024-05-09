# Comparing `tmp/silcar_it_tools-0.2.1.tar.gz` & `tmp/silcar_it_tools-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silcar_it_tools-0.2.1.tar", last modified: Fri Apr 19 17:32:26 2024, max compression
+gzip compressed data, was "silcar_it_tools-0.2.2.tar", last modified: Thu May  9 09:38:32 2024, max compression
```

## Comparing `silcar_it_tools-0.2.1.tar` & `silcar_it_tools-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-04-19 17:32:26.298112 silcar_it_tools-0.2.1/
--rw-rw-r--   0 nate      (1000) nate      (1000)     1074 2024-04-17 16:38:17.000000 silcar_it_tools-0.2.1/LICENSE
--rw-r--r--   0 nate      (1000) nate      (1000)     1266 2024-04-19 17:32:26.298112 silcar_it_tools-0.2.1/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)      691 2024-04-19 17:08:42.000000 silcar_it_tools-0.2.1/README.md
--rw-rw-r--   0 nate      (1000) nate      (1000)      868 2024-04-19 17:31:22.000000 silcar_it_tools-0.2.1/pyproject.toml
--rw-rw-r--   0 nate      (1000) nate      (1000)       38 2024-04-19 17:32:26.298112 silcar_it_tools-0.2.1/setup.cfg
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-04-19 17:32:26.294113 silcar_it_tools-0.2.1/src/
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-04-19 17:32:26.294113 silcar_it_tools-0.2.1/src/silcar_it_tools/
--rw-rw-r--   0 nate      (1000) nate      (1000)        0 2024-04-17 17:21:43.000000 silcar_it_tools-0.2.1/src/silcar_it_tools/__init__.py
--rw-rw-r--   0 nate      (1000) nate      (1000)       40 2024-04-19 17:31:35.000000 silcar_it_tools-0.2.1/src/silcar_it_tools/config.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     4063 2024-04-17 16:17:23.000000 silcar_it_tools-0.2.1/src/silcar_it_tools/exe_check.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     2150 2024-04-17 16:10:29.000000 silcar_it_tools-0.2.1/src/silcar_it_tools/packing.py
--rwxrwxr-x   0 nate      (1000) nate      (1000)     2574 2024-04-18 06:03:27.000000 silcar_it_tools-0.2.1/src/silcar_it_tools/usb_utils.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      746 2024-04-17 16:16:57.000000 silcar_it_tools-0.2.1/src/silcar_it_tools/utils.py
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-04-19 17:32:26.298112 silcar_it_tools-0.2.1/src/silcar_it_tools.egg-info/
--rw-r--r--   0 nate      (1000) nate      (1000)     1266 2024-04-19 17:32:26.000000 silcar_it_tools-0.2.1/src/silcar_it_tools.egg-info/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)      480 2024-04-19 17:32:26.000000 silcar_it_tools-0.2.1/src/silcar_it_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)        1 2024-04-19 17:32:26.000000 silcar_it_tools-0.2.1/src/silcar_it_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)      130 2024-04-19 17:32:26.000000 silcar_it_tools-0.2.1/src/silcar_it_tools.egg-info/entry_points.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)        7 2024-04-19 17:32:26.000000 silcar_it_tools-0.2.1/src/silcar_it_tools.egg-info/requires.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       16 2024-04-19 17:32:26.000000 silcar_it_tools-0.2.1/src/silcar_it_tools.egg-info/top_level.txt
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-09 09:38:31.997026 silcar_it_tools-0.2.2/
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1074 2024-04-17 16:38:17.000000 silcar_it_tools-0.2.2/LICENSE
+-rw-r--r--   0 nate      (1000) nate      (1000)     1266 2024-05-09 09:38:31.997026 silcar_it_tools-0.2.2/PKG-INFO
+-rw-rw-r--   0 nate      (1000) nate      (1000)      691 2024-04-19 17:08:42.000000 silcar_it_tools-0.2.2/README.md
+-rw-rw-r--   0 nate      (1000) nate      (1000)      868 2024-04-19 17:31:22.000000 silcar_it_tools-0.2.2/pyproject.toml
+-rw-rw-r--   0 nate      (1000) nate      (1000)       38 2024-05-09 09:38:31.997026 silcar_it_tools-0.2.2/setup.cfg
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-09 09:38:31.993012 silcar_it_tools-0.2.2/src/
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-09 09:38:31.997026 silcar_it_tools-0.2.2/src/silcar_it_tools/
+-rw-rw-r--   0 nate      (1000) nate      (1000)        0 2024-04-17 17:21:43.000000 silcar_it_tools-0.2.2/src/silcar_it_tools/__init__.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)       40 2024-05-09 09:37:47.000000 silcar_it_tools-0.2.2/src/silcar_it_tools/config.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     4063 2024-04-17 16:17:23.000000 silcar_it_tools-0.2.2/src/silcar_it_tools/exe_check.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     2150 2024-04-17 16:10:29.000000 silcar_it_tools-0.2.2/src/silcar_it_tools/packing.py
+-rwxrwxr-x   0 nate      (1000) nate      (1000)     2574 2024-05-09 09:32:40.000000 silcar_it_tools-0.2.2/src/silcar_it_tools/usb_utils.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)      746 2024-04-17 16:16:57.000000 silcar_it_tools-0.2.2/src/silcar_it_tools/utils.py
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-09 09:38:31.997026 silcar_it_tools-0.2.2/src/silcar_it_tools.egg-info/
+-rw-r--r--   0 nate      (1000) nate      (1000)     1266 2024-05-09 09:38:31.000000 silcar_it_tools-0.2.2/src/silcar_it_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 nate      (1000) nate      (1000)      480 2024-05-09 09:38:31.000000 silcar_it_tools-0.2.2/src/silcar_it_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)        1 2024-05-09 09:38:31.000000 silcar_it_tools-0.2.2/src/silcar_it_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)      130 2024-05-09 09:38:31.000000 silcar_it_tools-0.2.2/src/silcar_it_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)        7 2024-05-09 09:38:31.000000 silcar_it_tools-0.2.2/src/silcar_it_tools.egg-info/requires.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)       16 2024-05-09 09:38:31.000000 silcar_it_tools-0.2.2/src/silcar_it_tools.egg-info/top_level.txt
```

### Comparing `silcar_it_tools-0.2.1/LICENSE` & `silcar_it_tools-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `silcar_it_tools-0.2.1/PKG-INFO` & `silcar_it_tools-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silcar_it_tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Basic IT tools used to solve common problems in the Central African Republic.
 Author-email: Nate Marti <nate_marti@sil.org>
 Project-URL: Homepage, https://gitlab.com/acatbadmin/it-tools
 Project-URL: Issues, https://gitlab.com/acatbadmin/it-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `silcar_it_tools-0.2.1/README.md` & `silcar_it_tools-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `silcar_it_tools-0.2.1/pyproject.toml` & `silcar_it_tools-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `silcar_it_tools-0.2.1/src/silcar_it_tools/exe_check.py` & `silcar_it_tools-0.2.2/src/silcar_it_tools/exe_check.py`

 * *Files identical despite different names*

### Comparing `silcar_it_tools-0.2.1/src/silcar_it_tools/packing.py` & `silcar_it_tools-0.2.2/src/silcar_it_tools/packing.py`

 * *Files identical despite different names*

### Comparing `silcar_it_tools-0.2.1/src/silcar_it_tools/usb_utils.py` & `silcar_it_tools-0.2.2/src/silcar_it_tools/usb_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         '*.rar',
         '.~lock.*',
         '~*',
         'FOUND.*',
         'IndexerVolumeGuid',
         'System Volume Information',
     ]
-    srcdir = Path(args.dir[0])
+    srcdir = Path(args.DIR[0])
     outdir = Path.home() / srcdir.name
     if outdir.exists() and next(outdir.iterdir(), None):
         print(f"Folder is not empty: {outdir}")
         ans = input("Continue? [y/N] ")
         if ans.lower() != 'y':
             exit(1)
```

### Comparing `silcar_it_tools-0.2.1/src/silcar_it_tools/utils.py` & `silcar_it_tools-0.2.2/src/silcar_it_tools/utils.py`

 * *Files identical despite different names*

### Comparing `silcar_it_tools-0.2.1/src/silcar_it_tools.egg-info/PKG-INFO` & `silcar_it_tools-0.2.2/src/silcar_it_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silcar_it_tools
-Version: 0.2.1
+Version: 0.2.2
 Summary: Basic IT tools used to solve common problems in the Central African Republic.
 Author-email: Nate Marti <nate_marti@sil.org>
 Project-URL: Homepage, https://gitlab.com/acatbadmin/it-tools
 Project-URL: Issues, https://gitlab.com/acatbadmin/it-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

