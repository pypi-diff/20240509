# Comparing `tmp/sigmoid_check-0.0.7.tar.gz` & `tmp/sigmoid_check-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmoid_check-0.0.7.tar", last modified: Mon May  6 17:41:33 2024, max compression
+gzip compressed data, was "sigmoid_check-0.0.8.tar", last modified: Thu May  9 08:53:03 2024, max compression
```

## Comparing `sigmoid_check-0.0.7.tar` & `sigmoid_check-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 17:41:33.849909 sigmoid_check-0.0.7/
--rw-rw-rw-   0        0        0    11538 2024-04-23 18:15:46.000000 sigmoid_check-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     2756 2024-05-06 17:41:33.848886 sigmoid_check-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1881 2024-04-23 18:29:06.000000 sigmoid_check-0.0.7/README.md
--rw-rw-rw-   0        0        0       86 2024-05-06 17:41:33.851903 sigmoid_check-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1104 2024-05-06 17:41:05.000000 sigmoid_check-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:41:33.817110 sigmoid_check-0.0.7/sigmoid_check/
--rw-rw-rw-   0        0        0        0 2024-04-23 19:00:37.000000 sigmoid_check-0.0.7/sigmoid_check/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:41:33.831296 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/
--rw-rw-rw-   0        0        0      170 2024-05-05 08:15:26.000000 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:41:33.835295 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_10/
--rw-rw-rw-   0        0        0        0 2024-04-24 19:44:19.000000 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_10/__init__.py
--rw-rw-rw-   0        0        0    22558 2024-04-23 20:44:39.000000 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_10/lesson_10.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:41:33.838369 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_11/
--rw-rw-rw-   0        0        0        0 2024-04-24 19:44:19.000000 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_11/__init__.py
--rw-rw-rw-   0        0        0    41222 2024-04-24 20:20:21.000000 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_11/lesson_11.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:41:33.840894 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_13/
--rw-rw-rw-   0        0        0        0 2024-04-29 12:54:48.000000 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_13/__init__.py
--rw-rw-rw-   0        0        0    21468 2024-04-30 12:20:28.000000 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_13/lesson_13.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:41:33.843895 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_14/
--rw-rw-rw-   0        0        0        0 2024-05-05 08:14:58.000000 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_14/__init__.py
--rw-rw-rw-   0        0        0    13292 2024-05-06 17:40:12.000000 sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_14/lesson_14.py
-drwxrwxrwx   0        0        0        0 2024-05-06 17:41:33.846401 sigmoid_check-0.0.7/sigmoid_check.egg-info/
--rw-rw-rw-   0        0        0     2756 2024-05-06 17:41:33.000000 sigmoid_check-0.0.7/sigmoid_check.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      663 2024-05-06 17:41:33.000000 sigmoid_check-0.0.7/sigmoid_check.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 17:41:33.000000 sigmoid_check-0.0.7/sigmoid_check.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-06 17:41:33.000000 sigmoid_check-0.0.7/sigmoid_check.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 08:53:03.873135 sigmoid_check-0.0.8/
+-rw-rw-rw-   0        0        0    11538 2024-04-23 18:15:46.000000 sigmoid_check-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2756 2024-05-09 08:53:03.872136 sigmoid_check-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1881 2024-04-23 18:29:06.000000 sigmoid_check-0.0.8/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-09 08:53:03.876140 sigmoid_check-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1104 2024-05-09 08:52:11.000000 sigmoid_check-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:53:03.817131 sigmoid_check-0.0.8/sigmoid_check/
+-rw-rw-rw-   0        0        0        0 2024-04-23 19:00:37.000000 sigmoid_check-0.0.8/sigmoid_check/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:53:03.849131 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/
+-rw-rw-rw-   0        0        0      213 2024-05-09 08:51:55.000000 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:53:03.854127 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_10/
+-rw-rw-rw-   0        0        0        0 2024-04-24 19:44:19.000000 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_10/__init__.py
+-rw-rw-rw-   0        0        0    22558 2024-04-23 20:44:39.000000 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_10/lesson_10.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:53:03.858137 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_11/
+-rw-rw-rw-   0        0        0        0 2024-04-24 19:44:19.000000 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_11/__init__.py
+-rw-rw-rw-   0        0        0    41222 2024-04-24 20:20:21.000000 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_11/lesson_11.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:53:03.862126 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_13/
+-rw-rw-rw-   0        0        0        0 2024-04-29 12:54:48.000000 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_13/__init__.py
+-rw-rw-rw-   0        0        0    21468 2024-04-30 12:20:28.000000 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_13/lesson_13.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:53:03.865126 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_14/
+-rw-rw-rw-   0        0        0        0 2024-05-05 08:14:58.000000 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_14/__init__.py
+-rw-rw-rw-   0        0        0    13292 2024-05-09 08:27:41.000000 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_14/lesson_14.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:53:03.868127 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_15/
+-rw-rw-rw-   0        0        0        0 2024-05-09 08:26:59.000000 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_15/__init__.py
+-rw-rw-rw-   0        0        0    12212 2024-05-09 08:50:14.000000 sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_15/lesson_15.py
+drwxrwxrwx   0        0        0        0 2024-05-09 08:53:03.870125 sigmoid_check-0.0.8/sigmoid_check.egg-info/
+-rw-rw-rw-   0        0        0     2756 2024-05-09 08:53:03.000000 sigmoid_check-0.0.8/sigmoid_check.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      766 2024-05-09 08:53:03.000000 sigmoid_check-0.0.8/sigmoid_check.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 08:53:03.000000 sigmoid_check-0.0.8/sigmoid_check.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-09 08:53:03.000000 sigmoid_check-0.0.8/sigmoid_check.egg-info/top_level.txt
```

### Comparing `sigmoid_check-0.0.7/LICENSE` & `sigmoid_check-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.7/PKG-INFO` & `sigmoid_check-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmoid_check
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package for checking the implementation of tasks in Sigmoid Courses
 Author: SigmoidAI - Balamatiuc Eduard
 Author-email: balamatiuc2@gmail.com
 License: Apache License 2.0
 Keywords: tasks,check,sigmoid,sigmoidai,sigmoid_check
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sigmoid_check-0.0.7/README.md` & `sigmoid_check-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.7/setup.py` & `sigmoid_check-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="sigmoid_check",
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(),
     description="A package for checking the implementation of tasks in Sigmoid Courses",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="SigmoidAI - Balamatiuc Eduard",
     author_email="balamatiuc2@gmail.com",
     keywords=["tasks", "check", "sigmoid", "sigmoidai", "sigmoid_check"],
```

### Comparing `sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_10/lesson_10.py` & `sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_10/lesson_10.py`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_11/lesson_11.py` & `sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_11/lesson_11.py`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_13/lesson_13.py` & `sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_13/lesson_13.py`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.7/sigmoid_check/python_odyssey/lesson_14/lesson_14.py` & `sigmoid_check-0.0.8/sigmoid_check/python_odyssey/lesson_14/lesson_14.py`

 * *Files identical despite different names*

### Comparing `sigmoid_check-0.0.7/sigmoid_check.egg-info/PKG-INFO` & `sigmoid_check-0.0.8/sigmoid_check.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmoid_check
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package for checking the implementation of tasks in Sigmoid Courses
 Author: SigmoidAI - Balamatiuc Eduard
 Author-email: balamatiuc2@gmail.com
 License: Apache License 2.0
 Keywords: tasks,check,sigmoid,sigmoidai,sigmoid_check
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sigmoid_check-0.0.7/sigmoid_check.egg-info/SOURCES.txt` & `sigmoid_check-0.0.8/sigmoid_check.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,8 +11,10 @@
 sigmoid_check/python_odyssey/lesson_10/__init__.py
 sigmoid_check/python_odyssey/lesson_10/lesson_10.py
 sigmoid_check/python_odyssey/lesson_11/__init__.py
 sigmoid_check/python_odyssey/lesson_11/lesson_11.py
 sigmoid_check/python_odyssey/lesson_13/__init__.py
 sigmoid_check/python_odyssey/lesson_13/lesson_13.py
 sigmoid_check/python_odyssey/lesson_14/__init__.py
-sigmoid_check/python_odyssey/lesson_14/lesson_14.py
+sigmoid_check/python_odyssey/lesson_14/lesson_14.py
+sigmoid_check/python_odyssey/lesson_15/__init__.py
+sigmoid_check/python_odyssey/lesson_15/lesson_15.py
```

