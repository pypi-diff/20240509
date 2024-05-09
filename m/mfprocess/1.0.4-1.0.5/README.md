# Comparing `tmp/mfprocess-1.0.4.tar.gz` & `tmp/mfprocess-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfprocess-1.0.4.tar", last modified: Thu May  9 13:36:30 2024, max compression
+gzip compressed data, was "mfprocess-1.0.5.tar", last modified: Thu May  9 13:38:18 2024, max compression
```

## Comparing `mfprocess-1.0.4.tar` & `mfprocess-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:36:30.286280 mfprocess-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 13:36:26.000000 mfprocess-1.0.4/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 13:36:30.286280 mfprocess-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 13:36:26.000000 mfprocess-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:36:30.286280 mfprocess-1.0.4/mfprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 13:36:26.000000 mfprocess-1.0.4/mfprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-09 13:36:26.000000 mfprocess-1.0.4/mfprocess/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:36:30.286280 mfprocess-1.0.4/mfprocess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 13:36:30.000000 mfprocess-1.0.4/mfprocess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 13:36:30.000000 mfprocess-1.0.4/mfprocess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:36:30.000000 mfprocess-1.0.4/mfprocess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 13:36:30.000000 mfprocess-1.0.4/mfprocess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 13:36:30.000000 mfprocess-1.0.4/mfprocess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:36:30.286280 mfprocess-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-09 13:36:28.000000 mfprocess-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:38:18.161835 mfprocess-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 13:38:14.000000 mfprocess-1.0.5/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 13:38:18.161835 mfprocess-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 13:38:14.000000 mfprocess-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:38:18.161835 mfprocess-1.0.5/mfprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 13:38:14.000000 mfprocess-1.0.5/mfprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-09 13:38:14.000000 mfprocess-1.0.5/mfprocess/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:38:18.161835 mfprocess-1.0.5/mfprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 13:38:18.000000 mfprocess-1.0.5/mfprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 13:38:18.000000 mfprocess-1.0.5/mfprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:38:18.000000 mfprocess-1.0.5/mfprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 13:38:18.000000 mfprocess-1.0.5/mfprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 13:38:18.000000 mfprocess-1.0.5/mfprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:38:18.165835 mfprocess-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-09 13:38:16.000000 mfprocess-1.0.5/setup.py
```

### Comparing `mfprocess-1.0.4/LICENCE` & `mfprocess-1.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `mfprocess-1.0.4/PKG-INFO` & `mfprocess-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 1.0.4
+Version: 1.0.5
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-1.0.4/mfprocess/functions.py` & `mfprocess-1.0.5/mfprocess/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   answer = ''.join(filter(whitelist.__contains__, x))
   try:
     return pycountry.countries.search_fuzzy(answer)[0].alpha_3
   except:
     got_it=True
     while got_it:
       try:
-        other_fuzzy=get_gorilla_response(prompt=answer, functions=[function_documentation]).country
+        other_fuzzy=ask_gpt(prompt=answer, functions=[function_documentation]).country
         got_it=False
         return pycountry.countries.search_fuzzy(other_fuzzy)[0].alpha_3
       except:
         time.sleep(5)
 def get_data(path=False,sheet_name=0,usecols=None,header=0):  #easy get data from MES csv   ###############################################  path y sheet_name
     #import drive
     drive.mount("/content/drive")
```

### Comparing `mfprocess-1.0.4/mfprocess.egg-info/PKG-INFO` & `mfprocess-1.0.5/mfprocess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 1.0.4
+Version: 1.0.5
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-1.0.4/setup.py` & `mfprocess-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="mfprocess",
-    version= '1.0.4',  #'0.0.4',   #
+    version= '1.0.5',  #'0.0.4',   #
     author="Agustin Bustos Barton",
     author_email="agustinbustosbarton@gmail.com",
     description="Data Process",
     url = "https://github.com/agustinbustosbarton/mfprocess",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

