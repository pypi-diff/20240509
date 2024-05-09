# Comparing `tmp/cugdt-1.0.3.tar.gz` & `tmp/cugdt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cugdt-1.0.3.tar", last modified: Thu May  9 11:13:06 2024, max compression
+gzip compressed data, was "dist\cugdt-1.0.4.tar", last modified: Thu May  9 11:20:24 2024, max compression
```

## Comparing `cugdt-1.0.3.tar` & `cugdt-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 11:13:06.701720 cugdt-1.0.3/
--rw-rw-rw-   0        0        0      281 2024-05-09 11:13:06.701720 cugdt-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-09 11:04:12.000000 cugdt-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 11:13:06.690421 cugdt-1.0.3/cugdt/
--rw-rw-rw-   0        0        0     2294 2024-05-09 10:53:12.000000 cugdt-1.0.3/cugdt/Tiff.py
--rw-rw-rw-   0        0        0        0 2024-05-09 07:05:34.000000 cugdt-1.0.3/cugdt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 11:13:06.700718 cugdt-1.0.3/cugdt.egg-info/
--rw-rw-rw-   0        0        0      281 2024-05-09 11:13:06.000000 cugdt-1.0.3/cugdt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2024-05-09 11:13:06.000000 cugdt-1.0.3/cugdt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 11:13:06.000000 cugdt-1.0.3/cugdt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-09 11:13:06.000000 cugdt-1.0.3/cugdt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 11:13:06.701720 cugdt-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      758 2024-05-09 11:12:59.000000 cugdt-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:20:24.343888 cugdt-1.0.4/
+-rw-rw-rw-   0        0        0      781 2024-05-09 11:20:24.343888 cugdt-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-09 11:04:12.000000 cugdt-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 11:20:24.341888 cugdt-1.0.4/cugdt/
+-rw-rw-rw-   0        0        0     2294 2024-05-09 10:53:12.000000 cugdt-1.0.4/cugdt/Tiff.py
+-rw-rw-rw-   0        0        0        0 2024-05-09 07:05:34.000000 cugdt-1.0.4/cugdt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 11:20:24.343888 cugdt-1.0.4/cugdt.egg-info/
+-rw-rw-rw-   0        0        0      781 2024-05-09 11:20:24.000000 cugdt-1.0.4/cugdt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2024-05-09 11:20:24.000000 cugdt-1.0.4/cugdt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 11:20:24.000000 cugdt-1.0.4/cugdt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-09 11:20:24.000000 cugdt-1.0.4/cugdt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 11:20:24.343888 cugdt-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2024-05-09 11:20:12.000000 cugdt-1.0.4/setup.py
```

### Comparing `cugdt-1.0.3/cugdt/Tiff.py` & `cugdt-1.0.4/cugdt/Tiff.py`

 * *Files identical despite different names*

