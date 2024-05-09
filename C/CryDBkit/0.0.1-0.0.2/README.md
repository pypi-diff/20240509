# Comparing `tmp/CryDBkit-0.0.1.tar.gz` & `tmp/CryDBkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CryDBkit-0.0.1.tar", last modified: Wed May  8 12:18:45 2024, max compression
+gzip compressed data, was "CryDBkit-0.0.2.tar", last modified: Wed May  8 12:23:43 2024, max compression
```

## Comparing `CryDBkit-0.0.1.tar` & `CryDBkit-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-05-08 12:18:45.085421 CryDBkit-0.0.1/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-05-08 12:18:45.084337 CryDBkit-0.0.1/CryDBkit/
--rwxr-xr-x   0 jacob      (501) staff       (20)      295 2024-05-08 12:10:21.000000 CryDBkit-0.0.1/CryDBkit/__init__.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     1850 2024-05-08 12:11:49.000000 CryDBkit-0.0.1/CryDBkit/website.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-05-08 12:18:45.084966 CryDBkit-0.0.1/CryDBkit.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)      792 2024-05-08 12:18:44.000000 CryDBkit-0.0.1/CryDBkit.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      218 2024-05-08 12:18:45.000000 CryDBkit-0.0.1/CryDBkit.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2024-05-08 12:18:44.000000 CryDBkit-0.0.1/CryDBkit.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       42 2024-05-08 12:18:44.000000 CryDBkit-0.0.1/CryDBkit.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        9 2024-05-08 12:18:44.000000 CryDBkit-0.0.1/CryDBkit.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)      792 2024-05-08 12:18:45.085202 CryDBkit-0.0.1/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      132 2024-05-08 12:13:42.000000 CryDBkit-0.0.1/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2024-05-08 12:18:45.085468 CryDBkit-0.0.1/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1014 2024-05-08 12:18:42.000000 CryDBkit-0.0.1/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-05-08 12:23:43.343243 CryDBkit-0.0.2/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-05-08 12:23:43.342160 CryDBkit-0.0.2/CryDBkit/
+-rwxr-xr-x   0 jacob      (501) staff       (20)      295 2024-05-08 12:10:21.000000 CryDBkit-0.0.2/CryDBkit/__init__.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     1850 2024-05-08 12:11:49.000000 CryDBkit-0.0.2/CryDBkit/website.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-05-08 12:23:43.342786 CryDBkit-0.0.2/CryDBkit.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)      714 2024-05-08 12:23:43.000000 CryDBkit-0.0.2/CryDBkit.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      218 2024-05-08 12:23:43.000000 CryDBkit-0.0.2/CryDBkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2024-05-08 12:23:43.000000 CryDBkit-0.0.2/CryDBkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        9 2024-05-08 12:23:43.000000 CryDBkit-0.0.2/CryDBkit.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        9 2024-05-08 12:23:43.000000 CryDBkit-0.0.2/CryDBkit.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)      714 2024-05-08 12:23:43.343017 CryDBkit-0.0.2/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      132 2024-05-08 12:13:42.000000 CryDBkit-0.0.2/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2024-05-08 12:23:43.343290 CryDBkit-0.0.2/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)      973 2024-05-08 12:23:37.000000 CryDBkit-0.0.2/setup.py
```

### Comparing `CryDBkit-0.0.1/CryDBkit/website.py` & `CryDBkit-0.0.2/CryDBkit/website.py`

 * *Files identical despite different names*

### Comparing `CryDBkit-0.0.1/CryDBkit.egg-info/PKG-INFO` & `CryDBkit-0.0.2/CryDBkit.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: CryDBkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: ToolKit for building your own Crystal Database
 Home-page: https://github.com/WPEM
 Author: CaoBin
 Author-email: binjacobcao@gmail.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
-Requires-Dist: subprocess
-Requires-Dist: zipfile
 Requires-Dist: wget
-Requires-Dist: pkg_resources
 Requires-Dist: ase
 
 ToolKit for building your own Crystal Database. 
 For assistance, please contact me at binjacobcao@gmail.com. Cao Bin, HKUST, China."
```

### Comparing `CryDBkit-0.0.1/PKG-INFO` & `CryDBkit-0.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: CryDBkit
-Version: 0.0.1
+Version: 0.0.2
 Summary: ToolKit for building your own Crystal Database
 Home-page: https://github.com/WPEM
 Author: CaoBin
 Author-email: binjacobcao@gmail.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.5
-Requires-Dist: subprocess
-Requires-Dist: zipfile
 Requires-Dist: wget
-Requires-Dist: pkg_resources
 Requires-Dist: ase
 
 ToolKit for building your own Crystal Database. 
 For assistance, please contact me at binjacobcao@gmail.com. Cao Bin, HKUST, China."
```

### Comparing `CryDBkit-0.0.1/setup.py` & `CryDBkit-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CryDBkit',
-    version='0.0.1',
+    version='0.0.2',
     description="ToolKit for building your own Crystal Database",
     long_description=open('README.md', encoding='utf-8').read(),
     include_package_data=True,
     author='CaoBin',
     author_email='binjacobcao@gmail.com',
     maintainer='CaoBin',
     maintainer_email='binjacobcao@gmail.com',
@@ -17,14 +17,14 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
     python_requires='>=3.5',
-    install_requires=['subprocess', 'zipfile', 'wget', 'pkg_resources', 'ase',],
+    install_requires=[ 'wget', 'ase',],
     entry_points={
         'console_scripts': [
             '',
         ],
     },
 )
```

