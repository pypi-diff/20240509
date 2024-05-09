# Comparing `tmp/pylzss-0.3.7.tar.gz` & `tmp/pylzss-0.3.8-cp310-cp310-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylzss-0.3.7.tar", last modified: Wed Apr 17 04:11:15 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
