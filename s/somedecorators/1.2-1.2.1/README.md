# Comparing `tmp/somedecorators-1.2.tar.gz` & `tmp/somedecorators-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "somedecorators-1.2.tar", last modified: Thu Dec 21 00:43:54 2023, max compression
+gzip compressed data, was "somedecorators-1.2.1.tar", last modified: Thu May  9 06:38:45 2024, max compression
```

## Comparing `somedecorators-1.2.tar` & `somedecorators-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-12-21 00:43:54.224037 somedecorators-1.2/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1108 2023-11-17 06:58:43.000000 somedecorators-1.2/LICENSE
--rw-r--r--   0 aaron     (1000) aaron     (1000)     6718 2023-12-21 00:43:54.224037 somedecorators-1.2/PKG-INFO
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     5919 2023-12-21 00:42:55.000000 somedecorators-1.2/README.md
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       38 2023-12-21 00:43:54.224037 somedecorators-1.2/setup.cfg
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1957 2023-12-21 00:38:40.000000 somedecorators-1.2/setup.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-12-21 00:43:54.224037 somedecorators-1.2/somedecorators/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      151 2023-12-13 06:13:08.000000 somedecorators-1.2/somedecorators/__init__.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-12-21 00:43:54.224037 somedecorators-1.2/somedecorators/conf/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     8478 2023-12-13 06:34:22.000000 somedecorators-1.2/somedecorators/conf/__init__.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)    21956 2023-12-13 06:17:27.000000 somedecorators-1.2/somedecorators/conf/global_settings.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2330 2023-12-13 06:20:12.000000 somedecorators-1.2/somedecorators/email.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2056 2023-11-17 06:58:43.000000 somedecorators-1.2/somedecorators/retry.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1331 2023-11-17 06:58:43.000000 somedecorators-1.2/somedecorators/timeit.py
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     2786 2023-12-13 06:55:17.000000 somedecorators-1.2/somedecorators/wechat.py
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-12-21 00:43:54.224037 somedecorators-1.2/somedecorators.egg-info/
--rw-r--r--   0 aaron     (1000) aaron     (1000)     6718 2023-12-21 00:43:54.000000 somedecorators-1.2/somedecorators.egg-info/PKG-INFO
--rw-rw-r--   0 aaron     (1000) aaron     (1000)      426 2023-12-21 00:43:54.000000 somedecorators-1.2/somedecorators.egg-info/SOURCES.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)        1 2023-12-21 00:43:54.000000 somedecorators-1.2/somedecorators.egg-info/dependency_links.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       43 2023-12-21 00:43:54.000000 somedecorators-1.2/somedecorators.egg-info/requires.txt
--rw-rw-r--   0 aaron     (1000) aaron     (1000)       15 2023-12-21 00:43:54.000000 somedecorators-1.2/somedecorators.egg-info/top_level.txt
-drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2023-12-21 00:43:54.224037 somedecorators-1.2/tests/
--rw-rw-r--   0 aaron     (1000) aaron     (1000)     1902 2023-12-13 06:42:25.000000 somedecorators-1.2/tests/tests.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-09 06:38:45.115902 somedecorators-1.2.1/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1108 2023-11-17 06:58:43.000000 somedecorators-1.2.1/LICENSE
+-rw-r--r--   0 aaron     (1000) aaron     (1000)     6901 2024-05-09 06:38:45.111902 somedecorators-1.2.1/PKG-INFO
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     6100 2024-05-09 06:24:27.000000 somedecorators-1.2.1/README.md
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       38 2024-05-09 06:38:45.115902 somedecorators-1.2.1/setup.cfg
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1959 2024-05-09 06:24:52.000000 somedecorators-1.2.1/setup.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-09 06:38:45.107902 somedecorators-1.2.1/somedecorators/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      181 2024-05-09 06:21:29.000000 somedecorators-1.2.1/somedecorators/__init__.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-09 06:38:45.111902 somedecorators-1.2.1/somedecorators/conf/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     8478 2023-12-13 06:34:22.000000 somedecorators-1.2.1/somedecorators/conf/__init__.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)    21956 2023-12-13 06:17:27.000000 somedecorators-1.2.1/somedecorators/conf/global_settings.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     2330 2023-12-13 06:20:12.000000 somedecorators-1.2.1/somedecorators/email.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1571 2024-05-09 06:21:49.000000 somedecorators-1.2.1/somedecorators/log.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     2056 2023-11-17 06:58:43.000000 somedecorators-1.2.1/somedecorators/retry.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1331 2023-11-17 06:58:43.000000 somedecorators-1.2.1/somedecorators/timeit.py
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     2786 2023-12-13 06:55:17.000000 somedecorators-1.2.1/somedecorators/wechat.py
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-09 06:38:45.111902 somedecorators-1.2.1/somedecorators.egg-info/
+-rw-r--r--   0 aaron     (1000) aaron     (1000)     6901 2024-05-09 06:38:45.000000 somedecorators-1.2.1/somedecorators.egg-info/PKG-INFO
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)      448 2024-05-09 06:38:45.000000 somedecorators-1.2.1/somedecorators.egg-info/SOURCES.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)        1 2024-05-09 06:38:45.000000 somedecorators-1.2.1/somedecorators.egg-info/dependency_links.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       43 2024-05-09 06:38:45.000000 somedecorators-1.2.1/somedecorators.egg-info/requires.txt
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)       15 2024-05-09 06:38:45.000000 somedecorators-1.2.1/somedecorators.egg-info/top_level.txt
+drwxrwxr-x   0 aaron     (1000) aaron     (1000)        0 2024-05-09 06:38:45.111902 somedecorators-1.2.1/tests/
+-rw-rw-r--   0 aaron     (1000) aaron     (1000)     1902 2023-12-13 06:42:25.000000 somedecorators-1.2.1/tests/tests.py
```

### Comparing `somedecorators-1.2/LICENSE` & `somedecorators-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2/PKG-INFO` & `somedecorators-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somedecorators
-Version: 1.2
+Version: 1.2.1
 Summary: Some useful decorators in Python.
 Home-page: https://github.com/somenzz/somedecorators
 Author: somenzz
 Author-email: somenzz@163.com
 License: MIT
 Keywords: awesome decorators
 Classifier: Development Status :: 3 - Alpha
@@ -253,14 +253,23 @@
     elif args == 2:
         raise Exception2
     else:
         raise Exception3
 ```
 
 
+#### setup_logger
+
+一个简单的使用日志的方法
+
+```python
+from somedecorators import setup_logger
+logger = setup_logger("myapp")
+logger.info("hello this is myapp log")
+```
 
 
 ## 参与项目
 
 欢迎分享你最常用的装饰器，加入到这里。
```

### Comparing `somedecorators-1.2/README.md` & `somedecorators-1.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -230,14 +230,23 @@
     elif args == 2:
         raise Exception2
     else:
         raise Exception3
 ```
 
 
+#### setup_logger
+
+一个简单的使用日志的方法
+
+```python
+from somedecorators import setup_logger
+logger = setup_logger("myapp")
+logger.info("hello this is myapp log")
+```
 
 
 ## 参与项目
 
 欢迎分享你最常用的装饰器，加入到这里。
```

### Comparing `somedecorators-1.2/setup.py` & `somedecorators-1.2.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 readme = Path("README.md")
 license = Path("LICENSE")
 
 
 # Read the version without importing the package
 # (and thus attempting to import packages it depends on that may not be
 # installed yet)
-version = "1.2"
+version = "1.2.1"
 
 NAME = 'somedecorators'
 VERSION = version
 DESCRIPTION = 'Some useful decorators in Python.'
 KEYWORDS = 'awesome decorators'
 AUTHOR = 'somenzz'
 AUTHOR_EMAIL = 'somenzz@163.com'
```

### Comparing `somedecorators-1.2/somedecorators/conf/__init__.py` & `somedecorators-1.2.1/somedecorators/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2/somedecorators/conf/global_settings.py` & `somedecorators-1.2.1/somedecorators/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2/somedecorators/email.py` & `somedecorators-1.2.1/somedecorators/email.py`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2/somedecorators/retry.py` & `somedecorators-1.2.1/somedecorators/retry.py`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2/somedecorators/timeit.py` & `somedecorators-1.2.1/somedecorators/timeit.py`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2/somedecorators/wechat.py` & `somedecorators-1.2.1/somedecorators/wechat.py`

 * *Files identical despite different names*

### Comparing `somedecorators-1.2/somedecorators.egg-info/PKG-INFO` & `somedecorators-1.2.1/somedecorators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: somedecorators
-Version: 1.2
+Version: 1.2.1
 Summary: Some useful decorators in Python.
 Home-page: https://github.com/somenzz/somedecorators
 Author: somenzz
 Author-email: somenzz@163.com
 License: MIT
 Keywords: awesome decorators
 Classifier: Development Status :: 3 - Alpha
@@ -253,14 +253,23 @@
     elif args == 2:
         raise Exception2
     else:
         raise Exception3
 ```
 
 
+#### setup_logger
+
+一个简单的使用日志的方法
+
+```python
+from somedecorators import setup_logger
+logger = setup_logger("myapp")
+logger.info("hello this is myapp log")
+```
 
 
 ## 参与项目
 
 欢迎分享你最常用的装饰器，加入到这里。
```

### Comparing `somedecorators-1.2/tests/tests.py` & `somedecorators-1.2.1/tests/tests.py`

 * *Files identical despite different names*
