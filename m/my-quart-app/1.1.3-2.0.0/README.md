# Comparing `tmp/my_quart_app-1.1.3.tar.gz` & `tmp/my_quart_app-2.0.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_quart_app-1.1.3.tar", last modified: Thu Apr 25 12:21:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

