# Comparing `tmp/movoid_function-1.5.2.tar.gz` & `tmp/movoid_function-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_function-1.5.2.tar", last modified: Wed May  8 14:57:40 2024, max compression
+gzip compressed data, was "movoid_function-1.5.3.tar", last modified: Wed May  8 15:09:38 2024, max compression
```

## Comparing `movoid_function-1.5.2.tar` & `movoid_function-1.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 14:57:40.019929 movoid_function-1.5.2/
--rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_function-1.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0      213 2024-05-08 14:57:40.017925 movoid_function-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_function-1.5.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 14:57:40.002968 movoid_function-1.5.2/movoid_function/
--rw-rw-rw-   0        0        0      562 2024-04-13 09:15:08.000000 movoid_function-1.5.2/movoid_function/__init__.py
--rw-rw-rw-   0        0        0     9920 2024-05-08 14:50:45.000000 movoid_function-1.5.2/movoid_function/check.py
--rw-rw-rw-   0        0        0    16565 2024-02-20 11:49:02.000000 movoid_function-1.5.2/movoid_function/decorator.py
--rw-rw-rw-   0        0        0     1557 2024-04-14 08:03:48.000000 movoid_function-1.5.2/movoid_function/function.py
--rw-rw-rw-   0        0        0    16245 2024-05-08 14:50:45.000000 movoid_function-1.5.2/movoid_function/type.py
-drwxrwxrwx   0        0        0        0 2024-05-08 14:57:40.009339 movoid_function-1.5.2/movoid_function.egg-info/
--rw-rw-rw-   0        0        0      213 2024-05-08 14:57:39.000000 movoid_function-1.5.2/movoid_function.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-05-08 14:57:39.000000 movoid_function-1.5.2/movoid_function.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 14:57:39.000000 movoid_function-1.5.2/movoid_function.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-08 14:57:39.000000 movoid_function-1.5.2/movoid_function.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 14:57:40.019929 movoid_function-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0      462 2024-05-08 14:56:50.000000 movoid_function-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:38.954384 movoid_function-1.5.3/
+-rw-rw-rw-   0        0        0       10 2024-04-24 13:42:41.000000 movoid_function-1.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      213 2024-05-08 15:09:38.953387 movoid_function-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_function-1.5.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:38.936627 movoid_function-1.5.3/movoid_function/
+-rw-rw-rw-   0        0        0      562 2024-04-13 09:15:08.000000 movoid_function-1.5.3/movoid_function/__init__.py
+-rw-rw-rw-   0        0        0     9920 2024-05-08 14:50:45.000000 movoid_function-1.5.3/movoid_function/check.py
+-rw-rw-rw-   0        0        0    16565 2024-02-20 11:49:02.000000 movoid_function-1.5.3/movoid_function/decorator.py
+-rw-rw-rw-   0        0        0     1557 2024-04-14 08:03:48.000000 movoid_function-1.5.3/movoid_function/function.py
+-rw-rw-rw-   0        0        0    16232 2024-05-08 15:09:12.000000 movoid_function-1.5.3/movoid_function/type.py
+drwxrwxrwx   0        0        0        0 2024-05-08 15:09:38.944551 movoid_function-1.5.3/movoid_function.egg-info/
+-rw-rw-rw-   0        0        0      213 2024-05-08 15:09:38.000000 movoid_function-1.5.3/movoid_function.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-05-08 15:09:38.000000 movoid_function-1.5.3/movoid_function.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 15:09:38.000000 movoid_function-1.5.3/movoid_function.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-08 15:09:38.000000 movoid_function-1.5.3/movoid_function.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 15:09:38.954384 movoid_function-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      462 2024-05-08 15:09:12.000000 movoid_function-1.5.3/setup.py
```

### Comparing `movoid_function-1.5.2/movoid_function/__init__.py` & `movoid_function-1.5.3/movoid_function/__init__.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.2/movoid_function/check.py` & `movoid_function-1.5.3/movoid_function/check.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.2/movoid_function/decorator.py` & `movoid_function-1.5.3/movoid_function/decorator.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.2/movoid_function/function.py` & `movoid_function-1.5.3/movoid_function/function.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.5.2/movoid_function/type.py` & `movoid_function-1.5.3/movoid_function/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,15 @@
                     fail_str.append(f'{check_target} contain char more than <{self._char}>:{char_error}')
             if not self._length.check(len(check_target)):
                 fail_str.append(f'{len(check_target)} length of {check_target} did not match: {self._length.show_all_step()}')
             if self._regex:
                 if not bool(re.search(self._regex, check_target)):
                     fail_str.append(f'{check_target} does not meet rule {self._regex}')
         else:
-            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not str')
         return fail_str
 
     @property
     def annotation(self):
         return str
 
 
@@ -235,15 +235,15 @@
 
     def check_function(self, check_target) -> typing.List[str]:
         fail_str: typing.List[str] = []
         if isinstance(check_target, str):
             if not self._length.check(len(check_target)):
                 fail_str.append(f'{len(check_target)} length of {check_target} did not match: {self._length.show_all_step()}')
         else:
-            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not list')
         return fail_str
 
     def check(self, check_target, convert=None) -> bool:
         check_target = self.convert(check_target, convert)
         if isinstance(check_target, list):
             re_bool = True
             re_bool = re_bool and self._length.check(len(check_target))
@@ -275,15 +275,15 @@
 
     def check_function(self, check_target) -> typing.List[str]:
         fail_str: typing.List[str] = []
         if isinstance(check_target, str):
             if not self._length.check(len(check_target)):
                 fail_str.append(f'{len(check_target)} length of {check_target} did not match: {self._length.show_all_step()}')
         else:
-            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not tuple')
         return fail_str
 
     @property
     def annotation(self):
         if self._convert:
             return typing.Union[tuple, str]
         else:
@@ -306,15 +306,15 @@
 
     def check_function(self, check_target) -> typing.List[str]:
         fail_str: typing.List[str] = []
         if isinstance(check_target, str):
             if not self._length.check(len(check_target)):
                 fail_str.append(f'{len(check_target)} length of {check_target} did not match: {self._length.show_all_step()}')
         else:
-            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not set')
         return fail_str
 
     @property
     def annotation(self):
         if self._convert:
             return typing.Union[set, str]
         else:
@@ -337,15 +337,15 @@
 
     def check_function(self, check_target) -> typing.List[str]:
         fail_str: typing.List[str] = []
         if isinstance(check_target, str):
             if not self._length.check(len(check_target)):
                 fail_str.append(f'{len(check_target)} length of {check_target} did not match: {self._length.show_all_step()}')
         else:
-            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not dict')
         return fail_str
 
     @property
     def annotation(self):
         if self._convert:
             return typing.Union[dict, str]
         else:
@@ -384,15 +384,15 @@
             try:
                 tar_path = pathlib.Path(check_target)
                 if self._should_exist and not tar_path.exists():
                     fail_str.append(f'{check_target} does not exists.')
             except:
                 fail_str.append(f'{check_target} is not a valid path.')
         else:
-            fail_str.append(f'{check_target} is {type(check_target).__name__} not number')
+            fail_str.append(f'{check_target} is {type(check_target).__name__} not path')
         return fail_str
 
     @property
     def annotation(self):
         return str
```

