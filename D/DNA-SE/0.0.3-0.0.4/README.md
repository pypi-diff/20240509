# Comparing `tmp/dna_se-0.0.3.tar.gz` & `tmp/dna_se-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dna_se-0.0.3.tar", last modified: Thu May  9 06:32:07 2024, max compression
+gzip compressed data, was "dna_se-0.0.4.tar", last modified: Thu May  9 06:46:02 2024, max compression
```

## Comparing `dna_se-0.0.3.tar` & `dna_se-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 06:32:07.000000 dna_se-0.0.3/
-drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 06:32:07.000000 dna_se-0.0.3/DNA_SE/
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     5069 2024-05-08 12:53:11.000000 dna_se-0.0.3/DNA_SE/DNA_SE.py
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)       25 2024-05-08 12:46:34.000000 dna_se-0.0.3/DNA_SE/__init__.py
-drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 06:32:07.000000 dna_se-0.0.3/DNA_SE.egg-info/
--rw-r--r--   0 r12user2  (1003) r12user2  (1003)     2202 2024-05-09 06:32:07.000000 dna_se-0.0.3/DNA_SE.egg-info/PKG-INFO
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)      186 2024-05-09 06:32:07.000000 dna_se-0.0.3/DNA_SE.egg-info/SOURCES.txt
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)        1 2024-05-09 06:32:07.000000 dna_se-0.0.3/DNA_SE.egg-info/dependency_links.txt
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)        7 2024-05-09 06:32:07.000000 dna_se-0.0.3/DNA_SE.egg-info/top_level.txt
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     1091 2024-05-08 12:46:34.000000 dna_se-0.0.3/LICENSE.txt
--rw-r--r--   0 r12user2  (1003) r12user2  (1003)     2202 2024-05-09 06:32:07.000000 dna_se-0.0.3/PKG-INFO
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     1783 2024-05-08 12:46:34.000000 dna_se-0.0.3/README.md
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)       38 2024-05-09 06:32:07.000000 dna_se-0.0.3/setup.cfg
--rw-rw-r--   0 r12user2  (1003) r12user2  (1003)      686 2024-05-09 06:26:27.000000 dna_se-0.0.3/setup.py
+drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 06:46:02.000000 dna_se-0.0.4/
+drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 06:46:02.000000 dna_se-0.0.4/DNA_SE/
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     5069 2024-05-08 12:53:11.000000 dna_se-0.0.4/DNA_SE/DNA_SE.py
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)       25 2024-05-08 12:46:34.000000 dna_se-0.0.4/DNA_SE/__init__.py
+drwxrwxr-x   0 r12user2  (1003) r12user2  (1003)        0 2024-05-09 06:46:02.000000 dna_se-0.0.4/DNA_SE.egg-info/
+-rw-r--r--   0 r12user2  (1003) r12user2  (1003)     2202 2024-05-09 06:46:01.000000 dna_se-0.0.4/DNA_SE.egg-info/PKG-INFO
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)      186 2024-05-09 06:46:01.000000 dna_se-0.0.4/DNA_SE.egg-info/SOURCES.txt
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)        1 2024-05-09 06:46:01.000000 dna_se-0.0.4/DNA_SE.egg-info/dependency_links.txt
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)        7 2024-05-09 06:46:01.000000 dna_se-0.0.4/DNA_SE.egg-info/top_level.txt
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     1091 2024-05-08 12:46:34.000000 dna_se-0.0.4/LICENSE.txt
+-rw-r--r--   0 r12user2  (1003) r12user2  (1003)     2202 2024-05-09 06:46:02.000000 dna_se-0.0.4/PKG-INFO
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)     1783 2024-05-08 12:46:34.000000 dna_se-0.0.4/README.md
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)       38 2024-05-09 06:46:02.000000 dna_se-0.0.4/setup.cfg
+-rw-rw-r--   0 r12user2  (1003) r12user2  (1003)      686 2024-05-09 06:44:55.000000 dna_se-0.0.4/setup.py
```

### Comparing `dna_se-0.0.3/DNA_SE/DNA_SE.py` & `dna_se-0.0.4/DNA_SE/DNA_SE.py`

 * *Files identical despite different names*

### Comparing `dna_se-0.0.3/DNA_SE.egg-info/PKG-INFO` & `dna_se-0.0.4/DNA_SE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DNA_SE
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/liuqs111/DNA-SE
 Author: Qinshuo
 Author-email: u3008680@connect.hku.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dna_se-0.0.3/LICENSE.txt` & `dna_se-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dna_se-0.0.3/PKG-INFO` & `dna_se-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DNA_SE
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/liuqs111/DNA-SE
 Author: Qinshuo
 Author-email: u3008680@connect.hku.hk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dna_se-0.0.3/README.md` & `dna_se-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dna_se-0.0.3/setup.py` & `dna_se-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="DNA_SE", # Replace with your own username
-    version="0.0.3",
+    version="0.0.4",
     author="Qinshuo",
     author_email="u3008680@connect.hku.hk",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liuqs111/DNA-SE",
     packages=setuptools.find_packages(),
```

