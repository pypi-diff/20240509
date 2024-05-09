# Comparing `tmp/easy_k8s-0.2.0.post2.tar.gz` & `tmp/easy_k8s-0.2.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Apr  8 03:51:24 2024, max compression
+gzip compressed data, last modified: Thu May  9 08:54:34 2024, max compression
```

## Comparing `easy_k8s-0.2.0.post2.tar` & `easy_k8s-0.2.0.post4.tar`

### file list

```diff
@@ -1,2 +1,2 @@
--rw-r--r--   0      501       20     1024 2024-03-29 01:53:45.000000 easy_k8s-0.2.0.post2/pyproject.toml
--rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 easy_k8s-0.2.0.post2/PKG-INFO
+-rw-r--r--   0      501       20     1024 2024-03-29 01:53:45.000000 easy_k8s-0.2.0.post4/pyproject.toml
+-rw-r--r--   0        0        0      943 1970-01-01 00:00:00.000000 easy_k8s-0.2.0.post4/PKG-INFO
```

### Comparing `easy_k8s-0.2.0.post2/pyproject.toml` & `easy_k8s-0.2.0.post4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `easy_k8s-0.2.0.post2/PKG-INFO` & `easy_k8s-0.2.0.post4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: easy-k8s
-Version: 0.2.0.post2
+Version: 0.2.0.post4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Free for non-commercial use
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
```

