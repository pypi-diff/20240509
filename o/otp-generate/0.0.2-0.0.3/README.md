# Comparing `tmp/otp_generate-0.0.2.tar.gz` & `tmp/otp_generate-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otp_generate-0.0.2.tar", last modified: Thu May  9 05:35:28 2024, max compression
+gzip compressed data, was "otp_generate-0.0.3.tar", last modified: Thu May  9 05:36:06 2024, max compression
```

## Comparing `otp_generate-0.0.2.tar` & `otp_generate-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-09 05:35:28.276034 otp_generate-0.0.2/
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     1083 2024-05-08 11:06:07.000000 otp_generate-0.0.2/LICENSE
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      370 2024-05-09 05:35:28.276034 otp_generate-0.0.2/PKG-INFO
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       39 2024-05-08 11:06:07.000000 otp_generate-0.0.2/README.md
-drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-09 05:35:28.276034 otp_generate-0.0.2/otp_generate/
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       39 2024-05-08 13:44:02.000000 otp_generate-0.0.2/otp_generate/__init__.py
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      619 2024-05-08 13:44:02.000000 otp_generate-0.0.2/otp_generate/main.py
-drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-09 05:35:28.276034 otp_generate-0.0.2/otp_generate.egg-info/
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      370 2024-05-09 05:35:28.000000 otp_generate-0.0.2/otp_generate.egg-info/PKG-INFO
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      290 2024-05-09 05:35:28.000000 otp_generate-0.0.2/otp_generate.egg-info/SOURCES.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)        1 2024-05-09 05:35:28.000000 otp_generate-0.0.2/otp_generate.egg-info/dependency_links.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       61 2024-05-09 05:35:28.000000 otp_generate-0.0.2/otp_generate.egg-info/entry_points.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       13 2024-05-09 05:35:28.000000 otp_generate-0.0.2/otp_generate.egg-info/requires.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       13 2024-05-09 05:35:28.000000 otp_generate-0.0.2/otp_generate.egg-info/top_level.txt
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       38 2024-05-09 05:35:28.277034 otp_generate-0.0.2/setup.cfg
--rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      852 2024-05-09 05:35:18.000000 otp_generate-0.0.2/setup.py
+drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-09 05:36:06.291741 otp_generate-0.0.3/
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)     1083 2024-05-08 11:06:07.000000 otp_generate-0.0.3/LICENSE
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      370 2024-05-09 05:36:06.291741 otp_generate-0.0.3/PKG-INFO
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       39 2024-05-08 11:06:07.000000 otp_generate-0.0.3/README.md
+drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-09 05:36:06.290742 otp_generate-0.0.3/otp_generate/
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       39 2024-05-08 13:44:02.000000 otp_generate-0.0.3/otp_generate/__init__.py
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      619 2024-05-08 13:44:02.000000 otp_generate-0.0.3/otp_generate/main.py
+drwxr-xr-x   0 marimuthu  (1000) marimuthu  (1000)        0 2024-05-09 05:36:06.291741 otp_generate-0.0.3/otp_generate.egg-info/
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      370 2024-05-09 05:36:06.000000 otp_generate-0.0.3/otp_generate.egg-info/PKG-INFO
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      290 2024-05-09 05:36:06.000000 otp_generate-0.0.3/otp_generate.egg-info/SOURCES.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)        1 2024-05-09 05:36:06.000000 otp_generate-0.0.3/otp_generate.egg-info/dependency_links.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       61 2024-05-09 05:36:06.000000 otp_generate-0.0.3/otp_generate.egg-info/entry_points.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       13 2024-05-09 05:36:06.000000 otp_generate-0.0.3/otp_generate.egg-info/requires.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       13 2024-05-09 05:36:06.000000 otp_generate-0.0.3/otp_generate.egg-info/top_level.txt
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)       38 2024-05-09 05:36:06.291741 otp_generate-0.0.3/setup.cfg
+-rw-r--r--   0 marimuthu  (1000) marimuthu  (1000)      852 2024-05-09 05:35:57.000000 otp_generate-0.0.3/setup.py
```

### Comparing `otp_generate-0.0.2/LICENSE` & `otp_generate-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `otp_generate-0.0.2/otp_generate/main.py` & `otp_generate-0.0.3/otp_generate/main.py`

 * *Files identical despite different names*

### Comparing `otp_generate-0.0.2/setup.py` & `otp_generate-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 working_directory = path.abspath(path.dirname(__file__))
 
 with open(path.join(working_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='otp_generate',  # name of package which will be package dir below project
-    version='0.0.2',
+    version='0.0.3',
     url='https://github.com/MariMuthu15/otp-generate-package',
     author='Marimuthu',
     author_email='mahimari555@gmail.com',
     description='A simple otp generate package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

