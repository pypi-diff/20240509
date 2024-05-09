# Comparing `tmp/PFlowC-1.4.3.tar.gz` & `tmp/PFlowC-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PFlowC-1.4.3.tar", last modified: Sun Apr 28 10:51:14 2024, max compression
+gzip compressed data, was "PFlowC-1.4.4.tar", last modified: Sun Apr 28 10:53:40 2024, max compression
```

## Comparing `PFlowC-1.4.3.tar` & `PFlowC-1.4.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:51:14.557149 PFlowC-1.4.3/
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:51:14.554326 PFlowC-1.4.3/PFlowC/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 10:39:09.000000 PFlowC-1.4.3/PFlowC/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     6067 2024-04-28 10:41:10.000000 PFlowC-1.4.3/PFlowC/main.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-1.4.3/PFlowC/proxy.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:51:14.555450 PFlowC-1.4.3/PFlowC/proxy_helper/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-26 04:34:38.000000 PFlowC-1.4.3/PFlowC/proxy_helper/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     5857 2024-04-28 09:32:36.000000 PFlowC-1.4.3/PFlowC/proxy_helper/macosx.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:51:14.556131 PFlowC-1.4.3/PFlowC/utils/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-1.4.3/PFlowC/utils/__init__.py
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-1.4.3/PFlowC/utils/logger.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:51:14.555154 PFlowC-1.4.3/PFlowC.egg-info/
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1443 2024-04-28 10:51:14.000000 PFlowC-1.4.3/PFlowC.egg-info/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      382 2024-04-28 10:51:14.000000 PFlowC-1.4.3/PFlowC.egg-info/SOURCES.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 10:51:14.000000 PFlowC-1.4.3/PFlowC.egg-info/dependency_links.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-04-28 10:51:14.000000 PFlowC-1.4.3/PFlowC.egg-info/entry_points.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       15 2024-04-28 10:51:14.000000 PFlowC-1.4.3/PFlowC.egg-info/requires.txt
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-04-28 10:51:14.000000 PFlowC-1.4.3/PFlowC.egg-info/top_level.txt
--rw-r--r--   0 shadikesadamu   (501) staff       (20)     1443 2024-04-28 10:51:14.556939 PFlowC-1.4.3/PKG-INFO
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      483 2024-04-28 10:51:03.000000 PFlowC-1.4.3/README.rst
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 10:51:14.557189 PFlowC-1.4.3/setup.cfg
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1634 2024-04-28 10:39:18.000000 PFlowC-1.4.3/setup.py
-drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:51:14.556464 PFlowC-1.4.3/tests/
--rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      765 2024-04-28 10:17:38.000000 PFlowC-1.4.3/tests/test-banner.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:53:40.470011 PFlowC-1.4.4/
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:53:40.467629 PFlowC-1.4.4/PFlowC/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 10:53:34.000000 PFlowC-1.4.4/PFlowC/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     6067 2024-04-28 10:41:10.000000 PFlowC-1.4.4/PFlowC/main.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      722 2024-04-28 09:32:05.000000 PFlowC-1.4.4/PFlowC/proxy.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:53:40.468720 PFlowC-1.4.4/PFlowC/proxy_helper/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      197 2024-04-26 04:34:38.000000 PFlowC-1.4.4/PFlowC/proxy_helper/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     5857 2024-04-28 09:32:36.000000 PFlowC-1.4.4/PFlowC/proxy_helper/macosx.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:53:40.469148 PFlowC-1.4.4/PFlowC/utils/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      196 2024-04-26 04:14:18.000000 PFlowC-1.4.4/PFlowC/utils/__init__.py
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1886 2024-04-28 09:12:11.000000 PFlowC-1.4.4/PFlowC/utils/logger.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:53:40.468416 PFlowC-1.4.4/PFlowC.egg-info/
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     2625 2024-04-28 10:53:40.000000 PFlowC-1.4.4/PFlowC.egg-info/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      382 2024-04-28 10:53:40.000000 PFlowC-1.4.4/PFlowC.egg-info/SOURCES.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        1 2024-04-28 10:53:40.000000 PFlowC-1.4.4/PFlowC.egg-info/dependency_links.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       77 2024-04-28 10:53:40.000000 PFlowC-1.4.4/PFlowC.egg-info/entry_points.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       15 2024-04-28 10:53:40.000000 PFlowC-1.4.4/PFlowC.egg-info/requires.txt
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)        7 2024-04-28 10:53:40.000000 PFlowC-1.4.4/PFlowC.egg-info/top_level.txt
+-rw-r--r--   0 shadikesadamu   (501) staff       (20)     2625 2024-04-28 10:53:40.469822 PFlowC-1.4.4/PKG-INFO
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1665 2024-04-28 10:53:21.000000 PFlowC-1.4.4/README.rst
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)       38 2024-04-28 10:53:40.470053 PFlowC-1.4.4/setup.cfg
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)     1634 2024-04-28 10:53:29.000000 PFlowC-1.4.4/setup.py
+drwxrwxrwx   0 shadikesadamu   (501) staff       (20)        0 2024-04-28 10:53:40.469501 PFlowC-1.4.4/tests/
+-rw-rw-rw-   0 shadikesadamu   (501) staff       (20)      765 2024-04-28 10:17:38.000000 PFlowC-1.4.4/tests/test-banner.py
```

### Comparing `PFlowC-1.4.3/PFlowC/main.py` & `PFlowC-1.4.4/PFlowC/main.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.3/PFlowC/proxy.py` & `PFlowC-1.4.4/PFlowC/proxy.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.3/PFlowC/proxy_helper/macosx.py` & `PFlowC-1.4.4/PFlowC/proxy_helper/macosx.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.3/PFlowC/utils/logger.py` & `PFlowC-1.4.4/PFlowC/utils/logger.py`

 * *Files identical despite different names*

### Comparing `PFlowC-1.4.3/setup.py` & `PFlowC-1.4.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 except ImportError:
     from distutils.core import setup
 
 long_description = open('README.rst').read()
 
 setup(
     name='PFlowC',
-    version='1.4.3',
+    version='1.4.4',
     url='https://github.com/Haoke98/FlowPilot',
     author='Haoke98',
     author_email='BlackHaoke<Haoke98@outlook.com>',
     license='MIT',
     description='https://github.com/Haoke98/FlowPilot/README.md',
     packages=["PFlowC", "PFlowC.utils", "PFlowC.proxy_helper"],
     install_requires=['colorlog', 'click'],
```

### Comparing `PFlowC-1.4.3/tests/test-banner.py` & `PFlowC-1.4.4/tests/test-banner.py`

 * *Files identical despite different names*

