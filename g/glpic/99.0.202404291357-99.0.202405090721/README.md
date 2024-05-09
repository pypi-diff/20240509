# Comparing `tmp/glpic-99.0.202404291357.tar.gz` & `tmp/glpic-99.0.202405090721.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202404291357.tar", last modified: Mon Apr 29 13:57:50 2024, max compression
+gzip compressed data, was "glpic-99.0.202405090721.tar", last modified: Thu May  9 07:21:31 2024, max compression
```

## Comparing `glpic-99.0.202404291357.tar` & `glpic-99.0.202405090721.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:50.084308 glpic-99.0.202404291357/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-29 13:57:50.084308 glpic-99.0.202404291357/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-29 13:57:37.000000 glpic-99.0.202404291357/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:50.080308 glpic-99.0.202404291357/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-29 13:57:37.000000 glpic-99.0.202404291357/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-04-29 13:57:37.000000 glpic-99.0.202404291357/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:57:50.084308 glpic-99.0.202404291357/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-29 13:57:50.000000 glpic-99.0.202404291357/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-29 13:57:50.000000 glpic-99.0.202404291357/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:57:50.000000 glpic-99.0.202404291357/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-29 13:57:50.000000 glpic-99.0.202404291357/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:57:50.000000 glpic-99.0.202404291357/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 13:57:50.000000 glpic-99.0.202404291357/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 13:57:50.000000 glpic-99.0.202404291357/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:57:50.084308 glpic-99.0.202404291357/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-29 13:57:49.000000 glpic-99.0.202404291357/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:21:31.113812 glpic-99.0.202405090721/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-09 07:21:31.113812 glpic-99.0.202405090721/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-09 07:21:07.000000 glpic-99.0.202405090721/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:21:31.109812 glpic-99.0.202405090721/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-05-09 07:21:07.000000 glpic-99.0.202405090721/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-05-09 07:21:07.000000 glpic-99.0.202405090721/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:21:31.113812 glpic-99.0.202405090721/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 07:21:31.113812 glpic-99.0.202405090721/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-09 07:21:30.000000 glpic-99.0.202405090721/setup.py
```

### Comparing `glpic-99.0.202404291357/README.md` & `glpic-99.0.202405090721/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404291357/glpic/__init__.py` & `glpic-99.0.202405090721/glpic/__init__.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404291357/glpic/cli.py` & `glpic-99.0.202405090721/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202404291357/setup.py` & `glpic-99.0.202405090721/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202404291357',
+    version='99.0.202405090721',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

