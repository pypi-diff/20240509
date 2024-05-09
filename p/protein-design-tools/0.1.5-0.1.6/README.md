# Comparing `tmp/protein-design-tools-0.1.5.tar.gz` & `tmp/protein_design_tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protein-design-tools-0.1.5.tar", last modified: Thu May  9 20:12:05 2024, max compression
+gzip compressed data, was "protein_design_tools-0.1.6.tar", last modified: Thu May  9 20:52:39 2024, max compression
```

## Comparing `protein-design-tools-0.1.5.tar` & `protein_design_tools-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 20:12:05.402870 protein-design-tools-0.1.5/
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1069 2024-05-07 21:38:28.000000 protein-design-tools-0.1.5/LICENSE
--rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1304 2024-05-09 20:12:05.398728 protein-design-tools-0.1.5/PKG-INFO
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      695 2024-05-07 22:40:55.000000 protein-design-tools-0.1.5/README.md
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 20:12:05.388730 protein-design-tools-0.1.5/protein_design_tools/
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      255 2024-05-09 20:03:09.000000 protein-design-tools-0.1.5/protein_design_tools/__init__.py
--rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     7078 2024-05-09 20:00:56.000000 protein-design-tools-0.1.5/protein_design_tools/protein_structure.py
--rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)    18909 2024-05-09 20:03:36.000000 protein-design-tools-0.1.5/protein_design_tools/protein_structure_utils.py
--rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1856 2024-05-07 22:03:29.000000 protein-design-tools-0.1.5/protein_design_tools/test.py
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 20:12:05.397763 protein-design-tools-0.1.5/protein_design_tools.egg-info/
--rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1304 2024-05-09 20:12:05.000000 protein-design-tools-0.1.5/protein_design_tools.egg-info/PKG-INFO
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      435 2024-05-09 20:12:05.000000 protein-design-tools-0.1.5/protein_design_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        1 2024-05-09 20:12:05.000000 protein-design-tools-0.1.5/protein_design_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        6 2024-05-09 20:12:05.000000 protein-design-tools-0.1.5/protein_design_tools.egg-info/requires.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       21 2024-05-09 20:12:05.000000 protein-design-tools-0.1.5/protein_design_tools.egg-info/top_level.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       38 2024-05-09 20:12:05.402948 protein-design-tools-0.1.5/setup.cfg
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      898 2024-05-09 20:03:43.000000 protein-design-tools-0.1.5/setup.py
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 20:12:05.398223 protein-design-tools-0.1.5/tests/
--rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1318 2024-05-07 19:58:11.000000 protein-design-tools-0.1.5/tests/test_protein_structure_utils.py
+drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:52:39.923861 protein_design_tools-0.1.6/
+-rw-rw-r--   0 schaubaj (755442540) 1360859114     1069 2024-05-07 21:38:28.000000 protein_design_tools-0.1.6/LICENSE
+-rw-r--r--   0 schaubaj (755442540) 1360859114     1304 2024-05-09 20:52:39.921373 protein_design_tools-0.1.6/PKG-INFO
+-rw-rw-r--   0 schaubaj (755442540) 1360859114      695 2024-05-07 22:40:55.000000 protein_design_tools-0.1.6/README.md
+drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:52:39.903906 protein_design_tools-0.1.6/protein_design_tools/
+-rw-rw-r--   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:51:26.000000 protein_design_tools-0.1.6/protein_design_tools/__init__.py
+-rw-r--r--   0 schaubaj (755442540) 1360859114     7078 2024-05-09 20:00:56.000000 protein_design_tools-0.1.6/protein_design_tools/protein_structure.py
+-rw-r--r--   0 schaubaj (755442540) 1360859114    18909 2024-05-09 20:03:36.000000 protein_design_tools-0.1.6/protein_design_tools/protein_structure_utils.py
+-rw-r--r--   0 schaubaj (755442540) 1360859114     1856 2024-05-07 22:03:29.000000 protein_design_tools-0.1.6/protein_design_tools/test.py
+drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:52:39.918878 protein_design_tools-0.1.6/protein_design_tools.egg-info/
+-rw-r--r--   0 schaubaj (755442540) 1360859114     1304 2024-05-09 20:52:39.000000 protein_design_tools-0.1.6/protein_design_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 schaubaj (755442540) 1360859114      435 2024-05-09 20:52:39.000000 protein_design_tools-0.1.6/protein_design_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 schaubaj (755442540) 1360859114        1 2024-05-09 20:52:39.000000 protein_design_tools-0.1.6/protein_design_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 schaubaj (755442540) 1360859114        6 2024-05-09 20:52:39.000000 protein_design_tools-0.1.6/protein_design_tools.egg-info/requires.txt
+-rw-rw-r--   0 schaubaj (755442540) 1360859114       21 2024-05-09 20:52:39.000000 protein_design_tools-0.1.6/protein_design_tools.egg-info/top_level.txt
+-rw-rw-r--   0 schaubaj (755442540) 1360859114       38 2024-05-09 20:52:39.923948 protein_design_tools-0.1.6/setup.cfg
+-rw-rw-r--   0 schaubaj (755442540) 1360859114      899 2024-05-09 20:52:19.000000 protein_design_tools-0.1.6/setup.py
+drwxrwxr-x   0 schaubaj (755442540) 1360859114        0 2024-05-09 20:52:39.916884 protein_design_tools-0.1.6/tests/
+-rw-r--r--   0 schaubaj (755442540) 1360859114     1318 2024-05-07 19:58:11.000000 protein_design_tools-0.1.6/tests/test_protein_structure_utils.py
```

### Comparing `protein-design-tools-0.1.5/LICENSE` & `protein_design_tools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `protein-design-tools-0.1.5/PKG-INFO` & `protein_design_tools-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-design-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library of tools for protein design.
 Home-page: https://github.com/drewschaub/protein-design-tools
 Author: Andrew Schaub
 Author-email: andrew.schaub@protonmail.com
 License:  MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `protein-design-tools-0.1.5/README.md` & `protein_design_tools-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `protein-design-tools-0.1.5/protein_design_tools/protein_structure.py` & `protein_design_tools-0.1.6/protein_design_tools/protein_structure.py`

 * *Files identical despite different names*

### Comparing `protein-design-tools-0.1.5/protein_design_tools/protein_structure_utils.py` & `protein_design_tools-0.1.6/protein_design_tools/protein_structure_utils.py`

 * *Files identical despite different names*

### Comparing `protein-design-tools-0.1.5/protein_design_tools/test.py` & `protein_design_tools-0.1.6/protein_design_tools/test.py`

 * *Files identical despite different names*

### Comparing `protein-design-tools-0.1.5/protein_design_tools.egg-info/PKG-INFO` & `protein_design_tools-0.1.6/protein_design_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-design-tools
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library of tools for protein design.
 Home-page: https://github.com/drewschaub/protein-design-tools
 Author: Andrew Schaub
 Author-email: andrew.schaub@protonmail.com
 License:  MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `protein-design-tools-0.1.5/setup.py` & `protein_design_tools-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='protein-design-tools',
-    version='0.1.5',
+    version='0.1.6',
     author='Andrew Schaub',
     author_email='andrew.schaub@protonmail.com',
     description='A library of tools for protein design.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/drewschaub/protein-design-tools',
     license=' MIT License',
@@ -17,8 +17,8 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
     packages=['protein_design_tools'],
     package_dir={'protein_design_tools': 'protein_design_tools'},
     python_requires = ">=3.6",
     install_requires=['numpy'],  # List your project dependencies here
-)
+)
```

### Comparing `protein-design-tools-0.1.5/tests/test_protein_structure_utils.py` & `protein_design_tools-0.1.6/tests/test_protein_structure_utils.py`

 * *Files identical despite different names*

