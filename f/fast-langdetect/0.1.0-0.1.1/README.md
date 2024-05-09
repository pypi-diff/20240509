# Comparing `tmp/fast_langdetect-0.1.0.tar.gz` & `tmp/fast_langdetect-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_langdetect-0.1.0.tar", last modified: Thu Jan 18 07:10:22 2024, max compression
+gzip compressed data, was "fast_langdetect-0.1.1.tar", last modified: Thu May  9 04:52:33 2024, max compression
```

## Comparing `fast_langdetect-0.1.0.tar` & `fast_langdetect-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1065 2024-01-18 07:10:10.883337 fast_langdetect-0.1.0/LICENSE
--rw-r--r--   0        0        0     2258 2024-01-18 07:10:10.883337 fast_langdetect-0.1.0/README.md
--rw-r--r--   0        0        0      559 2024-01-18 07:10:22.591432 fast_langdetect-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      152 2024-01-18 07:10:10.883337 fast_langdetect-0.1.0/src/fast_langdetect/__init__.py
--rw-r--r--   0        0        0     1070 2024-01-18 07:10:10.883337 fast_langdetect-0.1.0/src/fast_langdetect/ft_detect/LICENSE
--rw-r--r--   0        0        0      763 2024-01-18 07:10:10.883337 fast_langdetect-0.1.0/src/fast_langdetect/ft_detect/__init__.py
--rw-r--r--   0        0        0     3457 2024-01-18 07:10:10.883337 fast_langdetect-0.1.0/src/fast_langdetect/ft_detect/infer.py
--rw-r--r--   0        0        0     2002 2024-01-18 07:10:10.883337 fast_langdetect-0.1.0/src/fast_langdetect/split/__init__.py
--rw-r--r--   0        0        0     2202 2024-01-18 07:10:10.883337 fast_langdetect-0.1.0/src/fast_langdetect/split/cut.py
--rw-r--r--   0        0        0        3 2024-01-18 07:10:10.883337 fast_langdetect-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      809 2024-01-18 07:10:10.883337 fast_langdetect-0.1.0/tests/test_detect.py
--rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 fast_langdetect-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-09 04:52:20.759880 fast_langdetect-0.1.1/LICENSE
+-rw-r--r--   0        0        0      186 2024-05-09 04:52:20.759880 fast_langdetect-0.1.1/NOTICE.MD
+-rw-r--r--   0        0        0     2305 2024-05-09 04:52:20.759880 fast_langdetect-0.1.1/README.md
+-rw-r--r--   0        0        0      582 2024-05-09 04:52:33.504030 fast_langdetect-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-05-09 04:52:20.759880 fast_langdetect-0.1.1/src/fast_langdetect/__init__.py
+-rw-r--r--   0        0        0     1070 2024-05-09 04:52:20.759880 fast_langdetect-0.1.1/src/fast_langdetect/ft_detect/LICENSE
+-rw-r--r--   0        0        0      763 2024-05-09 04:52:20.759880 fast_langdetect-0.1.1/src/fast_langdetect/ft_detect/__init__.py
+-rw-r--r--   0        0        0     3457 2024-05-09 04:52:20.759880 fast_langdetect-0.1.1/src/fast_langdetect/ft_detect/infer.py
+-rw-r--r--   0        0        0     2002 2024-05-09 04:52:20.759880 fast_langdetect-0.1.1/src/fast_langdetect/split/__init__.py
+-rw-r--r--   0        0        0     2202 2024-05-09 04:52:20.759880 fast_langdetect-0.1.1/src/fast_langdetect/split/cut.py
+-rw-r--r--   0        0        0        3 2024-05-09 04:52:20.759880 fast_langdetect-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      809 2024-05-09 04:52:20.759880 fast_langdetect-0.1.1/tests/test_detect.py
+-rw-r--r--   0        0        0     2698 1970-01-01 00:00:00.000000 fast_langdetect-0.1.1/PKG-INFO
```

### Comparing `fast_langdetect-0.1.0/LICENSE` & `fast_langdetect-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_langdetect-0.1.0/README.md` & `fast_langdetect-0.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,67 @@
-# fast-langdetect
+# fast-langdetect 🚀
 
 [![PyPI version](https://badge.fury.io/py/fast-langdetect.svg)](https://badge.fury.io/py/fast-langdetect)
 [![Downloads](https://pepy.tech/badge/fast-langdetect)](https://pepy.tech/project/fast-langdetect)
 [![Downloads](https://pepy.tech/badge/fast-langdetect/month)](https://pepy.tech/project/fast-langdetect/month)
 
-Python 3.8-3.11 support only.
+Python 3.9-3.12 support only. 🐍
 
-80x faster and 95% accurate language identification with Fasttext
+80x faster and 95% accurate language identification with Fasttext 🏎️
 
 This library is a wrapper for the language detection model trained on fasttext by Facebook. For more information, please
-visit: https://fasttext.cc/docs/en/language-identification.html
+visit: https://fasttext.cc/docs/en/language-identification.html 📘
 
 This repository is patched
 from [zafercavdar/fasttext-langdetect](https://github.com/zafercavdar/fasttext-langdetect#benchmark), adding
 multi-language segmentation and better packaging
-support.
+support. 🌐
 
-Facilitates more accurate TTS implementation.
+Facilitates more accurate TTS implementation. 🗣️
 
-## Installation
+**Need 200M+ memory to use low_memory mode** 💾
+
+## Installation 💻
 
 ```bash
 pip install fast-langdetect
 ```
 
-## Usage
+## Usage 🖥️
 
 **For more accurate language detection, please use `detect(text,low_memory=False)` to load the big model.**
 
 **Model will be downloaded in `/tmp/fasttext-langdetect` directory when you first use it.**
 
 ```python
 from fast_langdetect import detect_langs
 
 print(detect_langs("Hello, world!"))
-# [en:0.9999961853027344]
+# EN
 
 print(detect_langs("Привет, мир!"))
-# [ru:0.9999961853027344]
+# RU
 
 
 print(detect_langs("你好，世界！"))
-# [zh:0.9999961853027344]
+# ZH
 
 ```
 
-## Advanced usage
+## Advanced usage 🚀
 
 ```python
 from fast_langdetect import detect, parse_sentence, detect_multilingual
 
 print(detect("Hello, world!"))
 # {'lang': 'en', 'score': 0.1520957201719284}
 
 print(detect_multilingual("Hello, world!你好世界!Привет, мир!"))
 # [{'lang': 'ru', 'score': 0.39008623361587524}, {'lang': 'zh', 'score': 0.18235979974269867}, {'lang': 'ja', 'score': 0.08473210036754608}, {'lang': 'sr', 'score': 0.057975586503744125}, {'lang': 'en', 'score': 0.05422825738787651}]
 
 print(parse_sentence("你好世界！Hello, world！Привет, мир！"))
 # [{'text': '你好世界！Hello, world！', 'lang': 'ZH', 'length': 18}, {'text': 'Привет, мир！', 'lang': 'UK', 'length': 12}, {'text': '', 'lang': 'EN', 'length': 0}]
 ```
 
-## Accuracy
+## Accuracy 🎯
 
 References to the [benchmark](https://github.com/zafercavdar/fasttext-langdetect#benchmark)
```

### Comparing `fast_langdetect-0.1.0/pyproject.toml` & `fast_langdetect-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [project]
 name = "fast-langdetect"
-version = "0.1.0"
+version = "0.1.1"
 description = "Quickly detect text language and segment language"
 authors = [
     { name = "sudoskys", email = "coldlando@hotmail.com" },
 ]
 dependencies = [
     "fasttext-wheel>=0.9.2",
     "requests>=2.31.0",
     "robust-downloader>=0.0.2",
+    "numpy>=1.26.4,<2.0.0",
 ]
-requires-python = ">=3.8,<3.12"
+requires-python = ">=3.9,<3.13"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
-package-type = "library"
+distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest>=7.4.4",
 ]
```

### Comparing `fast_langdetect-0.1.0/src/fast_langdetect/ft_detect/LICENSE` & `fast_langdetect-0.1.1/src/fast_langdetect/ft_detect/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_langdetect-0.1.0/src/fast_langdetect/ft_detect/__init__.py` & `fast_langdetect-0.1.1/src/fast_langdetect/ft_detect/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_langdetect-0.1.0/src/fast_langdetect/ft_detect/infer.py` & `fast_langdetect-0.1.1/src/fast_langdetect/ft_detect/infer.py`

 * *Files identical despite different names*

### Comparing `fast_langdetect-0.1.0/src/fast_langdetect/split/__init__.py` & `fast_langdetect-0.1.1/src/fast_langdetect/split/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_langdetect-0.1.0/src/fast_langdetect/split/cut.py` & `fast_langdetect-0.1.1/src/fast_langdetect/split/cut.py`

 * *Files identical despite different names*

### Comparing `fast_langdetect-0.1.0/tests/test_detect.py` & `fast_langdetect-0.1.1/tests/test_detect.py`

 * *Files identical despite different names*

### Comparing `fast_langdetect-0.1.0/PKG-INFO` & `fast_langdetect-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,77 +1,80 @@
 Metadata-Version: 2.1
 Name: fast-langdetect
-Version: 0.1.0
+Version: 0.1.1
 Summary: Quickly detect text language and segment language
 Author-Email: sudoskys <coldlando@hotmail.com>
 License: MIT
-Requires-Python: <3.12,>=3.8
+Requires-Python: <3.13,>=3.9
 Requires-Dist: fasttext-wheel>=0.9.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: robust-downloader>=0.0.2
+Requires-Dist: numpy<2.0.0,>=1.26.4
 Description-Content-Type: text/markdown
 
-# fast-langdetect
+# fast-langdetect 🚀
 
 [![PyPI version](https://badge.fury.io/py/fast-langdetect.svg)](https://badge.fury.io/py/fast-langdetect)
 [![Downloads](https://pepy.tech/badge/fast-langdetect)](https://pepy.tech/project/fast-langdetect)
 [![Downloads](https://pepy.tech/badge/fast-langdetect/month)](https://pepy.tech/project/fast-langdetect/month)
 
-Python 3.8-3.11 support only.
+Python 3.9-3.12 support only. 🐍
 
-80x faster and 95% accurate language identification with Fasttext
+80x faster and 95% accurate language identification with Fasttext 🏎️
 
 This library is a wrapper for the language detection model trained on fasttext by Facebook. For more information, please
-visit: https://fasttext.cc/docs/en/language-identification.html
+visit: https://fasttext.cc/docs/en/language-identification.html 📘
 
 This repository is patched
 from [zafercavdar/fasttext-langdetect](https://github.com/zafercavdar/fasttext-langdetect#benchmark), adding
 multi-language segmentation and better packaging
-support.
+support. 🌐
 
-Facilitates more accurate TTS implementation.
+Facilitates more accurate TTS implementation. 🗣️
 
-## Installation
+**Need 200M+ memory to use low_memory mode** 💾
+
+## Installation 💻
 
 ```bash
 pip install fast-langdetect
 ```
 
-## Usage
+## Usage 🖥️
 
 **For more accurate language detection, please use `detect(text,low_memory=False)` to load the big model.**
 
 **Model will be downloaded in `/tmp/fasttext-langdetect` directory when you first use it.**
 
 ```python
 from fast_langdetect import detect_langs
 
 print(detect_langs("Hello, world!"))
-# [en:0.9999961853027344]
+# EN
 
 print(detect_langs("Привет, мир!"))
-# [ru:0.9999961853027344]
+# RU
 
 
 print(detect_langs("你好，世界！"))
-# [zh:0.9999961853027344]
+# ZH
 
 ```
 
-## Advanced usage
+## Advanced usage 🚀
 
 ```python
 from fast_langdetect import detect, parse_sentence, detect_multilingual
 
 print(detect("Hello, world!"))
 # {'lang': 'en', 'score': 0.1520957201719284}
 
 print(detect_multilingual("Hello, world!你好世界!Привет, мир!"))
 # [{'lang': 'ru', 'score': 0.39008623361587524}, {'lang': 'zh', 'score': 0.18235979974269867}, {'lang': 'ja', 'score': 0.08473210036754608}, {'lang': 'sr', 'score': 0.057975586503744125}, {'lang': 'en', 'score': 0.05422825738787651}]
 
 print(parse_sentence("你好世界！Hello, world！Привет, мир！"))
 # [{'text': '你好世界！Hello, world！', 'lang': 'ZH', 'length': 18}, {'text': 'Привет, мир！', 'lang': 'UK', 'length': 12}, {'text': '', 'lang': 'EN', 'length': 0}]
 ```
 
-## Accuracy
+## Accuracy 🎯
 
 References to the [benchmark](https://github.com/zafercavdar/fasttext-langdetect#benchmark)
```

