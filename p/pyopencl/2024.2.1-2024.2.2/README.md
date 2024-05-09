# Comparing `tmp/pyopencl-2024.2.1.tar.gz` & `tmp/pyopencl-2024.2.2-cp38-cp38-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyopencl-2024.2.1.tar", last modified: Tue May  7 14:22:45 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

