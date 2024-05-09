# Comparing `tmp/azure_simple_email-0.1.0.tar.gz` & `tmp/azure_simple_email-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure_simple_email-0.1.0.tar", last modified: Wed Apr 17 06:21:33 2024, max compression
+gzip compressed data, was "azure_simple_email-0.1.1.tar", last modified: Thu May  9 09:57:14 2024, max compression
```

## Comparing `azure_simple_email-0.1.0.tar` & `azure_simple_email-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:21:33.459202 azure_simple_email-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-17 06:21:22.000000 azure_simple_email-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-17 06:21:33.459202 azure_simple_email-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-17 06:21:22.000000 azure_simple_email-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:21:33.459202 azure_simple_email-0.1.0/azure_simple_email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:21:22.000000 azure_simple_email-0.1.0/azure_simple_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3152 2024-04-17 06:21:22.000000 azure_simple_email-0.1.0/azure_simple_email/azure_mail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:21:33.459202 azure_simple_email-0.1.0/azure_simple_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-17 06:21:33.000000 azure_simple_email-0.1.0/azure_simple_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-17 06:21:33.000000 azure_simple_email-0.1.0/azure_simple_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:21:33.000000 azure_simple_email-0.1.0/azure_simple_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 06:21:33.000000 azure_simple_email-0.1.0/azure_simple_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-17 06:21:33.000000 azure_simple_email-0.1.0/azure_simple_email.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:21:33.459202 azure_simple_email-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-17 06:21:22.000000 azure_simple_email-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:57:14.344980 azure_simple_email-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-09 09:57:05.000000 azure_simple_email-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-09 09:57:14.344980 azure_simple_email-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-09 09:57:05.000000 azure_simple_email-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:57:14.340980 azure_simple_email-0.1.1/azure_simple_email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:57:05.000000 azure_simple_email-0.1.1/azure_simple_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-09 09:57:05.000000 azure_simple_email-0.1.1/azure_simple_email/azure_mail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:57:14.344980 azure_simple_email-0.1.1/azure_simple_email.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-09 09:57:14.000000 azure_simple_email-0.1.1/azure_simple_email.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 09:57:14.000000 azure_simple_email-0.1.1/azure_simple_email.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:57:14.000000 azure_simple_email-0.1.1/azure_simple_email.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 09:57:14.000000 azure_simple_email-0.1.1/azure_simple_email.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-09 09:57:14.000000 azure_simple_email-0.1.1/azure_simple_email.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:57:14.344980 azure_simple_email-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-09 09:57:05.000000 azure_simple_email-0.1.1/setup.py
```

### Comparing `azure_simple_email-0.1.0/LICENSE` & `azure_simple_email-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `azure_simple_email-0.1.0/PKG-INFO` & `azure_simple_email-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure_simple_email
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is an esperimental library to send email using Microsoft Graph API
 Home-page: https://github.com/marcotn/azure_simple_email
 Author: Marco Pavanelli
 Author-email: marco.pavanelli@sasabz.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,12 +28,12 @@
 
 Moreover to send an email you need to have a valid Microsoft email account inside the organization 
 
 The you call instantiate AzureSendEmail passing the sender's email as paramenter
 
 this is the example that I have tested here of course with different email address.
 
-azure_email = AzureSendMail(user_id='service@example.com')
+`azure_email = AzureSendMail(user_id='service@example.com')
 azure_email.add_recipient('marco@test.com')
 azure_email.add_attachment('../README.md')
 azure_email.send_email(subject='test message', text='Hi, we are testing this python tool')
-
+`
```

### Comparing `azure_simple_email-0.1.0/README.md` & `azure_simple_email-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 
 Moreover to send an email you need to have a valid Microsoft email account inside the organization 
 
 The you call instantiate AzureSendEmail passing the sender's email as paramenter
 
 this is the example that I have tested here of course with different email address.
 
-azure_email = AzureSendMail(user_id='service@example.com')
+`azure_email = AzureSendMail(user_id='service@example.com')
 azure_email.add_recipient('marco@test.com')
 azure_email.add_attachment('../README.md')
 azure_email.send_email(subject='test message', text='Hi, we are testing this python tool')
-
+`
```

### Comparing `azure_simple_email-0.1.0/azure_simple_email.egg-info/PKG-INFO` & `azure_simple_email-0.1.1/azure_simple_email.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure_simple_email
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is an esperimental library to send email using Microsoft Graph API
 Home-page: https://github.com/marcotn/azure_simple_email
 Author: Marco Pavanelli
 Author-email: marco.pavanelli@sasabz.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,12 +28,12 @@
 
 Moreover to send an email you need to have a valid Microsoft email account inside the organization 
 
 The you call instantiate AzureSendEmail passing the sender's email as paramenter
 
 this is the example that I have tested here of course with different email address.
 
-azure_email = AzureSendMail(user_id='service@example.com')
+`azure_email = AzureSendMail(user_id='service@example.com')
 azure_email.add_recipient('marco@test.com')
 azure_email.add_attachment('../README.md')
 azure_email.send_email(subject='test message', text='Hi, we are testing this python tool')
-
+`
```

### Comparing `azure_simple_email-0.1.0/setup.py` & `azure_simple_email-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="azure_simple_email",
-    version="0.1.0",
+    version="0.1.1",
     author="Marco Pavanelli",
     author_email="marco.pavanelli@sasabz.it",
     description="This is an esperimental library to send email using Microsoft Graph API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/marcotn/azure_simple_email",
     packages=setuptools.find_packages(),
```

