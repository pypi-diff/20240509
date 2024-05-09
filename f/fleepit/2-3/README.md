# Comparing `tmp/fleepit-2.tar.gz` & `tmp/fleepit-3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleepit-2.tar", last modified: Wed May  8 23:58:17 2024, max compression
+gzip compressed data, was "fleepit-3.tar", last modified: Thu May  9 00:00:05 2024, max compression
```

## Comparing `fleepit-2.tar` & `fleepit-3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pegasko   (1000) pegasko   (1000)        0 2024-05-08 23:58:17.141579 fleepit-2/
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)    11358 2024-05-08 23:36:33.000000 fleepit-2/LICENSE
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      106 2024-05-08 23:46:21.000000 fleepit-2/NOTICE
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      792 2024-05-08 23:58:17.141579 fleepit-2/PKG-INFO
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      441 2024-05-08 23:49:01.000000 fleepit-2/README.md
-drwxr-xr-x   0 pegasko   (1000) pegasko   (1000)        0 2024-05-08 23:58:17.141579 fleepit-2/fleepit.egg-info/
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      792 2024-05-08 23:58:17.000000 fleepit-2/fleepit.egg-info/PKG-INFO
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      202 2024-05-08 23:58:17.000000 fleepit-2/fleepit.egg-info/SOURCES.txt
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)        1 2024-05-08 23:58:17.000000 fleepit-2/fleepit.egg-info/dependency_links.txt
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)       41 2024-05-08 23:58:17.000000 fleepit-2/fleepit.egg-info/entry_points.txt
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)        8 2024-05-08 23:58:17.000000 fleepit-2/fleepit.egg-info/top_level.txt
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)     2642 2024-05-08 23:37:42.000000 fleepit-2/fleepit.py
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)       38 2024-05-08 23:58:17.141579 fleepit-2/setup.cfg
--rw-r--r--   0 pegasko   (1000) pegasko   (1000)      823 2024-05-08 23:58:14.000000 fleepit-2/setup.py
+drwxr-xr-x   0 pegasko   (1000) pegasko   (1000)        0 2024-05-09 00:00:05.108961 fleepit-3/
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)    11358 2024-05-08 23:36:33.000000 fleepit-3/LICENSE
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      106 2024-05-08 23:46:21.000000 fleepit-3/NOTICE
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      831 2024-05-09 00:00:05.108961 fleepit-3/PKG-INFO
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      456 2024-05-08 23:59:32.000000 fleepit-3/README.md
+drwxr-xr-x   0 pegasko   (1000) pegasko   (1000)        0 2024-05-09 00:00:05.108961 fleepit-3/fleepit.egg-info/
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      831 2024-05-09 00:00:05.000000 fleepit-3/fleepit.egg-info/PKG-INFO
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      202 2024-05-09 00:00:05.000000 fleepit-3/fleepit.egg-info/SOURCES.txt
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)        1 2024-05-09 00:00:05.000000 fleepit-3/fleepit.egg-info/dependency_links.txt
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)       41 2024-05-09 00:00:05.000000 fleepit-3/fleepit.egg-info/entry_points.txt
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)        8 2024-05-09 00:00:05.000000 fleepit-3/fleepit.egg-info/top_level.txt
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)     2642 2024-05-08 23:37:42.000000 fleepit-3/fleepit.py
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)       38 2024-05-09 00:00:05.108961 fleepit-3/setup.cfg
+-rw-r--r--   0 pegasko   (1000) pegasko   (1000)      847 2024-05-09 00:00:02.000000 fleepit-3/setup.py
```

### Comparing `fleepit-2/LICENSE` & `fleepit-3/LICENSE`

 * *Files identical despite different names*

### Comparing `fleepit-2/PKG-INFO` & `fleepit-3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fleepit
-Version: 2
-Summary: keyboard layout switcher based on xclip & other things
+Version: 3
+Summary: Text seleciton keyboard layout switcher based on xclip / etc for X11 & wayland
 Home-page: https://git.pegasko.art/bitrate16/fleepit
 Author-email: pegasko@pegasko.art
 License: AGPL 3.0
 Keywords: keyboard layout shortcut layout-switcher
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # fleepit
 
-Keyboard layout switcher based on xclip / etc for X11 & wayland
+Text seleciton keyboard layout switcher based on xclip / etc for X11 & wayland
 
 # Install
 
 1. Install required packages:
   * X11: `xclip`, `xdotool`
 
 2. install module: `pip install fleepit`
```

### Comparing `fleepit-2/fleepit.egg-info/PKG-INFO` & `fleepit-3/fleepit.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fleepit
-Version: 2
-Summary: keyboard layout switcher based on xclip & other things
+Version: 3
+Summary: Text seleciton keyboard layout switcher based on xclip / etc for X11 & wayland
 Home-page: https://git.pegasko.art/bitrate16/fleepit
 Author-email: pegasko@pegasko.art
 License: AGPL 3.0
 Keywords: keyboard layout shortcut layout-switcher
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # fleepit
 
-Keyboard layout switcher based on xclip / etc for X11 & wayland
+Text seleciton keyboard layout switcher based on xclip / etc for X11 & wayland
 
 # Install
 
 1. Install required packages:
   * X11: `xclip`, `xdotool`
 
 2. install module: `pip install fleepit`
```

### Comparing `fleepit-2/fleepit.py` & `fleepit-3/fleepit.py`

 * *Files identical despite different names*

### Comparing `fleepit-2/setup.py` & `fleepit-3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     long_description_content_type = 'text/markdown'
 except:
     long_description = None
     long_description_content_type = None
 
 setup(
     name='fleepit',
-    version='2',
+    version='3',
     py_modules=['fleepit'],
-    description='keyboard layout switcher based on xclip & other things',
+    description='Text seleciton keyboard layout switcher based on xclip / etc for X11 & wayland',
     url='https://git.pegasko.art/bitrate16/fleepit',
     author_email='pegasko@pegasko.art',
     license='AGPL 3.0',
     keywords='keyboard layout shortcut layout-switcher',
     entry_points='''
         [console_scripts]
         fleepit=fleepit:main
```

