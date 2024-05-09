# Comparing `tmp/aiZero-0.0.1a3.tar.gz` & `tmp/aiZero-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiZero-0.0.1a3.tar", last modified: Wed May  8 02:24:21 2024, max compression
+gzip compressed data, was "aiZero-0.0.1a4.tar", last modified: Thu May  9 02:39:58 2024, max compression
```

## Comparing `aiZero-0.0.1a3.tar` & `aiZero-0.0.1a4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:24:21.080692 aiZero-0.0.1a3/
--rw-r--r--   0 emhang     (501) staff       (20)       71 2024-05-07 05:21:12.000000 aiZero-0.0.1a3/MANIFEST.in
--rw-r--r--   0 emhang     (501) staff       (20)     9594 2024-05-08 02:24:21.080558 aiZero-0.0.1a3/PKG-INFO
--rw-r--r--   0 emhang     (501) staff       (20)     9047 2024-05-07 07:27:48.000000 aiZero-0.0.1a3/README.md
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:24:21.076437 aiZero-0.0.1a3/aiZero/
--rw-r--r--   0 emhang     (501) staff       (20)    18610 2024-05-08 02:22:35.000000 aiZero-0.0.1a3/aiZero/__init__.py
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:24:21.075821 aiZero-0.0.1a3/aiZero/static/
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:24:21.077724 aiZero-0.0.1a3/aiZero/static/audios/
--rw-r--r--   0 emhang     (501) staff       (20)   276040 2024-05-07 07:22:42.000000 aiZero-0.0.1a3/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:24:21.079334 aiZero-0.0.1a3/aiZero/static/js/
--rw-r--r--   0 emhang     (501) staff       (20)    35418 2024-04-10 09:16:03.000000 aiZero-0.0.1a3/aiZero/static/js/marked.min.js
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:24:21.080054 aiZero-0.0.1a3/aiZero/templates/
--rw-r--r--   0 emhang     (501) staff       (20)    28097 2024-04-17 06:07:29.000000 aiZero-0.0.1a3/aiZero/templates/index.html
-drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-08 02:24:21.077601 aiZero-0.0.1a3/aiZero.egg-info/
--rw-r--r--   0 emhang     (501) staff       (20)     9594 2024-05-08 02:24:21.000000 aiZero-0.0.1a3/aiZero.egg-info/PKG-INFO
--rw-r--r--   0 emhang     (501) staff       (20)      319 2024-05-08 02:24:21.000000 aiZero-0.0.1a3/aiZero.egg-info/SOURCES.txt
--rw-r--r--   0 emhang     (501) staff       (20)        1 2024-05-08 02:24:21.000000 aiZero-0.0.1a3/aiZero.egg-info/dependency_links.txt
--rw-r--r--   0 emhang     (501) staff       (20)       40 2024-05-08 02:24:21.000000 aiZero-0.0.1a3/aiZero.egg-info/requires.txt
--rw-r--r--   0 emhang     (501) staff       (20)        7 2024-05-08 02:24:21.000000 aiZero-0.0.1a3/aiZero.egg-info/top_level.txt
--rw-r--r--   0 emhang     (501) staff       (20)       38 2024-05-08 02:24:21.080736 aiZero-0.0.1a3/setup.cfg
--rw-r--r--   0 emhang     (501) staff       (20)      820 2024-05-08 02:22:53.000000 aiZero-0.0.1a3/setup.py
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.439221 aiZero-0.0.1a4/
+-rw-r--r--   0 emhang     (501) staff       (20)       71 2024-05-07 05:21:12.000000 aiZero-0.0.1a4/MANIFEST.in
+-rw-r--r--   0 emhang     (501) staff       (20)     9606 2024-05-09 02:39:58.439050 aiZero-0.0.1a4/PKG-INFO
+-rw-r--r--   0 emhang     (501) staff       (20)     9059 2024-05-09 02:38:31.000000 aiZero-0.0.1a4/README.md
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.435054 aiZero-0.0.1a4/aiZero/
+-rw-r--r--   0 emhang     (501) staff       (20)    18610 2024-05-08 02:22:35.000000 aiZero-0.0.1a4/aiZero/__init__.py
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.433799 aiZero-0.0.1a4/aiZero/static/
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.436658 aiZero-0.0.1a4/aiZero/static/audios/
+-rw-r--r--   0 emhang     (501) staff       (20)   276040 2024-05-07 07:22:42.000000 aiZero-0.0.1a4/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.438169 aiZero-0.0.1a4/aiZero/static/js/
+-rw-r--r--   0 emhang     (501) staff       (20)    35418 2024-04-10 09:16:03.000000 aiZero-0.0.1a4/aiZero/static/js/marked.min.js
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.438604 aiZero-0.0.1a4/aiZero/templates/
+-rw-r--r--   0 emhang     (501) staff       (20)    28097 2024-04-17 06:07:29.000000 aiZero-0.0.1a4/aiZero/templates/index.html
+drwxr-xr-x   0 emhang     (501) staff       (20)        0 2024-05-09 02:39:58.436437 aiZero-0.0.1a4/aiZero.egg-info/
+-rw-r--r--   0 emhang     (501) staff       (20)     9606 2024-05-09 02:39:58.000000 aiZero-0.0.1a4/aiZero.egg-info/PKG-INFO
+-rw-r--r--   0 emhang     (501) staff       (20)      319 2024-05-09 02:39:58.000000 aiZero-0.0.1a4/aiZero.egg-info/SOURCES.txt
+-rw-r--r--   0 emhang     (501) staff       (20)        1 2024-05-09 02:39:58.000000 aiZero-0.0.1a4/aiZero.egg-info/dependency_links.txt
+-rw-r--r--   0 emhang     (501) staff       (20)       40 2024-05-09 02:39:58.000000 aiZero-0.0.1a4/aiZero.egg-info/requires.txt
+-rw-r--r--   0 emhang     (501) staff       (20)        7 2024-05-09 02:39:58.000000 aiZero-0.0.1a4/aiZero.egg-info/top_level.txt
+-rw-r--r--   0 emhang     (501) staff       (20)       38 2024-05-09 02:39:58.439271 aiZero-0.0.1a4/setup.cfg
+-rw-r--r--   0 emhang     (501) staff       (20)      820 2024-05-09 02:39:01.000000 aiZero-0.0.1a4/setup.py
```

### Comparing `aiZero-0.0.1a3/PKG-INFO` & `aiZero-0.0.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiZero
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A simple and easy-to-use library that connects to common artificial intelligence interfaces, allowing for quick development of local web applications. It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.
 Home-page: UNKNOWN
 Author: emhang
 Author-email: emhang@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -296,15 +296,15 @@
 ```python
 from aiZero import AIWebApp, text_generation, speech_recognition, speech_synthesis
 
 def my_ai_function():
     audio = app.input_audio
     text = speech_recognition(audio)
     chat_history.append(text)
-    reply = text_generation([text])
+    reply = text_generation(chat_history)
     chat_history.append(reply)
     reply_audio = speech_synthesis(reply)
     app.results.append({'audio': reply_audio})
 
 chat_history = []
 app = AIWebApp(title='人工智能助手')
 app.set_apikey('YOUR_API_KEY')
@@ -319,15 +319,15 @@
 
 ```python
 from aiZero import AIWebApp, text_generation, speech_synthesis
 
 def my_ai_function():
     text = app.input_text
     chat_history.append(text)
-    reply = text_generation([text])
+    reply = text_generation(chat_history)
     chat_history.append(reply)
     reply_audio = speech_synthesis(reply)
     app.results.append({'text': reply, 'audio': reply_audio})
 
 chat_history = []
 app = AIWebApp(title='人工智能助手')
 app.set_apikey('YOUR_API_KEY')
```

### Comparing `aiZero-0.0.1a3/README.md` & `aiZero-0.0.1a4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,15 @@
 ```python
 from aiZero import AIWebApp, text_generation, speech_recognition, speech_synthesis
 
 def my_ai_function():
     audio = app.input_audio
     text = speech_recognition(audio)
     chat_history.append(text)
-    reply = text_generation([text])
+    reply = text_generation(chat_history)
     chat_history.append(reply)
     reply_audio = speech_synthesis(reply)
     app.results.append({'audio': reply_audio})
 
 chat_history = []
 app = AIWebApp(title='人工智能助手')
 app.set_apikey('YOUR_API_KEY')
@@ -307,15 +307,15 @@
 
 ```python
 from aiZero import AIWebApp, text_generation, speech_synthesis
 
 def my_ai_function():
     text = app.input_text
     chat_history.append(text)
-    reply = text_generation([text])
+    reply = text_generation(chat_history)
     chat_history.append(reply)
     reply_audio = speech_synthesis(reply)
     app.results.append({'text': reply, 'audio': reply_audio})
 
 chat_history = []
 app = AIWebApp(title='人工智能助手')
 app.set_apikey('YOUR_API_KEY')
```

### Comparing `aiZero-0.0.1a3/aiZero/__init__.py` & `aiZero-0.0.1a4/aiZero/__init__.py`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a3/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav` & `aiZero-0.0.1a4/aiZero/static/audios/1a32d899-90f3-46e7-a26c-7a744b1516a7.wav`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a3/aiZero/static/js/marked.min.js` & `aiZero-0.0.1a4/aiZero/static/js/marked.min.js`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a3/aiZero/templates/index.html` & `aiZero-0.0.1a4/aiZero/templates/index.html`

 * *Files identical despite different names*

### Comparing `aiZero-0.0.1a3/aiZero.egg-info/PKG-INFO` & `aiZero-0.0.1a4/aiZero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiZero
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A simple and easy-to-use library that connects to common artificial intelligence interfaces, allowing for quick development of local web applications. It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.
 Home-page: UNKNOWN
 Author: emhang
 Author-email: emhang@126.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -296,15 +296,15 @@
 ```python
 from aiZero import AIWebApp, text_generation, speech_recognition, speech_synthesis
 
 def my_ai_function():
     audio = app.input_audio
     text = speech_recognition(audio)
     chat_history.append(text)
-    reply = text_generation([text])
+    reply = text_generation(chat_history)
     chat_history.append(reply)
     reply_audio = speech_synthesis(reply)
     app.results.append({'audio': reply_audio})
 
 chat_history = []
 app = AIWebApp(title='人工智能助手')
 app.set_apikey('YOUR_API_KEY')
@@ -319,15 +319,15 @@
 
 ```python
 from aiZero import AIWebApp, text_generation, speech_synthesis
 
 def my_ai_function():
     text = app.input_text
     chat_history.append(text)
-    reply = text_generation([text])
+    reply = text_generation(chat_history)
     chat_history.append(reply)
     reply_audio = speech_synthesis(reply)
     app.results.append({'text': reply, 'audio': reply_audio})
 
 chat_history = []
 app = AIWebApp(title='人工智能助手')
 app.set_apikey('YOUR_API_KEY')
```

### Comparing `aiZero-0.0.1a3/setup.py` & `aiZero-0.0.1a4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aiZero",
-    version="0.0.1a3",
+    version="0.0.1a4",
     author="emhang",
     author_email="emhang@126.com",
     description="A simple and easy-to-use library that connects to common artificial intelligence interfaces, "
                 "allowing for quick development of local web applications. "
                 "It includes mainstream AI capabilities such as LLM text interaction, image understanding, audio understanding, image generation, speech recognition, and speech synthesis.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

