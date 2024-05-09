# Comparing `tmp/media_downloader-0.8.0-py2.py3-none-any.whl.zip` & `tmp/media_downloader-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6552 bytes, number of entries: 9
+Zip file size: 6560 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      348 b- defN 23-Apr-16 04:38 media_downloader/__init__.py
 -rw-r--r--  2.0 unx     9232 b- defN 23-Apr-23 19:27 media_downloader/media_downloader.py
--rw-r--r--  2.0 unx      116 b- defN 23-Oct-15 15:14 media_downloader/version.py
--rw-r--r--  2.0 unx     1059 b- defN 23-Oct-15 15:14 media_downloader-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3937 b- defN 23-Oct-15 15:14 media_downloader-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Oct-15 15:14 media_downloader-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       77 b- defN 23-Oct-15 15:14 media_downloader-0.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Oct-15 15:14 media_downloader-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      796 b- defN 23-Oct-15 15:14 media_downloader-0.8.0.dist-info/RECORD
-9 files, 15692 bytes uncompressed, 5158 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx      116 b- defN 23-Oct-28 03:20 media_downloader/version.py
+-rw-r--r--  2.0 unx     1059 b- defN 23-Oct-28 03:20 media_downloader-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3988 b- defN 23-Oct-28 03:20 media_downloader-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Oct-28 03:20 media_downloader-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       77 b- defN 23-Oct-28 03:20 media_downloader-0.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Oct-28 03:20 media_downloader-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      796 b- defN 23-Oct-28 03:20 media_downloader-0.9.0.dist-info/RECORD
+9 files, 15743 bytes uncompressed, 5166 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: media_downloader/media_downloader.py
 Comment: 
 
 Filename: media_downloader/version.py
 Comment: 
 
-Filename: media_downloader-0.8.0.dist-info/LICENSE
+Filename: media_downloader-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: media_downloader-0.8.0.dist-info/METADATA
+Filename: media_downloader-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: media_downloader-0.8.0.dist-info/WHEEL
+Filename: media_downloader-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: media_downloader-0.8.0.dist-info/entry_points.txt
+Filename: media_downloader-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: media_downloader-0.8.0.dist-info/top_level.txt
+Filename: media_downloader-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: media_downloader-0.8.0.dist-info/RECORD
+Filename: media_downloader-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## media_downloader/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `media_downloader-0.8.0.dist-info/LICENSE` & `media_downloader-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `media_downloader-0.8.0.dist-info/METADATA` & `media_downloader-0.9.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: media-downloader
-Version: 0.8.0
+Version: 0.9.0
 Summary: Download audio/videos from the internet!
 Home-page: https://github.com/Knuckles-Team/media-downloader
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
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
 Requires-Dist: requests (>=2.28.1)
 Requires-Dist: yt-dlp (>=2023.3.4)
 
 # Media Downloader
 
@@ -38,15 +39,15 @@
 ![GitHub top language](https://img.shields.io/github/languages/top/Knuckles-Team/media-downloader)
 ![GitHub language count](https://img.shields.io/github/languages/count/Knuckles-Team/media-downloader)
 ![GitHub repo size](https://img.shields.io/github/repo-size/Knuckles-Team/media-downloader)
 ![GitHub repo file count (file type)](https://img.shields.io/github/directory-file-count/Knuckles-Team/media-downloader)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/media-downloader)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/media-downloader)
 
-*Version: 0.8.0*
+*Version: 0.9.0*
 
 Download videos and audio from the internet!
 
 This repository is actively maintained - Contributions are welcome!
 
 ### Supports:
 - YouTube
```

