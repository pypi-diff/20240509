# Comparing `tmp/lyyre-2.6.tar.gz` & `tmp/lyyre-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyyre-2.6.tar", last modified: Wed May  8 13:27:45 2024, max compression
+gzip compressed data, was "lyyre-2.7.tar", last modified: Wed May  8 14:10:03 2024, max compression
```

## Comparing `lyyre-2.6.tar` & `lyyre-2.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:27:45.754865 lyyre-2.6/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyre-2.6/LICENSE
--rw-rw-rw-   0        0        0      156 2024-05-08 13:27:45.754865 lyyre-2.6/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyre-2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 13:27:45.752855 lyyre-2.6/lyyre.egg-info/
--rw-rw-rw-   0        0        0      156 2024-05-08 13:27:45.000000 lyyre-2.6/lyyre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-08 13:27:45.000000 lyyre-2.6/lyyre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:27:45.000000 lyyre-2.6/lyyre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-05-08 13:27:45.000000 lyyre-2.6/lyyre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-08 13:27:45.000000 lyyre-2.6/lyyre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9790 2024-05-08 13:19:36.000000 lyyre-2.6/lyyre.py
--rw-rw-rw-   0        0        0       42 2024-05-08 13:27:45.754865 lyyre-2.6/setup.cfg
--rw-rw-rw-   0        0        0      262 2024-05-08 13:27:44.000000 lyyre-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:10:03.078329 lyyre-2.7/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyre-2.7/LICENSE
+-rw-rw-rw-   0        0        0      156 2024-05-08 14:10:03.078329 lyyre-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyre-2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 14:10:03.076826 lyyre-2.7/lyyre.egg-info/
+-rw-rw-rw-   0        0        0      156 2024-05-08 14:10:02.000000 lyyre-2.7/lyyre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-08 14:10:02.000000 lyyre-2.7/lyyre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 14:10:02.000000 lyyre-2.7/lyyre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        3 2024-05-08 14:10:02.000000 lyyre-2.7/lyyre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-08 14:10:02.000000 lyyre-2.7/lyyre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9789 2024-05-08 14:09:51.000000 lyyre-2.7/lyyre.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 14:10:03.079384 lyyre-2.7/setup.cfg
+-rw-rw-rw-   0        0        0      262 2024-05-08 14:10:02.000000 lyyre-2.7/setup.py
```

### Comparing `lyyre-2.6/LICENSE` & `lyyre-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lyyre-2.6/lyyre.py` & `lyyre-2.7/lyyre.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 import http.client
 from lyylog import log
 import json
 
-
-def format_url_in_ocr_text_include_markdown_img(text,debug=False)
+def format_url_in_ocr_text_include_markdown_img(text,debug=False):
     if debug: print("enter format_ocr_text_include_markdown_img")
     url_pattern = r'!\s?\[\s?(?:screenshot)?\s?\]\s?\((http:?//.*\.(bmp)|(png)|(jpg))'
 
     # 在文本中查找所有匹配的网址
     matches = re.findall(url_pattern, text)
     if len(matches)>0:
         for match in matches:
```

