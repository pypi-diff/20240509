# Comparing `tmp/asynctnt-2.2.0.tar.gz` & `tmp/asynctnt-2.3.0-pp310-pypy310_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asynctnt-2.2.0.tar", last modified: Sun May  5 20:10:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

