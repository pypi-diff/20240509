# Comparing `tmp/movoid_robotframework-1.4.6.tar.gz` & `tmp/movoid_robotframework-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_robotframework-1.4.6.tar", last modified: Tue May  7 13:36:17 2024, max compression
+gzip compressed data, was "movoid_robotframework-1.4.7.tar", last modified: Thu May  9 13:04:52 2024, max compression
```

## Comparing `movoid_robotframework-1.4.6.tar` & `movoid_robotframework-1.4.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 13:36:17.627655 movoid_robotframework-1.4.6/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0      290 2024-05-07 13:36:17.626659 movoid_robotframework-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 13:36:17.612182 movoid_robotframework-1.4.6/RobotFrameworkBasic/
--rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.4.6/RobotFrameworkBasic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:36:17.616320 movoid_robotframework-1.4.6/RobotFrameworkBasic/action/
--rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.6/RobotFrameworkBasic/action/__init__.py
--rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.6/RobotFrameworkBasic/action/calculate.py
--rw-rw-rw-   0        0        0     9664 2024-05-07 13:18:55.000000 movoid_robotframework-1.4.6/RobotFrameworkBasic/action/config.py
--rw-rw-rw-   0        0        0     6810 2024-05-06 14:37:08.000000 movoid_robotframework-1.4.6/RobotFrameworkBasic/common.py
--rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.4.6/RobotFrameworkBasic/decorator.py
--rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.6/RobotFrameworkBasic/error.py
--rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.6/RobotFrameworkBasic/main.py
--rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.6/RobotFrameworkBasic/version.py
-drwxrwxrwx   0        0        0        0 2024-05-07 13:36:17.625661 movoid_robotframework-1.4.6/movoid_robotframework.egg-info/
--rw-rw-rw-   0        0        0      290 2024-05-07 13:36:17.000000 movoid_robotframework-1.4.6/movoid_robotframework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-05-07 13:36:17.000000 movoid_robotframework-1.4.6/movoid_robotframework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 13:36:17.000000 movoid_robotframework-1.4.6/movoid_robotframework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-07 13:36:17.000000 movoid_robotframework-1.4.6/movoid_robotframework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-07 13:36:17.000000 movoid_robotframework-1.4.6/movoid_robotframework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 13:36:17.627655 movoid_robotframework-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      558 2024-05-07 13:35:48.000000 movoid_robotframework-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:52.926026 movoid_robotframework-1.4.7/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      290 2024-05-09 13:04:52.923992 movoid_robotframework-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_robotframework-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:52.909659 movoid_robotframework-1.4.7/RobotFrameworkBasic/
+-rw-rw-rw-   0        0        0      451 2024-02-20 17:41:03.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:52.914775 movoid_robotframework-1.4.7/RobotFrameworkBasic/action/
+-rw-rw-rw-   0        0        0      253 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/action/__init__.py
+-rw-rw-rw-   0        0        0     7070 2024-02-20 17:45:15.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/action/calculate.py
+-rw-rw-rw-   0        0        0     9735 2024-05-09 13:02:53.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/action/config.py
+-rw-rw-rw-   0        0        0     6810 2024-05-06 14:37:08.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/common.py
+-rw-rw-rw-   0        0        0    14138 2024-04-20 15:07:13.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/decorator.py
+-rw-rw-rw-   0        0        0      497 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/error.py
+-rw-rw-rw-   0        0        0      286 2024-04-24 13:42:41.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/main.py
+-rw-rw-rw-   0        0        0      911 2024-02-20 05:59:20.000000 movoid_robotframework-1.4.7/RobotFrameworkBasic/version.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:04:52.922971 movoid_robotframework-1.4.7/movoid_robotframework.egg-info/
+-rw-rw-rw-   0        0        0      290 2024-05-09 13:04:52.000000 movoid_robotframework-1.4.7/movoid_robotframework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-05-09 13:04:52.000000 movoid_robotframework-1.4.7/movoid_robotframework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 13:04:52.000000 movoid_robotframework-1.4.7/movoid_robotframework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-09 13:04:52.000000 movoid_robotframework-1.4.7/movoid_robotframework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-09 13:04:52.000000 movoid_robotframework-1.4.7/movoid_robotframework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 13:04:52.926026 movoid_robotframework-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      558 2024-05-09 13:04:15.000000 movoid_robotframework-1.4.7/setup.py
```

### Comparing `movoid_robotframework-1.4.6/RobotFrameworkBasic/action/calculate.py` & `movoid_robotframework-1.4.7/RobotFrameworkBasic/action/calculate.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.6/RobotFrameworkBasic/action/config.py` & `movoid_robotframework-1.4.7/RobotFrameworkBasic/action/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,17 @@
         self._path = Path('config.json')
         self._ori: Dict[str, Dict[str, Any]] = {}
         self._now: Dict[str, ConfigItem] = {}
         self._label_list: List[str] = []
         self.init(json_file)
         self.print = print if print_func is None else print_func
 
+    def __contains__(self, item):
+        return item in self._now
+
     def __getitem__(self, item):
         return self._now[item].value
 
     def init(self, json_file: str = None):
         self._path = self._path if json_file is None else Path(json_file)
         self.read()
```

### Comparing `movoid_robotframework-1.4.6/RobotFrameworkBasic/common.py` & `movoid_robotframework-1.4.7/RobotFrameworkBasic/common.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.6/RobotFrameworkBasic/decorator.py` & `movoid_robotframework-1.4.7/RobotFrameworkBasic/decorator.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.6/RobotFrameworkBasic/version.py` & `movoid_robotframework-1.4.7/RobotFrameworkBasic/version.py`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.6/movoid_robotframework.egg-info/SOURCES.txt` & `movoid_robotframework-1.4.7/movoid_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `movoid_robotframework-1.4.6/setup.py` & `movoid_robotframework-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='movoid_robotframework',
-    version='1.4.6',
+    version='1.4.7',
     packages=find_packages(),
     url='',
     license='',
     author='movoid',
     author_email='bobrobotsun@163.com',
     description='',
     long_description=long_description,
```

