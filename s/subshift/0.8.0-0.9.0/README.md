# Comparing `tmp/subshift-0.8.0-py2.py3-none-any.whl.zip` & `tmp/subshift-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5371 bytes, number of entries: 9
+Zip file size: 5377 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      295 b- defN 23-Oct-15 15:20 subshift/__init__.py
 -rw-r--r--  2.0 unx     5030 b- defN 23-Oct-15 15:20 subshift/subshift.py
--rw-r--r--  2.0 unx      116 b- defN 23-Oct-15 15:20 subshift/version.py
--rw-r--r--  2.0 unx     1059 b- defN 23-Oct-15 15:20 subshift-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3327 b- defN 23-Oct-15 15:20 subshift-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Oct-15 15:20 subshift-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 23-Oct-15 15:20 subshift-0.8.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Oct-15 15:20 subshift-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      715 b- defN 23-Oct-15 15:20 subshift-0.8.0.dist-info/RECORD
-9 files, 10714 bytes uncompressed, 4137 bytes compressed:  61.4%
+-rw-r--r--  2.0 unx      116 b- defN 23-Oct-28 03:26 subshift/version.py
+-rw-r--r--  2.0 unx     1059 b- defN 23-Oct-28 03:26 subshift-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3378 b- defN 23-Oct-28 03:26 subshift-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Oct-28 03:26 subshift-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 23-Oct-28 03:26 subshift-0.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Oct-28 03:26 subshift-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      715 b- defN 23-Oct-28 03:26 subshift-0.9.0.dist-info/RECORD
+9 files, 10765 bytes uncompressed, 4143 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: subshift/subshift.py
 Comment: 
 
 Filename: subshift/version.py
 Comment: 
 
-Filename: subshift-0.8.0.dist-info/LICENSE
+Filename: subshift-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: subshift-0.8.0.dist-info/METADATA
+Filename: subshift-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: subshift-0.8.0.dist-info/WHEEL
+Filename: subshift-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: subshift-0.8.0.dist-info/entry_points.txt
+Filename: subshift-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: subshift-0.8.0.dist-info/top_level.txt
+Filename: subshift-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: subshift-0.8.0.dist-info/RECORD
+Filename: subshift-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## subshift/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `subshift-0.8.0.dist-info/LICENSE` & `subshift-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `subshift-0.8.0.dist-info/METADATA` & `subshift-0.9.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: subshift
-Version: 0.8.0
+Version: 0.9.0
 Summary: Synchronize your subtitle files by shifting the subtitle time (+/-)
 Home-page: https://github.com/Knuckles-Team/subsync
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
 Requires-Dist: chardet (>=5.1.0)
 
 # Subshift
 
 ![PyPI - Version](https://img.shields.io/pypi/v/subshift)
@@ -37,15 +38,15 @@
 ![GitHub top language](https://img.shields.io/github/languages/top/Knuckles-Team/subshift)
 ![GitHub language count](https://img.shields.io/github/languages/count/Knuckles-Team/subshift)
 ![GitHub repo size](https://img.shields.io/github/repo-size/Knuckles-Team/subshift)
 ![GitHub repo file count (file type)](https://img.shields.io/github/directory-file-count/Knuckles-Team/subshift)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/subshift)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/subshift)
 
-*Version: 0.8.0*
+*Version: 0.9.0*
 
 A handy Python library to shift your subtitles +/- seconds so they align with your video
 
 This repository is actively maintained - Contributions are welcome!
 
 <details>
   <summary><b>Usage:</b></summary>
```

## Comparing `subshift-0.8.0.dist-info/RECORD` & `subshift-0.9.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 subshift/__init__.py,sha256=MBfaXzCBXzYGszrpFBaytIz-0p1thRA3esVGPlR1ehw,295
 subshift/subshift.py,sha256=z4PrR3HrOLT6NSdUiLTxlpQiejGXP-7BAwMbLUnAy0A,5030
-subshift/version.py,sha256=tDDkCMChiJvcYngqfjlW_EaRz0JpbXA3z7tYvqWYe8M,116
-subshift-0.8.0.dist-info/LICENSE,sha256=wtI1_YjppxJA2UTLHLbj_goBi-f3DebTfIFbe_XqJmY,1059
-subshift-0.8.0.dist-info/METADATA,sha256=dCb4mGd74YNDAZVlwllJ1-SKMZI8QJi-_rJ3vE1rS8o,3327
-subshift-0.8.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-subshift-0.8.0.dist-info/entry_points.txt,sha256=ho9GadTXRy9aOTvMooBwTsnHMBp2la3Si4Wf9VxEcDI,53
-subshift-0.8.0.dist-info/top_level.txt,sha256=PxxKSAnw6GSMcX-AQjMQgfcVnbKBInwuiUHt1lNbUCk,9
-subshift-0.8.0.dist-info/RECORD,,
+subshift/version.py,sha256=swhRnSKFIqDu9_CTMLtKcx393Adi5vpxEYYazFr8kkE,116
+subshift-0.9.0.dist-info/LICENSE,sha256=wtI1_YjppxJA2UTLHLbj_goBi-f3DebTfIFbe_XqJmY,1059
+subshift-0.9.0.dist-info/METADATA,sha256=QXos7Ur4XGHfjrXGWeUwdCNckIwHIaUQyR6Of_vIEiE,3378
+subshift-0.9.0.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+subshift-0.9.0.dist-info/entry_points.txt,sha256=ho9GadTXRy9aOTvMooBwTsnHMBp2la3Si4Wf9VxEcDI,53
+subshift-0.9.0.dist-info/top_level.txt,sha256=PxxKSAnw6GSMcX-AQjMQgfcVnbKBInwuiUHt1lNbUCk,9
+subshift-0.9.0.dist-info/RECORD,,
```

