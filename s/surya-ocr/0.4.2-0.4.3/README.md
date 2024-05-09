# Comparing `tmp/surya_ocr-0.4.2.tar.gz` & `tmp/surya_ocr-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surya_ocr-0.4.2.tar", max compression
+gzip compressed data, was "surya_ocr-0.4.3.tar", max compression
```

## Comparing `surya_ocr-0.4.2.tar` & `surya_ocr-0.4.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35085 2024-05-08 19:31:12.118507 surya_ocr-0.4.2/LICENSE
--rw-r--r--   0        0        0    24927 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/README.md
--rw-r--r--   0        0        0     3084 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/detect_layout.py
--rw-r--r--   0        0        0     3314 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/detect_text.py
--rw-r--r--   0        0        0     6909 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/ocr_app.py
--rw-r--r--   0        0        0     4112 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/ocr_text.py
--rw-r--r--   0        0        0     1326 2024-05-08 19:33:06.349772 surya_ocr-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     3720 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/reading_order.py
--rw-r--r--   0        0        0      530 2024-05-08 19:31:12.122507 surya_ocr-0.4.2/run_ocr_app.py
--rw-r--r--   0        0        0      827 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/benchmark/bbox.py
--rw-r--r--   0        0        0     4239 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/benchmark/metrics.py
--rw-r--r--   0        0        0     4971 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/benchmark/tesseract.py
--rw-r--r--   0        0        0      887 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/benchmark/util.py
--rw-r--r--   0        0        0     4802 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/detection.py
--rw-r--r--   0        0        0      603 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/input/langs.py
--rw-r--r--   0        0        0     2268 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/input/load.py
--rw-r--r--   0        0        0     3167 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/input/processing.py
--rw-r--r--   0        0        0     2138 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/languages.py
--rw-r--r--   0        0        0     8598 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/layout.py
--rw-r--r--   0        0        0     6139 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/detection/segformer.py
--rw-r--r--   0        0        0      159 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/ordering/config.py
--rw-r--r--   0        0        0    25734 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/ordering/decoder.py
--rw-r--r--   0        0        0     3670 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/ordering/encoder.py
--rw-r--r--   0        0        0     3902 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/ordering/encoderdecoder.py
--rw-r--r--   0        0        0     1568 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/ordering/model.py
--rw-r--r--   0        0        0     6199 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/ordering/processor.py
--rw-r--r--   0        0        0     1676 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/recognition/config.py
--rw-r--r--   0        0        0    32140 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/recognition/decoder.py
--rw-r--r--   0        0        0     2762 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/recognition/encoder.py
--rw-r--r--   0        0        0     2646 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/recognition/model.py
--rw-r--r--   0        0        0     9296 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/recognition/processor.py
--rw-r--r--   0        0        0     3588 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/model/recognition/tokenizer.py
--rw-r--r--   0        0        0     4154 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/ocr.py
--rw-r--r--   0        0        0     5667 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/ordering.py
--rw-r--r--   0        0        0     6085 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/postprocessing/affinity.py
--rw-r--r--   0        0        0      853 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/postprocessing/fonts.py
--rw-r--r--   0        0        0     7862 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/postprocessing/heatmap.py
--rw-r--r--   0        0        0     3313 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/postprocessing/math/latex.py
--rw-r--r--   0        0        0     3114 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/postprocessing/math/render.py
--rw-r--r--   0        0        0     4382 2024-05-08 19:31:12.266506 surya_ocr-0.4.2/surya/postprocessing/text.py
--rw-r--r--   0        0        0     1253 2024-05-08 19:31:12.270506 surya_ocr-0.4.2/surya/postprocessing/util.py
--rw-r--r--   0        0        0     3882 2024-05-08 19:31:12.270506 surya_ocr-0.4.2/surya/recognition.py
--rw-r--r--   0        0        0     4529 2024-05-08 19:31:12.270506 surya_ocr-0.4.2/surya/schema.py
--rw-r--r--   0        0        0     3615 2024-05-08 19:31:12.270506 surya_ocr-0.4.2/surya/settings.py
--rw-r--r--   0        0        0    26225 1970-01-01 00:00:00.000000 surya_ocr-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35085 2024-05-08 20:02:32.504612 surya_ocr-0.4.3/LICENSE
+-rw-r--r--   0        0        0    24927 2024-05-08 20:02:32.504612 surya_ocr-0.4.3/README.md
+-rw-r--r--   0        0        0     3084 2024-05-08 20:02:32.504612 surya_ocr-0.4.3/detect_layout.py
+-rw-r--r--   0        0        0     3314 2024-05-08 20:02:32.504612 surya_ocr-0.4.3/detect_text.py
+-rw-r--r--   0        0        0     6909 2024-05-08 20:02:32.504612 surya_ocr-0.4.3/ocr_app.py
+-rw-r--r--   0        0        0     4112 2024-05-08 20:02:32.504612 surya_ocr-0.4.3/ocr_text.py
+-rw-r--r--   0        0        0     1342 2024-05-08 20:02:32.504612 surya_ocr-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3720 2024-05-08 20:02:32.504612 surya_ocr-0.4.3/reading_order.py
+-rw-r--r--   0        0        0      530 2024-05-08 20:02:32.504612 surya_ocr-0.4.3/run_ocr_app.py
+-rw-r--r--   0        0        0      827 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/benchmark/bbox.py
+-rw-r--r--   0        0        0     4239 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/benchmark/metrics.py
+-rw-r--r--   0        0        0     4971 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/benchmark/tesseract.py
+-rw-r--r--   0        0        0      887 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/benchmark/util.py
+-rw-r--r--   0        0        0     4802 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/detection.py
+-rw-r--r--   0        0        0      603 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/input/langs.py
+-rw-r--r--   0        0        0     2268 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/input/load.py
+-rw-r--r--   0        0        0     3167 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/input/processing.py
+-rw-r--r--   0        0        0     2138 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/languages.py
+-rw-r--r--   0        0        0     8598 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/layout.py
+-rw-r--r--   0        0        0     6139 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/detection/segformer.py
+-rw-r--r--   0        0        0      159 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/ordering/config.py
+-rw-r--r--   0        0        0    25734 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/ordering/decoder.py
+-rw-r--r--   0        0        0     3670 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/ordering/encoder.py
+-rw-r--r--   0        0        0     3902 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/ordering/encoderdecoder.py
+-rw-r--r--   0        0        0     1568 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/ordering/model.py
+-rw-r--r--   0        0        0     6199 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/ordering/processor.py
+-rw-r--r--   0        0        0     1676 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/recognition/config.py
+-rw-r--r--   0        0        0    32140 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/recognition/decoder.py
+-rw-r--r--   0        0        0     2762 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/recognition/encoder.py
+-rw-r--r--   0        0        0     2646 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/recognition/model.py
+-rw-r--r--   0        0        0     9296 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/recognition/processor.py
+-rw-r--r--   0        0        0     3588 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/model/recognition/tokenizer.py
+-rw-r--r--   0        0        0     4154 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/ocr.py
+-rw-r--r--   0        0        0     5667 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/ordering.py
+-rw-r--r--   0        0        0     6085 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/postprocessing/affinity.py
+-rw-r--r--   0        0        0      853 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/postprocessing/fonts.py
+-rw-r--r--   0        0        0     7862 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/postprocessing/heatmap.py
+-rw-r--r--   0        0        0     3313 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/postprocessing/math/latex.py
+-rw-r--r--   0        0        0     3114 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/postprocessing/math/render.py
+-rw-r--r--   0        0        0     4382 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/postprocessing/text.py
+-rw-r--r--   0        0        0     1253 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/postprocessing/util.py
+-rw-r--r--   0        0        0     3882 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/recognition.py
+-rw-r--r--   0        0        0     4529 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/schema.py
+-rw-r--r--   0        0        0     3615 2024-05-08 20:02:32.652613 surya_ocr-0.4.3/surya/settings.py
+-rw-r--r--   0        0        0    26256 1970-01-01 00:00:00.000000 surya_ocr-0.4.3/PKG-INFO
```

### Comparing `surya_ocr-0.4.2/LICENSE` & `surya_ocr-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/README.md` & `surya_ocr-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/detect_layout.py` & `surya_ocr-0.4.3/detect_layout.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/detect_text.py` & `surya_ocr-0.4.3/detect_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/ocr_app.py` & `surya_ocr-0.4.3/ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/ocr_text.py` & `surya_ocr-0.4.3/ocr_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/pyproject.toml` & `surya_ocr-0.4.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surya-ocr"
-version = "0.4.2"
+version = "0.4.3"
 description = "OCR, layout, reading order, and line detection in 90+ languages"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/surya"
 keywords = ["ocr", "pdf", "text detection", "text recognition"]
 packages = [
@@ -18,14 +18,15 @@
     "detect_layout.py",
     "reading_order.py",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13,!=3.9.7"
 transformers = "4.36.2"
+torch = "2.2.2"
 pydantic = "^2.5.3"
 pydantic-settings = "^2.1.0"
 python-dotenv = "^1.0.0"
 pillow = "^10.2.0"
 pypdfium2 = "^4.25.0"
 opencv-python = "^4.9.0.80"
 tabulate = "^0.9.0"
```

### Comparing `surya_ocr-0.4.2/reading_order.py` & `surya_ocr-0.4.3/reading_order.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/run_ocr_app.py` & `surya_ocr-0.4.3/run_ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/benchmark/bbox.py` & `surya_ocr-0.4.3/surya/benchmark/bbox.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/benchmark/metrics.py` & `surya_ocr-0.4.3/surya/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/benchmark/tesseract.py` & `surya_ocr-0.4.3/surya/benchmark/tesseract.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/benchmark/util.py` & `surya_ocr-0.4.3/surya/benchmark/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/detection.py` & `surya_ocr-0.4.3/surya/detection.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/input/langs.py` & `surya_ocr-0.4.3/surya/input/langs.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/input/load.py` & `surya_ocr-0.4.3/surya/input/load.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/input/processing.py` & `surya_ocr-0.4.3/surya/input/processing.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/languages.py` & `surya_ocr-0.4.3/surya/languages.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/layout.py` & `surya_ocr-0.4.3/surya/layout.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/model/detection/segformer.py` & `surya_ocr-0.4.3/surya/model/detection/segformer.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/model/ordering/decoder.py` & `surya_ocr-0.4.3/surya/model/ordering/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/model/ordering/encoder.py` & `surya_ocr-0.4.3/surya/model/ordering/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/model/ordering/encoderdecoder.py` & `surya_ocr-0.4.3/surya/model/ordering/encoderdecoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/model/ordering/model.py` & `surya_ocr-0.4.3/surya/model/ordering/model.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/model/ordering/processor.py` & `surya_ocr-0.4.3/surya/model/ordering/processor.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/model/recognition/config.py` & `surya_ocr-0.4.3/surya/model/recognition/config.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/model/recognition/decoder.py` & `surya_ocr-0.4.3/surya/model/recognition/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/model/recognition/encoder.py` & `surya_ocr-0.4.3/surya/model/recognition/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/model/recognition/model.py` & `surya_ocr-0.4.3/surya/model/recognition/model.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/model/recognition/processor.py` & `surya_ocr-0.4.3/surya/model/recognition/processor.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/model/recognition/tokenizer.py` & `surya_ocr-0.4.3/surya/model/recognition/tokenizer.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/ocr.py` & `surya_ocr-0.4.3/surya/ocr.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/ordering.py` & `surya_ocr-0.4.3/surya/ordering.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/postprocessing/affinity.py` & `surya_ocr-0.4.3/surya/postprocessing/affinity.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/postprocessing/fonts.py` & `surya_ocr-0.4.3/surya/postprocessing/fonts.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/postprocessing/heatmap.py` & `surya_ocr-0.4.3/surya/postprocessing/heatmap.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/postprocessing/math/latex.py` & `surya_ocr-0.4.3/surya/postprocessing/math/latex.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/postprocessing/math/render.py` & `surya_ocr-0.4.3/surya/postprocessing/math/render.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/postprocessing/text.py` & `surya_ocr-0.4.3/surya/postprocessing/text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/postprocessing/util.py` & `surya_ocr-0.4.3/surya/postprocessing/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/recognition.py` & `surya_ocr-0.4.3/surya/recognition.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/schema.py` & `surya_ocr-0.4.3/surya/schema.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/surya/settings.py` & `surya_ocr-0.4.3/surya/settings.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.2/PKG-INFO` & `surya_ocr-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surya-ocr
-Version: 0.4.2
+Version: 0.4.3
 Summary: OCR, layout, reading order, and line detection in 90+ languages
 Home-page: https://github.com/VikParuchuri/surya
 License: GPL-3.0-or-later
 Keywords: ocr,pdf,text detection,text recognition
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -19,14 +19,15 @@
 Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.1.0,<3.0.0)
 Requires-Dist: pypdfium2 (>=4.25.0,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: torch (==2.2.2)
 Requires-Dist: transformers (==4.36.2)
 Project-URL: Repository, https://github.com/VikParuchuri/surya
 Description-Content-Type: text/markdown
 
 # Surya
 
 Surya is a document OCR toolkit that does:
```

