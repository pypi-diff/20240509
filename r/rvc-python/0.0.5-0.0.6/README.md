# Comparing `tmp/rvc_python-0.0.5.tar.gz` & `tmp/rvc_python-0.0.6.tar.gz`

## Comparing `rvc_python-0.0.5.tar` & `rvc_python-0.0.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 rvc_python-0.0.5/requirements.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/__init__.py
--rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/__main__.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/download_model.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/infer.py
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/configs/config.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/configs/v1/32k.json
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/configs/v1/40k.json
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/configs/v1/48k.json
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/configs/v2/32k.json
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/configs/v2/48k.json
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/audio.py
--rw-r--r--   0        0        0    24751 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/rmvpe.py
--rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/slicer2.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/globals/globals.py
--rw-r--r--   0        0        0    14944 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/attentions.py
--rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/commons.py
--rw-r--r--   0        0        0    40598 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/models.py
--rw-r--r--   0        0        0    39950 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/models_dml.py
--rw-r--r--   0        0        0    28664 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/models_onnx.py
--rw-r--r--   0        0        0    17185 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/modules.py
--rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/onnx_inference.py
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/transforms.py
--rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/modules/F0Predictor/DioF0Predictor.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/modules/F0Predictor/F0Predictor.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/modules/F0Predictor/HarvestF0Predictor.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/modules/F0Predictor/PMF0Predictor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/infer_pack/modules/F0Predictor/__init__.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/jit/__init__.py
--rw-r--r--   0        0        0    11677 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/jit/get_hubert.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/jit/get_rmvpe.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/lib/jit/get_synthesizer.py
--rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/modules/ipex/__init__.py
--rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/modules/ipex/attention.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/modules/ipex/gradscaler.py
--rw-r--r--   0        0        0    12459 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/modules/ipex/hijacks.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/modules/onnx/export.py
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/modules/train/preprocess.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/modules/vc/__init__.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/modules/vc/modules.py
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/modules/vc/pipeline.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 rvc_python-0.0.5/rvc_python/modules/vc/utils.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 rvc_python-0.0.5/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 rvc_python-0.0.5/LICENSE
--rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 rvc_python-0.0.5/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 rvc_python-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 rvc_python-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 rvc_python-0.0.6/requirements.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/__init__.py
+-rw-r--r--   0        0        0     2971 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/__main__.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/download_model.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/infer.py
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/configs/config.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/configs/v1/32k.json
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/configs/v1/40k.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/configs/v1/48k.json
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/configs/v2/32k.json
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/configs/v2/48k.json
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/audio.py
+-rw-r--r--   0        0        0    24751 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/rmvpe.py
+-rw-r--r--   0        0        0     9195 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/slicer2.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/globals/globals.py
+-rw-r--r--   0        0        0    14944 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/attentions.py
+-rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/commons.py
+-rw-r--r--   0        0        0    40598 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/models.py
+-rw-r--r--   0        0        0    39950 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/models_dml.py
+-rw-r--r--   0        0        0    28664 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/models_onnx.py
+-rw-r--r--   0        0        0    17185 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/modules.py
+-rw-r--r--   0        0        0     5351 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/onnx_inference.py
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/transforms.py
+-rw-r--r--   0        0        0     3280 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/modules/F0Predictor/DioF0Predictor.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/modules/F0Predictor/F0Predictor.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/modules/F0Predictor/HarvestF0Predictor.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/modules/F0Predictor/PMF0Predictor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/infer_pack/modules/F0Predictor/__init__.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/jit/__init__.py
+-rw-r--r--   0        0        0    11677 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/jit/get_hubert.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/jit/get_rmvpe.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/lib/jit/get_synthesizer.py
+-rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/modules/ipex/__init__.py
+-rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/modules/ipex/attention.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/modules/ipex/gradscaler.py
+-rw-r--r--   0        0        0    12459 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/modules/ipex/hijacks.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/modules/onnx/export.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/modules/train/preprocess.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/modules/vc/__init__.py
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/modules/vc/modules.py
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/modules/vc/pipeline.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 rvc_python-0.0.6/rvc_python/modules/vc/utils.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 rvc_python-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 rvc_python-0.0.6/LICENSE
+-rw-r--r--   0        0        0     7705 2020-02-02 00:00:00.000000 rvc_python-0.0.6/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 rvc_python-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 rvc_python-0.0.6/PKG-INFO
```

### Comparing `rvc_python-0.0.5/rvc_python/__main__.py` & `rvc_python-0.0.6/rvc_python/__main__.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/download_model.py` & `rvc_python-0.0.6/rvc_python/download_model.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/infer.py` & `rvc_python-0.0.6/rvc_python/infer.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/configs/config.py` & `rvc_python-0.0.6/rvc_python/configs/config.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/configs/v1/32k.json` & `rvc_python-0.0.6/rvc_python/configs/v1/32k.json`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/configs/v1/40k.json` & `rvc_python-0.0.6/rvc_python/configs/v1/40k.json`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/configs/v1/48k.json` & `rvc_python-0.0.6/rvc_python/configs/v1/48k.json`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/configs/v2/32k.json` & `rvc_python-0.0.6/rvc_python/configs/v2/32k.json`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/configs/v2/48k.json` & `rvc_python-0.0.6/rvc_python/configs/v2/48k.json`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/audio.py` & `rvc_python-0.0.6/rvc_python/lib/audio.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         out.mux(p)
 
     out.close()
     inp.close()
 
 
 def audio2(i, o, format, sr):
-    inp = av.open(i, "rb")
-    out = av.open(o, "wb", format=format)
+    inp = av.open(i, "r") # use "r" instead of "rb"
+    out = av.open(o, "w", format=format) # use "w" instead of "wb"
     if format == "ogg":
         format = "libvorbis"
     if format == "f32le":
         format = "pcm_f32le"
 
     ostream = out.add_stream(format, channels=1)
     ostream.sample_rate = sr
```

### Comparing `rvc_python-0.0.5/rvc_python/lib/rmvpe.py` & `rvc_python-0.0.6/rvc_python/lib/rmvpe.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/slicer2.py` & `rvc_python-0.0.6/rvc_python/lib/slicer2.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/infer_pack/attentions.py` & `rvc_python-0.0.6/rvc_python/lib/infer_pack/attentions.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/infer_pack/commons.py` & `rvc_python-0.0.6/rvc_python/lib/infer_pack/commons.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/infer_pack/models.py` & `rvc_python-0.0.6/rvc_python/lib/infer_pack/models.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/infer_pack/models_dml.py` & `rvc_python-0.0.6/rvc_python/lib/infer_pack/models_dml.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/infer_pack/models_onnx.py` & `rvc_python-0.0.6/rvc_python/lib/infer_pack/models_onnx.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/infer_pack/modules.py` & `rvc_python-0.0.6/rvc_python/lib/infer_pack/modules.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/infer_pack/onnx_inference.py` & `rvc_python-0.0.6/rvc_python/lib/infer_pack/onnx_inference.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/infer_pack/transforms.py` & `rvc_python-0.0.6/rvc_python/lib/infer_pack/transforms.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/infer_pack/modules/F0Predictor/DioF0Predictor.py` & `rvc_python-0.0.6/rvc_python/lib/infer_pack/modules/F0Predictor/DioF0Predictor.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/infer_pack/modules/F0Predictor/HarvestF0Predictor.py` & `rvc_python-0.0.6/rvc_python/lib/infer_pack/modules/F0Predictor/HarvestF0Predictor.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/infer_pack/modules/F0Predictor/PMF0Predictor.py` & `rvc_python-0.0.6/rvc_python/lib/infer_pack/modules/F0Predictor/PMF0Predictor.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/jit/__init__.py` & `rvc_python-0.0.6/rvc_python/lib/jit/__init__.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/jit/get_hubert.py` & `rvc_python-0.0.6/rvc_python/lib/jit/get_hubert.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/lib/jit/get_synthesizer.py` & `rvc_python-0.0.6/rvc_python/lib/jit/get_synthesizer.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/modules/ipex/__init__.py` & `rvc_python-0.0.6/rvc_python/modules/ipex/__init__.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/modules/ipex/attention.py` & `rvc_python-0.0.6/rvc_python/modules/ipex/attention.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/modules/ipex/gradscaler.py` & `rvc_python-0.0.6/rvc_python/modules/ipex/gradscaler.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/modules/ipex/hijacks.py` & `rvc_python-0.0.6/rvc_python/modules/ipex/hijacks.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/modules/onnx/export.py` & `rvc_python-0.0.6/rvc_python/modules/onnx/export.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/modules/train/preprocess.py` & `rvc_python-0.0.6/rvc_python/modules/train/preprocess.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/modules/vc/modules.py` & `rvc_python-0.0.6/rvc_python/modules/vc/modules.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/modules/vc/pipeline.py` & `rvc_python-0.0.6/rvc_python/modules/vc/pipeline.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/rvc_python/modules/vc/utils.py` & `rvc_python-0.0.6/rvc_python/modules/vc/utils.py`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/LICENSE` & `rvc_python-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/README.md` & `rvc_python-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rvc_python-0.0.5/pyproject.toml` & `rvc_python-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rvc-python"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="daswer123", email="daswerq123@gmail.com" },
 ]
 description = "Use RVC via console or python scripts"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `rvc_python-0.0.5/PKG-INFO` & `rvc_python-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rvc-python
-Version: 0.0.5
+Version: 0.0.6
 Summary: Use RVC via console or python scripts
 Project-URL: Homepage, https://github.com/daswer123/rvc-python
 Project-URL: Bug Tracker, https://github.com/daswer123/rvc-python/issues
 Author-email: daswer123 <daswerq123@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

