# Comparing `tmp/wifind-0.0.9.tar.gz` & `tmp/wifind-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wifind-0.0.9.tar", last modified: Thu Mar  7 12:42:02 2024, max compression
+gzip compressed data, was "wifind-0.1.0.tar", last modified: Thu May  9 07:53:32 2024, max compression
```

## Comparing `wifind-0.0.9.tar` & `wifind-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:42:02.100862 wifind-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-07 12:41:55.000000 wifind-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-07 12:42:02.100862 wifind-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-07 12:41:55.000000 wifind-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 12:42:02.100862 wifind-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-07 12:41:55.000000 wifind-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:42:02.100862 wifind-0.0.9/wifind/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 12:41:55.000000 wifind-0.0.9/wifind/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-07 12:41:55.000000 wifind-0.0.9/wifind/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-07 12:41:55.000000 wifind-0.0.9/wifind/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-07 12:41:55.000000 wifind-0.0.9/wifind/learn.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-07 12:41:55.000000 wifind-0.0.9/wifind/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-07 12:41:55.000000 wifind-0.0.9/wifind/rooms.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-07 12:41:55.000000 wifind-0.0.9/wifind/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-07 12:41:55.000000 wifind-0.0.9/wifind/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-03-07 12:41:55.000000 wifind-0.0.9/wifind/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 12:42:02.100862 wifind-0.0.9/wifind.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-07 12:42:02.000000 wifind-0.0.9/wifind.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-07 12:42:02.000000 wifind-0.0.9/wifind.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 12:42:02.000000 wifind-0.0.9/wifind.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-07 12:42:02.000000 wifind-0.0.9/wifind.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 12:42:01.000000 wifind-0.0.9/wifind.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-07 12:42:02.000000 wifind-0.0.9/wifind.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-07 12:42:02.000000 wifind-0.0.9/wifind.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:53:32.468236 wifind-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-09 07:53:26.000000 wifind-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-09 07:53:32.468236 wifind-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-09 07:53:26.000000 wifind-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 07:53:32.468236 wifind-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-09 07:53:26.000000 wifind-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:53:32.464236 wifind-0.1.0/wifind/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 07:53:26.000000 wifind-0.1.0/wifind/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-09 07:53:26.000000 wifind-0.1.0/wifind/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-09 07:53:26.000000 wifind-0.1.0/wifind/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-09 07:53:26.000000 wifind-0.1.0/wifind/learn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-09 07:53:26.000000 wifind-0.1.0/wifind/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-09 07:53:26.000000 wifind-0.1.0/wifind/rooms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-09 07:53:26.000000 wifind-0.1.0/wifind/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-09 07:53:26.000000 wifind-0.1.0/wifind/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-09 07:53:26.000000 wifind-0.1.0/wifind/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:53:32.464236 wifind-0.1.0/wifind.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-09 07:53:32.000000 wifind-0.1.0/wifind.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-09 07:53:32.000000 wifind-0.1.0/wifind.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:53:32.000000 wifind-0.1.0/wifind.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-09 07:53:32.000000 wifind-0.1.0/wifind.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:53:32.000000 wifind-0.1.0/wifind.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 07:53:32.000000 wifind-0.1.0/wifind.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 07:53:32.000000 wifind-0.1.0/wifind.egg-info/top_level.txt
```

### Comparing `wifind-0.0.9/LICENSE` & `wifind-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wifind-0.0.9/PKG-INFO` & `wifind-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wifind
-Version: 0.0.9
+Version: 0.1.0
 Summary: Wi-Fi indoor positioning system
 Home-page: https://github.com/micheledinelli/wifind
 Author: Dinelli Michele
 Author-email: dinellimichele00@gmail.com
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `wifind-0.0.9/README.md` & `wifind-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `wifind-0.0.9/setup.py` & `wifind-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import find_packages
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 MAJOR_VERSION = '0'
-MINOR_VERSION = '0'
-MICRO_VERSION = '9'
+MINOR_VERSION = '1'
+MICRO_VERSION = '0'
 VERSION = "{}.{}.{}".format(MAJOR_VERSION, MINOR_VERSION, MICRO_VERSION)
 
 setup(name='wifind',
       version=VERSION,
       description="Wi-Fi indoor positioning system",
       long_description=long_description,
       long_description_content_type='text/markdown',
```

### Comparing `wifind-0.0.9/wifind/__main__.py` & `wifind-0.1.0/wifind/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,14 @@
     try:
         parser = argparse.ArgumentParser(description="Scan Wi-Fi networks.")
         subparsers = parser.add_subparsers(title="subcommands", dest="subcommand")
 
         learn_parser = subparsers.add_parser("learn", help="Learn current position")
         learn_parser.add_argument("-r", "--room", help="Name of the room to sample", required=True)
 
-        # depp_learn_parser = subparsers.add_parser("deep-learn", help="Learn current position")
-        # depp_learn_parser.add_argument("-n", "--num", help="Number of samples to collect", required=True)
-        # depp_learn_parser.add_argument("-r", "--room", help="Name of the room to sample", required=True)
-
         clean_parser = subparsers.add_parser("clear", help="Clear the data file")
         predict_parser = subparsers.add_parser("predict", help="Predict the room")
         predict_parser.add_argument("-p", "--proba", help="Predict the probability", action="store_true", required=False)
         
         room_parser = subparsers.add_parser("rooms", help="List the rooms in the data file")
         room_parser.add_argument("-s", "--samples", help="List the number of sample", required=False)
```

### Comparing `wifind-0.0.9/wifind/predict.py` & `wifind-0.1.0/wifind/predict.py`

 * *Files identical despite different names*

### Comparing `wifind-0.0.9/wifind/scan.py` & `wifind-0.1.0/wifind/scan.py`

 * *Files identical despite different names*

### Comparing `wifind-0.0.9/wifind/utils.py` & `wifind-0.1.0/wifind/utils.py`

 * *Files identical despite different names*

### Comparing `wifind-0.0.9/wifind.egg-info/PKG-INFO` & `wifind-0.1.0/wifind.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wifind
-Version: 0.0.9
+Version: 0.1.0
 Summary: Wi-Fi indoor positioning system
 Home-page: https://github.com/micheledinelli/wifind
 Author: Dinelli Michele
 Author-email: dinellimichele00@gmail.com
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

