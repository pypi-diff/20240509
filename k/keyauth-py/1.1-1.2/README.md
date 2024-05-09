# Comparing `tmp/keyauth_py-1.1.tar.gz` & `tmp/keyauth_py-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyauth_py-1.1.tar", last modified: Thu May  9 17:01:33 2024, max compression
+gzip compressed data, was "keyauth_py-1.2.tar", last modified: Thu May  9 17:28:04 2024, max compression
```

## Comparing `keyauth_py-1.1.tar` & `keyauth_py-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 17:01:33.029651 keyauth_py-1.1/
--rw-rw-rw-   0        0        0      210 2024-05-09 17:01:33.028652 keyauth_py-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 17:01:32.996670 keyauth_py-1.1/keyauth-py/
--rw-rw-rw-   0        0        0       25 2024-05-09 17:00:57.000000 keyauth_py-1.1/keyauth-py/__init__.py
--rw-rw-rw-   0        0        0      251 2024-05-09 16:48:58.000000 keyauth_py-1.1/keyauth-py/keyauth.py
-drwxrwxrwx   0        0        0        0 2024-05-09 17:01:33.026652 keyauth_py-1.1/keyauth_py.egg-info/
--rw-rw-rw-   0        0        0      210 2024-05-09 17:01:32.000000 keyauth_py-1.1/keyauth_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-05-09 17:01:32.000000 keyauth_py-1.1/keyauth_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 17:01:32.000000 keyauth_py-1.1/keyauth_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 17:01:32.000000 keyauth_py-1.1/keyauth_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 17:01:32.000000 keyauth_py-1.1/keyauth_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 17:01:33.033648 keyauth_py-1.1/setup.cfg
--rw-rw-rw-   0        0        0      321 2024-05-09 17:01:16.000000 keyauth_py-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:28:04.854658 keyauth_py-1.2/
+-rw-rw-rw-   0        0        0      210 2024-05-09 17:28:04.853656 keyauth_py-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 17:28:04.823675 keyauth_py-1.2/keyauth-py/
+-rw-rw-rw-   0        0        0       21 2024-05-09 17:27:36.000000 keyauth_py-1.2/keyauth-py/__init__.py
+-rw-rw-rw-   0        0        0      251 2024-05-09 16:48:58.000000 keyauth_py-1.2/keyauth-py/keyauth.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:28:04.850660 keyauth_py-1.2/keyauth_py.egg-info/
+-rw-rw-rw-   0        0        0      210 2024-05-09 17:28:04.000000 keyauth_py-1.2/keyauth_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-05-09 17:28:04.000000 keyauth_py-1.2/keyauth_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 17:28:04.000000 keyauth_py-1.2/keyauth_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 17:28:04.000000 keyauth_py-1.2/keyauth_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 17:28:04.000000 keyauth_py-1.2/keyauth_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 17:28:04.857655 keyauth_py-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      321 2024-05-09 17:28:03.000000 keyauth_py-1.2/setup.py
```

