# Comparing `tmp/lctest-0.1.8.tar.gz` & `tmp/lctest-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lctest-0.1.8.tar", last modified: Wed Apr 26 22:37:46 2023, max compression
+gzip compressed data, was "lctest-0.1.9.tar", last modified: Wed May  8 23:00:53 2024, max compression
```

## Comparing `lctest-0.1.8.tar` & `lctest-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-04-26 22:37:46.825358 lctest-0.1.8/
--rw-r--r--   0 tuanchau   (503) staff       (20)      918 2023-04-26 22:37:46.825167 lctest-0.1.8/PKG-INFO
--rw-r--r--   0 tuanchau   (503) staff       (20)      252 2023-04-26 22:36:06.000000 lctest-0.1.8/README.md
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-04-26 22:37:46.823619 lctest-0.1.8/lctest/
--rw-r--r--   0 tuanchau   (503) staff       (20)      499 2022-08-14 01:47:19.000000 lctest-0.1.8/lctest/__init__.py
--rw-r--r--   0 tuanchau   (503) staff       (20)      704 2022-07-22 10:51:15.000000 lctest-0.1.8/lctest/arguments.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     3795 2022-08-01 23:49:59.000000 lctest-0.1.8/lctest/lib.py
--rw-r--r--   0 tuanchau   (503) staff       (20)      332 2022-07-22 10:51:15.000000 lctest-0.1.8/lctest/stdlib.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     2136 2022-08-01 23:47:00.000000 lctest-0.1.8/lctest/test.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     9218 2022-08-14 00:10:34.000000 lctest-0.1.8/lctest/testcase.py
--rw-r--r--   0 tuanchau   (503) staff       (20)     1340 2022-08-01 23:42:18.000000 lctest-0.1.8/lctest/text_format.py
-drwxr-xr-x   0 tuanchau   (503) staff       (20)        0 2023-04-26 22:37:46.824873 lctest-0.1.8/lctest.egg-info/
--rw-r--r--   0 tuanchau   (503) staff       (20)      918 2023-04-26 22:37:46.000000 lctest-0.1.8/lctest.egg-info/PKG-INFO
--rw-r--r--   0 tuanchau   (503) staff       (20)      264 2023-04-26 22:37:46.000000 lctest-0.1.8/lctest.egg-info/SOURCES.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)        1 2023-04-26 22:37:46.000000 lctest-0.1.8/lctest.egg-info/dependency_links.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)        7 2023-04-26 22:37:46.000000 lctest-0.1.8/lctest.egg-info/top_level.txt
--rw-r--r--   0 tuanchau   (503) staff       (20)       38 2023-04-26 22:37:46.825403 lctest-0.1.8/setup.cfg
--rw-r--r--   0 tuanchau   (503) staff       (20)     1268 2023-04-26 22:37:36.000000 lctest-0.1.8/setup.py
+drwxr-xr-x   0 tuanchau   (501) staff       (20)        0 2024-05-08 23:00:53.725719 lctest-0.1.9/
+-rw-r--r--   0 tuanchau   (501) staff       (20)      918 2024-05-08 23:00:53.725624 lctest-0.1.9/PKG-INFO
+-rw-r--r--   0 tuanchau   (501) staff       (20)      252 2024-04-21 19:57:57.000000 lctest-0.1.9/README.md
+drwxr-xr-x   0 tuanchau   (501) staff       (20)        0 2024-05-08 23:00:53.725111 lctest-0.1.9/lctest/
+-rw-r--r--   0 tuanchau   (501) staff       (20)      488 2024-04-21 19:57:57.000000 lctest-0.1.9/lctest/__init__.py
+-rw-r--r--   0 tuanchau   (501) staff       (20)      704 2024-04-21 19:57:57.000000 lctest-0.1.9/lctest/arguments.py
+-rw-r--r--   0 tuanchau   (501) staff       (20)     3795 2024-04-21 19:57:57.000000 lctest-0.1.9/lctest/lib.py
+-rw-r--r--   0 tuanchau   (501) staff       (20)      332 2024-04-21 19:57:57.000000 lctest-0.1.9/lctest/stdlib.py
+-rw-r--r--   0 tuanchau   (501) staff       (20)     2136 2024-04-21 19:57:57.000000 lctest-0.1.9/lctest/test.py
+-rw-r--r--   0 tuanchau   (501) staff       (20)     8844 2024-05-06 13:18:13.000000 lctest-0.1.9/lctest/testcase.py
+-rw-r--r--   0 tuanchau   (501) staff       (20)     1340 2024-04-21 19:57:57.000000 lctest-0.1.9/lctest/text_format.py
+drwxr-xr-x   0 tuanchau   (501) staff       (20)        0 2024-05-08 23:00:53.725486 lctest-0.1.9/lctest.egg-info/
+-rw-r--r--   0 tuanchau   (501) staff       (20)      918 2024-05-08 23:00:53.000000 lctest-0.1.9/lctest.egg-info/PKG-INFO
+-rw-r--r--   0 tuanchau   (501) staff       (20)      264 2024-05-08 23:00:53.000000 lctest-0.1.9/lctest.egg-info/SOURCES.txt
+-rw-r--r--   0 tuanchau   (501) staff       (20)        1 2024-05-08 23:00:53.000000 lctest-0.1.9/lctest.egg-info/dependency_links.txt
+-rw-r--r--   0 tuanchau   (501) staff       (20)        7 2024-05-08 23:00:53.000000 lctest-0.1.9/lctest.egg-info/top_level.txt
+-rw-r--r--   0 tuanchau   (501) staff       (20)       38 2024-05-08 23:00:53.725754 lctest-0.1.9/setup.cfg
+-rw-r--r--   0 tuanchau   (501) staff       (20)     1268 2024-05-08 22:55:46.000000 lctest-0.1.9/setup.py
```

### Comparing `lctest-0.1.8/PKG-INFO` & `lctest-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lctest
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simulate leetcode runner
 Home-page: https://lctest.readthedocs.io/
 Author: Tuan Chau
 Author-email: tuanchaujp@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,13 +25,13 @@
 from lctest import *
 
 @testcase(
     (Expected, Parameters)
 )
 class Solution:
     @solution
-    def doSomething(self, params):
+    fun doSomething(self, params):
         pass
 
     def sol(self, params):
         pass
 ```
```

### Comparing `lctest-0.1.8/lctest/arguments.py` & `lctest-0.1.9/lctest/arguments.py`

 * *Files identical despite different names*

### Comparing `lctest-0.1.8/lctest/lib.py` & `lctest-0.1.9/lctest/lib.py`

 * *Files identical despite different names*

### Comparing `lctest-0.1.8/lctest/test.py` & `lctest-0.1.9/lctest/test.py`

 * *Files identical despite different names*

### Comparing `lctest-0.1.8/lctest/testcase.py` & `lctest-0.1.9/lctest/testcase.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,21 +40,15 @@
     return wrapper
 
 
 def log(*args):
     """
     Shorthand to create a testcase with log turned on.
     """
-    return Testcase(args, is_log=True, benchmark=False)
-
-def benchmark(*args):
-    """
-    Shorthand to create a testcase with benchmark turned on.
-    """
-    return Testcase(args, is_log=False, benchmark=True)
+    return Testcase(args, is_log=True)
 
 
 def testcase(*testcases, log=False, param_length_limit=100):
     is_printable = log or len(testcases) == 1
     if param_length_limit == -1:
         param_length_limit = float('inf')
 
@@ -113,27 +107,28 @@
             printer = helper.create_case_helper(case)
 
             try:
                 t0 = time.time()
                 result = fun(*case.params_snapshot)
                 runtime = (time.time() - t0) * 1000
                 printer.print_result(result, runtime)
+            except KeyboardInterrupt:
+                raise
             except:
                 printer.print_error()
 
     return deco
 
 
 class _TestPrinter:
-    def __init__(self, params_text, params, expected, is_test_printable, is_shorthand_result):
+    def __init__(self, params_text, params, expected, is_test_printable):
         self.params_text = params_text
         self.params = params
         self.expected = expected
         self.is_test_printable = is_test_printable
-        self.is_shorthand_result = is_shorthand_result
 
         self.output = StringIO()
 
         if not is_test_printable:
             sys.stdout = self.output
         else:
             # Use gray color for log
@@ -163,17 +158,14 @@
                 print(textformat(f"<brightyellow>{str(print_log)}</c>"))
             else:
                 pass
         self.output.close()
 
     def _result_to_text(self, result):
         result_text = str(result)
-        if len(result_text) > 50 and self.is_shorthand_result:
-            result_text = result_text[:50] + "..."
-
         if self.expected is None:
             return None, result_text, ""
         if result == self.expected:
             return True, result_text, result_text
 
         if callable(self.expected):
             expected = self.expected(*self.params)
@@ -250,20 +242,19 @@
     def create_case_helper(self, testcase):
         param_texts = [str(param) for param in testcase.params]
         for i, text in enumerate(param_texts):
             param_texts[i] = text if len(text) < self.param_length_limit else text[:self.param_length_limit - 3] + "..."
 
         params_text = self.param_format % tuple(param_texts)
         is_case_loggable = self.is_test_printable or testcase.is_loggable
-        return _TestPrinter(params_text, testcase.params, testcase.expected, is_case_loggable, testcase.benchmark)
+        return _TestPrinter(params_text, testcase.params, testcase.expected, is_case_loggable)
 
 
 class Testcase:
-    def __init__(self, args, is_log=False, benchmark=False):
+    def __init__(self, args, is_log=False):
         self.expected = args[0]
         self.params = args[1:]
         self.is_loggable = is_log
-        self.benchmark=benchmark
 
     @property
     def params_snapshot(self):
         return copy.deepcopy(self.params)
```

### Comparing `lctest-0.1.8/lctest/text_format.py` & `lctest-0.1.9/lctest/text_format.py`

 * *Files identical despite different names*

### Comparing `lctest-0.1.8/lctest.egg-info/PKG-INFO` & `lctest-0.1.9/lctest.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lctest
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simulate leetcode runner
 Home-page: https://lctest.readthedocs.io/
 Author: Tuan Chau
 Author-email: tuanchaujp@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -25,13 +25,13 @@
 from lctest import *
 
 @testcase(
     (Expected, Parameters)
 )
 class Solution:
     @solution
-    def doSomething(self, params):
+    fun doSomething(self, params):
         pass
 
     def sol(self, params):
         pass
 ```
```

### Comparing `lctest-0.1.8/setup.py` & `lctest-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="lctest",
-    version="0.1.8",
+    version="0.1.9",
     description="Simulate leetcode runner",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://lctest.readthedocs.io/",
     author="Tuan Chau",
     author_email="tuanchaujp@gmail.com",
     license="MIT",
```

