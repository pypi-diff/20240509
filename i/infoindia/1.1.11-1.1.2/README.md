# Comparing `tmp/infoindia-1.1.11.tar.gz` & `tmp/infoindia-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infoindia-1.1.11.tar", last modified: Thu May  9 14:55:44 2024, max compression
+gzip compressed data, was "infoindia-1.1.2.tar", last modified: Wed May  8 14:22:30 2024, max compression
```

## Comparing `infoindia-1.1.11.tar` & `infoindia-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 14:55:44.456509 infoindia-1.1.11/
--rw-rw-rw-   0        0        0     1529 2024-05-09 14:55:44.456509 infoindia-1.1.11/PKG-INFO
--rw-rw-rw-   0        0        0     1120 2024-05-09 14:54:19.000000 infoindia-1.1.11/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 14:55:44.425207 infoindia-1.1.11/infoindia/
--rw-rw-rw-   0        0        0      142 2024-05-08 14:21:05.000000 infoindia-1.1.11/infoindia/__init__.py
--rw-rw-rw-   0        0        0     2166 2024-05-09 14:52:55.000000 infoindia-1.1.11/infoindia/infoindia.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:55:44.456509 infoindia-1.1.11/infoindia.egg-info/
--rw-rw-rw-   0        0        0     1529 2024-05-09 14:55:44.000000 infoindia-1.1.11/infoindia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2024-05-09 14:55:44.000000 infoindia-1.1.11/infoindia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 14:55:44.000000 infoindia-1.1.11/infoindia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 14:55:44.000000 infoindia-1.1.11/infoindia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-09 14:55:44.000000 infoindia-1.1.11/infoindia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 14:55:44.456509 infoindia-1.1.11/setup.cfg
--rw-rw-rw-   0        0        0      688 2024-05-09 14:53:38.000000 infoindia-1.1.11/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:22:30.146660 infoindia-1.1.2/
+-rw-rw-rw-   0        0        0     1472 2024-05-08 14:22:30.146660 infoindia-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1064 2024-05-08 14:13:34.000000 infoindia-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 14:22:30.109575 infoindia-1.1.2/infoindia/
+-rw-rw-rw-   0        0        0      142 2024-05-08 14:21:05.000000 infoindia-1.1.2/infoindia/__init__.py
+-rw-rw-rw-   0        0        0     2137 2024-05-08 13:47:28.000000 infoindia-1.1.2/infoindia/infoindia.py
+drwxrwxrwx   0        0        0        0 2024-05-08 14:22:30.140416 infoindia-1.1.2/infoindia.egg-info/
+-rw-rw-rw-   0        0        0     1472 2024-05-08 14:22:29.000000 infoindia-1.1.2/infoindia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2024-05-08 14:22:29.000000 infoindia-1.1.2/infoindia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 14:22:29.000000 infoindia-1.1.2/infoindia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-08 14:22:29.000000 infoindia-1.1.2/infoindia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-08 14:22:29.000000 infoindia-1.1.2/infoindia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-08 14:22:30.147921 infoindia-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      687 2024-05-08 14:22:15.000000 infoindia-1.1.2/setup.py
```

### Comparing `infoindia-1.1.11/PKG-INFO` & `infoindia-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: infoindia
-Version: 1.1.11
+Version: 1.1.2
 Summary: Wrapper for State Data APIs
 Home-page: https://github.com/NarutoUzumvki/state_data_api
 Author: Vijay Chouhan
 Author-email: vijay977364@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # INFOINDIA
 
-infoindia is a wrapper for [STATE DATA APIs](https://apis.travelrealindia.in).
+infoindia is a wrapper for [STATE DATA APIs](https://apis.travelrealindia.com).
 
 ## API KEY
 
-[Sign Up](https://apis.travelrealindia.in/signup) to get your api_key
-
-Or [Sign In](https://apis.travelrealindia.in/signin) if already a user
+Create a user [here](https://apis.travelrealindia.com/create_user) to get your api_key
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install infoindia.
 
 ```bash
 pip install infoindia
```

### Comparing `infoindia-1.1.11/README.md` & `infoindia-1.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # INFOINDIA
 
-infoindia is a wrapper for [STATE DATA APIs](https://apis.travelrealindia.in).
+infoindia is a wrapper for [STATE DATA APIs](https://apis.travelrealindia.com).
 
 ## API KEY
 
-[Sign Up](https://apis.travelrealindia.in/signup) to get your api_key
-
-Or [Sign In](https://apis.travelrealindia.in/signin) if already a user
+Create a user [here](https://apis.travelrealindia.com/create_user) to get your api_key
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install infoindia.
 
 ```bash
 pip install infoindia
```

### Comparing `infoindia-1.1.11/infoindia/infoindia.py` & `infoindia-1.1.2/infoindia/infoindia.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     def fetch(self) -> dict:
         if not self.code:
             return {"error": "CODE is required"}
         try:
             payload = {"api_key": get_api_key()}
             endpoint = f'{BASE_URL}/{self.var}/{self.code}/retrieve'
             response = requests.get(endpoint, json=payload).text
-            print(response)
             return json.loads(response)
         except:
             return {"error": "Failed to connect to host"}
 
 
 class City(Base):
     def __init__(self, code=None):
```

### Comparing `infoindia-1.1.11/infoindia.egg-info/PKG-INFO` & `infoindia-1.1.2/infoindia.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: infoindia
-Version: 1.1.11
+Version: 1.1.2
 Summary: Wrapper for State Data APIs
 Home-page: https://github.com/NarutoUzumvki/state_data_api
 Author: Vijay Chouhan
 Author-email: vijay977364@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # INFOINDIA
 
-infoindia is a wrapper for [STATE DATA APIs](https://apis.travelrealindia.in).
+infoindia is a wrapper for [STATE DATA APIs](https://apis.travelrealindia.com).
 
 ## API KEY
 
-[Sign Up](https://apis.travelrealindia.in/signup) to get your api_key
-
-Or [Sign In](https://apis.travelrealindia.in/signin) if already a user
+Create a user [here](https://apis.travelrealindia.com/create_user) to get your api_key
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install infoindia.
 
 ```bash
 pip install infoindia
```

### Comparing `infoindia-1.1.11/setup.py` & `infoindia-1.1.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='infoindia',
-    version='1.1.11',
+    version='1.1.2',
     packages=find_packages(),
     install_requires=['requests'],
     author='Vijay Chouhan',
     author_email='vijay977364@gmail.com',
     description='Wrapper for State Data APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

