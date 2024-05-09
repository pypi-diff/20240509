# Comparing `tmp/mfprocess-1.0.2.tar.gz` & `tmp/mfprocess-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfprocess-1.0.2.tar", last modified: Tue May  7 17:59:35 2024, max compression
+gzip compressed data, was "mfprocess-1.0.3.tar", last modified: Thu May  9 13:22:59 2024, max compression
```

## Comparing `mfprocess-1.0.2.tar` & `mfprocess-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:35.989344 mfprocess-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-07 17:59:31.000000 mfprocess-1.0.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-07 17:59:35.989344 mfprocess-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-07 17:59:31.000000 mfprocess-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:35.989344 mfprocess-1.0.2/mfprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-07 17:59:31.000000 mfprocess-1.0.2/mfprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-07 17:59:31.000000 mfprocess-1.0.2/mfprocess/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:59:35.989344 mfprocess-1.0.2/mfprocess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-07 17:59:35.000000 mfprocess-1.0.2/mfprocess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-07 17:59:35.000000 mfprocess-1.0.2/mfprocess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:59:35.000000 mfprocess-1.0.2/mfprocess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 17:59:35.000000 mfprocess-1.0.2/mfprocess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-07 17:59:35.000000 mfprocess-1.0.2/mfprocess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:59:35.989344 mfprocess-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-07 17:59:34.000000 mfprocess-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:22:59.182748 mfprocess-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 13:22:55.000000 mfprocess-1.0.3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-09 13:22:59.182748 mfprocess-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 13:22:55.000000 mfprocess-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:22:59.182748 mfprocess-1.0.3/mfprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 13:22:55.000000 mfprocess-1.0.3/mfprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-09 13:22:55.000000 mfprocess-1.0.3/mfprocess/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:22:59.182748 mfprocess-1.0.3/mfprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-09 13:22:59.000000 mfprocess-1.0.3/mfprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 13:22:59.000000 mfprocess-1.0.3/mfprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:22:59.000000 mfprocess-1.0.3/mfprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 13:22:59.000000 mfprocess-1.0.3/mfprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 13:22:59.000000 mfprocess-1.0.3/mfprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:22:59.182748 mfprocess-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-09 13:22:57.000000 mfprocess-1.0.3/setup.py
```

### Comparing `mfprocess-1.0.2/LICENCE` & `mfprocess-1.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `mfprocess-1.0.2/PKG-INFO` & `mfprocess-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 1.0.2
+Version: 1.0.3
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-1.0.2/mfprocess.egg-info/PKG-INFO` & `mfprocess-1.0.3/mfprocess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 1.0.2
+Version: 1.0.3
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-1.0.2/setup.py` & `mfprocess-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="mfprocess",
-    version= '1.0.2',  #'0.0.4',   #
+    version= '1.0.3',  #'0.0.4',   #
     author="Agustin Bustos Barton",
     author_email="agustinbustosbarton@gmail.com",
     description="Data Process",
     url = "https://github.com/agustinbustosbarton/mfprocess",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

