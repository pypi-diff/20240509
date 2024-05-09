# Comparing `tmp/converttentotwenty-3.0.1.tar.gz` & `tmp/converttentotwenty-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "converttentotwenty-3.0.1.tar", last modified: Wed Apr 24 11:09:39 2024, max compression
+gzip compressed data, was "converttentotwenty-3.1.1.tar", last modified: Thu May  9 15:49:34 2024, max compression
```

## Comparing `converttentotwenty-3.0.1.tar` & `converttentotwenty-3.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 11:09:39.668000 converttentotwenty-3.0.1/
--rw-rw-rw-   0        0        0     2415 2024-04-24 11:09:39.663000 converttentotwenty-3.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1961 2024-04-24 11:04:44.000000 converttentotwenty-3.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-24 11:09:39.625000 converttentotwenty-3.0.1/converttentotwenty/
--rw-rw-rw-   0        0        0       42 2024-03-13 15:38:18.000000 converttentotwenty-3.0.1/converttentotwenty/__init__.py
--rw-rw-rw-   0        0        0     1231 2024-04-24 10:59:51.000000 converttentotwenty-3.0.1/converttentotwenty/converttentotwenty.py
-drwxrwxrwx   0        0        0        0 2024-04-24 11:09:39.658000 converttentotwenty-3.0.1/converttentotwenty.egg-info/
--rw-rw-rw-   0        0        0     2415 2024-04-24 11:09:39.000000 converttentotwenty-3.0.1/converttentotwenty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-04-24 11:09:39.000000 converttentotwenty-3.0.1/converttentotwenty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 11:09:39.000000 converttentotwenty-3.0.1/converttentotwenty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-04-24 11:09:39.000000 converttentotwenty-3.0.1/converttentotwenty.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 11:09:39.667000 converttentotwenty-3.0.1/setup.cfg
--rw-rw-rw-   0        0        0      672 2024-04-24 11:08:29.000000 converttentotwenty-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 15:49:34.186000 converttentotwenty-3.1.1/
+-rw-rw-rw-   0        0        0     2415 2024-05-09 15:49:34.180000 converttentotwenty-3.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1961 2024-04-24 11:04:44.000000 converttentotwenty-3.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 15:49:34.134000 converttentotwenty-3.1.1/converttentotwenty/
+-rw-rw-rw-   0        0        0       42 2024-03-13 15:38:18.000000 converttentotwenty-3.1.1/converttentotwenty/__init__.py
+-rw-rw-rw-   0        0        0     1505 2024-05-09 15:48:45.000000 converttentotwenty-3.1.1/converttentotwenty/converttentotwenty.py
+drwxrwxrwx   0        0        0        0 2024-05-09 15:49:34.174000 converttentotwenty-3.1.1/converttentotwenty.egg-info/
+-rw-rw-rw-   0        0        0     2415 2024-05-09 15:49:33.000000 converttentotwenty-3.1.1/converttentotwenty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-09 15:49:33.000000 converttentotwenty-3.1.1/converttentotwenty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 15:49:33.000000 converttentotwenty-3.1.1/converttentotwenty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-09 15:49:33.000000 converttentotwenty-3.1.1/converttentotwenty.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 15:49:34.184000 converttentotwenty-3.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      672 2024-05-09 15:48:56.000000 converttentotwenty-3.1.1/setup.py
```

### Comparing `converttentotwenty-3.0.1/PKG-INFO` & `converttentotwenty-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: converttentotwenty
-Version: 3.0.1
+Version: 3.1.1
 Summary: Ma bibliothèque Python
 Home-page: https://github.com/Joris-ROBIN/Converttentotwenty.git
 Author: Skairipa
 Author-email: jorisrobin34@gmail.com
 License: MEEF
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `converttentotwenty-3.0.1/README.md` & `converttentotwenty-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `converttentotwenty-3.0.1/converttentotwenty/converttentotwenty.py` & `converttentotwenty-3.1.1/converttentotwenty/converttentotwenty.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,19 @@
     >>> traduction([4, 0, 16])
     ['4', '0', 'g']
     >>> traduction([5, 1, 4])
     ['5', '1', '4']
     >>> traduction([11, 16])
     ['b', 'g']
     """
+    assert type(message) == list, "traduction() attend une liste en argument"
+    for i in message:
+        assert type(i) == int, "La liste ne doit contenir que des entiers"
+        assert i >= 0 and i <= 19, "Les entiers doivent être compris entre 0\
+et 19 compris"
     base20='0123456789abcdefghij'
     res = []
     for i in message:
         res.append(base20[i])
     return res
```

### Comparing `converttentotwenty-3.0.1/converttentotwenty.egg-info/PKG-INFO` & `converttentotwenty-3.1.1/converttentotwenty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: converttentotwenty
-Version: 3.0.1
+Version: 3.1.1
 Summary: Ma bibliothèque Python
 Home-page: https://github.com/Joris-ROBIN/Converttentotwenty.git
 Author: Skairipa
 Author-email: jorisrobin34@gmail.com
 License: MEEF
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `converttentotwenty-3.0.1/setup.py` & `converttentotwenty-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="converttentotwenty",
-    version="3.0.1",
+    version="3.1.1",
     description="Ma bibliothèque Python",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Joris-ROBIN/Converttentotwenty.git",
     author="Skairipa",
     author_email="jorisrobin34@gmail.com",
     license="MEEF",
```

