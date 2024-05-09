# Comparing `tmp/emotion_ai_api-0.1.3.tar.gz` & `tmp/emotion_ai_api-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emotion_ai_api-0.1.3.tar", last modified: Thu May  9 06:56:20 2024, max compression
+gzip compressed data, was "emotion_ai_api-0.1.4.tar", last modified: Thu May  9 06:58:07 2024, max compression
```

## Comparing `emotion_ai_api-0.1.3.tar` & `emotion_ai_api-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 06:56:20.225208 emotion_ai_api-0.1.3/
--rw-rw-rw-   0        0        0        0 2024-05-09 00:29:10.000000 emotion_ai_api-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      734 2024-05-09 06:56:20.224208 emotion_ai_api-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-09 00:29:21.000000 emotion_ai_api-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 06:56:20.215701 emotion_ai_api-0.1.3/emotion_ai_api/
--rw-rw-rw-   0        0        0        0 2024-05-09 00:28:44.000000 emotion_ai_api-0.1.3/emotion_ai_api/__init__.py
--rw-rw-rw-   0        0        0     3525 2024-05-09 06:55:51.000000 emotion_ai_api-0.1.3/emotion_ai_api/client.py
-drwxrwxrwx   0        0        0        0 2024-05-09 06:56:20.224208 emotion_ai_api-0.1.3/emotion_ai_api.egg-info/
--rw-rw-rw-   0        0        0      734 2024-05-09 06:56:20.000000 emotion_ai_api-0.1.3/emotion_ai_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2024-05-09 06:56:20.000000 emotion_ai_api-0.1.3/emotion_ai_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 06:56:20.000000 emotion_ai_api-0.1.3/emotion_ai_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 06:56:20.000000 emotion_ai_api-0.1.3/emotion_ai_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-09 06:56:20.000000 emotion_ai_api-0.1.3/emotion_ai_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 06:56:20.225208 emotion_ai_api-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1015 2024-05-09 06:56:17.000000 emotion_ai_api-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 06:58:07.969032 emotion_ai_api-0.1.4/
+-rw-rw-rw-   0        0        0        0 2024-05-09 00:29:10.000000 emotion_ai_api-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      734 2024-05-09 06:58:07.969032 emotion_ai_api-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-09 00:29:21.000000 emotion_ai_api-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 06:58:07.957010 emotion_ai_api-0.1.4/emotion_ai_api/
+-rw-rw-rw-   0        0        0        0 2024-05-09 00:28:44.000000 emotion_ai_api-0.1.4/emotion_ai_api/__init__.py
+-rw-rw-rw-   0        0        0     3538 2024-05-09 06:57:58.000000 emotion_ai_api-0.1.4/emotion_ai_api/client.py
+drwxrwxrwx   0        0        0        0 2024-05-09 06:58:07.968032 emotion_ai_api-0.1.4/emotion_ai_api.egg-info/
+-rw-rw-rw-   0        0        0      734 2024-05-09 06:58:07.000000 emotion_ai_api-0.1.4/emotion_ai_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2024-05-09 06:58:07.000000 emotion_ai_api-0.1.4/emotion_ai_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 06:58:07.000000 emotion_ai_api-0.1.4/emotion_ai_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 06:58:07.000000 emotion_ai_api-0.1.4/emotion_ai_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-09 06:58:07.000000 emotion_ai_api-0.1.4/emotion_ai_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 06:58:07.969032 emotion_ai_api-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-09 06:57:54.000000 emotion_ai_api-0.1.4/setup.py
```

### Comparing `emotion_ai_api-0.1.3/PKG-INFO` & `emotion_ai_api-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emotion_ai_api
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python client for interfacing with Emotion AI API services.
 Home-page: https://api.emotion-ai.io
 Author: Wes Lagarde
 Author-email: weslagarde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `emotion_ai_api-0.1.3/emotion_ai_api/client.py` & `emotion_ai_api-0.1.4/emotion_ai_api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 class EmotionAI:
     def __init__(self, base_url, api_key, version="v1"):
         self.base_url = base_url.rstrip("/")
         self.api_key = api_key
         self.version = version
         print(f"EmotionAI client initialized with base URL: {self.base_url}, version: {self.version}")
 
-    def sentiment_injection(self, messages, session_id):
+    def sentiment_injection(self, messages, session_id=None):
         """
         Sends messages to the sentiment_context_injection endpoint
         and returns the server's response.
         """
         endpoint = f"{self.base_url}/{self.version}/sentiment_injection"
         headers = {"X-Api-Key": self.api_key, "Content-Type": "application/json"}
         payload = {
             "messages": messages,
-            "session_id": session_id
+            "session_id": session_id or None
         }
 
         print(f"Sending request to {endpoint} with payload:")
         print(json.dumps(payload, indent=2))
         try:
             response = requests.post(endpoint, json=payload, headers=headers)
             response.raise_for_status()
```

### Comparing `emotion_ai_api-0.1.3/emotion_ai_api.egg-info/PKG-INFO` & `emotion_ai_api-0.1.4/emotion_ai_api.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emotion_ai_api
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python client for interfacing with Emotion AI API services.
 Home-page: https://api.emotion-ai.io
 Author: Wes Lagarde
 Author-email: weslagarde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `emotion_ai_api-0.1.3/setup.py` & `emotion_ai_api-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='emotion_ai_api',
-    version='0.1.3',
+    version='0.1.4',
     author='Wes Lagarde',
     author_email='weslagarde@gmail.com',
     packages=find_packages(),
     install_requires=[
         'requests',  # Assuming requests is a dependency; add others as needed
     ],
     description='A Python client for interfacing with Emotion AI API services.',
```

