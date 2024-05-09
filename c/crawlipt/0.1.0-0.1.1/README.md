# Comparing `tmp/crawlipt-0.1.0.tar.gz` & `tmp/crawlipt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlipt-0.1.0.tar", last modified: Thu May  9 04:51:05 2024, max compression
+gzip compressed data, was "crawlipt-0.1.1.tar", last modified: Thu May  9 05:53:42 2024, max compression
```

## Comparing `crawlipt-0.1.0.tar` & `crawlipt-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:05.303023 crawlipt-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 04:51:01.000000 crawlipt-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 04:51:01.000000 crawlipt-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 04:51:05.299023 crawlipt-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-09 04:51:01.000000 crawlipt-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:05.295023 crawlipt-0.1.0/crawlipt/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:05.299023 crawlipt-0.1.0/crawlipt/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/scroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/slide.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/actions/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:05.299023 crawlipt-0.1.0/crawlipt/conditions/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/conditions/element.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/conditions/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/conditions/presence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/conditions/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/conditions/visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/pojo.py
--rw-r--r--   0 runner    (1001) docker     (127)    25831 2024-05-09 04:51:01.000000 crawlipt-0.1.0/crawlipt/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 04:51:05.299023 crawlipt-0.1.0/crawlipt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 04:51:05.000000 crawlipt-0.1.0/crawlipt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-09 04:51:05.000000 crawlipt-0.1.0/crawlipt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 04:51:05.000000 crawlipt-0.1.0/crawlipt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 04:51:05.000000 crawlipt-0.1.0/crawlipt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 04:51:05.000000 crawlipt-0.1.0/crawlipt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 04:51:05.303023 crawlipt-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-09 04:51:01.000000 crawlipt-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:53:42.364158 crawlipt-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 05:53:38.000000 crawlipt-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 05:53:38.000000 crawlipt-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 05:53:42.364158 crawlipt-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-09 05:53:38.000000 crawlipt-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:53:42.360158 crawlipt-0.1.1/crawlipt/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:53:42.360158 crawlipt-0.1.1/crawlipt/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/actions/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/actions/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/actions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/actions/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/actions/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/actions/scroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/actions/slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/actions/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/actions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/actions/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:53:42.360158 crawlipt-0.1.1/crawlipt/conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/conditions/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/conditions/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/conditions/presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/conditions/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/conditions/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/pojo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25853 2024-05-09 05:53:38.000000 crawlipt-0.1.1/crawlipt/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 05:53:42.360158 crawlipt-0.1.1/crawlipt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 05:53:42.000000 crawlipt-0.1.1/crawlipt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-09 05:53:42.000000 crawlipt-0.1.1/crawlipt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 05:53:42.000000 crawlipt-0.1.1/crawlipt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 05:53:42.000000 crawlipt-0.1.1/crawlipt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 05:53:42.000000 crawlipt-0.1.1/crawlipt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 05:53:42.364158 crawlipt-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-09 05:53:38.000000 crawlipt-0.1.1/setup.py
```

### Comparing `crawlipt-0.1.0/LICENSE` & `crawlipt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/PKG-INFO` & `crawlipt-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.1.0
+Version: 0.1.1
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
-Metadata-Version: 2.1 Name: crawlipt Version: 0.1.0 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.1.1 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
```

### Comparing `crawlipt-0.1.0/README.md` & `crawlipt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/actions/alert.py` & `crawlipt-0.1.1/crawlipt/actions/alert.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/actions/click.py` & `crawlipt-0.1.1/crawlipt/actions/click.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/actions/get.py` & `crawlipt-0.1.1/crawlipt/actions/get.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/actions/input.py` & `crawlipt-0.1.1/crawlipt/actions/input.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/actions/redirect.py` & `crawlipt-0.1.1/crawlipt/actions/redirect.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/actions/scroll.py` & `crawlipt-0.1.1/crawlipt/actions/scroll.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,27 @@
 import time
 
 from selenium.webdriver import ActionChains, Keys
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from crawlipt.annotation import check
 
-js_code = '''he = setInterval(() => {
-                    document.documentElement.scrollTop += document.documentElement.scrollHeight
-                    if (document.documentElement.scrollTop >= (document.documentElement.scrollHeight - document.documentElement.scrollWidth)) {
-                        clearInterval(he)
-                    }
-                },100)
-            '''
-
 
 class Scroll:
 
     @staticmethod
     @check(exclude="driver")
-    def scrollByJs(driver: WebDriver) -> None:
+    def scrollByJs(driver: WebDriver, height: str | int) -> None:
         """
         Handling scroll events by Js
         :param driver: selenium webdriver
+        :param height: scroll height
         """
+        height = str(height)
+        js_code = "document.documentElement.scrollTop += %s" % height
         driver.execute_script(js_code)
 
     @staticmethod
     @check(exclude="driver")
     def scrollBySpace(driver: WebDriver, cnt: str | int, frequency: int = 0.1) -> None:
         """
         Handling scroll events by space
@@ -39,7 +34,23 @@
             cnt = int(cnt)
         actions = ActionChains(driver)
         actions.move_by_offset(0, 0).click().perform()
         time.sleep(random.uniform(frequency / 2, frequency))
         for _ in range(cnt):
             actions.send_keys(Keys.SPACE).perform()
             time.sleep(random.uniform(frequency / 2, frequency))
+
+    @staticmethod
+    @check(exclude="driver")
+    def scrollToBottom(driver: WebDriver) -> None:
+        """
+        Handling scroll to bottom events by Js
+        :param driver: selenium webdriver
+        """
+        js_code = '''he = setInterval(() => {
+                            document.documentElement.scrollTop += document.documentElement.scrollHeight
+                            if (document.documentElement.scrollTop >= (document.documentElement.scrollHeight - document.documentElement.scrollWidth)) {
+                                clearInterval(he)
+                            }
+                        },100)
+                    '''
+        driver.execute_script(js_code)
```

### Comparing `crawlipt-0.1.0/crawlipt/actions/select.py` & `crawlipt-0.1.1/crawlipt/actions/select.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/actions/slide.py` & `crawlipt-0.1.1/crawlipt/actions/slide.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/actions/switch.py` & `crawlipt-0.1.1/crawlipt/actions/switch.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/actions/util.py` & `crawlipt-0.1.1/crawlipt/actions/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,8 +28,22 @@
         :param driver: selenium webdriver
         :param num: the interval number
         """
         if not driver:
             return
         if isinstance(num, str):
             num = int(num)
-        time.sleep(random.uniform(num / 2, num))
+        time.sleep(num)
+
+    @staticmethod
+    @check(exclude="driver")
+    def intervalRandom(driver: WebDriver, num: str | int) -> None:
+        """
+        delay [num/2, num] seconds
+        :param driver: selenium webdriver
+        :param num: the interval number
+        """
+        if not driver:
+            return
+        if isinstance(num, str):
+            num = int(num)
+        time.sleep(random.uniform(num/2, num))
```

### Comparing `crawlipt-0.1.0/crawlipt/actions/window.py` & `crawlipt-0.1.1/crawlipt/actions/window.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/annotation.py` & `crawlipt-0.1.1/crawlipt/annotation.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/conditions/element.py` & `crawlipt-0.1.1/crawlipt/conditions/element.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/conditions/frame.py` & `crawlipt-0.1.1/crawlipt/conditions/frame.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/conditions/presence.py` & `crawlipt-0.1.1/crawlipt/conditions/presence.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/conditions/text.py` & `crawlipt-0.1.1/crawlipt/conditions/text.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/conditions/visibility.py` & `crawlipt-0.1.1/crawlipt/conditions/visibility.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/pojo.py` & `crawlipt-0.1.1/crawlipt/pojo.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/crawlipt/script.py` & `crawlipt-0.1.1/crawlipt/script.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def __condition_check(temp_condition: dict, name: str, pre_deep: str, current_deep: int, return_record: dict) -> None:
         condition = temp_condition.get("condition")
         temp_args = {"driver": None}
         if not condition:
             msg = "(Deep %s) condition of '%s' is missing" % (pre_deep + str(current_deep), name)
             raise ScriptSyntaxError(ParamTypeError(msg), "", pre_deep + str(current_deep))
         if condition not in ScriptProcess.CONDITIONS.keys():
-            msg = "(Deep %s) Could not found condition of '%s'" % (pre_deep + str(current_deep), name)
+            msg = "(Deep %s) Could not found the Condition Method in '%s'" % (pre_deep + str(current_deep), name)
             raise ScriptSyntaxError(ParamTypeError(msg), condition, pre_deep + str(current_deep))
         return_flag = temp_condition.get("return_flag")
         if return_flag and not isinstance(return_flag, str):
             msg = "(Deep %s) return_flag must be the type of str" % (pre_deep + str(current_deep))
             raise ScriptSyntaxError(ParamTypeError(msg), condition, pre_deep + str(current_deep))
         for key, value in temp_condition.items():
             if key.lower() not in ScriptProcess.__POP_KEY:
@@ -159,15 +159,15 @@
                                                 current_deep=current_deep)
             temp_args = {"driver": None}
             method = script.get("method")
             if not method:
                 msg = "(Deep %s) Method is missing" % (pre_deep + str(current_deep))
                 raise ScriptSyntaxError(ParamTypeError(msg), "", pre_deep + str(current_deep))
             if method not in ScriptProcess.ACTIONS.keys():
-                msg = "(Deep %s) Could not found Method" % (pre_deep + str(current_deep))
+                msg = "(Deep %s) Could not found the Action Method" % (pre_deep + str(current_deep))
                 raise ScriptSyntaxError(ParamTypeError(msg), method, pre_deep + str(current_deep))
             return_flag = script.get("return_flag")
             if return_flag and not isinstance(return_flag, str):
                 msg = "(Deep %s) return_flag must be the type of str" % (pre_deep + str(current_deep))
                 raise ScriptSyntaxError(ParamTypeError(msg), method, pre_deep + str(current_deep))
             for key, value in script.items():
                 if key.lower() not in ScriptProcess.__POP_KEY:
```

### Comparing `crawlipt-0.1.0/crawlipt.egg-info/PKG-INFO` & `crawlipt-0.1.1/crawlipt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.1.0
+Version: 0.1.1
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
-Metadata-Version: 2.1 Name: crawlipt Version: 0.1.0 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.1.1 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
```

### Comparing `crawlipt-0.1.0/crawlipt.egg-info/SOURCES.txt` & `crawlipt-0.1.1/crawlipt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlipt-0.1.0/setup.py` & `crawlipt-0.1.1/setup.py`

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
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "selenium>=4.0.0"
 ]
 
 # What packages are optional?
```

