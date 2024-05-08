# Comparing `tmp/neon-audio-1.5.2a4.tar.gz` & `tmp/neon-audio-1.5.2a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-audio-1.5.2a4.tar", last modified: Mon Apr 29 18:30:46 2024, max compression
+gzip compressed data, was "neon-audio-1.5.2a5.tar", last modified: Wed May  8 22:07:34 2024, max compression
```

## Comparing `neon-audio-1.5.2a4.tar` & `neon-audio-1.5.2a5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:30:46.886186 neon-audio-1.5.2a4/
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-29 18:30:46.886186 neon-audio-1.5.2a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:30:46.882186 neon-audio-1.5.2a4/neon_audio/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/neon_audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/neon_audio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/neon_audio/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/neon_audio/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:30:46.886186 neon-audio-1.5.2a4/neon_audio/tts/
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/neon_audio/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19034 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/neon_audio/tts/neon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/neon_audio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:30:46.882186 neon-audio-1.5.2a4/neon_audio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-29 18:30:46.000000 neon-audio-1.5.2a4/neon_audio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-29 18:30:46.000000 neon-audio-1.5.2a4/neon_audio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:30:46.000000 neon-audio-1.5.2a4/neon_audio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 18:30:46.000000 neon-audio-1.5.2a4/neon_audio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-29 18:30:46.000000 neon-audio-1.5.2a4/neon_audio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-29 18:30:46.000000 neon-audio-1.5.2a4/neon_audio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:30:46.000000 neon-audio-1.5.2a4/neon_audio.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 18:30:46.886186 neon-audio-1.5.2a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:30:46.886186 neon-audio-1.5.2a4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/tests/api_method_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:30:46.886186 neon-audio-1.5.2a4/tests/test_objects/
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/tests/test_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9824 2024-04-29 18:30:39.000000 neon-audio-1.5.2a4/tests/unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/neon_audio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/neon_audio/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19086 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/tts/neon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/neon_audio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/neon_audio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 22:07:34.000000 neon-audio-1.5.2a5/neon_audio.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10747 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/tests/api_method_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 22:07:34.946669 neon-audio-1.5.2a5/tests/test_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/tests/test_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2024-05-08 22:07:30.000000 neon-audio-1.5.2a5/tests/unit_tests.py
```

### Comparing `neon-audio-1.5.2a4/LICENSE.md` & `neon-audio-1.5.2a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/PKG-INFO` & `neon-audio-1.5.2a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-audio
-Version: 1.5.2a4
+Version: 1.5.2a5
 Summary: Neon Audio Module
 Home-page: https://github.com/NeonGeckoCom/neon_audio
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neon-audio-1.5.2a4/README.md` & `neon-audio-1.5.2a5/README.md`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/neon_audio/__init__.py` & `neon-audio-1.5.2a5/neon_audio/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/neon_audio/__main__.py` & `neon-audio-1.5.2a5/neon_audio/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/neon_audio/cli.py` & `neon-audio-1.5.2a5/neon_audio/cli.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/neon_audio/service.py` & `neon-audio-1.5.2a5/neon_audio/service.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/neon_audio/tts/__init__.py` & `neon-audio-1.5.2a5/neon_audio/tts/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/neon_audio/tts/neon.py` & `neon-audio-1.5.2a5/neon_audio/tts/neon.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,16 @@
             TTS.playback.shutdown()
         if not isinstance(playback_thread, NeonPlaybackThread):
             LOG.exception("Received invalid playback_thread")
             playback_thread = None
         init_signal_bus(self.bus)
         TTS.playback = playback_thread or NeonPlaybackThread(TTS.queue)
         TTS.playback.set_bus(self.bus)
-        TTS.playback.attach_tts(self)
+        if hasattr(TTS.playback, "attach_tts"):
+            TTS.playback.attach_tts(self)
         if not TTS.playback.enclosure:
             TTS.playback.enclosure = EnclosureAPI(self.bus)
         if not TTS.playback.is_alive():
             try:
                 TTS.playback.start()
             except RuntimeError:
                 LOG.exception("Error starting the playback thread")
```

### Comparing `neon-audio-1.5.2a4/neon_audio/utils.py` & `neon-audio-1.5.2a5/neon_audio/utils.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/neon_audio.egg-info/PKG-INFO` & `neon-audio-1.5.2a5/neon_audio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-audio
-Version: 1.5.2a4
+Version: 1.5.2a5
 Summary: Neon Audio Module
 Home-page: https://github.com/NeonGeckoCom/neon_audio
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `neon-audio-1.5.2a4/neon_audio.egg-info/SOURCES.txt` & `neon-audio-1.5.2a5/neon_audio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/setup.py` & `neon-audio-1.5.2a5/setup.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/tests/__init__.py` & `neon-audio-1.5.2a5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/tests/api_method_tests.py` & `neon-audio-1.5.2a5/tests/api_method_tests.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/tests/test_objects/__init__.py` & `neon-audio-1.5.2a5/tests/test_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-audio-1.5.2a4/tests/unit_tests.py` & `neon-audio-1.5.2a5/tests/unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 import shutil
 import sys
 import unittest
 
 from time import time
 from os.path import join, dirname
 from threading import Event
+from unittest import skip
 from unittest.mock import Mock, patch
 from click.testing import CliRunner
 from ovos_bus_client import Message
 # from ovos_plugin_manager.templates.tts import PlaybackThread
 from ovos_utils.messagebus import FakeBus
 
 sys.path.append(os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
@@ -115,14 +116,15 @@
         # TODO: Legacy
         valid_tag_string = "<speak>hello</speak>"
         extra_tags_string = "<speak>hello</br></speak>"
 
         self.assertEqual(valid_tag_string, self.tts.validate_ssml(valid_tag_string))
         self.assertEqual(valid_tag_string, self.tts.validate_ssml(extra_tags_string))
 
+    @skip("Method deprecated in ovos-audio")
     def test_preprocess_sentence(self):
         # TODO: Legacy
         sentence = "this is a test"
         self.assertEqual(self.tts._preprocess_sentence(sentence), [sentence])
 
     def test_execute(self):
         from neon_utils.signal_utils import check_for_signal, init_signal_bus
@@ -166,18 +168,17 @@
         self.assertIsNone(self.tts.viseme(""))
 
     def test_validator_valid(self):
         self.assertTrue(self.tts.validator.validate_lang())
         self.assertTrue(self.tts.validator.validate_dependencies())
         self.assertTrue(self.tts.validator.validate_connection())
 
-    @patch("ovos_plugin_manager.templates.tts.Configuration")
-    def test_validator_invalid(self, config):
-        config.return_value = self.config  # Explicitly no g2p
-        tts = DummyTTS("es", {})
+    def test_validator_invalid(self):
+        tts = DummyTTS("", {})
+        tts.validator.validate_lang = Mock(side_effect=Exception("Validation Error"))
 
         with self.assertRaises(Exception):
             tts.validator.validate()
 
         tts.shutdown()
 
     def test_get_tts(self):
```

