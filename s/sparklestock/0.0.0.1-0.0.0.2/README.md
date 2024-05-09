# Comparing `tmp/sparklestock-0.0.0.1.tar.gz` & `tmp/sparklestock-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparklestock-0.0.0.1.tar", last modified: Wed May  8 13:56:59 2024, max compression
+gzip compressed data, was "sparklestock-0.0.0.2.tar", last modified: Wed May  8 14:20:28 2024, max compression
```

## Comparing `sparklestock-0.0.0.1.tar` & `sparklestock-0.0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-08 13:56:59.050400 sparklestock-0.0.0.1/
--rw-r--r--   0 seyong     (501) staff       (20)        0 2024-04-12 06:49:57.000000 sparklestock-0.0.0.1/LICENSE.txt
--rw-r--r--   0 seyong     (501) staff       (20)      465 2024-05-08 13:56:59.050479 sparklestock-0.0.0.1/PKG-INFO
--rw-r--r--   0 seyong     (501) staff       (20)       46 2024-05-08 13:10:42.000000 sparklestock-0.0.0.1/README.md
--rw-r--r--   0 seyong     (501) staff       (20)      270 2024-04-05 11:07:26.000000 sparklestock-0.0.0.1/pyproject.toml
--rw-r--r--   0 seyong     (501) staff       (20)       79 2024-05-08 13:56:59.050686 sparklestock-0.0.0.1/setup.cfg
--rw-r--r--   0 seyong     (501) staff       (20)      685 2024-05-08 13:53:27.000000 sparklestock-0.0.0.1/setup.py
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-08 13:56:59.049689 sparklestock-0.0.0.1/sparklestock/
--rw-r--r--   0 seyong     (501) staff       (20)     2034 2024-05-08 12:44:44.000000 sparklestock-0.0.0.1/sparklestock/Stock.py
--rw-r--r--   0 seyong     (501) staff       (20)       58 2024-05-08 13:55:13.000000 sparklestock-0.0.0.1/sparklestock/__init__.py
--rw-r--r--   0 seyong     (501) staff       (20)       23 2024-05-08 13:55:23.000000 sparklestock-0.0.0.1/sparklestock/__version__.py
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-08 13:56:59.050290 sparklestock-0.0.0.1/sparklestock.egg-info/
--rw-r--r--   0 seyong     (501) staff       (20)      465 2024-05-08 13:56:59.000000 sparklestock-0.0.0.1/sparklestock.egg-info/PKG-INFO
--rw-r--r--   0 seyong     (501) staff       (20)      274 2024-05-08 13:56:59.000000 sparklestock-0.0.0.1/sparklestock.egg-info/SOURCES.txt
--rw-r--r--   0 seyong     (501) staff       (20)        1 2024-05-08 13:56:59.000000 sparklestock-0.0.0.1/sparklestock.egg-info/dependency_links.txt
--rw-r--r--   0 seyong     (501) staff       (20)       13 2024-05-08 13:56:59.000000 sparklestock-0.0.0.1/sparklestock.egg-info/top_level.txt
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-08 14:20:28.175861 sparklestock-0.0.0.2/
+-rw-r--r--   0 seyong     (501) staff       (20)      439 2024-05-08 14:20:28.175936 sparklestock-0.0.0.2/PKG-INFO
+-rw-r--r--   0 seyong     (501) staff       (20)       46 2024-05-08 13:10:42.000000 sparklestock-0.0.0.2/README.md
+-rw-r--r--   0 seyong     (501) staff       (20)      270 2024-04-05 11:07:26.000000 sparklestock-0.0.0.2/pyproject.toml
+-rw-r--r--   0 seyong     (501) staff       (20)       79 2024-05-08 14:20:28.176132 sparklestock-0.0.0.2/setup.cfg
+-rw-r--r--   0 seyong     (501) staff       (20)      720 2024-05-08 14:19:05.000000 sparklestock-0.0.0.2/setup.py
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-08 14:20:28.174884 sparklestock-0.0.0.2/sparklestock/
+-rw-r--r--   0 seyong     (501) staff       (20)     2034 2024-05-08 12:44:44.000000 sparklestock-0.0.0.2/sparklestock/Stock.py
+-rw-r--r--   0 seyong     (501) staff       (20)       58 2024-05-08 13:55:13.000000 sparklestock-0.0.0.2/sparklestock/__init__.py
+-rw-r--r--   0 seyong     (501) staff       (20)       23 2024-05-08 14:19:05.000000 sparklestock-0.0.0.2/sparklestock/__version__.py
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-08 14:20:28.175738 sparklestock-0.0.0.2/sparklestock.egg-info/
+-rw-r--r--   0 seyong     (501) staff       (20)      439 2024-05-08 14:20:28.000000 sparklestock-0.0.0.2/sparklestock.egg-info/PKG-INFO
+-rw-r--r--   0 seyong     (501) staff       (20)      297 2024-05-08 14:20:28.000000 sparklestock-0.0.0.2/sparklestock.egg-info/SOURCES.txt
+-rw-r--r--   0 seyong     (501) staff       (20)        1 2024-05-08 14:20:28.000000 sparklestock-0.0.0.2/sparklestock.egg-info/dependency_links.txt
+-rw-r--r--   0 seyong     (501) staff       (20)        9 2024-05-08 14:20:28.000000 sparklestock-0.0.0.2/sparklestock.egg-info/requires.txt
+-rw-r--r--   0 seyong     (501) staff       (20)       13 2024-05-08 14:20:28.000000 sparklestock-0.0.0.2/sparklestock.egg-info/top_level.txt
```

### Comparing `sparklestock-0.0.0.1/setup.py` & `sparklestock-0.0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sparklestock", ## 소문자 영단어
-    version="0.0.0.1", ##
+    version="0.0.0.2", ##
     author="Seyong Ahn", ## ex) Sunkyeong Lee
     author_email="hiseyong1008@gmail.com", ##
     description="sparkle stock package", ##
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hiseyong", ##
+    install_requires=['requests'],
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3',
```

### Comparing `sparklestock-0.0.0.1/sparklestock/Stock.py` & `sparklestock-0.0.0.2/sparklestock/Stock.py`

 * *Files identical despite different names*

