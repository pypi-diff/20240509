# Comparing `tmp/flort-0.1.5.tar.gz` & `tmp/flort-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flort-0.1.5.tar", last modified: Thu Apr  4 14:44:07 2024, max compression
+gzip compressed data, was "flort-0.1.6.tar", last modified: Thu May  9 20:36:34 2024, max compression
```

## Comparing `flort-0.1.5.tar` & `flort-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 14:44:07.093076 flort-0.1.5/
--rw-r--r--   0 nd        (1000) nd        (1000)     1500 2024-04-04 14:04:22.000000 flort-0.1.5/LICENSE
--rw-r--r--   0 nd        (1000) nd        (1000)     1716 2024-04-04 14:44:07.092076 flort-0.1.5/PKG-INFO
--rw-r--r--   0 nd        (1000) nd        (1000)     1264 2024-04-04 14:43:55.000000 flort-0.1.5/README.md
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 14:44:07.092076 flort-0.1.5/flort/
--rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-04-04 12:51:02.000000 flort-0.1.5/flort/__init__.py
--rw-r--r--   0 nd        (1000) nd        (1000)       60 2024-04-04 12:51:31.000000 flort-0.1.5/flort/__main__.py
--rw-r--r--   0 nd        (1000) nd        (1000)     4136 2024-04-04 14:41:31.000000 flort-0.1.5/flort/cli.py
-drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-04-04 14:44:07.092076 flort-0.1.5/flort.egg-info/
--rw-r--r--   0 nd        (1000) nd        (1000)     1716 2024-04-04 14:44:06.000000 flort-0.1.5/flort.egg-info/PKG-INFO
--rw-r--r--   0 nd        (1000) nd        (1000)      223 2024-04-04 14:44:07.000000 flort-0.1.5/flort.egg-info/SOURCES.txt
--rw-r--r--   0 nd        (1000) nd        (1000)        1 2024-04-04 14:44:06.000000 flort-0.1.5/flort.egg-info/dependency_links.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       46 2024-04-04 14:44:06.000000 flort-0.1.5/flort.egg-info/entry_points.txt
--rw-r--r--   0 nd        (1000) nd        (1000)        6 2024-04-04 14:44:07.000000 flort-0.1.5/flort.egg-info/top_level.txt
--rw-r--r--   0 nd        (1000) nd        (1000)       38 2024-04-04 14:44:07.093076 flort-0.1.5/setup.cfg
--rw-r--r--   0 nd        (1000) nd        (1000)      778 2024-04-04 14:44:04.000000 flort-0.1.5/setup.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-09 20:36:34.169705 flort-0.1.6/
+-rw-r--r--   0 nd        (1000) nd        (1000)     1500 2024-04-04 14:04:22.000000 flort-0.1.6/LICENSE
+-rw-r--r--   0 nd        (1000) nd        (1000)     1716 2024-05-09 20:36:34.169705 flort-0.1.6/PKG-INFO
+-rw-r--r--   0 nd        (1000) nd        (1000)     1264 2024-04-04 14:43:55.000000 flort-0.1.6/README.md
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-09 20:36:34.169705 flort-0.1.6/flort/
+-rw-r--r--   0 nd        (1000) nd        (1000)        0 2024-04-04 12:51:02.000000 flort-0.1.6/flort/__init__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)       60 2024-04-04 12:51:31.000000 flort-0.1.6/flort/__main__.py
+-rw-r--r--   0 nd        (1000) nd        (1000)     4268 2024-05-09 20:35:43.000000 flort-0.1.6/flort/cli.py
+drwxr-xr-x   0 nd        (1000) nd        (1000)        0 2024-05-09 20:36:34.169705 flort-0.1.6/flort.egg-info/
+-rw-r--r--   0 nd        (1000) nd        (1000)     1716 2024-05-09 20:36:33.000000 flort-0.1.6/flort.egg-info/PKG-INFO
+-rw-r--r--   0 nd        (1000) nd        (1000)      223 2024-05-09 20:36:34.000000 flort-0.1.6/flort.egg-info/SOURCES.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)        1 2024-05-09 20:36:33.000000 flort-0.1.6/flort.egg-info/dependency_links.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       46 2024-05-09 20:36:33.000000 flort-0.1.6/flort.egg-info/entry_points.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)        6 2024-05-09 20:36:34.000000 flort-0.1.6/flort.egg-info/top_level.txt
+-rw-r--r--   0 nd        (1000) nd        (1000)       38 2024-05-09 20:36:34.169705 flort-0.1.6/setup.cfg
+-rw-r--r--   0 nd        (1000) nd        (1000)      778 2024-05-09 20:35:56.000000 flort-0.1.6/setup.py
```

### Comparing `flort-0.1.5/LICENSE` & `flort-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flort-0.1.5/PKG-INFO` & `flort-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flort
-Version: 0.1.5
+Version: 0.1.6
 Summary: A utilty to flatten your source code directory into a single file for LLM usage
 Home-page: https://github.com/chris17453/flort
 Author: Chris Watkins
 Author-email: chris@watkinslabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `flort-0.1.5/README.md` & `flort-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `flort-0.1.5/flort/cli.py` & `flort-0.1.6/flort/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     parser.add_argument('--compress', default=False, action='store_true', help='Compress the listed files by removing whitespace.')
     parser.add_argument('--output', type=str, default="stdio", help='Output file path. Defaults to stdout if not specified.')
     parser.add_argument('--php', action='store_true', help='Include PHP files.')
     parser.add_argument('--js', action='store_true', help='Include JavaScript files.')
     parser.add_argument('--py', action='store_true', help='Include Python files.')
     parser.add_argument('--c', action='store_true', help='Include C files.')
     parser.add_argument('--cpp', action='store_true', help='Include C++ files.')    
+    parser.add_argument('--sh', action='store_true', help='Include sh files.')    
     parser.add_argument('--no-tree', action='store_true', help='Dont print the tree at the beginning.')    
     args = parser.parse_args()
     
     extensions = []
     output = []
     if args.php:
         extensions.append('.php')
@@ -86,14 +87,16 @@
         extensions.append('.py')
     if args.c:
         extensions.append('.c')
         extensions.append('.h')
     if args.cpp:
         extensions.append('.cpp')
         extensions.append('.h')
+    if args.sh:
+        extensions.append('.sh')
     if args.no_tree != True:
         output.append(generate_tree(args.dir))
     
     output.append(list_files(args.dir, compress=args.compress, extensions=extensions))
 
     if args.output != "stdio":    
         write_file(args.output, "\n".join(output))
```

### Comparing `flort-0.1.5/flort.egg-info/PKG-INFO` & `flort-0.1.6/flort.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flort
-Version: 0.1.5
+Version: 0.1.6
 Summary: A utilty to flatten your source code directory into a single file for LLM usage
 Home-page: https://github.com/chris17453/flort
 Author: Chris Watkins
 Author-email: chris@watkinslabs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `flort-0.1.5/setup.py` & `flort-0.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flort',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'flort = flort.__main__:main'
         ]
     },
     install_requires=[
```

