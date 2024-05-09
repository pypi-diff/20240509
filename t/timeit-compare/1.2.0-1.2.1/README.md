# Comparing `tmp/timeit_compare-1.2.0.tar.gz` & `tmp/timeit_compare-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeit_compare-1.2.0.tar", last modified: Thu May  2 15:07:03 2024, max compression
+gzip compressed data, was "timeit_compare-1.2.1.tar", last modified: Thu May  9 10:08:49 2024, max compression
```

## Comparing `timeit_compare-1.2.0.tar` & `timeit_compare-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 15:07:03.304433 timeit_compare-1.2.0/
--rw-rw-rw-   0        0        0     1089 2024-04-13 14:44:22.000000 timeit_compare-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     3916 2024-05-02 15:07:03.303054 timeit_compare-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2945 2024-05-02 10:48:47.000000 timeit_compare-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-02 15:07:03.304433 timeit_compare-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1248 2024-04-29 17:34:19.000000 timeit_compare-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:07:03.301429 timeit_compare-1.2.0/timeit_compare.egg-info/
--rw-rw-rw-   0        0        0     3916 2024-05-02 15:07:03.000000 timeit_compare-1.2.0/timeit_compare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-05-02 15:07:03.000000 timeit_compare-1.2.0/timeit_compare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 15:07:03.000000 timeit_compare-1.2.0/timeit_compare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-02 15:07:03.000000 timeit_compare-1.2.0/timeit_compare.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    25810 2024-05-02 11:05:39.000000 timeit_compare-1.2.0/timeit_compare.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:08:49.224308 timeit_compare-1.2.1/
+-rw-rw-rw-   0        0        0     1089 2024-04-13 14:44:22.000000 timeit_compare-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3916 2024-05-09 10:08:49.224308 timeit_compare-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2945 2024-05-02 10:48:47.000000 timeit_compare-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-09 10:08:49.224308 timeit_compare-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1248 2024-05-09 08:44:15.000000 timeit_compare-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 10:08:49.224308 timeit_compare-1.2.1/timeit_compare.egg-info/
+-rw-rw-rw-   0        0        0     3916 2024-05-09 10:08:49.000000 timeit_compare-1.2.1/timeit_compare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-05-09 10:08:49.000000 timeit_compare-1.2.1/timeit_compare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 10:08:49.000000 timeit_compare-1.2.1/timeit_compare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-09 10:08:49.000000 timeit_compare-1.2.1/timeit_compare.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    25929 2024-05-09 09:00:02.000000 timeit_compare-1.2.1/timeit_compare.py
```

### Comparing `timeit_compare-1.2.0/LICENSE` & `timeit_compare-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timeit_compare-1.2.0/PKG-INFO` & `timeit_compare-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeit_compare
-Version: 1.2.0
+Version: 1.2.1
 Summary: Based on the timeit library, timeit_compare can time multiple statements and provide comparison results.
 Home-page: https://github.com/AomandeNiuma/timeit_compare
 Author: Liu Wei
 Author-email: 23S112099@stu.hit.edu.cn
 Maintainer: Liu Wei
 Maintainer-email: 23S112099@stu.hit.edu.cn
 License: MIT
```

### Comparing `timeit_compare-1.2.0/README.md` & `timeit_compare-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `timeit_compare-1.2.0/setup.py` & `timeit_compare-1.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='timeit_compare',
-    version='1.2.0',
+    version='1.2.1',
     py_modules=['timeit_compare'],
     license='MIT',
     python_requires='>=3.6.0',
     description='Based on the timeit library, timeit_compare can time multiple '
                 'statements and provide comparison results.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `timeit_compare-1.2.0/timeit_compare.egg-info/PKG-INFO` & `timeit_compare-1.2.1/timeit_compare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeit_compare
-Version: 1.2.0
+Version: 1.2.1
 Summary: Based on the timeit library, timeit_compare can time multiple statements and provide comparison results.
 Home-page: https://github.com/AomandeNiuma/timeit_compare
 Author: Liu Wei
 Author-email: 23S112099@stu.hit.edu.cn
 Maintainer: Liu Wei
 Maintainer-email: 23S112099@stu.hit.edu.cn
 License: MIT
```

### Comparing `timeit_compare-1.2.0/timeit_compare.py` & `timeit_compare-1.2.1/timeit_compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,16 +363,17 @@
         error = 0
         total_repeat = timer_num * repeat
         complete = 0
 
         def update_process():
             if not show_process:
                 return
-            process = _process_bar(_percent(complete, total_repeat), 16)
-            string = (f'\r|{process}| {complete}/{total_repeat} completed, '
+            percent = _percent(complete, total_repeat)
+            string = (f'\r|{_process_bar(percent, 12)}| '
+                      f'{complete}/{total_repeat} completed, '
                       f'{error}/{timer_num} error')
             print(string, end='', flush=True)
 
         if show_process:
             print('timing now...')
 
         if number == 0:
@@ -386,16 +387,16 @@
                         if pre_time is not None:
                             total_time += pre_time
                         if turn_error:
                             error += 1
                     if error == timer_num:
                         return 0
                     if total_time > 0.2:
-                        return max(round((time * (n / total_time)) / repeat), 1)
-                    n <<= 1
+                        return max(round(n * time / total_time / repeat), 1)
+                    n = int(n * 0.25 / total_time) + 1 if total_time else n * 2
 
             try:
                 number = estimate()
             except (KeyboardInterrupt, SystemExit) as e:
                 for timer in timers:
                     turn_error = timer.pre_interrupt(e)
                     if turn_error:
@@ -537,14 +538,15 @@
 def compare(
         *timer_args: Union[Sequence, Callable, str],
         setup: Union[Callable, str] = 'pass',
         globals: dict = None,
         repeat: int = 5,
         number: int = 0,
         time: Union[float, int] = 1.0,
+        show_process: bool = True,
         sort_by: str = 'mean',
         reverse: bool = False,
         decimal: int = 2
 ) -> None:
     """
     Convenience function to create Compare object, call add_timer, run and
     print_results methods.
@@ -554,15 +556,15 @@
     :param setup: default setup for positional parameters with no or None setup
         given (default: same as Compare.add_timer).
     :param globals: default globals for positional parameters with no or None
         globals given (default: same as Compare.add_timer).
 
     See add_timer, run, and print_results methods of the class Compare.
     """
-    run_args = Compare._run_args(repeat, number, time, True)
+    run_args = Compare._run_args(repeat, number, time, show_process)
     print_results_args = Compare._print_results_args(sort_by, reverse, decimal)
     cmp = Compare()
     for args in timer_args:
         if isinstance(args, Sequence) and not isinstance(args, str):
             args = list(args)
             if len(args) < 3:
                 args.extend([None] * (3 - len(args)))
```

