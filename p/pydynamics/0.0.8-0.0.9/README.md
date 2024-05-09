# Comparing `tmp/pydynamics-0.0.8.tar.gz` & `tmp/pydynamics-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pydynamics-0.0.8.tar", last modified: Wed Aug 14 10:43:48 2019, max compression
+gzip compressed data, was "dist/pydynamics-0.0.9.tar", last modified: Tue May 26 15:29:08 2020, max compression
```

## Comparing `pydynamics-0.0.8.tar` & `pydynamics-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)        0 2019-08-14 10:43:48.000000 pydynamics-0.0.8/
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)     3292 2019-08-14 10:43:48.000000 pydynamics-0.0.8/PKG-INFO
-drwxr-xr-x   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)        0 2019-08-14 10:43:48.000000 pydynamics-0.0.8/pydynamics/
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)     3485 2019-04-26 11:00:02.000000 pydynamics-0.0.8/pydynamics/token.py
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)     4059 2019-04-26 10:59:34.000000 pydynamics-0.0.8/pydynamics/client.py
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)       20 2019-04-26 10:59:34.000000 pydynamics-0.0.8/pydynamics/__init__.py
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)     6983 2019-08-14 10:42:27.000000 pydynamics-0.0.8/pydynamics/querybuilder.py
-drwxr-xr-x   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)        0 2019-08-14 10:43:48.000000 pydynamics-0.0.8/pydynamics.egg-info/
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)     3292 2019-08-14 10:43:48.000000 pydynamics-0.0.8/pydynamics.egg-info/PKG-INFO
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)      278 2019-08-14 10:43:48.000000 pydynamics-0.0.8/pydynamics.egg-info/SOURCES.txt
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)       14 2019-08-14 10:43:48.000000 pydynamics-0.0.8/pydynamics.egg-info/requires.txt
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)       11 2019-08-14 10:43:48.000000 pydynamics-0.0.8/pydynamics.egg-info/top_level.txt
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)        1 2019-08-14 10:43:48.000000 pydynamics-0.0.8/pydynamics.egg-info/dependency_links.txt
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)     2343 2019-04-26 10:59:34.000000 pydynamics-0.0.8/README.md
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)      707 2019-08-14 10:43:15.000000 pydynamics-0.0.8/setup.py
--rw-r--r--   0 dan.goscomb (104810328) HSO\Domain Users (1017296624)       38 2019-08-14 10:43:48.000000 pydynamics-0.0.8/setup.cfg
+drwxr-xr-x   0 dan.goscomb   (501) staff       (20)        0 2020-05-26 15:29:08.000000 pydynamics-0.0.9/
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)     3292 2020-05-26 15:29:08.000000 pydynamics-0.0.9/PKG-INFO
+drwxr-xr-x   0 dan.goscomb   (501) staff       (20)        0 2020-05-26 15:29:08.000000 pydynamics-0.0.9/pydynamics/
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)     3485 2020-05-26 12:33:43.000000 pydynamics-0.0.9/pydynamics/token.py
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)     4947 2020-05-26 13:50:44.000000 pydynamics-0.0.9/pydynamics/client.py
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)       20 2018-12-29 08:11:12.000000 pydynamics-0.0.9/pydynamics/__init__.py
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)     7564 2020-05-26 13:50:28.000000 pydynamics-0.0.9/pydynamics/querybuilder.py
+drwxr-xr-x   0 dan.goscomb   (501) staff       (20)        0 2020-05-26 15:29:08.000000 pydynamics-0.0.9/pydynamics.egg-info/
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)     3292 2020-05-26 15:29:07.000000 pydynamics-0.0.9/pydynamics.egg-info/PKG-INFO
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)      278 2020-05-26 15:29:08.000000 pydynamics-0.0.9/pydynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)       14 2020-05-26 15:29:07.000000 pydynamics-0.0.9/pydynamics.egg-info/requires.txt
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)       11 2020-05-26 15:29:07.000000 pydynamics-0.0.9/pydynamics.egg-info/top_level.txt
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)        1 2020-05-26 15:29:07.000000 pydynamics-0.0.9/pydynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)     2343 2018-12-30 11:29:30.000000 pydynamics-0.0.9/README.md
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)      707 2020-05-26 15:28:43.000000 pydynamics-0.0.9/setup.py
+-rw-r--r--   0 dan.goscomb   (501) staff       (20)       38 2020-05-26 15:29:08.000000 pydynamics-0.0.9/setup.cfg
```

### Comparing `pydynamics-0.0.8/PKG-INFO` & `pydynamics-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydynamics
-Version: 0.0.8
+Version: 0.0.9
 Summary: Talk to On-Prem Dynamics CRM
 Home-page: https://github.com/dangoscomb/pydynamics
 Author: Dan Goscomb
 Author-email: dan@flowplex.co.uk
 License: UNKNOWN
 Description: # PyDynamics
```

### Comparing `pydynamics-0.0.8/pydynamics/token.py` & `pydynamics-0.0.9/pydynamics/token.py`

 * *Files identical despite different names*

### Comparing `pydynamics-0.0.8/pydynamics/client.py` & `pydynamics-0.0.9/pydynamics/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -34,14 +34,33 @@
                 if resp.status_code != 200:
                     raise Exception("Failed to query nextLink")
                 results = results + resp.json()['value']
                 if '@odata.nextLink' in resp.json():
                     nextlink = resp.json()['@odata.nextLink']
                 else:
                     nextlink = None
+
+            cookie = None
+            page = 2
+            if '@Microsoft.Dynamics.CRM.fetchxmlpagingcookie' in resp.json():
+                cookie = resp.json()['@Microsoft.Dynamics.CRM.fetchxmlpagingcookie']
+                query.update_fetchxml_cookie(cookie, page)
+
+            while cookie is not None:
+                page += 1
+                resp = requests.get(self._endpoint + query.buildquery(), headers=self._headers)
+                if resp.status_code != 200:
+                    raise Exception("Failed to query next page")
+                results = results + resp.json()['value']
+                if '@Microsoft.Dynamics.CRM.fetchxmlpagingcookie' in resp.json():
+                    cookie = resp.json()['@Microsoft.Dynamics.CRM.fetchxmlpagingcookie']
+                    query.update_fetchxml_cookie(cookie, page)
+                else:
+                    cookie = None
+
             return results
         else:
             raise Exception("Bad Request")
 
     def update(self, query):
         if not isinstance(query, pydynamics.querybuilder.QueryBuilder):
             raise Exception("Query must be of type QueryBuilder")
```

### Comparing `pydynamics-0.0.8/pydynamics/querybuilder.py` & `pydynamics-0.0.9/pydynamics/querybuilder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import urllib.parse
 import json
+from lxml import etree
+import urllib
+
 
 class QueryBuilder:
 
     def __init__(self, entity: str):
         self._query = None
         self._action = None
         self._fetchxml = None
@@ -91,14 +94,28 @@
     def fetchxml(self, xml: str):
         if self._action is not None or self._action is not None or len(self._filters) > 0:
             raise Exception('FetchXML can not be used in conjunction with other query methods')
 
         self._fetchxml = xml
         return self
 
+    def update_fetchxml_cookie(self, cookie: str, page: int):
+        if self._fetchxml is None:
+            raise Exception('No FetchXML has been set')
+
+        try:
+            xml = etree.fromstring(self._fetchxml)
+            cook = etree.fromstring(cookie)
+            lecookie = urllib.parse.unquote(urllib.parse.unquote(cook.get('pagingcookie')))
+            xml.set('page', '%d' % page)
+            xml.set('paging-cookie', lecookie)
+            self._fetchxml = etree.tostring(xml)
+        except Exception as e:
+            raise e
+
     def data(self, data):
         self._data = data
         return self
 
     def _buildentity(self):
         if self._entity is None:
             raise Exception('Entity must be set')
```

### Comparing `pydynamics-0.0.8/pydynamics.egg-info/PKG-INFO` & `pydynamics-0.0.9/pydynamics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydynamics
-Version: 0.0.8
+Version: 0.0.9
 Summary: Talk to On-Prem Dynamics CRM
 Home-page: https://github.com/dangoscomb/pydynamics
 Author: Dan Goscomb
 Author-email: dan@flowplex.co.uk
 License: UNKNOWN
 Description: # PyDynamics
```

### Comparing `pydynamics-0.0.8/README.md` & `pydynamics-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pydynamics-0.0.8/setup.py` & `pydynamics-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pydynamics",
-    version="0.0.8",
+    version="0.0.9",
     author="Dan Goscomb",
     author_email="dan@flowplex.co.uk",
     description="Talk to On-Prem Dynamics CRM",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dangoscomb/pydynamics",
     packages=setuptools.find_packages(),
```

