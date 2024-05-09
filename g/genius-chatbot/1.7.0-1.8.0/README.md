# Comparing `tmp/genius_chatbot-1.7.0-py2.py3-none-any.whl.zip` & `tmp/genius_chatbot-1.8.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10514 bytes, number of entries: 9
+Zip file size: 10516 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      352 b- defN 23-May-14 05:52 genius_chatbot/__init__.py
 -rw-r--r--  2.0 unx    23871 b- defN 23-Oct-24 05:48 genius_chatbot/genius_chatbot.py
--rw-r--r--  2.0 unx      116 b- defN 23-Oct-24 05:48 genius_chatbot/version.py
--rw-r--r--  2.0 unx     1059 b- defN 23-Oct-24 05:48 genius_chatbot-1.7.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     7503 b- defN 23-Oct-24 05:48 genius_chatbot-1.7.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Oct-24 05:48 genius_chatbot-1.7.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 23-Oct-24 05:48 genius_chatbot-1.7.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Oct-24 05:48 genius_chatbot-1.7.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      777 b- defN 23-Oct-24 05:48 genius_chatbot-1.7.0.dist-info/RECORD
-9 files, 33874 bytes uncompressed, 9160 bytes compressed:  73.0%
+-rw-r--r--  2.0 unx      116 b- defN 23-Oct-28 03:21 genius_chatbot/version.py
+-rw-r--r--  2.0 unx     1059 b- defN 23-Oct-28 03:22 genius_chatbot-1.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7554 b- defN 23-Oct-28 03:22 genius_chatbot-1.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Oct-28 03:22 genius_chatbot-1.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 23-Oct-28 03:22 genius_chatbot-1.8.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Oct-28 03:22 genius_chatbot-1.8.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      777 b- defN 23-Oct-28 03:22 genius_chatbot-1.8.0.dist-info/RECORD
+9 files, 33925 bytes uncompressed, 9162 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: genius_chatbot/genius_chatbot.py
 Comment: 
 
 Filename: genius_chatbot/version.py
 Comment: 
 
-Filename: genius_chatbot-1.7.0.dist-info/LICENSE
+Filename: genius_chatbot-1.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: genius_chatbot-1.7.0.dist-info/METADATA
+Filename: genius_chatbot-1.8.0.dist-info/METADATA
 Comment: 
 
-Filename: genius_chatbot-1.7.0.dist-info/WHEEL
+Filename: genius_chatbot-1.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: genius_chatbot-1.7.0.dist-info/entry_points.txt
+Filename: genius_chatbot-1.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: genius_chatbot-1.7.0.dist-info/top_level.txt
+Filename: genius_chatbot-1.8.0.dist-info/top_level.txt
 Comment: 
 
-Filename: genius_chatbot-1.7.0.dist-info/RECORD
+Filename: genius_chatbot-1.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genius_chatbot/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '1.7.0'
+__version__ = '1.8.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `genius_chatbot-1.7.0.dist-info/LICENSE` & `genius_chatbot-1.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `genius_chatbot-1.7.0.dist-info/METADATA` & `genius_chatbot-1.8.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genius-chatbot
-Version: 1.7.0
+Version: 1.8.0
 Summary: Use huggingface models to create an intelligent and scalable chatbot
 Home-page: https://github.com/Knuckles-Team/genius-chatbot
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 Maintainer: Audel Rouhi
 Maintainer-email: knucklessg1@gmail.com
 License: MIT
@@ -13,14 +13,15 @@
 Classifier: License :: Public Domain
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: EbookLib (==0.18)
 Requires-Dist: PyMuPDF (==1.23.5)
 Requires-Dist: appengine-python-standard (==1.1.4)
 Requires-Dist: chromadb (==0.4.14)
 Requires-Dist: extract-msg (==0.45.0)
@@ -57,15 +58,15 @@
 ![GitHub top language](https://img.shields.io/github/languages/top/Knuckles-Team/genius-chatbot)
 ![GitHub language count](https://img.shields.io/github/languages/count/Knuckles-Team/genius-chatbot)
 ![GitHub repo size](https://img.shields.io/github/repo-size/Knuckles-Team/genius-chatbot)
 ![GitHub repo file count (file type)](https://img.shields.io/github/directory-file-count/Knuckles-Team/genius-chatbot)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/genius-chatbot)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/genius-chatbot)
 
-*Version: 1.7.0*
+*Version: 1.8.0*
 
 Chatbot that uses any hugging face model or OpenAI endpoint. 
 
 Local vector store supported with ChromaDB, or connect to a PGVector database
 
 Allows for scalable intelligence tailored for hardware limitations
```

## Comparing `genius_chatbot-1.7.0.dist-info/RECORD` & `genius_chatbot-1.8.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 genius_chatbot/__init__.py,sha256=O7ooBgWBS78QTZQbc5cxfQuQcZDrsKKBGuhrUv_sUPU,352
 genius_chatbot/genius_chatbot.py,sha256=2S6ItbRrvDeXt7xykc_cG3feQdVsgwJDTOtWUtO3zLU,23871
-genius_chatbot/version.py,sha256=f6IdlelHR19-XKmAZdInKmHo9riDxNIRsXMFYIydxbU,116
-genius_chatbot-1.7.0.dist-info/LICENSE,sha256=wtI1_YjppxJA2UTLHLbj_goBi-f3DebTfIFbe_XqJmY,1059
-genius_chatbot-1.7.0.dist-info/METADATA,sha256=JwypAI-KoTWb96HcUg6k7_QI_Vb7Bg_dnpTAmOkvEBw,7503
-genius_chatbot-1.7.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-genius_chatbot-1.7.0.dist-info/entry_points.txt,sha256=asyPpl1aicuFo099ocwKb7JL7wpedAluDYXKU1XV4XA,71
-genius_chatbot-1.7.0.dist-info/top_level.txt,sha256=uWSPUAqHcTpwWn3twHwOq2syGyPX6ksCZkz97j0_hZI,15
-genius_chatbot-1.7.0.dist-info/RECORD,,
+genius_chatbot/version.py,sha256=NHUQMTFjlz_tgehwhywIj5hbFsSAN98oa7Z_bgtC9ug,116
+genius_chatbot-1.8.0.dist-info/LICENSE,sha256=wtI1_YjppxJA2UTLHLbj_goBi-f3DebTfIFbe_XqJmY,1059
+genius_chatbot-1.8.0.dist-info/METADATA,sha256=V5SKBRM3cUz057WqX6bF60vEyxgIlvuQJ3TFCH6s3Ko,7554
+genius_chatbot-1.8.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+genius_chatbot-1.8.0.dist-info/entry_points.txt,sha256=asyPpl1aicuFo099ocwKb7JL7wpedAluDYXKU1XV4XA,71
+genius_chatbot-1.8.0.dist-info/top_level.txt,sha256=uWSPUAqHcTpwWn3twHwOq2syGyPX6ksCZkz97j0_hZI,15
+genius_chatbot-1.8.0.dist-info/RECORD,,
```

