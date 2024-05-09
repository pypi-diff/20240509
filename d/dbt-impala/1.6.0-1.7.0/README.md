# Comparing `tmp/dbt-impala-1.6.0.tar.gz` & `tmp/dbt_impala-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-impala-1.6.0.tar", last modified: Fri Apr 12 16:22:19 2024, max compression
+gzip compressed data, was "dbt_impala-1.7.0.tar", last modified: Tue May  7 14:48:35 2024, max compression
```

## Comparing `dbt-impala-1.6.0.tar` & `dbt_impala-1.7.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.535736 dbt-impala-1.6.0/
--rw-r--r--   0 jenkins   (1001) users      (100)    10837 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/LICENSE
--rw-r--r--   0 jenkins   (1001) users      (100)       83 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) users      (100)     3196 2024-04-12 16:22:19.535736 dbt-impala-1.6.0/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     2433 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/README.md
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.527736 dbt-impala-1.6.0/dbt/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.527736 dbt-impala-1.6.0/dbt/adapters/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.531736 dbt-impala-1.6.0/dbt/adapters/impala/
--rw-------   0 jenkins   (1001) users      (100)      227 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt/adapters/impala/.env
--rw-r--r--   0 jenkins   (1001) users      (100)     1062 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)      596 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/__version__.py
--rw-r--r--   0 jenkins   (1001) users      (100)     8443 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/cloudera_tracking.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2771 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/column.py
--rw-r--r--   0 jenkins   (1001) users      (100)    15338 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/connections.py
--rw-r--r--   0 jenkins   (1001) users      (100)    15711 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/impl.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2431 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/adapters/impala/relation.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.527736 dbt-impala-1.6.0/dbt/include/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.531736 dbt-impala-1.6.0/dbt/include/impala/
--rw-r--r--   0 jenkins   (1001) users      (100)      630 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)      651 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/dbt_project.yml
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.531736 dbt-impala-1.6.0/dbt/include/impala/macros/
--rw-r--r--   0 jenkins   (1001) users      (100)    15594 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/adapters.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1591 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/apply_grants.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      676 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/catalog.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     6325 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/incremental.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1899 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/insertoverwrite.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1877 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/seed.sql
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.535736 dbt-impala-1.6.0/dbt/include/impala/macros/utils/
--rw-r--r--   0 jenkins   (1001) users      (100)      721 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/any_value.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      157 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/array_append.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      155 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/array_concat.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      159 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/array_construct.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      751 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/bool_or.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      672 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/concat.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      750 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/dateadd.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     5180 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/datediff.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      696 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      825 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/hash.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1208 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/last_day.sql
--rw-r--r--   0 jenkins   (1001) users      (100)     1106 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/listagg.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      727 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/position.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      863 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/split_part.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      665 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/macros/utils/timestamps.sql
--rw-r--r--   0 jenkins   (1001) users      (100)      779 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/dbt/include/impala/sample_profiles.yml
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-04-12 16:22:19.535736 dbt-impala-1.6.0/dbt_impala.egg-info/
--rw-r--r--   0 jenkins   (1001) users      (100)     3196 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt_impala.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     1544 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt_impala.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        1 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt_impala.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        1 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt_impala.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) users      (100)       50 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt_impala.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        4 2024-04-12 16:22:19.000000 dbt-impala-1.6.0/dbt_impala.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) users      (100)       38 2024-04-12 16:22:19.535736 dbt-impala-1.6.0/setup.cfg
--rw-r--r--   0 jenkins   (1001) users      (100)     3118 2024-04-12 16:21:48.000000 dbt-impala-1.6.0/setup.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:48:35.872305 dbt_impala-1.7.0/
+-rw-r--r--   0 jenkins   (1001) users      (100)    10837 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/LICENSE
+-rw-r--r--   0 jenkins   (1001) users      (100)       83 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) users      (100)     3151 2024-05-07 14:48:35.872305 dbt_impala-1.7.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     2388 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/README.md
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:48:35.860305 dbt_impala-1.7.0/dbt/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:48:35.860305 dbt_impala-1.7.0/dbt/adapters/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:48:35.864305 dbt_impala-1.7.0/dbt/adapters/impala/
+-rw-------   0 jenkins   (1001) users      (100)      227 2024-05-07 14:48:35.000000 dbt_impala-1.7.0/dbt/adapters/impala/.env
+-rw-r--r--   0 jenkins   (1001) users      (100)     1062 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/adapters/impala/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)      596 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/adapters/impala/__version__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     8443 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/adapters/impala/cloudera_tracking.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2729 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/adapters/impala/column.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    15338 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/adapters/impala/connections.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    15711 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/adapters/impala/impl.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2431 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/adapters/impala/relation.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:48:35.864305 dbt_impala-1.7.0/dbt/include/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:48:35.864305 dbt_impala-1.7.0/dbt/include/impala/
+-rw-r--r--   0 jenkins   (1001) users      (100)      630 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)      651 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/dbt_project.yml
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:48:35.868305 dbt_impala-1.7.0/dbt/include/impala/macros/
+-rw-r--r--   0 jenkins   (1001) users      (100)    15594 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/adapters.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1591 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/apply_grants.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      676 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/catalog.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     6325 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/incremental.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1899 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/insertoverwrite.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1877 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/seed.sql
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:48:35.868305 dbt_impala-1.7.0/dbt/include/impala/macros/utils/
+-rw-r--r--   0 jenkins   (1001) users      (100)      721 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/any_value.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      157 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/array_append.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      155 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/array_concat.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      159 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/array_construct.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      751 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/bool_or.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      672 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/concat.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      750 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/dateadd.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     5180 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/datediff.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      696 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      825 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/hash.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1208 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/last_day.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)     1106 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/listagg.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      727 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/position.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      863 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/split_part.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      665 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/macros/utils/timestamps.sql
+-rw-r--r--   0 jenkins   (1001) users      (100)      779 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/dbt/include/impala/sample_profiles.yml
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2024-05-07 14:48:35.872305 dbt_impala-1.7.0/dbt_impala.egg-info/
+-rw-r--r--   0 jenkins   (1001) users      (100)     3151 2024-05-07 14:48:35.000000 dbt_impala-1.7.0/dbt_impala.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     1544 2024-05-07 14:48:35.000000 dbt_impala-1.7.0/dbt_impala.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        1 2024-05-07 14:48:35.000000 dbt_impala-1.7.0/dbt_impala.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        1 2024-05-07 14:48:35.000000 dbt_impala-1.7.0/dbt_impala.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) users      (100)       50 2024-05-07 14:48:35.000000 dbt_impala-1.7.0/dbt_impala.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        4 2024-05-07 14:48:35.000000 dbt_impala-1.7.0/dbt_impala.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)       38 2024-05-07 14:48:35.872305 dbt_impala-1.7.0/setup.cfg
+-rw-r--r--   0 jenkins   (1001) users      (100)     3118 2024-05-07 14:47:12.000000 dbt_impala-1.7.0/setup.py
```

### Comparing `dbt-impala-1.6.0/LICENSE` & `dbt_impala-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/PKG-INFO` & `dbt_impala-1.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dbt-impala
-Version: 1.6.0
+Version: 1.7.0
 Summary: Impala adapter for DBT
 Home-page: https://github.com/cloudera/dbt-impala
 Author: Cloudera
 Author-email: innovation-feedback@cloudera.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-core~=1.6.0
+Requires-Dist: dbt-core~=1.7.0
 Requires-Dist: impyla==0.18
 Requires-Dist: python-decouple>=3.6
 
 # dbt-impala
 
 The `dbt-impala` adapter allows you to use [dbt](https://www.getdbt.com/) along with [Apache Impala](https://impala.apache.org/) and [Cloudera Data Platform](https://cloudera.com)
 
@@ -27,19 +27,18 @@
 ## Getting started
 
 - [Install dbt](https://docs.getdbt.com/docs/installation)
 - Read the [introduction](https://docs.getdbt.com/docs/introduction/) and [viewpoint](https://docs.getdbt.com/docs/about/viewpoint/)
 
 ### Requirements
 
-Current version of dbt-impala work only with dbt-core 1.4 but not with dbt-core >= 1.5.
-We are actively working on next release 1.5 which will work with dbt-core 1.5
+Current version of dbt-impala use dbt-core 1.7.*. We are actively working on supporting the next version of dbt-core 1.8
 
 Python >= 3.7
-dbt-core == 1.3.*
+dbt-core == 1.7.*
 
 For development/testing or contribution to the dbt-impala, please follow [Contributing](CONTRIBUTING.md) guidelines.
 
 ### Installing dbt-impala
 
 `pip install dbt-impala`
```

### Comparing `dbt-impala-1.6.0/README.md` & `dbt_impala-1.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 ## Getting started
 
 - [Install dbt](https://docs.getdbt.com/docs/installation)
 - Read the [introduction](https://docs.getdbt.com/docs/introduction/) and [viewpoint](https://docs.getdbt.com/docs/about/viewpoint/)
 
 ### Requirements
 
-Current version of dbt-impala work only with dbt-core 1.4 but not with dbt-core >= 1.5.
-We are actively working on next release 1.5 which will work with dbt-core 1.5
+Current version of dbt-impala use dbt-core 1.7.*. We are actively working on supporting the next version of dbt-core 1.8
 
 Python >= 3.7
-dbt-core == 1.3.*
+dbt-core == 1.7.*
 
 For development/testing or contribution to the dbt-impala, please follow [Contributing](CONTRIBUTING.md) guidelines.
 
 ### Installing dbt-impala
 
 `pip install dbt-impala`
```

### Comparing `dbt-impala-1.6.0/dbt/adapters/impala/__init__.py` & `dbt_impala-1.7.0/dbt/adapters/impala/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/adapters/impala/__version__.py` & `dbt_impala-1.7.0/dbt/adapters/impala/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-version = "1.6.0"
+version = "1.7.0"
```

### Comparing `dbt-impala-1.6.0/dbt/adapters/impala/cloudera_tracking.py` & `dbt_impala-1.7.0/dbt/adapters/impala/cloudera_tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/adapters/impala/column.py` & `dbt_impala-1.7.0/dbt/adapters/impala/column.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 from dataclasses import dataclass
 from typing import TypeVar, Optional, Dict, Any
 
 from dbt.adapters.base.column import Column
 from dbt.dataclass_schema import dbtClassMixin
-from hologram import JsonDict
 
 Self = TypeVar("Self", bound="ImpalaColumn")
 
 
 @dataclass
 class ImpalaColumn(dbtClassMixin, Column):
     table_database: Optional[str] = None
@@ -65,15 +64,15 @@
             for key, val in stats.items():
                 table_stats[f"stats:{key}:label"] = key
                 table_stats[f"stats:{key}:value"] = val
                 table_stats[f"stats:{key}:description"] = ""
                 table_stats[f"stats:{key}:include"] = True
         return table_stats
 
-    def to_column_dict(self, omit_none: bool = True, validate: bool = False) -> JsonDict:
+    def to_column_dict(self, omit_none: bool = True, validate: bool = False):
         original_dict = self.to_dict(omit_none=omit_none)
 
         # If there are stats, merge them into the root of the dict
         original_stats = original_dict.pop("table_stats", None)
         if original_stats:
             original_dict.update(original_stats)
         return original_dict
```

### Comparing `dbt-impala-1.6.0/dbt/adapters/impala/connections.py` & `dbt_impala-1.7.0/dbt/adapters/impala/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/adapters/impala/impl.py` & `dbt_impala-1.7.0/dbt/adapters/impala/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/adapters/impala/relation.py` & `dbt_impala-1.7.0/dbt/adapters/impala/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/__init__.py` & `dbt_impala-1.7.0/dbt/include/impala/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/dbt_project.yml` & `dbt_impala-1.7.0/dbt/include/impala/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/adapters.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/apply_grants.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/catalog.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/incremental.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/insertoverwrite.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/insertoverwrite.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/seed.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/utils/any_value.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/utils/any_value.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/utils/bool_or.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/utils/bool_or.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/utils/concat.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/utils/concat.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/utils/dateadd.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/utils/datediff.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/utils/escape_single_quotes.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/utils/escape_single_quotes.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/utils/hash.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/utils/hash.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/utils/last_day.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/utils/listagg.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/utils/position.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/utils/split_part.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/macros/utils/timestamps.sql` & `dbt_impala-1.7.0/dbt/include/impala/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt/include/impala/sample_profiles.yml` & `dbt_impala-1.7.0/dbt/include/impala/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/dbt_impala.egg-info/PKG-INFO` & `dbt_impala-1.7.0/dbt_impala.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: dbt-impala
-Version: 1.6.0
+Version: 1.7.0
 Summary: Impala adapter for DBT
 Home-page: https://github.com/cloudera/dbt-impala
 Author: Cloudera
 Author-email: innovation-feedback@cloudera.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dbt-core~=1.6.0
+Requires-Dist: dbt-core~=1.7.0
 Requires-Dist: impyla==0.18
 Requires-Dist: python-decouple>=3.6
 
 # dbt-impala
 
 The `dbt-impala` adapter allows you to use [dbt](https://www.getdbt.com/) along with [Apache Impala](https://impala.apache.org/) and [Cloudera Data Platform](https://cloudera.com)
 
@@ -27,19 +27,18 @@
 ## Getting started
 
 - [Install dbt](https://docs.getdbt.com/docs/installation)
 - Read the [introduction](https://docs.getdbt.com/docs/introduction/) and [viewpoint](https://docs.getdbt.com/docs/about/viewpoint/)
 
 ### Requirements
 
-Current version of dbt-impala work only with dbt-core 1.4 but not with dbt-core >= 1.5.
-We are actively working on next release 1.5 which will work with dbt-core 1.5
+Current version of dbt-impala use dbt-core 1.7.*. We are actively working on supporting the next version of dbt-core 1.8
 
 Python >= 3.7
-dbt-core == 1.3.*
+dbt-core == 1.7.*
 
 For development/testing or contribution to the dbt-impala, please follow [Contributing](CONTRIBUTING.md) guidelines.
 
 ### Installing dbt-impala
 
 `pip install dbt-impala`
```

### Comparing `dbt-impala-1.6.0/dbt_impala.egg-info/SOURCES.txt` & `dbt_impala-1.7.0/dbt_impala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-impala-1.6.0/setup.py` & `dbt_impala-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-impala"
 # make sure this always matches dbt/adapters/dbt_impala/__version__.py
-package_version = "1.6.0"
+package_version = "1.7.0"
 description = """The Impala adapter plugin for dbt"""
 
 dbt_core_version = _get_dbt_core_version()
 
 setup(
     name=package_name,
     version=package_version,
```

