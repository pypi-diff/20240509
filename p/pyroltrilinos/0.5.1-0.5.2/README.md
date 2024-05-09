# Comparing `tmp/pyroltrilinos-0.5.1.tar.gz` & `tmp/pyroltrilinos-0.5.2-cp310-cp310-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroltrilinos-0.5.1.tar", last modified: Thu May  2 22:40:00 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

