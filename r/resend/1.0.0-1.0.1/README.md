# Comparing `tmp/resend-1.0.0.tar.gz` & `tmp/resend-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resend-1.0.0.tar", last modified: Thu May  9 01:40:50 2024, max compression
+gzip compressed data, was "resend-1.0.1.tar", last modified: Thu May  9 02:27:02 2024, max compression
```

## Comparing `resend-1.0.0.tar` & `resend-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,43 @@
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 01:40:50.684505 resend-1.0.0/
--rw-r--r--   0 derich     (501) staff       (20)     1070 2023-08-19 17:45:00.000000 resend-1.0.0/LICENSE.md
--rw-r--r--   0 derich     (501) staff       (20)     2408 2024-05-09 01:40:50.684424 resend-1.0.0/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)     1605 2024-05-09 01:36:14.000000 resend-1.0.0/README.md
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 01:40:50.683156 resend-1.0.0/resend/
--rw-r--r--   0 derich     (501) staff       (20)      743 2024-05-09 01:36:14.000000 resend-1.0.0/resend/__init__.py
--rw-r--r--   0 derich     (501) staff       (20)     5985 2024-05-09 01:36:14.000000 resend-1.0.0/resend/exceptions.py
--rw-r--r--   0 derich     (501) staff       (20)     2331 2024-05-09 01:36:14.000000 resend-1.0.0/resend/request.py
--rw-r--r--   0 derich     (501) staff       (20)      133 2024-05-09 01:36:14.000000 resend-1.0.0/resend/version.py
-drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 01:40:50.683851 resend-1.0.0/resend.egg-info/
--rw-r--r--   0 derich     (501) staff       (20)     2408 2024-05-09 01:40:50.000000 resend-1.0.0/resend.egg-info/PKG-INFO
--rw-r--r--   0 derich     (501) staff       (20)      293 2024-05-09 01:40:50.000000 resend-1.0.0/resend.egg-info/SOURCES.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-09 01:40:50.000000 resend-1.0.0/resend.egg-info/dependency_links.txt
--rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-09 01:40:50.000000 resend-1.0.0/resend.egg-info/not-zip-safe
--rw-r--r--   0 derich     (501) staff       (20)       35 2024-05-09 01:40:50.000000 resend-1.0.0/resend.egg-info/requires.txt
--rw-r--r--   0 derich     (501) staff       (20)        7 2024-05-09 01:40:50.000000 resend-1.0.0/resend.egg-info/top_level.txt
--rw-r--r--   0 derich     (501) staff       (20)       67 2024-05-09 01:40:50.684681 resend-1.0.0/setup.cfg
--rw-r--r--   0 derich     (501) staff       (20)     1112 2023-08-19 17:45:00.000000 resend-1.0.0/setup.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.991140 resend-1.0.1/
+-rw-r--r--   0 derich     (501) staff       (20)     1070 2023-08-19 17:45:00.000000 resend-1.0.1/LICENSE.md
+-rw-r--r--   0 derich     (501) staff       (20)     2408 2024-05-09 02:27:02.991051 resend-1.0.1/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)     1605 2024-05-09 01:36:14.000000 resend-1.0.1/README.md
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.987158 resend-1.0.1/resend/
+-rw-r--r--   0 derich     (501) staff       (20)      743 2024-05-09 01:36:14.000000 resend-1.0.1/resend/__init__.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.988472 resend-1.0.1/resend/api_keys/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.1/resend/api_keys/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)      998 2024-05-09 01:36:14.000000 resend-1.0.1/resend/api_keys/_api_key.py
+-rw-r--r--   0 derich     (501) staff       (20)     2310 2024-05-09 01:36:14.000000 resend-1.0.1/resend/api_keys/_api_keys.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.988907 resend-1.0.1/resend/audiences/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.1/resend/audiences/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     1192 2024-05-09 01:36:14.000000 resend-1.0.1/resend/audiences/_audience.py
+-rw-r--r--   0 derich     (501) staff       (20)     2305 2024-05-09 01:36:14.000000 resend-1.0.1/resend/audiences/_audiences.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.989311 resend-1.0.1/resend/contacts/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.1/resend/contacts/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     1795 2024-05-09 01:36:14.000000 resend-1.0.1/resend/contacts/_contact.py
+-rw-r--r--   0 derich     (501) staff       (20)     4400 2024-05-09 01:36:14.000000 resend-1.0.1/resend/contacts/_contacts.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.989829 resend-1.0.1/resend/domains/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.1/resend/domains/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)     1987 2024-05-09 01:36:14.000000 resend-1.0.1/resend/domains/_domain.py
+-rw-r--r--   0 derich     (501) staff       (20)     3887 2024-05-09 01:36:14.000000 resend-1.0.1/resend/domains/_domains.py
+-rw-r--r--   0 derich     (501) staff       (20)     1416 2024-05-09 01:36:14.000000 resend-1.0.1/resend/domains/_record.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.990781 resend-1.0.1/resend/emails/
+-rw-r--r--   0 derich     (501) staff       (20)        0 2024-05-09 01:36:14.000000 resend-1.0.1/resend/emails/__init__.py
+-rw-r--r--   0 derich     (501) staff       (20)      489 2024-05-09 01:36:14.000000 resend-1.0.1/resend/emails/_attachment.py
+-rw-r--r--   0 derich     (501) staff       (20)      755 2024-05-09 01:36:14.000000 resend-1.0.1/resend/emails/_batch.py
+-rw-r--r--   0 derich     (501) staff       (20)     2601 2024-05-09 01:36:14.000000 resend-1.0.1/resend/emails/_email.py
+-rw-r--r--   0 derich     (501) staff       (20)     2717 2024-05-09 01:36:14.000000 resend-1.0.1/resend/emails/_emails.py
+-rw-r--r--   0 derich     (501) staff       (20)      524 2024-05-09 01:36:14.000000 resend-1.0.1/resend/emails/_tag.py
+-rw-r--r--   0 derich     (501) staff       (20)     5985 2024-05-09 01:36:14.000000 resend-1.0.1/resend/exceptions.py
+-rw-r--r--   0 derich     (501) staff       (20)        0 2023-08-19 17:45:00.000000 resend-1.0.1/resend/py.typed
+-rw-r--r--   0 derich     (501) staff       (20)     2331 2024-05-09 01:36:14.000000 resend-1.0.1/resend/request.py
+-rw-r--r--   0 derich     (501) staff       (20)      133 2024-05-09 02:27:00.000000 resend-1.0.1/resend/version.py
+drwxr-xr-x   0 derich     (501) staff       (20)        0 2024-05-09 02:27:02.988020 resend-1.0.1/resend.egg-info/
+-rw-r--r--   0 derich     (501) staff       (20)     2408 2024-05-09 02:27:02.000000 resend-1.0.1/resend.egg-info/PKG-INFO
+-rw-r--r--   0 derich     (501) staff       (20)      825 2024-05-09 02:27:02.000000 resend-1.0.1/resend.egg-info/SOURCES.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-09 02:27:02.000000 resend-1.0.1/resend.egg-info/dependency_links.txt
+-rw-r--r--   0 derich     (501) staff       (20)        1 2024-05-09 02:15:39.000000 resend-1.0.1/resend.egg-info/not-zip-safe
+-rw-r--r--   0 derich     (501) staff       (20)       35 2024-05-09 02:27:02.000000 resend-1.0.1/resend.egg-info/requires.txt
+-rw-r--r--   0 derich     (501) staff       (20)        7 2024-05-09 02:27:02.000000 resend-1.0.1/resend.egg-info/top_level.txt
+-rw-r--r--   0 derich     (501) staff       (20)       67 2024-05-09 02:27:02.991731 resend-1.0.1/setup.cfg
+-rw-r--r--   0 derich     (501) staff       (20)     1171 2024-05-09 02:27:00.000000 resend-1.0.1/setup.py
```

### Comparing `resend-1.0.0/LICENSE.md` & `resend-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `resend-1.0.0/PKG-INFO` & `resend-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 1.0.0
+Version: 1.0.1
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 Keywords: email,email platform
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `resend-1.0.0/README.md` & `resend-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `resend-1.0.0/resend/__init__.py` & `resend-1.0.1/resend/__init__.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.0/resend/exceptions.py` & `resend-1.0.1/resend/exceptions.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.0/resend/request.py` & `resend-1.0.1/resend/request.py`

 * *Files identical despite different names*

### Comparing `resend-1.0.0/resend.egg-info/PKG-INFO` & `resend-1.0.1/resend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 1.0.0
+Version: 1.0.1
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 Keywords: email,email platform
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

