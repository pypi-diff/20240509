# Comparing `tmp/crawlipt-0.0.8.tar.gz` & `tmp/crawlipt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlipt-0.0.8.tar", last modified: Wed May  8 14:03:59 2024, max compression
+gzip compressed data, was "crawlipt-0.0.9.tar", last modified: Thu May  9 03:26:18 2024, max compression
```

## Comparing `crawlipt-0.0.8.tar` & `crawlipt-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:59.717919 crawlipt-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-08 14:03:55.000000 crawlipt-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 14:03:55.000000 crawlipt-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-08 14:03:59.717919 crawlipt-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-08 14:03:55.000000 crawlipt-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:59.713919 crawlipt-0.0.8/crawlipt/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:59.717919 crawlipt-0.0.8/crawlipt/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/scroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/slide.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:59.717919 crawlipt-0.0.8/crawlipt/conditions/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/conditions/element.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/conditions/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/conditions/presence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/conditions/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/conditions/visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/pojo.py
--rw-r--r--   0 runner    (1001) docker     (127)    20140 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:59.717919 crawlipt-0.0.8/crawlipt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-08 14:03:59.000000 crawlipt-0.0.8/crawlipt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-08 14:03:59.000000 crawlipt-0.0.8/crawlipt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:03:59.000000 crawlipt-0.0.8/crawlipt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 14:03:59.000000 crawlipt-0.0.8/crawlipt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 14:03:59.000000 crawlipt-0.0.8/crawlipt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:03:59.717919 crawlipt-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-08 14:03:55.000000 crawlipt-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:26:18.417564 crawlipt-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-09 03:26:14.000000 crawlipt-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 03:26:14.000000 crawlipt-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 03:26:18.417564 crawlipt-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-09 03:26:14.000000 crawlipt-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:26:18.409563 crawlipt-0.0.9/crawlipt/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:26:18.413564 crawlipt-0.0.9/crawlipt/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/scroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/actions/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:26:18.413564 crawlipt-0.0.9/crawlipt/conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/conditions/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/conditions/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/conditions/presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/conditions/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/conditions/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/pojo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25822 2024-05-09 03:26:14.000000 crawlipt-0.0.9/crawlipt/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:26:18.413564 crawlipt-0.0.9/crawlipt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-09 03:26:18.000000 crawlipt-0.0.9/crawlipt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-09 03:26:18.000000 crawlipt-0.0.9/crawlipt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 03:26:18.000000 crawlipt-0.0.9/crawlipt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-09 03:26:18.000000 crawlipt-0.0.9/crawlipt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 03:26:18.000000 crawlipt-0.0.9/crawlipt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 03:26:18.417564 crawlipt-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-09 03:26:14.000000 crawlipt-0.0.9/setup.py
```

### Comparing `crawlipt-0.0.8/LICENSE` & `crawlipt-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/PKG-INFO` & `crawlipt-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.8
+Version: 0.0.9
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
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.8 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.9 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
```

### Comparing `crawlipt-0.0.8/README.md` & `crawlipt-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/actions/alert.py` & `crawlipt-0.0.9/crawlipt/actions/alert.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,16 @@
         Handling alert events
         :param driver: selenium webdriver
         :param operation: option in ["dismiss", "accept"]
         :param text: text to input
         """
         assert operation == "dismiss" or operation == "accept"
         alert = driver.switch_to.alert
+        alert_text = alert.text
         if text:
             alert.send_keys(text)
         if operation == "dismiss":
             alert.dismiss()
         else:
             alert.accept()
-        return alert.text
+        return alert_text
```

### Comparing `crawlipt-0.0.8/crawlipt/actions/click.py` & `crawlipt-0.0.9/crawlipt/actions/click.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import random
 import time
 
 from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.remote.webdriver import WebDriver
-
 from crawlipt.annotation import check, alias
 
 
 class Click:
     @staticmethod
     @check(exclude="driver")
     @alias("C")
@@ -55,15 +55,16 @@
         """
         Handling click events of all element
         :param driver: selenium webdriver
         :param xpath: click on the xpath path of the button
         """
         elements = driver.find_elements(By.XPATH, xpath)
         for element in elements:
-            element.click()
+            if EC.element_to_be_clickable(element):
+                element.click()
 
     @staticmethod
     @check(exclude="driver")
     def clickAllByJs(driver: WebDriver, xpath: str) -> None:
         """
         Handling click events of all element by js 'arguments[0].click();'
         :param driver: selenium webdriver
```

### Comparing `crawlipt-0.0.8/crawlipt/actions/get.py` & `crawlipt-0.0.9/crawlipt/actions/get.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/actions/input.py` & `crawlipt-0.0.9/crawlipt/actions/input.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/actions/redirect.py` & `crawlipt-0.0.9/crawlipt/actions/redirect.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/actions/scroll.py` & `crawlipt-0.0.9/crawlipt/actions/scroll.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/actions/select.py` & `crawlipt-0.0.9/crawlipt/actions/select.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/actions/slide.py` & `crawlipt-0.0.9/crawlipt/actions/slide.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/actions/switch.py` & `crawlipt-0.0.9/crawlipt/actions/switch.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/actions/util.py` & `crawlipt-0.0.9/crawlipt/actions/util.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/actions/window.py` & `crawlipt-0.0.9/crawlipt/actions/window.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,57 @@
-from selenium.common import NoSuchWindowException
-from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 
 from crawlipt.annotation import check, alias
 
 
 class Window:
     @staticmethod
     @check(exclude="driver")
+    @alias("window.clear")
     def clear(driver: WebDriver) -> None:
         """
         close all windows
         :param driver: selenium webdriver
         """
         for _ in range(driver.window_handles.__len__()-1):
             driver.close()
         driver.get("data:,")
 
     @staticmethod
     @check(exclude="driver")
+    @alias("window.back")
     def back(driver: WebDriver) -> None:
         """
         Goes one step backward in the browser history.
         :param driver: selenium webdriver
         """
         driver.back()
 
     @staticmethod
     @check(exclude="driver")
-    def forword(driver: WebDriver) -> None:
+    @alias("window.forward")
+    def forward(driver: WebDriver) -> None:
         """
         Goes one step forward in the browser history.
         :param driver: selenium webdriver
         """
         driver.forward()
 
     @staticmethod
     @check(exclude="driver")
+    @alias("window.close")
     def close(driver: WebDriver) -> None:
         """
         Closes the current window.
         :param driver: selenium webdriver
         """
         driver.close()
+
+    @staticmethod
+    @check(exclude="driver")
+    @alias("window.url")
+    def url(driver: WebDriver) -> str:
+        """
+        return the current url
+        :param driver: selenium webdriver
+        """
+        return driver.current_url
```

### Comparing `crawlipt-0.0.8/crawlipt/annotation.py` & `crawlipt-0.0.9/crawlipt/annotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,17 @@
                     raise ParamTypeError(f"Parameter {name} must be indicated the type.")
                 if name not in all_kwargs:
                     raise ParamTypeError(f"Parameter {name} is not in the defined parameter list.")
                 if all_kwargs[name] is None and type_.default is not type_.empty:
                     continue
                 if all_kwargs[name] == "__PRE_RETURN__":
                     continue
-                if isinstance(all_kwargs[name], str) and all_kwargs[name].startswith("__v-") and all_kwargs[
-                    name].endswith("__"):
+                if isinstance(all_kwargs[name], str) and all_kwargs[name].startswith("__rf-") and all_kwargs[name].endswith("__"):
+                    continue
+                if isinstance(all_kwargs[name], str) and all_kwargs[name].startswith("__v-") and all_kwargs[name].endswith("__"):
                     continue
                 if isinstance(all_kwargs[name], int) and type_.annotation is float:
                     all_kwargs[name] = float(all_kwargs.get(name))
                 if not isinstance(all_kwargs[name], type_.annotation):
                     raise ParamTypeError(f"Parameter {name} must be {type_.annotation}.")
             return func(*args, **kwargs)
```

### Comparing `crawlipt-0.0.8/crawlipt/conditions/element.py` & `crawlipt-0.0.9/crawlipt/conditions/element.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/conditions/frame.py` & `crawlipt-0.0.9/crawlipt/conditions/frame.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/conditions/presence.py` & `crawlipt-0.0.9/crawlipt/conditions/presence.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/conditions/text.py` & `crawlipt-0.0.9/crawlipt/conditions/text.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/conditions/visibility.py` & `crawlipt-0.0.9/crawlipt/conditions/visibility.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt/pojo.py` & `crawlipt-0.0.9/crawlipt/pojo.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/crawlipt.egg-info/PKG-INFO` & `crawlipt-0.0.9/crawlipt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.8
+Version: 0.0.9
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
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.8 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.9 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
```

### Comparing `crawlipt-0.0.8/crawlipt.egg-info/SOURCES.txt` & `crawlipt-0.0.9/crawlipt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.8/setup.py` & `crawlipt-0.0.9/setup.py`

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
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "selenium>=4.0.0"
 ]
 
 # What packages are optional?
```

