# Comparing `tmp/emotion_ai_api-0.1.2.tar.gz` & `tmp/emotion_ai_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emotion_ai_api-0.1.2.tar", last modified: Thu May  9 06:53:05 2024, max compression
+gzip compressed data, was "emotion_ai_api-0.1.3.tar", last modified: Thu May  9 06:56:20 2024, max compression
```

## Comparing `emotion_ai_api-0.1.2.tar` & `emotion_ai_api-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 06:53:05.085202 emotion_ai_api-0.1.2/
--rw-rw-rw-   0        0        0        0 2024-05-09 00:29:10.000000 emotion_ai_api-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      734 2024-05-09 06:53:05.085202 emotion_ai_api-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-09 00:29:21.000000 emotion_ai_api-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 06:53:05.076190 emotion_ai_api-0.1.2/emotion_ai_api/
--rw-rw-rw-   0        0        0        0 2024-05-09 00:28:44.000000 emotion_ai_api-0.1.2/emotion_ai_api/__init__.py
--rw-rw-rw-   0        0        0     3533 2024-05-09 06:44:26.000000 emotion_ai_api-0.1.2/emotion_ai_api/client.py
-drwxrwxrwx   0        0        0        0 2024-05-09 06:53:05.085202 emotion_ai_api-0.1.2/emotion_ai_api.egg-info/
--rw-rw-rw-   0        0        0      734 2024-05-09 06:53:05.000000 emotion_ai_api-0.1.2/emotion_ai_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2024-05-09 06:53:05.000000 emotion_ai_api-0.1.2/emotion_ai_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 06:53:05.000000 emotion_ai_api-0.1.2/emotion_ai_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 06:53:05.000000 emotion_ai_api-0.1.2/emotion_ai_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-09 06:53:05.000000 emotion_ai_api-0.1.2/emotion_ai_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 06:53:05.086704 emotion_ai_api-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1015 2024-05-09 06:53:01.000000 emotion_ai_api-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 06:56:20.225208 emotion_ai_api-0.1.3/
+-rw-rw-rw-   0        0        0        0 2024-05-09 00:29:10.000000 emotion_ai_api-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      734 2024-05-09 06:56:20.224208 emotion_ai_api-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-09 00:29:21.000000 emotion_ai_api-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 06:56:20.215701 emotion_ai_api-0.1.3/emotion_ai_api/
+-rw-rw-rw-   0        0        0        0 2024-05-09 00:28:44.000000 emotion_ai_api-0.1.3/emotion_ai_api/__init__.py
+-rw-rw-rw-   0        0        0     3525 2024-05-09 06:55:51.000000 emotion_ai_api-0.1.3/emotion_ai_api/client.py
+drwxrwxrwx   0        0        0        0 2024-05-09 06:56:20.224208 emotion_ai_api-0.1.3/emotion_ai_api.egg-info/
+-rw-rw-rw-   0        0        0      734 2024-05-09 06:56:20.000000 emotion_ai_api-0.1.3/emotion_ai_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2024-05-09 06:56:20.000000 emotion_ai_api-0.1.3/emotion_ai_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 06:56:20.000000 emotion_ai_api-0.1.3/emotion_ai_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 06:56:20.000000 emotion_ai_api-0.1.3/emotion_ai_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-09 06:56:20.000000 emotion_ai_api-0.1.3/emotion_ai_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 06:56:20.225208 emotion_ai_api-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-09 06:56:17.000000 emotion_ai_api-0.1.3/setup.py
```

### Comparing `emotion_ai_api-0.1.2/PKG-INFO` & `emotion_ai_api-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emotion_ai_api
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python client for interfacing with Emotion AI API services.
 Home-page: https://api.emotion-ai.io
 Author: Wes Lagarde
 Author-email: weslagarde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `emotion_ai_api-0.1.2/emotion_ai_api/client.py` & `emotion_ai_api-0.1.3/emotion_ai_api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         print(f"EmotionAI client initialized with base URL: {self.base_url}, version: {self.version}")
 
     def sentiment_injection(self, messages, session_id):
         """
         Sends messages to the sentiment_context_injection endpoint
         and returns the server's response.
         """
-        endpoint = f"{self.base_url}/{self.version}/sentiment_context_injection"
+        endpoint = f"{self.base_url}/{self.version}/sentiment_injection"
         headers = {"X-Api-Key": self.api_key, "Content-Type": "application/json"}
         payload = {
             "messages": messages,
             "session_id": session_id
         }
 
         print(f"Sending request to {endpoint} with payload:")
```

### Comparing `emotion_ai_api-0.1.2/emotion_ai_api.egg-info/PKG-INFO` & `emotion_ai_api-0.1.3/emotion_ai_api.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emotion_ai_api
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python client for interfacing with Emotion AI API services.
 Home-page: https://api.emotion-ai.io
 Author: Wes Lagarde
 Author-email: weslagarde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `emotion_ai_api-0.1.2/setup.py` & `emotion_ai_api-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='emotion_ai_api',
-    version='0.1.2',
+    version='0.1.3',
     author='Wes Lagarde',
     author_email='weslagarde@gmail.com',
     packages=find_packages(),
     install_requires=[
         'requests',  # Assuming requests is a dependency; add others as needed
     ],
     description='A Python client for interfacing with Emotion AI API services.',
```

