# Comparing `tmp/dbt-hive-1.6.0.tar.gz` & `tmp/dbt_hive-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-hive-1.6.0.tar", last modified: Fri Apr 12 16:23:04 2024, max compression
+gzip compressed data, was "dbt_hive-1.7.0.tar", last modified: Tue May  7 14:51:03 2024, max compression
```

## Comparing `dbt-hive-1.6.0.tar` & `dbt_hive-1.7.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.175416 dbt-hive-1.6.0/
--rw-r--r--   0 jenkins   (1001) users      (100)    11346 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/LICENSE
--rw-r--r--   0 jenkins   (1001) users      (100)       83 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) users      (100)     4934 2024-04-12 16:23:04.175416 dbt-hive-1.6.0/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     4317 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/README.md
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.135417 dbt-hive-1.6.0/dbt/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.135417 dbt-hive-1.6.0/dbt/adapters/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.167416 dbt-hive-1.6.0/dbt/adapters/hive/
--rw-r--r--   0 jenkins   (1001) users      (100)      225 2024-04-12 16:23:03.000000 dbt-hive-1.6.0/dbt/adapters/hive/.env
--rw-r--r--   0 jenkins   (1001) users      (100)     1033 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)      595 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/__version__.py
--rw-r--r--   0 jenkins   (1001) users      (100)     8443 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/cloudera_tracking.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2899 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/column.py
--rw-r--r--   0 jenkins   (1001) users      (100)    16071 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/connections.py
--rw-r--r--   0 jenkins   (1001) users      (100)    20594 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/impl.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2662 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/adapters/hive/relation.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.135417 dbt-hive-1.6.0/dbt/include/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.167416 dbt-hive-1.6.0/dbt/include/hive/
--rw-r--r--   0 jenkins   (1001) users      (100)      629 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)      648 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/dbt_project.yml
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.167416 dbt-hive-1.6.0/dbt/include/hive/macros/
--rw-r--r--   0 jenkins   (1001) users      (100)    11287 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/adapters.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1553 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/apply_grants.sql
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.167416 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.171416 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/
--rw-r--r--   0 jenkins   (1001) users      (100)     5936 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     2378 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/on_schema_change.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     4690 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     2070 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/validate.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     4185 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/seed.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     6916 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/snapshot.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     2056 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/table.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      697 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/materializations/view.sql
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.175416 dbt-hive-1.6.0/dbt/include/hive/macros/utils/
--rw-r--r--   0 jenkins   (1001) users      (100)      719 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/any_value.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      192 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/array_append.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      127 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/array_concat.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      425 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/array_construct.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      665 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/bool_or.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      720 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      669 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/concat.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1615 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/date_trunc.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1592 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/dateadd.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     3069 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/datediff.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      689 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      742 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/hash.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1208 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/last_day.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      514 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/listagg.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      724 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/position.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      894 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/right.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1210 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/split_part.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      662 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/macros/utils/timestamps.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      776 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/dbt/include/hive/sample_profiles.yml
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:23:04.175416 dbt-hive-1.6.0/dbt_hive.egg-info/
--rw-r--r--   0 jenkins   (1001) users      (100)     4934 2024-04-12 16:23:04.000000 dbt-hive-1.6.0/dbt_hive.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     1903 2024-04-12 16:23:04.000000 dbt-hive-1.6.0/dbt_hive.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        1 2024-04-12 16:23:04.000000 dbt-hive-1.6.0/dbt_hive.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) users      (100)      235 2024-04-12 16:23:04.000000 dbt-hive-1.6.0/dbt_hive.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        4 2024-04-12 16:23:04.000000 dbt-hive-1.6.0/dbt_hive.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) users      (100)       38 2024-04-12 16:23:04.175416 dbt-hive-1.6.0/setup.cfg
--rw-r--r--   0 jenkins   (1001) users      (100)     3363 2024-04-12 16:21:43.000000 dbt-hive-1.6.0/setup.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:51:03.444068 dbt_hive-1.7.0/
+-rw-r--r--   0 jenkins   (1001) users      (100)    11346 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/LICENSE
+-rw-r--r--   0 jenkins   (1001) users      (100)       83 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) users      (100)     4934 2024-05-07 14:51:03.444068 dbt_hive-1.7.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     4317 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/README.md
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:51:03.432068 dbt_hive-1.7.0/dbt/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:51:03.432068 dbt_hive-1.7.0/dbt/adapters/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:51:03.436068 dbt_hive-1.7.0/dbt/adapters/hive/
+-rw-r--r--   0 jenkins   (1001) users      (100)      225 2024-05-07 14:51:03.000000 dbt_hive-1.7.0/dbt/adapters/hive/.env
+-rw-r--r--   0 jenkins   (1001) users      (100)     1033 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/adapters/hive/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)      595 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/adapters/hive/__version__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     8443 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/adapters/hive/cloudera_tracking.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2857 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/adapters/hive/column.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    16071 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/adapters/hive/connections.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    20594 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/adapters/hive/impl.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2662 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/adapters/hive/relation.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:51:03.432068 dbt_hive-1.7.0/dbt/include/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:51:03.436068 dbt_hive-1.7.0/dbt/include/hive/
+-rw-r--r--   0 jenkins   (1001) users      (100)      629 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)      648 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/dbt_project.yml
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:51:03.436068 dbt_hive-1.7.0/dbt/include/hive/macros/
+-rw-r--r--   0 jenkins   (1001) users      (100)    11287 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/adapters.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1553 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/apply_grants.sql
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:51:03.436068 dbt_hive-1.7.0/dbt/include/hive/macros/materializations/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:51:03.436068 dbt_hive-1.7.0/dbt/include/hive/macros/materializations/incremental/
+-rw-r--r--   0 jenkins   (1001) users      (100)     5936 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     2378 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/materializations/incremental/on_schema_change.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     4690 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     2070 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     4185 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/materializations/seed.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     6916 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/materializations/snapshot.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     2056 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/materializations/table.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      697 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/materializations/view.sql
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:51:03.440068 dbt_hive-1.7.0/dbt/include/hive/macros/utils/
+-rw-r--r--   0 jenkins   (1001) users      (100)      719 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/any_value.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      192 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/array_append.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      127 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/array_concat.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      425 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/array_construct.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      665 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/bool_or.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      720 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      669 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/concat.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1615 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/date_trunc.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1592 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/dateadd.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     3069 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/datediff.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      689 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      742 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/hash.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1208 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/last_day.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      514 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/listagg.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      724 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/position.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      894 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/right.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1210 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/split_part.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      662 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/macros/utils/timestamps.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      776 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/dbt/include/hive/sample_profiles.yml
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:51:03.440068 dbt_hive-1.7.0/dbt_hive.egg-info/
+-rw-r--r--   0 jenkins   (1001) users      (100)     4934 2024-05-07 14:51:03.000000 dbt_hive-1.7.0/dbt_hive.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     1903 2024-05-07 14:51:03.000000 dbt_hive-1.7.0/dbt_hive.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        1 2024-05-07 14:51:03.000000 dbt_hive-1.7.0/dbt_hive.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)      235 2024-05-07 14:51:03.000000 dbt_hive-1.7.0/dbt_hive.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        4 2024-05-07 14:51:03.000000 dbt_hive-1.7.0/dbt_hive.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)       38 2024-05-07 14:51:03.444068 dbt_hive-1.7.0/setup.cfg
+-rw-r--r--   0 jenkins   (1001) users      (100)     3363 2024-05-07 14:47:18.000000 dbt_hive-1.7.0/setup.py
```

### Comparing `dbt-hive-1.6.0/LICENSE` & `dbt_hive-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/PKG-INFO` & `dbt_hive-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dbt-hive
-Version: 1.6.0
+Version: 1.7.0
 Summary: The Hive adapter plugin for dbt
 Home-page: https://github.com/cloudera/dbt-hive
 Author: Cloudera
 Author-email: innovation-feedback@cloudera.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-core~=1.6.0
+Requires-Dist: dbt-core~=1.7.0
 Requires-Dist: setuptools>=40.3.0
 Requires-Dist: impyla==0.18
 Requires-Dist: sqlparams>=3.0.0
 Requires-Dist: python-decouple>=3.6
 Requires-Dist: protobuf<5,>=4.0.0
 Requires-Dist: kerberos>=1.3.0; platform_system == "Darwin" or platform_system == "Linux"
 Requires-Dist: winkerberos>=0.9.1; platform_system == "Windows"
@@ -29,18 +29,18 @@
 ### Credits
 
 The initial adapter code was developed by bachng2017 who agreed to transfer the ownership and continue active development.
 This code base is now being actively developed and maintained by Cloudera.
 
 ### Requirements
 
-Current version of dbt-hive use dbt-core 1.4.*. We are actively working on supporting the next version of dbt-core 1.5
+Current version of dbt-hive use dbt-core 1.7.*. We are actively working on supporting the next version of dbt-core 1.8
 
 Python >= 3.8
-dbt-core ~= 1.4.*
+dbt-core ~= 1.7.*
 impyla >= 0.18
 
 ### Install
 ```
 pip3 install --user dbt-hive
 ```
```

### Comparing `dbt-hive-1.6.0/README.md` & `dbt_hive-1.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 ### Credits
 
 The initial adapter code was developed by bachng2017 who agreed to transfer the ownership and continue active development.
 This code base is now being actively developed and maintained by Cloudera.
 
 ### Requirements
 
-Current version of dbt-hive use dbt-core 1.4.*. We are actively working on supporting the next version of dbt-core 1.5
+Current version of dbt-hive use dbt-core 1.7.*. We are actively working on supporting the next version of dbt-core 1.8
 
 Python >= 3.8
-dbt-core ~= 1.4.*
+dbt-core ~= 1.7.*
 impyla >= 0.18
 
 ### Install
 ```
 pip3 install --user dbt-hive
 ```
```

### Comparing `dbt-hive-1.6.0/dbt/adapters/hive/__init__.py` & `dbt_hive-1.7.0/dbt/adapters/hive/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/adapters/hive/__version__.py` & `dbt_hive-1.7.0/dbt/adapters/hive/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-version = "1.6.0"
+version = "1.7.0"
```

### Comparing `dbt-hive-1.6.0/dbt/adapters/hive/cloudera_tracking.py` & `dbt_hive-1.7.0/dbt/adapters/hive/cloudera_tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/adapters/hive/column.py` & `dbt_hive-1.7.0/dbt/adapters/hive/column.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from dataclasses import dataclass
 from typing import TypeVar, Optional, Dict, Any
 
 from dbt.adapters.base.column import Column
 from dbt.dataclass_schema import dbtClassMixin
-from hologram import JsonDict
 
 Self = TypeVar("Self", bound="HiveColumn")
 
 
 @dataclass
 class HiveColumn(dbtClassMixin, Column):
     """A  HiveColumn"""
@@ -67,14 +66,14 @@
     #             for key, val in stats.items():
     #                 table_stats[f'stats:{key}:label'] = key
     #                 table_stats[f'stats:{key}:value'] = val
     #                 table_stats[f'stats:{key}:description'] = ''
     #                 table_stats[f'stats:{key}:include'] = True
     #         return table_stats
 
-    def to_column_dict(self, omit_none: bool = True, validate: bool = False) -> JsonDict:
+    def to_column_dict(self, omit_none: bool = True, validate: bool = False):
         original_dict = self.to_dict(omit_none=omit_none)
         # If there are stats, merge them into the root of the dict
         # original_stats = original_dict.pop('table_stats', None)
         # if original_stats:
         #    original_dict.update(original_stats)
         return original_dict
```

### Comparing `dbt-hive-1.6.0/dbt/adapters/hive/connections.py` & `dbt_hive-1.7.0/dbt/adapters/hive/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/adapters/hive/impl.py` & `dbt_hive-1.7.0/dbt/adapters/hive/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/adapters/hive/relation.py` & `dbt_hive-1.7.0/dbt/adapters/hive/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/__init__.py` & `dbt_hive-1.7.0/dbt/include/hive/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/dbt_project.yml` & `dbt_hive-1.7.0/dbt/include/hive/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/adapters.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/apply_grants.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/incremental.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/on_schema_change.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/materializations/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/strategies.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/incremental/validate.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/seed.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/snapshot.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/table.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/materializations/view.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/any_value.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/any_value.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/bool_or.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/bool_or.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/cast_bool_to_text.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/cast_bool_to_text.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/concat.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/concat.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/date_trunc.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/date_trunc.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/dateadd.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/datediff.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/escape_single_quotes.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/escape_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/hash.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/hash.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/last_day.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/listagg.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/position.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/right.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/right.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/split_part.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/macros/utils/timestamps.sql` & `dbt_hive-1.7.0/dbt/include/hive/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt/include/hive/sample_profiles.yml` & `dbt_hive-1.7.0/dbt/include/hive/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/dbt_hive.egg-info/PKG-INFO` & `dbt_hive-1.7.0/dbt_hive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: dbt-hive
-Version: 1.6.0
+Version: 1.7.0
 Summary: The Hive adapter plugin for dbt
 Home-page: https://github.com/cloudera/dbt-hive
 Author: Cloudera
 Author-email: innovation-feedback@cloudera.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-core~=1.6.0
+Requires-Dist: dbt-core~=1.7.0
 Requires-Dist: setuptools>=40.3.0
 Requires-Dist: impyla==0.18
 Requires-Dist: sqlparams>=3.0.0
 Requires-Dist: python-decouple>=3.6
 Requires-Dist: protobuf<5,>=4.0.0
 Requires-Dist: kerberos>=1.3.0; platform_system == "Darwin" or platform_system == "Linux"
 Requires-Dist: winkerberos>=0.9.1; platform_system == "Windows"
@@ -29,18 +29,18 @@
 ### Credits
 
 The initial adapter code was developed by bachng2017 who agreed to transfer the ownership and continue active development.
 This code base is now being actively developed and maintained by Cloudera.
 
 ### Requirements
 
-Current version of dbt-hive use dbt-core 1.4.*. We are actively working on supporting the next version of dbt-core 1.5
+Current version of dbt-hive use dbt-core 1.7.*. We are actively working on supporting the next version of dbt-core 1.8
 
 Python >= 3.8
-dbt-core ~= 1.4.*
+dbt-core ~= 1.7.*
 impyla >= 0.18
 
 ### Install
 ```
 pip3 install --user dbt-hive
 ```
```

### Comparing `dbt-hive-1.6.0/dbt_hive.egg-info/SOURCES.txt` & `dbt_hive-1.7.0/dbt_hive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-hive-1.6.0/setup.py` & `dbt_hive-1.7.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-hive"
 # make sure this always matches dbt/adapters/hive/__version__.py
-package_version = "1.6.0"
+package_version = "1.7.0"
 description = """The Hive adapter plugin for dbt"""
 
 dbt_core_version = _get_dbt_core_version()
 
 setup(
     name=package_name,
     version=package_version,
```

