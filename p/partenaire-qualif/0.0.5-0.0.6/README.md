# Comparing `tmp/partenaire-qualif-0.0.5.tar.gz` & `tmp/partenaire-qualif-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partenaire-qualif-0.0.5.tar", last modified: Thu May  9 04:41:15 2024, max compression
+gzip compressed data, was "partenaire-qualif-0.0.6.tar", last modified: Thu May  9 04:44:37 2024, max compression
```

## Comparing `partenaire-qualif-0.0.5.tar` & `partenaire-qualif-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 04:41:15.638443 partenaire-qualif-0.0.5/
--rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3256 2024-05-09 04:41:15.638443 partenaire-qualif-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2733 2024-05-09 03:25:03.000000 partenaire-qualif-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 04:41:15.634363 partenaire-qualif-0.0.5/partenaire_qualif.egg-info/
--rw-rw-rw-   0        0        0     3256 2024-05-09 04:41:15.000000 partenaire-qualif-0.0.5/partenaire_qualif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-05-09 04:41:15.000000 partenaire-qualif-0.0.5/partenaire_qualif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 04:41:15.000000 partenaire-qualif-0.0.5/partenaire_qualif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-09 04:41:15.000000 partenaire-qualif-0.0.5/partenaire_qualif.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-09 04:41:15.000000 partenaire-qualif-0.0.5/partenaire_qualif.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 04:41:15.636446 partenaire-qualif-0.0.5/qualif/
--rw-rw-rw-   0        0        0      101 2024-05-09 04:06:13.000000 partenaire-qualif-0.0.5/qualif/__init__.py
--rw-rw-rw-   0        0        0     7992 2024-05-09 04:32:27.000000 partenaire-qualif-0.0.5/qualif/qualif.py
--rw-rw-rw-   0        0        0       42 2024-05-09 04:41:15.639415 partenaire-qualif-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      911 2024-05-09 04:38:46.000000 partenaire-qualif-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 04:44:37.056261 partenaire-qualif-0.0.6/
+-rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3256 2024-05-09 04:44:37.056261 partenaire-qualif-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2733 2024-05-09 03:25:03.000000 partenaire-qualif-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 04:44:37.024940 partenaire-qualif-0.0.6/partenaire_qualif.egg-info/
+-rw-rw-rw-   0        0        0     3256 2024-05-09 04:44:36.000000 partenaire-qualif-0.0.6/partenaire_qualif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-05-09 04:44:36.000000 partenaire-qualif-0.0.6/partenaire_qualif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 04:44:36.000000 partenaire-qualif-0.0.6/partenaire_qualif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-09 04:44:36.000000 partenaire-qualif-0.0.6/partenaire_qualif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-09 04:44:36.000000 partenaire-qualif-0.0.6/partenaire_qualif.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 04:44:37.056261 partenaire-qualif-0.0.6/qualif/
+-rw-rw-rw-   0        0        0      101 2024-05-09 04:06:13.000000 partenaire-qualif-0.0.6/qualif/__init__.py
+-rw-rw-rw-   0        0        0     7992 2024-05-09 04:32:27.000000 partenaire-qualif-0.0.6/qualif/qualif.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 04:44:37.056261 partenaire-qualif-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      911 2024-05-09 04:44:30.000000 partenaire-qualif-0.0.6/setup.py
```

### Comparing `partenaire-qualif-0.0.5/LICENSE` & `partenaire-qualif-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.5/PKG-INFO` & `partenaire-qualif-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire-qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `partenaire-qualif-0.0.5/README.md` & `partenaire-qualif-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.5/partenaire_qualif.egg-info/PKG-INFO` & `partenaire-qualif-0.0.6/partenaire_qualif.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.0.5
+Version: 0.0.6
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire-qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `partenaire-qualif-0.0.5/qualif/qualif.py` & `partenaire-qualif-0.0.6/qualif/qualif.py`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.5/setup.py` & `partenaire-qualif-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="partenaire-qualif",
-    version="0.0.5",
+    version="0.0.6",
     author="Yanchao MURONG",
     author_email="yanchao.murong@gmail.com",
     description="A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ymurong/partenaire-qualif.git",
     packages=setuptools.find_packages(),
```

