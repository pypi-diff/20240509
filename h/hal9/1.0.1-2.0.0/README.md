# Comparing `tmp/hal9-1.0.1.tar.gz` & `tmp/hal9-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hal9-1.0.1.tar", max compression
+gzip compressed data, was "hal9-2.0.0.tar", max compression
```

## Comparing `hal9-1.0.1.tar` & `hal9-2.0.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1836 2023-03-08 19:18:50.683389 hal9-1.0.1/README.md
--rw-r--r--   0        0        0       23 2023-03-08 19:18:50.687389 hal9-1.0.1/hal9/__init__.py
--rw-r--r--   0        0        0     1127 2023-03-08 19:18:50.687389 hal9-1.0.1/hal9/core.py
--rw-r--r--   0        0        0      322 2023-03-08 19:18:50.687389 hal9-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2423 1970-01-01 00:00:00.000000 hal9-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      117 2024-05-08 22:33:23.124203 hal9-2.0.0/README.md
+-rw-r--r--   0        0        0       24 2024-05-08 22:33:23.124203 hal9-2.0.0/hal9/__init__.py
+-rw-r--r--   0        0        0      957 2024-05-08 22:33:23.124203 hal9-2.0.0/hal9/core.py
+-rw-r--r--   0        0        0      304 2024-05-08 22:33:23.124203 hal9-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 hal9-2.0.0/PKG-INFO
```

