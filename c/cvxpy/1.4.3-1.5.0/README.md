# Comparing `tmp/cvxpy-1.4.3.tar.gz` & `tmp/cvxpy-1.5.0-cp312-cp312-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxpy-1.4.3.tar", last modified: Tue Apr 16 08:08:50 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

