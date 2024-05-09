# Comparing `tmp/gamsapi-46.4.1.tar.gz` & `tmp/gamsapi-46.5.0-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamsapi-46.4.1.tar", last modified: Tue Apr 16 07:47:49 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

