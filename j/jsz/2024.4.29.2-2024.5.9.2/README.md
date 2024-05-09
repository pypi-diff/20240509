# Comparing `tmp/jsz-2024.4.29.2.tar.gz` & `tmp/jsz-2024.5.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsz-2024.4.29.2.tar", last modified: Mon Apr 29 12:44:02 2024, max compression
+gzip compressed data, was "jsz-2024.5.9.2.tar", last modified: Thu May  9 15:40:15 2024, max compression
```

## Comparing `jsz-2024.4.29.2.tar` & `jsz-2024.5.9.2.tar`

### file list

```diff
@@ -1,5 +1,16 @@
--rw-r--r--   0        0        0      682 2024-04-29 12:44:02.192504 jsz-2024.4.29.2/pyproject.toml
--rw-r--r--   0        0        0      335 2024-04-29 12:38:56.293265 jsz-2024.4.29.2/src/jsz/__init__.py
--rw-r--r--   0        0        0     4366 2024-04-21 16:16:14.272168 jsz-2024.4.29.2/src/jsz/newpool.py
--rw-r--r--   0        0        0    19767 2024-04-29 12:24:48.871056 jsz-2024.4.29.2/src/jsz/tools.py
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 jsz-2024.4.29.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 15:40:15.162739 jsz-2024.5.9.2/
+-rw-rw-rw-   0        0        0      854 2024-05-09 15:40:15.161749 jsz-2024.5.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0      128 2024-05-09 15:00:28.000000 jsz-2024.5.9.2/README.md
+-rw-rw-rw-   0        0        0      645 2024-05-09 15:17:28.000000 jsz-2024.5.9.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 15:40:15.163740 jsz-2024.5.9.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-09 15:40:15.140010 jsz-2024.5.9.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-09 15:40:15.145378 jsz-2024.5.9.2/src/jsz/
+-rw-rw-rw-   0        0        0      304 2024-04-29 13:27:07.000000 jsz-2024.5.9.2/src/jsz/__init__.py
+-rw-rw-rw-   0        0        0     4366 2024-04-21 16:16:14.000000 jsz-2024.5.9.2/src/jsz/newpool.py
+-rw-rw-rw-   0        0        0    19859 2024-05-09 14:59:07.000000 jsz-2024.5.9.2/src/jsz/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-09 15:40:15.160731 jsz-2024.5.9.2/src/jsz.egg-info/
+-rw-rw-rw-   0        0        0      854 2024-05-09 15:40:15.000000 jsz-2024.5.9.2/src/jsz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-05-09 15:40:15.000000 jsz-2024.5.9.2/src/jsz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 15:40:15.000000 jsz-2024.5.9.2/src/jsz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2024-05-09 15:40:15.000000 jsz-2024.5.9.2/src/jsz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-09 15:40:15.000000 jsz-2024.5.9.2/src/jsz.egg-info/top_level.txt
```

### Comparing `jsz-2024.4.29.2/src/jsz/newpool.py` & `jsz-2024.5.9.2/src/jsz/newpool.py`

 * *Files identical despite different names*

### Comparing `jsz-2024.4.29.2/src/jsz/tools.py` & `jsz-2024.5.9.2/src/jsz/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,44 +25,48 @@
     parse_qsl,
 )
 from pypdf import PdfReader
 from faker import Faker
 from rich import print
 from rich.progress import Progress, track
 from rich.console import Console
+from rich.columns import Columns
 from rich.markdown import Markdown
 from rich.panel import Panel
 from rich.rule import Rule
 from rich.status import Status
 from rich.table import Table
 from rich.pretty import pprint
 import datetime
 import time
 from dateutil.parser import parse as timeparse
+from dateparser import parse as timeparse2
 from bs4 import BeautifulSoup, element
 import re
 import html2text
 import hashlib
 import base64
 from pymongo import MongoClient
 import oss2
-from parsel import Selector, css2xpath
+from parsel import Selector
 
 
 __all__ = [
     "base64_decode",
     "base64_encode",
     "bs_get_text",
     "bs_get_text2",
     "bs_html",
-    "css2xpath",
+    "clear",
+    "Columns",
     "connect_to_mongodb",
     "date_next",
     "fake",
     "fromtimestamp",
+    "hashlib",
     "html2md",
     "httpx",
     "listdir",
     "logger",
     "Markdown",
     "md5",
     "now",
@@ -80,23 +84,23 @@
     "quote",
     "randint",
     "re",
     "read_json",
     "retry",
     "Rule",
     "send_bot",
-    "sha256",
     "sleep",
     "sleep_progress",
     "Status",
     "Selector",
     "Table",
     "time_next",
     "timeit",
     "timeparse",
+    "timeparse2",
     "timestamp",
     "to_excel",
     "to_json",
     "today",
     "tongji_content",
     "track",
     "ua",
@@ -193,14 +197,24 @@
 fake = Faker()
 fake.zh = Faker("zh")
 
 console = Console()
 print_exception = console.print_exception
 
 
+def clear():
+    """
+    清屏
+    """
+    if os.name == "nt":
+        os.system("cls")
+    else:
+        os.system("clear")
+
+
 def ua(version_from=101, version_to=125):
     """
     随机ua
 
     chrome 版本101-125
     """
     return fake.chrome(
@@ -229,21 +243,14 @@
 def md5(string: bytes):
     if isinstance(string, str):
         string = string.encode()
     result = hashlib.md5(string).hexdigest()
     return result
 
 
-def sha256(string: bytes):
-    if isinstance(string, str):
-        string = string.encode()
-    result = hashlib.sha256(string).hexdigest()
-    return result
-
-
 def base64_encode(string: bytes):
     """
     base64编码
     """
     if isinstance(string, str):
         string = string.encode()
     return base64.b64encode(string).decode()
@@ -325,19 +332,19 @@
 
 def tongji_content(content: str, keywords: list[str], strict=False, to_dict=False):
     """
     统计每篇文章中关键词出现次数
 
     - content: 需要统计的文本。
     - keywords: 需要统计的关键词。
-    - strict: 默认模糊搜索, True 为严格搜索。
+    - strict: 是否严格模式，默认False 忽略大小写, True 不忽略。
     - to_dict: 是否导出为字典格式。
     """
     keyword_tongji_list = []
-    for keyword in keywords:
+    for keyword in set(keywords):
         if not strict:
             p1 = content.upper().count(keyword.upper())
         else:
             p1 = content.count(keyword)
         if p1 > 0:
             keyword_tongji_list.append([keyword, p1])
     if to_dict:
```

