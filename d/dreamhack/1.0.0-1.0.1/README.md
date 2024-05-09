# Comparing `tmp/dreamhack-1.0.0.tar.gz` & `tmp/dreamhack-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamhack-1.0.0.tar", last modified: Thu May  9 12:28:08 2024, max compression
+gzip compressed data, was "dreamhack-1.0.1.tar", last modified: Thu May  9 14:41:32 2024, max compression
```

## Comparing `dreamhack-1.0.0.tar` & `dreamhack-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 12:28:08.117922 dreamhack-1.0.0/
--rw-r--r--   0 runner    (1000) runner    (1000)      657 2024-05-09 12:28:08.117922 dreamhack-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 12:28:08.113922 dreamhack-1.0.0/dreamhack/
--rw-r--r--   0 runner    (1000) runner    (1000)      121 2024-05-09 01:04:16.000000 dreamhack-1.0.0/dreamhack/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      691 2024-05-09 01:04:26.000000 dreamhack-1.0.0/dreamhack/colorcodes.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-05-09 01:04:34.000000 dreamhack-1.0.0/dreamhack/encryption.py
--rw-r--r--   0 runner    (1000) runner    (1000)        0 2024-05-09 01:04:15.000000 dreamhack-1.0.0/dreamhack/logging.py
--rw-r--r--   0 runner    (1000) runner    (1000)      801 2024-05-09 01:04:10.000000 dreamhack-1.0.0/dreamhack/windows.py
--rw-r--r--   0 runner    (1000) runner    (1000)      760 2024-05-09 01:04:36.000000 dreamhack-1.0.0/dreamhack/zipfiles.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 12:28:08.117922 dreamhack-1.0.0/dreamhack.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      657 2024-05-09 12:28:07.000000 dreamhack-1.0.0/dreamhack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      306 2024-05-09 12:28:07.000000 dreamhack-1.0.0/dreamhack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-09 12:28:07.000000 dreamhack-1.0.0/dreamhack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-05-09 12:28:07.000000 dreamhack-1.0.0/dreamhack.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-09 12:28:07.000000 dreamhack-1.0.0/dreamhack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-09 12:28:08.117922 dreamhack-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      950 2024-05-09 12:26:10.000000 dreamhack-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 14:41:32.763700 dreamhack-1.0.1/
+-rw-r--r--   0 runner    (1000) runner    (1000)      667 2024-05-09 14:41:32.763700 dreamhack-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 14:41:32.763700 dreamhack-1.0.1/dreamhack/
+-rw-r--r--   0 runner    (1000) runner    (1000)      198 2024-05-09 14:39:32.000000 dreamhack-1.0.1/dreamhack/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      865 2024-05-09 14:39:14.000000 dreamhack-1.0.1/dreamhack/colorcodes.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       26 2024-05-09 14:40:04.000000 dreamhack-1.0.1/dreamhack/encryption.py
+-rw-r--r--   0 runner    (1000) runner    (1000)       23 2024-05-09 14:39:58.000000 dreamhack-1.0.1/dreamhack/logging.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      923 2024-05-09 13:41:32.000000 dreamhack-1.0.1/dreamhack/windows.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      863 2024-05-09 13:40:58.000000 dreamhack-1.0.1/dreamhack/zipfiles.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-09 14:41:32.763700 dreamhack-1.0.1/dreamhack.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      667 2024-05-09 14:41:32.000000 dreamhack-1.0.1/dreamhack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      306 2024-05-09 14:41:32.000000 dreamhack-1.0.1/dreamhack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-09 14:41:32.000000 dreamhack-1.0.1/dreamhack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       29 2024-05-09 14:41:32.000000 dreamhack-1.0.1/dreamhack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       10 2024-05-09 14:41:32.000000 dreamhack-1.0.1/dreamhack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-09 14:41:32.763700 dreamhack-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      965 2024-05-09 14:41:10.000000 dreamhack-1.0.1/setup.py
```

### Comparing `dreamhack-1.0.0/PKG-INFO` & `dreamhack-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.0
+Version: 1.0.1
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
 Requires-Dist: tqdm
 Requires-Dist: setuptools
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
-RELEASE NOTES:
-v1.0.0:
-- Initial release
-- NOTE: Encryption and logging are both empty for this first version.
-- v1.0.1 coming very soon.
+RELEASE NOTES: 
+
+v1.0.0: 
+
+- Initial release 
+
+- NOTE: Encryption and logging are both empty for this first version. 
+
+- v1.0.1 coming very soon. 
+
```

### Comparing `dreamhack-1.0.0/dreamhack/windows.py` & `dreamhack-1.0.1/dreamhack/windows.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
+class windows():
+  def create_windows_account(username, password): #type:ignore
+    import subprocess
+    command = f"net user {username} {password} /add /Y"
+    try:
+      subprocess.run(command, shell=False, check=True)
+    except Exception as e: 
+      raise e
+    else:
+      return username, password
 
-def create_windows_account(username, password):
-  import subprocess
-  command = f"net user {username} {password} /add /Y"
-  try:
-    subprocess.run(command, shell=False, check=True)
-  except Exception as e: 
-    raise e
-  else:
-    return username, password
-
-def multi_account_create(accounts, username=None, password=None):
-  def random_string_generator(length):
-    import random
-    characters = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
-    master = ""
-    for x in range(int(length)):
-      master = master + random.choice(characters)
-    return master
-  for x in range(int(accounts)):
-    if username is None:
-      username = random_string_generator(14)
-    if password is None:
-      password = random_string_generator(14)
-    create_windows_account(username, password)
+  def multi_account_create(accounts, username=None, password=None): #type:ignore
+    def random_string_generator(length):
+      import random
+      characters = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789"
+      master = ""
+      for x in range(int(length)):
+        master = master + random.choice(characters)
+      return master
+    for x in range(int(accounts)): #type:ignore
+      if username is None:
+        username = random_string_generator(14)
+      if password is None:
+        password = random_string_generator(14)
+      windows.create_windows_account(username, password) #type:ignore
```

### Comparing `dreamhack-1.0.0/dreamhack/zipfiles.py` & `dreamhack-1.0.1/dreamhack/zipfiles.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-def crack_using_wordlist(zip_file, wordlist_path):
-  from tqdm import tqdm
-  import zipfile
-  import colorcodes
-  import os
-  #type:ignore
-  if not os.path.exists(wordlist_path):
-    raise FileNotFoundError(colorcodes.red('Invalid Wordlist Path.'))
-    
-  zip_file = zipfile.ZipFile(zip_file)
-  n_words = len(list(open(wordlist_path, "rb")))
-  print("Total passwords to test:", n_words)
-  with open(wordlist_path, "rb") as wordlist:
-    for word in tqdm(wordlist, total=n_words, unit="word"):
-        try:
-            zip_file.extractall(pwd=word.strip())
-        except Exception:
-            continue
-        else:
-            print("[+] Password found:", word.decode().strip())
-            exit(0)
-    print("[!] Password not found, try other wordlist.")
+class zipfiles():
+  def crack_using_wordlist(zip_file, wordlist_path): #type:ignore
+    from tqdm import tqdm
+    import zipfile
+    import colorcodes
+    import os
+    #type:ignore
+    if not os.path.exists(wordlist_path):
+        raise FileNotFoundError(colorcodes.red('Invalid Wordlist Path.'))
+    zip_file = zipfile.ZipFile(zip_file) #type:ignore
+    n_words = len(list(open(wordlist_path, "rb")))
+    print("Total passwords to test:", n_words)
+    with open(wordlist_path, "rb") as wordlist:
+        for word in tqdm(wordlist, total=n_words, unit="word"):
+            try:
+                zip_file.extractall(pwd=word.strip())
+            except Exception:
+                continue
+            else:
+                print("[+] Password found:", word.decode().strip())
+                exit(0)
+        print("[!] Password not found, try other wordlist.")
+
+
```

### Comparing `dreamhack-1.0.0/dreamhack.egg-info/PKG-INFO` & `dreamhack-1.0.1/dreamhack.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: dreamhack
-Version: 1.0.0
+Version: 1.0.1
 Summary: The ultimate PyPi package for cyber-security and many other things.
 Author: Jack Burr
 Author-email: BurrJ22@Outlook.com
 Keywords: python,windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: cryptography
 Requires-Dist: tqdm
 Requires-Dist: setuptools
 
 The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
-RELEASE NOTES:
-v1.0.0:
-- Initial release
-- NOTE: Encryption and logging are both empty for this first version.
-- v1.0.1 coming very soon.
+RELEASE NOTES: 
+
+v1.0.0: 
+
+- Initial release 
+
+- NOTE: Encryption and logging are both empty for this first version. 
+
+- v1.0.1 coming very soon. 
+
```

### Comparing `dreamhack-1.0.0/setup.py` & `dreamhack-1.0.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0' 
+VERSION = '1.0.1' 
 DESCRIPTION = 'The ultimate PyPi package for cyber-security and many other things.'
 LONG_DESCRIPTION = '''The ultimate PyPi package for cyber-security, encryption, and many other things to simplify your code and make more advanced programs.
 
-RELEASE NOTES:
-v1.0.0:
-- Initial release
-- NOTE: Encryption and logging are both empty for this first version.
-- v1.0.1 coming very soon.
+RELEASE NOTES: \n
+v1.0.0: \n
+- Initial release \n
+- NOTE: Encryption and logging are both empty for this first version. \n
+- v1.0.1 coming very soon. \n
 '''
 
 # Setting up
 setup(
         name="dreamhack", 
         version=VERSION,
         author="Jack Burr",
```

