# Comparing `tmp/keyauth_py-1.3.tar.gz` & `tmp/keyauth_py-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyauth_py-1.3.tar", last modified: Thu May  9 17:51:27 2024, max compression
+gzip compressed data, was "keyauth_py-1.4.tar", last modified: Thu May  9 17:52:54 2024, max compression
```

## Comparing `keyauth_py-1.3.tar` & `keyauth_py-1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 17:51:27.861167 keyauth_py-1.3/
--rw-rw-rw-   0        0        0      210 2024-05-09 17:51:27.860167 keyauth_py-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 17:51:27.840180 keyauth_py-1.3/keyauth-py/
--rw-rw-rw-   0        0        0       21 2024-05-09 17:27:36.000000 keyauth_py-1.3/keyauth-py/__init__.py
--rw-rw-rw-   0        0        0      307 2024-05-09 17:30:48.000000 keyauth_py-1.3/keyauth-py/keyauth.py
-drwxrwxrwx   0        0        0        0 2024-05-09 17:51:27.858169 keyauth_py-1.3/keyauth_py.egg-info/
--rw-rw-rw-   0        0        0      210 2024-05-09 17:51:27.000000 keyauth_py-1.3/keyauth_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-05-09 17:51:27.000000 keyauth_py-1.3/keyauth_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 17:51:27.000000 keyauth_py-1.3/keyauth_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-09 17:51:27.000000 keyauth_py-1.3/keyauth_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-09 17:51:27.000000 keyauth_py-1.3/keyauth_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 17:51:27.864166 keyauth_py-1.3/setup.cfg
--rw-rw-rw-   0        0        0      321 2024-05-09 17:51:20.000000 keyauth_py-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:52:54.895999 keyauth_py-1.4/
+-rw-rw-rw-   0        0        0      210 2024-05-09 17:52:54.894999 keyauth_py-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-09 17:52:54.873013 keyauth_py-1.4/keyauth-py/
+-rw-rw-rw-   0        0        0       27 2024-05-09 17:52:44.000000 keyauth_py-1.4/keyauth-py/__init__.py
+-rw-rw-rw-   0        0        0      307 2024-05-09 17:30:48.000000 keyauth_py-1.4/keyauth-py/keyauth.py
+drwxrwxrwx   0        0        0        0 2024-05-09 17:52:54.892001 keyauth_py-1.4/keyauth_py.egg-info/
+-rw-rw-rw-   0        0        0      210 2024-05-09 17:52:54.000000 keyauth_py-1.4/keyauth_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-05-09 17:52:54.000000 keyauth_py-1.4/keyauth_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 17:52:54.000000 keyauth_py-1.4/keyauth_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-09 17:52:54.000000 keyauth_py-1.4/keyauth_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-09 17:52:54.000000 keyauth_py-1.4/keyauth_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-09 17:52:54.897997 keyauth_py-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      321 2024-05-09 17:52:47.000000 keyauth_py-1.4/setup.py
```

