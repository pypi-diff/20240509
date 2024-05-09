# Comparing `tmp/AyiinXd-0.0.6.tar.gz` & `tmp/AyiinXd-0.0.9-cp39-cp39-manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AyiinXd-0.0.6.tar", last modified: Tue Nov  8 13:09:40 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

