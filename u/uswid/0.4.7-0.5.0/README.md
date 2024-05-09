# Comparing `tmp/uswid-0.4.7.tar.gz` & `tmp/uswid-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uswid-0.4.7.tar", last modified: Sun Dec  3 10:59:30 2023, max compression
+gzip compressed data, was "uswid-0.5.0.tar", last modified: Thu May  9 09:42:57 2024, max compression
```

## Comparing `uswid-0.4.7.tar` & `uswid-0.5.0.tar`

### file list

```diff
@@ -1,56 +1,67 @@
-drwxr-xr-x   0 hughsie   (1000) hughsie   (1000)        0 2023-12-03 10:59:30.059852 uswid-0.4.7/
--rw-rw-r--   0 hughsie   (1000) hughsie   (1000)    26462 2021-10-12 08:38:57.000000 uswid-0.4.7/LICENSE
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      790 2023-12-03 10:59:30.059852 uswid-0.4.7/PKG-INFO
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)    10307 2023-11-10 10:46:04.000000 uswid-0.4.7/README.md
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)       38 2023-12-03 10:59:30.059852 uswid-0.4.7/setup.cfg
--rwxr-xr-x   0 hughsie   (1000) hughsie   (1000)     1975 2023-11-30 14:43:23.000000 uswid-0.4.7/setup.py
-drwxr-xr-x   0 hughsie   (1000) hughsie   (1000)        0 2023-12-03 10:59:30.057852 uswid-0.4.7/uswid/
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1080 2023-11-30 14:43:23.000000 uswid-0.4.7/uswid/__init__.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1384 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/__init__.pyi
--rwxr-xr-x   0 hughsie   (1000) hughsie   (1000)    16086 2023-11-30 14:43:23.000000 uswid-0.4.7/uswid/cli.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2981 2023-11-30 14:43:23.000000 uswid-0.4.7/uswid/container.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2546 2023-11-30 14:43:23.000000 uswid-0.4.7/uswid/entity.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      573 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/entity.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2171 2023-11-14 15:07:48.000000 uswid-0.4.7/uswid/enums.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1533 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/enums.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      258 2023-10-02 19:58:45.000000 uswid-0.4.7/uswid/errors.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)       50 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/errors.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1211 2023-11-30 14:43:23.000000 uswid-0.4.7/uswid/evidence.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      366 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/evidence.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      957 2023-10-03 10:58:18.000000 uswid-0.4.7/uswid/format.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      286 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/format.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)    15580 2023-10-15 15:08:42.000000 uswid-0.4.7/uswid/format_coswid.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      852 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/format_coswid.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     5157 2023-10-15 15:08:42.000000 uswid-0.4.7/uswid/format_cyclonedx.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      408 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/format_cyclonedx.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)    11574 2023-10-15 15:08:42.000000 uswid-0.4.7/uswid/format_goswid.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      734 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/format_goswid.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)    11352 2023-10-15 15:08:42.000000 uswid-0.4.7/uswid/format_ini.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      737 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/format_ini.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2524 2023-10-03 10:58:18.000000 uswid-0.4.7/uswid/format_pkgconfig.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     4327 2023-10-15 15:08:42.000000 uswid-0.4.7/uswid/format_spdx.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      403 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/format_spdx.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)    11715 2023-10-09 08:37:16.000000 uswid-0.4.7/uswid/format_swid.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      768 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/format_swid.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     5428 2023-11-10 10:46:04.000000 uswid-0.4.7/uswid/format_uswid.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      864 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/format_uswid.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2211 2023-11-06 15:58:07.000000 uswid-0.4.7/uswid/hash.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      525 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/hash.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)    11767 2023-11-30 14:43:23.000000 uswid-0.4.7/uswid/identity.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1714 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/identity.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2783 2023-11-30 14:43:23.000000 uswid-0.4.7/uswid/link.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      836 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/link.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2439 2023-11-30 14:43:23.000000 uswid-0.4.7/uswid/payload.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      622 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/payload.pyi
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      772 2023-11-30 14:43:23.000000 uswid-0.4.7/uswid/problem.py
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      202 2023-12-03 10:59:29.000000 uswid-0.4.7/uswid/problem.pyi
--rw-rw-r--   0 hughsie   (1000) hughsie   (1000)       64 2021-10-12 18:42:52.000000 uswid-0.4.7/uswid/py.typed
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)    13923 2023-11-06 15:58:07.000000 uswid-0.4.7/uswid/test_uswid.py
-drwxr-xr-x   0 hughsie   (1000) hughsie   (1000)        0 2023-12-03 10:59:30.058852 uswid-0.4.7/uswid.egg-info/
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)      790 2023-12-03 10:59:30.000000 uswid-0.4.7/uswid.egg-info/PKG-INFO
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1011 2023-12-03 10:59:30.000000 uswid-0.4.7/uswid.egg-info/SOURCES.txt
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)        1 2023-12-03 10:59:30.000000 uswid-0.4.7/uswid.egg-info/dependency_links.txt
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)       41 2023-12-03 10:59:30.000000 uswid-0.4.7/uswid.egg-info/entry_points.txt
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)        1 2023-01-07 14:29:56.000000 uswid-0.4.7/uswid.egg-info/not-zip-safe
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)       69 2023-12-03 10:59:30.000000 uswid-0.4.7/uswid.egg-info/requires.txt
--rw-r--r--   0 hughsie   (1000) hughsie   (1000)        6 2023-12-03 10:59:30.000000 uswid-0.4.7/uswid.egg-info/top_level.txt
+drwxr-xr-x   0 hughsie   (1000) hughsie   (1000)        0 2024-05-09 09:42:57.832042 uswid-0.5.0/
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2667 2024-02-21 14:35:30.000000 uswid-0.5.0/LICENSE
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      748 2024-05-09 09:42:57.832042 uswid-0.5.0/PKG-INFO
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)    12227 2024-05-02 14:44:28.000000 uswid-0.5.0/README.md
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)       38 2024-05-09 09:42:57.832042 uswid-0.5.0/setup.cfg
+-rwxr-xr-x   0 hughsie   (1000) hughsie   (1000)     2054 2024-05-02 14:08:40.000000 uswid-0.5.0/setup.py
+drwxr-xr-x   0 hughsie   (1000) hughsie   (1000)        0 2024-05-09 09:42:57.831042 uswid-0.5.0/uswid/
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1310 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/__init__.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1709 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/__init__.pyi
+-rwxr-xr-x   0 hughsie   (1000) hughsie   (1000)    16629 2024-05-09 09:42:36.000000 uswid-0.5.0/uswid/cli.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1188 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/cli.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)    13939 2024-05-02 14:44:28.000000 uswid-0.5.0/uswid/component.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2010 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/component.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     4682 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/container.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      824 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/container.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2881 2024-05-02 14:44:28.000000 uswid-0.5.0/uswid/entity.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      533 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/entity.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2352 2024-05-02 14:44:28.000000 uswid-0.5.0/uswid/enums.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1533 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/enums.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      258 2023-10-02 19:58:45.000000 uswid-0.5.0/uswid/errors.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)       50 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/errors.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1366 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/evidence.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      328 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/evidence.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      967 2024-02-21 14:35:30.000000 uswid-0.5.0/uswid/format.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      256 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/format.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)    16060 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/format_coswid.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      825 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/format_coswid.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     5123 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/format_cyclonedx.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      411 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/format_cyclonedx.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)    11537 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/format_goswid.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      707 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/format_goswid.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)    11364 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/format_ini.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      710 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/format_ini.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2553 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/format_pkgconfig.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      471 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/format_pkgconfig.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     4294 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/format_spdx.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      406 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/format_spdx.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)    11762 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/format_swid.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      741 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/format_swid.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     5441 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/format_uswid.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      839 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/format_uswid.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2303 2024-05-02 14:44:28.000000 uswid-0.5.0/uswid/hash.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      557 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/hash.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2985 2024-05-02 14:44:28.000000 uswid-0.5.0/uswid/link.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      924 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/link.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2590 2024-02-21 14:35:30.000000 uswid-0.5.0/uswid/payload.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      584 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/payload.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      783 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/problem.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      202 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/problem.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     2974 2024-02-21 14:35:30.000000 uswid-0.5.0/uswid/purl.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      321 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/purl.pyi
+-rw-rw-r--   0 hughsie   (1000) hughsie   (1000)       64 2021-10-12 18:42:52.000000 uswid-0.5.0/uswid/py.typed
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)    15509 2024-05-02 14:08:40.000000 uswid-0.5.0/uswid/test_uswid.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     3512 2024-02-21 14:35:30.000000 uswid-0.5.0/uswid/vex_document.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      580 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/vex_document.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1346 2024-02-21 14:35:30.000000 uswid-0.5.0/uswid/vex_product.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      252 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/vex_product.pyi
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     5130 2024-02-21 14:35:30.000000 uswid-0.5.0/uswid/vex_statement.py
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1099 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid/vex_statement.pyi
+drwxr-xr-x   0 hughsie   (1000) hughsie   (1000)        0 2024-05-09 09:42:57.832042 uswid-0.5.0/uswid.egg-info/
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)      748 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid.egg-info/PKG-INFO
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)     1238 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid.egg-info/SOURCES.txt
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)        1 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid.egg-info/dependency_links.txt
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)       41 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid.egg-info/entry_points.txt
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)        1 2024-05-09 09:26:08.000000 uswid-0.5.0/uswid.egg-info/not-zip-safe
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)       69 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid.egg-info/requires.txt
+-rw-r--r--   0 hughsie   (1000) hughsie   (1000)        6 2024-05-09 09:42:57.000000 uswid-0.5.0/uswid.egg-info/top_level.txt
```

### Comparing `uswid-0.4.7/PKG-INFO` & `uswid-0.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: uswid
-Version: 0.4.7
+Version: 0.5.0
 Summary: A pure-python library for embedding CoSWID data
 Home-page: https://github.com/hughsie/python-uswid
 Author: Richard Hughes
 Author-email: richard@hughsie.com
-License: LGPL-2.1-or-later
+License: BSD-2-Clause-Patent
 Keywords: swid,sbom,coswid
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Archiving
 License-File: LICENSE
 Requires-Dist: cbor2
 Requires-Dist: lxml
 Requires-Dist: pefile
```

### Comparing `uswid-0.4.7/README.md` & `uswid-0.5.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 - `pkgconfig` -- `.pc` files that are shipped with most open source libraries
 - [PE binaries](https://learn.microsoft.com/en-us/windows/win32/debug/pe-format) -- coSWID metadata can be inserted in a `.sbom` section at link time
 - unspecified firmware files -- using a 24 byte header to locate the coSWID CBOR SBoM entry
 
 There are three elements of an SBoM that uswid supports. These are:
 
 - Identities -- the *what*, describing the software subcomponents
-- Entities -- the *who*, describing the company or person responsible for the identity in some way
+- Entities -- the *who*, describing the company or person responsible for the component in some way
 - Payloads (optional) -- the *file* that we are referring to, for when the SBoM is not embedded
 - Evidence (optional) -- the *proof*, typically the date and time the SBoM was built
 
-One of the core features of uswid is that you can import multiple files to build a single identity at construction time.
+One of the core features of uswid is that you can import multiple files to build a single component at construction time.
 
 For instance, you could combine the pkgconfig `.pc` file, a `.exe` binary and `.ini` override to build one SBoM component. In most cases SBoM metadata is merged, but it can also be replaced.
 
 There is also a [web-generator on the LVFS](https://fwupd.org/lvfs/uswid) that uses uSWID to easily build INI, coSWID and coSWID with uSWID header.
 
 ![LVFS Web Generator](docs/lvfs-uswid.png)
 
@@ -150,15 +150,15 @@
 Dependancies like compilers or other security-relevant libraries can be added using:
 
     uswid --load uswid.ini compiler.ini --save ./example.uswid
 
 Where we have added an extra link section in `uswid.ini`:
 
     [uSWID-Link:gcc]
-    rel = see-also
+    rel = compiler
     href = swid:077b4576-92f7-52fd-94eb-af9fc3d52c58
 
 Where `compiler.ini` looks something like:
 
     [uSWID]
     tag-id = 077b4576-92f7-52fd-94eb-af9fc3d52c58
     software-name = gcc
@@ -214,14 +214,48 @@
 
 If `pefile` doesn't add the SWID metadata to the PE file correctly, you can use the alternate method of using `objcopy`, either available by default on Linux or installable using WSL on Windows. e.g.
 
     uswid --load sbom.ini --save ./payload.efi --objcopy /usr/bin/objcopy
 
 You can use `objdump -s -j .sbom payload.efi` to verify that the tag has been written correctly to the binary.
 
+# Generating Test Data
+
+The `uswid` CLI can generate a complete "worst case" platform SBoM, with 1000 plausible (but random) components. This is generates a ~140kB file, or ~60kB when compressed with LZMA.
+
+You can use the uswid command line to generate a plausible UEFI platform SBoM:
+
+    uswid --generate --save test.uswid --compression lzma
+
+Each generated component includes:
+
+ * A unique tag-id GUID
+ * A unique software-name of size 4-30 chars
+ * A colloquial-version from a random selection of 10 SHA-1 hashes
+ * An edition from a random SHA-1 hash
+ * A semantic version of size 3-8 chars
+ * An entity from a random selection of 10 entities
+
+# VEX
+
+The `uswid` binary can load VEX data from [OpenVEX](https://github.com/openvex) and [CSAF-2.0](https://docs.oasis-open.org/csaf/csaf/v2.0/csaf-v2.0.html) files, and will generate a report for the end-user.
+
+For example:
+
+    uswid --load examples/intel-ucode.ini examples/intel-ucode.vex --verbose
+    Loaded:
+    uSwidComponent(tag_id="bcbd84ff-9898-4922-8ade-dd4bbe2e40ba",tag_version="0",software_name="MCU 06-03-02",software_version="20230808"):
+     - uSwidEntity(regid="com.intel",name="Intel Corporation",roles=TAG_CREATOR,SOFTWARE_CREATOR)
+     - uSwidPayload(name="intel-ucode-06-03-02",size=12)
+     - uSwidHash(alg_id=SHA256,value="a948904f2f0f479b8f8197694b30184b0d2ed1c1cd2a1ec0fb85d299a192a447")
+     - uSwidEvidence(date="2023-09-15 12:34:56",device_id=None)
+     - uSwidVexStatement(vulnerability_name="CVE-2022-40982",status="uSwidVexStatementStatus.NOT_AFFECTED",justification="uSwidVexStatementJustification.VULNERABLE_CODE_NOT_IN_EXECUTE_PATH",impact_statement="These processors do not use GDS and are not vulnerable to this CVE."):
+       - uSwidVexProduct(tag_ids="[uSwidPurl("pkg:swid/bcbd84ff-9898-4922-8ade-dd4bbe2e40ba")]"):
+         - uSwidHash(alg_id=SHA256,value="a948904f2f0f479b8f8197694b30184b0d2ed1c1cd2a1ec0fb85d299a192a447")
+
 # Installing
 
 This library and helper binary can be installed using `pip`:
 
     pip install --user uswid
 
 This will download any required dependancies and also install the `uswid` tool into your bindir.
```

### Comparing `uswid-0.4.7/setup.py` & `uswid-0.5.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # note: this is a repeat of the README, to evolve, good enough for now.
 long_desc = """
 Contributors welcome, either adding new functionality or fixing bugs.
 """
 
 setup(
     name="uswid",
-    version="0.4.7",
-    license="LGPL-2.1-or-later",
+    version="0.5.0",
+    license="BSD-2-Clause-Patent",
     license_files=[
         "LICENSE",
     ],
     description="A pure-python library for embedding CoSWID data",
     long_description=long_desc,
     author="Richard Hughes",
     author_email="richard@hughsie.com",
@@ -35,15 +35,15 @@
         ]
     },
     zip_safe=False,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
+        "License :: OSI Approved :: BSD License",
         "Programming Language :: Python :: 3",
         "Topic :: Utilities",
         "Topic :: System :: Archiving",
     ],
     keywords=["swid", "sbom", "coswid"],
     package_data={
         "uswid": [
@@ -57,16 +57,20 @@
             "format_ini.pyi",
             "format.pyi",
             "format_spdx.pyi",
             "format_swid.pyi",
             "format_uswid.pyi",
             "hash.pyi",
             "payload.pyi",
+            "purl.pyi",
             "evidence.pyi",
-            "identity.pyi",
+            "component.pyi",
             "link.pyi",
             "problem.pyi",
+            "vex_document.pyi",
+            "vex_product.pyi",
+            "vex_statement.pyi",
             "__init__.pyi",
         ]
     },
     setup_requires=["wheel"],
 )
```

### Comparing `uswid-0.4.7/uswid/__init__.py` & `uswid-0.5.0/uswid/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 
 from uswid.container import uSwidContainer
 from uswid.link import uSwidLink, uSwidLinkRel
 from uswid.hash import uSwidHash, uSwidHashAlg
 from uswid.payload import uSwidPayload
 from uswid.evidence import uSwidEvidence
-from uswid.identity import uSwidIdentity
+from uswid.component import uSwidComponent
 from uswid.problem import uSwidProblem
 from uswid.entity import uSwidEntity, uSwidEntityRole
 from uswid.enums import (
     uSwidGlobalMap,
     uSwidVersionScheme,
     uSwidHeaderFlags,
     uSwidPayloadCompression,
@@ -25,7 +25,14 @@
 from uswid.format_goswid import uSwidFormatGoswid
 from uswid.format_ini import uSwidFormatIni
 from uswid.format_pkgconfig import uSwidFormatPkgconfig
 from uswid.format_swid import uSwidFormatSwid
 from uswid.format_uswid import uSwidFormatUswid
 from uswid.format_cyclonedx import uSwidFormatCycloneDX
 from uswid.format_spdx import uSwidFormatSpdx
+from uswid.vex_document import uSwidVexDocument
+from uswid.vex_product import uSwidVexProduct
+from uswid.vex_statement import (
+    uSwidVexStatement,
+    uSwidVexStatementJustification,
+    uSwidVexStatementStatus,
+)
```

### Comparing `uswid-0.4.7/uswid/__init__.pyi` & `uswid-0.5.0/uswid/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+from uswid.component import uSwidComponent as uSwidComponent
 from uswid.container import uSwidContainer as uSwidContainer
 from uswid.entity import uSwidEntity as uSwidEntity, uSwidEntityRole as uSwidEntityRole
 from uswid.enums import USWID_HEADER_MAGIC as USWID_HEADER_MAGIC, uSwidGlobalMap as uSwidGlobalMap, uSwidHeaderFlags as uSwidHeaderFlags, uSwidPayloadCompression as uSwidPayloadCompression, uSwidVersionScheme as uSwidVersionScheme
 from uswid.errors import NotSupportedError as NotSupportedError
 from uswid.evidence import uSwidEvidence as uSwidEvidence
 from uswid.format_coswid import uSwidFormatCoswid as uSwidFormatCoswid
 from uswid.format_cyclonedx import uSwidFormatCycloneDX as uSwidFormatCycloneDX
 from uswid.format_goswid import uSwidFormatGoswid as uSwidFormatGoswid
 from uswid.format_ini import uSwidFormatIni as uSwidFormatIni
 from uswid.format_pkgconfig import uSwidFormatPkgconfig as uSwidFormatPkgconfig
 from uswid.format_spdx import uSwidFormatSpdx as uSwidFormatSpdx
 from uswid.format_swid import uSwidFormatSwid as uSwidFormatSwid
 from uswid.format_uswid import uSwidFormatUswid as uSwidFormatUswid
 from uswid.hash import uSwidHash as uSwidHash, uSwidHashAlg as uSwidHashAlg
-from uswid.identity import uSwidIdentity as uSwidIdentity
 from uswid.link import uSwidLink as uSwidLink, uSwidLinkRel as uSwidLinkRel
 from uswid.payload import uSwidPayload as uSwidPayload
 from uswid.problem import uSwidProblem as uSwidProblem
+from uswid.vex_document import uSwidVexDocument as uSwidVexDocument
+from uswid.vex_product import uSwidVexProduct as uSwidVexProduct
+from uswid.vex_statement import uSwidVexStatement as uSwidVexStatement, uSwidVexStatementJustification as uSwidVexStatementJustification, uSwidVexStatementStatus as uSwidVexStatementStatus
```

### Comparing `uswid-0.4.7/uswid/cli.py` & `uswid-0.5.0/uswid/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
 # pylint: disable=wrong-import-position
 
 from enum import IntEnum
 from collections import defaultdict
 from random import choices, randrange
 from datetime import datetime
 from typing import Optional, Any, List
 import argparse
 import tempfile
 import subprocess
 import socket
+import json
 
 import os
 import sys
 import shutil
 import uuid
 import string
 
-if sys.version_info >= (3, 8):
-    from importlib import metadata as importlib_metadata
-else:
-    import importlib_metadata
+from importlib import metadata as importlib_metadata
+from importlib.metadata import PackageNotFoundError
 
 import pefile
 
 sys.path.append(os.path.realpath("."))
 
 from uswid import (
     NotSupportedError,
     uSwidContainer,
     uSwidEntity,
     uSwidEntityRole,
-    uSwidIdentity,
+    uSwidComponent,
     uSwidProblem,
     uSwidVersionScheme,
     uSwidPayloadCompression,
 )
 from uswid.format_coswid import uSwidFormatCoswid
 from uswid.format_ini import uSwidFormatIni
 from uswid.format_goswid import uSwidFormatGoswid
 from uswid.format_pkgconfig import uSwidFormatPkgconfig
 from uswid.format_swid import uSwidFormatSwid
 from uswid.format_uswid import uSwidFormatUswid
 from uswid.format_cyclonedx import uSwidFormatCycloneDX
 from uswid.format_spdx import uSwidFormatSpdx
+from uswid.vex_document import uSwidVexDocument
 
 
 def _adjust_SectionSize(sz, align):
     if sz % align:
         sz = ((sz + align) // align) * align
     return sz
 
@@ -74,15 +74,15 @@
     return uSwidFormatCoswid().load(sect.get_data())
 
 
 def _load_efi_objcopy(filepath: str, objcopy: str) -> uSwidContainer:
     """read EFI file using objcopy"""
     objcopy_full = shutil.which(objcopy)
     if not objcopy_full:
-        print("executable {} not found".format(objcopy))
+        print(f"executable {objcopy} not found")
         sys.exit(1)
     with tempfile.NamedTemporaryFile(
         mode="w+b", prefix="objcopy_", suffix=".bin", delete=True
     ) as dst:
         try:
             # pylint: disable=unexpected-keyword-arg
             subprocess.check_output(
@@ -98,18 +98,18 @@
             )
         except subprocess.CalledProcessError as e:
             print(e)
             sys.exit(1)
         return uSwidFormatCoswid().load(dst.read())
 
 
-def _save_efi_pefile(identity: uSwidIdentity, filepath: str) -> None:
+def _save_efi_pefile(component: uSwidComponent, filepath: str) -> None:
     """modify EFI file using pefile"""
 
-    blob = uSwidFormatCoswid().save(uSwidContainer([identity]))
+    blob = uSwidFormatCoswid().save(uSwidContainer([component]))
     pe = pefile.PE(filepath)
     sect = _pe_get_section_by_name(pe, ".sbom")
     if not sect:
         raise NotSupportedError("PE files have to have an linker-defined .sbom section")
 
     # can we squeeze the new uSWID blob into the existing space
     sect.Misc = len(blob)
@@ -117,32 +117,36 @@
         pe.set_bytes_at_offset(sect.PointerToRawData, blob)
 
     # save
     pe.write(filepath)
 
 
 def _save_efi_objcopy(
-    identity: uSwidIdentity, filepath: str, cc: Optional[str], cflags: str, objcopy: str
+    component: uSwidComponent,
+    filepath: str,
+    cc: Optional[str],
+    cflags: str,
+    objcopy: str,
 ) -> None:
     """modify EFI file using objcopy"""
     objcopy_full = shutil.which(objcopy)
     if not objcopy_full:
-        print("executable {} not found".format(objcopy))
+        print(f"executable {objcopy} not found")
         sys.exit(1)
     if not os.path.exists(filepath):
         if not cc:
             raise NotSupportedError("compiler is required for missing section")
         subprocess.run(
             [cc, "-x", "c", "-c", "-o", filepath, "/dev/null"] + cflags.split(" "),
             check=True,
         )
 
     # save to file?
     try:
-        blob = uSwidFormatIni().save(uSwidContainer([identity]))
+        blob = uSwidFormatIni().save(uSwidContainer([component]))
     except NotSupportedError as e:
         print(e)
         sys.exit(1)
 
     with tempfile.NamedTemporaryFile(
         mode="wb", prefix="objcopy_", suffix=".bin", delete=True
     ) as src:
@@ -151,15 +155,15 @@
         try:
             # pylint: disable=unexpected-keyword-arg
             subprocess.check_output(
                 [
                     objcopy_full,
                     "--remove-section=.sbom",
                     "--add-section",
-                    ".sbom={}".format(src.name),
+                    f".sbom={src.name}",
                     "--set-section-flags",
                     ".sbom=contents,alloc,load,readonly,data",
                     filepath,
                 ]
             )
         except subprocess.CalledProcessError as e:
             print(e)
@@ -175,14 +179,15 @@
     USWID = 3
     PE = 4
     JSON = 5
     PKG_CONFIG = 6
     COSWID = 7
     CYCLONE_DX = 8
     SPDX = 9
+    VEX = 10
 
 
 def _detect_format(filepath: str) -> SwidFormat:
     if os.path.basename(filepath).endswith("bom.json"):
         return SwidFormat.CYCLONE_DX
     if os.path.basename(filepath).endswith("spdx.json"):
         return SwidFormat.SPDX
@@ -197,14 +202,16 @@
         return SwidFormat.INI
     if ext == "xml":
         return SwidFormat.XML
     if ext == "json":
         return SwidFormat.JSON
     if ext == "pc":
         return SwidFormat.PKG_CONFIG
+    if ext == "vex":
+        return SwidFormat.VEX
     return SwidFormat.UNKNOWN
 
 
 def _type_for_fmt(
     fmt: SwidFormat, args: Any, filepath: Optional[str] = None
 ) -> Optional[Any]:
     if fmt == SwidFormat.INI:
@@ -227,19 +234,22 @@
 
 
 def main():
     """Main entrypoint"""
     parser = argparse.ArgumentParser(
         prog="uswid", description="Generate CoSWID metadata"
     )
-    parser.add_argument(
-        "--version",
-        action="version",
-        version="%(prog)s " + importlib_metadata.version("uswid"),
-    )
+    try:
+        parser.add_argument(
+            "--version",
+            action="version",
+            version="%(prog)s " + importlib_metadata.version("uswid"),
+        )
+    except PackageNotFoundError:
+        pass
     parser.add_argument("--cc", default="gcc", help="Compiler to use for empty object")
     parser.add_argument(
         "--cflags", default="", help="C compiler flags to be used by CC"
     )
     parser.add_argument("--binfile", default=None, help=argparse.SUPPRESS)
     parser.add_argument("--rawfile", default=None, help=argparse.SUPPRESS)
     parser.add_argument("--inifile", default=None, help=argparse.SUPPRESS)
@@ -315,18 +325,18 @@
         load_filepaths.append(args.xmlfile)
 
     # sanity check
     if not load_filepaths and not save_filepaths:
         print("Use uswid --help for command line arguments")
         sys.exit(1)
 
-    # always load into a temporary identity so that we can query the tag_id
+    # always load into a temporary component so that we can query the tag_id
     container = uSwidContainer()
 
-    # generate 1000 plausible identities, each with:
+    # generate 1000 plausible components, each with:
     # - unique tag-id GUID
     # - unique software-name of size 4-30 chars
     # - colloquial-version from a random selection of 10 SHA-1 hashes
     # - edition from a random SHA-1 hash
     # - semantic version of size 3-8 chars
     # - entity from a random selection of 10 entities
     if args.generate:
@@ -337,156 +347,164 @@
         for i in range(10):
             entity = uSwidEntity()
             entity.name = "Entity#" + str(i)
             entity.regid = "com.entity" + str(i)
             entity.roles = [uSwidEntityRole.TAG_CREATOR]
             entities.append(entity)
         for i in range(1000):
-            identity = uSwidIdentity()
-            identity.tag_id = str(uuid.uuid4())
-            identity.software_name = "".join(
+            component = uSwidComponent()
+            component.tag_id = str(uuid.uuid4())
+            component.software_name = "".join(
                 choices(string.ascii_lowercase, k=randrange(4, 30))
             )
-            identity.software_version = "1." + "".join(
+            component.software_version = "1." + "".join(
                 choices("123456789", k=randrange(1, 6))
             )
-            identity.colloquial_version = tree_hashes[randrange(len(tree_hashes))]
-            identity.edition = "".join(choices("0123456789abcdef", k=40))
-            identity.version_scheme = uSwidVersionScheme.MULTIPARTNUMERIC
-            identity.add_entity(entities[randrange(len(entities))])
-            container.append(identity)
+            component.colloquial_version = tree_hashes[randrange(len(tree_hashes))]
+            component.edition = "".join(choices("0123456789abcdef", k=40))
+            component.version_scheme = uSwidVersionScheme.MULTIPARTNUMERIC
+            component.add_entity(entities[randrange(len(entities))])
+            container.append(component)
 
     # collect data here
     for filepath in load_filepaths:
         try:
             fmt = _detect_format(filepath)
             if fmt == SwidFormat.UNKNOWN:
-                print("{} has unknown extension, using uSWID".format(filepath))
+                print(f"{filepath} has unknown extension, using uSWID")
                 fmt = SwidFormat.USWID
             if fmt == SwidFormat.PE:
                 if args.objcopy:
                     container_tmp = _load_efi_objcopy(filepath, objcopy=args.objcopy)
                 else:
                     container_tmp = _load_efi_pefile(filepath)
-                for identity in container_tmp:
-                    identity_new = container.merge(identity)
-                    if identity_new:
+                for component in container_tmp:
+                    component_new = container.merge(component)
+                    if component_new:
                         print(
-                            "{} was merged into existing identity {}".format(
-                                filepath, identity_new.tag_id
+                            "{} was merged into existing component {}".format(
+                                filepath, component_new.tag_id
                             )
                         )
+            elif fmt == SwidFormat.VEX:
+                with open(filepath, "rb") as f:
+                    container.add_vex_document(
+                        uSwidVexDocument(json.loads(f.read().decode()))
+                    )
             elif fmt in [
                 SwidFormat.INI,
                 SwidFormat.JSON,
                 SwidFormat.COSWID,
                 SwidFormat.USWID,
                 SwidFormat.XML,
                 SwidFormat.PKG_CONFIG,
             ]:
                 base = _type_for_fmt(fmt, args, filepath=filepath)
                 if not base:
-                    print("{} no type for format".format(fmt))
+                    print(f"{fmt} no type for format")
                     sys.exit(1)
                 with open(filepath, "rb") as f:
-                    for identity in base.load(f.read(), path=os.path.dirname(filepath)):
-                        identity_new = container.merge(identity)
-                        if identity_new:
+                    for component in base.load(
+                        f.read(), path=os.path.dirname(filepath)
+                    ):
+                        component_new = container.merge(component)
+                        if component_new:
                             print(
-                                "{} was merged into existing identity {}".format(
-                                    filepath, identity_new.tag_id
+                                "{} was merged into existing component {}".format(
+                                    filepath, component_new.tag_id
                                 )
                             )
 
         except FileNotFoundError:
-            print("{} does not exist".format(filepath))
+            print(f"{filepath} does not exist")
             sys.exit(1)
         except NotSupportedError as e:
             print(e)
             sys.exit(1)
 
     # depsolve any internal SWID links
     container.depsolve()
 
     # validate
     rc: int = 0
     if args.validate:
-        problems_dict: dict[Optional[uSwidIdentity], List[uSwidProblem]] = defaultdict(
+        problems_dict: dict[Optional[uSwidComponent], List[uSwidProblem]] = defaultdict(
             list
         )
         if len(container) == 0:
-            problems_dict[None] += uSwidProblem(
-                "all", "There are no defined identities", since="0.4.7"
-            )
-        for identity in container:
-            problems_dict[identity].extend(identity.problems())
+            problems_dict[None] += [
+                uSwidProblem("all", "There are no defined components", since="0.4.7")
+            ]
+        for component in container:
+            problems = component.problems()
+            if problems:
+                problems_dict[component].extend(problems)
         if problems_dict:
             rc = 2
             print("Validation problems:")
-            for identity, problems in problems_dict.items():
+            for opt_component, problems in problems_dict.items():
                 for problem in problems:
-                    if identity:
-                        key = identity.tag_id
-                    else:
-                        key = "*"
+                    key: str = "*"
+                    if opt_component and opt_component.tag_id:
+                        key = opt_component.tag_id
                     print(
                         f"{key.ljust(40)} {problem.kind.rjust(10)}: "
                         f"{problem.description} (uSWID >= v{problem.since})"
                     )
 
     # add any missing evidence
-    for identity in container:
-        for evidence in identity.evidences:
+    for component in container:
+        for evidence in component.evidences:
             if not evidence.date and not evidence.device_id:
                 evidence.date = datetime.now()
                 evidence.device_id = socket.getfqdn()
 
     # debug
     if load_filepaths and args.verbose:
         print("Loaded:")
-        for identity in container:
-            print(f"{identity}")
+        for component in container:
+            print(f"{component}")
 
     # optional save
     if save_filepaths and args.verbose:
         print("Saving:")
-        for identity in container:
-            print(f"{identity}")
+        for component in container:
+            print(f"{component}")
     for filepath in save_filepaths:
         try:
             fmt = _detect_format(filepath)
             if fmt == SwidFormat.PE:
-                identity_pe: Optional[uSwidIdentity] = container.get_default()
-                if not identity_pe:
-                    print("cannot save PE when no default identity")
+                component_pe: Optional[uSwidComponent] = container.get_default()
+                if not component_pe:
+                    print("cannot save PE when no default component")
                     sys.exit(1)
                 if args.objcopy:
                     _save_efi_objcopy(
-                        identity_pe, filepath, args.cc, args.cflags, args.objcopy
+                        component_pe, filepath, args.cc, args.cflags, args.objcopy
                     )
                 else:
-                    _save_efi_pefile(identity_pe, filepath)
+                    _save_efi_pefile(component_pe, filepath)
             elif fmt in [
                 SwidFormat.INI,
                 SwidFormat.COSWID,
                 SwidFormat.JSON,
                 SwidFormat.XML,
                 SwidFormat.USWID,
                 SwidFormat.CYCLONE_DX,
                 SwidFormat.SPDX,
             ]:
                 base = _type_for_fmt(fmt, args)
                 if not base:
-                    print("{} no type for format".format(fmt))
+                    print(f"{fmt} no type for format")
                     sys.exit(1)
                 blob = base.save(container)
                 with open(filepath, "wb") as f:
                     f.write(blob)
             else:
-                print("{} extension is not supported".format(filepath))
+                print(f"{filepath} extension is not supported")
                 sys.exit(1)
         except NotSupportedError as e:
             print(e)
             sys.exit(1)
 
     # success
     sys.exit(rc)
```

### Comparing `uswid-0.4.7/uswid/entity.py` & `uswid-0.5.0/uswid/entity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
 # pylint: disable=too-few-public-methods
 
 from enum import IntEnum
 from typing import List, Optional
 
 from .problem import uSwidProblem
@@ -19,16 +19,19 @@
     TAG_CREATOR = 1
     SOFTWARE_CREATOR = 2
     AGGREGATOR = 3
     DISTRIBUTOR = 4
     LICENSOR = 5
     MAINTAINER = 6
 
+    def __str__(self):
+        return self.name.lower()
 
-def _fix_vendor_id(dns: str) -> str:
+
+def _fix_vendor_id(dns: str) -> Optional[str]:
 
     if not dns:
         return None
 
     # remove protocol prefix
     if dns.startswith("http://") or dns.startswith("https://"):
         dns = dns.split("/")[2]
@@ -65,16 +68,20 @@
 
     def problems(self) -> List[uSwidProblem]:
         """Checks the entity for common problems"""
 
         problems: List[uSwidProblem] = []
         if not self.name:
             problems += [uSwidProblem("entity", "No name", since="0.4.7")]
+        elif self.name.find("REDACTED") != -1:
+            problems += [uSwidProblem("entity", "Redacted name", since="0.4.8")]
         if not self.regid:
             problems += [uSwidProblem("entity", "No regid", since="0.4.7")]
+        elif self.regid.find("REDACTED") != -1:
+            problems += [uSwidProblem("entity", "Redacted regid", since="0.4.8")]
 
         # should be DNS name
         elif self.regid != _fix_vendor_id(self.regid):
             problems += [
                 uSwidProblem(
                     "entity",
                     f"Invalid regid {self.regid}, "
```

### Comparing `uswid-0.4.7/uswid/enums.py` & `uswid-0.5.0/uswid/enums.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 
 from enum import IntEnum
 
 
 class uSwidGlobalMap(IntEnum):
     """Represents an enumerated tag ID"""
 
@@ -65,37 +65,46 @@
     PRODUCT = 52
     PRODUCT_FAMILY = 53
     REVISION = 54
     SUMMARY = 55
     UNSPSC_CODE = 56
     UNSPSC_VERSION = 57
 
+    def __str__(self):
+        return self.name.lower()
+
 
 class uSwidVersionScheme(IntEnum):
     """Represents an enumerated version scheme"""
 
     MULTIPARTNUMERIC = 1
     MULTIPARTNUMERIC_SUFFIX = 2
     ALPHANUMERIC = 3
     DECIMAL = 4
     SEMVER = 16384
 
+    def __str__(self):
+        return self.name.lower()
+
 
 USWID_HEADER_MAGIC = b"\x53\x42\x4F\x4D\xD6\xBA\x2E\xAC\xA3\xE6\x7A\x52\xAA\xEE\x3B\xAF"
 
 # deprecated
 USWID_HEADER_FLAG_COMPRESSED = 0x01
 
 
 class uSwidHeaderFlags(IntEnum):
     """The header flags type"""
 
     NONE = 0x00
     COMPRESSED = 0x01
 
+    def __str__(self):
+        return self.name.lower()
+
 
 class uSwidPayloadCompression(IntEnum):
     """The payload compression type"""
 
     NONE = 0
     ZLIB = 1
     LZMA = 2
```

### Comparing `uswid-0.4.7/uswid/enums.pyi` & `uswid-0.5.0/uswid/enums.pyi`

 * *Files identical despite different names*

### Comparing `uswid-0.4.7/uswid/evidence.py` & `uswid-0.5.0/uswid/evidence.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2023 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
 # pylint: disable=too-few-public-methods
 
 from typing import List, Optional
 
 from datetime import datetime
 
@@ -29,14 +29,16 @@
         """Device ID, typically a machine hostname"""
 
     def problems(self) -> List[uSwidProblem]:
         """Checks the payload for common problems"""
 
         problems: List[uSwidProblem] = []
         if not self.date:
-            problems += uSwidProblem("evidence", "No date", since="0.4.7")
+            problems += [uSwidProblem("evidence", "No date", since="0.4.7")]
         if not self.device_id:
-            problems += uSwidProblem("payload", "No device_id", since="0.4.7")
+            problems += [uSwidProblem("evidence", "No device_id", since="0.4.7")]
+        elif self.device_id.find("REDACTED") != -1:
+            problems += [uSwidProblem("evidence", "Redacted device_id", since="0.4.8")]
         return problems
 
     def __repr__(self) -> str:
         return f'uSwidEvidence(date="{self.date}",device_id={self.device_id})'
```

### Comparing `uswid-0.4.7/uswid/format.py` & `uswid-0.5.0/uswid/format.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2023 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 
 from typing import Optional
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from .container import uSwidContainer
```

### Comparing `uswid-0.4.7/uswid/format_coswid.py` & `uswid-0.5.0/uswid/format_coswid.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
 # pylint: disable=too-few-public-methods,protected-access
 
-from typing import Dict, Any, Optional, List, Tuple
+from typing import Dict, Any, Optional, List, Tuple, Union
 
 import io
 import uuid
 from datetime import datetime
 
 import cbor2
 
 from .enums import uSwidGlobalMap
 from .container import uSwidContainer
 from .format import uSwidFormatBase
 from .errors import NotSupportedError
-from .identity import uSwidIdentity
+from .component import uSwidComponent
 from .entity import uSwidEntity, uSwidEntityRole
 from .link import uSwidLink, uSwidLinkRel
 from .hash import uSwidHash, uSwidHashAlg
 from .payload import uSwidPayload
 from .evidence import uSwidEvidence
 
 
@@ -38,32 +38,48 @@
     data: Dict[uSwidGlobalMap, Any], key: uSwidGlobalMap, value: List[Any]
 ) -> None:
     if not value:
         return
     data[key] = value if len(value) > 1 else value[0]
 
 
+def _to_perhaps_hex_bytes(value: str) -> Union[bytes, str]:
+
+    try:
+        return bytes.fromhex(value)
+    except ValueError:
+        return value
+
+
+def _from_perhaps_hex_bytes(value: Union[bytes, str]) -> str:
+
+    try:
+        return value.hex()  # type: ignore
+    except AttributeError:
+        return value  # type: ignore
+
+
 class uSwidFormatCoswid(uSwidFormatBase):
     """CoSWID file"""
 
     def __init__(self) -> None:
         """Initializes uSwidFormatCoswid"""
         uSwidFormatBase.__init__(self)
 
     def load(self, blob: bytes, path: Optional[str] = None) -> uSwidContainer:
-        identity = uSwidIdentity()
-        container = uSwidContainer([identity])
-        self._load_identity(identity, blob)
+        component = uSwidComponent()
+        container = uSwidContainer([component])
+        self._load_component(component, blob)
         return container
 
     def save(self, container: uSwidContainer) -> bytes:
-        identity = container.get_default()
-        if not identity:
-            raise NotSupportedError("cannot save when no default identity")
-        return self._save_identity(identity)
+        component = container.get_default()
+        if not component:
+            raise NotSupportedError("cannot save when no default component")
+        return self._save_component(component)
 
     def _save_link(self, link: uSwidLink) -> Dict[uSwidGlobalMap, Any]:
         """Exports a uSwidLink CoSWID section"""
 
         data: Dict[uSwidGlobalMap, Any] = {}
         data[uSwidGlobalMap.HREF] = link.href
 
@@ -122,99 +138,101 @@
         data: Dict[uSwidGlobalMap, Any] = {}
         data[uSwidGlobalMap.ENTITY_NAME] = entity.name
         if entity.regid:
             data[uSwidGlobalMap.REG_ID] = entity.regid
         _set_one_or_more(data, uSwidGlobalMap.ROLE, entity.roles)
         return data
 
-    def _save_identity(self, identity: uSwidIdentity) -> bytes:
-        """Exports a uSwidIdentity CoSWID blob"""
+    def _save_component(self, component: uSwidComponent) -> bytes:
+        """Exports a uSwidComponent CoSWID blob"""
 
-        # general identity section
+        # general component section
         data: Dict[uSwidGlobalMap, Any] = {}
 
-        if identity.lang:
-            data[uSwidGlobalMap.LANG] = identity.lang
-        if identity.tag_id:
+        if component.lang:
+            data[uSwidGlobalMap.LANG] = component.lang
+        if component.tag_id:
             try:
-                data[uSwidGlobalMap.TAG_ID] = uuid.UUID(hex=identity.tag_id).bytes
+                data[uSwidGlobalMap.TAG_ID] = uuid.UUID(hex=component.tag_id).bytes
             except (KeyError, ValueError):
-                data[uSwidGlobalMap.TAG_ID] = identity.tag_id
-        if identity.tag_version:
-            tag_version = identity.tag_version
-            if identity._auto_increment_tag_version:
+                data[uSwidGlobalMap.TAG_ID] = component.tag_id
+        if component.tag_version:
+            tag_version = component.tag_version
+            if component._auto_increment_tag_version:
                 tag_version += 1
             data[uSwidGlobalMap.TAG_VERSION] = tag_version
         data[uSwidGlobalMap.CORPUS] = True  # is firmware installable?
-        if identity.software_name:
-            data[uSwidGlobalMap.SOFTWARE_NAME] = identity.software_name
-        if not identity.software_version:
+        if component.software_name:
+            data[uSwidGlobalMap.SOFTWARE_NAME] = component.software_name
+        if not component.software_version:
             raise NotSupportedError("a software_version MUST be provided")
-        data[uSwidGlobalMap.SOFTWARE_VERSION] = identity.software_version
-        if identity.version_scheme:
-            data[uSwidGlobalMap.VERSION_SCHEME] = identity.version_scheme
+        data[uSwidGlobalMap.SOFTWARE_VERSION] = component.software_version
+        if component.version_scheme:
+            data[uSwidGlobalMap.VERSION_SCHEME] = component.version_scheme
 
         # metadata section
         metadata: Dict[uSwidGlobalMap, Any] = {
-            uSwidGlobalMap.GENERATOR: identity.generator
+            uSwidGlobalMap.GENERATOR: component.generator
         }
-        if identity.summary:
-            metadata[uSwidGlobalMap.SUMMARY] = identity.summary
-        if identity.revision:
-            metadata[uSwidGlobalMap.REVISION] = identity.revision
-        if identity.product:
-            metadata[uSwidGlobalMap.PRODUCT] = identity.product
-        if identity.edition:
-            metadata[uSwidGlobalMap.EDITION] = identity.edition
-        if identity.colloquial_version:
-            metadata[uSwidGlobalMap.COLLOQUIAL_VERSION] = identity.colloquial_version
-        if identity.persistent_id:
-            metadata[uSwidGlobalMap.PERSISTENT_ID] = identity.persistent_id
+        if component.summary:
+            metadata[uSwidGlobalMap.SUMMARY] = component.summary
+        if component.revision:
+            metadata[uSwidGlobalMap.REVISION] = component.revision
+        if component.product:
+            metadata[uSwidGlobalMap.PRODUCT] = component.product
+        if component.edition:
+            metadata[uSwidGlobalMap.EDITION] = _to_perhaps_hex_bytes(component.edition)
+        if component.colloquial_version:
+            metadata[uSwidGlobalMap.COLLOQUIAL_VERSION] = _to_perhaps_hex_bytes(
+                component.colloquial_version
+            )
+        if component.persistent_id:
+            metadata[uSwidGlobalMap.PERSISTENT_ID] = component.persistent_id
         data[uSwidGlobalMap.SOFTWARE_META] = metadata
 
         # payloads
-        if identity.payloads:
+        if component.payloads:
             _set_one_or_more(
                 data,
                 uSwidGlobalMap.PAYLOAD,
-                [self._save_payload(payload) for payload in identity.payloads],
+                [self._save_payload(payload) for payload in component.payloads],
             )
 
         # evidences
-        if identity.evidences:
+        if component.evidences:
             _set_one_or_more(
                 data,
                 uSwidGlobalMap.EVIDENCE,
-                [self._save_evidence(evidence) for evidence in identity.evidences],
+                [self._save_evidence(evidence) for evidence in component.evidences],
             )
 
         # entities
-        if not identity._entities:
+        if not component._entities:
             raise NotSupportedError("at least one entity MUST be provided")
         has_tag_creator = False
-        for entity in identity._entities.values():
+        for entity in component._entities.values():
             if not entity.roles:
                 raise NotSupportedError(
-                    "all entities MUST have at least one role: {}".format(str(entity))
+                    f"all entities MUST have at least one role: {str(entity)}"
                 )
             if not entity.name:
                 raise NotSupportedError("all entities MUST have a name")
             if uSwidEntityRole.TAG_CREATOR in entity.roles:
                 has_tag_creator = True
         if not has_tag_creator:
             raise NotSupportedError("all entries MUST have a tag-creator")
         _set_one_or_more(
             data,
             uSwidGlobalMap.ENTITY,
-            [self._save_entity(entity) for entity in identity._entities.values()],
+            [self._save_entity(entity) for entity in component._entities.values()],
         )
         _set_one_or_more(
             data,
             uSwidGlobalMap.LINK,
-            [self._save_link(link) for link in identity._links.values()],
+            [self._save_link(link) for link in component._links.values()],
         )
         return cbor2.dumps(data)
 
     def _load_link(self, link: uSwidLink, data: Dict[uSwidGlobalMap, Any]) -> None:
         """Imports a uSwidLink CoSWID section"""
 
         # always a string
@@ -242,17 +260,15 @@
                 uSwidLinkRel.SUPERSEDES: "supersedes",
                 uSwidLinkRel.SUPPLEMENTAL: "supplemental",
             }
             try:
                 link.rel = LINK_MAP[rel_data]
             except KeyError as e:
                 raise NotSupportedError(
-                    "{} not supported from {}".format(
-                        rel_data, ",".join(LINK_MAP.values())
-                    )
+                    f"{rel_data} not supported from {','.join(LINK_MAP.values())}"
                 ) from e
 
     def _load_hash(self, ihash: uSwidHash, data: Any) -> None:
         """Imports a uSwidHash CoSWID section"""
         ihash.alg_id = uSwidHashAlg(data[0])
         if isinstance(data[1], bytes):
             ihash.value = bytes.hex(data[1])
@@ -302,21 +318,21 @@
         entity_roles = data.get(uSwidGlobalMap.ROLE, [])
         if isinstance(entity_roles, int):
             entity_roles = [entity_roles]
         for role in entity_roles:
             try:
                 entity.roles.append(uSwidEntityRole(int(role)))
             except KeyError:
-                print("ignoring invalid role of {}".format(role))
+                print(f"ignoring invalid role of {role}")
                 continue
 
-    def _load_identity(
-        self, identity: uSwidIdentity, blob: bytes, offset: Optional[int] = 0
+    def _load_component(
+        self, component: uSwidComponent, blob: bytes, offset: Optional[int] = 0
     ) -> int:
-        """Imports a uSwidIdentity CoSWID blob"""
+        """Imports a uSwidComponent CoSWID blob"""
 
         if not blob:
             return 0
         consumed: int = 0
         try:
             f = io.BytesIO(blob[offset:])
             data = cbor2.load(f)
@@ -326,46 +342,46 @@
 
         # strip off digital signature
         if isinstance(data, cbor2.CBORTag):
             if data.tag != 98:
                 raise NotSupportedError("invalid digital signature")
             data = cbor2.loads(data.value[2])
 
-        # identity can be specified as a string or in binary
+        # component can be specified as a string or in binary
         tag_id_bytes = data.get(uSwidGlobalMap.TAG_ID, None)
         if isinstance(tag_id_bytes, str):
-            identity.tag_id = tag_id_bytes
+            component.tag_id = tag_id_bytes
         else:
             try:
-                identity.tag_id = str(uuid.UUID(bytes=tag_id_bytes))
+                component.tag_id = str(uuid.UUID(bytes=tag_id_bytes))
             except ValueError:
-                identity.tag_id = tag_id_bytes.hex()
+                component.tag_id = tag_id_bytes.hex()
 
-        identity.tag_version = data.get(uSwidGlobalMap.TAG_VERSION, 0)
-        identity.software_name = data.get(uSwidGlobalMap.SOFTWARE_NAME, None)
-        identity.software_version = data.get(uSwidGlobalMap.SOFTWARE_VERSION, None)
-        identity.version_scheme = data.get(uSwidGlobalMap.VERSION_SCHEME, None)
+        component.tag_version = data.get(uSwidGlobalMap.TAG_VERSION, 0)
+        component.software_name = data.get(uSwidGlobalMap.SOFTWARE_NAME, None)
+        component.software_version = data.get(uSwidGlobalMap.SOFTWARE_VERSION, None)
+        component.version_scheme = data.get(uSwidGlobalMap.VERSION_SCHEME, None)
 
         # optional metadata
         for sm in _get_one_or_more(data, uSwidGlobalMap.SOFTWARE_META):
             for key, value in sm.items():
                 if key == uSwidGlobalMap.GENERATOR:
-                    identity.generator = value
+                    component.generator = value
                 elif key == uSwidGlobalMap.SUMMARY:
-                    identity.summary = value
+                    component.summary = value
                 elif key == uSwidGlobalMap.REVISION:
-                    identity.revision = value
+                    component.revision = value
                 elif key == uSwidGlobalMap.PRODUCT:
-                    identity.product = value
+                    component.product = value
                 elif key == uSwidGlobalMap.EDITION:
-                    identity.edition = value
+                    component.edition = _from_perhaps_hex_bytes(value)
                 elif key == uSwidGlobalMap.COLLOQUIAL_VERSION:
-                    identity.colloquial_version = value
+                    component.colloquial_version = _from_perhaps_hex_bytes(value)
                 elif key == uSwidGlobalMap.PERSISTENT_ID:
-                    identity.persistent_id = value
+                    component.persistent_id = value
 
         # payload
         file_datas = []
         for payload_data in _get_one_or_more(data, uSwidGlobalMap.PAYLOAD):
             file_datas.extend(_get_one_or_more(payload_data, uSwidGlobalMap.FILE))
             for directory_data in _get_one_or_more(
                 payload_data, uSwidGlobalMap.DIRECTORY
@@ -373,34 +389,34 @@
                 for path_data in _get_one_or_more(
                     directory_data, uSwidGlobalMap.PATH_ELEMENTS
                 ):
                     file_datas.extend(_get_one_or_more(path_data, uSwidGlobalMap.FILE))
         for file_data in file_datas:
             payload = uSwidPayload()
             self._load_payload(payload, file_data)
-            identity.add_payload(payload)
+            component.add_payload(payload)
 
         # evidence
         for evidence_data in _get_one_or_more(data, uSwidGlobalMap.EVIDENCE):
             evidence = uSwidEvidence()
             self._load_evidence(evidence, evidence_data)
-            identity.add_evidence(evidence)
+            component.add_evidence(evidence)
 
         # entities
         for entity_data in _get_one_or_more(data, uSwidGlobalMap.ENTITY):
             entity = uSwidEntity()
             self._load_entity(entity, entity_data)
             # skip invalid entries
             if not entity.roles:
                 continue
-            identity.add_entity(entity)
+            component.add_entity(entity)
 
         # links
         for link_data in _get_one_or_more(data, uSwidGlobalMap.LINK):
             link = uSwidLink()
             self._load_link(link, link_data)
-            identity.add_link(link)
+            component.add_link(link)
 
-        identity._auto_increment_tag_version = True
+        component._auto_increment_tag_version = True
 
         # number of bytes consumed, i.e. where the next CBOR blob is found
         return consumed
```

### Comparing `uswid-0.4.7/uswid/format_coswid.pyi` & `uswid-0.5.0/uswid/format_coswid.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,15 @@
+from .component import uSwidComponent as uSwidComponent
 from .container import uSwidContainer as uSwidContainer
 from .entity import uSwidEntity as uSwidEntity, uSwidEntityRole as uSwidEntityRole
 from .enums import uSwidGlobalMap as uSwidGlobalMap
 from .errors import NotSupportedError as NotSupportedError
 from .evidence import uSwidEvidence as uSwidEvidence
 from .format import uSwidFormatBase as uSwidFormatBase
 from .hash import uSwidHash as uSwidHash, uSwidHashAlg as uSwidHashAlg
-from .identity import uSwidIdentity as uSwidIdentity
 from .link import uSwidLink as uSwidLink, uSwidLinkRel as uSwidLinkRel
 from .payload import uSwidPayload as uSwidPayload
-from typing import Optional
 
 class uSwidFormatCoswid(uSwidFormatBase):
     def __init__(self) -> None: ...
-    def load(self, blob: bytes, path: Optional[str] = ...) -> uSwidContainer: ...
+    def load(self, blob: bytes, path: str | None = None) -> uSwidContainer: ...
     def save(self, container: uSwidContainer) -> bytes: ...
```

### Comparing `uswid-0.4.7/uswid/format_cyclonedx.py` & `uswid-0.5.0/uswid/format_cyclonedx.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 
 from typing import Dict, Any, Optional, List
 
 import json
 import uuid
 from datetime import datetime
 
 from .container import uSwidContainer
 from .format import uSwidFormatBase
-from .identity import uSwidIdentity
+from .component import uSwidComponent
 from .entity import uSwidEntityRole
 from .hash import uSwidHashAlg
 
 
 def _convert_hash_alg_id(alg_id: uSwidHashAlg) -> str:
     return {
         uSwidHashAlg.SHA256: "SHA-256",
@@ -34,15 +34,15 @@
         uSwidFormatBase.__init__(self)
 
     def save(self, container: uSwidContainer) -> bytes:
         # header
         root: Dict[str, Any] = {}
         root["bomFormat"] = "CycloneDX"
         root["specVersion"] = "1.4"
-        root["serialNumber"] = "urn:uuid:{}".format(str(uuid.uuid4()))
+        root["serialNumber"] = f"urn:uuid:{str(uuid.uuid4())}"
         root["version"] = 1
 
         # metadata
         metadata: Dict[str, Any] = {}
         metadata["timestamp"] = datetime.now().isoformat()
         root["metadata"] = metadata
 
@@ -51,17 +51,17 @@
             {"vendor": "uSWID Authors", "name": "uSWID", "version": "0.4.0"}
         ]
 
         # find components
         components: List[Dict[str, Any]] = []
         licenses: List[Dict[str, Any]] = []
         dependencies: List[Dict[str, str]] = []
-        for identity in container:
-            components.append(self._save_identity(identity))
-            for link in identity.links:
+        for component in container:
+            components.append(self._save_component(component))
+            for link in component.links:
                 if not link.href:
                     continue
                 if link.rel == "license":
                     license_choice: Dict[str, Any] = {}
                     license_choice["license"] = {"url": link.href}
                     licenses.append(license_choice)
                 if link.rel in ["component", "compiler"]:
@@ -73,79 +73,79 @@
         if dependencies:
             root["dependencies"] = dependencies
         if licenses:
             root["licenses"] = licenses
 
         return json.dumps(root, indent=2).encode()
 
-    def _save_identity(self, identity: uSwidIdentity) -> Dict[str, Any]:
-        component: Dict[str, Any] = {}
-        component["type"] = "firmware"
-        if identity.persistent_id:
-            component["group"] = identity.persistent_id
-        if identity.product:
-            component["name"] = identity.product
-        if identity.summary:
-            component["description"] = identity.summary
+    def _save_component(self, component: uSwidComponent) -> Dict[str, Any]:
+        root: Dict[str, Any] = {}
+        root["type"] = "firmware"
+        if component.persistent_id:
+            root["group"] = component.persistent_id
+        if component.product:
+            root["name"] = component.product
+        if component.summary:
+            root["description"] = component.summary
 
         swid: Dict[str, Any] = {}
-        if identity.tag_id:
-            swid["tagId"] = identity.tag_id
-        if identity.software_name:
-            swid["name"] = identity.software_name
-        if identity.software_version:
-            swid["version"] = identity.software_version
-        if identity.tag_version:
-            swid["tagVersion"] = identity.tag_version
-        component["swid"] = swid
+        if component.tag_id:
+            swid["tagId"] = component.tag_id
+        if component.software_name:
+            swid["name"] = component.software_name
+        if component.software_version:
+            swid["version"] = component.software_version
+        if component.tag_version:
+            swid["tagVersion"] = component.tag_version
+        root["swid"] = swid
 
-        if identity.colloquial_version:
+        if component.colloquial_version:
             commit: Dict[str, str] = {}
-            commit["uid"] = identity.colloquial_version
-            component["commit"] = commit
+            commit["uid"] = component.colloquial_version
+            root["commit"] = commit
 
         # supplier and authors
         supplier: Dict[str, Any] = {}
         publisher: Optional[str] = None
         author: Optional[str] = None
-        for entity in identity.entities:
+        for entity in component.entities:
             if uSwidEntityRole.LICENSOR in entity.roles:
                 if entity.name:
                     supplier["name"] = entity.name
                 if entity.regid:
                     supplier["url"] = [entity.regid]
             if uSwidEntityRole.DISTRIBUTOR in entity.roles:
                 if entity.name:
                     publisher = entity.name
             if uSwidEntityRole.SOFTWARE_CREATOR in entity.roles:
                 if entity.name:
                     author = entity.name
         if supplier:
-            component["supplier"] = supplier
+            root["supplier"] = supplier
         if publisher:
-            component["publisher"] = publisher
+            root["publisher"] = publisher
         if author:
-            component["author"] = author
+            root["author"] = author
         hashes: List[Any] = []
-        for payload in identity.payloads:
+        for payload in component.payloads:
             for ihash in payload.hashes:
                 if not ihash.alg_id:
                     continue
                 hashes.append(
                     {"alg": _convert_hash_alg_id(ihash.alg_id), "content": ihash.value}
                 )
         if hashes:
-            component["hashes"] = hashes
+            root["hashes"] = hashes
 
         # annotations
         annotations: List[Dict[str, Any]] = []
-        for evidence in identity.evidences:
-            annotation = {"subjects": [identity.tag_id], "annotator": "component"}
+        for evidence in component.evidences:
+            annotation = {"subjects": [component.tag_id], "annotator": "component"}
             if evidence.date:
                 annotation["timestamp"] = evidence.date.isoformat()
             if evidence.device_id:
                 annotation["text"] = evidence.device_id
             annotations.append(annotation)
         if annotations:
-            component["annotations"] = annotations
+            root["annotations"] = annotations
 
-        return component
+        return root
```

### Comparing `uswid-0.4.7/uswid/format_goswid.py` & `uswid-0.5.0/uswid/format_ini.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,329 +1,310 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
-# pylint: disable=too-few-public-methods,protected-access,too-many-boolean-expressions
+# pylint: disable=too-few-public-methods,protected-access
 
-from typing import Dict, Any, Optional, List
+from typing import Dict, List, Any, Optional, Union
 
-import json
+import configparser
+import io
+import os
 from datetime import datetime
 
 from .container import uSwidContainer
 from .format import uSwidFormatBase
 from .errors import NotSupportedError
-from .identity import (
-    uSwidIdentity,
+from .component import (
+    uSwidComponent,
     _VERSION_SCHEME_TO_STRING,
     _VERSION_SCHEME_FROM_STRING,
 )
-from .entity import uSwidEntity
+from .entity import uSwidEntity, uSwidEntityRole
 from .link import uSwidLink
-from .hash import uSwidHash, uSwidHashAlg
+from .hash import uSwidHash
 from .payload import uSwidPayload
 from .evidence import uSwidEvidence
-from .format_swid import _ENTITY_MAP_FROM_XML, _ENTITY_MAP_TO_XML
 
+_ENTITY_MAP_FROM_INI = {
+    "TagCreator": uSwidEntityRole.TAG_CREATOR,
+    "SoftwareCreator": uSwidEntityRole.SOFTWARE_CREATOR,
+    "Aggregator": uSwidEntityRole.AGGREGATOR,
+    "Distributor": uSwidEntityRole.DISTRIBUTOR,
+    "Licensor": uSwidEntityRole.LICENSOR,
+    "Maintainer": uSwidEntityRole.MAINTAINER,
+}
+_ENTITY_MAP_TO_INI = {
+    uSwidEntityRole.TAG_CREATOR: "TagCreator",
+    uSwidEntityRole.SOFTWARE_CREATOR: "SoftwareCreator",
+    uSwidEntityRole.AGGREGATOR: "Aggregator",
+    uSwidEntityRole.DISTRIBUTOR: "Distributor",
+    uSwidEntityRole.LICENSOR: "Licensor",
+    uSwidEntityRole.MAINTAINER: "Maintainer",
+}
 
-def _get_one_or_more(data: Dict[str, Any], key: str) -> List[Any]:
-    value = data.get(key, [])
-    if isinstance(value, list):
-        return value
-    return [value]
 
-
-class uSwidFormatGoswid(uSwidFormatBase):
-    """goSWID file"""
+class uSwidFormatIni(uSwidFormatBase):
+    """INI file"""
 
     def __init__(self) -> None:
-        """Initializes uSwidFormatGoswid"""
+        """Initializes uSwidFormatIni"""
         uSwidFormatBase.__init__(self)
 
     def load(self, blob: bytes, path: Optional[str] = None) -> uSwidContainer:
-        try:
-            data = json.loads(blob)
-        except json.decoder.JSONDecodeError as e:
-            raise NotSupportedError("invalid GoSWID: {}".format(e)) from e
-        container = uSwidContainer()
-        if "corim_id" in data:
-            data = data["corim_tags"]
-        for identity_json in data:
-            identity = uSwidIdentity()
-            self._load_identity_internal(identity, identity_json)
-            container.merge(identity)
-        return container
+        component = uSwidComponent()
+        self._load_component(component, blob, path=path)
+        return uSwidContainer([component])
 
     def save(self, container: uSwidContainer) -> bytes:
-        root = []
-        for identity in container:
-            root.append(self._save_identity_internal(identity))
-        return json.dumps(root, indent=2).encode()
+        component = container.get_default()
+        if not component:
+            raise NotSupportedError("cannot save when no default component")
+        return self._save_component(component)
 
-    def _save_link(self, link: uSwidLink) -> Dict[str, str]:
-        """Exports a uSwidLink goSWID section"""
+    def _save_link(self, link: uSwidLink) -> Dict[str, Any]:
+        """Exports a uSwidLink INI section"""
 
-        node: Dict[str, str] = {}
-        if link.href:
-            node["href"] = link.href
+        data: Dict[str, Any] = {}
         if link.rel:
-            node["rel"] = link.rel
-        return node
+            data["rel"] = link.rel
+        if link.href:
+            data["href"] = link.href
+        return data
 
     def _save_payload(self, payload: uSwidPayload) -> Dict[str, Any]:
-        """Exports a uSwidLink goSWID section"""
+        """Exports a uSwidLink INI section"""
 
-        node: Dict[str, Any] = {}
+        data: Dict[str, Any] = {}
         if payload.name:
-            node["fs-name"] = payload.name
+            data["name"] = payload.name
         if payload.size:
-            node["size"] = str(payload.size)
+            data["size"] = payload.size
         if payload.hashes:
-            node["hash"] = [payload.hashes[0].alg_id or 0, payload.hashes[0].value]
-        return {"file": [node]}
+            data["hash"] = payload.hashes[0].value
+        return data
 
     def _save_evidence(self, evidence: uSwidEvidence) -> Dict[str, Any]:
-        """Exports a uSwidLink goSWID section"""
+        """Exports a uSwidLink INI section"""
 
-        node: Dict[str, str] = {}
+        data: Dict[str, Any] = {}
         if evidence.date:
-            node["date"] = evidence.date.isoformat()
+            data["date"] = evidence.date.isoformat()
         if evidence.device_id:
-            node["device_id"] = evidence.device_id
-        return node
+            data["device-id"] = evidence.device_id
+        return data
 
     def _save_entity(self, entity: uSwidEntity) -> Dict[str, Any]:
-        """Exports a uSwidEntity goSWID section"""
+        """Exports a uSwidEntity INI section"""
 
-        node: Dict[str, Any] = {}
+        data: Dict[str, Any] = {}
         if entity.name:
-            node["entity-name"] = entity.name
+            data["name"] = entity.name
         if entity.regid:
-            node["reg-id"] = entity.regid
-        roles = []
+            data["regid"] = entity.regid
+        extra_roles: List[str] = []
         for role in entity.roles:
-            try:
-                roles.append(_ENTITY_MAP_TO_XML[role])
-            except KeyError as e:
-                raise NotSupportedError(
-                    "{} not supported from {}".format(
-                        role, ",".join(_ENTITY_MAP_TO_XML.values())
-                    )
-                ) from e
-        # use string if only one role
-        if len(roles) == 1:
-            node["role"] = roles[0]
-        else:
-            node["role"] = roles
-        return node
-
-    def _save_identity_internal(self, identity: uSwidIdentity) -> Dict[str, Any]:
-        # identity
-        root: Dict[str, Any] = {}
-        if identity.lang:
-            root["lang"] = identity.lang
-        if identity.tag_id:
-            root["tag-id"] = identity.tag_id
-        if identity.tag_version:
-            root["tag-version"] = identity.tag_version
-        if identity.software_name:
-            root["software-name"] = identity.software_name
-        if identity.software_version:
-            root["software-version"] = identity.software_version
-        if identity.version_scheme:
-            root["version-scheme"] = _VERSION_SCHEME_TO_STRING[identity.version_scheme]
-
-        # optional metadata
-        if (
-            identity.summary
-            or identity.revision
-            or identity.product
-            or identity.edition
-            or identity.colloquial_version
-            or identity.persistent_id
-        ):
-            node: Dict[str, str] = {}
-            if identity.summary:
-                node["summary"] = identity.summary
-            if identity.revision:
-                node["revision"] = identity.revision
-            if identity.product:
-                node["product"] = identity.product
-            if identity.edition:
-                node["edition"] = identity.edition
-            if identity.colloquial_version:
-                node["colloquial-version"] = identity.colloquial_version
-            if identity.persistent_id:
-                node["persistent-id"] = identity.persistent_id
-            # the CoSWID spec says: 'software-meta => one-or-more'
-            root["software-meta"] = [node]
-
-        # checksum
-        if identity.payloads:
-            root["payload"] = []
-            for payload in identity.payloads:
-                root["payload"].append(self._save_payload(payload))
-
-        # evidences
-        if identity.evidences:
-            root["evidence"] = []
-            for evidence in identity.evidences:
-                root["evidence"].append(self._save_evidence(evidence))
-
-        # entities
-        if identity.entities:
-            root["entity"] = []
-            for entity in identity.entities:
-                root["entity"].append(self._save_entity(entity))
-
-        # links
-        if identity.links:
-            root["link"] = []
-            for link in identity.links:
-                root["link"].append(self._save_link(link))
-
-        # success
-        return root
-
-    def _save_identity(self, identity: uSwidIdentity) -> bytes:
-        """Exports a uSwidIdentity goSWID blob"""
-        return json.dumps(self._save_identity_internal(identity), indent=2).encode(
-            "utf-8"
-        )
-
-    def _load_link(self, link: uSwidLink, node: Dict[str, str]) -> None:
-        """Imports a uSwidLink goSWID section"""
-
-        link.href = node.get("href")
-        link.rel = node.get("rel")
-
-    def _load_evidence(self, evidence: uSwidEvidence, node: Dict[str, str]) -> None:
-        """Imports a uSwidEvidence goSWID section"""
-
-        iso_date = node.get("date")
-        if iso_date:
-            evidence.date = datetime.fromisoformat(iso_date)
-        evidence.device_id = node.get("device_id")
-
-    def _load_file(self, payload: uSwidPayload, node: Dict[str, Any]) -> None:
-        """Imports a uSwidPayload goSWID section"""
-
-        # for compat with Intel FSP template
-        for key in list(node):
-            node[key.replace("_", "-")] = node.pop(key)
-
-        payload.name = node.get("fs-name")
-        try:
-            payload.size = int(node["size"])
-        except (ValueError, KeyError):
-            pass
-        if "hash" in node:
-            ihash = uSwidHash()
-            # Intel FSP order is reversed
-            try:
-                ihash.alg_id = uSwidHashAlg(int(node["hash"][0]))
-                ihash.value = node["hash"][1]
-            except ValueError:
-                ihash.value = node["hash"][0]
-                ihash.alg_id = uSwidHashAlg(int(node["hash"][1]))
-            payload.add_hash(ihash)
+            if role == uSwidEntityRole.TAG_CREATOR:
+                continue
+            extra_roles.append(_ENTITY_MAP_TO_INI[role])
+        if extra_roles:
+            data["extra-roles"] = ",".join(extra_roles)
+        return data
+
+    def _save_component(self, component: uSwidComponent) -> bytes:
+        config = configparser.ConfigParser()
+
+        # main section
+        main = {}
+        if component.tag_id:
+            main["tag-id"] = component.tag_id
+        if component.tag_version:
+            main["tag-version"] = str(component.tag_version)
+        if component.software_name:
+            main["software-name"] = component.software_name
+        if component.software_version:
+            main["software-version"] = component.software_version
+        if component.version_scheme:
+            main["version-scheme"] = _VERSION_SCHEME_TO_STRING[component.version_scheme]
+        if component.summary:
+            main["summary"] = component.summary
+        if component.revision:
+            main["revision"] = component.revision
+        if component.product:
+            main["product"] = component.product
+        if component.edition:
+            main["edition"] = component.edition
+        if component.colloquial_version:
+            main["colloquial-version"] = component.colloquial_version
+        if component.persistent_id:
+            main["persistent-id"] = component.persistent_id
+        config["uSWID"] = main
+
+        # entity
+        if component.entities:
+            config["uSWID-Entity:TagCreator"] = self._save_entity(component.entities[0])
+
+        # link
+        if component.links:
+            config["uSWID-Link"] = self._save_link(component.links[0])
+
+        # payload
+        if component.payloads:
+            config["uSWID-Payload"] = self._save_payload(component.payloads[0])
+
+        # evidence
+        if component.evidences:
+            config["uSWID-Evidence"] = self._save_evidence(component.evidences[0])
+
+        # as string
+        with io.StringIO() as f:
+            config.write(f)
+            f.seek(0)
+            return f.read().encode()
+
+    def _load_link(
+        self, link: uSwidLink, data: Union[configparser.SectionProxy, Dict[str, str]]
+    ) -> None:
+        """Imports a uSwidLink INI section"""
+
+        for key, value in data.items():
+            if key == "href":
+                link.href = value
+            elif key == "rel":
+                link.rel = value
+            else:
+                print(f"unknown key {key} found in ini file!")
+        if not link.href:
+            raise NotSupportedError("all entities MUST have a href")
+
+    def _load_payload(
+        self,
+        payload: uSwidPayload,
+        data: Union[configparser.SectionProxy, Dict[str, str]],
+        path: Optional[str] = None,
+    ) -> None:
+        """Imports a uSwidPayload INI section"""
+
+        for key, value in data.items():
+            if key == "name":
+                payload.name = value
+            elif key == "size":
+                payload.size = int(value)
+            elif key == "hash":
+                payload.add_hash(uSwidHash(value=value))
+            elif key == "path":
+                payload.name = os.path.basename(value)
+                if os.path.exists(value):
+                    payload.ensure_from_filename(value)
+            else:
+                print(f"unknown key {key} found in ini file!")
+
+        # can we load this and work it out
+        if path and payload.name:
+            fn = os.path.join(path, payload.name)
+            if os.path.exists(fn):
+                payload.ensure_from_filename(fn)
+        if not payload.hashes:
+            raise NotSupportedError("all payloads MUST have at least one hash")
+
+    def _load_evidence(
+        self,
+        evidence: uSwidEvidence,
+        data: Union[configparser.SectionProxy, Dict[str, str]],
+    ) -> None:
+        """Imports a uSwidEvidence INI section"""
+
+        for key, value in data.items():
+            if key == "date":
+                evidence.date = datetime.fromisoformat(value)
+            elif key == "device-id":
+                evidence.device_id = value
+            else:
+                print(f"unknown key {key} found in ini file!")
 
     def _load_entity(
         self,
         entity: uSwidEntity,
-        node: Dict[str, str],
+        data: Union[configparser.SectionProxy, Dict[str, str]],
+        role_hint: Optional[str] = None,
     ) -> None:
-        """Imports a uSwidEntity goSWID section"""
+        """Imports a uSwidEntity INI section"""
 
-        # for compat with Intel FSP template
-        for key in list(node):
-            node[key.replace("_", "-")] = node.pop(key)
-
-        entity.name = node.get("entity-name")
-        entity.regid = node.get("reg-id")
-        roles = node.get("role")
-        if roles and isinstance(roles, str):
-            roles = [roles]  # type: ignore
-        for role_str in roles:  # type: ignore
+        if role_hint:
             try:
-                entity.roles.append(_ENTITY_MAP_FROM_XML[role_str])
-            except KeyError as e:
-                raise NotSupportedError(
-                    "{} not supported from {}".format(
-                        role_str, ",".join(_ENTITY_MAP_FROM_XML)
-                    )
-                ) from e
+                entity.roles.append(_ENTITY_MAP_FROM_INI[role_hint.split(":")[1]])
+            except (KeyError, TypeError, IndexError):
+                pass
+        for key, value in data.items():
+            if key == "name":
+                entity.name = value
+            elif key == "regid":
+                entity.regid = value
+            elif key == "extra-roles":
+                for role_str in value.split(","):
+                    try:
+                        entity.roles.append(_ENTITY_MAP_FROM_INI[role_str])
+                    except KeyError as e:
+                        raise NotSupportedError(
+                            "{} not supported from {}".format(
+                                role_str, ",".join(_ENTITY_MAP_FROM_INI)
+                            )
+                        ) from e
+            else:
+                print(f"unknown key {key} found in ini file!")
+        if not entity.name:
+            raise NotSupportedError("all entities MUST have a name")
+        if not entity.roles:
+            raise NotSupportedError(f"entity {entity.name} MUST have at least one role")
 
-    def _load_identity_internal(
-        self, identity: uSwidIdentity, data: Dict[str, Any]
+    def _load_component(
+        self, component: uSwidComponent, blob: bytes, path: Optional[str]
     ) -> None:
-        # for compat with Intel FSP template
-        for key in list(data):
-            data[key.replace("_", "-")] = data.pop(key)
-
-        # identity
-        identity.tag_id = data.get("tag-id")
-        tag_version = data.get("tag-version")
-        if tag_version:
-            identity.tag_version = int(tag_version)
-        identity.software_name = data.get("software-name")
-        identity.software_version = data.get("software-version")
-        version_scheme = data.get("version-scheme")
-        if version_scheme:
-            identity.version_scheme = _VERSION_SCHEME_FROM_STRING[version_scheme]
-
-        # optional metadata
-        for meta in _get_one_or_more(data, "software-meta"):
-            for attr_name, attrib_name in [
-                ("summary", "summary"),
-                ("revision", "revision"),
-                ("product", "product"),
-                ("edition", "edition"),
-                ("colloquial-version", "colloquial_version"),
-            ]:
-                if attr_name in meta:
-                    setattr(identity, attrib_name, meta[attr_name])
-
-        # entities
-        for node in _get_one_or_more(data, "entity"):
-            entity = uSwidEntity()
-            self._load_entity(entity, node)
-            identity.add_entity(entity)
-
-        # links
-        for node in _get_one_or_more(data, "links"):
-            link = uSwidLink()
-            self._load_link(link, node)
-            identity.add_link(link)
-
-        # payloads
-        for node in _get_one_or_more(data, "payload"):
-            for node_file in _get_one_or_more(node, "file"):
+        config = configparser.ConfigParser()
+        config.read_string(blob.decode())
+        for group in config.sections():
+            if group == "uSWID":
+                for key, value in config[group].items():
+                    if key == "tag-id":
+                        component.tag_id = value
+                    elif key == "tag-version":
+                        component.tag_version = int(value)
+                        component._auto_increment_tag_version = False
+                    elif key == "software-name":
+                        component.software_name = value
+                    elif key == "software-version":
+                        component.software_version = value
+                    elif key == "version-scheme":
+                        component.version_scheme = _VERSION_SCHEME_FROM_STRING[value]
+                    elif key == "summary":
+                        component.summary = value
+                    elif key == "revision":
+                        component.revision = value
+                    elif key == "product":
+                        component.product = value
+                    elif key == "edition":
+                        component.edition = value
+                    elif key == "colloquial-version":
+                        component.colloquial_version = value
+                    elif key == "persistent-id":
+                        component.persistent_id = value
+                    else:
+                        print(f"unknown key {key} found in ini file!")
+            if group.startswith("uSWID-Entity:"):
+                entity = uSwidEntity()
+                self._load_entity(entity, config[group], role_hint=group)
+                component.add_entity(entity)
+            if group.startswith("uSWID-Link"):
+                link = uSwidLink()
+                self._load_link(link, config[group])
+                component.add_link(link)
+            if group.startswith("uSWID-Payload"):
                 payload = uSwidPayload()
-                self._load_file(payload, node_file)
-                identity.add_payload(payload)
-            for node_directory in _get_one_or_more(node, "directory"):
-                for node_path_elements in _get_one_or_more(
-                    node_directory, "path_elements"
-                ):
-                    for node_file in _get_one_or_more(node_path_elements, "file"):
-                        payload = uSwidPayload()
-                        self._load_file(payload, node_file)
-                        identity.add_payload(payload)
-
-        # evidences
-        for node in _get_one_or_more(data, "evidence"):
-            evidence = uSwidEvidence()
-            self._load_evidence(evidence, node)
-            identity.add_evidence(evidence)
-
-    def _load_identity(self, identity: uSwidIdentity, blob: bytes) -> None:
-        """Imports a uSwidIdentity goSWID blob"""
-
-        try:
-            data: Dict[str, Any] = json.loads(blob)
-        except json.decoder.JSONDecodeError as e:
-            raise NotSupportedError("invalid goSWID: {}".format(e)) from e
-        self._load_identity_internal(identity, data)
+                self._load_payload(payload, config[group], path=path)
+                component.add_payload(payload)
+            if group.startswith("uSWID-Evidence"):
+                evidence = uSwidEvidence()
+                self._load_evidence(evidence, config[group])
+                component.add_evidence(evidence)
```

### Comparing `uswid-0.4.7/uswid/format_goswid.pyi` & `uswid-0.5.0/uswid/format_uswid.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+from .component import uSwidComponent as uSwidComponent
 from .container import uSwidContainer as uSwidContainer
-from .entity import uSwidEntity as uSwidEntity
+from .enums import USWID_HEADER_MAGIC as USWID_HEADER_MAGIC, uSwidHeaderFlags as uSwidHeaderFlags, uSwidPayloadCompression as uSwidPayloadCompression
 from .errors import NotSupportedError as NotSupportedError
-from .evidence import uSwidEvidence as uSwidEvidence
 from .format import uSwidFormatBase as uSwidFormatBase
-from .hash import uSwidHash as uSwidHash, uSwidHashAlg as uSwidHashAlg
-from .identity import uSwidIdentity as uSwidIdentity
-from .link import uSwidLink as uSwidLink
-from .payload import uSwidPayload as uSwidPayload
-from typing import Optional
+from .format_coswid import uSwidFormatCoswid as uSwidFormatCoswid
+from _typeshed import Incomplete
 
-class uSwidFormatGoswid(uSwidFormatBase):
-    def __init__(self) -> None: ...
-    def load(self, blob: bytes, path: Optional[str] = ...) -> uSwidContainer: ...
+class uSwidFormatUswid(uSwidFormatBase):
+    compression: Incomplete
+    def __init__(self, compress: bool = False, compression: uSwidPayloadCompression = ...) -> None: ...
+    @property
+    def compress(self) -> bool: ...
+    def load(self, blob: bytes, path: str | None = None) -> uSwidContainer: ...
     def save(self, container: uSwidContainer) -> bytes: ...
```

### Comparing `uswid-0.4.7/uswid/format_ini.pyi` & `uswid-0.5.0/uswid/format_goswid.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+from .component import uSwidComponent as uSwidComponent
 from .container import uSwidContainer as uSwidContainer
-from .entity import uSwidEntity as uSwidEntity, uSwidEntityRole as uSwidEntityRole
+from .entity import uSwidEntity as uSwidEntity
 from .errors import NotSupportedError as NotSupportedError
 from .evidence import uSwidEvidence as uSwidEvidence
 from .format import uSwidFormatBase as uSwidFormatBase
-from .hash import uSwidHash as uSwidHash
-from .identity import uSwidIdentity as uSwidIdentity
+from .hash import uSwidHash as uSwidHash, uSwidHashAlg as uSwidHashAlg
 from .link import uSwidLink as uSwidLink
 from .payload import uSwidPayload as uSwidPayload
-from typing import Optional
 
-class uSwidFormatIni(uSwidFormatBase):
+class uSwidFormatGoswid(uSwidFormatBase):
     def __init__(self) -> None: ...
-    def load(self, blob: bytes, path: Optional[str] = ...) -> uSwidContainer: ...
+    def load(self, blob: bytes, path: str | None = None) -> uSwidContainer: ...
     def save(self, container: uSwidContainer) -> bytes: ...
```

### Comparing `uswid-0.4.7/uswid/format_pkgconfig.py` & `uswid-0.5.0/uswid/format_pkgconfig.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
 # pylint: disable=too-few-public-methods,protected-access
 
 from typing import Optional
 
 import os
 
 from .container import uSwidContainer
 from .format import uSwidFormatBase
-from .identity import uSwidIdentity
+from .component import uSwidComponent
 from .entity import uSwidEntityRole
 
 _ENTITY_MAP_FROM_INI = {
     "TagCreator": uSwidEntityRole.TAG_CREATOR,
     "SoftwareCreator": uSwidEntityRole.SOFTWARE_CREATOR,
     "Aggregator": uSwidEntityRole.AGGREGATOR,
     "Distributor": uSwidEntityRole.DISTRIBUTOR,
@@ -39,38 +39,38 @@
 
     def __init__(self, filepath: Optional[str] = None) -> None:
         """Initializes uSwidFormatPkgconfig"""
         uSwidFormatBase.__init__(self)
         self.filepath: Optional[str] = filepath
 
     def load(self, blob: bytes, path: Optional[str] = None) -> uSwidContainer:
-        identity = uSwidIdentity()
-        self._load_identity(identity, blob)
-        return uSwidContainer([identity])
+        component = uSwidComponent()
+        self._load_component(component, blob)
+        return uSwidContainer([component])
 
-    def _load_identity(self, identity: uSwidIdentity, blob: bytes) -> None:
-        """Imports a pkg-conifg file as overrides to the uSwidIdentity data"""
+    def _load_component(self, component: uSwidComponent, blob: bytes) -> None:
+        """Imports a pkg-conifg file as overrides to the uSwidComponent data"""
 
         # filename base is the ID
         if self.filepath:
-            identity.tag_id = os.path.basename(self.filepath)
-            if identity.tag_id.endswith(".pc"):
-                identity.tag_id = identity.tag_id[:-3]
+            component.tag_id = os.path.basename(self.filepath)
+            if component.tag_id.endswith(".pc"):
+                component.tag_id = component.tag_id[:-3]
 
         # read out properties
         for line in blob.decode().split("\n"):
             try:
                 key, value = line.split(":", maxsplit=2)
             except ValueError:
                 continue
             if key == "Name":
-                identity.software_name = value.strip()
+                component.software_name = value.strip()
                 continue
             if key == "Description":
-                identity.summary = value.strip()
+                component.summary = value.strip()
                 continue
             if key == "Version":
-                identity.software_version = value.strip()
+                component.software_version = value.strip()
                 continue
             if key == "AppstreamId":
-                identity.persistent_id = value.strip()
+                component.persistent_id = value.strip()
                 continue
```

### Comparing `uswid-0.4.7/uswid/format_swid.py` & `uswid-0.5.0/uswid/format_goswid.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,326 +1,325 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
 # pylint: disable=too-few-public-methods,protected-access,too-many-boolean-expressions
 
-from typing import Dict, List, Optional
+from typing import Dict, Any, Optional, List
 
+import json
 from datetime import datetime
-from lxml import etree as ET
 
 from .container import uSwidContainer
 from .format import uSwidFormatBase
 from .errors import NotSupportedError
-from .identity import (
-    uSwidIdentity,
-    _VERSION_SCHEME_FROM_STRING,
+from .component import (
+    uSwidComponent,
     _VERSION_SCHEME_TO_STRING,
+    _VERSION_SCHEME_FROM_STRING,
 )
-from .entity import uSwidEntity, uSwidEntityRole
+from .entity import uSwidEntity
 from .link import uSwidLink
 from .hash import uSwidHash, uSwidHashAlg
 from .payload import uSwidPayload
 from .evidence import uSwidEvidence
+from .format_swid import _ENTITY_MAP_FROM_XML, _ENTITY_MAP_TO_XML
+
 
-_ENTITY_MAP_FROM_XML = {
-    "tagCreator": uSwidEntityRole.TAG_CREATOR,
-    "softwareCreator": uSwidEntityRole.SOFTWARE_CREATOR,
-    "aggregator": uSwidEntityRole.AGGREGATOR,
-    "distributor": uSwidEntityRole.DISTRIBUTOR,
-    "licensor": uSwidEntityRole.LICENSOR,
-    "maintainer": uSwidEntityRole.MAINTAINER,
-}
-_ENTITY_MAP_TO_XML = {
-    uSwidEntityRole.TAG_CREATOR: "tagCreator",
-    uSwidEntityRole.SOFTWARE_CREATOR: "softwareCreator",
-    uSwidEntityRole.AGGREGATOR: "aggregator",
-    uSwidEntityRole.DISTRIBUTOR: "distributor",
-    uSwidEntityRole.LICENSOR: "licensor",
-    uSwidEntityRole.MAINTAINER: "maintainer",
-}
+def _get_one_or_more(data: Dict[str, Any], key: str) -> List[Any]:
+    value = data.get(key, [])
+    if isinstance(value, list):
+        return value
+    return [value]
 
 
-class uSwidFormatSwid(uSwidFormatBase):
-    """SWID file"""
+class uSwidFormatGoswid(uSwidFormatBase):
+    """goSWID file"""
 
     def __init__(self) -> None:
-        """Initializes uSwidFormatSwid"""
+        """Initializes uSwidFormatGoswid"""
         uSwidFormatBase.__init__(self)
 
     def load(self, blob: bytes, path: Optional[str] = None) -> uSwidContainer:
-        identity = uSwidIdentity()
-        self._load_identity(identity, blob)
-        return uSwidContainer([identity])
+        try:
+            data = json.loads(blob)
+        except json.decoder.JSONDecodeError as e:
+            raise NotSupportedError(f"invalid GoSWID: {e}") from e
+        container = uSwidContainer()
+        if "corim_id" in data:
+            data = data["corim_tags"]
+        for component_json in data:
+            component = uSwidComponent()
+            self._load_component_internal(component, component_json)
+            container.merge(component)
+        return container
 
     def save(self, container: uSwidContainer) -> bytes:
-        identity = container.get_default()
-        if not identity:
-            raise NotSupportedError("cannot save when no default identity")
-        return self._save_identity(identity)
+        root = []
+        for component in container:
+            root.append(self._save_component_internal(component))
+        return json.dumps(root, indent=2).encode()
 
-    def _save_link(self, link: uSwidLink, root: ET.Element) -> None:
-        """Exports a uSwidLink SWID section"""
+    def _save_link(self, link: uSwidLink) -> Dict[str, str]:
+        """Exports a uSwidLink goSWID section"""
 
-        node = ET.SubElement(root, "Link")
+        node: Dict[str, str] = {}
         if link.href:
-            node.set("href", link.href)
+            node["href"] = link.href
         if link.rel:
-            node.set("rel", link.rel)
+            node["rel"] = link.rel
+        return node
 
-    def _save_payload(self, payload: uSwidPayload, root: ET.Element) -> None:
-        """Exports a uSwidHash SWID section"""
-        node = ET.SubElement(
-            root,
-            "File",
-            nsmap={
-                "SHA256": "http://www.w3.org/2001/04/xmlenc#sha256",
-                "SHA512": "http://www.w3.org/2001/04/xmlenc#sha512",
-            },
-        )
+    def _save_payload(self, payload: uSwidPayload) -> Dict[str, Any]:
+        """Exports a uSwidLink goSWID section"""
+
+        node: Dict[str, Any] = {}
         if payload.name:
-            node.set("name", payload.name)
+            node["fs-name"] = payload.name
         if payload.size:
-            node.set("size", str(payload.size))
-        for ihash in payload.hashes:
-            if ihash.alg_id == uSwidHashAlg.SHA256:
-                node.set("{http://www.w3.org/2001/04/xmlenc#sha256}hash", ihash.value)
-            elif ihash.alg_id == uSwidHashAlg.SHA512:
-                node.set("{http://www.w3.org/2001/04/xmlenc#sha512}hash", ihash.value)
-
-    def _save_evidence(self, evidence: uSwidEvidence, root: ET.Element) -> None:
-        """Exports a uSwidEvidence SWID section"""
-        node = ET.SubElement(
-            root,
-            "Evidence",
-        )
+            node["size"] = str(payload.size)
+        if payload.hashes:
+            node["hash"] = [payload.hashes[0].alg_id or 0, payload.hashes[0].value]
+        return {"file": [node]}
+
+    def _save_evidence(self, evidence: uSwidEvidence) -> Dict[str, Any]:
+        """Exports a uSwidLink goSWID section"""
+
+        node: Dict[str, str] = {}
         if evidence.date:
-            node.set("date", evidence.date.isoformat())
+            node["date"] = evidence.date.isoformat()
         if evidence.device_id:
-            node.set("deviceId", evidence.device_id)
+            node["device_id"] = evidence.device_id
+        return node
 
-    def _save_entity(self, entity: uSwidEntity, root: ET.Element) -> None:
-        """Exports a uSwidEntity SWID section"""
+    def _save_entity(self, entity: uSwidEntity) -> Dict[str, Any]:
+        """Exports a uSwidEntity goSWID section"""
 
-        node = ET.SubElement(root, "Entity")
+        node: Dict[str, Any] = {}
         if entity.name:
-            node.set("name", entity.name)
+            node["entity-name"] = entity.name
         if entity.regid:
-            node.set("regid", entity.regid)
-        roles: List[str] = []
+            node["reg-id"] = entity.regid
+        roles = []
         for role in entity.roles:
             try:
                 roles.append(_ENTITY_MAP_TO_XML[role])
             except KeyError as e:
                 raise NotSupportedError(
-                    "{} not supported from {}".format(
-                        role, ",".join(_ENTITY_MAP_TO_XML.values())
-                    )
+                    f"{role} not supported from {','.join(_ENTITY_MAP_TO_XML.values())}"
                 ) from e
-        if roles:
-            node.set("role", " ".join(roles))
-
-    def _save_identity(self, identity: uSwidIdentity) -> bytes:
-        """Exports a uSwidIdentity SWID blob"""
-
-        # identity
-        NSMAP = {
-            None: "http://standards.iso.org/iso/19770/-2/2015/schema.xsd",
-            "SHA256": "http://www.w3.org/2001/04/xmlenc#sha256",
-            "SHA512": "http://www.w3.org/2001/04/xmlenc#sha512",
-            "n8060": "http://csrc.nist.gov/ns/swid/2015-extensions/1.0",
-        }
-        root = ET.Element("SoftwareIdentity", nsmap=NSMAP)
-        if identity.lang:
-            root.attrib["{http://www.w3.org/XML/1998/namespace}lang"] = identity.lang
-        if identity.software_name:
-            root.set("name", identity.software_name)
-        if identity.tag_id:
-            root.set("tagId", identity.tag_id)
-        if identity.tag_version:
-            root.set("tagVersion", str(identity.tag_version))
-        if identity.software_version:
-            root.set("version", identity.software_version)
-        if identity.version_scheme:
-            root.set(
-                "versionScheme", _VERSION_SCHEME_TO_STRING[identity.version_scheme]
-            )
-
-        # entities
-        for entity in identity._entities.values():
-            self._save_entity(entity, root)
-        for link in identity._links.values():
-            self._save_link(link, root)
-
-        # payloads
-        if identity.payloads:
-            node = ET.SubElement(root, "Payload", nsmap=NSMAP)
-            node2 = ET.SubElement(node, "Directory", nsmap=NSMAP)
-            for payload in identity.payloads:
-                self._save_payload(payload, node2)
+        # use string if only one role
+        if len(roles) == 1:
+            node["role"] = roles[0]
+        else:
+            node["role"] = roles
+        return node
 
-        # evidences
-        if identity.evidences:
-            for evidence in identity.evidences:
-                self._save_evidence(evidence, root)
+    def _save_component_internal(self, component: uSwidComponent) -> Dict[str, Any]:
+        # component
+        root: Dict[str, Any] = {}
+        if component.lang:
+            root["lang"] = component.lang
+        if component.tag_id:
+            root["tag-id"] = component.tag_id
+        if component.tag_version:
+            root["tag-version"] = component.tag_version
+        if component.software_name:
+            root["software-name"] = component.software_name
+        if component.software_version:
+            root["software-version"] = component.software_version
+        if component.version_scheme:
+            root["version-scheme"] = _VERSION_SCHEME_TO_STRING[component.version_scheme]
 
         # optional metadata
         if (
-            identity.summary
-            or identity.revision
-            or identity.product
-            or identity.edition
-            or identity.colloquial_version
-            or identity.persistent_id
+            component.summary
+            or component.revision
+            or component.product
+            or component.edition
+            or component.colloquial_version
+            or component.persistent_id
         ):
-            node = ET.SubElement(root, "Meta")
-            if identity.revision:
-                node.set("revision", identity.revision)
-            if identity.product:
-                node.set("product", identity.product)
-            if identity.edition:
-                node.set("edition", identity.edition)
-            if identity.colloquial_version:
-                node.set("colloquialVersion", identity.colloquial_version)
-            if identity.persistent_id:
-                node.set("persistentId", identity.persistent_id)
+            node: Dict[str, str] = {}
+            if component.summary:
+                node["summary"] = component.summary
+            if component.revision:
+                node["revision"] = component.revision
+            if component.product:
+                node["product"] = component.product
+            if component.edition:
+                node["edition"] = component.edition
+            if component.colloquial_version:
+                node["colloquial-version"] = component.colloquial_version
+            if component.persistent_id:
+                node["persistent-id"] = component.persistent_id
+            # the CoSWID spec says: 'software-meta => one-or-more'
+            root["software-meta"] = [node]
+
+        # checksum
+        if component.payloads:
+            root["payload"] = []
+            for payload in component.payloads:
+                root["payload"].append(self._save_payload(payload))
+
+        # evidences
+        if component.evidences:
+            root["evidence"] = []
+            for evidence in component.evidences:
+                root["evidence"].append(self._save_evidence(evidence))
+
+        # entities
+        if component.entities:
+            root["entity"] = []
+            for entity in component.entities:
+                root["entity"].append(self._save_entity(entity))
+
+        # links
+        if component.links:
+            root["link"] = []
+            for link in component.links:
+                root["link"].append(self._save_link(link))
 
         # success
-        return ET.tostring(
-            root, encoding="utf-8", xml_declaration=True, pretty_print=True
+        return root
+
+    def _save_component(self, component: uSwidComponent) -> bytes:
+        """Exports a uSwidComponent goSWID blob"""
+        return json.dumps(self._save_component_internal(component), indent=2).encode(
+            "utf-8"
         )
 
-    def _load_link(self, link: uSwidLink, node: ET.SubElement) -> None:
-        """Imports a uSwidLink SWID section"""
+    def _load_link(self, link: uSwidLink, node: Dict[str, str]) -> None:
+        """Imports a uSwidLink goSWID section"""
 
-        LINK_MAP: Dict[str, str] = {
-            "seeAlso": "see-also",
-        }
         link.href = node.get("href")
-        rel_data = node.get("rel")
-        link.rel = LINK_MAP.get(rel_data, rel_data)
+        link.rel = node.get("rel")
 
-    def _load_payload(self, payload: uSwidPayload, node: ET.SubElement) -> None:
-        """Imports a uSwidPayload SWID section"""
-
-        payload.name = node.get("name")
-        try:
-            payload.size = int(node.get("size"))
-        except TypeError:
-            pass
-        try:
-            value = node.attrib["{http://www.w3.org/2001/04/xmlenc#sha256}hash"]
-            if value:
-                payload.add_hash(uSwidHash(alg_id=uSwidHashAlg.SHA256, value=value))
-        except KeyError:
-            pass
-        try:
-            value = node.attrib["{http://www.w3.org/2001/04/xmlenc#sha512}hash"]
-            if value:
-                payload.add_hash(uSwidHash(alg_id=uSwidHashAlg.SHA512, value=value))
-        except KeyError:
-            pass
-
-    def _load_evidence(self, evidence: uSwidEvidence, node: ET.SubElement) -> None:
-        """Imports a uSwidEvidence SWID section"""
+    def _load_evidence(self, evidence: uSwidEvidence, node: Dict[str, str]) -> None:
+        """Imports a uSwidEvidence goSWID section"""
 
         iso_date = node.get("date")
         if iso_date:
             evidence.date = datetime.fromisoformat(iso_date)
+        evidence.device_id = node.get("device_id")
+
+    def _load_file(self, payload: uSwidPayload, node: Dict[str, Any]) -> None:
+        """Imports a uSwidPayload goSWID section"""
+
+        # for compat with Intel FSP template
+        for key in list(node):
+            node[key.replace("_", "-")] = node.pop(key)
+
+        payload.name = node.get("fs-name")
         try:
-            evidence.device_id = node.get("deviceId")
-        except TypeError:
+            payload.size = int(node["size"])
+        except (ValueError, KeyError):
             pass
+        if "hash" in node:
+            ihash = uSwidHash()
+            # Intel FSP order is reversed
+            try:
+                ihash.alg_id = uSwidHashAlg(int(node["hash"][0]))
+                ihash.value = node["hash"][1]
+            except ValueError:
+                ihash.value = node["hash"][0]
+                ihash.alg_id = uSwidHashAlg(int(node["hash"][1]))
+            payload.add_hash(ihash)
 
     def _load_entity(
         self,
         entity: uSwidEntity,
-        node: ET.SubElement,
+        node: Dict[str, str],
     ) -> None:
-        """Imports a uSwidEntity SWID section"""
+        """Imports a uSwidEntity goSWID section"""
 
-        entity.name = node.get("name")
-        entity.regid = node.get("regid", None)
-        for role_str in node.get("role", "").split(" "):
+        # for compat with Intel FSP template
+        for key in list(node):
+            node[key.replace("_", "-")] = node.pop(key)
+
+        entity.name = node.get("entity-name")
+        entity.regid = node.get("reg-id")
+        roles = node.get("role")
+        if roles and isinstance(roles, str):
+            roles = [roles]  # type: ignore
+        for role_str in roles:  # type: ignore
             try:
                 entity.roles.append(_ENTITY_MAP_FROM_XML[role_str])
             except KeyError as e:
                 raise NotSupportedError(
-                    "{} not supported from {}".format(
-                        role_str, ",".join(_ENTITY_MAP_FROM_XML)
-                    )
+                    f"{role_str} not supported from {','.join(_ENTITY_MAP_FROM_XML)}"
                 ) from e
 
-    def _load_identity(self, identity: uSwidIdentity, blob: bytes) -> None:
-        """Imports a uSwidIdentity SWID blob"""
-
-        parser = ET.XMLParser()
-        tree = ET.fromstring(blob, parser)
-        namespaces = {
-            "ns": "http://standards.iso.org/iso/19770/-2/2015/schema.xsd",
-            "ds": "http://www.w3.org/2000/09/xmldsig#",
-            "SHA256": "http://www.w3.org/2001/04/xmlenc#sha256",
-            "SHA512": "http://www.w3.org/2001/04/xmlenc#sha512",
-        }
-
-        # strip off digital signature
-        if tree.xpath("/ds:Signature", namespaces=namespaces):
-            element = tree.xpath(
-                "/ds:Signature/ds:Object/ns:SoftwareIdentity", namespaces=namespaces
-            )[0]
-        else:
-            element = tree.xpath("/ns:SoftwareIdentity", namespaces=namespaces)[0]
-
-        # identity
-        identity.tag_id = element.get("tagId")
-        identity.tag_version = element.get("tagVersion")
-        identity.software_name = element.get("name")
-        identity.software_version = element.get("version")
-        try:
-            identity.version_scheme = _VERSION_SCHEME_FROM_STRING[
-                element.get("versionScheme")
-            ]
-        except KeyError:
-            identity.version_scheme = None
+    def _load_component_internal(
+        self, component: uSwidComponent, data: Dict[str, Any]
+    ) -> None:
+        # for compat with Intel FSP template
+        for key in list(data):
+            data[key.replace("_", "-")] = data.pop(key)
+
+        # component
+        component.tag_id = data.get("tag-id")
+        tag_version = data.get("tag-version")
+        if tag_version:
+            component.tag_version = int(tag_version)
+        component.software_name = data.get("software-name")
+        component.software_version = data.get("software-version")
+        version_scheme = data.get("version-scheme")
+        if version_scheme:
+            component.version_scheme = _VERSION_SCHEME_FROM_STRING[version_scheme]
 
         # optional metadata
-        for meta in element.xpath("ns:Meta", namespaces=namespaces):
+        for meta in _get_one_or_more(data, "software-meta"):
             for attr_name, attrib_name in [
                 ("summary", "summary"),
                 ("revision", "revision"),
                 ("product", "product"),
                 ("edition", "edition"),
-                ("colloquialVersion", "colloquial_version"),
-                ("persistentId", "persistent_id"),
+                ("colloquial-version", "colloquial_version"),
             ]:
-                if attr_name in meta.attrib:
-                    setattr(identity, attrib_name, meta.attrib[attr_name])
+                if attr_name in meta:
+                    setattr(component, attrib_name, meta[attr_name])
 
         # entities
-        for node in element.xpath("ns:Entity", namespaces=namespaces):
+        for node in _get_one_or_more(data, "entity"):
             entity = uSwidEntity()
             self._load_entity(entity, node)
-            identity.add_entity(entity)
+            component.add_entity(entity)
 
         # links
-        for node in element.xpath("ns:Link", namespaces=namespaces):
+        for node in _get_one_or_more(data, "links"):
             link = uSwidLink()
             self._load_link(link, node)
-            identity.add_link(link)
+            component.add_link(link)
 
         # payloads
-        for node in element.xpath(
-            "ns:Payload/ns:Directory/ns:File", namespaces=namespaces
-        ):
-            payload = uSwidPayload()
-            self._load_payload(payload, node)
-            identity.add_payload(payload)
+        for node in _get_one_or_more(data, "payload"):
+            for node_file in _get_one_or_more(node, "file"):
+                payload = uSwidPayload()
+                self._load_file(payload, node_file)
+                component.add_payload(payload)
+            for node_directory in _get_one_or_more(node, "directory"):
+                for node_path_elements in _get_one_or_more(
+                    node_directory, "path_elements"
+                ):
+                    for node_file in _get_one_or_more(node_path_elements, "file"):
+                        payload = uSwidPayload()
+                        self._load_file(payload, node_file)
+                        component.add_payload(payload)
 
         # evidences
-        for node in element.xpath("ns:Evidence", namespaces=namespaces):
+        for node in _get_one_or_more(data, "evidence"):
             evidence = uSwidEvidence()
             self._load_evidence(evidence, node)
-            identity.add_evidence(evidence)
+            component.add_evidence(evidence)
+
+    def _load_component(self, component: uSwidComponent, blob: bytes) -> None:
+        """Imports a uSwidComponent goSWID blob"""
+
+        try:
+            data: Dict[str, Any] = json.loads(blob)
+        except json.decoder.JSONDecodeError as e:
+            raise NotSupportedError(f"invalid goSWID: {e}") from e
+        self._load_component_internal(component, data)
```

### Comparing `uswid-0.4.7/uswid/format_swid.pyi` & `uswid-0.5.0/uswid/format_ini.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+from .component import uSwidComponent as uSwidComponent
 from .container import uSwidContainer as uSwidContainer
 from .entity import uSwidEntity as uSwidEntity, uSwidEntityRole as uSwidEntityRole
 from .errors import NotSupportedError as NotSupportedError
 from .evidence import uSwidEvidence as uSwidEvidence
 from .format import uSwidFormatBase as uSwidFormatBase
-from .hash import uSwidHash as uSwidHash, uSwidHashAlg as uSwidHashAlg
-from .identity import uSwidIdentity as uSwidIdentity
+from .hash import uSwidHash as uSwidHash
 from .link import uSwidLink as uSwidLink
 from .payload import uSwidPayload as uSwidPayload
-from typing import Optional
 
-class uSwidFormatSwid(uSwidFormatBase):
+class uSwidFormatIni(uSwidFormatBase):
     def __init__(self) -> None: ...
-    def load(self, blob: bytes, path: Optional[str] = ...) -> uSwidContainer: ...
+    def load(self, blob: bytes, path: str | None = None) -> uSwidContainer: ...
     def save(self, container: uSwidContainer) -> bytes: ...
```

### Comparing `uswid-0.4.7/uswid/format_uswid.py` & `uswid-0.5.0/uswid/format_uswid.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
 # pylint: disable=too-few-public-methods,protected-access
 
 from typing import Optional
 
 import struct
 import zlib
 import lzma
 
 from .enums import USWID_HEADER_MAGIC, uSwidHeaderFlags, uSwidPayloadCompression
 from .container import uSwidContainer
 from .format import uSwidFormatBase
 from .errors import NotSupportedError
-from .identity import uSwidIdentity
+from .component import uSwidComponent
 from .format_coswid import uSwidFormatCoswid
 
 
 class uSwidFormatUswid(uSwidFormatBase):
     """uSWID file"""
 
     def __init__(
         self,
-        compress: bool = True,
+        compress: bool = False,
         compression: uSwidPayloadCompression = uSwidPayloadCompression.NONE,
     ) -> None:
         """Initializes uSwidFormatUswid"""
         uSwidFormatBase.__init__(self)
         self.compression: uSwidPayloadCompression = compression
         if self.compression == uSwidPayloadCompression.NONE and compress:
             self.compression = uSwidPayloadCompression.ZLIB
@@ -46,25 +46,25 @@
         # find magic GUIDs marking external uSWID sections
         offset: int = 0
         cnt: int = 0
         while 1:
             offset = blob.find(USWID_HEADER_MAGIC, offset)
             if offset == -1:
                 break
-            print("Found USWID header at offset: {}".format(offset))
+            print(f"Found USWID header at offset: {offset}")
             offset += self._load_bytes(container, blob, offset)
             cnt += 1
         if cnt == 0:
             raise NotSupportedError("file does not have expected magic GUID")
         return container
 
     def save(self, container: uSwidContainer) -> bytes:
         blob: bytes = b""
-        for identity in container:
-            blob += uSwidFormatCoswid()._save_identity(identity)
+        for component in container:
+            blob += uSwidFormatCoswid()._save_component(component)
 
         # v3 header specifies the compression type
         if self.compression == uSwidPayloadCompression.LZMA:
             payload = lzma.compress(blob, preset=9)
             return (
                 struct.pack(
                     "<16sBHIBB",
@@ -145,15 +145,15 @@
             payload = zlib.decompress(payload)
         elif self.compression == uSwidPayloadCompression.LZMA:
             payload = lzma.decompress(payload)
 
         # read each CBOR blob
         payload_offset = 0
         while payload_offset < len(payload):
-            identity = uSwidIdentity()
-            payload_offset += uSwidFormatCoswid()._load_identity(
-                identity, payload, payload_offset
+            component = uSwidComponent()
+            payload_offset += uSwidFormatCoswid()._load_component(
+                component, payload, payload_offset
             )
-            container.append(identity)
+            container.append(component)
 
         # consumed
         return hdrsz + payloadsz
```

### Comparing `uswid-0.4.7/uswid/hash.py` & `uswid-0.5.0/uswid/hash.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2023 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
 # pylint: disable=too-few-public-methods
 
 from enum import IntEnum
 
 from typing import Optional
 
@@ -16,23 +16,26 @@
     """Represents an enumerated type of hash"""
 
     UNKNOWN = 0
     SHA256 = 1
     SHA384 = 7
     SHA512 = 8
 
+    def __str__(self):
+        return self.name.lower()
+
     @classmethod
     def from_string(cls, alg_id: str) -> "uSwidHashAlg":
         """Creates a uSwidHashAlg from a string identifier"""
         return cls(
             {
                 "SHA256": uSwidHashAlg.SHA256,
                 "SHA384": uSwidHashAlg.SHA384,
                 "SHA512": uSwidHashAlg.SHA512,
-            }[alg_id]
+            }[alg_id.replace("-", "").upper()]
         )
 
 
 class uSwidHash:
     """Represents a SWID link"""
 
     def __init__(
```

### Comparing `uswid-0.4.7/uswid/identity.pyi` & `uswid-0.5.0/uswid/component.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 from .entity import uSwidEntity as uSwidEntity, uSwidEntityRole as uSwidEntityRole
 from .enums import uSwidVersionScheme as uSwidVersionScheme
 from .errors import NotSupportedError as NotSupportedError
 from .evidence import uSwidEvidence as uSwidEvidence
 from .link import uSwidLink as uSwidLink, uSwidLinkRel as uSwidLinkRel
 from .payload import uSwidPayload as uSwidPayload
 from .problem import uSwidProblem as uSwidProblem
+from .vex_statement import uSwidVexStatement as uSwidVexStatement
 from _typeshed import Incomplete
-from typing import List, Optional
 
-class uSwidIdentity:
+class uSwidComponent:
     tag_version: Incomplete
     software_version: Incomplete
     version_scheme: Incomplete
     summary: Incomplete
     product: Incomplete
     colloquial_version: Incomplete
     revision: Incomplete
     edition: Incomplete
     persistent_id: Incomplete
     lang: str
     generator: Incomplete
     payloads: Incomplete
     evidences: Incomplete
-    def __init__(self, tag_id: Optional[str] = ..., tag_version: int = ..., software_name: Optional[str] = ..., software_version: Optional[str] = ..., generator: Optional[str] = ...) -> None: ...
+    vex_statements: Incomplete
+    def __init__(self, tag_id: str | None = None, tag_version: int = 0, software_name: str | None = None, software_version: str | None = None, generator: str | None = 'uSWID') -> None: ...
     @property
-    def software_name(self) -> Optional[str]: ...
+    def software_name(self) -> str | None: ...
+    @software_name.setter
+    def software_name(self, software_name: str | None) -> None: ...
     @property
-    def generator_href(self) -> Optional[str]: ...
+    def generator_href(self) -> str | None: ...
     @property
-    def tag_id(self) -> Optional[str]: ...
-    def problems(self) -> List[uSwidProblem]: ...
-    def merge(self, identity_new: uSwidIdentity) -> None: ...
+    def tag_id(self) -> str | None: ...
+    @tag_id.setter
+    def tag_id(self, tag_id: str | None) -> None: ...
+    def problems(self) -> list[uSwidProblem]: ...
+    def add_vex_statement(self, vex_statement: uSwidVexStatement) -> None: ...
+    def merge(self, component_new: uSwidComponent) -> None: ...
     def add_entity(self, entity: uSwidEntity) -> None: ...
     def add_link(self, link: uSwidLink) -> None: ...
     def add_payload(self, payload: uSwidPayload) -> None: ...
     def add_evidence(self, evidence: uSwidEvidence) -> None: ...
     @property
-    def links(self) -> List[uSwidLink]: ...
+    def links(self) -> list[uSwidLink]: ...
     @property
-    def entities(self) -> List[uSwidEntity]: ...
+    def entities(self) -> list[uSwidEntity]: ...
```

### Comparing `uswid-0.4.7/uswid/link.py` & `uswid-0.5.0/uswid/link.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
 # pylint: disable=too-few-public-methods
 
 from enum import IntEnum
 import uuid
 
 from typing import List, Optional, TYPE_CHECKING
 
 from .problem import uSwidProblem
 
 if TYPE_CHECKING:
-    from .identity import uSwidIdentity
+    from .component import uSwidComponent
 
 
 class uSwidLinkRel(IntEnum):
     """Represents an enumerated types of link"""
 
     LICENSE = -2
     COMPILER = -1
@@ -31,28 +31,31 @@
     PARENT = 6
     PATCHES = 7
     REQUIRES = 8
     SEE_ALSO = 9
     SUPERSEDES = 10
     SUPPLEMENTAL = 11
 
+    def __str__(self):
+        return self.name.lower()
+
 
 class uSwidLink:
     """Represents a SWID link"""
 
     def __init__(
         self,
         href: Optional[str] = None,
         rel: Optional[str] = None,
     ):
         """Initializes uSwidLink"""
         self._href: Optional[str] = href
         self._rel: Optional[str] = rel
-        self.identity: Optional[uSwidIdentity] = None
-        """Identity, if the SWID reference in internally resolvable"""
+        self.component: Optional[uSwidComponent] = None
+        """Component, if the SWID reference in internally resolvable"""
 
     @property
     def rel(self) -> Optional[str]:
         """Returns rel, guessing from the ``href`` if not provided"""
         if not self._rel:
             if self.href and self.href.startswith("swid"):
                 return "component"
@@ -89,14 +92,16 @@
         return self.href.split("/")[-1].replace(".html", "")
 
     def problems(self) -> List[uSwidProblem]:
         """Checks the link for common problems"""
 
         problems: List[uSwidProblem] = []
         if not self.href:
-            problems += uSwidProblem("link", "No href", since="0.4.7")
+            problems += [uSwidProblem("link", "No href", since="0.4.7")]
+        elif self.href.find("REDACTED") != -1:
+            problems += [uSwidProblem("link", "Redacted href", since="0.4.8")]
         if not self.rel:
-            problems += uSwidProblem("link", "No rel", since="0.4.7")
+            problems += [uSwidProblem("link", "No rel", since="0.4.7")]
         return problems
 
     def __repr__(self) -> str:
         return f'uSwidLink(rel="{self.rel or "none"}",href="{self.href}")'
```

### Comparing `uswid-0.4.7/uswid/payload.py` & `uswid-0.5.0/uswid/payload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2023 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
 # pylint: disable=too-few-public-methods
 
 from typing import Optional, List, Dict
 
 import hashlib
 
@@ -52,14 +52,16 @@
         m.update(buf)
         self.add_hash(uSwidHash(alg_id=uSwidHashAlg.SHA256, value=m.hexdigest()))
 
     def problems(self) -> List[uSwidProblem]:
         """Checks the payload for common problems"""
 
         problems: List[uSwidProblem] = []
+        if self.name and self.name.find("REDACTED") != -1:
+            problems += [uSwidProblem("payload", "Redacted name", since="0.4.8")]
         if not self.size:
             problems += [
                 uSwidProblem("payload", f"No size in {self.name}", since="0.4.7")
             ]
         if not self.hashes:
             problems += [
                 uSwidProblem("payload", f"No hashes in {self.name}", since="0.4.7")
```

### Comparing `uswid-0.4.7/uswid/payload.pyi` & `uswid-0.5.0/uswid/payload.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from .hash import uSwidHash as uSwidHash, uSwidHashAlg as uSwidHashAlg
 from .problem import uSwidProblem as uSwidProblem
 from _typeshed import Incomplete
-from typing import List, Optional
 
 class uSwidPayload:
     name: Incomplete
     size: Incomplete
-    def __init__(self, name: Optional[str] = ..., size: Optional[int] = ...) -> None: ...
+    def __init__(self, name: str | None = None, size: int | None = None) -> None: ...
     def add_hash(self, ihash: uSwidHash) -> None: ...
     def remove_hash(self, alg_id: uSwidHashAlg) -> None: ...
     @property
-    def hashes(self) -> List[uSwidHash]: ...
+    def hashes(self) -> list[uSwidHash]: ...
     def ensure_from_filename(self, fn: str) -> None: ...
-    def problems(self) -> List[uSwidProblem]: ...
+    def problems(self) -> list[uSwidProblem]: ...
```

### Comparing `uswid-0.4.7/uswid/problem.py` & `uswid-0.5.0/uswid/problem.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2023 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
 # pylint: disable=too-few-public-methods
 
 
 class uSwidProblem:
-    """Represents a SWID identity problem"""
+    """Represents a SWID component problem"""
 
     def __init__(
         self,
         kind: str,
         description: str,
         since: str,
     ):
```

### Comparing `uswid-0.4.7/uswid/test_uswid.py` & `uswid-0.5.0/uswid/test_uswid.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/python3
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Richard Hughes <richard@hughsie.com>
 #
-# SPDX-License-Identifier: LGPL-2.1+
+# SPDX-License-Identifier: BSD-2-Clause-Patent
 #
 # pylint: disable=wrong-import-position,protected-access
 
 import os
 import sys
 import unittest
 from lxml import etree as ET
@@ -16,27 +16,29 @@
 sys.path.append(os.path.realpath("."))
 
 from .container import uSwidContainer
 from .errors import NotSupportedError
 from .link import uSwidLink
 from .entity import uSwidEntity, uSwidEntityRole
 from .enums import uSwidVersionScheme
-from .identity import uSwidIdentity
+from .component import uSwidComponent
 from .hash import uSwidHash, uSwidHashAlg
 from .payload import uSwidPayload
 
 from .format_ini import uSwidFormatIni
 from .format_coswid import uSwidFormatCoswid
 from .format_swid import uSwidFormatSwid
 from .format_cyclonedx import uSwidFormatCycloneDX
 from .format_spdx import uSwidFormatSpdx
 
+from .purl import uSwidPurl
+
 
 class TestSwidEntity(unittest.TestCase):
-    """Tescases for identities, entities, links, evidence and payloads"""
+    """Tescases for components, entities, links, evidence and payloads"""
 
     def test_entity(self):
         """Unit tests for uSwidEntity"""
         entity = uSwidEntity(
             name="test", regid="example.com", roles=[uSwidEntityRole.MAINTAINER]
         )
         self.assertEqual(
@@ -220,35 +222,35 @@
             b"<SoftwareIdentity>"
             b'<File xmlns:SHA256="http://www.w3.org/2001/04/xmlenc#sha256" '
             b'xmlns:SHA512="http://www.w3.org/2001/04/xmlenc#sha512" name="foo" size="123" '
             b'SHA256:hash="8cab6b2125c2b561351b4e02ee531f26dde05c3c6a2be8ff942975fbdef6823c"/>'
             b"</SoftwareIdentity>",
         )
 
-    def test_identity(self):
-        """Unit tests for uSwidIdentity"""
+    def test_component(self):
+        """Unit tests for uSwidComponent"""
         self.maxDiff = None
-        identity = uSwidIdentity(
+        component = uSwidComponent(
             tag_id="foobarbaz",
             tag_version=5,
             software_name="foo",
             software_version="1.2.3",
         )
-        identity.version_scheme = uSwidVersionScheme.MULTIPARTNUMERIC
+        component.version_scheme = uSwidVersionScheme.MULTIPARTNUMERIC
         self.assertEqual(
-            str(identity),
-            'uSwidIdentity(tag_id="foobarbaz",tag_version="5",software_name="foo",software_version="1.2.3")',
+            str(component),
+            'uSwidComponent(tag_id="foobarbaz",tag_version="5",software_name="foo",software_version="1.2.3")',
         )
         entity = uSwidEntity(
             name="test", regid="example.com", roles=[uSwidEntityRole.MAINTAINER]
         )
-        identity.add_entity(entity)
+        component.add_entity(entity)
         self.assertEqual(
-            str(identity),
-            'uSwidIdentity(tag_id="foobarbaz",tag_version="5",software_name="foo",software_version="1.2.3"):\n'
+            str(component),
+            'uSwidComponent(tag_id="foobarbaz",tag_version="5",software_name="foo",software_version="1.2.3"):\n'
             ' - uSwidEntity(regid="example.com",name="test",roles=MAINTAINER)',
         )
 
         # SWID XML import
         xml = b"""<?xml version='1.0' encoding='UTF-8'?>
 <SoftwareIdentity name="DellBiosConnectNetwork"
 tagId="acbd84ff-9898-4922-8ade-dd4bbe2e40ba" tagVersion="1" version="1.5.2"
@@ -259,30 +261,30 @@
 xmlns:n8060="http://csrc.nist.gov/ns/swid/2015-extensions/1.0">
 <Entity name="Dell Technologies" regid="dell.com" role="softwareCreator tagCreator" />
 <Link rel="seeAlso" href="http://hughsie.com"/>
 <Link rel="license" href="www.gnu.org/licenses/gpl.txt"/>
 <Meta product="Fedora" colloquialVersion="29" persistentId="org.hughski.colorhug"
   summary="Linux distribution developed by the community-supported Fedora Project" />
 </SoftwareIdentity>"""
-        identity = uSwidFormatSwid().load(xml).get_default()  # type: ignore
+        component = uSwidFormatSwid().load(xml).get_default()  # type: ignore
         self.assertEqual(
-            str(identity),
-            'uSwidIdentity(tag_id="acbd84ff-9898-4922-8ade-dd4bbe2e40ba",tag_version="1",'
+            str(component),
+            'uSwidComponent(tag_id="acbd84ff-9898-4922-8ade-dd4bbe2e40ba",tag_version="1",'
             'software_name="DellBiosConnectNetwork",software_version="1.5.2"):\n'
             ' - uSwidLink(rel="see-also",href="http://hughsie.com")\n'
             ' - uSwidLink(rel="license",href="www.gnu.org/licenses/gpl.txt")\n'
             ' - uSwidEntity(regid="dell.com",name="Dell Technologies",roles=SOFTWARE_CREATOR,TAG_CREATOR)',
         )
         self.assertEqual(
-            identity.summary,
+            component.summary,
             "Linux distribution developed by the community-supported Fedora Project",
         )
-        self.assertEqual(identity.product, "Fedora")
-        self.assertEqual(identity.colloquial_version, "29")
-        self.assertEqual(identity.persistent_id, "org.hughski.colorhug")
+        self.assertEqual(component.product, "Fedora")
+        self.assertEqual(component.colloquial_version, "29")
+        self.assertEqual(component.persistent_id, "org.hughski.colorhug")
 
         # INI import
         ini = """[uSWID]
 tag-id = acbd84ff-9898-4922-8ade-dd4bbe2e40ba
 tag-version = 1
 software-name = HughskiColorHug.efi
 software-version = 1.0.0
@@ -297,35 +299,35 @@
 regid = hughski.com
 extra-roles = Aggregator
 
 [uSWID-Link:ANYTHING]
 href = https://hughski.com/
 rel = see-also
 """
-        identity = uSwidFormatIni().load(ini.encode()).get_default()  # type: ignore
-        self.assertIsNotNone(identity)
+        component = uSwidFormatIni().load(ini.encode()).get_default()  # type: ignore
+        self.assertIsNotNone(component)
         self.assertEqual(
-            str(identity),
-            'uSwidIdentity(tag_id="acbd84ff-9898-4922-8ade-dd4bbe2e40ba",tag_version="1",'
+            str(component),
+            'uSwidComponent(tag_id="acbd84ff-9898-4922-8ade-dd4bbe2e40ba",tag_version="1",'
             'software_name="HughskiColorHug.efi",software_version="1.0.0"):\n'
             ' - uSwidLink(rel="see-also",href="https://hughski.com/")\n'
             ' - uSwidEntity(regid="hughsie.com",name="Richard Hughes",roles=TAG_CREATOR)\n'
             ' - uSwidEntity(regid="hughski.com",name="Hughski Limited",roles=AGGREGATOR)',
         )
 
         # INI export
-        tmp = uSwidFormatIni().save(uSwidContainer([identity])).decode()
+        tmp = uSwidFormatIni().save(uSwidContainer([component])).decode()
         assert "uSWID" in tmp
         assert "uSWID-Entity" in tmp
         assert "uSWID-Link" in tmp
 
         # SWID XML export
-        identity.colloquial_version = "22905301d08e69473393d94c3e787e4bf0453268"
+        component.colloquial_version = "22905301d08e69473393d94c3e787e4bf0453268"
         self.assertEqual(
-            uSwidFormatSwid().save(uSwidContainer([identity])),
+            uSwidFormatSwid().save(uSwidContainer([component])),
             b"<?xml version='1.0' encoding='utf-8'?>\n"
             b"<SoftwareIdentity "
             b'xmlns="http://standards.iso.org/iso/19770/-2/2015/schema.xsd" '
             b'xmlns:SHA256="http://www.w3.org/2001/04/xmlenc#sha256" '
             b'xmlns:SHA512="http://www.w3.org/2001/04/xmlenc#sha512" '
             b'xmlns:n8060="http://csrc.nist.gov/ns/swid/2015-extensions/1.0" '
             b'xml:lang="en-US" name="HughskiColorHug.efi" tagId="acbd84ff-9898-4922-8ade-dd4bbe2e40ba" '
@@ -335,21 +337,55 @@
             b'  <Link href="https://hughski.com/" rel="see-also"/>\n'
             b'  <Meta colloquialVersion="22905301d08e69473393d94c3e787e4bf0453268" '
             b'persistentId="org.hughski.colorhug"/>\n'
             b"</SoftwareIdentity>\n",
         )
 
         # CycloneDX export
-        tmp = uSwidFormatCycloneDX().save(uSwidContainer([identity])).decode()
+        tmp = uSwidFormatCycloneDX().save(uSwidContainer([component])).decode()
         assert "CycloneDX" in tmp
         assert "uSWID" in tmp
         assert "org.hughski.colorhug" in tmp
         assert "22905301d08e69473393d94c3e787e4bf0453268" in tmp
 
         # SPDX export
-        tmp = uSwidFormatSpdx().save(uSwidContainer([identity])).decode()
+        tmp = uSwidFormatSpdx().save(uSwidContainer([component])).decode()
         assert "SPDX" in tmp
         assert "uSWID" in tmp
 
+    def test_parse(self):
+        """Unit tests for parsing PURL text"""
+        purl = uSwidPurl("pkg:protocol/namespace/name@version?qualifiers#subpath")
+        self.assertEqual(purl.scheme, "pkg")
+        self.assertEqual(purl.protocol, "protocol")
+        self.assertEqual(purl.namespace, "namespace")
+        self.assertEqual(purl.name, "name")
+        self.assertEqual(purl.version, "version")
+        self.assertEqual(purl.qualifiers, "qualifiers")
+        self.assertEqual(purl.subpath, "subpath")
+
+        purl = uSwidPurl("pkg:protocol/name")
+        self.assertEqual(purl.scheme, "pkg")
+        self.assertEqual(purl.protocol, "protocol")
+        self.assertEqual(purl.name, "name")
+
+        purl = uSwidPurl("pkg:protocol/name@version")
+        self.assertEqual(purl.scheme, "pkg")
+        self.assertEqual(purl.protocol, "protocol")
+        self.assertEqual(purl.namespace, None)
+        self.assertEqual(purl.name, "name")
+        self.assertEqual(purl.version, "version")
+        self.assertEqual(purl.qualifiers, None)
+        self.assertEqual(purl.subpath, None)
+
+        purl = uSwidPurl("pkg:bcbd84ff-9898-4922-8ade-dd4bbe2e40ba@20230808")
+        self.assertEqual(purl.scheme, "pkg")
+        self.assertEqual(purl.protocol, None)
+        self.assertEqual(purl.namespace, None)
+        self.assertEqual(purl.name, "bcbd84ff-9898-4922-8ade-dd4bbe2e40ba")
+        self.assertEqual(purl.version, "20230808")
+        self.assertEqual(purl.qualifiers, None)
+        self.assertEqual(purl.subpath, None)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `uswid-0.4.7/uswid.egg-info/PKG-INFO` & `uswid-0.5.0/uswid.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: uswid
-Version: 0.4.7
+Version: 0.5.0
 Summary: A pure-python library for embedding CoSWID data
 Home-page: https://github.com/hughsie/python-uswid
 Author: Richard Hughes
 Author-email: richard@hughsie.com
-License: LGPL-2.1-or-later
+License: BSD-2-Clause-Patent
 Keywords: swid,sbom,coswid
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Archiving
 License-File: LICENSE
 Requires-Dist: cbor2
 Requires-Dist: lxml
 Requires-Dist: pefile
```

### Comparing `uswid-0.4.7/uswid.egg-info/SOURCES.txt` & `uswid-0.5.0/uswid.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 LICENSE
 README.md
 setup.py
 uswid/__init__.py
 uswid/__init__.pyi
 uswid/cli.py
+uswid/cli.pyi
+uswid/component.py
+uswid/component.pyi
 uswid/container.py
+uswid/container.pyi
 uswid/entity.py
 uswid/entity.pyi
 uswid/enums.py
 uswid/enums.pyi
 uswid/errors.py
 uswid/errors.pyi
 uswid/evidence.py
@@ -20,32 +24,39 @@
 uswid/format_cyclonedx.py
 uswid/format_cyclonedx.pyi
 uswid/format_goswid.py
 uswid/format_goswid.pyi
 uswid/format_ini.py
 uswid/format_ini.pyi
 uswid/format_pkgconfig.py
+uswid/format_pkgconfig.pyi
 uswid/format_spdx.py
 uswid/format_spdx.pyi
 uswid/format_swid.py
 uswid/format_swid.pyi
 uswid/format_uswid.py
 uswid/format_uswid.pyi
 uswid/hash.py
 uswid/hash.pyi
-uswid/identity.py
-uswid/identity.pyi
 uswid/link.py
 uswid/link.pyi
 uswid/payload.py
 uswid/payload.pyi
 uswid/problem.py
 uswid/problem.pyi
+uswid/purl.py
+uswid/purl.pyi
 uswid/py.typed
 uswid/test_uswid.py
+uswid/vex_document.py
+uswid/vex_document.pyi
+uswid/vex_product.py
+uswid/vex_product.pyi
+uswid/vex_statement.py
+uswid/vex_statement.pyi
 uswid.egg-info/PKG-INFO
 uswid.egg-info/SOURCES.txt
 uswid.egg-info/dependency_links.txt
 uswid.egg-info/entry_points.txt
 uswid.egg-info/not-zip-safe
 uswid.egg-info/requires.txt
 uswid.egg-info/top_level.txt
```

