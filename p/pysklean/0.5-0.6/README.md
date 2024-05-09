# Comparing `tmp/pysklean-0.5.tar.gz` & `tmp/pysklean-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysklean-0.5.tar", last modified: Thu May  2 16:21:19 2024, max compression
+gzip compressed data, was "pysklean-0.6.tar", last modified: Thu May  9 13:26:56 2024, max compression
```

## Comparing `pysklean-0.5.tar` & `pysklean-0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 16:21:19.539848 pysklean-0.5/
--rw-rw-rw-   0        0        0      113 2024-05-02 16:21:19.525075 pysklean-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 16:21:19.419758 pysklean-0.5/pysklean/
--rw-rw-rw-   0        0        0       42 2024-05-02 16:19:33.000000 pysklean-0.5/pysklean/__init__.py
--rw-rw-rw-   0        0        0    59692 2024-05-02 16:19:22.000000 pysklean-0.5/pysklean/main.py
-drwxrwxrwx   0        0        0        0 2024-05-02 16:21:19.521073 pysklean-0.5/pysklean.egg-info/
--rw-rw-rw-   0        0        0      113 2024-05-02 16:21:18.000000 pysklean-0.5/pysklean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2024-05-02 16:21:19.000000 pysklean-0.5/pysklean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 16:21:18.000000 pysklean-0.5/pysklean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 16:21:18.000000 pysklean-0.5/pysklean.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 16:21:19.540849 pysklean-0.5/setup.cfg
--rw-rw-rw-   0        0        0      225 2024-05-02 16:19:39.000000 pysklean-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:26:56.806532 pysklean-0.6/
+-rw-rw-rw-   0        0        0      113 2024-05-09 13:26:56.803517 pysklean-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 13:26:56.771355 pysklean-0.6/pysklean/
+-rw-rw-rw-   0        0        0       30 2024-05-09 13:25:42.000000 pysklean-0.6/pysklean/__init__.py
+-rw-rw-rw-   0        0        0    15926 2024-05-09 13:25:25.000000 pysklean-0.6/pysklean/main.py
+drwxrwxrwx   0        0        0        0 2024-05-09 13:26:56.796495 pysklean-0.6/pysklean.egg-info/
+-rw-rw-rw-   0        0        0      113 2024-05-09 13:26:56.000000 pysklean-0.6/pysklean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2024-05-09 13:26:56.000000 pysklean-0.6/pysklean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 13:26:56.000000 pysklean-0.6/pysklean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 13:26:56.000000 pysklean-0.6/pysklean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 13:26:56.807514 pysklean-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      225 2024-05-09 13:25:49.000000 pysklean-0.6/setup.py
```

