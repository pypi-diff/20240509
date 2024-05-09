# Comparing `tmp/crawlipt-0.0.7.tar.gz` & `tmp/crawlipt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlipt-0.0.7.tar", last modified: Wed May  8 11:28:42 2024, max compression
+gzip compressed data, was "crawlipt-0.0.8.tar", last modified: Wed May  8 14:03:59 2024, max compression
```

## Comparing `crawlipt-0.0.7.tar` & `crawlipt-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:28:42.978835 crawlipt-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-08 11:28:35.000000 crawlipt-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 11:28:35.000000 crawlipt-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-08 11:28:42.978835 crawlipt-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-08 11:28:35.000000 crawlipt-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:28:42.974835 crawlipt-0.0.7/crawlipt/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:28:42.974835 crawlipt-0.0.7/crawlipt/actions/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/redirect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/scroll.py
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/slide.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/actions/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:28:42.978835 crawlipt-0.0.7/crawlipt/conditions/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/conditions/element.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/conditions/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/conditions/presence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/conditions/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/conditions/visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/pojo.py
--rw-r--r--   0 runner    (1001) docker     (127)    20140 2024-05-08 11:28:35.000000 crawlipt-0.0.7/crawlipt/script.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:28:42.978835 crawlipt-0.0.7/crawlipt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-08 11:28:42.000000 crawlipt-0.0.7/crawlipt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-08 11:28:42.000000 crawlipt-0.0.7/crawlipt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:28:42.000000 crawlipt-0.0.7/crawlipt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 11:28:42.000000 crawlipt-0.0.7/crawlipt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 11:28:42.000000 crawlipt-0.0.7/crawlipt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:28:42.978835 crawlipt-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-08 11:28:35.000000 crawlipt-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:59.717919 crawlipt-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-08 14:03:55.000000 crawlipt-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-08 14:03:55.000000 crawlipt-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-08 14:03:59.717919 crawlipt-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-08 14:03:55.000000 crawlipt-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:59.713919 crawlipt-0.0.8/crawlipt/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:59.717919 crawlipt-0.0.8/crawlipt/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/redirect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/scroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/slide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/actions/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:59.717919 crawlipt-0.0.8/crawlipt/conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/conditions/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/conditions/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/conditions/presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/conditions/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/conditions/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/pojo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20140 2024-05-08 14:03:55.000000 crawlipt-0.0.8/crawlipt/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 14:03:59.717919 crawlipt-0.0.8/crawlipt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-08 14:03:59.000000 crawlipt-0.0.8/crawlipt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-08 14:03:59.000000 crawlipt-0.0.8/crawlipt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 14:03:59.000000 crawlipt-0.0.8/crawlipt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 14:03:59.000000 crawlipt-0.0.8/crawlipt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-08 14:03:59.000000 crawlipt-0.0.8/crawlipt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 14:03:59.717919 crawlipt-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-08 14:03:55.000000 crawlipt-0.0.8/setup.py
```

### Comparing `crawlipt-0.0.7/LICENSE` & `crawlipt-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/PKG-INFO` & `crawlipt-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.7
+Version: 0.0.8
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
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.7 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.8 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
```

### Comparing `crawlipt-0.0.7/README.md` & `crawlipt-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/actions/alert.py` & `crawlipt-0.0.8/crawlipt/actions/alert.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/actions/click.py` & `crawlipt-0.0.8/crawlipt/actions/click.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,43 +9,66 @@
 
 class Click:
     @staticmethod
     @check(exclude="driver")
     @alias("C")
     def click(driver: WebDriver, xpath: str) -> None:
         """
-        Handling click events
+        Handling click events of first element
         :param driver: selenium webdriver
         :param xpath: click on the xpath path of the button
         """
         element = driver.find_element(By.XPATH, xpath)
         element.click()
 
     @staticmethod
     @check(exclude="driver")
     def clickMulti(driver: WebDriver, xpath: str, cnt: str | int, frequency: int = 0.1) -> None:
         """
-        Handling click events multiple times
+        Handling click events of first element multiple times
         :param driver: selenium webdriver
         :param xpath: click on the xpath path of the button
         :param cnt: click count of the button
         :param frequency: click frequency of the button
         """
         if isinstance(cnt, str):
             cnt = int(cnt)
         element = driver.find_element(By.XPATH, xpath)
         while cnt:
             cnt -= 1
             element.click()
-            time.sleep(random.uniform(frequency/2, frequency))
+            time.sleep(random.uniform(frequency / 2, frequency))
 
     @staticmethod
     @check(exclude="driver")
     def clickByJs(driver: WebDriver, xpath: str) -> None:
         """
-        Handling click events by js 'arguments[0].click();'
+        Handling click events of first element by js 'arguments[0].click();'
         :param driver: selenium webdriver
         :param xpath: click on the xpath path of the button
         """
         element = driver.find_element(By.XPATH, xpath)
         driver.execute_script("arguments[0].click();", element)
 
+    @staticmethod
+    @check(exclude="driver")
+    def clickAll(driver: WebDriver, xpath: str) -> None:
+        """
+        Handling click events of all element
+        :param driver: selenium webdriver
+        :param xpath: click on the xpath path of the button
+        """
+        elements = driver.find_elements(By.XPATH, xpath)
+        for element in elements:
+            element.click()
+
+    @staticmethod
+    @check(exclude="driver")
+    def clickAllByJs(driver: WebDriver, xpath: str) -> None:
+        """
+        Handling click events of all element by js 'arguments[0].click();'
+        :param driver: selenium webdriver
+        :param xpath: click on the xpath path of the button
+        """
+        elements = driver.find_elements(By.XPATH, xpath)
+        for element in elements:
+            driver.execute_script("arguments[0].click();", element)
```

### Comparing `crawlipt-0.0.7/crawlipt/actions/get.py` & `crawlipt-0.0.8/crawlipt/actions/get.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/actions/input.py` & `crawlipt-0.0.8/crawlipt/actions/input.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/actions/redirect.py` & `crawlipt-0.0.8/crawlipt/actions/redirect.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/actions/scroll.py` & `crawlipt-0.0.8/crawlipt/actions/scroll.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/actions/select.py` & `crawlipt-0.0.8/crawlipt/actions/select.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/actions/slide.py` & `crawlipt-0.0.8/crawlipt/actions/slide.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/actions/switch.py` & `crawlipt-0.0.8/crawlipt/actions/switch.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/actions/util.py` & `crawlipt-0.0.8/crawlipt/actions/util.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/actions/window.py` & `crawlipt-0.0.8/crawlipt/actions/window.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/annotation.py` & `crawlipt-0.0.8/crawlipt/annotation.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/conditions/element.py` & `crawlipt-0.0.8/crawlipt/conditions/element.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/conditions/frame.py` & `crawlipt-0.0.8/crawlipt/conditions/frame.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/conditions/presence.py` & `crawlipt-0.0.8/crawlipt/conditions/presence.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/conditions/text.py` & `crawlipt-0.0.8/crawlipt/conditions/text.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/conditions/visibility.py` & `crawlipt-0.0.8/crawlipt/conditions/visibility.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/pojo.py` & `crawlipt-0.0.8/crawlipt/pojo.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt/script.py` & `crawlipt-0.0.8/crawlipt/script.py`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/crawlipt.egg-info/PKG-INFO` & `crawlipt-0.0.8/crawlipt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawlipt
-Version: 0.0.7
+Version: 0.0.8
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
-Metadata-Version: 2.1 Name: crawlipt Version: 0.0.7 Summary: The script for
+Metadata-Version: 2.1 Name: crawlipt Version: 0.0.8 Summary: The script for
 selenium in python Home-page: https://github.com/WwwwwyDev/crawlipt Author:
 WwwwwyDev Author-email: wwy20001014@foxmail.com License: MIT Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
 Implementation :: CPython Classifier: Programming Language :: Python ::
 Implementation :: PyPy Requires-Python: >=3.10.0 Description-Content-Type:
```

### Comparing `crawlipt-0.0.7/crawlipt.egg-info/SOURCES.txt` & `crawlipt-0.0.8/crawlipt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlipt-0.0.7/setup.py` & `crawlipt-0.0.8/setup.py`

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
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "selenium>=4.0.0"
 ]
 
 # What packages are optional?
```

