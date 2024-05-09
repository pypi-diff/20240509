# Comparing `tmp/sparklestock-0.0.0.3.tar.gz` & `tmp/sparklestock-0.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparklestock-0.0.0.3.tar", last modified: Thu May  9 01:43:55 2024, max compression
+gzip compressed data, was "sparklestock-0.0.0.4.tar", last modified: Thu May  9 01:52:35 2024, max compression
```

## Comparing `sparklestock-0.0.0.3.tar` & `sparklestock-0.0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 01:43:55.899011 sparklestock-0.0.0.3/
--rw-r--r--   0 seyong     (501) staff       (20)      439 2024-05-09 01:43:55.899075 sparklestock-0.0.0.3/PKG-INFO
--rw-r--r--   0 seyong     (501) staff       (20)       46 2024-05-08 13:10:42.000000 sparklestock-0.0.0.3/README.md
--rw-r--r--   0 seyong     (501) staff       (20)      270 2024-04-05 11:07:26.000000 sparklestock-0.0.0.3/pyproject.toml
--rw-r--r--   0 seyong     (501) staff       (20)       79 2024-05-09 01:43:55.899269 sparklestock-0.0.0.3/setup.cfg
--rw-r--r--   0 seyong     (501) staff       (20)      720 2024-05-09 01:43:54.000000 sparklestock-0.0.0.3/setup.py
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 01:43:55.898267 sparklestock-0.0.0.3/sparklestock/
--rw-r--r--   0 seyong     (501) staff       (20)     2184 2024-05-09 01:42:15.000000 sparklestock-0.0.0.3/sparklestock/Stock.py
--rw-r--r--   0 seyong     (501) staff       (20)       58 2024-05-08 13:55:13.000000 sparklestock-0.0.0.3/sparklestock/__init__.py
--rw-r--r--   0 seyong     (501) staff       (20)       23 2024-05-09 01:43:54.000000 sparklestock-0.0.0.3/sparklestock/__version__.py
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 01:43:55.898904 sparklestock-0.0.0.3/sparklestock.egg-info/
--rw-r--r--   0 seyong     (501) staff       (20)      439 2024-05-09 01:43:55.000000 sparklestock-0.0.0.3/sparklestock.egg-info/PKG-INFO
--rw-r--r--   0 seyong     (501) staff       (20)      297 2024-05-09 01:43:55.000000 sparklestock-0.0.0.3/sparklestock.egg-info/SOURCES.txt
--rw-r--r--   0 seyong     (501) staff       (20)        1 2024-05-09 01:43:55.000000 sparklestock-0.0.0.3/sparklestock.egg-info/dependency_links.txt
--rw-r--r--   0 seyong     (501) staff       (20)        9 2024-05-09 01:43:55.000000 sparklestock-0.0.0.3/sparklestock.egg-info/requires.txt
--rw-r--r--   0 seyong     (501) staff       (20)       13 2024-05-09 01:43:55.000000 sparklestock-0.0.0.3/sparklestock.egg-info/top_level.txt
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 01:52:35.513949 sparklestock-0.0.0.4/
+-rw-r--r--   0 seyong     (501) staff       (20)      439 2024-05-09 01:52:35.514015 sparklestock-0.0.0.4/PKG-INFO
+-rw-r--r--   0 seyong     (501) staff       (20)       46 2024-05-08 13:10:42.000000 sparklestock-0.0.0.4/README.md
+-rw-r--r--   0 seyong     (501) staff       (20)      270 2024-04-05 11:07:26.000000 sparklestock-0.0.0.4/pyproject.toml
+-rw-r--r--   0 seyong     (501) staff       (20)       79 2024-05-09 01:52:35.514211 sparklestock-0.0.0.4/setup.cfg
+-rw-r--r--   0 seyong     (501) staff       (20)      720 2024-05-09 01:52:22.000000 sparklestock-0.0.0.4/setup.py
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 01:52:35.513276 sparklestock-0.0.0.4/sparklestock/
+-rw-r--r--   0 seyong     (501) staff       (20)     2320 2024-05-09 01:51:54.000000 sparklestock-0.0.0.4/sparklestock/Stock.py
+-rw-r--r--   0 seyong     (501) staff       (20)       58 2024-05-08 13:55:13.000000 sparklestock-0.0.0.4/sparklestock/__init__.py
+-rw-r--r--   0 seyong     (501) staff       (20)       23 2024-05-09 01:52:22.000000 sparklestock-0.0.0.4/sparklestock/__version__.py
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 01:52:35.513842 sparklestock-0.0.0.4/sparklestock.egg-info/
+-rw-r--r--   0 seyong     (501) staff       (20)      439 2024-05-09 01:52:35.000000 sparklestock-0.0.0.4/sparklestock.egg-info/PKG-INFO
+-rw-r--r--   0 seyong     (501) staff       (20)      297 2024-05-09 01:52:35.000000 sparklestock-0.0.0.4/sparklestock.egg-info/SOURCES.txt
+-rw-r--r--   0 seyong     (501) staff       (20)        1 2024-05-09 01:52:35.000000 sparklestock-0.0.0.4/sparklestock.egg-info/dependency_links.txt
+-rw-r--r--   0 seyong     (501) staff       (20)        9 2024-05-09 01:52:35.000000 sparklestock-0.0.0.4/sparklestock.egg-info/requires.txt
+-rw-r--r--   0 seyong     (501) staff       (20)       13 2024-05-09 01:52:35.000000 sparklestock-0.0.0.4/sparklestock.egg-info/top_level.txt
```

### Comparing `sparklestock-0.0.0.3/setup.py` & `sparklestock-0.0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sparklestock", ## 소문자 영단어
-    version="0.0.0.3", ##
+    version="0.0.0.4", ##
     author="Seyong Ahn", ## ex) Sunkyeong Lee
     author_email="hiseyong1008@gmail.com", ##
     description="sparkle stock package", ##
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hiseyong", ##
     install_requires=['requests'],
```

### Comparing `sparklestock-0.0.0.3/sparklestock/Stock.py` & `sparklestock-0.0.0.4/sparklestock/Stock.py`

 * *Files 18% similar despite different names*

```diff
@@ -65,9 +65,12 @@
     def check_my_asset(self):
         self.check_login()
 
         checking_status = post(self.address+'/api/check', json={'id':self.id, 'pw':self.pw}).text
         if checking_status[0] != '{':
             raise ConnectionError(checking_status)
         self.asset = eval(checking_status)
+        self.asset['money'] = int(self.asset['money'])
+        self.asset['stock'] = int(self.asset['stock'])
         self.money = self.asset['money']
-        self.stock = self.asset['stock']
+        self.stock = self.asset['stock']
+        return self.asset
```

