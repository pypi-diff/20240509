# Comparing `tmp/plastics-0.1.0.tar.gz` & `tmp/plastics-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plastics-0.1.0.tar", last modified: Thu May  9 00:53:21 2024, max compression
+gzip compressed data, was "plastics-0.1.1.tar", last modified: Thu May  9 01:09:03 2024, max compression
```

## Comparing `plastics-0.1.0.tar` & `plastics-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 00:53:21.090970 plastics-0.1.0/
--rw-rw-rw-   0        0        0     1082 2024-05-08 03:02:34.000000 plastics-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2336 2024-05-09 00:53:21.090970 plastics-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1435 2024-05-08 15:48:34.000000 plastics-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-09 00:53:21.063608 plastics-0.1.0/plastics/
--rw-rw-rw-   0        0        0       92 2023-09-22 17:17:37.000000 plastics-0.1.0/plastics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 00:53:21.089912 plastics-0.1.0/plastics.egg-info/
--rw-rw-rw-   0        0        0     2336 2024-05-09 00:53:20.000000 plastics-0.1.0/plastics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-05-09 00:53:20.000000 plastics-0.1.0/plastics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 00:53:20.000000 plastics-0.1.0/plastics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-09 00:53:20.000000 plastics-0.1.0/plastics.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 00:53:20.000000 plastics-0.1.0/plastics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 00:53:21.092350 plastics-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1578 2024-05-08 15:27:10.000000 plastics-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 01:09:03.395832 plastics-0.1.1/
+-rw-rw-rw-   0        0        0     1082 2024-05-08 03:02:34.000000 plastics-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2336 2024-05-09 01:09:03.395832 plastics-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1435 2024-05-08 15:48:34.000000 plastics-0.1.1/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-09 01:09:03.332414 plastics-0.1.1/plastics/
+-rw-rw-rw-   0        0        0       92 2023-09-22 17:17:37.000000 plastics-0.1.1/plastics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 01:09:03.395832 plastics-0.1.1/plastics/strap/
+-rw-rw-rw-   0        0        0      790 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/__init__.py
+-rw-rw-rw-   0        0        0     2380 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/dissolution_steps.py
+-rw-rw-rw-   0        0        0     2904 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/precipitation_steps.py
+-rw-rw-rw-   0        0        0     9553 2024-05-08 16:59:06.000000 plastics-0.1.1/plastics/strap/process_model.py
+-rw-rw-rw-   0        0        0     1410 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/process_settings.py
+-rw-rw-rw-   0        0        0     1688 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/property_package.py
+-rw-rw-rw-   0        0        0    17156 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/simulation.py
+-rw-rw-rw-   0        0        0    19328 2024-05-08 17:16:43.000000 plastics-0.1.1/plastics/strap/systems.py
+-rw-rw-rw-   0        0        0    12304 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/tea.py
+-rw-rw-rw-   0        0        0    18667 2024-05-08 13:43:02.000000 plastics-0.1.1/plastics/strap/units.py
+drwxrwxrwx   0        0        0        0 2024-05-09 01:09:03.364043 plastics-0.1.1/plastics.egg-info/
+-rw-rw-rw-   0        0        0     2336 2024-05-09 01:09:03.000000 plastics-0.1.1/plastics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      511 2024-05-09 01:09:03.000000 plastics-0.1.1/plastics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 01:09:03.000000 plastics-0.1.1/plastics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-09 01:09:03.000000 plastics-0.1.1/plastics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 01:09:03.000000 plastics-0.1.1/plastics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 01:09:03.395832 plastics-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1543 2024-05-09 01:08:20.000000 plastics-0.1.1/setup.py
```

### Comparing `plastics-0.1.0/LICENSE` & `plastics-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plastics-0.1.0/PKG-INFO` & `plastics-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plastics
-Version: 0.1.0
+Version: 0.1.1
 Summary: Plastic processing models in BioSTEAM
 Home-page: https://github.com/yoelcortes/plastics
 Download-URL: https://github.com/yoelcortes/plastics
 Author: Yoel Cortes-Pena
 Author-email: yoelcortes@gmail.com
 License: MIT
 Keywords: chemical process simulation plastic bioprocess engineering STRAP solvent targeted dissolution precipitation
```

### Comparing `plastics-0.1.0/README.rst` & `plastics-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `plastics-0.1.0/plastics.egg-info/PKG-INFO` & `plastics-0.1.1/plastics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plastics
-Version: 0.1.0
+Version: 0.1.1
 Summary: Plastic processing models in BioSTEAM
 Home-page: https://github.com/yoelcortes/plastics
 Download-URL: https://github.com/yoelcortes/plastics
 Author: Yoel Cortes-Pena
 Author-email: yoelcortes@gmail.com
 License: MIT
 Keywords: chemical process simulation plastic bioprocess engineering STRAP solvent targeted dissolution precipitation
```

### Comparing `plastics-0.1.0/setup.py` & `plastics-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 # for license details.
 from setuptools import setup
 
 setup(
     name='plastics',
     packages=['plastics'],
     license='MIT',
-    version='0.1.0',
+    version='0.1.1',
     description="Plastic processing models in BioSTEAM",
     long_description=open('README.rst', encoding='utf-8').read(),
     author='Yoel Cortes-Pena',
     install_requires=['biosteam>=2.44.0,<2.45.0'],
     python_requires=">=3.9",
     package_data={
         'plastics': [
-            'plastics/*',
-            'plastics/strap/*'
+            'strap/*',
         ]
     },
     platforms=['Windows', 'Mac', 'Linux'],
     author_email='yoelcortes@gmail.com',
     url='https://github.com/yoelcortes/plastics',
     download_url='https://github.com/yoelcortes/plastics',
     classifiers=['Development Status :: 3 - Alpha',
```

