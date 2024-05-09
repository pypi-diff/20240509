# Comparing `tmp/podonos-0.1.1.tar.gz` & `tmp/podonos-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podonos-0.1.1.tar", last modified: Fri Apr 26 05:39:41 2024, max compression
+gzip compressed data, was "podonos-0.1.3.tar", last modified: Thu May  9 05:04:35 2024, max compression
```

## Comparing `podonos-0.1.1.tar` & `podonos-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 soohyun    (501) staff       (20)        0 2024-04-26 05:39:41.798365 podonos-0.1.1/
--rw-r--r--   0 soohyun    (501) staff       (20)     1063 2024-04-14 07:16:47.000000 podonos-0.1.1/LICENSE
--rw-r--r--   0 soohyun    (501) staff       (20)     3129 2024-04-26 05:39:41.798154 podonos-0.1.1/PKG-INFO
--rw-r--r--   0 soohyun    (501) staff       (20)      997 2024-04-14 07:16:47.000000 podonos-0.1.1/README.md
-drwxr-xr-x   0 soohyun    (501) staff       (20)        0 2024-04-26 05:39:41.796754 podonos-0.1.1/podonos/
--rw-r--r--   0 soohyun    (501) staff       (20)       81 2024-04-26 05:35:43.000000 podonos-0.1.1/podonos/__init__.py
--rw-r--r--   0 soohyun    (501) staff       (20)     1980 2024-04-23 03:57:37.000000 podonos-0.1.1/podonos/audio_meta.py
--rw-r--r--   0 soohyun    (501) staff       (20)      398 2024-04-25 06:32:35.000000 podonos-0.1.1/podonos/constant.py
--rw-r--r--   0 soohyun    (501) staff       (20)      118 2024-04-22 06:38:27.000000 podonos-0.1.1/podonos/default_config.py
--rw-r--r--   0 soohyun    (501) staff       (20)      210 2024-04-22 06:38:27.000000 podonos-0.1.1/podonos/eval_name.py
--rw-r--r--   0 soohyun    (501) staff       (20)    10417 2024-04-26 05:32:12.000000 podonos-0.1.1/podonos/evaluator.py
--rw-r--r--   0 soohyun    (501) staff       (20)     7242 2024-04-25 06:29:56.000000 podonos-0.1.1/podonos/sdk.py
--rw-r--r--   0 soohyun    (501) staff       (20)     2398 2024-04-25 06:31:21.000000 podonos-0.1.1/podonos/version.py
-drwxr-xr-x   0 soohyun    (501) staff       (20)        0 2024-04-26 05:39:41.797920 podonos-0.1.1/podonos.egg-info/
--rw-r--r--   0 soohyun    (501) staff       (20)     3129 2024-04-26 05:39:41.000000 podonos-0.1.1/podonos.egg-info/PKG-INFO
--rw-r--r--   0 soohyun    (501) staff       (20)      368 2024-04-26 05:39:41.000000 podonos-0.1.1/podonos.egg-info/SOURCES.txt
--rw-r--r--   0 soohyun    (501) staff       (20)        1 2024-04-26 05:39:41.000000 podonos-0.1.1/podonos.egg-info/dependency_links.txt
--rw-r--r--   0 soohyun    (501) staff       (20)       19 2024-04-26 05:39:41.000000 podonos-0.1.1/podonos.egg-info/requires.txt
--rw-r--r--   0 soohyun    (501) staff       (20)        8 2024-04-26 05:39:41.000000 podonos-0.1.1/podonos.egg-info/top_level.txt
--rw-r--r--   0 soohyun    (501) staff       (20)      974 2024-04-26 05:35:43.000000 podonos-0.1.1/pyproject.toml
--rw-r--r--   0 soohyun    (501) staff       (20)       38 2024-04-26 05:39:41.798408 podonos-0.1.1/setup.cfg
-drwxr-xr-x   0 soohyun    (501) staff       (20)        0 2024-04-26 05:39:41.797592 podonos-0.1.1/tests/
--rw-r--r--   0 soohyun    (501) staff       (20)     3589 2024-04-22 06:38:27.000000 podonos-0.1.1/tests/test_sdk.py
+drwxrwxr-x   0 soohyun   (1000) soohyun   (1000)        0 2024-05-09 05:04:35.977618 podonos-0.1.3/
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)     1063 2024-04-09 06:37:31.000000 podonos-0.1.3/LICENSE
+-rw-r--r--   0 soohyun   (1000) soohyun   (1000)     3233 2024-05-09 05:04:35.977618 podonos-0.1.3/PKG-INFO
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)     1098 2024-05-09 05:02:55.000000 podonos-0.1.3/README.md
+drwxrwxr-x   0 soohyun   (1000) soohyun   (1000)        0 2024-05-09 05:04:35.977618 podonos-0.1.3/podonos/
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)       81 2024-05-09 05:03:09.000000 podonos-0.1.3/podonos/__init__.py
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)     1980 2024-05-09 00:08:47.000000 podonos-0.1.3/podonos/audio_meta.py
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)      398 2024-05-09 00:08:47.000000 podonos-0.1.3/podonos/constant.py
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)      118 2024-05-09 00:08:47.000000 podonos-0.1.3/podonos/default_config.py
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)      252 2024-05-09 03:32:57.000000 podonos-0.1.3/podonos/eval_name.py
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)    11392 2024-05-09 03:32:57.000000 podonos-0.1.3/podonos/evaluator.py
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)     7416 2024-05-09 04:42:19.000000 podonos-0.1.3/podonos/sdk.py
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)     2398 2024-05-09 00:08:47.000000 podonos-0.1.3/podonos/version.py
+drwxrwxr-x   0 soohyun   (1000) soohyun   (1000)        0 2024-05-09 05:04:35.977618 podonos-0.1.3/podonos.egg-info/
+-rw-r--r--   0 soohyun   (1000) soohyun   (1000)     3233 2024-05-09 05:04:35.000000 podonos-0.1.3/podonos.egg-info/PKG-INFO
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)      368 2024-05-09 05:04:35.000000 podonos-0.1.3/podonos.egg-info/SOURCES.txt
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)        1 2024-05-09 05:04:35.000000 podonos-0.1.3/podonos.egg-info/dependency_links.txt
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)       19 2024-05-09 05:04:35.000000 podonos-0.1.3/podonos.egg-info/requires.txt
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)        8 2024-05-09 05:04:35.000000 podonos-0.1.3/podonos.egg-info/top_level.txt
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)      977 2024-05-09 05:03:09.000000 podonos-0.1.3/pyproject.toml
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)       38 2024-05-09 05:04:35.977618 podonos-0.1.3/setup.cfg
+drwxrwxr-x   0 soohyun   (1000) soohyun   (1000)        0 2024-05-09 05:04:35.977618 podonos-0.1.3/tests/
+-rw-rw-r--   0 soohyun   (1000) soohyun   (1000)     4279 2024-05-09 04:03:32.000000 podonos-0.1.3/tests/test_sdk.py
```

### Comparing `podonos-0.1.1/LICENSE` & `podonos-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `podonos-0.1.1/PKG-INFO` & `podonos-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: podonos
-Version: 0.1.1
+Version: 0.1.3
 Summary: Managed evaluation for audio & speech
-Author-email: Soohyun Bae <sb@podonos.com>
+Author-email: David Anderson <da@podonos.com>
 License: MIT License
         
         Copyright (c) 2024 Podonos
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -71,13 +71,20 @@
 for i in script_list:
   gen_audio = my_model.generate_and_save(i, script_list[i], f'/a/b/{i}.wav')
   etor.add_file(f'/a/b/{i}.wav')
 etor.close()
 ```
 Once we evaluate the audio files, we will email you the evaluation report within 12 hours.
 
+## 👌 How to run the code testing
+
+Run this at the base directory:
+```bash
+python -m unittest
+```
+
 ## 📗 Documentation
 
 For a deeper dive on all capabilities and details, please refer to [Documentation](https://docs.podonos.com/).
 
 ## 📑 License
 [MIT License](https://github.com/podonos/pysdk/blob/main/LICENSE)
```

### Comparing `podonos-0.1.1/README.md` & `podonos-0.1.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -27,13 +27,20 @@
 for i in script_list:
   gen_audio = my_model.generate_and_save(i, script_list[i], f'/a/b/{i}.wav')
   etor.add_file(f'/a/b/{i}.wav')
 etor.close()
 ```
 Once we evaluate the audio files, we will email you the evaluation report within 12 hours.
 
+## 👌 How to run the code testing
+
+Run this at the base directory:
+```bash
+python -m unittest
+```
+
 ## 📗 Documentation
 
 For a deeper dive on all capabilities and details, please refer to [Documentation](https://docs.podonos.com/).
 
 ## 📑 License
 [MIT License](https://github.com/podonos/pysdk/blob/main/LICENSE)
```

### Comparing `podonos-0.1.1/podonos/audio_meta.py` & `podonos-0.1.3/podonos/audio_meta.py`

 * *Files identical despite different names*

### Comparing `podonos-0.1.1/podonos/evaluator.py` & `podonos-0.1.3/podonos/evaluator.py`

 * *Files 10% similar despite different names*

```diff
@@ -146,14 +146,31 @@
             audio_json['name0'] = path_base0
             audio_json['nchannels0'] = nchannels0
             audio_json['framerate0'] = framerate0
             audio_json['duration_in_ms0'] = duration_in_ms0
             if 'tag' in kwargs:
                 audio_json['tag'] = kwargs['tag']
 
+        if 'P808' == self._eval_config['eval_type']:
+            if 'path' not in kwargs:
+                raise ValueError(f'"path" must be set for the evaluation type {self._eval_config["eval_type"]}')
+            path0 = kwargs['path']
+            path_base0 = os.path.basename(path0)
+            assert os.path.isfile(path0), f"File {path0} doesn't exist"
+            assert os.access(path0, os.R_OK), f"File {path0} isn't readable"
+            remote_object_name0 = os.path.join(self._eval_config['eval_creation_timestamp'], path_base0)
+            log.debug(f'remote_object_name: {remote_object_name0}\n')
+            nchannels0, framerate0, duration_in_ms0 = get_audio_info(path0)
+            audio_json['name0'] = path_base0
+            audio_json['nchannels0'] = nchannels0
+            audio_json['framerate0'] = framerate0
+            audio_json['duration_in_ms0'] = duration_in_ms0
+            if 'tag' in kwargs:
+                audio_json['tag'] = kwargs['tag']
+
         if 'SMOS' == self._eval_config['eval_type']:
             if 'path' in kwargs:
                 raise ValueError(f'"path" must not be set for {self._eval_config["_eval_type"]}')
             if 'path0' not in kwargs or 'path1' not in kwargs:
                 raise ValueError(f'Both "path0" and "path1" must be set for {self._eval_config["_eval_type"]}')
             path0 = kwargs['path0']
             path1 = kwargs['path1']
```

### Comparing `podonos-0.1.1/podonos/sdk.py` & `podonos-0.1.3/podonos/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,20 +48,21 @@
     def __init__(self, api_key, api_base_url):
         self._api_key = api_key
         self._api_base_url = api_base_url
         self._initialized = True
 
     def create_evaluator(self, **kwargs) -> Evaluator:
         """Creates a new evaluator with a unique evaluation session ID.
+        For the language code, see https://docs.dyspatch.io/localization/supported_languages/
 
         Args:
             name: This session name. Its length must be > 1. If empty, a random name is used. Optional.
             desc: Description of this session. Optional.
-            type: Evaluation type. One of {'NMOS', 'SMOS'}. Default: NMOS
-            lan: Human language for this audio. One of {'en-us', 'audio'}. Default: en-us
+            type: Evaluation type. One of {'NMOS', 'SMOS', 'P808'}. Default: NMOS
+            lan: Human language for this audio. One of {'en-us', 'ko-kr', 'audio'}. Default: en-us
             num_eval: The minimum number of repetition for each audio evaluation. Should be >=1. Default: 3.
             due_hours: An expected number of days of finishing this mission and getting the evaluation report.
                       Must be >= 12. Default: 12.
 
         Returns:
             Evaluator instance.
 
@@ -94,28 +95,28 @@
 
         # Evaluation type
         if 'type' not in kwargs:
             eval_type = 'NMOS'
         else:
             eval_type = kwargs['type']
         # We support one evaluation type in one session.
-        if eval_type not in ['NMOS', 'SMOS']:
-            raise ValueError(f'"type" must be one of {{NMOS, SMOS}}. '
+        if eval_type not in ['NMOS', 'SMOS', 'P808']:
+            raise ValueError(f'"type" must be one of {{NMOS, SMOS, P808}}. '
                              f'Do you want other evaluation types? Let us know at {PODONOS_CONTACT_EMAIL}.')
         log.debug(f'Eval type: {eval_type}')
         self._eval_config['eval_type'] = eval_type
 
         # Language
         if 'lan' not in kwargs:
             eval_language = 'en-us'
         else:
             eval_language = kwargs['lan']
 
-        if eval_language not in ['en-us']:
-            raise ValueError(f'"lan" must be {{en-us}}. '
+        if eval_language not in ['en-us', 'ko-kr', 'audio']:
+            raise ValueError(f'"lan" must be one of {{en-us, ko-kr, audio}}. '
                              f'Do you want us to support other languages? Let us know at {PODONOS_CONTACT_EMAIL}.')
         log.debug(f'Language: {eval_language}')
         self._eval_config['eval_lan'] = eval_language
 
         # Num eval per sample
         if 'num_eval' not in kwargs:
             num_eval = DefaultConfig.NUM_EVAL
@@ -129,16 +130,16 @@
         # Expected due
         if 'due_hours' not in kwargs:
             # In 12 hours.
             due_hours = DefaultConfig.DUE_HOURS
         else:
             due_hours = int(kwargs['due_hours'])
         # TODO: allow floating point hours, e.g. 0.5.
-        if due_hours < 1:
-            raise ValueError('"due_hours" must be >=1.')
+        if due_hours < 12:
+            raise ValueError('"due_hours" must be >=12.')
         utcnow = datetime.datetime.now()
         due = utcnow + datetime.timedelta(hours=due_hours)
 
         # Due string in ISO 8601.
         self._eval_config['eval_expected_due'] = due.astimezone().isoformat(timespec='milliseconds')
         self._eval_config['eval_expected_due_tzname'] = utcnow.astimezone().tzname()
         log.debug(f'Expected due: {self._eval_config["eval_expected_due"]} '
@@ -185,15 +186,15 @@
 
         Podonos._api_key = api_key
         Podonos._api_base_url = api_base_url
 
         headers = {
             'x-api-key': Podonos._api_key
         }
-        response = requests.get(f'{Podonos._api_base_url}/clients/verify', headers=headers)
+        response = requests.get(f'{Podonos._api_base_url}/clients/verify/api-key', headers=headers)
         if response.status_code != 200:
             raise requests.exceptions.HTTPError
 
         # Successfully initialized.
         Podonos._initialized = True
 
         client = EvalClient(Podonos._api_key, Podonos._api_base_url)
```

### Comparing `podonos-0.1.1/podonos/version.py` & `podonos-0.1.3/podonos/version.py`

 * *Files identical despite different names*

### Comparing `podonos-0.1.1/podonos.egg-info/PKG-INFO` & `podonos-0.1.3/podonos.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: podonos
-Version: 0.1.1
+Version: 0.1.3
 Summary: Managed evaluation for audio & speech
-Author-email: Soohyun Bae <sb@podonos.com>
+Author-email: David Anderson <da@podonos.com>
 License: MIT License
         
         Copyright (c) 2024 Podonos
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -71,13 +71,20 @@
 for i in script_list:
   gen_audio = my_model.generate_and_save(i, script_list[i], f'/a/b/{i}.wav')
   etor.add_file(f'/a/b/{i}.wav')
 etor.close()
 ```
 Once we evaluate the audio files, we will email you the evaluation report within 12 hours.
 
+## 👌 How to run the code testing
+
+Run this at the base directory:
+```bash
+python -m unittest
+```
+
 ## 📗 Documentation
 
 For a deeper dive on all capabilities and details, please refer to [Documentation](https://docs.podonos.com/).
 
 ## 📑 License
 [MIT License](https://github.com/podonos/pysdk/blob/main/LICENSE)
```

### Comparing `podonos-0.1.1/pyproject.toml` & `podonos-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "podonos"
-version = "0.1.1"
+version = "0.1.3"
 description = "Managed evaluation for audio & speech"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
-    {name = "Soohyun Bae", email = "sb@podonos.com"}
+    {name = "David Anderson", email = "da@podonos.com"}
 ]
 requires-python = ">=3.8"
 dependencies = [
     "packaging",
     "requests"
 ]
 keywords = ["ai", "speech", "synthesis"]
```

### Comparing `podonos-0.1.1/tests/test_sdk.py` & `podonos-0.1.3/tests/test_sdk.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,30 +2,37 @@
 import unittest
 from unittest import mock
 
 
 # Mocks HTTP GET request.
 def mocked_requests_get(*args, **kwargs):
     class MockResponse:
-        def __init__(self, response_text, status_code):
-            self.text = response_text
+        def __init__(self, response_text, response_json, status_code):
+            self.text_response = response_text
+            self.json_response = response_json
             self.status_code = status_code
 
         def json(self):
-            return self.json_data
+            return self.json_response
 
     if '/clients/verify' in args[0]:
         # API key verification
-        return MockResponse('true', 200)
+        return MockResponse('true', None, 200)
 
-    if '/version/min-required' in args[0]:
-        # Minimum version
-        return MockResponse('0.0.1', 200)
+    if '/version/sdk' in args[0]:
+        # SDK versions
+        version_response = dict(
+            latest="0.1.0",
+            recommended="0.0.12",
+            minimum="0.0.12")
+        return MockResponse(None,
+                            version_response,
+                            200)
 
-    return MockResponse(None, 404)
+    return MockResponse(None, None, 404)
 
 
 class TestPodonos(unittest.TestCase):
 
     @mock.patch('requests.get', side_effect=mocked_requests_get)
     def test_init(self, mock_get):
         # Invalid api_key
@@ -46,68 +53,84 @@
         valid_api_key = "1234567890"
         self._mock_client = podonos.init(api_key=valid_api_key)
 
         self.config = {
             'name': 'my_new_model_03272024_p1_k2_en_us',
             'desc': 'Updated model',
             'type': 'NMOS',
-            'language': 'en-us'
+            'lan': 'en-us'
         }
 
     @mock.patch('requests.get', side_effect=mocked_requests_get)
     def test_create_evaluator(self, mock_get):
         # Missing name is allowed.
         etor = self._mock_client.create_evaluator(
             desc=self.config['desc'],
             type=self.config['type'],
-            language=self.config['language'])
+            lan=self.config['lan'])
         self.assertIsNotNone(etor)
 
         # Too short name.
         with self.assertRaises(ValueError) as context:
             _ = self._mock_client.create_evaluator(
                 name='a',
                 desc=self.config['desc'],
                 type=self.config['type'],
-                language=self.config['language'])
+                lan=self.config['lan'])
 
         # Missing description is allowed.
         etor = self._mock_client.create_evaluator(
             name=self.config['name'],
             type=self.config['type'],
-            language=self.config['language'])
+            lan=self.config['lan'])
         self.assertIsNotNone(etor)
 
         # Unknown type.
         with self.assertRaises(ValueError) as context:
             _ = self._mock_client.create_evaluator(
                 name=self.config['name'],
                 desc=self.config['desc'],
                 type="unknown_type",
-                language=self.config['language'])
+                lan=self.config['lan'])
 
         # Missing language is allowed.
         etor = self._mock_client.create_evaluator(
             name=self.config['name'],
             desc=self.config['desc'],
             type=self.config['type'])
         self.assertIsNotNone(etor)
 
         # Invalid language.
         with self.assertRaises(ValueError) as context:
             _ = self._mock_client.create_evaluator(
                 name=self.config['name'],
                 desc=self.config['desc'],
                 type=self.config['type'],
-                language='abcd')
+                lan='abcd')
 
         # Valid configuration
         etor = self._mock_client.create_evaluator(
             name=self.config['name'],
             desc=self.config['desc'],
             type=self.config['type'],
-            language=self.config['language'])
+            lan=self.config['lan'])
+        self.assertIsNotNone(etor)
+
+        # P.808
+        etor = self._mock_client.create_evaluator(
+            name=self.config['name'],
+            desc=self.config['desc'],
+            type='P808',
+            lan=self.config['lan'])
+        self.assertIsNotNone(etor)
+
+        # SMOS
+        etor = self._mock_client.create_evaluator(
+            name=self.config['name'],
+            desc=self.config['desc'],
+            type='SMOS',
+            lan=self.config['lan'])
         self.assertIsNotNone(etor)
 
 
 if __name__ == '__main__':
     unittest.main()
```

