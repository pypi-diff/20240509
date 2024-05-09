# Comparing `tmp/mcbcdc-0.12.tar.gz` & `tmp/mcbcdc-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcbcdc-0.12.tar", last modified: Wed May  8 21:20:33 2024, max compression
+gzip compressed data, was "mcbcdc-0.8.tar", last modified: Tue Apr 30 07:31:01 2024, max compression
```

## Comparing `mcbcdc-0.12.tar` & `mcbcdc-0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 21:20:33.951900 mcbcdc-0.12/
--rw-rw-rw-   0        0        0       38 2024-05-08 21:17:34.000000 mcbcdc-0.12/MANIFEST.in
--rw-rw-rw-   0        0        0      146 2024-05-08 21:20:33.950898 mcbcdc-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-08 21:20:33.910539 mcbcdc-0.12/data/
--rw-rw-rw-   0        0        0     1367 2024-05-08 03:35:28.000000 mcbcdc-0.12/data/facebook.txt
--rw-rw-rw-   0        0        0     4820 2024-05-08 20:21:15.000000 mcbcdc-0.12/data/hadoop.txt
--rw-rw-rw-   0        0        0     2321 2024-05-08 04:32:12.000000 mcbcdc-0.12/data/heart.txt
--rw-rw-rw-   0        0        0     1048 2024-05-08 20:07:23.000000 mcbcdc-0.12/data/hive.txt
--rw-rw-rw-   0        0        0      842 2024-05-08 05:59:44.000000 mcbcdc-0.12/data/tableau.txt
--rw-rw-rw-   0        0        0      777 2024-05-08 15:17:29.000000 mcbcdc-0.12/data/web.txt
--rw-rw-rw-   0        0        0     1023 2024-05-08 20:42:14.000000 mcbcdc-0.12/data/web1.txt
-drwxrwxrwx   0        0        0        0 2024-05-08 21:20:33.895298 mcbcdc-0.12/file/
--rw-rw-rw-   0        0        0        0 2024-05-08 21:17:36.000000 mcbcdc-0.12/file/__init__.py
--rw-rw-rw-   0        0        0      313 2024-05-08 21:17:36.000000 mcbcdc-0.12/file/file2.py
-drwxrwxrwx   0        0        0        0 2024-05-08 21:20:33.946897 mcbcdc-0.12/mcbcdc.egg-info/
--rw-rw-rw-   0        0        0      146 2024-05-08 21:20:33.000000 mcbcdc-0.12/mcbcdc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2024-05-08 21:20:33.000000 mcbcdc-0.12/mcbcdc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 21:20:33.000000 mcbcdc-0.12/mcbcdc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-08 21:20:33.000000 mcbcdc-0.12/mcbcdc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 21:20:33.952899 mcbcdc-0.12/setup.cfg
--rw-rw-rw-   0        0        0      422 2024-05-08 21:20:29.000000 mcbcdc-0.12/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:31:01.671441 mcbcdc-0.8/
+-rw-rw-rw-   0        0        0       42 2023-11-20 18:26:19.000000 mcbcdc-0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      145 2024-04-30 07:31:01.668439 mcbcdc-0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-30 07:31:01.627772 mcbcdc-0.8/data/
+-rw-rw-rw-   0        0        0    13233 2023-11-20 20:19:16.000000 mcbcdc-0.8/data/daa.txt
+-rw-rw-rw-   0        0        0     1405 2024-04-30 07:01:43.000000 mcbcdc-0.8/data/ddos.txt
+-rw-rw-rw-   0        0        0     1882 2024-04-30 07:01:49.000000 mcbcdc-0.8/data/dns.txt
+-rw-rw-rw-   0        0        0      349 2024-04-30 07:01:24.000000 mcbcdc-0.8/data/ip_spoofing.txt
+-rw-rw-rw-   0        0        0      113 2024-04-30 07:01:55.000000 mcbcdc-0.8/data/sniffer_A.txt
+-rw-rw-rw-   0        0        0      645 2024-04-30 07:02:04.000000 mcbcdc-0.8/data/sniffer_B.txt
+-rw-rw-rw-   0        0        0     1952 2024-04-30 07:01:37.000000 mcbcdc-0.8/data/spam_mail.txt
+drwxrwxrwx   0        0        0        0 2024-04-30 07:31:01.363556 mcbcdc-0.8/file/
+-rw-rw-rw-   0        0        0        0 2023-11-20 17:20:14.000000 mcbcdc-0.8/file/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-11-20 18:43:45.000000 mcbcdc-0.8/file/file2.py
+drwxrwxrwx   0        0        0        0 2024-04-30 07:31:01.663445 mcbcdc-0.8/mcbcdc.egg-info/
+-rw-rw-rw-   0        0        0      145 2024-04-30 07:31:01.000000 mcbcdc-0.8/mcbcdc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2024-04-30 07:31:01.000000 mcbcdc-0.8/mcbcdc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 07:31:01.000000 mcbcdc-0.8/mcbcdc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-30 07:31:01.000000 mcbcdc-0.8/mcbcdc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 07:31:01.672438 mcbcdc-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      438 2024-04-30 06:59:46.000000 mcbcdc-0.8/setup.py
```

