# Comparing `tmp/crawlipt-0.0.9.tar.gz` & `tmp/crawlipt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlipt-0.0.9.tar", last modified: Thu May  9 03:26:18 2024, max compression
+gzip compressed data, was "crawlipt-0.1.0.tar", last modified: Thu May  9 04:51:05 2024, max compression
```

## Comparing `crawlipt-0.0.9.tar` & `crawlipt-0.1.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:26:18.417564 crawlipt-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 03:26:14.000000 crawlipt-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 03:26:14.000000 crawlipt-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 03:26:18.417564 crawlipt-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-09 03:26:14.000000 crawlipt-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:26:18.409563 crawlipt-0.0.9/crawlipt/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:26:18.413564 crawlipt-0.0.9/crawlipt/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/scroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/slide.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:26:18.413564 crawlipt-0.0.9/crawlipt/conditions/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/conditions/element.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/conditions/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/conditions/presence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/conditions/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/conditions/visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/pojo.py
--rw-r--r--   0 runner    (1001) docker     (127)    25822 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:26:18.413564 crawlipt-0.0.9/crawlipt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 03:26:18.000000 crawlipt-0.0.9/crawlipt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-09 03:26:18.000000 crawlipt-0.0.9/crawlipt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 03:26:18.000000 crawlipt-0.0.9/crawlipt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 03:26:18.000000 crawlipt-0.0.9/crawlipt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 03:26:18.000000 crawlipt-0.0.9/crawlipt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 03:26:18.417564 crawlipt-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-09 03:26:14.000000 crawlipt-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:05.303023 crawlipt-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 04:51:01.000000 crawlipt-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 04:51:01.000000 crawlipt-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 04:51:05.299023 crawlipt-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-09 04:51:01.000000 crawlipt-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:05.295023 crawlipt-0.1.0/crawlipt/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:05.299023 crawlipt-0.1.0/crawlipt/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/scroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:05.299023 crawlipt-0.1.0/crawlipt/conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/conditions/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/conditions/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/conditions/presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/conditions/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/conditions/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/pojo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25831 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:05.299023 crawlipt-0.1.0/crawlipt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 04:51:05.000000 crawlipt-0.1.0/crawlipt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-09 04:51:05.000000 crawlipt-0.1.0/crawlipt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:51:05.000000 crawlipt-0.1.0/crawlipt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 04:51:05.000000 crawlipt-0.1.0/crawlipt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 04:51:05.000000 crawlipt-0.1.0/crawlipt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 04:51:05.303023 crawlipt-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-09 04:51:01.000000 crawlipt-0.1.0/setup.py
```

### Comparing `crawlipt-0.0.9/LICENSE` & `crawlipt-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/PKG-INFO` & `crawlipt-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.9
+Version: 0.1.0
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.9 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.1.0 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
```

### Comparing `crawlipt-0.0.9/README.md` & `crawlipt-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/actions/alert.py` & `crawlipt-0.1.0/crawlipt/actions/alert.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/actions/click.py` & `crawlipt-0.1.0/crawlipt/actions/click.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/actions/get.py` & `crawlipt-0.1.0/crawlipt/actions/get.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/actions/input.py` & `crawlipt-0.1.0/crawlipt/actions/input.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/actions/redirect.py` & `crawlipt-0.1.0/crawlipt/actions/redirect.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/actions/scroll.py` & `crawlipt-0.1.0/crawlipt/actions/scroll.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/actions/select.py` & `crawlipt-0.1.0/crawlipt/actions/select.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/actions/slide.py` & `crawlipt-0.1.0/crawlipt/actions/slide.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/actions/switch.py` & `crawlipt-0.1.0/crawlipt/actions/switch.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/actions/util.py` & `crawlipt-0.1.0/crawlipt/actions/util.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/actions/window.py` & `crawlipt-0.1.0/crawlipt/actions/window.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/annotation.py` & `crawlipt-0.1.0/crawlipt/annotation.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/conditions/element.py` & `crawlipt-0.1.0/crawlipt/conditions/element.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/conditions/frame.py` & `crawlipt-0.1.0/crawlipt/conditions/frame.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/conditions/presence.py` & `crawlipt-0.1.0/crawlipt/conditions/presence.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/conditions/text.py` & `crawlipt-0.1.0/crawlipt/conditions/text.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/conditions/visibility.py` & `crawlipt-0.1.0/crawlipt/conditions/visibility.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/pojo.py` & `crawlipt-0.1.0/crawlipt/pojo.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/crawlipt/script.py` & `crawlipt-0.1.0/crawlipt/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     all_dict.update(alias_dict)
     return all_dict
 
 
 class ScriptProcess:
     ACTIONS = get_dict(Action)
     CONDITIONS = get_dict(Condition)
-    __POP_KEY = {"method", "next", "if", "check", "condition", "loop", "return_flag"}
+    __POP_KEY = {"method", "next", "if", "check", "condition", "loop", "return_flag", "while"}
 
     @staticmethod
     @check
     def __condition_check(temp_condition: dict, name: str, pre_deep: str, current_deep: int, return_record: dict) -> None:
         condition = temp_condition.get("condition")
         temp_args = {"driver": None}
         if not condition:
```

### Comparing `crawlipt-0.0.9/crawlipt.egg-info/PKG-INFO` & `crawlipt-0.1.0/crawlipt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.9
+Version: 0.1.0
 Summary: The script for selenium in python
 Home-page: https://github.com/WwwwwyDev/crawlipt
 Author: WwwwwyDev
 Author-email: wwy20001014@foxmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.9 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.1.0 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
```

### Comparing `crawlipt-0.0.9/crawlipt.egg-info/SOURCES.txt` & `crawlipt-0.1.0/crawlipt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.9/setup.py` & `crawlipt-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'crawlipt'
 DESCRIPTION = 'The script for selenium in python'
 URL = 'https://github.com/WwwwwyDev/crawlipt'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwwwwyDev'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.0.9'
+VERSION = '0.1.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "selenium>=4.0.0"
 ]
 
 # What packages are optional?
```

