# Comparing `tmp/lyyre-2.8.tar.gz` & `tmp/lyyre-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyyre-2.8.tar", last modified: Wed May  8 23:25:28 2024, max compression
+gzip compressed data, was "lyyre-2.9.tar", last modified: Wed May  8 23:37:07 2024, max compression
```

## Comparing `lyyre-2.8.tar` & `lyyre-2.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 23:25:28.915859 lyyre-2.8/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyre-2.8/LICENSE
--rw-rw-rw-   0        0        0      156 2024-05-08 23:25:28.914840 lyyre-2.8/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyre-2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 23:25:28.912826 lyyre-2.8/lyyre.egg-info/
--rw-rw-rw-   0        0        0      156 2024-05-08 23:25:28.000000 lyyre-2.8/lyyre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-05-08 23:25:28.000000 lyyre-2.8/lyyre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 23:25:28.000000 lyyre-2.8/lyyre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        3 2024-05-08 23:25:28.000000 lyyre-2.8/lyyre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-08 23:25:28.000000 lyyre-2.8/lyyre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9789 2024-05-08 14:09:51.000000 lyyre-2.8/lyyre.py
--rw-rw-rw-   0        0        0       42 2024-05-08 23:25:28.915859 lyyre-2.8/setup.cfg
--rw-rw-rw-   0        0        0      262 2024-05-08 23:25:27.000000 lyyre-2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-08 23:37:07.618140 lyyre-2.9/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyre-2.9/LICENSE
+-rw-rw-rw-   0        0        0      156 2024-05-08 23:37:07.618140 lyyre-2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyre-2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-08 23:37:07.617123 lyyre-2.9/lyyre.egg-info/
+-rw-rw-rw-   0        0        0      156 2024-05-08 23:37:07.000000 lyyre-2.9/lyyre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      151 2024-05-08 23:37:07.000000 lyyre-2.9/lyyre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-08 23:37:07.000000 lyyre-2.9/lyyre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-08 23:37:07.000000 lyyre-2.9/lyyre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3862 2024-05-08 23:35:36.000000 lyyre-2.9/lyyre.py
+-rw-rw-rw-   0        0        0       42 2024-05-08 23:37:07.619142 lyyre-2.9/setup.cfg
+-rw-rw-rw-   0        0        0      258 2024-05-08 23:37:06.000000 lyyre-2.9/setup.py
```

### Comparing `lyyre-2.8/LICENSE` & `lyyre-2.9/LICENSE`

 * *Files identical despite different names*

