# Comparing `tmp/sparklestock-0.0.0.2.tar.gz` & `tmp/sparklestock-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparklestock-0.0.0.2.tar", last modified: Wed May  8 14:20:28 2024, max compression
+gzip compressed data, was "sparklestock-0.0.0.3.tar", last modified: Thu May  9 01:43:55 2024, max compression
```

## Comparing `sparklestock-0.0.0.2.tar` & `sparklestock-0.0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-08 14:20:28.175861 sparklestock-0.0.0.2/
--rw-r--r--   0 seyong     (501) staff       (20)      439 2024-05-08 14:20:28.175936 sparklestock-0.0.0.2/PKG-INFO
--rw-r--r--   0 seyong     (501) staff       (20)       46 2024-05-08 13:10:42.000000 sparklestock-0.0.0.2/README.md
--rw-r--r--   0 seyong     (501) staff       (20)      270 2024-04-05 11:07:26.000000 sparklestock-0.0.0.2/pyproject.toml
--rw-r--r--   0 seyong     (501) staff       (20)       79 2024-05-08 14:20:28.176132 sparklestock-0.0.0.2/setup.cfg
--rw-r--r--   0 seyong     (501) staff       (20)      720 2024-05-08 14:19:05.000000 sparklestock-0.0.0.2/setup.py
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-08 14:20:28.174884 sparklestock-0.0.0.2/sparklestock/
--rw-r--r--   0 seyong     (501) staff       (20)     2034 2024-05-08 12:44:44.000000 sparklestock-0.0.0.2/sparklestock/Stock.py
--rw-r--r--   0 seyong     (501) staff       (20)       58 2024-05-08 13:55:13.000000 sparklestock-0.0.0.2/sparklestock/__init__.py
--rw-r--r--   0 seyong     (501) staff       (20)       23 2024-05-08 14:19:05.000000 sparklestock-0.0.0.2/sparklestock/__version__.py
-drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-08 14:20:28.175738 sparklestock-0.0.0.2/sparklestock.egg-info/
--rw-r--r--   0 seyong     (501) staff       (20)      439 2024-05-08 14:20:28.000000 sparklestock-0.0.0.2/sparklestock.egg-info/PKG-INFO
--rw-r--r--   0 seyong     (501) staff       (20)      297 2024-05-08 14:20:28.000000 sparklestock-0.0.0.2/sparklestock.egg-info/SOURCES.txt
--rw-r--r--   0 seyong     (501) staff       (20)        1 2024-05-08 14:20:28.000000 sparklestock-0.0.0.2/sparklestock.egg-info/dependency_links.txt
--rw-r--r--   0 seyong     (501) staff       (20)        9 2024-05-08 14:20:28.000000 sparklestock-0.0.0.2/sparklestock.egg-info/requires.txt
--rw-r--r--   0 seyong     (501) staff       (20)       13 2024-05-08 14:20:28.000000 sparklestock-0.0.0.2/sparklestock.egg-info/top_level.txt
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 01:43:55.899011 sparklestock-0.0.0.3/
+-rw-r--r--   0 seyong     (501) staff       (20)      439 2024-05-09 01:43:55.899075 sparklestock-0.0.0.3/PKG-INFO
+-rw-r--r--   0 seyong     (501) staff       (20)       46 2024-05-08 13:10:42.000000 sparklestock-0.0.0.3/README.md
+-rw-r--r--   0 seyong     (501) staff       (20)      270 2024-04-05 11:07:26.000000 sparklestock-0.0.0.3/pyproject.toml
+-rw-r--r--   0 seyong     (501) staff       (20)       79 2024-05-09 01:43:55.899269 sparklestock-0.0.0.3/setup.cfg
+-rw-r--r--   0 seyong     (501) staff       (20)      720 2024-05-09 01:43:54.000000 sparklestock-0.0.0.3/setup.py
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 01:43:55.898267 sparklestock-0.0.0.3/sparklestock/
+-rw-r--r--   0 seyong     (501) staff       (20)     2184 2024-05-09 01:42:15.000000 sparklestock-0.0.0.3/sparklestock/Stock.py
+-rw-r--r--   0 seyong     (501) staff       (20)       58 2024-05-08 13:55:13.000000 sparklestock-0.0.0.3/sparklestock/__init__.py
+-rw-r--r--   0 seyong     (501) staff       (20)       23 2024-05-09 01:43:54.000000 sparklestock-0.0.0.3/sparklestock/__version__.py
+drwxr-xr-x   0 seyong     (501) staff       (20)        0 2024-05-09 01:43:55.898904 sparklestock-0.0.0.3/sparklestock.egg-info/
+-rw-r--r--   0 seyong     (501) staff       (20)      439 2024-05-09 01:43:55.000000 sparklestock-0.0.0.3/sparklestock.egg-info/PKG-INFO
+-rw-r--r--   0 seyong     (501) staff       (20)      297 2024-05-09 01:43:55.000000 sparklestock-0.0.0.3/sparklestock.egg-info/SOURCES.txt
+-rw-r--r--   0 seyong     (501) staff       (20)        1 2024-05-09 01:43:55.000000 sparklestock-0.0.0.3/sparklestock.egg-info/dependency_links.txt
+-rw-r--r--   0 seyong     (501) staff       (20)        9 2024-05-09 01:43:55.000000 sparklestock-0.0.0.3/sparklestock.egg-info/requires.txt
+-rw-r--r--   0 seyong     (501) staff       (20)       13 2024-05-09 01:43:55.000000 sparklestock-0.0.0.3/sparklestock.egg-info/top_level.txt
```

### Comparing `sparklestock-0.0.0.2/setup.py` & `sparklestock-0.0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sparklestock", ## 소문자 영단어
-    version="0.0.0.2", ##
+    version="0.0.0.3", ##
     author="Seyong Ahn", ## ex) Sunkyeong Lee
     author_email="hiseyong1008@gmail.com", ##
     description="sparkle stock package", ##
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hiseyong", ##
     install_requires=['requests'],
```

### Comparing `sparklestock-0.0.0.2/sparklestock/Stock.py` & `sparklestock-0.0.0.3/sparklestock/Stock.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,25 +23,27 @@
             raise ValueError("비밀번호가 틀렸습니다.")
 
 
     def get_current_price(self) -> int:
         self.check_login()
 
         response = get(self.address+'/api/getprice').text
-        if response == "close":
+        print(response)
+        if response == '"close"':
             raise ConnectionError("폐장되었습니다.")
         self.price = int(response)
         return self.price
 
 
     def get_price_history(self) -> list:
         self.check_login()
 
         price_history = get(self.address+'/api/gethistory').text
-        return eval(price_history)
+        self.history = eval(price_history)
+        return self.history
 
 
     def buy_stock(self, amount:int):
         self.check_login()
 
         buying_status = post(self.address+'/api/buy', json={'id':self.id, 'pw':self.pw, 'amount':str(amount)}).text
         if buying_status == 'true':
@@ -62,8 +64,10 @@
 
     def check_my_asset(self):
         self.check_login()
 
         checking_status = post(self.address+'/api/check', json={'id':self.id, 'pw':self.pw}).text
         if checking_status[0] != '{':
             raise ConnectionError(checking_status)
-        return eval(checking_status)
+        self.asset = eval(checking_status)
+        self.money = self.asset['money']
+        self.stock = self.asset['stock']
```

