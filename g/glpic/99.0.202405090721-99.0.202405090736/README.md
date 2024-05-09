# Comparing `tmp/glpic-99.0.202405090721.tar.gz` & `tmp/glpic-99.0.202405090736.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glpic-99.0.202405090721.tar", last modified: Thu May  9 07:21:31 2024, max compression
+gzip compressed data, was "glpic-99.0.202405090736.tar", last modified: Thu May  9 07:36:37 2024, max compression
```

## Comparing `glpic-99.0.202405090721.tar` & `glpic-99.0.202405090736.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:21:31.113812 glpic-99.0.202405090721/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-09 07:21:31.113812 glpic-99.0.202405090721/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-09 07:21:07.000000 glpic-99.0.202405090721/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:21:31.109812 glpic-99.0.202405090721/glpic/
--rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-05-09 07:21:07.000000 glpic-99.0.202405090721/glpic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-05-09 07:21:07.000000 glpic-99.0.202405090721/glpic/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:21:31.113812 glpic-99.0.202405090721/glpic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 07:21:31.000000 glpic-99.0.202405090721/glpic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 07:21:31.113812 glpic-99.0.202405090721/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-09 07:21:30.000000 glpic-99.0.202405090721/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:36:37.713766 glpic-99.0.202405090736/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-09 07:36:37.713766 glpic-99.0.202405090736/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-09 07:36:14.000000 glpic-99.0.202405090736/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:36:37.713766 glpic-99.0.202405090736/glpic/
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-05-09 07:36:14.000000 glpic-99.0.202405090736/glpic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10521 2024-05-09 07:36:14.000000 glpic-99.0.202405090736/glpic/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 07:36:37.713766 glpic-99.0.202405090736/glpic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-09 07:36:37.000000 glpic-99.0.202405090736/glpic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-09 07:36:37.000000 glpic-99.0.202405090736/glpic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:36:37.000000 glpic-99.0.202405090736/glpic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-09 07:36:37.000000 glpic-99.0.202405090736/glpic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 07:36:37.000000 glpic-99.0.202405090736/glpic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 07:36:37.000000 glpic-99.0.202405090736/glpic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 07:36:37.000000 glpic-99.0.202405090736/glpic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 07:36:37.713766 glpic-99.0.202405090736/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-09 07:36:37.000000 glpic-99.0.202405090736/setup.py
```

### Comparing `glpic-99.0.202405090721/README.md` & `glpic-99.0.202405090736/README.md`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405090721/glpic/__init__.py` & `glpic-99.0.202405090736/glpic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from ast import literal_eval
 from dateutil.parser import parse
-from datetime import date, timedelta
+from datetime import date, datetime, timedelta
+from dateutil.relativedelta import relativedelta
 import json
 import ssl
 import os
 import sys
 from urllib.request import urlopen, Request
 from urllib.parse import urlencode
 
@@ -245,16 +246,18 @@
         valid_keys = list(_get(f'{self.base_url}/Reservation/', self.headers)[0].keys()) + ['user']
         wrong_keys = [key for key in overrides if key not in valid_keys]
         if wrong_keys:
             error(f"Ignoring keys {','.join(wrong_keys)}")
             for key in wrong_keys:
                 del overrides[key]
         if not overrides:
-            info("Nothing to update")
-            return
+            date_after_month = datetime.today() + relativedelta(months=1)
+            new_date = date_after_month.strftime('%Y-%m-%d 00:00:00')
+            info(f"Updating end date to {new_date}")
+            overrides['end'] = new_date
         if 'end' in overrides:
             overrides['end'] = parse(str(overrides['end'])).strftime('%Y-%m-%d 00:00:00')
         new_user = overrides.get('user') or overrides.get('users_id')
         if new_user is not None and not str(new_user).isnumeric():
             overrides['users_id'] = self.get_user(new_user)['id']
         if 'user' in overrides:
             del overrides['user']
```

### Comparing `glpic-99.0.202405090721/glpic/cli.py` & `glpic-99.0.202405090736/glpic/cli.py`

 * *Files identical despite different names*

### Comparing `glpic-99.0.202405090721/setup.py` & `glpic-99.0.202405090736/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 description = 'Glpic wrapper'
 long_description = description
 if os.path.exists('README.rst'):
     long_description = open('README.rst').read()
 
 setup(
     name='glpic',
-    version='99.0.202405090721',
+    version='99.0.202405090736',
     include_package_data=True,
     packages=find_packages(),
     zip_safe=False,
     description=description,
     long_description=long_description,
     url='http://github.com/karmab/glpic',
     author='Karim Boumedhel',
```

