# Comparing `tmp/gdmath-1.5.3.tar.gz` & `tmp/gdmath-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmath-1.5.3.tar", last modified: Mon Apr  8 10:48:55 2024, max compression
+gzip compressed data, was "gdmath-1.5.4.tar", last modified: Thu May  9 03:15:58 2024, max compression
```

## Comparing `gdmath-1.5.3.tar` & `gdmath-1.5.4.tar`

### file list

```diff
@@ -1,19 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 10:48:55.445239 gdmath-1.5.3/
--rw-rw-rw-   0        0        0     1091 2024-04-08 10:48:36.000000 gdmath-1.5.3/LICENSE.txt
--rw-rw-rw-   0        0        0      180 2024-04-08 10:48:36.000000 gdmath-1.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4669 2024-04-08 10:48:55.445239 gdmath-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     2250 2024-04-08 10:48:36.000000 gdmath-1.5.3/README.md
--rw-rw-rw-   0        0        0     1437 2024-04-08 10:48:36.000000 gdmath-1.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 10:48:55.445239 gdmath-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      503 2024-04-08 10:48:36.000000 gdmath-1.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 10:48:55.445239 gdmath-1.5.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 10:48:55.445239 gdmath-1.5.3/src/gdmath/
--rw-rw-rw-   0        0        0      225 2024-04-08 10:48:36.000000 gdmath-1.5.3/src/gdmath/__init__.py
--rw-rw-rw-   0        0        0      225 2024-04-08 10:48:36.000000 gdmath-1.5.3/src/gdmath/__init__.pyi
--rw-rw-rw-   0        0        0  1108332 2024-04-08 10:48:36.000000 gdmath-1.5.3/src/gdmath/_gdmath.pyi
--rw-rw-rw-   0        0        0  1955852 2024-04-08 10:48:36.000000 gdmath-1.5.3/src/gdmath/_gdmath.pyx
-drwxrwxrwx   0        0        0        0 2024-04-08 10:48:55.445239 gdmath-1.5.3/src/gdmath.egg-info/
--rw-rw-rw-   0        0        0     4669 2024-04-08 10:48:55.000000 gdmath-1.5.3/src/gdmath.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-04-08 10:48:55.000000 gdmath-1.5.3/src/gdmath.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 10:48:55.000000 gdmath-1.5.3/src/gdmath.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-08 10:48:55.000000 gdmath-1.5.3/src/gdmath.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-09 03:15:58.771101 gdmath-1.5.4/
+-rw-rw-rw-   0        0        0     7652 2024-05-07 04:56:52.000000 gdmath-1.5.4/LICENSE.txt
+-rw-rw-rw-   0        0        0    11135 2024-05-09 03:15:58.770100 gdmath-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0      137 2024-05-09 03:15:21.000000 gdmath-1.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 03:15:58.749006 gdmath-1.5.4/gdmath/
+-rw-rw-rw-   0        0        0      363 2024-05-09 03:15:52.000000 gdmath-1.5.4/gdmath/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-09 03:15:58.769100 gdmath-1.5.4/gdmath.egg-info/
+-rw-rw-rw-   0        0        0    11135 2024-05-09 03:15:58.000000 gdmath-1.5.4/gdmath.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2024-05-09 03:15:58.000000 gdmath-1.5.4/gdmath.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 03:15:58.000000 gdmath-1.5.4/gdmath.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-09 03:15:58.000000 gdmath-1.5.4/gdmath.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-09 03:15:58.000000 gdmath-1.5.4/gdmath.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1911 2024-05-09 03:12:57.000000 gdmath-1.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-09 03:15:58.771101 gdmath-1.5.4/setup.cfg
```

