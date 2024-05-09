# Comparing `tmp/pvorcademo-0.2.0.tar.gz` & `tmp/pvorcademo-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvorcademo-0.2.0.tar", last modified: Fri May  3 22:32:58 2024, max compression
+gzip compressed data, was "pvorcademo-0.2.1.tar", last modified: Thu May  9 21:51:58 2024, max compression
```

## Comparing `pvorcademo-0.2.0.tar` & `pvorcademo-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-03 22:32:58.576616 pvorcademo-0.2.0/
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      101 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/MANIFEST.in
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     3069 2024-05-03 22:32:58.576616 pvorcademo-0.2.0/PKG-INFO
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     2377 2024-05-03 22:08:49.000000 pvorcademo-0.2.0/README.md
-drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-03 22:32:58.576616 pvorcademo-0.2.0/pvorcademo/
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)    11344 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo/LICENSE
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     2822 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo/orca_demo.py
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)    13421 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo/orca_demo_streaming.py
-drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-03 22:32:58.576616 pvorcademo-0.2.0/pvorcademo.egg-info/
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     3069 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo.egg-info/PKG-INFO
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      313 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo.egg-info/SOURCES.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)        1 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo.egg-info/dependency_links.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      115 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo.egg-info/entry_points.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       63 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo.egg-info/requires.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       11 2024-05-03 22:32:58.000000 pvorcademo-0.2.0/pvorcademo.egg-info/top_level.txt
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       38 2024-05-03 22:32:58.576616 pvorcademo-0.2.0/setup.cfg
--rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     1794 2024-05-03 22:26:21.000000 pvorcademo-0.2.0/setup.py
+drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-09 21:51:58.862597 pvorcademo-0.2.1/
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      101 2024-05-09 21:51:58.000000 pvorcademo-0.2.1/MANIFEST.in
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     3069 2024-05-09 21:51:58.858596 pvorcademo-0.2.1/PKG-INFO
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     2377 2024-05-08 21:13:07.000000 pvorcademo-0.2.1/README.md
+drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-09 21:51:58.858596 pvorcademo-0.2.1/pvorcademo/
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)    11344 2024-05-09 21:51:58.000000 pvorcademo-0.2.1/pvorcademo/LICENSE
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     2822 2024-05-09 21:51:58.000000 pvorcademo-0.2.1/pvorcademo/orca_demo.py
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)    13421 2024-05-09 21:51:58.000000 pvorcademo-0.2.1/pvorcademo/orca_demo_streaming.py
+drwxrwxr-x   0 srinivasa  (1000) srinivasa  (1000)        0 2024-05-09 21:51:58.858596 pvorcademo-0.2.1/pvorcademo.egg-info/
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     3069 2024-05-09 21:51:58.000000 pvorcademo-0.2.1/pvorcademo.egg-info/PKG-INFO
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      313 2024-05-09 21:51:58.000000 pvorcademo-0.2.1/pvorcademo.egg-info/SOURCES.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)        1 2024-05-09 21:51:58.000000 pvorcademo-0.2.1/pvorcademo.egg-info/dependency_links.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)      115 2024-05-09 21:51:58.000000 pvorcademo-0.2.1/pvorcademo.egg-info/entry_points.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       63 2024-05-09 21:51:58.000000 pvorcademo-0.2.1/pvorcademo.egg-info/requires.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       11 2024-05-09 21:51:58.000000 pvorcademo-0.2.1/pvorcademo.egg-info/top_level.txt
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)       38 2024-05-09 21:51:58.862597 pvorcademo-0.2.1/setup.cfg
+-rw-rw-r--   0 srinivasa  (1000) srinivasa  (1000)     1794 2024-05-09 21:48:48.000000 pvorcademo-0.2.1/setup.py
```

### Comparing `pvorcademo-0.2.0/PKG-INFO` & `pvorcademo-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvorcademo
-Version: 0.2.0
+Version: 0.2.1
 Summary: Orca Streaming Text-to-Speech Engine demos
 Home-page: https://github.com/Picovoice/orca
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
 Keywords: Streaming Text-to-Speech,TTS,Speech Synthesis,Voice Generation,Speech Engine
 Platform: UNKNOWN
@@ -63,15 +63,15 @@
 
 In this demo, we simulate a response from a language model by creating a text stream from a user-defined text.
 We stream that text to Orca and play the synthesized audio as soon as it gets generated.
 
 To run it, execute the following:
 
 ```console
-orca_demo_streaming --access_key ${ACCESS_KEY} --text-to-stream ${TEXT}
+orca_demo_streaming --access_key ${ACCESS_KEY} --text_to_stream ${TEXT}
 ```
 
 Replace `${ACCESS_KEY}` with your `AccessKey` obtained from Picovoice Console and `${TEXT}` with your text to be
 streamed to Orca. Please note that this demo was not tested on macOS.
 
 ### Single synthesis demo
```

### Comparing `pvorcademo-0.2.0/README.md` & `pvorcademo-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 In this demo, we simulate a response from a language model by creating a text stream from a user-defined text.
 We stream that text to Orca and play the synthesized audio as soon as it gets generated.
 
 To run it, execute the following:
 
 ```console
-orca_demo_streaming --access_key ${ACCESS_KEY} --text-to-stream ${TEXT}
+orca_demo_streaming --access_key ${ACCESS_KEY} --text_to_stream ${TEXT}
 ```
 
 Replace `${ACCESS_KEY}` with your `AccessKey` obtained from Picovoice Console and `${TEXT}` with your text to be
 streamed to Orca. Please note that this demo was not tested on macOS.
 
 ### Single synthesis demo
```

### Comparing `pvorcademo-0.2.0/pvorcademo/LICENSE` & `pvorcademo-0.2.1/pvorcademo/LICENSE`

 * *Files identical despite different names*

### Comparing `pvorcademo-0.2.0/pvorcademo/orca_demo.py` & `pvorcademo-0.2.1/pvorcademo/orca_demo.py`

 * *Files identical despite different names*

### Comparing `pvorcademo-0.2.0/pvorcademo/orca_demo_streaming.py` & `pvorcademo-0.2.1/pvorcademo/orca_demo_streaming.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             num_tokens_per_second: int,
             model_path: Optional[str] = None,
             library_path: Optional[str] = None,
             audio_wait_chunks: Optional[int] = None,
     ) -> None:
 
         self._orca = pvorca.create(access_key=access_key, model_path=model_path, library_path=library_path)
-        self._orca_stream = self._orca.open_stream()
+        self._orca_stream = self._orca.stream_open()
         self._sample_rate = self._orca.sample_rate
 
         self._play_audio_callback = play_audio_callback
         self._num_tokens_per_second = num_tokens_per_second
         assert self._num_tokens_per_second > 0
 
         self._queue: Queue[Optional[OrcaThread.OrcaInput]] = Queue()
@@ -296,30 +296,30 @@
         "-l",
         help="Absolute path to dynamic library. Default: using the library provided by `pvorca`")
     parser.add_argument(
         "--model_path",
         "-m",
         help="Absolute path to Orca model. Default: using the model provided by `pvorca`")
     parser.add_argument(
-        "--text-to-stream",
+        "--text_to_stream",
         "-t",
         required=True,
         help="Text to be streamed to Orca")
     parser.add_argument(
-        "--tokens-per-second",
+        "--tokens_per_second",
         type=int,
         default=15,
         help="Number of tokens per second to be streamed to Orca, simulating an LLM response.")
     parser.add_argument(
-        "--audio-wait-chunks",
+        "--audio_wait_chunks",
         type=int,
         default=None,
         help="Number of PCM chunks to wait before starting to play audio. Default: system-dependent.")
     parser.add_argument(
-        "--show-audio-devices",
+        "--show_audio_devices",
         action="store_true",
         help="Only list available audio output devices and exit")
     parser.add_argument('--audio-device-index', type=int, default=None, help='Index of input audio device')
     args = parser.parse_args()
 
     if args.show_audio_devices:
         print(StreamingAudioDevice.list_output_devices())
```

### Comparing `pvorcademo-0.2.0/pvorcademo.egg-info/PKG-INFO` & `pvorcademo-0.2.1/pvorcademo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvorcademo
-Version: 0.2.0
+Version: 0.2.1
 Summary: Orca Streaming Text-to-Speech Engine demos
 Home-page: https://github.com/Picovoice/orca
 Author: Picovoice
 Author-email: hello@picovoice.ai
 License: UNKNOWN
 Keywords: Streaming Text-to-Speech,TTS,Speech Synthesis,Voice Generation,Speech Engine
 Platform: UNKNOWN
@@ -63,15 +63,15 @@
 
 In this demo, we simulate a response from a language model by creating a text stream from a user-defined text.
 We stream that text to Orca and play the synthesized audio as soon as it gets generated.
 
 To run it, execute the following:
 
 ```console
-orca_demo_streaming --access_key ${ACCESS_KEY} --text-to-stream ${TEXT}
+orca_demo_streaming --access_key ${ACCESS_KEY} --text_to_stream ${TEXT}
 ```
 
 Replace `${ACCESS_KEY}` with your `AccessKey` obtained from Picovoice Console and `${TEXT}` with your text to be
 streamed to Orca. Please note that this demo was not tested on macOS.
 
 ### Single synthesis demo
```

### Comparing `pvorcademo-0.2.0/setup.py` & `pvorcademo-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     f.write(manifest_in)
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pvorcademo",
-    version="0.2.0",
+    version="0.2.1",
     author="Picovoice",
     author_email="hello@picovoice.ai",
     description="Orca Streaming Text-to-Speech Engine demos",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Picovoice/orca",
     packages=["pvorcademo"],
-    install_requires=["numpy>=1.24.0", "pvorca==0.2.0", "sounddevice==0.4.6", "tiktoken==0.6.0"],
+    install_requires=["numpy>=1.24.0", "pvorca==0.2.1", "sounddevice==0.4.6", "tiktoken==0.6.0"],
     include_package_data=True,
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
```

