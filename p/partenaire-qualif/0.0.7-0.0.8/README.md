# Comparing `tmp/partenaire-qualif-0.0.7.tar.gz` & `tmp/partenaire-qualif-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partenaire-qualif-0.0.7.tar", last modified: Thu May  9 04:51:58 2024, max compression
+gzip compressed data, was "partenaire-qualif-0.0.8.tar", last modified: Thu May  9 04:55:37 2024, max compression
```

## Comparing `partenaire-qualif-0.0.7.tar` & `partenaire-qualif-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 04:51:58.092166 partenaire-qualif-0.0.7/
--rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       30 2024-05-09 04:51:13.000000 partenaire-qualif-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     3256 2024-05-09 04:51:58.090829 partenaire-qualif-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2733 2024-05-09 03:25:03.000000 partenaire-qualif-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 04:51:58.054117 partenaire-qualif-0.0.7/partenaire_qualif.egg-info/
--rw-rw-rw-   0        0        0     3256 2024-05-09 04:51:57.000000 partenaire-qualif-0.0.7/partenaire_qualif.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2024-05-09 04:51:57.000000 partenaire-qualif-0.0.7/partenaire_qualif.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 04:51:57.000000 partenaire-qualif-0.0.7/partenaire_qualif.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-09 04:51:57.000000 partenaire-qualif-0.0.7/partenaire_qualif.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-09 04:51:57.000000 partenaire-qualif-0.0.7/partenaire_qualif.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 04:51:58.084348 partenaire-qualif-0.0.7/qualif/
--rw-rw-rw-   0        0        0      101 2024-05-09 04:06:13.000000 partenaire-qualif-0.0.7/qualif/__init__.py
--rw-rw-rw-   0        0        0     7992 2024-05-09 04:32:27.000000 partenaire-qualif-0.0.7/qualif/qualif.py
-drwxrwxrwx   0        0        0        0 2024-05-09 04:51:58.088344 partenaire-qualif-0.0.7/qualif/templates/
--rw-rw-rw-   0        0        0     2452 2024-05-09 03:11:23.000000 partenaire-qualif-0.0.7/qualif/templates/prompt_find_website_template.txt
--rw-rw-rw-   0        0        0     1747 2024-05-09 03:11:23.000000 partenaire-qualif-0.0.7/qualif/templates/prompt_qualification_template.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 04:51:58.092166 partenaire-qualif-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      943 2024-05-09 04:48:44.000000 partenaire-qualif-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 04:55:37.164001 partenaire-qualif-0.0.8/
+-rw-rw-rw-   0        0        0     1087 2024-05-09 03:19:27.000000 partenaire-qualif-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       30 2024-05-09 04:51:13.000000 partenaire-qualif-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3256 2024-05-09 04:55:37.164001 partenaire-qualif-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2733 2024-05-09 03:25:03.000000 partenaire-qualif-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 04:55:37.128185 partenaire-qualif-0.0.8/partenaire_qualif.egg-info/
+-rw-rw-rw-   0        0        0     3256 2024-05-09 04:55:37.000000 partenaire-qualif-0.0.8/partenaire_qualif.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2024-05-09 04:55:37.000000 partenaire-qualif-0.0.8/partenaire_qualif.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 04:55:37.000000 partenaire-qualif-0.0.8/partenaire_qualif.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-09 04:55:37.000000 partenaire-qualif-0.0.8/partenaire_qualif.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-09 04:55:37.000000 partenaire-qualif-0.0.8/partenaire_qualif.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 04:55:37.164001 partenaire-qualif-0.0.8/qualif/
+-rw-rw-rw-   0        0        0      101 2024-05-09 04:06:13.000000 partenaire-qualif-0.0.8/qualif/__init__.py
+-rw-rw-rw-   0        0        0     7992 2024-05-09 04:32:27.000000 partenaire-qualif-0.0.8/qualif/qualif.py
+drwxrwxrwx   0        0        0        0 2024-05-09 04:55:37.164001 partenaire-qualif-0.0.8/qualif/templates/
+-rw-rw-rw-   0        0        0     2452 2024-05-09 03:11:23.000000 partenaire-qualif-0.0.8/qualif/templates/prompt_find_website_template.txt
+-rw-rw-rw-   0        0        0     1747 2024-05-09 03:11:23.000000 partenaire-qualif-0.0.8/qualif/templates/prompt_qualification_template.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 04:55:37.164001 partenaire-qualif-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      943 2024-05-09 04:55:21.000000 partenaire-qualif-0.0.8/setup.py
```

### Comparing `partenaire-qualif-0.0.7/LICENSE` & `partenaire-qualif-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.7/PKG-INFO` & `partenaire-qualif-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire-qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `partenaire-qualif-0.0.7/README.md` & `partenaire-qualif-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.7/partenaire_qualif.egg-info/PKG-INFO` & `partenaire-qualif-0.0.8/partenaire_qualif.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partenaire-qualif
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.
 Home-page: https://github.com/ymurong/partenaire-qualif.git
 Author: Yanchao MURONG
 Author-email: yanchao.murong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `partenaire-qualif-0.0.7/qualif/qualif.py` & `partenaire-qualif-0.0.8/qualif/qualif.py`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.7/qualif/templates/prompt_find_website_template.txt` & `partenaire-qualif-0.0.8/qualif/templates/prompt_find_website_template.txt`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.7/qualif/templates/prompt_qualification_template.txt` & `partenaire-qualif-0.0.8/qualif/templates/prompt_qualification_template.txt`

 * *Files identical despite different names*

### Comparing `partenaire-qualif-0.0.7/setup.py` & `partenaire-qualif-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="partenaire-qualif",
-    version="0.0.7",
+    version="0.0.8",
     author="Yanchao MURONG",
     author_email="yanchao.murong@gmail.com",
     description="A simple tool that automates the qualification of a partner(reseller/integrator/editor) by finding its website, industries, business functions and services.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ymurong/partenaire-qualif.git",
     packages=setuptools.find_packages(),
```

