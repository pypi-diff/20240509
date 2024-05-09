# Comparing `tmp/flytekitplugins_mmcloud-1.12.0b7.tar.gz` & `tmp/flytekitplugins_mmcloud-1.12.1b0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_mmcloud-1.12.0b7.tar", last modified: Fri Apr 26 22:22:42 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
