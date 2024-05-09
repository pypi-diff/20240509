# Comparing `tmp/anabih_python_test-2.0.0.tar.gz` & `tmp/anabih_python_test-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anabih_python_test-2.0.0.tar", last modified: Thu May  9 02:37:39 2024, max compression
+gzip compressed data, was "anabih_python_test-3.0.0.tar", last modified: Thu May  9 02:42:23 2024, max compression
```

## Comparing `anabih_python_test-2.0.0.tar` & `anabih_python_test-3.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 02:37:39.696946 anabih_python_test-2.0.0/
--rw-rw-rw-   0        0        0      431 2024-05-09 02:37:39.695946 anabih_python_test-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       19 2024-05-09 00:01:05.000000 anabih_python_test-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 02:37:39.694993 anabih_python_test-2.0.0/anabih_python_test.egg-info/
--rw-rw-rw-   0        0        0      431 2024-05-09 02:37:39.000000 anabih_python_test-2.0.0/anabih_python_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2024-05-09 02:37:39.000000 anabih_python_test-2.0.0/anabih_python_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 02:37:39.000000 anabih_python_test-2.0.0/anabih_python_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 02:37:39.000000 anabih_python_test-2.0.0/anabih_python_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 02:37:39.696946 anabih_python_test-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      657 2024-05-09 02:36:16.000000 anabih_python_test-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 02:42:23.389889 anabih_python_test-3.0.0/
+-rw-rw-rw-   0        0        0      431 2024-05-09 02:42:23.388893 anabih_python_test-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2024-05-09 00:01:05.000000 anabih_python_test-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-09 02:42:23.387879 anabih_python_test-3.0.0/anabih_python_test.egg-info/
+-rw-rw-rw-   0        0        0      431 2024-05-09 02:42:23.000000 anabih_python_test-3.0.0/anabih_python_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2024-05-09 02:42:23.000000 anabih_python_test-3.0.0/anabih_python_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 02:42:23.000000 anabih_python_test-3.0.0/anabih_python_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 02:42:23.000000 anabih_python_test-3.0.0/anabih_python_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 02:42:23.389889 anabih_python_test-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      657 2024-05-09 02:42:20.000000 anabih_python_test-3.0.0/setup.py
```

