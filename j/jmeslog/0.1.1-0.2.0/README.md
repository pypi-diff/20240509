# Comparing `tmp/jmeslog-0.1.1.tar.gz` & `tmp/jmeslog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jmeslog-0.1.1.tar", last modified: Mon Mar 23 21:43:39 2020, max compression
+gzip compressed data, was "jmeslog-0.2.0.tar", max compression
```

## Comparing `jmeslog-0.1.1.tar` & `jmeslog-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 jamessar (1120452788) ANT\Domain Users (1896053708)        0 2020-03-23 21:43:39.000000 jmeslog-0.1.1/
--rw-r--r--   0 jamessar (1120452788) ANT\Domain Users (1896053708)     5524 2020-03-23 21:43:39.000000 jmeslog-0.1.1/PKG-INFO
--rw-r--r--   0 jamessar (1120452788) ANT\Domain Users (1896053708)     4083 2020-03-17 21:47:35.000000 jmeslog-0.1.1/README.rst
-drwxr-xr-x   0 jamessar (1120452788) ANT\Domain Users (1896053708)        0 2020-03-23 21:43:39.000000 jmeslog-0.1.1/jmeslog.egg-info/
--rw-r--r--   0 jamessar (1120452788) ANT\Domain Users (1896053708)     5524 2020-03-23 21:43:39.000000 jmeslog-0.1.1/jmeslog.egg-info/PKG-INFO
--rw-r--r--   0 jamessar (1120452788) ANT\Domain Users (1896053708)      214 2020-03-23 21:43:39.000000 jmeslog-0.1.1/jmeslog.egg-info/SOURCES.txt
--rw-r--r--   0 jamessar (1120452788) ANT\Domain Users (1896053708)        1 2020-03-23 21:43:39.000000 jmeslog-0.1.1/jmeslog.egg-info/dependency_links.txt
--rw-r--r--   0 jamessar (1120452788) ANT\Domain Users (1896053708)       42 2020-03-23 21:43:39.000000 jmeslog-0.1.1/jmeslog.egg-info/entry_points.txt
--rw-r--r--   0 jamessar (1120452788) ANT\Domain Users (1896053708)        8 2020-03-23 21:43:39.000000 jmeslog-0.1.1/jmeslog.egg-info/top_level.txt
--rw-r--r--   0 jamessar (1120452788) ANT\Domain Users (1896053708)        1 2020-03-05 21:04:03.000000 jmeslog-0.1.1/jmeslog.egg-info/zip-safe
--rw-r--r--   0 jamessar (1120452788) ANT\Domain Users (1896053708)    18436 2020-03-23 21:42:25.000000 jmeslog-0.1.1/jmeslog.py
--rw-r--r--   0 jamessar (1120452788) ANT\Domain Users (1896053708)       38 2020-03-23 21:43:39.000000 jmeslog-0.1.1/setup.cfg
--rw-r--r--   0 jamessar (1120452788) ANT\Domain Users (1896053708)      918 2020-03-23 21:42:50.000000 jmeslog-0.1.1/setup.py
+-rw-r--r--   0        0        0    11357 2024-05-09 21:06:48.634124 jmeslog-0.2.0/LICENSE
+-rw-r--r--   0        0        0       64 2024-05-09 21:06:48.634124 jmeslog-0.2.0/NOTICE
+-rw-r--r--   0        0        0     7597 2024-05-09 21:06:48.634124 jmeslog-0.2.0/README.md
+-rw-r--r--   0        0        0     2253 2024-05-09 21:06:49.146129 jmeslog-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-09 21:06:48.634124 jmeslog-0.2.0/src/jmeslog/__init__.py
+-rw-r--r--   0        0        0       97 2024-05-09 21:06:48.634124 jmeslog-0.2.0/src/jmeslog/__main__.py
+-rw-r--r--   0        0        0     5461 2024-05-09 21:06:48.634124 jmeslog-0.2.0/src/jmeslog/cli.py
+-rw-r--r--   0        0        0     1058 2024-05-09 21:06:48.634124 jmeslog-0.2.0/src/jmeslog/constants.py
+-rw-r--r--   0        0        0    10372 2024-05-09 21:06:48.634124 jmeslog-0.2.0/src/jmeslog/core.py
+-rw-r--r--   0        0        0      460 2024-05-09 21:06:48.634124 jmeslog-0.2.0/src/jmeslog/errors.py
+-rw-r--r--   0        0        0     2731 2024-05-09 21:06:48.634124 jmeslog-0.2.0/src/jmeslog/model.py
+-rw-r--r--   0        0        0     8673 1970-01-01 00:00:00.000000 jmeslog-0.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

