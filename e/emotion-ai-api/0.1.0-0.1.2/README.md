# Comparing `tmp/emotion_ai_api-0.1.0.tar.gz` & `tmp/emotion_ai_api-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emotion_ai_api-0.1.0.tar", last modified: Thu May  9 04:09:28 2024, max compression
+gzip compressed data, was "emotion_ai_api-0.1.2.tar", last modified: Thu May  9 06:53:05 2024, max compression
```

## Comparing `emotion_ai_api-0.1.0.tar` & `emotion_ai_api-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 04:09:28.373961 emotion_ai_api-0.1.0/
--rw-rw-rw-   0        0        0        0 2024-05-09 00:29:10.000000 emotion_ai_api-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      739 2024-05-09 04:09:28.373961 emotion_ai_api-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-09 00:29:21.000000 emotion_ai_api-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 04:09:28.363454 emotion_ai_api-0.1.0/emotion_ai_api/
--rw-rw-rw-   0        0        0        0 2024-05-09 00:28:44.000000 emotion_ai_api-0.1.0/emotion_ai_api/__init__.py
--rw-rw-rw-   0        0        0     3541 2024-05-09 03:51:17.000000 emotion_ai_api-0.1.0/emotion_ai_api/client.py
-drwxrwxrwx   0        0        0        0 2024-05-09 04:09:28.371960 emotion_ai_api-0.1.0/emotion_ai_api.egg-info/
--rw-rw-rw-   0        0        0      739 2024-05-09 04:09:28.000000 emotion_ai_api-0.1.0/emotion_ai_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2024-05-09 04:09:28.000000 emotion_ai_api-0.1.0/emotion_ai_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 04:09:28.000000 emotion_ai_api-0.1.0/emotion_ai_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 04:09:28.000000 emotion_ai_api-0.1.0/emotion_ai_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-09 04:09:28.000000 emotion_ai_api-0.1.0/emotion_ai_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 04:09:28.373961 emotion_ai_api-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1020 2024-05-09 04:07:39.000000 emotion_ai_api-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 06:53:05.085202 emotion_ai_api-0.1.2/
+-rw-rw-rw-   0        0        0        0 2024-05-09 00:29:10.000000 emotion_ai_api-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      734 2024-05-09 06:53:05.085202 emotion_ai_api-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-09 00:29:21.000000 emotion_ai_api-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 06:53:05.076190 emotion_ai_api-0.1.2/emotion_ai_api/
+-rw-rw-rw-   0        0        0        0 2024-05-09 00:28:44.000000 emotion_ai_api-0.1.2/emotion_ai_api/__init__.py
+-rw-rw-rw-   0        0        0     3533 2024-05-09 06:44:26.000000 emotion_ai_api-0.1.2/emotion_ai_api/client.py
+drwxrwxrwx   0        0        0        0 2024-05-09 06:53:05.085202 emotion_ai_api-0.1.2/emotion_ai_api.egg-info/
+-rw-rw-rw-   0        0        0      734 2024-05-09 06:53:05.000000 emotion_ai_api-0.1.2/emotion_ai_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2024-05-09 06:53:05.000000 emotion_ai_api-0.1.2/emotion_ai_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 06:53:05.000000 emotion_ai_api-0.1.2/emotion_ai_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 06:53:05.000000 emotion_ai_api-0.1.2/emotion_ai_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-09 06:53:05.000000 emotion_ai_api-0.1.2/emotion_ai_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 06:53:05.086704 emotion_ai_api-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-09 06:53:01.000000 emotion_ai_api-0.1.2/setup.py
```

### Comparing `emotion_ai_api-0.1.0/PKG-INFO` & `emotion_ai_api-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: emotion_ai_api
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Python client for interfacing with Emotion AI API services.
-Home-page: https://platform.emotion-ai.io
+Home-page: https://api.emotion-ai.io
 Author: Wes Lagarde
 Author-email: weslagarde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
```

### Comparing `emotion_ai_api-0.1.0/emotion_ai_api/client.py` & `emotion_ai_api-0.1.2/emotion_ai_api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 class EmotionAI:
     def __init__(self, base_url, api_key, version="v1"):
         self.base_url = base_url.rstrip("/")
         self.api_key = api_key
         self.version = version
         print(f"EmotionAI client initialized with base URL: {self.base_url}, version: {self.version}")
 
-    def sentiment_context_injection(self, messages, session_id):
+    def sentiment_injection(self, messages, session_id):
         """
         Sends messages to the sentiment_context_injection endpoint
         and returns the server's response.
         """
         endpoint = f"{self.base_url}/{self.version}/sentiment_context_injection"
         headers = {"X-Api-Key": self.api_key, "Content-Type": "application/json"}
         payload = {
```

### Comparing `emotion_ai_api-0.1.0/emotion_ai_api.egg-info/PKG-INFO` & `emotion_ai_api-0.1.2/emotion_ai_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: emotion_ai_api
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Python client for interfacing with Emotion AI API services.
-Home-page: https://platform.emotion-ai.io
+Home-page: https://api.emotion-ai.io
 Author: Wes Lagarde
 Author-email: weslagarde@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
```

### Comparing `emotion_ai_api-0.1.0/setup.py` & `emotion_ai_api-0.1.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name='emotion_ai_api',
-    version='0.1.0',
+    version='0.1.2',
     author='Wes Lagarde',
     author_email='weslagarde@gmail.com',
     packages=find_packages(),
     install_requires=[
         'requests',  # Assuming requests is a dependency; add others as needed
     ],
     description='A Python client for interfacing with Emotion AI API services.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://platform.emotion-ai.io',  # Optional: your project's repo
+    url='https://api.emotion-ai.io',  # Optional: your project's repo
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.11',
+    python_requires='>=3.10',
 )
```

