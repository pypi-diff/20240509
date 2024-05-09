# Comparing `tmp/dbt-spark-1.8.0b2.tar.gz` & `tmp/dbt_spark-1.8.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-spark-1.8.0b2.tar", last modified: Wed Apr  3 21:47:45 2024, max compression
+gzip compressed data, was "dbt_spark-1.8.0rc1.tar", last modified: Mon May  6 23:11:36 2024, max compression
```

## Comparing `dbt-spark-1.8.0b2.tar` & `dbt_spark-1.8.0rc1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.289870 dbt-spark-1.8.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-03 21:47:45.285870 dbt-spark-1.8.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.277870 dbt-spark-1.8.0b2/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.273870 dbt-spark-1.8.0b2/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.277870 dbt-spark-1.8.0b2/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    20528 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.277870 dbt-spark-1.8.0b2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.277870 dbt-spark-1.8.0b2/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.281870 dbt-spark-1.8.0b2/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/apply_grants.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.281870 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/clone.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.281870 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/validate.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.285870 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.285870 dbt-spark-1.8.0b2/dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-03 21:47:45.000000 dbt-spark-1.8.0b2/dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-03 21:47:45.000000 dbt-spark-1.8.0b2/dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:47:45.000000 dbt-spark-1.8.0b2/dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:47:45.000000 dbt-spark-1.8.0b2/dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 21:47:45.000000 dbt-spark-1.8.0b2/dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 21:47:45.000000 dbt-spark-1.8.0b2/dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:47:45.289870 dbt-spark-1.8.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:11:35.997550 dbt_spark-1.8.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-06 23:11:35.997550 dbt_spark-1.8.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:11:35.985550 dbt_spark-1.8.0rc1/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:11:35.985550 dbt_spark-1.8.0rc1/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:11:35.989550 dbt_spark-1.8.0rc1/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20528 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/adapters/spark/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/adapters/spark/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:11:35.985550 dbt_spark-1.8.0rc1/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:11:35.989550 dbt_spark-1.8.0rc1/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:11:35.989550 dbt_spark-1.8.0rc1/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/apply_grants.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:11:35.993550 dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/clone.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:11:35.993550 dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:11:35.993550 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 23:11:35.997550 dbt_spark-1.8.0rc1/dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-05-06 23:11:35.000000 dbt_spark-1.8.0rc1/dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-06 23:11:35.000000 dbt_spark-1.8.0rc1/dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:11:35.000000 dbt_spark-1.8.0rc1/dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 23:11:35.000000 dbt_spark-1.8.0rc1/dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-06 23:11:35.000000 dbt_spark-1.8.0rc1/dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-06 23:11:35.000000 dbt_spark-1.8.0rc1/dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 23:11:35.997550 dbt_spark-1.8.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-06 23:11:24.000000 dbt_spark-1.8.0rc1/setup.py
```

### Comparing `dbt-spark-1.8.0b2/PKG-INFO` & `dbt_spark-1.8.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.8.0b2
+Version: 1.8.0rc1
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.8.0b2 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.8.0rc1 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dbt-spark-1.8.0b2/README.md` & `dbt_spark-1.8.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/adapters/spark/column.py` & `dbt_spark-1.8.0rc1/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/adapters/spark/connections.py` & `dbt_spark-1.8.0rc1/dbt/adapters/spark/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/adapters/spark/impl.py` & `dbt_spark-1.8.0rc1/dbt/adapters/spark/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/adapters/spark/python_submissions.py` & `dbt_spark-1.8.0rc1/dbt/adapters/spark/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/adapters/spark/relation.py` & `dbt_spark-1.8.0rc1/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/adapters/spark/session.py` & `dbt_spark-1.8.0rc1/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/adapters.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/apply_grants.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/clone.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/column_helpers.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/validate.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/seed.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/snapshot.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/table.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/dateadd.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/datediff.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/listagg.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/split_part.sql` & `dbt_spark-1.8.0rc1/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt/include/spark/profile_template.yml` & `dbt_spark-1.8.0rc1/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/dbt_spark.egg-info/PKG-INFO` & `dbt_spark-1.8.0rc1/dbt_spark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.8.0b2
+Version: 1.8.0rc1
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.8.0b2 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.8.0rc1 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dbt-spark-1.8.0b2/dbt_spark.egg-info/SOURCES.txt` & `dbt_spark-1.8.0rc1/dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b2/setup.py` & `dbt_spark-1.8.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         match = re.search(_version_pattern, f.read().strip())
         if match is None:
             raise ValueError(f"invalid version at {_version_path}")
         return match.groupdict()
 
 
 package_name = "dbt-spark"
-package_version = "1.8.0b2"
+package_version = "1.8.0rc1"
 description = """The Apache Spark adapter plugin for dbt"""
 
 odbc_extras = ["pyodbc~=4.0.39"]
 pyhive_extras = [
     "PyHive[hive_pure_sasl]~=0.7.0",
     "thrift>=0.11.0,<0.17.0",
 ]
```

