# Comparing `tmp/anabih_python_test-4.0.0.tar.gz` & `tmp/anabih_python_test-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anabih_python_test-4.0.0.tar", last modified: Thu May  9 02:56:22 2024, max compression
+gzip compressed data, was "anabih_python_test-5.0.0.tar", last modified: Thu May  9 14:36:21 2024, max compression
```

## Comparing `anabih_python_test-4.0.0.tar` & `anabih_python_test-5.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 02:56:22.947592 anabih_python_test-4.0.0/
--rw-rw-rw-   0        0        0      431 2024-05-09 02:56:22.946593 anabih_python_test-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       19 2024-05-09 00:01:05.000000 anabih_python_test-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 02:56:22.944593 anabih_python_test-4.0.0/anabih_python_test.egg-info/
--rw-rw-rw-   0        0        0      431 2024-05-09 02:56:22.000000 anabih_python_test-4.0.0/anabih_python_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-05-09 02:56:22.000000 anabih_python_test-4.0.0/anabih_python_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 02:56:22.000000 anabih_python_test-4.0.0/anabih_python_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 02:56:22.000000 anabih_python_test-4.0.0/anabih_python_test.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 02:56:22.943593 anabih_python_test-4.0.0/my_package/
--rw-rw-rw-   0        0        0        0 2024-05-09 02:56:07.000000 anabih_python_test-4.0.0/my_package/__init__.py
--rw-rw-rw-   0        0        0       30 2024-05-09 02:56:07.000000 anabih_python_test-4.0.0/my_package/greetings.py
--rw-rw-rw-   0        0        0       42 2024-05-09 02:56:22.947592 anabih_python_test-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0      657 2024-05-09 02:53:42.000000 anabih_python_test-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 14:36:21.677881 anabih_python_test-5.0.0/
+-rw-rw-rw-   0        0        0      431 2024-05-09 14:36:21.675880 anabih_python_test-5.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2024-05-09 00:01:05.000000 anabih_python_test-5.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 14:36:21.674881 anabih_python_test-5.0.0/anabih_python_test.egg-info/
+-rw-rw-rw-   0        0        0      431 2024-05-09 14:36:21.000000 anabih_python_test-5.0.0/anabih_python_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2024-05-09 14:36:21.000000 anabih_python_test-5.0.0/anabih_python_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 14:36:21.000000 anabih_python_test-5.0.0/anabih_python_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 14:36:21.000000 anabih_python_test-5.0.0/anabih_python_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 14:36:21.673881 anabih_python_test-5.0.0/my_package/
+-rw-rw-rw-   0        0        0        0 2024-05-09 03:08:34.000000 anabih_python_test-5.0.0/my_package/__init__.py
+-rw-rw-rw-   0        0        0       58 2024-05-09 14:36:05.000000 anabih_python_test-5.0.0/my_package/greetings.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 14:36:21.677881 anabih_python_test-5.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      657 2024-05-09 14:35:31.000000 anabih_python_test-5.0.0/setup.py
```

### Comparing `anabih_python_test-4.0.0/setup.py` & `anabih_python_test-5.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="anabih_python_test",
-    version="4.0.0",
+    version="5.0.0",
     author="Ahmed Nabih",
     author_email="anabih2000@yahoo.com",
     description="Python test",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/anabih/python-test",
     packages=setuptools.find_packages(),
```

