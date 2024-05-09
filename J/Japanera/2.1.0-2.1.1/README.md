# Comparing `tmp/Japanera-2.1.0.tar.gz` & `tmp/Japanera-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Japanera-2.1.0.tar", last modified: Wed Nov  8 08:17:31 2023, max compression
+gzip compressed data, was "Japanera-2.1.1.tar", last modified: Wed Mar 13 11:14:23 2024, max compression
```

## Comparing `Japanera-2.1.0.tar` & `Japanera-2.1.1.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-11-08 08:17:31.475153 Japanera-2.1.0/
-drwxrwxrwx   0        0        0        0 2023-11-08 08:17:31.464609 Japanera-2.1.0/Japanera.egg-info/
--rw-rw-rw-   0        0        0     1335 2023-11-08 08:17:31.000000 Japanera-2.1.0/Japanera.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2023-11-08 08:17:31.000000 Japanera-2.1.0/Japanera.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-08 08:17:31.000000 Japanera-2.1.0/Japanera.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-07 08:07:56.000000 Japanera-2.1.0/Japanera.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-11-08 08:17:31.000000 Japanera-2.1.0/Japanera.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-11-08 08:17:31.000000 Japanera-2.1.0/Japanera.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1062 2023-11-08 08:14:09.000000 Japanera-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     1335 2023-11-08 08:17:31.474146 Japanera-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    11658 2023-03-07 08:13:25.000000 Japanera-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-11-08 08:17:31.472140 Japanera-2.1.0/japanera/
--rw-rw-rw-   0        0        0      378 2023-11-08 08:14:02.000000 Japanera-2.1.0/japanera/__about__.py
--rw-rw-rw-   0        0        0      881 2023-03-07 08:02:16.000000 Japanera-2.1.0/japanera/__init__.py
--rw-rw-rw-   0        0        0    25455 2023-03-07 06:42:42.000000 Japanera-2.1.0/japanera/era_data.py
--rw-rw-rw-   0        0        0    16298 2023-03-07 07:59:24.000000 Japanera-2.1.0/japanera/japanera.py
--rw-rw-rw-   0        0        0    25605 2023-11-08 08:16:13.000000 Japanera-2.1.0/japanera/parser.py
--rw-rw-rw-   0        0        0       42 2023-11-08 08:17:31.475153 Japanera-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1743 2023-11-08 08:14:55.000000 Japanera-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-13 11:14:23.809735 Japanera-2.1.1/
+drwxrwxrwx   0        0        0        0 2024-03-13 11:14:23.807186 Japanera-2.1.1/Japanera.egg-info/
+-rw-rw-rw-   0        0        0     1361 2024-03-13 11:14:23.000000 Japanera-2.1.1/Japanera.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2024-03-13 11:14:23.000000 Japanera-2.1.1/Japanera.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-13 11:14:23.000000 Japanera-2.1.1/Japanera.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-07 08:07:56.000000 Japanera-2.1.1/Japanera.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       15 2024-03-13 11:14:23.000000 Japanera-2.1.1/Japanera.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-03-13 11:14:23.000000 Japanera-2.1.1/Japanera.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1062 2024-03-13 11:03:57.000000 Japanera-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1361 2024-03-13 11:14:23.807689 Japanera-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11658 2023-03-07 08:13:25.000000 Japanera-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-03-13 11:14:23.801187 Japanera-2.1.1/japanera/
+-rw-rw-rw-   0        0        0      373 2024-03-13 11:03:32.000000 Japanera-2.1.1/japanera/__about__.py
+-rw-rw-rw-   0        0        0      881 2024-03-13 11:03:32.000000 Japanera-2.1.1/japanera/__init__.py
+-rw-rw-rw-   0        0        0    25455 2023-03-07 06:42:42.000000 Japanera-2.1.1/japanera/era_data.py
+-rw-rw-rw-   0        0        0    16298 2023-03-07 07:59:24.000000 Japanera-2.1.1/japanera/japanera.py
+-rw-rw-rw-   0        0        0    25593 2024-03-13 11:02:53.000000 Japanera-2.1.1/japanera/parser.py
+-rw-rw-rw-   0        0        0       42 2024-03-13 11:14:23.809735 Japanera-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1776 2024-03-13 11:08:45.000000 Japanera-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-13 11:14:23.805186 Japanera-2.1.1/tests/
+-rw-rw-rw-   0        0        0     6364 2023-03-07 08:03:07.000000 Japanera-2.1.1/tests/test.py
+-rw-rw-rw-   0        0        0     1488 2023-03-07 08:02:45.000000 Japanera-2.1.1/tests/test_era_data.py
+-rw-rw-rw-   0        0        0    20664 2023-03-07 08:07:21.000000 Japanera-2.1.1/tests/test_parser.py
```

### Comparing `Japanera-2.1.0/Japanera.egg-info/PKG-INFO` & `Japanera-2.1.1/Japanera.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: Japanera
-Version: 2.1.0
+Version: 2.1.1
 Summary: Easy japanese era tool
 Home-page: https://github.com/nagataaaas/Japanera
 Author: Yamato Nagata
-Author-email: nagata@mail.nagata.pro
+Author-email: nagata@nagata.pro
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: kanjize==1.4.0
 
 
 Easy japanese era tool
 ----------------------
 Powered by [Yamato Nagata](https://twitter.com/514YJ)
 
 [GitHub](https://github.com/delta114514/Japanera)
```

### Comparing `Japanera-2.1.0/LICENSE` & `Japanera-2.1.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) 2023 Yamato Nagata
+Copyright (c) 2024 Yamato Nagata
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `Japanera-2.1.0/PKG-INFO` & `Japanera-2.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: Japanera
-Version: 2.1.0
+Version: 2.1.1
 Summary: Easy japanese era tool
 Home-page: https://github.com/nagataaaas/Japanera
 Author: Yamato Nagata
-Author-email: nagata@mail.nagata.pro
+Author-email: nagata@nagata.pro
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: kanjize==1.4.0
 
 
 Easy japanese era tool
 ----------------------
 Powered by [Yamato Nagata](https://twitter.com/514YJ)
 
 [GitHub](https://github.com/delta114514/Japanera)
```

### Comparing `Japanera-2.1.0/README.md` & `Japanera-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Japanera-2.1.0/japanera/__init__.py` & `Japanera-2.1.1/japanera/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Easy japanese era tool
     All Information's source is [Wikipedia Page](https://ja.wikipedia.org/wiki/%E5%85%83%E5%8F%B7%E4%B8%80%E8%A6%A7_(%E6%97%A5%E6%9C%AC))
     Powered by [Yamato Nagata](https://twitter.com/514YJ)
 
     [GitHub](https://github.com/nagataaaas/Japanera)
     [ReadTheDocs](https://japanera.readthedocs.io/en/latest/)
 
-    :copyright: (c) 2019-2023 by Yamato Nagata.
+    :copyright: (c) 2019-2024 by Yamato Nagata.
     :license: MIT.
 """
 
 from .__about__ import __version__
 from .japanera import (Era, EraDate, EraDateTime, ERA_DATA_COMMON, ERA_DATA_DAIKAKUJI, ERA_DATA_JIMYOUIN,
                        ERA_DATA_GENERAL)
 from .era_data import (EraType)
```

### Comparing `Japanera-2.1.0/japanera/era_data.py` & `Japanera-2.1.1/japanera/era_data.py`

 * *Files identical despite different names*

### Comparing `Japanera-2.1.0/japanera/japanera.py` & `Japanera-2.1.1/japanera/japanera.py`

 * *Files identical despite different names*

### Comparing `Japanera-2.1.0/japanera/parser.py` & `Japanera-2.1.1/japanera/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import calendar
 import datetime
 import time
+from _strptime import (_CACHE_MAX_SIZE, IGNORECASE, LocaleTime, _cache_lock,
+                       _calc_julian_from_U_or_W, _getlang, _regex_cache,
+                       re_compile, re_escape)
 from calendar import monthrange
 from collections import defaultdict
 from typing import List, Optional, Set, Tuple
 
-from _strptime import (_CACHE_MAX_SIZE, IGNORECASE, LocaleTime, _cache_lock,
-                       _calc_julian_from_U_or_W, _getlang, _regex_cache,
-                       re_compile, re_escape)
 from kanjize import kanji2number
 
 _ERA_DATA_COMMON, _ERA_DATA_GENERAL, _ERA_DATA_DAIKAKUJI, _ERA_DATA_JIMYOUIN = [], [], [], []
 
 _era_kanji_dict = defaultdict(set)
 _era_alphabet_dict = defaultdict(set)
 _era_alphabet_vowel_shortened_dict = defaultdict(set)
@@ -436,18 +436,18 @@
             year, julian = _calc_julian_from_V(iso_year, iso_week, weekday + 1)
         if julian is not None and julian <= 0:
             year -= 1
             yday = 366 if calendar.isleap(year) else 365
             julian += yday
     return (era_kanji, era_english, era_english_vowel_shortened,
             era_head, relative_year), \
-           (year, month, day,
-            hour, minute, second,
-            weekday, julian, tz, tzname,
-            gmtoff), fraction, gmtoff_fraction
+        (year, month, day,
+         hour, minute, second,
+         weekday, julian, tz, tzname,
+         gmtoff), fraction, gmtoff_fraction
 
 
 def find_era_and_date(era_kanji: Optional[str] = None,
                       era_english: Optional[str] = None,
                       era_english_vowel_shortened: Optional[str] = None,
                       era_head_english: Optional[str] = None,
                       absolute_year: Optional[int] = None,
@@ -555,15 +555,15 @@
     Find all eras that contains `year`.
     Args:
         year: year to find
 
     Returns: set of Era that contains `year`
     """
 
-    def _find_first_era_after_year_index(era_list: list["Era"]) -> int:
+    def _find_first_era_after_year_index(era_list: List["Era"]) -> int:
         # return the index of first era that starts after `year`
         ok = len(era_list)
         ng = -1
         while abs(ok - ng) > 1:
             mid = (ok + ng) // 2
             if era_list[mid].since.year <= year:
                 ng = mid
```

### Comparing `Japanera-2.1.0/setup.py` & `Japanera-2.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
       author_email=about["__author_email__"],
       description=about["__description__"],
       long_description=__doc__,
       long_description_content_type="text/markdown",
       install_requires=["kanjize==1.4.0"],
       packages=["japanera"],
       zip_safe=False,
+      setup_requires=['wheel'],
       platforms="any",
       classifiers=[
           "Development Status :: 4 - Beta",
           "Environment :: Other Environment",
           "Intended Audience :: Developers",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
```

