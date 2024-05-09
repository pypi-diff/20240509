# Comparing `tmp/mfprocess-1.0.5.tar.gz` & `tmp/mfprocess-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfprocess-1.0.5.tar", last modified: Thu May  9 13:38:18 2024, max compression
+gzip compressed data, was "mfprocess-1.0.6.tar", last modified: Thu May  9 13:46:49 2024, max compression
```

## Comparing `mfprocess-1.0.5.tar` & `mfprocess-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:38:18.161835 mfprocess-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 13:38:14.000000 mfprocess-1.0.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 13:38:18.161835 mfprocess-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 13:38:14.000000 mfprocess-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:38:18.161835 mfprocess-1.0.5/mfprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 13:38:14.000000 mfprocess-1.0.5/mfprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3275 2024-05-09 13:38:14.000000 mfprocess-1.0.5/mfprocess/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:38:18.161835 mfprocess-1.0.5/mfprocess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 13:38:18.000000 mfprocess-1.0.5/mfprocess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 13:38:18.000000 mfprocess-1.0.5/mfprocess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:38:18.000000 mfprocess-1.0.5/mfprocess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 13:38:18.000000 mfprocess-1.0.5/mfprocess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 13:38:18.000000 mfprocess-1.0.5/mfprocess.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:38:18.165835 mfprocess-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-09 13:38:16.000000 mfprocess-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:46:49.523936 mfprocess-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-09 13:46:41.000000 mfprocess-1.0.6/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 13:46:49.523936 mfprocess-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 13:46:41.000000 mfprocess-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:46:49.523936 mfprocess-1.0.6/mfprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-09 13:46:41.000000 mfprocess-1.0.6/mfprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-09 13:46:41.000000 mfprocess-1.0.6/mfprocess/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:46:49.523936 mfprocess-1.0.6/mfprocess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-09 13:46:49.000000 mfprocess-1.0.6/mfprocess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-09 13:46:49.000000 mfprocess-1.0.6/mfprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:46:49.000000 mfprocess-1.0.6/mfprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 13:46:49.000000 mfprocess-1.0.6/mfprocess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 13:46:49.000000 mfprocess-1.0.6/mfprocess.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:46:49.523936 mfprocess-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-09 13:46:47.000000 mfprocess-1.0.6/setup.py
```

### Comparing `mfprocess-1.0.5/LICENCE` & `mfprocess-1.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `mfprocess-1.0.5/PKG-INFO` & `mfprocess-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 1.0.5
+Version: 1.0.6
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-1.0.5/mfprocess/functions.py` & `mfprocess-1.0.6/mfprocess/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,8 +88,14 @@
        pass
     try:
       df["Weeks"]=pd.to_datetime(df["Weeks"])
     except:
       pass
     
     return df
+def next_weekday(d, weekday): #0 monday
+    days_ahead = weekday - d.weekday()
+    if days_ahead <= 0: # Target day already happened this week
+        days_ahead += 7
+    return d + datetime.timedelta(days_ahead)
+
```

### Comparing `mfprocess-1.0.5/mfprocess.egg-info/PKG-INFO` & `mfprocess-1.0.6/mfprocess.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfprocess
-Version: 1.0.5
+Version: 1.0.6
 Summary: Data Process
 Home-page: https://github.com/agustinbustosbarton/mfprocess
 Author: Agustin Bustos Barton
 Author-email: agustinbustosbarton@gmail.com
 Keywords: pypi,cicd,python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `mfprocess-1.0.5/setup.py` & `mfprocess-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="mfprocess",
-    version= '1.0.5',  #'0.0.4',   #
+    version= '1.0.6',  #'0.0.4',   #
     author="Agustin Bustos Barton",
     author_email="agustinbustosbarton@gmail.com",
     description="Data Process",
     url = "https://github.com/agustinbustosbarton/mfprocess",
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

