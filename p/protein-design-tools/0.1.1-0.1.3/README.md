# Comparing `tmp/protein_design_tools-0.1.1.tar.gz` & `tmp/protein_design_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protein_design_tools-0.1.1.tar", last modified: Tue May  7 22:48:08 2024, max compression
+gzip compressed data, was "protein_design_tools-0.1.3.tar", last modified: Thu May  9 19:31:36 2024, max compression
```

## Comparing `protein_design_tools-0.1.1.tar` & `protein_design_tools-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-07 22:48:08.850143 protein_design_tools-0.1.1/
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1069 2024-05-07 21:38:28.000000 protein_design_tools-0.1.1/LICENSE
--rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1853 2024-05-07 22:48:08.847633 protein_design_tools-0.1.1/PKG-INFO
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      695 2024-05-07 22:40:55.000000 protein_design_tools-0.1.1/README.md
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-07 22:48:08.845980 protein_design_tools-0.1.1/protein_design_tools.egg-info/
--rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1853 2024-05-07 22:48:08.000000 protein_design_tools-0.1.1/protein_design_tools.egg-info/PKG-INFO
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      283 2024-05-07 22:48:08.000000 protein_design_tools-0.1.1/protein_design_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        1 2024-05-07 22:48:08.000000 protein_design_tools-0.1.1/protein_design_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       45 2024-05-07 22:48:08.000000 protein_design_tools-0.1.1/protein_design_tools.egg-info/requires.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        1 2024-05-07 22:48:08.000000 protein_design_tools-0.1.1/protein_design_tools.egg-info/top_level.txt
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       38 2024-05-07 22:48:08.850291 protein_design_tools-0.1.1/setup.cfg
--rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1338 2024-05-07 22:47:53.000000 protein_design_tools-0.1.1/setup.py
-drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-07 22:48:08.837933 protein_design_tools-0.1.1/tests/
--rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1318 2024-05-07 19:58:11.000000 protein_design_tools-0.1.1/tests/test_protein_structure_utils.py
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 19:31:36.872403 protein_design_tools-0.1.3/
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1069 2024-05-07 21:38:28.000000 protein_design_tools-0.1.3/LICENSE
+-rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1748 2024-05-09 19:31:36.868376 protein_design_tools-0.1.3/PKG-INFO
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      695 2024-05-07 22:40:55.000000 protein_design_tools-0.1.3/README.md
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)       38 2024-05-09 19:31:36.872537 protein_design_tools-0.1.3/setup.cfg
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1300 2024-05-09 19:31:01.000000 protein_design_tools-0.1.3/setup.py
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 19:31:36.838446 protein_design_tools-0.1.3/src/
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 19:31:36.865736 protein_design_tools-0.1.3/src/protein_design_tools.egg-info/
+-rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1748 2024-05-09 19:31:36.000000 protein_design_tools-0.1.3/src/protein_design_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)      303 2024-05-09 19:31:36.000000 protein_design_tools-0.1.3/src/protein_design_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        1 2024-05-09 19:31:36.000000 protein_design_tools-0.1.3/src/protein_design_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        6 2024-05-09 19:31:36.000000 protein_design_tools-0.1.3/src/protein_design_tools.egg-info/requires.txt
+-rw-rw-r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)        1 2024-05-09 19:31:36.000000 protein_design_tools-0.1.3/src/protein_design_tools.egg-info/top_level.txt
+drwxrwxr-x   0 schaubaj (755442540) NIH\Domain Users (1360859114)        0 2024-05-09 19:31:36.850263 protein_design_tools-0.1.3/tests/
+-rw-r--r--   0 schaubaj (755442540) NIH\Domain Users (1360859114)     1318 2024-05-07 19:58:11.000000 protein_design_tools-0.1.3/tests/test_protein_structure_utils.py
```

### Comparing `protein_design_tools-0.1.1/LICENSE` & `protein_design_tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `protein_design_tools-0.1.1/PKG-INFO` & `protein_design_tools-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-design-tools
-Version: 0.1.1
+Version: 0.1.3
 Summary: A library of tools for protein design.
 Home-page: https://github.com/drewschaub/protein-design-tools
 Author: Andrew Schaub
 Author-email: andrew.schaub@protonmail.com
 License:  MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -16,21 +16,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Provides-Extra: dev
-Requires-Dist: check-manifest; extra == "dev"
-Provides-Extra: test
-Requires-Dist: coverage; extra == "test"
 
 ![Banner](assets/banner.png)
 
 <br>
 <br>
 
 A library of tools for protein design.
```

### Comparing `protein_design_tools-0.1.1/README.md` & `protein_design_tools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `protein_design_tools-0.1.1/protein_design_tools.egg-info/PKG-INFO` & `protein_design_tools-0.1.3/src/protein_design_tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-design-tools
-Version: 0.1.1
+Version: 0.1.3
 Summary: A library of tools for protein design.
 Home-page: https://github.com/drewschaub/protein-design-tools
 Author: Andrew Schaub
 Author-email: andrew.schaub@protonmail.com
 License:  MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
@@ -16,21 +16,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Provides-Extra: dev
-Requires-Dist: check-manifest; extra == "dev"
-Provides-Extra: test
-Requires-Dist: coverage; extra == "test"
 
 ![Banner](assets/banner.png)
 
 <br>
 <br>
 
 A library of tools for protein design.
```

### Comparing `protein_design_tools-0.1.1/setup.py` & `protein_design_tools-0.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='protein-design-tools',
-    version='0.1.1',
+    version='0.1.3',
     author='Andrew Schaub',
     author_email='andrew.schaub@protonmail.com',
     description='A library of tools for protein design.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/drewschaub/protein-design-tools',
     license=' MIT License',
@@ -22,14 +22,12 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: 3.13',
     ],
-    packages=find_packages(exclude=['tests*']),
+    package_dir = {"": "src"},
+    packages=find_packages(where="src"),
+    python_requires = ">=3.6",
     install_requires=['numpy'],  # List your project dependencies here
-    extras_require={
-        'dev': ['check-manifest'],
-        'test': ['coverage'],
-    },
 )
```

### Comparing `protein_design_tools-0.1.1/tests/test_protein_structure_utils.py` & `protein_design_tools-0.1.3/tests/test_protein_structure_utils.py`

 * *Files identical despite different names*

