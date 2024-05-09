# Comparing `tmp/emotion_ai_api-0.1.4.tar.gz` & `tmp/emotion_ai_api-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emotion_ai_api-0.1.4.tar", last modified: Thu May  9 06:58:07 2024, max compression
+gzip compressed data, was "emotion_ai_api-0.1.5.tar", last modified: Thu May  9 07:09:35 2024, max compression
```

## Comparing `emotion_ai_api-0.1.4.tar` & `emotion_ai_api-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 06:58:07.969032 emotion_ai_api-0.1.4/
--rw-rw-rw-   0        0        0        0 2024-05-09 00:29:10.000000 emotion_ai_api-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      734 2024-05-09 06:58:07.969032 emotion_ai_api-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-09 00:29:21.000000 emotion_ai_api-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 06:58:07.957010 emotion_ai_api-0.1.4/emotion_ai_api/
--rw-rw-rw-   0        0        0        0 2024-05-09 00:28:44.000000 emotion_ai_api-0.1.4/emotion_ai_api/__init__.py
--rw-rw-rw-   0        0        0     3538 2024-05-09 06:57:58.000000 emotion_ai_api-0.1.4/emotion_ai_api/client.py
-drwxrwxrwx   0        0        0        0 2024-05-09 06:58:07.968032 emotion_ai_api-0.1.4/emotion_ai_api.egg-info/
--rw-rw-rw-   0        0        0      734 2024-05-09 06:58:07.000000 emotion_ai_api-0.1.4/emotion_ai_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2024-05-09 06:58:07.000000 emotion_ai_api-0.1.4/emotion_ai_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 06:58:07.000000 emotion_ai_api-0.1.4/emotion_ai_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 06:58:07.000000 emotion_ai_api-0.1.4/emotion_ai_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-09 06:58:07.000000 emotion_ai_api-0.1.4/emotion_ai_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 06:58:07.969032 emotion_ai_api-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1015 2024-05-09 06:57:54.000000 emotion_ai_api-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:09:35.310910 emotion_ai_api-0.1.5/
+-rw-rw-rw-   0        0        0        0 2024-05-09 00:29:10.000000 emotion_ai_api-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      734 2024-05-09 07:09:35.310910 emotion_ai_api-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-09 00:29:21.000000 emotion_ai_api-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 07:09:35.302894 emotion_ai_api-0.1.5/emotion_ai_api/
+-rw-rw-rw-   0        0        0        0 2024-05-09 00:28:44.000000 emotion_ai_api-0.1.5/emotion_ai_api/__init__.py
+-rw-rw-rw-   0        0        0     3542 2024-05-09 07:05:45.000000 emotion_ai_api-0.1.5/emotion_ai_api/client.py
+drwxrwxrwx   0        0        0        0 2024-05-09 07:09:35.309906 emotion_ai_api-0.1.5/emotion_ai_api.egg-info/
+-rw-rw-rw-   0        0        0      734 2024-05-09 07:09:35.000000 emotion_ai_api-0.1.5/emotion_ai_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2024-05-09 07:09:35.000000 emotion_ai_api-0.1.5/emotion_ai_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 07:09:35.000000 emotion_ai_api-0.1.5/emotion_ai_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 07:09:35.000000 emotion_ai_api-0.1.5/emotion_ai_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-09 07:09:35.000000 emotion_ai_api-0.1.5/emotion_ai_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 07:09:35.311911 emotion_ai_api-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-09 07:09:23.000000 emotion_ai_api-0.1.5/setup.py
```

### Comparing `emotion_ai_api-0.1.4/PKG-INFO` & `emotion_ai_api-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emotion_ai_api
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python client for interfacing with Emotion AI API services.
 Home-page: https://api.emotion-ai.io
 Author: Wes Lagarde
 Author-email: weslagarde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `emotion_ai_api-0.1.4/emotion_ai_api/client.py` & `emotion_ai_api-0.1.5/emotion_ai_api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         print(f"EmotionAI client initialized with base URL: {self.base_url}, version: {self.version}")
 
     def sentiment_injection(self, messages, session_id=None):
         """
         Sends messages to the sentiment_context_injection endpoint
         and returns the server's response.
         """
-        endpoint = f"{self.base_url}/{self.version}/sentiment_injection"
+        endpoint = f"{self.base_url}/{self.version}/api/sentiment_injection"
         headers = {"X-Api-Key": self.api_key, "Content-Type": "application/json"}
         payload = {
             "messages": messages,
             "session_id": session_id or None
         }
 
         print(f"Sending request to {endpoint} with payload:")
```

### Comparing `emotion_ai_api-0.1.4/emotion_ai_api.egg-info/PKG-INFO` & `emotion_ai_api-0.1.5/emotion_ai_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emotion_ai_api
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python client for interfacing with Emotion AI API services.
 Home-page: https://api.emotion-ai.io
 Author: Wes Lagarde
 Author-email: weslagarde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `emotion_ai_api-0.1.4/setup.py` & `emotion_ai_api-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='emotion_ai_api',
-    version='0.1.4',
+    version='0.1.5',
     author='Wes Lagarde',
     author_email='weslagarde@gmail.com',
     packages=find_packages(),
     install_requires=[
         'requests',  # Assuming requests is a dependency; add others as needed
     ],
     description='A Python client for interfacing with Emotion AI API services.',
```

