# Comparing `tmp/once-utils-0.0.6.tar.gz` & `tmp/once_utils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "once-utils-0.0.6.tar", last modified: Sat Jun 10 10:54:26 2023, max compression
+gzip compressed data, was "once_utils-0.0.7.tar", last modified: Thu May  9 07:06:26 2024, max compression
```

## Comparing `once-utils-0.0.6.tar` & `once_utils-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 10:54:26.915557 once-utils-0.0.6/
--rw-rw-rw-   0        0        0      852 2023-06-10 10:54:26.915557 once-utils-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       56 2022-09-25 12:18:04.000000 once-utils-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 10:54:26.890558 once-utils-0.0.6/once_utils.egg-info/
--rw-rw-rw-   0        0        0      852 2023-06-10 10:54:26.000000 once-utils-0.0.6/once_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-06-10 10:54:26.000000 once-utils-0.0.6/once_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 10:54:26.000000 once-utils-0.0.6/once_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-10 10:54:26.000000 once-utils-0.0.6/once_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-10 10:54:26.905573 once-utils-0.0.6/onceutils/
--rw-rw-rw-   0        0        0      184 2023-04-16 05:52:44.000000 once-utils-0.0.6/onceutils/__init__.py
--rw-rw-rw-   0        0        0     3805 2023-06-04 14:37:47.000000 once-utils-0.0.6/onceutils/_cmd.py
--rw-rw-rw-   0        0        0     1115 2022-09-10 06:29:17.000000 once-utils-0.0.6/onceutils/_convert.py
--rw-rw-rw-   0        0        0      436 2022-09-24 05:27:27.000000 once-utils-0.0.6/onceutils/_iter.py
--rw-rw-rw-   0        0        0      629 2022-08-26 16:47:36.000000 once-utils-0.0.6/onceutils/_pymodule.py
--rw-rw-rw-   0        0        0     6652 2022-09-25 11:20:31.000000 once-utils-0.0.6/onceutils/_random.py
--rw-rw-rw-   0        0        0      618 2022-09-24 13:55:11.000000 once-utils-0.0.6/onceutils/const.py
--rw-rw-rw-   0        0        0      322 2023-04-16 05:49:32.000000 once-utils-0.0.6/onceutils/ex_dict.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:54:26.909134 once-utils-0.0.6/onceutils/github/
--rw-rw-rw-   0        0        0        0 2022-08-28 14:34:38.000000 once-utils-0.0.6/onceutils/github/__init__.py
--rw-rw-rw-   0        0        0     4764 2022-08-29 14:40:26.000000 once-utils-0.0.6/onceutils/github/personal_token.py
-drwxrwxrwx   0        0        0        0 2023-06-10 10:54:26.913560 once-utils-0.0.6/onceutils/xjson/
--rw-rw-rw-   0        0        0      164 2023-06-10 10:01:41.000000 once-utils-0.0.6/onceutils/xjson/__init__.py
--rw-rw-rw-   0        0        0     1680 2023-06-10 10:00:10.000000 once-utils-0.0.6/onceutils/xjson/_common.py
--rw-rw-rw-   0        0        0     1048 2023-06-10 07:17:05.000000 once-utils-0.0.6/onceutils/xjson/encoder.py
--rw-rw-rw-   0        0        0       42 2023-06-10 10:54:26.916558 once-utils-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1216 2023-06-10 10:51:54.000000 once-utils-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:06:26.193040 once_utils-0.0.7/
+-rw-rw-rw-   0        0        0      904 2024-05-09 07:06:26.192043 once_utils-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       56 2023-05-31 06:32:04.000000 once_utils-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 07:06:26.191046 once_utils-0.0.7/once_utils.egg-info/
+-rw-rw-rw-   0        0        0      904 2024-05-09 07:06:26.000000 once_utils-0.0.7/once_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      640 2024-05-09 07:06:26.000000 once_utils-0.0.7/once_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 07:06:26.000000 once_utils-0.0.7/once_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-09 07:06:26.000000 once_utils-0.0.7/once_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 07:06:26.178084 once_utils-0.0.7/onceutils/
+-rw-rw-rw-   0        0        0      205 2024-05-09 06:11:26.000000 once_utils-0.0.7/onceutils/__init__.py
+-rw-rw-rw-   0        0        0     3805 2023-09-14 01:48:03.000000 once_utils-0.0.7/onceutils/_cmd.py
+-rw-rw-rw-   0        0        0     1115 2023-05-31 06:32:04.000000 once_utils-0.0.7/onceutils/_convert.py
+-rw-rw-rw-   0        0        0      436 2023-05-31 06:32:04.000000 once_utils-0.0.7/onceutils/_iter.py
+-rw-rw-rw-   0        0        0      629 2023-09-14 01:51:06.000000 once_utils-0.0.7/onceutils/_pymodule.py
+-rw-rw-rw-   0        0        0     6652 2023-05-31 06:32:04.000000 once_utils-0.0.7/onceutils/_random.py
+-rw-rw-rw-   0        0        0      618 2023-05-31 06:32:04.000000 once_utils-0.0.7/onceutils/const.py
+-rw-rw-rw-   0        0        0      322 2023-05-31 06:32:04.000000 once_utils-0.0.7/onceutils/ex_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:06:26.180075 once_utils-0.0.7/onceutils/github/
+-rw-rw-rw-   0        0        0        0 2023-05-31 06:32:04.000000 once_utils-0.0.7/onceutils/github/__init__.py
+-rw-rw-rw-   0        0        0     4764 2023-05-31 06:32:04.000000 once_utils-0.0.7/onceutils/github/personal_token.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:06:26.182073 once_utils-0.0.7/onceutils/http/
+-rw-rw-rw-   0        0        0       26 2024-05-09 06:12:09.000000 once_utils-0.0.7/onceutils/http/__init__.py
+-rw-rw-rw-   0        0        0     4414 2024-05-09 04:05:46.000000 once_utils-0.0.7/onceutils/http/_http_raw.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:06:26.185063 once_utils-0.0.7/onceutils/xjson/
+-rw-rw-rw-   0        0        0      187 2024-05-09 03:59:38.000000 once_utils-0.0.7/onceutils/xjson/__init__.py
+-rw-rw-rw-   0        0        0     1680 2023-09-14 01:41:49.000000 once_utils-0.0.7/onceutils/xjson/_common.py
+-rw-rw-rw-   0        0        0     1048 2023-09-14 01:41:49.000000 once_utils-0.0.7/onceutils/xjson/encoder.py
+-rw-rw-rw-   0        0        0       42 2024-05-09 07:06:26.193040 once_utils-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1267 2024-05-09 06:16:33.000000 once_utils-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:06:26.190048 once_utils-0.0.7/tests/
+-rw-rw-rw-   0        0        0      662 2023-09-14 01:41:49.000000 once_utils-0.0.7/tests/test_cmd.py
+-rw-rw-rw-   0        0        0      245 2023-05-31 06:32:04.000000 once_utils-0.0.7/tests/test_dict.py
+-rw-rw-rw-   0        0        0      624 2024-05-09 06:12:42.000000 once_utils-0.0.7/tests/test_http_raw.py
+-rw-rw-rw-   0        0        0      607 2023-05-31 06:32:04.000000 once_utils-0.0.7/tests/test_iter.py
+-rw-rw-rw-   0        0        0      866 2023-05-31 06:32:04.000000 once_utils-0.0.7/tests/test_random.py
+-rw-rw-rw-   0        0        0     1809 2023-09-14 01:41:49.000000 once_utils-0.0.7/tests/test_xjson.py
```

### Comparing `once-utils-0.0.6/PKG-INFO` & `once_utils-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: once-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simplest utils.
 Home-page: https://github.com/Mingyueyixi/once-utils
 Author: Lu
 Author-email: Mingyueyixi@hotmail.com
 License: MIT Licence
 Keywords: pip,once-utils
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 
 # once-utils
```

### Comparing `once-utils-0.0.6/once_utils.egg-info/PKG-INFO` & `once_utils-0.0.7/once_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: once-utils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simplest utils.
 Home-page: https://github.com/Mingyueyixi/once-utils
 Author: Lu
 Author-email: Mingyueyixi@hotmail.com
 License: MIT Licence
 Keywords: pip,once-utils
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 
 # once-utils
```

### Comparing `once-utils-0.0.6/onceutils/_cmd.py` & `once_utils-0.0.7/onceutils/_cmd.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.6/onceutils/_convert.py` & `once_utils-0.0.7/onceutils/_convert.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.6/onceutils/_pymodule.py` & `once_utils-0.0.7/onceutils/_pymodule.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.6/onceutils/_random.py` & `once_utils-0.0.7/onceutils/_random.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.6/onceutils/const.py` & `once_utils-0.0.7/onceutils/const.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.6/onceutils/github/personal_token.py` & `once_utils-0.0.7/onceutils/github/personal_token.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.6/onceutils/xjson/_common.py` & `once_utils-0.0.7/onceutils/xjson/_common.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.6/onceutils/xjson/encoder.py` & `once_utils-0.0.7/onceutils/xjson/encoder.py`

 * *Files identical despite different names*

### Comparing `once-utils-0.0.6/setup.py` & `once_utils-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,28 +9,29 @@
     with open(readme_md_path) as f:
         ret = f.read()
     return ret
 
 
 setup(
     name="once-utils",
-    version="0.0.6",
+    version="0.0.7",
     keywords=["pip", "once-utils"],
     description="Simplest utils.",
     long_description=readme_md(),
     long_description_content_type='text/markdown',
     license="MIT Licence",
     classifiers=[
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers'],
 
     url="https://github.com/Mingyueyixi/once-utils",
     author="Lu",
     author_email="Mingyueyixi@hotmail.com",
```

