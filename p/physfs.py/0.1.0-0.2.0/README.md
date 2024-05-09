# Comparing `tmp/physfs.py-0.1.0.tar.gz` & `tmp/physfs.py-0.2.0-cp312-cp312-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physfs.py-0.1.0.tar", last modified: Sat Mar 23 07:45:25 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

