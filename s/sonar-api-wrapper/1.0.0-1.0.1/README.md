# Comparing `tmp/sonar_api_wrapper-1.0.0-py3-none-any.whl.zip` & `tmp/sonar_api_wrapper-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5709 bytes, number of entries: 7
+Zip file size: 5711 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      168 b- defN 20-Feb-02 00:00 sonar_api_wrapper/__init__.py
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 sonar_api_wrapper/__version__.py
--rw-r--r--  2.0 unx     4152 b- defN 20-Feb-02 00:00 sonar_api_wrapper/client.py
-?rw-r--r--  2.0 unx     4608 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.0.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1078 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.0.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      599 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.0.0.dist-info/RECORD
-7 files, 10714 bytes uncompressed, 4637 bytes compressed:  56.7%
+-rw-r--r--  2.0 unx     4136 b- defN 20-Feb-02 00:00 sonar_api_wrapper/client.py
+?rw-r--r--  2.0 unx     4608 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.0.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1078 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.0.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      599 b- defN 20-Feb-02 00:00 sonar_api_wrapper-1.0.1.dist-info/RECORD
+7 files, 10698 bytes uncompressed, 4639 bytes compressed:  56.6%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: sonar_api_wrapper/__version__.py
 Comment: 
 
 Filename: sonar_api_wrapper/client.py
 Comment: 
 
-Filename: sonar_api_wrapper-1.0.0.dist-info/METADATA
+Filename: sonar_api_wrapper-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: sonar_api_wrapper-1.0.0.dist-info/WHEEL
+Filename: sonar_api_wrapper-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: sonar_api_wrapper-1.0.0.dist-info/licenses/LICENSE
+Filename: sonar_api_wrapper-1.0.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: sonar_api_wrapper-1.0.0.dist-info/RECORD
+Filename: sonar_api_wrapper-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sonar_api_wrapper/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.0"
+__version__ = "1.0.1"
```

## sonar_api_wrapper/client.py

```diff
@@ -64,21 +64,21 @@
     :param is_json: if set to True (the default) it will parse the response as a json,
         otherwise it returns the decoded content
     :param username: username used to log (should be the token if accessing via token).
         Default value "admin", can also be set via the environment variable SONAR_USERNAME
     :param password: password used to log (should be empty if accessing via token).
         Default value "admin", can also be set via the environment variable SONAR_PASSWORD
     :param base_path: the base endpoint used to build the api call.
-        Default: "http://localhost:9000/api/" can also be set via the environment variable DEFAULT_SONAR_ENDPOINT
+        Default: "http://localhost:9000/api/" can also be set via the environment variable SONAR_ENDPOINT
     :return: the api response or raise the exception
     """
 
     sonar_username = set_from_env('SONAR_USERNAME', username)
     sonar_password = set_from_env('SONAR_PASSWORD', password)
-    sonar_base_path = set_from_env('DEFAULT_SONAR_ENDPOINT', base_path)
+    sonar_base_path = set_from_env('SONAR_ENDPOINT', base_path)
 
     response = requests.request(
         method=method,
         url=build_endpoint(route, sonar_base_path),
         data=body,
         params=parameters,
         headers=headers,
```

## Comparing `sonar_api_wrapper-1.0.0.dist-info/METADATA` & `sonar_api_wrapper-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sonar-api-wrapper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Sonar API Wrapper - a Sonarqube api wrapper
 Project-URL: Homepage, https://github.com/AlessandroStaffolani/sonar-api-wrapper
 Project-URL: Repository, https://github.com/AlessandroStaffolani/sonar-api-wrapper.git
 Author-email: Alessandro Staffolani <alestam93@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Alessandro Staffolani
```

## Comparing `sonar_api_wrapper-1.0.0.dist-info/licenses/LICENSE` & `sonar_api_wrapper-1.0.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

