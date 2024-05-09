# Comparing `tmp/sparklestock-0.0.0.5.tar.gz` & `tmp/sparklestock-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparklestock-0.0.0.5.tar", last modified: Thu May  9 01:55:15 2024, max compression
+gzip compressed data, was "sparklestock-0.0.0.6.tar", last modified: Thu May  9 02:17:55 2024, max compression
```

## Comparing `sparklestock-0.0.0.5.tar` & `sparklestock-0.0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 01:55:15.733008 sparklestock-0.0.0.5/
--rw-r--r--   0 seyong     (501) staff       (20)      438 2024-05-09 01:55:15.733081 sparklestock-0.0.0.5/PKG-INFO
--rw-r--r--   0 seyong     (501) staff       (20)       45 2024-05-09 01:53:19.000000 sparklestock-0.0.0.5/README.md
--rw-r--r--   0 seyong     (501) staff       (20)      270 2024-04-05 11:07:26.000000 sparklestock-0.0.0.5/pyproject.toml
--rw-r--r--   0 seyong     (501) staff       (20)       79 2024-05-09 01:55:15.733288 sparklestock-0.0.0.5/setup.cfg
--rw-r--r--   0 seyong     (501) staff       (20)      720 2024-05-09 01:55:13.000000 sparklestock-0.0.0.5/setup.py
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 01:55:15.732246 sparklestock-0.0.0.5/sparklestock/
--rw-r--r--   0 seyong     (501) staff       (20)     2296 2024-05-09 01:55:13.000000 sparklestock-0.0.0.5/sparklestock/Stock.py
--rw-r--r--   0 seyong     (501) staff       (20)       58 2024-05-08 13:55:13.000000 sparklestock-0.0.0.5/sparklestock/__init__.py
--rw-r--r--   0 seyong     (501) staff       (20)       23 2024-05-09 01:55:13.000000 sparklestock-0.0.0.5/sparklestock/__version__.py
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 01:55:15.732907 sparklestock-0.0.0.5/sparklestock.egg-info/
--rw-r--r--   0 seyong     (501) staff       (20)      438 2024-05-09 01:55:15.000000 sparklestock-0.0.0.5/sparklestock.egg-info/PKG-INFO
--rw-r--r--   0 seyong     (501) staff       (20)      297 2024-05-09 01:55:15.000000 sparklestock-0.0.0.5/sparklestock.egg-info/SOURCES.txt
--rw-r--r--   0 seyong     (501) staff       (20)        1 2024-05-09 01:55:15.000000 sparklestock-0.0.0.5/sparklestock.egg-info/dependency_links.txt
--rw-r--r--   0 seyong     (501) staff       (20)        9 2024-05-09 01:55:15.000000 sparklestock-0.0.0.5/sparklestock.egg-info/requires.txt
--rw-r--r--   0 seyong     (501) staff       (20)       13 2024-05-09 01:55:15.000000 sparklestock-0.0.0.5/sparklestock.egg-info/top_level.txt
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 02:17:55.286874 sparklestock-0.0.0.6/
+-rw-r--r--   0 seyong     (501) staff       (20)      462 2024-05-09 02:17:55.286803 sparklestock-0.0.0.6/PKG-INFO
+-rw-r--r--   0 seyong     (501) staff       (20)       45 2024-05-09 01:53:19.000000 sparklestock-0.0.0.6/README.md
+-rw-r--r--   0 seyong     (501) staff       (20)      270 2024-04-05 11:07:26.000000 sparklestock-0.0.0.6/pyproject.toml
+-rw-r--r--   0 seyong     (501) staff       (20)       79 2024-05-09 02:17:55.287095 sparklestock-0.0.0.6/setup.cfg
+-rw-r--r--   0 seyong     (501) staff       (20)      720 2024-05-09 02:16:31.000000 sparklestock-0.0.0.6/setup.py
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 02:17:55.285472 sparklestock-0.0.0.6/sparklestock/
+-rw-r--r--   0 seyong     (501) staff       (20)     2298 2024-05-09 02:15:06.000000 sparklestock-0.0.0.6/sparklestock/Stock.py
+-rw-r--r--   0 seyong     (501) staff       (20)       58 2024-05-08 13:55:13.000000 sparklestock-0.0.0.6/sparklestock/__init__.py
+-rw-r--r--   0 seyong     (501) staff       (20)       23 2024-05-09 02:16:31.000000 sparklestock-0.0.0.6/sparklestock/__version__.py
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 02:17:55.286587 sparklestock-0.0.0.6/sparklestock.egg-info/
+-rw-r--r--   0 seyong     (501) staff       (20)      462 2024-05-09 02:17:55.000000 sparklestock-0.0.0.6/sparklestock.egg-info/PKG-INFO
+-rw-r--r--   0 seyong     (501) staff       (20)      297 2024-05-09 02:17:55.000000 sparklestock-0.0.0.6/sparklestock.egg-info/SOURCES.txt
+-rw-r--r--   0 seyong     (501) staff       (20)        1 2024-05-09 02:17:55.000000 sparklestock-0.0.0.6/sparklestock.egg-info/dependency_links.txt
+-rw-r--r--   0 seyong     (501) staff       (20)        9 2024-05-09 02:17:55.000000 sparklestock-0.0.0.6/sparklestock.egg-info/requires.txt
+-rw-r--r--   0 seyong     (501) staff       (20)       13 2024-05-09 02:17:55.000000 sparklestock-0.0.0.6/sparklestock.egg-info/top_level.txt
```

### Comparing `sparklestock-0.0.0.5/setup.py` & `sparklestock-0.0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sparklestock", ## 소문자 영단어
-    version="0.0.0.5", ##
+    version="0.0.0.6", ##
     author="Seyong Ahn", ## ex) Sunkyeong Lee
     author_email="hiseyong1008@gmail.com", ##
     description="sparkle stock package", ##
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hiseyong", ##
     install_requires=['requests'],
```

### Comparing `sparklestock-0.0.0.5/sparklestock/Stock.py` & `sparklestock-0.0.0.6/sparklestock/Stock.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def get_current_price(self) -> int:
         self.check_login()
 
         response = get(self.address+'/api/getprice').text
         if response == '"close"':
             raise ConnectionError("폐장되었습니다.")
-        self.price = int(response)
+        self.price = float(response)
         return self.price
 
 
     def get_price_history(self) -> list:
         self.check_login()
 
         price_history = get(self.address+'/api/gethistory').text
```

