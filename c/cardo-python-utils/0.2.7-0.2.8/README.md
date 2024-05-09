# Comparing `tmp/cardo-python-utils-0.2.7.tar.gz` & `tmp/cardo-python-utils-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardo-python-utils-0.2.7.tar", last modified: Wed Feb 14 09:43:14 2024, max compression
+gzip compressed data, was "cardo-python-utils-0.2.8.tar", last modified: Thu May  9 10:41:05 2024, max compression
```

## Comparing `cardo-python-utils-0.2.7.tar` & `cardo-python-utils-0.2.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 09:43:14.245715 cardo-python-utils-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-02-14 09:43:14.245715 cardo-python-utils-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 09:43:14.245715 cardo-python-utils-0.2.7/cardo_python_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-02-14 09:43:14.000000 cardo-python-utils-0.2.7/cardo_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-14 09:43:14.000000 cardo-python-utils-0.2.7/cardo_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 09:43:14.000000 cardo-python-utils-0.2.7/cardo_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-14 09:43:14.000000 cardo-python-utils-0.2.7/cardo_python_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-14 09:43:14.000000 cardo-python-utils-0.2.7/cardo_python_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 09:43:14.245715 cardo-python-utils-0.2.7/python_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)    16820 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    17515 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/django_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/esma_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/python_utils/types_hinting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-02-14 09:43:14.245715 cardo-python-utils-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-14 09:43:04.000000 cardo-python-utils-0.2.7/setup.py
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-05-09 10:41:05.977048 cardo-python-utils-0.2.8/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1046 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/LICENSE
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       60 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/MANIFEST.in
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2024-05-09 10:41:05.977048 cardo-python-utils-0.2.8/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1114 2023-06-09 16:11:25.000000 cardo-python-utils-0.2.8/README.rst
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-05-09 10:41:05.977048 cardo-python-utils-0.2.8/cardo_python_utils.egg-info/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2146 2024-05-09 10:41:05.000000 cardo-python-utils-0.2.8/cardo_python_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      610 2024-05-09 10:41:05.000000 cardo-python-utils-0.2.8/cardo_python_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        1 2024-05-09 10:41:05.000000 cardo-python-utils-0.2.8/cardo_python_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      187 2024-05-09 10:41:05.000000 cardo-python-utils-0.2.8/cardo_python_utils.egg-info/requires.txt
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)       13 2024-05-09 10:41:05.000000 cardo-python-utils-0.2.8/cardo_python_utils.egg-info/top_level.txt
+drwxrwxr-x   0 klajdi    (1000) klajdi    (1000)        0 2024-05-09 10:41:05.977048 cardo-python-utils-0.2.8/python_utils/
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)        0 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/python_utils/__init__.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     2501 2023-07-11 13:35:59.000000 cardo-python-utils-0.2.8/python_utils/choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16820 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/python_utils/data_structures.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      455 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/python_utils/db.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    17515 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/python_utils/django_utils.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)    16197 2024-05-09 10:40:31.000000 cardo-python-utils-0.2.8/python_utils/esma_choices.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      751 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/python_utils/exceptions.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      913 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/python_utils/imports.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     5603 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/python_utils/math.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     6159 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/python_utils/pandas_utils.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1290 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/python_utils/rest.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     3740 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/python_utils/text.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     9614 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/python_utils/time.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      120 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/python_utils/types_hinting.py
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)     1137 2024-05-09 10:41:05.981048 cardo-python-utils-0.2.8/setup.cfg
+-rw-rw-r--   0 klajdi    (1000) klajdi    (1000)      142 2023-05-05 12:21:33.000000 cardo-python-utils-0.2.8/setup.py
```

### Comparing `cardo-python-utils-0.2.7/LICENSE` & `cardo-python-utils-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/PKG-INFO` & `cardo-python-utils-0.2.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardo-python-utils
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python library enhanced with a wide range of functions for different scenarios.
 Home-page: https://github.com/CardoAI/cardo-python-utils
 Author: Kristi Kotini
 Author-email: hello@cardoai.com
 License: MIT (X11)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -16,29 +16,19 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
-License-File: LICENSE
 Provides-Extra: pandas
-Requires-Dist: pandas>=1.4.0; extra == "pandas"
 Provides-Extra: django
-Requires-Dist: Django; extra == "django"
-Requires-Dist: django-model-utils==4.2.0; extra == "django"
 Provides-Extra: rest
-Requires-Dist: djangorestframework; extra == "rest"
-Requires-Dist: requests; extra == "rest"
 Provides-Extra: all
-Requires-Dist: Django; extra == "all"
-Requires-Dist: pandas>=1.4.0; extra == "all"
-Requires-Dist: django-model-utils>=4.2.0; extra == "all"
-Requires-Dist: djangorestframework; extra == "all"
-Requires-Dist: requests; extra == "all"
+License-File: LICENSE
 
 ============================
 CardoAI Python Helper Module
 ============================
 
 This library allows the utilization of different utility functions for different scenarios.
```

### Comparing `cardo-python-utils-0.2.7/README.rst` & `cardo-python-utils-0.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/cardo_python_utils.egg-info/PKG-INFO` & `cardo-python-utils-0.2.8/cardo_python_utils.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardo-python-utils
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python library enhanced with a wide range of functions for different scenarios.
 Home-page: https://github.com/CardoAI/cardo-python-utils
 Author: Kristi Kotini
 Author-email: hello@cardoai.com
 License: MIT (X11)
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -16,29 +16,19 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
-License-File: LICENSE
 Provides-Extra: pandas
-Requires-Dist: pandas>=1.4.0; extra == "pandas"
 Provides-Extra: django
-Requires-Dist: Django; extra == "django"
-Requires-Dist: django-model-utils==4.2.0; extra == "django"
 Provides-Extra: rest
-Requires-Dist: djangorestframework; extra == "rest"
-Requires-Dist: requests; extra == "rest"
 Provides-Extra: all
-Requires-Dist: Django; extra == "all"
-Requires-Dist: pandas>=1.4.0; extra == "all"
-Requires-Dist: django-model-utils>=4.2.0; extra == "all"
-Requires-Dist: djangorestframework; extra == "all"
-Requires-Dist: requests; extra == "all"
+License-File: LICENSE
 
 ============================
 CardoAI Python Helper Module
 ============================
 
 This library allows the utilization of different utility functions for different scenarios.
```

### Comparing `cardo-python-utils-0.2.7/cardo_python_utils.egg-info/SOURCES.txt` & `cardo-python-utils-0.2.8/cardo_python_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/python_utils/choices.py` & `cardo-python-utils-0.2.8/python_utils/choices.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/python_utils/data_structures.py` & `cardo-python-utils-0.2.8/python_utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/python_utils/django_utils.py` & `cardo-python-utils-0.2.8/python_utils/django_utils.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/python_utils/esma_choices.py` & `cardo-python-utils-0.2.8/python_utils/esma_choices.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,14 +256,15 @@
     PRBO = 24, "PRIBOR"
     TLBO = 25, "TELBOR"
     WIBO = 26, "WIBOR"
     BOER = 27, "Bank of England Base Rate"
     ECBR = 28, "European Central Bank Base Rate"
     LDOR = 29, "Lender's Own Rate"
     OTHR = 30, "Other"
+    SOFR = 31, "SOFR"
 
 
 class InterestRateIndexTenorChoices(ChoiceEnum):
     OVNG = 1, "Overnight"
     INDA = 2, "IntraDay"
     DAIL = 3, "1 day"
     WEEK = 4, "1 week"
```

### Comparing `cardo-python-utils-0.2.7/python_utils/exceptions.py` & `cardo-python-utils-0.2.8/python_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/python_utils/imports.py` & `cardo-python-utils-0.2.8/python_utils/imports.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/python_utils/math.py` & `cardo-python-utils-0.2.8/python_utils/math.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/python_utils/pandas_utils.py` & `cardo-python-utils-0.2.8/python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/python_utils/rest.py` & `cardo-python-utils-0.2.8/python_utils/rest.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/python_utils/text.py` & `cardo-python-utils-0.2.8/python_utils/text.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/python_utils/time.py` & `cardo-python-utils-0.2.8/python_utils/time.py`

 * *Files identical despite different names*

### Comparing `cardo-python-utils-0.2.7/setup.cfg` & `cardo-python-utils-0.2.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cardo-python-utils
-version = 0.2.7
+version = 0.2.8
 description = Python library enhanced with a wide range of functions for different scenarios.
 long_description = file: README.rst
 url = https://github.com/CardoAI/cardo-python-utils
 author = Kristi Kotini
 author_email = hello@cardoai.com
 license = MIT (X11)
 classifiers =
```

