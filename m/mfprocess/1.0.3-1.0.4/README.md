# Comparing `tmp/mfprocess-1.0.3.tar.gz` & `tmp/mfprocess-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfprocess-1.0.3.tar", last modified: Thu May  9 13:22:59 2024, max compression
+gzip compressed data, was "mfprocess-1.0.4.tar", last modified: Thu May  9 13:36:30 2024, max compression
```

## Comparing `mfprocess-1.0.3.tar` & `mfprocess-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:22:59.182748 mfprocess-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 13:22:55.000000 mfprocess-1.0.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-09 13:22:59.182748 mfprocess-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 13:22:55.000000 mfprocess-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:22:59.182748 mfprocess-1.0.3/mfprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 13:22:55.000000 mfprocess-1.0.3/mfprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-09 13:22:55.000000 mfprocess-1.0.3/mfprocess/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:22:59.182748 mfprocess-1.0.3/mfprocess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-09 13:22:59.000000 mfprocess-1.0.3/mfprocess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 13:22:59.000000 mfprocess-1.0.3/mfprocess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:22:59.000000 mfprocess-1.0.3/mfprocess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 13:22:59.000000 mfprocess-1.0.3/mfprocess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 13:22:59.000000 mfprocess-1.0.3/mfprocess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:22:59.182748 mfprocess-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-09 13:22:57.000000 mfprocess-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:36:30.286280 mfprocess-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 13:36:26.000000 mfprocess-1.0.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 13:36:30.286280 mfprocess-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 13:36:26.000000 mfprocess-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:36:30.286280 mfprocess-1.0.4/mfprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 13:36:26.000000 mfprocess-1.0.4/mfprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-09 13:36:26.000000 mfprocess-1.0.4/mfprocess/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:36:30.286280 mfprocess-1.0.4/mfprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 13:36:30.000000 mfprocess-1.0.4/mfprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 13:36:30.000000 mfprocess-1.0.4/mfprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:36:30.000000 mfprocess-1.0.4/mfprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 13:36:30.000000 mfprocess-1.0.4/mfprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 13:36:30.000000 mfprocess-1.0.4/mfprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:36:30.286280 mfprocess-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-09 13:36:28.000000 mfprocess-1.0.4/setup.py
```

### Comparing `mfprocess-1.0.3/LICENCE` & `mfprocess-1.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `mfprocess-1.0.3/PKG-INFO` & `mfprocess-1.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 1.0.3
+Version: 1.0.4
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -12,10 +12,13 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: pycountry
+Requires-Dist: pyreadstat
+Requires-Dist: openai==0.28.1
 
 \n# mfprocess
 Data Process
```

### Comparing `mfprocess-1.0.3/mfprocess.egg-info/PKG-INFO` & `mfprocess-1.0.4/mfprocess.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 1.0.3
+Version: 1.0.4
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -12,10 +12,13 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENCE
 Requires-Dist: numpy
 Requires-Dist: pandas
+Requires-Dist: pycountry
+Requires-Dist: pyreadstat
+Requires-Dist: openai==0.28.1
 
 \n# mfprocess
 Data Process
```

### Comparing `mfprocess-1.0.3/setup.py` & `mfprocess-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="mfprocess",
-    version= '1.0.3',  #'0.0.4',   #
+    version= '1.0.4',  #'0.0.4',   #
     author="Agustin Bustos Barton",
     author_email="agustinbustosbarton@gmail.com",
     description="Data Process",
     url = "https://github.com/agustinbustosbarton/mfprocess",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['numpy','pandas'],
+    install_requires=['numpy','pandas','pycountry','pyreadstat','openai==0.28.1'],
     keywords=['pypi', 'cicd', 'python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

