# Comparing `tmp/automvs-0.0.9.tar.gz` & `tmp/automvs-0.0.9.post1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automvs-0.0.9.tar", last modified: Thu May  9 18:41:28 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

