# Comparing `tmp/ihm-1.0.tar.gz` & `tmp/ihm-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ihm-1.0.tar", last modified: Wed Feb 14 00:08:33 2024, max compression
+gzip compressed data, was "ihm-1.1.tar", last modified: Thu May  9 20:02:44 2024, max compression
```

## Comparing `ihm-1.0.tar` & `ihm-1.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-02-14 00:08:33.491470 ihm-1.0/
--rw-r--r--   0 ben        (501) staff       (20)    21744 2024-02-13 23:53:43.000000 ihm-1.0/ChangeLog.rst
--rw-r--r--   0 ben        (501) staff       (20)     1079 2023-01-09 21:25:29.000000 ihm-1.0/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)      168 2024-02-13 23:54:33.000000 ihm-1.0/MANIFEST.in
--rw-r--r--   0 ben        (501) staff       (20)     3877 2024-02-14 00:08:33.490814 ihm-1.0/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     3302 2024-01-08 21:48:27.000000 ihm-1.0/README.md
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-02-14 00:08:33.429817 ihm-1.0/examples/
--rw-r--r--   0 ben        (501) staff       (20)     3609 2018-11-21 18:14:46.000000 ihm-1.0/examples/atom_reader.c
--rw-r--r--   0 ben        (501) staff       (20)     3809 2024-02-13 19:46:42.000000 ihm-1.0/examples/ligands_water.py
--rw-r--r--   0 ben        (501) staff       (20)     3229 2020-12-19 07:34:48.000000 ihm-1.0/examples/locations.py
--rw-r--r--   0 ben        (501) staff       (20)     5661 2021-12-16 08:25:03.000000 ihm-1.0/examples/mini.cif
--rw-r--r--   0 ben        (501) staff       (20)     2526 2020-12-19 07:30:19.000000 ihm-1.0/examples/non_standard_residues.py
--rw-r--r--   0 ben        (501) staff       (20)     6883 2023-12-14 21:04:25.000000 ihm-1.0/examples/simple-docking.py
--rw-r--r--   0 ben        (501) staff       (20)     1296 2018-03-15 23:56:40.000000 ihm-1.0/examples/simple.pdb
--rw-r--r--   0 ben        (501) staff       (20)     1411 2022-06-01 16:20:40.000000 ihm-1.0/examples/stream_parser.py
--rw-r--r--   0 ben        (501) staff       (20)     2168 2024-01-08 21:32:39.000000 ihm-1.0/examples/validate_pdb_dev.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-02-14 00:08:33.446743 ihm-1.0/ihm/
--rw-r--r--   0 ben        (501) staff       (20)    75249 2024-02-13 23:54:27.000000 ihm-1.0/ihm/__init__.py
--rw-r--r--   0 ben        (501) staff       (20)     3629 2024-02-13 21:15:38.000000 ihm-1.0/ihm/analysis.py
--rw-r--r--   0 ben        (501) staff       (20)     5485 2022-10-05 17:19:57.000000 ihm-1.0/ihm/citations.py
--rw-r--r--   0 ben        (501) staff       (20)     3691 2023-07-10 19:08:20.000000 ihm-1.0/ihm/cross_linkers.py
--rw-r--r--   0 ben        (501) staff       (20)     6236 2023-12-06 01:58:54.000000 ihm-1.0/ihm/dataset.py
--rw-r--r--   0 ben        (501) staff       (20)    17022 2023-09-26 23:50:13.000000 ihm-1.0/ihm/dictionary.py
--rw-r--r--   0 ben        (501) staff       (20)   169816 2024-02-10 06:47:29.000000 ihm-1.0/ihm/dumper.py
--rw-r--r--   0 ben        (501) staff       (20)    49161 2024-02-13 21:15:38.000000 ihm-1.0/ihm/flr.py
--rw-r--r--   0 ben        (501) staff       (20)    26464 2024-02-13 21:15:38.000000 ihm-1.0/ihm/format.py
--rw-r--r--   0 ben        (501) staff       (20)    20309 2023-08-29 05:38:44.000000 ihm-1.0/ihm/format_bcif.py
--rw-r--r--   0 ben        (501) staff       (20)     7048 2023-08-28 23:45:38.000000 ihm-1.0/ihm/geometry.py
--rw-r--r--   0 ben        (501) staff       (20)    14043 2024-02-13 21:15:38.000000 ihm-1.0/ihm/location.py
--rw-r--r--   0 ben        (501) staff       (20)    34866 2023-10-24 00:54:14.000000 ihm-1.0/ihm/metadata.py
--rw-r--r--   0 ben        (501) staff       (20)    19675 2024-02-13 21:15:38.000000 ihm-1.0/ihm/model.py
--rw-r--r--   0 ben        (501) staff       (20)    12093 2024-02-13 21:25:54.000000 ihm-1.0/ihm/multi_state_scheme.py
--rw-r--r--   0 ben        (501) staff       (20)     3384 2023-08-28 23:22:37.000000 ihm-1.0/ihm/protocol.py
--rw-r--r--   0 ben        (501) staff       (20)   163043 2024-02-13 21:15:38.000000 ihm-1.0/ihm/reader.py
--rw-r--r--   0 ben        (501) staff       (20)     6505 2023-08-30 04:16:54.000000 ihm-1.0/ihm/reference.py
--rw-r--r--   0 ben        (501) staff       (20)     6713 2023-09-07 20:20:29.000000 ihm-1.0/ihm/report.py
--rw-r--r--   0 ben        (501) staff       (20)     7102 2023-09-13 03:36:54.000000 ihm-1.0/ihm/representation.py
--rw-r--r--   0 ben        (501) staff       (20)    34303 2024-02-13 21:15:38.000000 ihm-1.0/ihm/restraint.py
--rw-r--r--   0 ben        (501) staff       (20)     1743 2024-02-13 21:15:38.000000 ihm-1.0/ihm/source.py
--rw-r--r--   0 ben        (501) staff       (20)     8580 2023-08-29 05:46:41.000000 ihm-1.0/ihm/startmodel.py
--rw-r--r--   0 ben        (501) staff       (20)      698 2023-07-31 19:45:45.000000 ihm-1.0/ihm/test.py
--rw-r--r--   0 ben        (501) staff       (20)     2030 2023-04-26 18:43:07.000000 ihm-1.0/ihm/util.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-02-14 00:08:33.489931 ihm-1.0/ihm.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     3877 2024-02-14 00:08:33.000000 ihm-1.0/ihm.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)     1487 2024-02-14 00:08:33.000000 ihm-1.0/ihm.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2024-02-14 00:08:33.000000 ihm-1.0/ihm.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)        8 2024-02-14 00:08:33.000000 ihm-1.0/ihm.egg-info/requires.txt
--rw-r--r--   0 ben        (501) staff       (20)        4 2024-02-14 00:08:33.000000 ihm-1.0/ihm.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)       38 2024-02-14 00:08:33.491614 ihm-1.0/setup.cfg
--rwxr-xr-x   0 ben        (501) staff       (20)     2019 2024-02-13 23:54:45.000000 ihm-1.0/setup.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-02-14 00:08:33.451977 ihm-1.0/src/
--rw-r--r--   0 ben        (501) staff       (20)    40957 2023-07-19 20:19:37.000000 ihm-1.0/src/ihm_format.c
--rw-r--r--   0 ben        (501) staff       (20)     6791 2019-05-08 19:45:22.000000 ihm-1.0/src/ihm_format.h
--rw-r--r--   0 ben        (501) staff       (20)    16903 2023-12-01 01:11:14.000000 ihm-1.0/src/ihm_format.i
--rw-r--r--   0 ben        (501) staff       (20)   187439 2024-02-14 00:08:27.000000 ihm-1.0/src/ihm_format_wrap_1.0.c
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-02-14 00:08:33.488257 ihm-1.0/test/
--rw-r--r--   0 ben        (501) staff       (20)     2481 2023-08-28 23:21:00.000000 ihm-1.0/test/test_analysis.py
--rw-r--r--   0 ben        (501) staff       (20)      459 2021-12-22 00:15:17.000000 ihm-1.0/test/test_citations.py
--rw-r--r--   0 ben        (501) staff       (20)      515 2021-12-22 00:15:17.000000 ihm-1.0/test/test_cross_linkers.py
--rw-r--r--   0 ben        (501) staff       (20)     9118 2023-12-06 02:07:47.000000 ihm-1.0/test/test_dataset.py
--rw-r--r--   0 ben        (501) staff       (20)    17429 2024-01-08 21:32:39.000000 ihm-1.0/test/test_dictionary.py
--rw-r--r--   0 ben        (501) staff       (20)   194899 2024-02-10 06:53:07.000000 ihm-1.0/test/test_dumper.py
--rw-r--r--   0 ben        (501) staff       (20)      856 2021-12-22 00:15:17.000000 ihm-1.0/test/test_edit.py
--rw-r--r--   0 ben        (501) staff       (20)     3692 2023-09-27 00:32:12.000000 ihm-1.0/test/test_examples.py
--rw-r--r--   0 ben        (501) staff       (20)    71220 2023-12-14 21:05:29.000000 ihm-1.0/test/test_flr.py
--rw-r--r--   0 ben        (501) staff       (20)    30546 2023-03-13 17:56:56.000000 ihm-1.0/test/test_format.py
--rw-r--r--   0 ben        (501) staff       (20)    26357 2021-12-22 00:15:17.000000 ihm-1.0/test/test_format_bcif.py
--rw-r--r--   0 ben        (501) staff       (20)     5176 2021-12-22 00:15:17.000000 ihm-1.0/test/test_geometry.py
--rw-r--r--   0 ben        (501) staff       (20)    12444 2023-08-30 01:32:46.000000 ihm-1.0/test/test_location.py
--rw-r--r--   0 ben        (501) staff       (20)    51208 2024-02-12 20:31:53.000000 ihm-1.0/test/test_main.py
--rw-r--r--   0 ben        (501) staff       (20)     9494 2024-02-13 19:47:19.000000 ihm-1.0/test/test_make_mmcif.py
--rw-r--r--   0 ben        (501) staff       (20)    23762 2023-12-01 04:01:53.000000 ihm-1.0/test/test_metadata.py
--rw-r--r--   0 ben        (501) staff       (20)     7177 2022-08-02 23:57:09.000000 ihm-1.0/test/test_model.py
--rw-r--r--   0 ben        (501) staff       (20)    23932 2023-12-14 21:05:29.000000 ihm-1.0/test/test_multi_state_scheme.py
--rw-r--r--   0 ben        (501) staff       (20)     1342 2023-08-29 05:54:07.000000 ihm-1.0/test/test_protocol.py
--rw-r--r--   0 ben        (501) staff       (20)   192839 2024-02-13 20:13:15.000000 ihm-1.0/test/test_reader.py
--rw-r--r--   0 ben        (501) staff       (20)     5088 2021-12-22 00:15:17.000000 ihm-1.0/test/test_reference.py
--rw-r--r--   0 ben        (501) staff       (20)     7785 2023-09-07 20:21:19.000000 ihm-1.0/test/test_report.py
--rw-r--r--   0 ben        (501) staff       (20)     3480 2023-09-13 03:38:54.000000 ihm-1.0/test/test_representation.py
--rw-r--r--   0 ben        (501) staff       (20)    10674 2023-09-07 20:18:01.000000 ihm-1.0/test/test_restraint.py
--rw-r--r--   0 ben        (501) staff       (20)     2632 2021-12-22 00:15:17.000000 ihm-1.0/test/test_startmodel.py
--rw-r--r--   0 ben        (501) staff       (20)     2349 2021-12-22 00:15:17.000000 ihm-1.0/test/test_util.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-02-14 00:08:33.489007 ihm-1.0/util/
--rw-r--r--   0 ben        (501) staff       (20)     8233 2024-02-13 00:50:18.000000 ihm-1.0/util/make-mmcif.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-09 20:02:44.213485 ihm-1.1/
+-rw-r--r--   0 ben        (501) staff       (20)    22488 2024-05-09 19:49:59.000000 ihm-1.1/ChangeLog.rst
+-rw-r--r--   0 ben        (501) staff       (20)     1079 2024-03-07 17:10:07.000000 ihm-1.1/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)      168 2024-05-09 19:45:56.000000 ihm-1.1/MANIFEST.in
+-rw-r--r--   0 ben        (501) staff       (20)     4089 2024-05-09 20:02:44.212611 ihm-1.1/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     3514 2024-03-07 22:38:21.000000 ihm-1.1/README.md
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-09 20:02:44.174804 ihm-1.1/examples/
+-rw-r--r--   0 ben        (501) staff       (20)     3609 2018-11-21 18:14:46.000000 ihm-1.1/examples/atom_reader.c
+-rw-r--r--   0 ben        (501) staff       (20)     3809 2024-02-13 19:46:42.000000 ihm-1.1/examples/ligands_water.py
+-rw-r--r--   0 ben        (501) staff       (20)     3229 2020-12-19 07:34:48.000000 ihm-1.1/examples/locations.py
+-rw-r--r--   0 ben        (501) staff       (20)     5661 2021-12-16 08:25:03.000000 ihm-1.1/examples/mini.cif
+-rw-r--r--   0 ben        (501) staff       (20)     2526 2020-12-19 07:30:19.000000 ihm-1.1/examples/non_standard_residues.py
+-rw-r--r--   0 ben        (501) staff       (20)     6883 2023-12-14 21:04:25.000000 ihm-1.1/examples/simple-docking.py
+-rw-r--r--   0 ben        (501) staff       (20)     1296 2018-03-15 23:56:40.000000 ihm-1.1/examples/simple.pdb
+-rw-r--r--   0 ben        (501) staff       (20)     1411 2022-06-01 16:20:40.000000 ihm-1.1/examples/stream_parser.py
+-rw-r--r--   0 ben        (501) staff       (20)     2168 2024-01-08 21:32:39.000000 ihm-1.1/examples/validate_pdb_dev.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-09 20:02:44.187485 ihm-1.1/ihm/
+-rw-r--r--   0 ben        (501) staff       (20)    76414 2024-05-09 19:45:53.000000 ihm-1.1/ihm/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     3629 2024-02-13 21:15:38.000000 ihm-1.1/ihm/analysis.py
+-rw-r--r--   0 ben        (501) staff       (20)     5485 2022-10-05 17:19:57.000000 ihm-1.1/ihm/citations.py
+-rw-r--r--   0 ben        (501) staff       (20)     3691 2023-07-10 19:08:20.000000 ihm-1.1/ihm/cross_linkers.py
+-rw-r--r--   0 ben        (501) staff       (20)     6236 2023-12-06 01:58:54.000000 ihm-1.1/ihm/dataset.py
+-rw-r--r--   0 ben        (501) staff       (20)    17022 2023-09-26 23:50:13.000000 ihm-1.1/ihm/dictionary.py
+-rw-r--r--   0 ben        (501) staff       (20)   170615 2024-05-08 15:59:21.000000 ihm-1.1/ihm/dumper.py
+-rw-r--r--   0 ben        (501) staff       (20)    49161 2024-02-13 21:15:38.000000 ihm-1.1/ihm/flr.py
+-rw-r--r--   0 ben        (501) staff       (20)    26464 2024-04-06 00:29:14.000000 ihm-1.1/ihm/format.py
+-rw-r--r--   0 ben        (501) staff       (20)    20309 2023-08-29 05:38:44.000000 ihm-1.1/ihm/format_bcif.py
+-rw-r--r--   0 ben        (501) staff       (20)     7048 2023-08-28 23:45:38.000000 ihm-1.1/ihm/geometry.py
+-rw-r--r--   0 ben        (501) staff       (20)    14168 2024-05-08 15:59:21.000000 ihm-1.1/ihm/location.py
+-rw-r--r--   0 ben        (501) staff       (20)    34866 2023-10-24 00:54:14.000000 ihm-1.1/ihm/metadata.py
+-rw-r--r--   0 ben        (501) staff       (20)    19675 2024-02-13 21:15:38.000000 ihm-1.1/ihm/model.py
+-rw-r--r--   0 ben        (501) staff       (20)    12093 2024-02-13 21:25:54.000000 ihm-1.1/ihm/multi_state_scheme.py
+-rw-r--r--   0 ben        (501) staff       (20)     3384 2023-08-28 23:22:37.000000 ihm-1.1/ihm/protocol.py
+-rw-r--r--   0 ben        (501) staff       (20)   165673 2024-05-08 15:59:21.000000 ihm-1.1/ihm/reader.py
+-rw-r--r--   0 ben        (501) staff       (20)     6505 2023-08-30 04:16:54.000000 ihm-1.1/ihm/reference.py
+-rw-r--r--   0 ben        (501) staff       (20)     6713 2023-09-07 20:20:29.000000 ihm-1.1/ihm/report.py
+-rw-r--r--   0 ben        (501) staff       (20)     7102 2023-09-13 03:36:54.000000 ihm-1.1/ihm/representation.py
+-rw-r--r--   0 ben        (501) staff       (20)    34303 2024-02-13 21:15:38.000000 ihm-1.1/ihm/restraint.py
+-rw-r--r--   0 ben        (501) staff       (20)     1743 2024-02-13 21:15:38.000000 ihm-1.1/ihm/source.py
+-rw-r--r--   0 ben        (501) staff       (20)     8580 2023-08-29 05:46:41.000000 ihm-1.1/ihm/startmodel.py
+-rw-r--r--   0 ben        (501) staff       (20)      698 2023-07-31 19:45:45.000000 ihm-1.1/ihm/test.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-09 20:02:44.191129 ihm-1.1/ihm/util/
+-rw-r--r--   0 ben        (501) staff       (20)     2030 2023-04-26 18:43:07.000000 ihm-1.1/ihm/util/__init__.py
+-rw-r--r--   0 ben        (501) staff       (20)     8373 2024-03-25 20:23:07.000000 ihm-1.1/ihm/util/make_mmcif.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-09 20:02:44.211825 ihm-1.1/ihm.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     4089 2024-05-09 20:02:44.000000 ihm-1.1/ihm.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     1500 2024-05-09 20:02:44.000000 ihm-1.1/ihm.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2024-05-09 20:02:44.000000 ihm-1.1/ihm.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)        8 2024-05-09 20:02:44.000000 ihm-1.1/ihm.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)        4 2024-05-09 20:02:44.000000 ihm-1.1/ihm.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)       38 2024-05-09 20:02:44.213644 ihm-1.1/setup.cfg
+-rwxr-xr-x   0 ben        (501) staff       (20)     2031 2024-05-09 19:45:58.000000 ihm-1.1/setup.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-09 20:02:44.193917 ihm-1.1/src/
+-rw-r--r--   0 ben        (501) staff       (20)    40957 2023-07-19 20:19:37.000000 ihm-1.1/src/ihm_format.c
+-rw-r--r--   0 ben        (501) staff       (20)     6791 2019-05-08 19:45:22.000000 ihm-1.1/src/ihm_format.h
+-rw-r--r--   0 ben        (501) staff       (20)    16903 2023-12-01 01:11:14.000000 ihm-1.1/src/ihm_format.i
+-rw-r--r--   0 ben        (501) staff       (20)   187723 2024-05-09 20:02:39.000000 ihm-1.1/src/ihm_format_wrap_1.1.c
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-05-09 20:02:44.210871 ihm-1.1/test/
+-rw-r--r--   0 ben        (501) staff       (20)     2481 2023-08-28 23:21:00.000000 ihm-1.1/test/test_analysis.py
+-rw-r--r--   0 ben        (501) staff       (20)      459 2021-12-22 00:15:17.000000 ihm-1.1/test/test_citations.py
+-rw-r--r--   0 ben        (501) staff       (20)      515 2021-12-22 00:15:17.000000 ihm-1.1/test/test_cross_linkers.py
+-rw-r--r--   0 ben        (501) staff       (20)     9118 2023-12-06 02:07:47.000000 ihm-1.1/test/test_dataset.py
+-rw-r--r--   0 ben        (501) staff       (20)    17429 2024-01-08 21:32:39.000000 ihm-1.1/test/test_dictionary.py
+-rw-r--r--   0 ben        (501) staff       (20)   196582 2024-05-08 15:59:21.000000 ihm-1.1/test/test_dumper.py
+-rw-r--r--   0 ben        (501) staff       (20)      856 2021-12-22 00:15:17.000000 ihm-1.1/test/test_edit.py
+-rw-r--r--   0 ben        (501) staff       (20)     3692 2024-05-08 15:59:21.000000 ihm-1.1/test/test_examples.py
+-rw-r--r--   0 ben        (501) staff       (20)    71220 2023-12-14 21:05:29.000000 ihm-1.1/test/test_flr.py
+-rw-r--r--   0 ben        (501) staff       (20)    30546 2024-04-06 00:29:35.000000 ihm-1.1/test/test_format.py
+-rw-r--r--   0 ben        (501) staff       (20)    26357 2021-12-22 00:15:17.000000 ihm-1.1/test/test_format_bcif.py
+-rw-r--r--   0 ben        (501) staff       (20)     5176 2021-12-22 00:15:17.000000 ihm-1.1/test/test_geometry.py
+-rw-r--r--   0 ben        (501) staff       (20)    12444 2023-08-30 01:32:46.000000 ihm-1.1/test/test_location.py
+-rw-r--r--   0 ben        (501) staff       (20)    51250 2024-04-03 18:14:20.000000 ihm-1.1/test/test_main.py
+-rw-r--r--   0 ben        (501) staff       (20)     9564 2024-03-25 20:28:07.000000 ihm-1.1/test/test_make_mmcif.py
+-rw-r--r--   0 ben        (501) staff       (20)    23762 2023-12-01 04:01:53.000000 ihm-1.1/test/test_metadata.py
+-rw-r--r--   0 ben        (501) staff       (20)     7177 2022-08-02 23:57:09.000000 ihm-1.1/test/test_model.py
+-rw-r--r--   0 ben        (501) staff       (20)    23932 2024-02-15 20:29:49.000000 ihm-1.1/test/test_multi_state_scheme.py
+-rw-r--r--   0 ben        (501) staff       (20)     1342 2023-08-29 05:54:07.000000 ihm-1.1/test/test_protocol.py
+-rw-r--r--   0 ben        (501) staff       (20)   194967 2024-05-08 16:00:11.000000 ihm-1.1/test/test_reader.py
+-rw-r--r--   0 ben        (501) staff       (20)     5088 2021-12-22 00:15:17.000000 ihm-1.1/test/test_reference.py
+-rw-r--r--   0 ben        (501) staff       (20)     7785 2023-09-07 20:21:19.000000 ihm-1.1/test/test_report.py
+-rw-r--r--   0 ben        (501) staff       (20)     3480 2023-09-13 03:38:54.000000 ihm-1.1/test/test_representation.py
+-rw-r--r--   0 ben        (501) staff       (20)    10674 2023-09-07 20:18:01.000000 ihm-1.1/test/test_restraint.py
+-rw-r--r--   0 ben        (501) staff       (20)     2632 2021-12-22 00:15:17.000000 ihm-1.1/test/test_startmodel.py
+-rw-r--r--   0 ben        (501) staff       (20)     2349 2021-12-22 00:15:17.000000 ihm-1.1/test/test_util.py
```

### Comparing `ihm-1.0/ChangeLog.rst` & `ihm-1.1/ChangeLog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+1.1 - 2024-05-09
+================
+  - :class:`ihm.System` now allows for one or more official database IDs to
+    be associated with the system using the new :class:`ihm.Database` class.
+    This maps to the mmCIF ``_database_2`` category (#135).
+  - :class:`ihm.location.FileLocation` now allows for an optional file format
+    to be specified (#139).
+  - The ``util/make-mmcif.py`` script is now included in the installed package,
+    so can be run if desired with ``python3 -m ihm.util.make_mmcif`` (#134).
+  - Bugfix: allow for file sizes in input mmCIF files to be floating point
+    values (#138).
+  - Bugfix: the 'Other' content type is now handled correctly when reading
+    information about external files from an mmCIF file (#139).
+
 1.0 - 2024-02-13
 ================
   - Support for multi-state schemes (such as kinetic rates and relaxation
     times for conversions between states) was added;
     see :mod:`ihm.multi_state_scheme`.
   - Residue numbering in non-polymer, water, and branched entities should
     now be better handled, no longer requiring the various scheme tables
```

### Comparing `ihm-1.0/LICENSE` & `ihm-1.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2023 IHM Working Group
+Copyright (c) 2018-2024 IHM Working Group
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ihm-1.0/PKG-INFO` & `ihm-1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ihm
-Version: 1.0
+Version: 1.1
 Summary: Package for handling IHM mmCIF and BinaryCIF files
 Home-page: https://github.com/ihmwg/python-ihm
 Author: Ben Webb
 Author-email: ben@salilab.org
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -55,14 +55,22 @@
 
 On a Fedora or RedHat Enterprise Linux box, install with
 
 ```
 dnf copr enable salilab/salilab; dnf install python3-ihm
 ```
 
+On an Ubuntu LTS box, install from
+[our PPA](https://launchpad.net/~salilab/+archive/ubuntu/ppa) with
+
+```
+apt install software-properties-common; add-apt-repository ppa:salilab/ppa;
+apt install python3-ihm
+```
+
 Alternatively, install with pip:
 
 ```
 pip install ihm
 ```
 
 (Note that pip builds a C extension module for faster parsing of mmCIF files.
```

### Comparing `ihm-1.0/README.md` & `ihm-1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,22 @@
 
 On a Fedora or RedHat Enterprise Linux box, install with
 
 ```
 dnf copr enable salilab/salilab; dnf install python3-ihm
 ```
 
+On an Ubuntu LTS box, install from
+[our PPA](https://launchpad.net/~salilab/+archive/ubuntu/ppa) with
+
+```
+apt install software-properties-common; add-apt-repository ppa:salilab/ppa;
+apt install python3-ihm
+```
+
 Alternatively, install with pip:
 
 ```
 pip install ihm
 ```
 
 (Note that pip builds a C extension module for faster parsing of mmCIF files.
```

### Comparing `ihm-1.0/examples/atom_reader.c` & `ihm-1.1/examples/atom_reader.c`

 * *Files identical despite different names*

### Comparing `ihm-1.0/examples/ligands_water.py` & `ihm-1.1/examples/ligands_water.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/examples/locations.py` & `ihm-1.1/examples/locations.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/examples/mini.cif` & `ihm-1.1/examples/mini.cif`

 * *Files identical despite different names*

### Comparing `ihm-1.0/examples/non_standard_residues.py` & `ihm-1.1/examples/non_standard_residues.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/examples/simple-docking.py` & `ihm-1.1/examples/simple-docking.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/examples/simple.pdb` & `ihm-1.1/examples/simple.pdb`

 * *Files identical despite different names*

### Comparing `ihm-1.0/examples/stream_parser.py` & `ihm-1.1/examples/stream_parser.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/examples/validate_pdb_dev.py` & `ihm-1.1/examples/validate_pdb_dev.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/__init__.py` & `ihm-1.1/ihm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 try:
     import urllib.request as urllib2
 except ImportError:    # pragma: no cover
     import urllib2
 import json
 from . import util
 
-__version__ = '1.0'
+__version__ = '1.1'
 
 
 class __UnknownValue(object):
     # Represent the mmCIF 'unknown' special value
 
     def __str__(self):
         return '?'
@@ -70,22 +70,30 @@
 class System(object):
     """Top-level class representing a complete modeled system.
 
        :param str title: Title (longer text description) of the system.
        :param str id: Unique identifier for this system in the mmCIF file.
        :param str model_details: Detailed description of the system, like an
                                  abstract.
+       :param databases: If this system is part of one or more official
+              databases (e.g. PDB, PDB-Dev, SwissModel), details of
+              the database identifiers.
+       :type databases: sequence of :class:`Database`
     """
 
     structure_determination_methodology = "integrative"
 
-    def __init__(self, title=None, id='model', model_details=None):
+    def __init__(self, title=None, id='model', model_details=None,
+                 databases=[]):
         self.id = id
         self.title = title
         self.model_details = model_details
+        self.databases = []
+        self.databases.extend(databases)
+        self._database_status = {}
 
         #: List of plain text comments. These will be added to the top of
         #: the mmCIF file.
         self.comments = []
 
         #: List of all software used in the modeling. See :class:`Software`.
         self.software = []
@@ -659,14 +667,32 @@
                     "of Restraints. Due to limitations of the underlying "
                     "dictionary, all objects in a RestraintGroup must be of "
                     "the same type, and only certain types (currently only "
                     "DerivedDistanceRestraint or PredictedContactRestraint) "
                     "can be grouped." % g)
 
 
+class Database(object):
+    """Information about a System that is part of an official database.
+
+       If a :class:`System` is part of one or more official databases
+       (e.g. PDB, PDB-Dev, SwissModel), this class contains details of the
+       database identifiers. It should be passed to the :class:`System`
+       constructor.
+
+       :param str id: Abbreviated name of the database (e.g. PDB).
+       :param str code: Identifier from the database (e.g. 1abc).
+       :param str doi: Digital Object Identifier of the database entry.
+       :param str accession: Extended accession code of the database entry.
+       """
+    def __init__(self, id, code, doi=None, accession=None):
+        self.id, self.code = id, code
+        self.doi, self.accession = doi, accession
+
+
 class Software(object):
     """Software used as part of the modeling protocol.
 
        :param str name: The name of the software.
        :param str classification: The major function of the software, for
               example 'model building', 'sample preparation',
               'data collection'.
@@ -1246,15 +1272,15 @@
         self.asym = asym
         if entity is None and asym:
             self.entity = asym.entity
         # todo: check id for validity (at property read time)
         self.seq_id = seq_id
 
     def atom(self, atom_id):
-        """Get a :class:`Atom` in this residue with the given name."""
+        """Get a :class:`~ihm.Atom` in this residue with the given name."""
         return Atom(residue=self, id=atom_id)
 
     def _get_auth_seq_id(self):
         return self.asym._get_auth_seq_id_ins_code(self.seq_id)[0]
     auth_seq_id = property(_get_auth_seq_id,
                            doc="Author-provided seq_id; only makes sense "
                                "for asymmetric units")
@@ -1376,19 +1402,19 @@
         self.description, self.details = description, details
         self.source = source
         self.references = []
         self.references.extend(references)
 
         #: String descriptors of branched chemical structure.
         #: These generally only make sense for oligosaccharide entities,
-        #: and should be a list of :class:`BranchDescriptor` objects.
+        #: and should be a list of :class:`~ihm.BranchDescriptor` objects.
         self.branch_descriptors = []
 
         #: Any links between components in a branched entity.
-        #: This is a list of :class:`BranchLink` objects.
+        #: This is a list of :class:`~ihm.BranchLink` objects.
         self.branch_links = []
 
     def __str__(self):
         return "<ihm.Entity(%s)>" % self.description
 
     def is_polymeric(self):
         """Return True iff this entity represents a polymer, such as an
@@ -1487,15 +1513,15 @@
 
 
 class AsymUnit(object):
     """An asymmetric unit, i.e. a unique instance of an Entity that
        was modeled.
 
        Note that this class should not be used to describe crystal waters;
-       for that, see :class:`WaterAsymUnit`.
+       for that, see :class:`ihm.WaterAsymUnit`.
 
        :param entity: The unique sequence of this asymmetric unit.
        :type entity: :class:`Entity`
        :param str details: Longer text description of this unit.
        :param auth_seq_id_map: Mapping from internal 1-based consecutive
               residue numbering (`seq_id`) to PDB "author-provided" numbering
               (`auth_seq_id` plus an optional `ins_code`). This can be either
```

### Comparing `ihm-1.0/ihm/analysis.py` & `ihm-1.1/ihm/analysis.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/citations.py` & `ihm-1.1/ihm/citations.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/cross_linkers.py` & `ihm-1.1/ihm/cross_linkers.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/dataset.py` & `ihm-1.1/ihm/dataset.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/dictionary.py` & `ihm-1.1/ihm/dictionary.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/dumper.py` & `ihm-1.1/ihm/dumper.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,14 +215,32 @@
                           "ordinal"]) as lp:
             for n, grant in enumerate(system.grants):
                 lp.write(funding_organization=grant.funding_organization,
                          country=grant.country,
                          grant_number=grant.grant_number, ordinal=n + 1)
 
 
+class _DatabaseDumper(Dumper):
+    def dump(self, system, writer):
+        with writer.loop("_database_2",
+                         ["database_id", "database_code",
+                          "pdbx_database_accession", "pdbx_DOI"]) as lp:
+            for d in system.databases:
+                lp.write(database_id=d.id, database_code=d.code,
+                         pdbx_DOI=d.doi,
+                         pdbx_database_accession=d.accession)
+
+
+class _DatabaseStatusDumper(Dumper):
+    def dump(self, system, writer):
+        with writer.category("_pdbx_database_status") as lp:
+            # Pass through all data items from a Python dict
+            lp.write(**system._database_status)
+
+
 class _ChemCompDumper(Dumper):
     def dump(self, system, writer):
         comps = frozenset(comp for e in system.entities for comp in e.sequence)
 
         with writer.loop("_chem_comp", ["id", "type", "name",
                                         "formula", "formula_weight"]) as lp:
             for comp in sorted(comps, key=operator.attrgetter('id')):
@@ -975,23 +993,24 @@
                          reference_type=repo.reference_type,
                          reference=repo.reference, refers_to=repo.refers_to,
                          associated_url=repo.url, details=repo.details)
 
     def dump_refs(self, writer):
         with writer.loop("_ihm_external_files",
                          ["id", "reference_id", "file_path", "content_type",
-                          "file_size_bytes", "details"]) as lp:
+                          "file_format", "file_size_bytes", "details"]) as lp:
             for r in self._ref_by_id:
                 repo = r.repo or self._local_files
                 if r.path is None:
                     file_path = None
                 else:
                     file_path = self._posix_path(repo._get_full_path(r.path))
                 lp.write(id=r._id, reference_id=repo._id,
                          file_path=file_path, content_type=r.content_type,
+                         file_format=r.file_format,
                          file_size_bytes=r.file_size, details=r.details)
 
     # On Windows systems, convert native paths to POSIX-like (/-separated)
     # paths
     if os.sep == '/':
         def _posix_path(self, path):
             return path
@@ -3572,16 +3591,16 @@
         return writer
 
 
 class IHMVariant(Variant):
     """Used to select typical PDBx/IHM file output. See :func:`write`."""
     _dumpers = [
         _EntryDumper,  # must be first
-        _CollectionDumper,
-        _StructDumper, _CommentDumper, _AuditConformDumper, _CitationDumper,
+        _CollectionDumper, _StructDumper, _CommentDumper, _AuditConformDumper,
+        _DatabaseDumper, _DatabaseStatusDumper, _CitationDumper,
         _SoftwareDumper, _AuditAuthorDumper, _GrantDumper, _ChemCompDumper,
         _ChemDescriptorDumper, _EntityDumper, _EntitySrcGenDumper,
         _EntitySrcNatDumper, _EntitySrcSynDumper, _StructRefDumper,
         _EntityPolyDumper, _EntityNonPolyDumper, _EntityPolySeqDumper,
         _EntityPolySegmentDumper, _EntityBranchListDumper, _EntityBranchDumper,
         _StructAsymDumper, _PolySeqSchemeDumper,
         _NonPolySchemeDumper, _BranchSchemeDumper, _BranchDescriptorDumper,
```

### Comparing `ihm-1.0/ihm/flr.py` & `ihm-1.1/ihm/flr.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/format.py` & `ihm-1.1/ihm/format.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/format_bcif.py` & `ihm-1.1/ihm/format_bcif.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/geometry.py` & `ihm-1.1/ihm/geometry.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/location.py` & `ihm-1.1/ihm/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,23 +187,24 @@
 
        :param str path: the location of the file or directory (this can
               be `None` if `repo` is set, to refer to the entire repository)
        :param repo: object that describes the repository
               containing the file, or `None` if it is stored on the local disk
        :type repo: :class:`Repository`
        :param str details: optional description of the file
+       :param str file_format: optional file type (e.g. TXT, PNG, FASTA)
     """
 
     _eq_keys = Location._eq_keys + ['repo', 'path', 'content_type']
 
-    content_type = None
+    content_type = 'Other'
 
-    def __init__(self, path, repo=None, details=None):
+    def __init__(self, path, repo=None, details=None, file_format=None):
         super(FileLocation, self).__init__(details)
-        self.repo = repo
+        self.repo, self.file_format = repo, file_format
         if repo:
             self.path = path
             # Cannot determine file size if non-local
             self.file_size = None
         else:
             if not os.path.exists(path):
                 raise ValueError("%s does not exist" % path)
```

### Comparing `ihm-1.0/ihm/metadata.py` & `ihm-1.1/ihm/metadata.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/model.py` & `ihm-1.1/ihm/model.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/multi_state_scheme.py` & `ihm-1.1/ihm/multi_state_scheme.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/protocol.py` & `ihm-1.1/ihm/protocol.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/reader.py` & `ihm-1.1/ihm/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1021,14 +1021,61 @@
 
     def __call__(self, citation_id, name):
         s = self.sysr.citations.get_by_id(citation_id)
         if name is not None:
             s.authors.append(name)
 
 
+class _DatabaseHandler(Handler):
+    category = '_database_2'
+
+    def __call__(self, database_code, database_id, pdbx_doi,
+                 pdbx_database_accession):
+        d = ihm.Database(id=database_id, code=database_code,
+                         doi=pdbx_doi, accession=pdbx_database_accession)
+        self.system.databases.append(d)
+
+
+class _DatabaseStatusHandler(Handler):
+    category = '_pdbx_database_status'
+
+    # placeholder; the reader will otherwise only return strings or None
+    not_in_file = 0
+    _keys = ['entry_id', 'sg_entry', 'author_approval_type',
+             'author_release_status_code', 'date_author_approval',
+             'date_author_release_request', 'date_begin_deposition',
+             'date_begin_processing', 'date_begin_release_preparation',
+             'date_chemical_shifts', 'date_coordinates',
+             'date_deposition_form', 'date_end_processing',
+             'date_hold_chemical_shifts', 'date_hold_coordinates',
+             'date_hold_nmr_constraints', 'date_hold_struct_fact',
+             'date_manuscript', 'date_nmr_constraints', 'date_of_pdb_release',
+             'date_of_cs_release', 'date_of_mr_release', 'date_of_sf_release',
+             'date_struct_fact', 'date_submitted',
+             'dep_release_code_chemical_shifts',
+             'dep_release_code_coordinates',
+             'dep_release_code_nmr_constraints', 'dep_release_code_sequence',
+             'dep_release_code_struct_fact', 'deposit_site',
+             'hold_for_publication', 'methods_development_category',
+             'name_depositor', 'pdb_date_of_author_approval',
+             'pdb_format_compatible', 'process_site', 'rcsb_annotator',
+             'recvd_author_approval', 'recvd_chemical_shifts',
+             'recvd_coordinates', 'recvd_deposit_form',
+             'recvd_initial_deposition_date', 'recvd_internal_approval',
+             'recvd_manuscript', 'recvd_nmr_constraints', 'recvd_struct_fact',
+             'status_code', 'status_code_cs', 'status_code_mr',
+             'status_code_sf']
+
+    def __call__(self, *args):
+        # Just pass through all data items present in the file, as a dict
+        self.system._database_status = dict(
+            (k, v) for (k, v) in zip(self._keys, args)
+            if v != self.not_in_file)
+
+
 class _ChemCompHandler(Handler):
     category = '_chem_comp'
 
     def __init__(self, *args):
         super(_ChemCompHandler, self).__init__(*args)
         # Map _chem_comp.type to corresponding subclass of ihm.ChemComp
         self.type_map = dict((x[1].type.lower(), x[1])
@@ -1400,22 +1447,28 @@
         self.type_map = dict(
             (x[1].content_type.lower(), x[1])
             for x in inspect.getmembers(ihm.location, inspect.isclass)
             if issubclass(x[1], ihm.location.FileLocation)
             and x[1] is not ihm.location.FileLocation)
 
     def __call__(self, content_type, id, reference_id, details, file_path,
-                 file_size_bytes):
+                 file_format, file_size_bytes):
         typ = None if content_type is None else content_type.lower()
         f = self.sysr.external_files.get_by_id(
             id, self.type_map.get(typ, ihm.location.FileLocation))
         f.repo = self.sysr.repos.get_by_id(reference_id)
-        f.file_size = self.get_int(file_size_bytes)
+        # IHMCIF dictionary defines file size as a float, although only int
+        # values make sense, so allow for either ints or floats here
+        try:
+            f.file_size = self.get_int(file_size_bytes)
+        except ValueError:
+            f.file_size = self.get_float(file_size_bytes)
         self.copy_if_present(
-            f, locals(), keys=['details'], mapkeys={'file_path': 'path'})
+            f, locals(), keys=['details', 'file_format'],
+            mapkeys={'file_path': 'path'})
         # Handle DOI that is itself a file
         if file_path is None:
             f.path = '.'
 
 
 class _DatasetListHandler(Handler):
     category = '_ihm_dataset_list'
@@ -3687,14 +3740,15 @@
 
 class IHMVariant(Variant):
     """Used to select typical PDBx/IHM file input. See :func:`read`."""
     system_reader = SystemReader
 
     _handlers = [
         _CollectionHandler, _StructHandler, _SoftwareHandler, _CitationHandler,
+        _DatabaseHandler, _DatabaseStatusHandler,
         _AuditAuthorHandler, _GrantHandler, _CitationAuthorHandler,
         _ChemCompHandler, _ChemDescriptorHandler, _EntityHandler,
         _EntitySrcNatHandler, _EntitySrcGenHandler, _EntitySrcSynHandler,
         _StructRefHandler, _StructRefSeqHandler, _StructRefSeqDifHandler,
         _EntityPolyHandler, _EntityPolySeqHandler, _EntityNonPolyHandler,
         _EntityPolySegmentHandler, _StructAsymHandler, _AssemblyDetailsHandler,
         _AssemblyHandler, _ExtRefHandler, _ExtFileHandler, _DatasetListHandler,
```

### Comparing `ihm-1.0/ihm/reference.py` & `ihm-1.1/ihm/reference.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/report.py` & `ihm-1.1/ihm/report.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/representation.py` & `ihm-1.1/ihm/representation.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/restraint.py` & `ihm-1.1/ihm/restraint.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/source.py` & `ihm-1.1/ihm/source.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/startmodel.py` & `ihm-1.1/ihm/startmodel.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/test.py` & `ihm-1.1/ihm/test.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm/util.py` & `ihm-1.1/ihm/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/ihm.egg-info/PKG-INFO` & `ihm-1.1/ihm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ihm
-Version: 1.0
+Version: 1.1
 Summary: Package for handling IHM mmCIF and BinaryCIF files
 Home-page: https://github.com/ihmwg/python-ihm
 Author: Ben Webb
 Author-email: ben@salilab.org
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -55,14 +55,22 @@
 
 On a Fedora or RedHat Enterprise Linux box, install with
 
 ```
 dnf copr enable salilab/salilab; dnf install python3-ihm
 ```
 
+On an Ubuntu LTS box, install from
+[our PPA](https://launchpad.net/~salilab/+archive/ubuntu/ppa) with
+
+```
+apt install software-properties-common; add-apt-repository ppa:salilab/ppa;
+apt install python3-ihm
+```
+
 Alternatively, install with pip:
 
 ```
 pip install ihm
 ```
 
 (Note that pip builds a C extension module for faster parsing of mmCIF files.
```

### Comparing `ihm-1.0/ihm.egg-info/SOURCES.txt` & `ihm-1.1/ihm.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,24 +32,25 @@
 ihm/reference.py
 ihm/report.py
 ihm/representation.py
 ihm/restraint.py
 ihm/source.py
 ihm/startmodel.py
 ihm/test.py
-ihm/util.py
 ihm.egg-info/PKG-INFO
 ihm.egg-info/SOURCES.txt
 ihm.egg-info/dependency_links.txt
 ihm.egg-info/requires.txt
 ihm.egg-info/top_level.txt
+ihm/util/__init__.py
+ihm/util/make_mmcif.py
 src/ihm_format.c
 src/ihm_format.h
 src/ihm_format.i
-src/ihm_format_wrap_1.0.c
+src/ihm_format_wrap_1.1.c
 test/test_analysis.py
 test/test_citations.py
 test/test_cross_linkers.py
 test/test_dataset.py
 test/test_dictionary.py
 test/test_dumper.py
 test/test_edit.py
@@ -67,9 +68,8 @@
 test/test_protocol.py
 test/test_reader.py
 test/test_reference.py
 test/test_report.py
 test/test_representation.py
 test/test_restraint.py
 test/test_startmodel.py
-test/test_util.py
-util/make-mmcif.py
+test/test_util.py
```

### Comparing `ihm-1.0/setup.py` & `ihm-1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     from setuptools import setup, Extension
 except ImportError:
     from distutils.core import setup, Extension
 import sys
 import os
 
-VERSION = "1.0"
+VERSION = "1.1"
 
 copy_args = sys.argv[1:]
 
 # Allow building without the C extension
 build_ext = True
 if '--without-ext' in copy_args:
     build_ext = False
@@ -48,15 +48,15 @@
       description='Package for handling IHM mmCIF and BinaryCIF files',
       long_description=long_description,
       long_description_content_type="text/markdown",
       author='Ben Webb',
       author_email='ben@salilab.org',
       url='https://github.com/ihmwg/python-ihm',
       ext_modules=mod,
-      packages=['ihm'],
+      packages=['ihm', 'ihm.util'],
       install_requires=['msgpack'],
       classifiers=[
           "Programming Language :: Python :: 2.7",
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
           "Intended Audience :: Science/Research",
```

### Comparing `ihm-1.0/src/ihm_format.c` & `ihm-1.1/src/ihm_format.c`

 * *Files identical despite different names*

### Comparing `ihm-1.0/src/ihm_format.h` & `ihm-1.1/src/ihm_format.h`

 * *Files identical despite different names*

### Comparing `ihm-1.0/src/ihm_format.i` & `ihm-1.1/src/ihm_format.i`

 * *Files identical despite different names*

### Comparing `ihm-1.0/src/ihm_format_wrap_1.0.c` & `ihm-1.1/src/ihm_format_wrap_1.1.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 /* ----------------------------------------------------------------------------
  * This file was automatically generated by SWIG (https://www.swig.org).
- * Version 4.2.0
+ * Version 4.2.1
  *
  * Do not make changes to this file unless you know what you are doing - modify
  * the SWIG interface file instead.
  * ----------------------------------------------------------------------------- */
 
 
-#define SWIG_VERSION 0x040200
+#define SWIG_VERSION 0x040201
 #define SWIGPYTHON
 #define SWIG_PYTHON_DIRECTOR_NO_VTABLE
 
 /* -----------------------------------------------------------------------------
  *  This section contains generic SWIG labels for method/variable
  *  declarations/attributes, and other compiler dependent labels.
  * ----------------------------------------------------------------------------- */
@@ -131,20 +131,25 @@
  * are aware a variable isn't used.  So we just silence that warning.
  * See: https://github.com/swig/swig/issues/192 for more discussion.
  */
 #ifdef __INTEL_COMPILER
 # pragma warning disable 592
 #endif
 
-#if __cplusplus >=201103L
+#if defined(__cplusplus) && __cplusplus >=201103L
 # define SWIG_NULLPTR nullptr
 #else
 # define SWIG_NULLPTR NULL
 #endif 
 
+/* -----------------------------------------------------------------------------
+ * swigcompat.swg
+ *
+ * Macros to provide support compatibility with older C and C++ standards.
+ * ----------------------------------------------------------------------------- */
 
 /* C99 and C++11 should provide snprintf, but define SWIG_NO_SNPRINTF
  * if you're missing it.
  */
 #if ((defined __STDC_VERSION__ && __STDC_VERSION__ >= 199901L) || \
      (defined __cplusplus && __cplusplus >= 201103L) || \
      defined SWIG_HAVE_SNPRINTF) && \
@@ -157,15 +162,14 @@
  * enough.
  */
 # define SWIG_snprintf(O,S,F,A) sprintf(O,F,A)
 # define SWIG_snprintf2(O,S,F,A,B) sprintf(O,F,A,B)
 #endif
 
 
-
 #if defined(__GNUC__) && defined(_WIN32) && !defined(SWIG_PYTHON_NO_HYPOT_WORKAROUND)
 /* Workaround for '::hypot' has not been declared', see https://bugs.python.org/issue11566 */
 # include <math.h>
 #endif
 
 #if !defined(PY_SSIZE_T_CLEAN) && !defined(SWIG_NO_PY_SSIZE_T_CLEAN)
 #define PY_SSIZE_T_CLEAN
```

### Comparing `ihm-1.0/test/test_analysis.py` & `ihm-1.1/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_cross_linkers.py` & `ihm-1.1/test/test_cross_linkers.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_dataset.py` & `ihm-1.1/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_dictionary.py` & `ihm-1.1/test/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_dumper.py` & `ihm-1.1/test/test_dumper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1195,15 +1195,16 @@
         repo1 = ihm.location.Repository(doi="foo", details='test repo')
         repo2 = ihm.location.Repository(doi="10.5281/zenodo.46266",
                                         url='nup84-v1.0.zip',
                                         top_directory=os.path.join('foo',
                                                                    'bar'))
         repo3 = ihm.location.Repository(doi="10.5281/zenodo.58025",
                                         url='foo.spd')
-        loc = ihm.location.InputFileLocation(repo=repo1, path='bar')
+        loc = ihm.location.InputFileLocation(repo=repo1, path='bar',
+                                             file_format='TXT')
         system.locations.append(loc)
         # Duplicates should be ignored
         loc = ihm.location.InputFileLocation(repo=repo1, path='bar')
         system.locations.append(loc)
         # Different file, same repository
         loc = ihm.location.InputFileLocation(repo=repo1, path='baz')
         system.locations.append(loc)
@@ -1257,22 +1258,23 @@
 #
 #
 loop_
 _ihm_external_files.id
 _ihm_external_files.reference_id
 _ihm_external_files.file_path
 _ihm_external_files.content_type
+_ihm_external_files.file_format
 _ihm_external_files.file_size_bytes
 _ihm_external_files.details
-1 1 bar 'Input data or restraints' . .
-2 1 baz 'Input data or restraints' . .
-3 2 foo/bar/baz 'Modeling or post-processing output' . .
-4 3 foo.spd 'Input data or restraints' . 'EM micrographs'
-5 3 . 'Input data or restraints' . 'EM micrographs'
-6 4 %s 'Modeling workflow or script' 4 .
+1 1 bar 'Input data or restraints' TXT . .
+2 1 baz 'Input data or restraints' . . .
+3 2 foo/bar/baz 'Modeling or post-processing output' . . .
+4 3 foo.spd 'Input data or restraints' . . 'EM micrographs'
+5 3 . 'Input data or restraints' . . 'EM micrographs'
+6 4 %s 'Modeling workflow or script' . 4 .
 #
 """ % bar.replace(os.sep, '/'))
 
     def test_dataset_dumper_duplicates_details(self):
         """DatasetDumper ignores duplicate datasets with differing details"""
         system = ihm.System()
         dump = ihm.dumper._DatasetDumper()
@@ -5204,10 +5206,54 @@
 _pdbx_entity_branch_link.value_order
 _pdbx_entity_branch_link.details
 1 1 1 NAG CA H1 2 BMC N H2 sing foo
 2 1 2 BMC CA H1 3 FUC N H2 . .
 #
 """)
 
+    def test_database_dumper(self):
+        """Test DatabaseDumper"""
+        system = ihm.System()
+        dumper = ihm.dumper._DatabaseDumper()
+        out = _get_dumper_output(dumper, system)
+        self.assertEqual(out, '')
+
+        system = ihm.System(
+            databases=[ihm.Database(id='foo', code='bar'),
+                       ihm.Database(id='baz', code='1abc', accession='1abcxyz',
+                                    doi='1.2.3.4')])
+        dumper = ihm.dumper._DatabaseDumper()
+        out = _get_dumper_output(dumper, system)
+        self.assertEqual(out, """#
+loop_
+_database_2.database_id
+_database_2.database_code
+_database_2.pdbx_database_accession
+_database_2.pdbx_DOI
+foo bar . .
+baz 1abc 1abcxyz 1.2.3.4
+#
+""")
+
+    def test_database_status_dumper(self):
+        """Test DatabaseStatusDumper"""
+        system = ihm.System()
+        system._database_status = {
+            'status_code': 'REL', 'entry_id': '5FD1',
+            'recvd_initial_deposition_date': '1993-06-29',
+            'deposit_site': ihm.unknown, 'process_site': 'BNL',
+            'sg_entry': None}
+        dumper = ihm.dumper._DatabaseStatusDumper()
+        out = _get_dumper_output(dumper, system)
+        # sort to remove dict order
+        self.assertEqual("\n".join(sorted(out.split('\n'))),
+                         """
+_pdbx_database_status.deposit_site ?
+_pdbx_database_status.entry_id 5FD1
+_pdbx_database_status.process_site BNL
+_pdbx_database_status.recvd_initial_deposition_date 1993-06-29
+_pdbx_database_status.sg_entry .
+_pdbx_database_status.status_code REL""")
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ihm-1.0/test/test_edit.py` & `ihm-1.1/test/test_edit.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_examples.py` & `ihm-1.1/test/test_examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                               cwd=get_example_dir())
         out = get_example_path("output.cif")
 
         # Make sure that a complete output file was produced and that we
         # can read it
         with open(out) as fh:
             contents = fh.readlines()
-        self.assertEqual(len(contents), 70)
+        self.assertEqual(len(contents), 71)
         with open(out) as fh:
             s, = ihm.reader.read(fh)
         os.unlink(out)
 
     def test_ligands_water_example(self):
         """Test ligands_water example"""
         subprocess.check_call([sys.executable, "ligands_water.py"],
```

### Comparing `ihm-1.0/test/test_flr.py` & `ihm-1.1/test/test_flr.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_format.py` & `ihm-1.1/test/test_format.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_format_bcif.py` & `ihm-1.1/test/test_format_bcif.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_geometry.py` & `ihm-1.1/test/test_geometry.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_location.py` & `ihm-1.1/test/test_location.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_main.py` & `ihm-1.1/test/test_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 class Tests(unittest.TestCase):
     def test_system(self):
         """Test System class"""
         s = ihm.System(title='test system')
         self.assertEqual(s.title, 'test system')
         self.assertEqual(s.id, 'model')
+        self.assertEqual(s.databases, [])
 
     def test_chem_comp(self):
         """Test ChemComp class"""
         cc1 = ihm.ChemComp(id='GLY', code='G', code_canonical='G')
         self.assertEqual(cc1.id, 'GLY')
         self.assertEqual(cc1.code, 'G')
         self.assertEqual(cc1.code_canonical, 'G')
```

### Comparing `ihm-1.0/test/test_make_mmcif.py` & `ihm-1.1/test/test_make_mmcif.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,71 +3,72 @@
 import sys
 import unittest
 import subprocess
 
 TOPDIR = os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 utils.set_search_paths(TOPDIR)
 import ihm.reader
+import ihm.util.make_mmcif  # Script should also be importable
 
 
-MAKE_MMCIF = os.path.join(TOPDIR, 'util', 'make-mmcif.py')
+MAKE_MMCIF = os.path.join(TOPDIR, 'ihm', 'util', 'make_mmcif.py')
 
 
 class Tests(unittest.TestCase):
-    @unittest.skipIf(sys.version_info[0] < 3, "make-mmcif.py needs Python 3")
+    @unittest.skipIf(sys.version_info[0] < 3, "make_mmcif.py needs Python 3")
     def test_simple(self):
-        """Simple test of make-mmcif utility script"""
+        """Simple test of make_mmcif utility script"""
         incif = utils.get_input_file_name(TOPDIR, 'struct_only.cif')
         subprocess.check_call([sys.executable, MAKE_MMCIF, incif])
         with open('output.cif') as fh:
             s, = ihm.reader.read(fh)
         self.assertEqual(s.title,
                          'Architecture of Pol II(G) and molecular mechanism '
                          'of transcription regulation by Gdown1')
         os.unlink('output.cif')
 
-    @unittest.skipIf(sys.version_info[0] < 3, "make-mmcif.py needs Python 3")
+    @unittest.skipIf(sys.version_info[0] < 3, "make_mmcif.py needs Python 3")
     def test_non_default_output(self):
-        """Simple test of make-mmcif with non-default output name"""
+        """Simple test of make_mmcif with non-default output name"""
         incif = utils.get_input_file_name(TOPDIR, 'struct_only.cif')
         subprocess.check_call([sys.executable, MAKE_MMCIF, incif,
                                'non-default-output.cif'])
         with open('non-default-output.cif') as fh:
             s, = ihm.reader.read(fh)
         self.assertEqual(s.title,
                          'Architecture of Pol II(G) and molecular mechanism '
                          'of transcription regulation by Gdown1')
         os.unlink('non-default-output.cif')
 
-    @unittest.skipIf(sys.version_info[0] < 3, "make-mmcif.py needs Python 3")
+    @unittest.skipIf(sys.version_info[0] < 3, "make_mmcif.py needs Python 3")
     def test_no_title(self):
-        """Check that make-mmcif adds missing title"""
+        """Check that make_mmcif adds missing title"""
         incif = utils.get_input_file_name(TOPDIR, 'no_title.cif')
         subprocess.check_call([sys.executable, MAKE_MMCIF, incif])
         with open('output.cif') as fh:
             s, = ihm.reader.read(fh)
         self.assertEqual(s.title, 'Auto-generated system')
         os.unlink('output.cif')
 
-    @unittest.skipIf(sys.version_info[0] < 3, "make-mmcif.py needs Python 3")
+    @unittest.skipIf(sys.version_info[0] < 3, "make_mmcif.py needs Python 3")
     def test_bad_usage(self):
-        """Bad usage of make-mmcif utility script"""
+        """Bad usage of make_mmcif utility script"""
         ret = subprocess.call([sys.executable, MAKE_MMCIF])
         self.assertEqual(ret, 2)
 
-    @unittest.skipIf(sys.version_info[0] < 3, "make-mmcif.py needs Python 3")
+    @unittest.skipIf(sys.version_info[0] < 3, "make_mmcif.py needs Python 3")
     def test_same_file(self):
-        """Check that make-mmcif fails if input and output are the same"""
+        """Check that make_mmcif fails if input and output are the same"""
         incif = utils.get_input_file_name(TOPDIR, 'struct_only.cif')
         ret = subprocess.call([sys.executable, MAKE_MMCIF, incif, incif])
         self.assertEqual(ret, 1)
 
-    @unittest.skipIf(sys.version_info[0] < 3, "make-mmcif.py needs Python 3")
+    @unittest.skipIf(sys.version_info[0] < 3, "make_mmcif.py needs Python 3")
     def test_mini(self):
-        """Check that make-mmcif works given only basic atom info"""
+        """Check that make_mmcif works given only basic atom info"""
         incif = utils.get_input_file_name(TOPDIR, 'mini.cif')
         subprocess.check_call([sys.executable, MAKE_MMCIF, incif])
         with open('output.cif') as fh:
             s, = ihm.reader.read(fh)
         self.assertEqual(len(s.state_groups), 1)
         self.assertEqual(len(s.state_groups[0]), 1)
         self.assertEqual(len(s.state_groups[0][0]), 1)
@@ -78,17 +79,17 @@
         chain_a, chain_b, = m.representation
         for chain in chain_a, chain_b:
             self.assertIsInstance(chain, ihm.representation.AtomicSegment)
             self.assertFalse(chain.rigid)
         self.assertEqual(s.title, 'Auto-generated system')
         os.unlink('output.cif')
 
-    @unittest.skipIf(sys.version_info[0] < 3, "make-mmcif.py needs Python 3")
+    @unittest.skipIf(sys.version_info[0] < 3, "make_mmcif.py needs Python 3")
     def test_pass_through(self):
-        """Check that make-mmcif passes through already-compliant files"""
+        """Check that make_mmcif passes through already-compliant files"""
         incif = utils.get_input_file_name(TOPDIR, 'docking.cif')
         subprocess.check_call([sys.executable, MAKE_MMCIF, incif])
         with open('output.cif') as fh:
             s, = ihm.reader.read(fh)
         self.assertEqual(len(s.state_groups), 1)
         self.assertEqual(len(s.state_groups[0]), 1)
         self.assertEqual(len(s.state_groups[0][0]), 1)
@@ -100,17 +101,17 @@
         self.assertIsInstance(chain_a, ihm.representation.AtomicSegment)
         self.assertTrue(chain_a.rigid)
         self.assertIsInstance(chain_b, ihm.representation.FeatureSegment)
         self.assertFalse(chain_b.rigid)
         self.assertEqual(s.title, 'Output from simple-docking example')
         os.unlink('output.cif')
 
-    @unittest.skipIf(sys.version_info[0] < 3, "make-mmcif.py needs Python 3")
+    @unittest.skipIf(sys.version_info[0] < 3, "make_mmcif.py needs Python 3")
     def test_add_polymers(self):
-        """Check that make-mmcif combines polymer information"""
+        """Check that make_mmcif combines polymer information"""
         # mini.cif contains two chains A, B
         incif = utils.get_input_file_name(TOPDIR, 'mini.cif')
         # mini_add.cif also contains A, B; A is the same sequence as mini.cif
         # but B is different (so should be renamed C when we add)
         addcif = utils.get_input_file_name(TOPDIR, 'mini_add.cif')
         subprocess.check_call([sys.executable, MAKE_MMCIF, incif,
                                '--add', addcif])
@@ -144,17 +145,17 @@
         self.assertIs(chain_c.asym_unit.asym, s.asym_units[2])
         for chain in chain_a, chain_c:
             self.assertIsInstance(chain, ihm.representation.AtomicSegment)
             self.assertFalse(chain.rigid)
         self.assertEqual(s.title, 'Auto-generated system')
         os.unlink('output.cif')
 
-    @unittest.skipIf(sys.version_info[0] < 3, "make-mmcif.py needs Python 3")
+    @unittest.skipIf(sys.version_info[0] < 3, "make_mmcif.py needs Python 3")
     def test_add_non_polymers(self):
-        """Check that make-mmcif combines non-polymer information"""
+        """Check that make_mmcif combines non-polymer information"""
         # mini_nonpoly.cif contains two hemes A, B
         incif = utils.get_input_file_name(TOPDIR, 'mini_nonpoly.cif')
         # mini_nonpoly_add.cif also contains A, B; A has the same author
         # provided residue number as mini_nonpoly.cif but B is different
         # (so should be renamed C when we add)
         addcif = utils.get_input_file_name(TOPDIR, 'mini_nonpoly_add.cif')
         subprocess.check_call([sys.executable, MAKE_MMCIF, incif,
```

### Comparing `ihm-1.0/test/test_metadata.py` & `ihm-1.1/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_model.py` & `ihm-1.1/test/test_model.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_multi_state_scheme.py` & `ihm-1.1/test/test_multi_state_scheme.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,15 +382,15 @@
         self.assertEqual(e4.value, 4.0)
         self.assertEqual(e4.unit, 'c')
         self.assertEqual(
             e4.method,
             'equilibrium constant is determined from kinetic rates, kAB/kBA')
 
     def test_equilibrium_constant_eq(self):
-        """Test equality of EquilibriumConstant objetcs"""
+        """Test equality of EquilibriumConstant objects"""
         e_ref1 = ihm.multi_state_scheme.EquilibriumConstant(
             value='1.0',
             unit='a')
         e_equal1 = ihm.multi_state_scheme.EquilibriumConstant(
             value='1.0',
             unit='a')
         eq_unequal1 = ihm.multi_state_scheme.EquilibriumConstant(
@@ -546,15 +546,15 @@
         self.assertRaises(
             ValueError,
             ihm.multi_state_scheme.RelaxationTime,
             value=2.0,
             unit='wrong_unit')
 
     def test_relaxationtime_eq(self):
-        """Test equality of RelaxationTime objetcs"""
+        """Test equality of RelaxationTime objects"""
         r_ref = ihm.multi_state_scheme.RelaxationTime(
             value=1.0,
             unit='milliseconds',
             details='details1',
             dataset_group='dataset_group1',
             file='file1'
         )
```

### Comparing `ihm-1.0/test/test_protocol.py` & `ihm-1.1/test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_reader.py` & `ihm-1.1/test/test_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -910,55 +910,66 @@
 """
         ext_file_cat = """
 loop_
 _ihm_external_files.id
 _ihm_external_files.reference_id
 _ihm_external_files.file_path
 _ihm_external_files.content_type
+_ihm_external_files.file_format
 _ihm_external_files.file_size_bytes
 _ihm_external_files.details
-1 1 scripts/test.py 'Modeling workflow or script' 180 'Test script'
-2 2 foo/bar.txt 'Input data or restraints' . 'Test text'
-3 3 . 'Modeling or post-processing output' . 'Ensemble structures'
-4 3 . . . .
+1 1 scripts/test.py 'Modeling workflow or script' TXT 180 'Test script'
+2 2 foo/bar.txt 'Input data or restraints' TXT 42.0 'Test text'
+3 3 . 'Modeling or post-processing output' . . 'Ensemble structures'
+4 3 . . . . .
+5 3 foo.txt Other . . 'Other file'
 """
         # Order of the categories shouldn't matter
         cif1 = ext_ref_cat + ext_file_cat
         cif2 = ext_file_cat + ext_ref_cat
         for cif in cif1, cif2:
             for fh in cif_file_handles(cif):
                 s, = ihm.reader.read(fh)
-                l1, l2, l3, l4 = s.locations
+                l1, l2, l3, l4, l5 = s.locations
                 self.assertEqual(l1.path, 'scripts/test.py')
                 self.assertEqual(l1.details, 'Test script')
                 self.assertEqual(l1.repo.doi, '10.5281/zenodo.1218053')
+                self.assertIsInstance(l1.file_size, int)
                 self.assertEqual(l1.file_size, 180)
+                self.assertEqual(l1.file_format, 'TXT')
                 self.assertEqual(l1.repo.details, 'test repo')
                 self.assertEqual(l1.__class__,
                                  ihm.location.WorkflowFileLocation)
 
                 self.assertEqual(l2.path, 'foo/bar.txt')
                 self.assertEqual(l2.details, 'Test text')
                 self.assertIsNone(l2.repo)
-                self.assertIsNone(l2.file_size)
+                self.assertIsInstance(l2.file_size, float)
+                self.assertAlmostEqual(l2.file_size, 42.0, delta=0.01)
+                self.assertEqual(l2.file_format, 'TXT')
                 self.assertEqual(l2.__class__, ihm.location.InputFileLocation)
 
                 self.assertEqual(l3.path, '.')
                 self.assertEqual(l3.details, 'Ensemble structures')
                 self.assertIsNone(l3.file_size)
+                self.assertIsNone(l3.file_format)
                 self.assertEqual(l3.repo.doi, '10.5281/zenodo.1218058')
                 self.assertEqual(l3.__class__, ihm.location.OutputFileLocation)
 
                 self.assertEqual(l4.path, '.')
                 self.assertIsNone(l4.file_size)
+                self.assertIsNone(l4.file_format)
                 self.assertIsNone(l4.details)
                 self.assertEqual(l4.repo.doi, '10.5281/zenodo.1218058')
                 # Type is unspecified
                 self.assertEqual(l4.__class__, ihm.location.FileLocation)
 
+                self.assertEqual(l5.content_type, 'Other')
+                self.assertEqual(l5.__class__, ihm.location.FileLocation)
+
     def test_dataset_list_handler(self):
         """Test DatasetListHandler"""
         cif = """
 loop_
 _ihm_dataset_list.id
 _ihm_dataset_list.data_type
 _ihm_dataset_list.database_hosted
@@ -5126,10 +5137,52 @@
         self.assertEqual(lnk2.leaving_atom_id1, 'H1')
         self.assertEqual(lnk2.num2, 3)
         self.assertEqual(lnk2.atom_id2, 'N')
         self.assertEqual(lnk2.leaving_atom_id2, 'H2')
         self.assertIsNone(lnk2.order)
         self.assertIsNone(lnk2.details)
 
+    def test_database_handler(self):
+        """Test DatabaseHandler"""
+        fh = StringIO("""
+loop_
+_database_2.database_id
+_database_2.database_code
+_database_2.pdbx_database_accession
+_database_2.pdbx_DOI
+foo bar . ?
+baz 1abc 1abcxyz 1.2.3.4
+""")
+        s, = ihm.reader.read(fh)
+        d1, d2 = s.databases
+        self.assertEqual(d1.id, 'foo')
+        self.assertEqual(d1.code, 'bar')
+        self.assertIsNone(d1.accession)
+        self.assertIs(d1.doi, ihm.unknown)
+        self.assertEqual(d2.id, 'baz')
+        self.assertEqual(d2.code, '1abc')
+        self.assertEqual(d2.accession, '1abcxyz')
+        self.assertEqual(d2.doi, '1.2.3.4')
+
+    def test_database_status_handler(self):
+        """Test DatabaseStatusHandler"""
+        fh = StringIO("""
+_pdbx_database_status.status_code                     REL
+_pdbx_database_status.entry_id                        5FD1
+_pdbx_database_status.recvd_initial_deposition_date   1993-06-29
+_pdbx_database_status.deposit_site                    ?
+_pdbx_database_status.process_site                    BNL
+_pdbx_database_status.SG_entry                        .
+""")
+        s, = ihm.reader.read(fh)
+        # Should pass through to a dict
+        self.assertEqual(s._database_status,
+                         {'status_code': 'REL',
+                          'entry_id': '5FD1',
+                          'recvd_initial_deposition_date': '1993-06-29',
+                          'deposit_site': ihm.unknown,
+                          'process_site': 'BNL',
+                          'sg_entry': None})
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ihm-1.0/test/test_reference.py` & `ihm-1.1/test/test_reference.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_report.py` & `ihm-1.1/test/test_report.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_representation.py` & `ihm-1.1/test/test_representation.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_restraint.py` & `ihm-1.1/test/test_restraint.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_startmodel.py` & `ihm-1.1/test/test_startmodel.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/test/test_util.py` & `ihm-1.1/test/test_util.py`

 * *Files identical despite different names*

### Comparing `ihm-1.0/util/make-mmcif.py` & `ihm-1.1/ihm/util/make_mmcif.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,27 +180,33 @@
                    default="output.cif", nargs="?")
     p.add_argument("--add", "-a", action='append', metavar="add.cif",
                    help="also add model information from the named mmCIF "
                         "file to the output file")
     return p.parse_args()
 
 
-args = get_args()
+def main():
+    args = get_args()
 
-if (os.path.exists(args.input) and os.path.exists(args.output)
-        and os.path.samefile(args.input, args.output)):
-    raise ValueError("Input and output are the same file")
-
-if args.add:
-    s = add_ihm_info_one_system(args.input)
-    for other in args.add:
-        other_s = add_ihm_info_one_system(other)
-        combine(s, other_s)
-    with open(args.output, 'w') as fhout:
-        ihm.dumper.write(
-            fhout, [s], variant=ihm.dumper.IgnoreVariant(['_audit_conform']))
-else:
-    with open(args.input) as fh:
+    if (os.path.exists(args.input) and os.path.exists(args.output)
+            and os.path.samefile(args.input, args.output)):
+        raise ValueError("Input and output are the same file")
+
+    if args.add:
+        s = add_ihm_info_one_system(args.input)
+        for other in args.add:
+            other_s = add_ihm_info_one_system(other)
+            combine(s, other_s)
         with open(args.output, 'w') as fhout:
             ihm.dumper.write(
-                fhout, [add_ihm_info(s) for s in ihm.reader.read(fh)],
+                fhout, [s],
                 variant=ihm.dumper.IgnoreVariant(['_audit_conform']))
+    else:
+        with open(args.input) as fh:
+            with open(args.output, 'w') as fhout:
+                ihm.dumper.write(
+                    fhout, [add_ihm_info(s) for s in ihm.reader.read(fh)],
+                    variant=ihm.dumper.IgnoreVariant(['_audit_conform']))
+
+
+if __name__ == '__main__':
+    main()
```

