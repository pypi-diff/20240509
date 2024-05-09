# Comparing `tmp/zoy-0.1.1.tar.gz` & `tmp/zoy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoy-0.1.1.tar", max compression
+gzip compressed data, was "zoy-0.2.0.tar", max compression
```

## Comparing `zoy-0.1.1.tar` & `zoy-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      436 2024-05-09 10:05:58.048076 zoy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      434 2024-05-09 10:02:40.346058 zoy-0.1.1/README.md
--rw-r--r--   0        0        0       45 2024-05-09 10:06:03.983135 zoy-0.1.1/zoy/__init__.py
--rw-r--r--   0        0        0       65 2024-05-09 10:04:09.316799 zoy-0.1.1/zoy/__main__.py
--rw-r--r--   0        0        0     1561 2024-05-09 10:03:53.543148 zoy-0.1.1/zoy/zoy.py
--rw-r--r--   0        0        0      895 1970-01-01 00:00:00.000000 zoy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      583 2024-05-09 13:04:09.462837 zoy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      250 2024-05-09 13:01:42.394456 zoy-0.2.0/README.md
+-rw-r--r--   0        0        0       45 2024-05-09 13:04:02.488917 zoy-0.2.0/zoy/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-09 10:43:08.836724 zoy-0.2.0/zoy/__main__.py
+-rw-r--r--   0        0        0     3840 2024-05-09 13:02:23.309789 zoy-0.2.0/zoy/zoy.py
+-rw-r--r--   0        0        0      834 1970-01-01 00:00:00.000000 zoy-0.2.0/PKG-INFO
```

