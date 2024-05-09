# Comparing `tmp/unified-json-api-0.0.8.tar.gz` & `tmp/unified-json-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unified-json-api-0.0.8.tar", last modified: Wed Sep 27 14:36:43 2023, max compression
+gzip compressed data, was "unified-json-api-0.0.9.tar", last modified: Wed Oct 25 11:51:27 2023, max compression
```

## Comparing `unified-json-api-0.0.8.tar` & `unified-json-api-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 14:36:43.224424 unified-json-api-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2023-09-27 14:36:43.224424 unified-json-api-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-09-27 14:36:03.000000 unified-json-api-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-09-27 14:36:03.000000 unified-json-api-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-27 14:36:43.224424 unified-json-api-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-09-27 14:36:03.000000 unified-json-api-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 14:36:43.220424 unified-json-api-0.0.8/unified_json_api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 14:36:43.220424 unified-json-api-0.0.8/unified_json_api/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-27 14:36:03.000000 unified-json-api-0.0.8/unified_json_api/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-09-27 14:36:03.000000 unified-json-api-0.0.8/unified_json_api/src/constants_unified_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2023-09-27 14:36:03.000000 unified-json-api-0.0.8/unified_json_api/src/unified_json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 14:36:43.220424 unified-json-api-0.0.8/unified_json_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2023-09-27 14:36:43.000000 unified-json-api-0.0.8/unified_json_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-09-27 14:36:43.000000 unified-json-api-0.0.8/unified_json_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-27 14:36:43.000000 unified-json-api-0.0.8/unified_json_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-09-27 14:36:43.000000 unified-json-api-0.0.8/unified_json_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-27 14:36:43.000000 unified-json-api-0.0.8/unified_json_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 11:51:27.461247 unified-json-api-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2023-10-25 11:51:27.461247 unified-json-api-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-10-25 11:50:49.000000 unified-json-api-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-10-25 11:50:49.000000 unified-json-api-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-25 11:51:27.461247 unified-json-api-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-10-25 11:50:49.000000 unified-json-api-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 11:51:27.457247 unified-json-api-0.0.9/unified_json_api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 11:51:27.461247 unified-json-api-0.0.9/unified_json_api/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 11:50:49.000000 unified-json-api-0.0.9/unified_json_api/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2023-10-25 11:50:49.000000 unified-json-api-0.0.9/unified_json_api/src/constants_unified_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2023-10-25 11:50:49.000000 unified-json-api-0.0.9/unified_json_api/src/unified_json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 11:51:27.457247 unified-json-api-0.0.9/unified_json_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2023-10-25 11:51:27.000000 unified-json-api-0.0.9/unified_json_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2023-10-25 11:51:27.000000 unified-json-api-0.0.9/unified_json_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 11:51:27.000000 unified-json-api-0.0.9/unified_json_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-10-25 11:51:27.000000 unified-json-api-0.0.9/unified_json_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-25 11:51:27.000000 unified-json-api-0.0.9/unified_json_api.egg-info/top_level.txt
```

### Comparing `unified-json-api-0.0.8/PKG-INFO` & `unified-json-api-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unified-json-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles unified-json-api Python
 Home-page: https://github.com/circles-zone/unified-json-api-python-pacakge
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `unified-json-api-0.0.8/README.md` & `unified-json-api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `unified-json-api-0.0.8/pyproject.toml` & `unified-json-api-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `unified-json-api-0.0.8/setup.py` & `unified-json-api-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 with open('README.md') as f:
     readme = f.read()
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # https://pypi.org/project/unified-json-api/
+    version='0.0.9',  # https://pypi.org/project/unified-json-api/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles unified-json-api Python",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/unified-json-api-python-pacakge",
     # packages=setuptools.find_packages(),
```

### Comparing `unified-json-api-0.0.8/unified_json_api/src/constants_unified_json.py` & `unified-json-api-0.0.9/unified_json_api/src/constants_unified_json.py`

 * *Files identical despite different names*

### Comparing `unified-json-api-0.0.8/unified_json_api/src/unified_json.py` & `unified-json-api-0.0.9/unified_json_api/src/unified_json.py`

 * *Files 22% similar despite different names*

```diff
@@ -122,7 +122,39 @@
         body = {}
         body["text_prompts"] = self.unified_json.get("body", {}).get("inputText", [])
         body["cfg_scale"] = self.unified_json.get("body", {}).get("textGenerationConfig", {}).get("cfg_scale", 50)
         body["seed"] = self.unified_json.get("body", {}).get("textGenerationConfig", {}).get("seed", 0)
         body["steps"] = self.unified_json.get("body", {}).get("textGenerationConfig", {}).get("steps", 1)
         bedrock_stability_ai_json["body"] = json.dumps(body)
         return bedrock_stability_ai_json
+    
+    def get_deepface_ai_json(self) -> Dict[str, any]:
+        # the deepface structure should be:
+        #  request = {
+        #               headers: 
+        #                       {
+        #                         contentType: 'application/json'
+        #                       }, 
+        #               body:{ 
+        #                       jwtToken: [TOKEN],
+        #                       storage_id: [STORAGE_ID] 
+        #                    }
+        #            }
+        # so if I understand the structure correctly the jwtToken structure is fine
+        
+
+        deepface_ai_json = {}
+        deepface_ai_json['headers'] = {}
+        deepface_ai_json['body'] = {}
+        deepface_ai_json['headers']['Content-Type'] = self.unified_json['contentType']
+
+        try:
+            deepface_ai_json['body']['jwtToken'] = self.unified_json['body']['jwtToken']
+        except KeyError:
+            raise KeyError("jwtToken is missing from the unified json body")
+        
+        try:
+            deepface_ai_json['body']['storage_id'] = self.unified_json['body']['storage_id']
+        except KeyError:
+            raise KeyError("storage_id is missing from the unified json body")
+        
+        return deepface_ai_json
```

### Comparing `unified-json-api-0.0.8/unified_json_api.egg-info/PKG-INFO` & `unified-json-api-0.0.9/unified_json_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unified-json-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles unified-json-api Python
 Home-page: https://github.com/circles-zone/unified-json-api-python-pacakge
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

