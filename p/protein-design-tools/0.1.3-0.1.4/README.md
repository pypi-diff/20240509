# Comparing `tmp/protein_design_tools-0.1.3.tar.gz` & `tmp/protein_design_tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protein_design_tools-0.1.3.tar", last modified: Thu May  9 19:31:36 2024, max compression
+gzip compressed data, was "protein_design_tools-0.1.4.tar", last modified: Thu May  9 19:45:41 2024, max compression
```

## Comparing `protein_design_tools-0.1.3.tar` & `protein_design_tools-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 19:31:36.872403 protein_design_tools-0.1.3/
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1069 2024-05-07 21:38:28.000000 protein_design_tools-0.1.3/LICENSE
--rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1748 2024-05-09 19:31:36.868376 protein_design_tools-0.1.3/PKG-INFO
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      695 2024-05-07 22:40:55.000000 protein_design_tools-0.1.3/README.md
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       38 2024-05-09 19:31:36.872537 protein_design_tools-0.1.3/setup.cfg
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1300 2024-05-09 19:31:01.000000 protein_design_tools-0.1.3/setup.py
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 19:31:36.838446 protein_design_tools-0.1.3/src/
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 19:31:36.865736 protein_design_tools-0.1.3/src/protein_design_tools.egg-info/
--rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1748 2024-05-09 19:31:36.000000 protein_design_tools-0.1.3/src/protein_design_tools.egg-info/PKG-INFO
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      303 2024-05-09 19:31:36.000000 protein_design_tools-0.1.3/src/protein_design_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        1 2024-05-09 19:31:36.000000 protein_design_tools-0.1.3/src/protein_design_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        6 2024-05-09 19:31:36.000000 protein_design_tools-0.1.3/src/protein_design_tools.egg-info/requires.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        1 2024-05-09 19:31:36.000000 protein_design_tools-0.1.3/src/protein_design_tools.egg-info/top_level.txt
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 19:31:36.850263 protein_design_tools-0.1.3/tests/
--rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1318 2024-05-07 19:58:11.000000 protein_design_tools-0.1.3/tests/test_protein_structure_utils.py
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 19:45:41.085378 protein_design_tools-0.1.4/
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1069 2024-05-07 21:38:28.000000 protein_design_tools-0.1.4/LICENSE
+-rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1304 2024-05-09 19:45:41.084616 protein_design_tools-0.1.4/PKG-INFO
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      695 2024-05-07 22:40:55.000000 protein_design_tools-0.1.4/README.md
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 19:45:41.070378 protein_design_tools-0.1.4/protein_design_tools/
+-rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     7546 2024-05-09 19:30:56.000000 protein_design_tools-0.1.4/protein_design_tools/protein_structure.py
+-rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)    19107 2024-05-09 19:30:50.000000 protein_design_tools-0.1.4/protein_design_tools/protein_structure_utils.py
+-rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1856 2024-05-07 22:03:29.000000 protein_design_tools-0.1.4/protein_design_tools/test.py
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 19:45:41.083985 protein_design_tools-0.1.4/protein_design_tools.egg-info/
+-rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1304 2024-05-09 19:45:40.000000 protein_design_tools-0.1.4/protein_design_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      402 2024-05-09 19:45:40.000000 protein_design_tools-0.1.4/protein_design_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        1 2024-05-09 19:45:40.000000 protein_design_tools-0.1.4/protein_design_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        6 2024-05-09 19:45:40.000000 protein_design_tools-0.1.4/protein_design_tools.egg-info/requires.txt
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       21 2024-05-09 19:45:40.000000 protein_design_tools-0.1.4/protein_design_tools.egg-info/top_level.txt
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       38 2024-05-09 19:45:41.085543 protein_design_tools-0.1.4/setup.cfg
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      898 2024-05-09 19:45:38.000000 protein_design_tools-0.1.4/setup.py
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 19:45:41.079821 protein_design_tools-0.1.4/tests/
+-rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1318 2024-05-07 19:58:11.000000 protein_design_tools-0.1.4/tests/test_protein_structure_utils.py
```

### Comparing `protein_design_tools-0.1.3/LICENSE` & `protein_design_tools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `protein_design_tools-0.1.3/README.md` & `protein_design_tools-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `protein_design_tools-0.1.3/tests/test_protein_structure_utils.py` & `protein_design_tools-0.1.4/tests/test_protein_structure_utils.py`

 * *Files identical despite different names*

