# Comparing `tmp/dreamhack-1.0.1.tar.gz` & `tmp/dreamhack-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamhack-1.0.1.tar", last modified: Thu May  9 14:41:32 2024, max compression
+gzip compressed data, was "dreamhack-1.0.2.tar", last modified: Thu May  9 17:10:03 2024, max compression
```

## Comparing `dreamhack-1.0.1.tar` & `dreamhack-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 14:41:32.763700 dreamhack-1.0.1/
--rw-r--r--   0 runner    (1000) runner    (1000)      667 2024-05-09 14:41:32.763700 dreamhack-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 14:41:32.763700 dreamhack-1.0.1/dreamhack/
--rw-r--r--   0 runner    (1000) runner    (1000)      198 2024-05-09 14:39:32.000000 dreamhack-1.0.1/dreamhack/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      865 2024-05-09 14:39:14.000000 dreamhack-1.0.1/dreamhack/colorcodes.py
--rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-05-09 14:40:04.000000 dreamhack-1.0.1/dreamhack/encryption.py
--rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-05-09 14:39:58.000000 dreamhack-1.0.1/dreamhack/logging.py
--rw-r--r--   0 runner    (1000) runner    (1000)      923 2024-05-09 13:41:32.000000 dreamhack-1.0.1/dreamhack/windows.py
--rw-r--r--   0 runner    (1000) runner    (1000)      863 2024-05-09 13:40:58.000000 dreamhack-1.0.1/dreamhack/zipfiles.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 14:41:32.763700 dreamhack-1.0.1/dreamhack.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      667 2024-05-09 14:41:32.000000 dreamhack-1.0.1/dreamhack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      306 2024-05-09 14:41:32.000000 dreamhack-1.0.1/dreamhack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-09 14:41:32.000000 dreamhack-1.0.1/dreamhack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-05-09 14:41:32.000000 dreamhack-1.0.1/dreamhack.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-09 14:41:32.000000 dreamhack-1.0.1/dreamhack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-09 14:41:32.763700 dreamhack-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      965 2024-05-09 14:41:10.000000 dreamhack-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 17:10:03.105242 dreamhack-1.0.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)      904 2024-05-09 17:10:03.105242 dreamhack-1.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 17:10:03.097242 dreamhack-1.0.2/dreamhack/
+-rw-r--r--   0 runner    (1000) runner    (1000)      506 2024-05-09 17:00:39.000000 dreamhack-1.0.2/dreamhack/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      865 2024-05-09 14:39:14.000000 dreamhack-1.0.2/dreamhack/colorcodes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2599 2024-05-09 16:57:17.000000 dreamhack-1.0.2/dreamhack/encryption.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-05-09 14:39:58.000000 dreamhack-1.0.2/dreamhack/logging.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1243 2024-05-09 17:07:51.000000 dreamhack-1.0.2/dreamhack/networking.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      923 2024-05-09 13:41:32.000000 dreamhack-1.0.2/dreamhack/windows.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      892 2024-05-09 14:50:05.000000 dreamhack-1.0.2/dreamhack/zipfiles.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 17:10:03.105242 dreamhack-1.0.2/dreamhack.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      904 2024-05-09 17:10:02.000000 dreamhack-1.0.2/dreamhack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      330 2024-05-09 17:10:02.000000 dreamhack-1.0.2/dreamhack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-09 17:10:02.000000 dreamhack-1.0.2/dreamhack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       44 2024-05-09 17:10:02.000000 dreamhack-1.0.2/dreamhack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-09 17:10:02.000000 dreamhack-1.0.2/dreamhack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-09 17:10:03.105242 dreamhack-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1184 2024-05-09 17:09:45.000000 dreamhack-1.0.2/setup.py
```

### Comparing `dreamhack-1.0.1/dreamhack/colorcodes.py` & `dreamhack-1.0.2/dreamhack/colorcodes.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.1/dreamhack/windows.py` & `dreamhack-1.0.2/dreamhack/windows.py`

 * *Files identical despite different names*

### Comparing `dreamhack-1.0.1/dreamhack/zipfiles.py` & `dreamhack-1.0.2/dreamhack/zipfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 class zipfiles():
   def crack_using_wordlist(zip_file, wordlist_path): #type:ignore
     from tqdm import tqdm
     import zipfile
-    import colorcodes
+    from .colorcodes import colorcodes
     import os
     #type:ignore
     if not os.path.exists(wordlist_path):
-        raise FileNotFoundError(colorcodes.red('Invalid Wordlist Path.'))
+        raise FileNotFoundError(colorcodes.red('Invalid Wordlist Path.'))#type:ignore
     zip_file = zipfile.ZipFile(zip_file) #type:ignore
     n_words = len(list(open(wordlist_path, "rb")))
     print("Total passwords to test:", n_words)
     with open(wordlist_path, "rb") as wordlist:
         for word in tqdm(wordlist, total=n_words, unit="word"):
             try:
                 zip_file.extractall(pwd=word.strip())
```

### Comparing `dreamhack-1.0.1/setup.py` & `dreamhack-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.1' 
+VERSION = '1.0.2' 
 DESCRIPTION = 'The ultimate PyPi package for cyber-security and many other things.'
 LONG_DESCRIPTION = '''The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
 RELEASE NOTES: \n
+v1.0.2: \n
+- First official stable version, DO NOT USE PREVIOUS VERSIONS \n
+- Added content to encryption and logging \n
+- Created networking \n
+
+v1.0.1: \n
+- Fixed critical error from v1.0.1 \n
+- Working on new version \n
+
 v1.0.0: \n
 - Initial release \n
-- NOTE: Encryption and logging are both empty for this first version. \n
-- v1.0.1 coming very soon. \n
+- NOTE: Encryption and logging are both empty for the first few versions. \n
 '''
 
 # Setting up
 setup(
         name="dreamhack", 
         version=VERSION,
         author="Jack Burr",
         author_email="BurrJ22@Outlook.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['cryptography', 'tqdm', 'setuptools'], 
+        install_requires=['cryptography', 'tqdm', 'setuptools', 'pyuac', 'requests'], 
         keywords=['python', 'windows'],
         classifiers= [
             "Programming Language :: Python :: 3",
             "Operating System :: Microsoft :: Windows",
         ]
 )
```

