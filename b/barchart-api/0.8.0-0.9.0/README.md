# Comparing `tmp/barchart_api-0.8.0-py2.py3-none-any.whl.zip` & `tmp/barchart_api-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5923 bytes, number of entries: 10
+Zip file size: 6236 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      284 b- defN 23-Mar-16 07:15 barchart_api/__init__.py
 -rw-r--r--  2.0 unx     7790 b- defN 23-Sep-26 02:19 barchart_api/barchart_api.py
 -rw-r--r--  2.0 unx      519 b- defN 23-Mar-16 07:18 barchart_api/decorators.py
 -rw-r--r--  2.0 unx      463 b- defN 23-Mar-16 07:15 barchart_api/exceptions.py
--rw-r--r--  2.0 unx      116 b- defN 23-Sep-26 02:19 barchart_api/version.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Sep-26 02:19 barchart_api-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1803 b- defN 23-Sep-26 02:19 barchart_api-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Sep-26 02:19 barchart_api-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Sep-26 02:19 barchart_api-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      820 b- defN 23-Sep-26 02:19 barchart_api-0.8.0.dist-info/RECORD
-10 files, 12988 bytes uncompressed, 4519 bytes compressed:  65.2%
+-rw-r--r--  2.0 unx      116 b- defN 23-Oct-15 13:54 barchart_api/version.py
+-rw-r--r--  2.0 unx     1059 b- defN 23-Oct-15 13:55 barchart_api-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3427 b- defN 23-Oct-15 13:55 barchart_api-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Oct-15 13:55 barchart_api-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-Oct-15 13:55 barchart_api-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      820 b- defN 23-Oct-15 13:55 barchart_api-0.9.0.dist-info/RECORD
+10 files, 14601 bytes uncompressed, 4832 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: barchart_api/exceptions.py
 Comment: 
 
 Filename: barchart_api/version.py
 Comment: 
 
-Filename: barchart_api-0.8.0.dist-info/LICENSE
+Filename: barchart_api-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: barchart_api-0.8.0.dist-info/METADATA
+Filename: barchart_api-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: barchart_api-0.8.0.dist-info/WHEEL
+Filename: barchart_api-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: barchart_api-0.8.0.dist-info/top_level.txt
+Filename: barchart_api-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: barchart_api-0.8.0.dist-info/RECORD
+Filename: barchart_api-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## barchart_api/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

