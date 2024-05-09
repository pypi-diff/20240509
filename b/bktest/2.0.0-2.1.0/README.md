# Comparing `tmp/bktest-2.0.0.tar.gz` & `tmp/bktest-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bktest-2.0.0.tar", last modified: Thu Jan 25 12:25:16 2024, max compression
+gzip compressed data, was "bktest-2.1.0.tar", last modified: Thu May  9 09:36:18 2024, max compression
```

## Comparing `bktest-2.0.0.tar` & `bktest-2.1.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 12:25:16.036512 bktest-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10962 2024-01-25 12:25:16.036512 bktest-2.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     9795 2024-01-25 12:25:07.000000 bktest-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 12:25:16.028512 bktest-2.0.0/bktest/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)    21962 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 12:25:16.028512 bktest-2.0.0/bktest/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/data/holidays.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 12:25:16.032512 bktest-2.0.0/bktest/data/source/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/data/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/data/source/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/data/source/coinmarketcap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/data/source/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/data/source/delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/data/source/factset.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/data/source/yahoo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 12:25:16.032512 bktest-2.0.0/bktest/export/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/export/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/export/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/export/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/export/influx.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/export/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/export/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/export/quants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/export/specific_return.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/fee.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/holding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/price_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 12:25:16.032512 bktest-2.0.0/bktest/template/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/template/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/template/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/template/sketch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/template/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-25 12:25:07.000000 bktest-2.0.0/bktest/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 12:25:16.036512 bktest-2.0.0/bktest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10962 2024-01-25 12:25:16.000000 bktest-2.0.0/bktest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-01-25 12:25:16.000000 bktest-2.0.0/bktest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 12:25:16.000000 bktest-2.0.0/bktest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-25 12:25:16.000000 bktest-2.0.0/bktest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 12:25:16.000000 bktest-2.0.0/bktest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-25 12:25:16.000000 bktest-2.0.0/bktest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-25 12:25:16.000000 bktest-2.0.0/bktest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 12:25:16.036512 bktest-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-01-25 12:25:07.000000 bktest-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 12:25:16.036512 bktest-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 12:25:07.000000 bktest-2.0.0/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6772 2024-01-25 12:25:07.000000 bktest-2.0.0/tests/test_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-01-25 12:25:07.000000 bktest-2.0.0/tests/test_data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-01-25 12:25:07.000000 bktest-2.0.0/tests/test_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-01-25 12:25:07.000000 bktest-2.0.0/tests/test_holdings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-01-25 12:25:07.000000 bktest-2.0.0/tests/test_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-01-25 12:25:07.000000 bktest-2.0.0/tests/test_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-01-25 12:25:07.000000 bktest-2.0.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:36:18.915528 bktest-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-05-09 09:36:18.911528 bktest-2.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9003 2024-05-09 09:36:14.000000 bktest-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:36:18.907528 bktest-2.1.0/bktest/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10604 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21697 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:36:18.907528 bktest-2.1.0/bktest/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/data/holidays.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:36:18.911528 bktest-2.1.0/bktest/data/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/data/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/data/source/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/data/source/coinmarketcap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/data/source/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/data/source/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/data/source/factset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/data/source/yahoo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:36:18.911528 bktest-2.1.0/bktest/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/export/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/export/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/export/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/export/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/export/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/export/quants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/export/specific_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/holding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/price_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:36:18.911528 bktest-2.1.0/bktest/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/template/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11253 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/template/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/template/sketch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-09 09:36:14.000000 bktest-2.1.0/bktest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:36:18.911528 bktest-2.1.0/bktest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-05-09 09:36:18.000000 bktest-2.1.0/bktest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-09 09:36:18.000000 bktest-2.1.0/bktest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:36:18.000000 bktest-2.1.0/bktest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-09 09:36:18.000000 bktest-2.1.0/bktest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:36:18.000000 bktest-2.1.0/bktest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-09 09:36:18.000000 bktest-2.1.0/bktest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 09:36:18.000000 bktest-2.1.0/bktest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 09:36:18.915528 bktest-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-09 09:36:14.000000 bktest-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:36:18.911528 bktest-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:36:14.000000 bktest-2.1.0/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6772 2024-05-09 09:36:14.000000 bktest-2.1.0/tests/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-09 09:36:14.000000 bktest-2.1.0/tests/test_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-09 09:36:14.000000 bktest-2.1.0/tests/test_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-09 09:36:14.000000 bktest-2.1.0/tests/test_holdings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-09 09:36:14.000000 bktest-2.1.0/tests/test_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-09 09:36:14.000000 bktest-2.1.0/tests/test_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-09 09:36:14.000000 bktest-2.1.0/tests/test_utils.py
```

### Comparing `bktest-2.0.0/PKG-INFO` & `bktest-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: bktest
-Version: 2.0.0
+Version: 2.1.0
 Summary: bktest - A simple backtester by CrunchDAO
 Home-page: https://github.com/crunchdao/backtest
 Author: Enzo CACERES
 Author-email: enzo.caceres@crunchdao.com
 Keywords: package development template
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: click<8.1.2,>=8.0
 Requires-Dist: pandas<2.0.0,>=1.5
 Requires-Dist: python-dateutil<2.8.3,>=2.8.2
 Requires-Dist: tqdm<4.65.0,>=4.48.0
-Requires-Dist: influxdb<5.3.1,>=5.2.2
 Requires-Dist: numpy<1.25.0,>=1.23.0
 Requires-Dist: py_expression_eval<0.3.14,>=0.3.9
 Requires-Dist: pyarrow<12.0,>=11.0
 Requires-Dist: quantstats==0.0.62
 Requires-Dist: pytest<7.3.0,>=7.1.0
 Requires-Dist: yfinance<0.2.27,>=0.2.24
 Requires-Dist: python-dotenv<1.0.0,>=0.20
@@ -28,28 +27,28 @@
 Requires-Dist: python-slugify
 Requires-Dist: cached-property
 Requires-Dist: fpdf2==2.7.4
 Requires-Dist: contexttimer
 Requires-Dist: watchdog
 Requires-Dist: fastparquet
 Requires-Dist: readwrite
+Requires-Dist: holidays
 
 A small backtesting utility.
 
 ![image](https://user-images.githubusercontent.com/7386242/189368488-b0c30d48-9a1f-4362-9f78-10a451535682.png)
 
 [![PyTest](https://github.com/crunchdao/backtest/actions/workflows/pytest.yml/badge.svg)](https://github.com/crunchdao/backtest/actions/workflows/pytest.yml)
 
 - [Install](#install)
 - [Usage](#usage)
   - [Options](#options)
     - [Exporters](#exporters)
       - [Console](#console)
       - [Dump](#dump)
-      - [Influx](#influx)
       - [QuantStats](#quantstats)
       - [PDF](#pdf)
       - [Specific Return](#specific-return)
     - [Data Sources](#data-sources)
       - [Yahoo](#yahoo)
       - [CoinMarketCap](#coinmarketcap)
       - [FactSet](#factset)
@@ -70,31 +69,31 @@
 
 ## Options
 
 | Option | Value | Default | Format | Description |
 | --- | --- | --- | --- | --- |
 | `--start` | `<start date>` | `orders' first date` | `date` (ISO-8601) | The starting date of the backtesting. If the value is before the first ordering day, the value will be discarded. |
 | `--end` | `<end date>` | `orders' last date` | `date` (ISO-8601) | The ending date of the backtesting. If the value is after today, the value will be discarded. |
-| `--offset-before-trading` | `<days>` | `1` | `int` | Number of day to offset to push the signal before trading it. |
+| `--offset-before-trading` | `<days>` | `1` | `int` | Number of day to offset to push each date of the portfolio before trading it. |
 | `--offset-before-ending` | `<days>` | `0` | `int` | Number of day to continue the backtest after every orders. |
 | `--order-file` | `<file>` | | `path` | The single order file to use. The file must contain symbol, quantity and date information. |
 | `--single-file-provider-column-date` | `<column>` | `date` | `string` | Change the date column name to use. |
 | `--single-file-provider-column-symbol` | `<column>` | `symbol` | `string` | Change the symbol column name to use. |
 | `--single-file-provider-column-quantity` | `<column>` | `quantity` | `string` | Change the quantity column name to use. |
 | `--order-files` | `<directory>` | | `path` | The directory of order file to use. The filename must be a date. The file must contain symbol and quantity information. |
 | `--order-files-extension` | `<extension>` | `csv`  | `[csv, parquet, json]` | Change the file extension to use when listing for order files. |
 | `--initial-cash` | `<amount>` | `100_000` | `number` | Change the initial cash to use for the backtesting. |
 | `--quantity-mode` | `<mode>` | `percent` | `[percent, share]` | If the mode is `share`, all quantities will be interpreted as integers. If the mode is `percent`, all values will be multiplied by the current cash value. |
-| `--auto-close-others` | | `false` | | Should other position be closed after an ordering? |
 | `--weekends` | | `false` | | Enable ordering on weekends. |
 | `--holidays` | | `false` | | Enable ordering on holidays. |
 | `--symbol-mapping` | `<mapping>` | | `path` (.json) | Specify a custom symbol mapping file enabling vendor-id translation. |
 | `--no-caching` | | `false` | | Disable prices caching. |
 | `--fee-model` | `<model>` | | `expression` or `constant` | Specify a fee model to use. The value can be a `constant`. Or an expression that allow the usage of the `price` and `quantity` variable. <br /> Example: `abs(price * quantity) * 0.1` |
-| `--rfr-file` | `<directory>` | | `path` | The directory of rfr file to use. The file must contain a column with date information and a column with the rfr information in %. |
+| `--holiday-provider` | `<name>` | `nyse` | `[legacy, nyse]` | Specify which holiday provider to use. |
+| `--rfr-file` | `<directory>` |  | `path` | The directory of rfr file to use. The file must contain a column with date information and a column with the rfr information in %. |
 | `--rfr-file-column-date` | `<column>` | `date` | `string` | Change the date column name to use. |
 
 ### Exporters
 
 Multiple exporters can be enabled at one time.
 
 #### Console
@@ -115,28 +114,14 @@
 
 | Option | Value | Default | Format | Description |
 | --- | --- | --- | --- | --- |
 | `--dump` | | `false` | | Enable the dump exporter. |
 | `--dump-output-file` | `<file>` | `dump.csv` | `path` | Specify the output file. |
 | `--dump-auto-delete` | | `false` | | Automatically delete the previous dump file if it is present. |
 
-#### Influx
-
-Export the generated data to an Influx database. <br />
-Making it easier to plot the values using software like Grafana.
-
-| Option | Value | Default | Format | Description |
-| --- | --- | --- | --- | --- |
-| `--influx` | | `false` | | Enable the influx exporter. |
-| `--influx-host` | `<host>` | `localhost` | `string` | Specify the remote influx address. |
-| `--influx-port` | `<port>` | `8086` | `number` | Specify the remote influx port. |
-| `--influx-database` | `<database>` | `backtest` | `string` | Specify the influx database to use. |
-| `--influx-measurement` | `<measurement>` | `snapshots` |`string` | Specify the table name to use. |
-| `--influx-key` | `<key>` | `test` | `string` | Specify the unique key to use. **Previous data with the same key will be deleted!** |
-
 #### QuantStats
 
 Generate a tearsheet from the backtest data.
 
 | Option | Value | Default | Format | Description |
 | --- | --- | --- | --- | --- |
 | `--quantstats` | | `false` | | Enable the quantstats exporter. |
```

### Comparing `bktest-2.0.0/README.md` & `bktest-2.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 - [Install](#install)
 - [Usage](#usage)
   - [Options](#options)
     - [Exporters](#exporters)
       - [Console](#console)
       - [Dump](#dump)
-      - [Influx](#influx)
       - [QuantStats](#quantstats)
       - [PDF](#pdf)
       - [Specific Return](#specific-return)
     - [Data Sources](#data-sources)
       - [Yahoo](#yahoo)
       - [CoinMarketCap](#coinmarketcap)
       - [FactSet](#factset)
@@ -35,31 +34,31 @@
 
 ## Options
 
 | Option | Value | Default | Format | Description |
 | --- | --- | --- | --- | --- |
 | `--start` | `<start date>` | `orders' first date` | `date` (ISO-8601) | The starting date of the backtesting. If the value is before the first ordering day, the value will be discarded. |
 | `--end` | `<end date>` | `orders' last date` | `date` (ISO-8601) | The ending date of the backtesting. If the value is after today, the value will be discarded. |
-| `--offset-before-trading` | `<days>` | `1` | `int` | Number of day to offset to push the signal before trading it. |
+| `--offset-before-trading` | `<days>` | `1` | `int` | Number of day to offset to push each date of the portfolio before trading it. |
 | `--offset-before-ending` | `<days>` | `0` | `int` | Number of day to continue the backtest after every orders. |
 | `--order-file` | `<file>` | | `path` | The single order file to use. The file must contain symbol, quantity and date information. |
 | `--single-file-provider-column-date` | `<column>` | `date` | `string` | Change the date column name to use. |
 | `--single-file-provider-column-symbol` | `<column>` | `symbol` | `string` | Change the symbol column name to use. |
 | `--single-file-provider-column-quantity` | `<column>` | `quantity` | `string` | Change the quantity column name to use. |
 | `--order-files` | `<directory>` | | `path` | The directory of order file to use. The filename must be a date. The file must contain symbol and quantity information. |
 | `--order-files-extension` | `<extension>` | `csv`  | `[csv, parquet, json]` | Change the file extension to use when listing for order files. |
 | `--initial-cash` | `<amount>` | `100_000` | `number` | Change the initial cash to use for the backtesting. |
 | `--quantity-mode` | `<mode>` | `percent` | `[percent, share]` | If the mode is `share`, all quantities will be interpreted as integers. If the mode is `percent`, all values will be multiplied by the current cash value. |
-| `--auto-close-others` | | `false` | | Should other position be closed after an ordering? |
 | `--weekends` | | `false` | | Enable ordering on weekends. |
 | `--holidays` | | `false` | | Enable ordering on holidays. |
 | `--symbol-mapping` | `<mapping>` | | `path` (.json) | Specify a custom symbol mapping file enabling vendor-id translation. |
 | `--no-caching` | | `false` | | Disable prices caching. |
 | `--fee-model` | `<model>` | | `expression` or `constant` | Specify a fee model to use. The value can be a `constant`. Or an expression that allow the usage of the `price` and `quantity` variable. <br /> Example: `abs(price * quantity) * 0.1` |
-| `--rfr-file` | `<directory>` | | `path` | The directory of rfr file to use. The file must contain a column with date information and a column with the rfr information in %. |
+| `--holiday-provider` | `<name>` | `nyse` | `[legacy, nyse]` | Specify which holiday provider to use. |
+| `--rfr-file` | `<directory>` |  | `path` | The directory of rfr file to use. The file must contain a column with date information and a column with the rfr information in %. |
 | `--rfr-file-column-date` | `<column>` | `date` | `string` | Change the date column name to use. |
 
 ### Exporters
 
 Multiple exporters can be enabled at one time.
 
 #### Console
@@ -80,28 +79,14 @@
 
 | Option | Value | Default | Format | Description |
 | --- | --- | --- | --- | --- |
 | `--dump` | | `false` | | Enable the dump exporter. |
 | `--dump-output-file` | `<file>` | `dump.csv` | `path` | Specify the output file. |
 | `--dump-auto-delete` | | `false` | | Automatically delete the previous dump file if it is present. |
 
-#### Influx
-
-Export the generated data to an Influx database. <br />
-Making it easier to plot the values using software like Grafana.
-
-| Option | Value | Default | Format | Description |
-| --- | --- | --- | --- | --- |
-| `--influx` | | `false` | | Enable the influx exporter. |
-| `--influx-host` | `<host>` | `localhost` | `string` | Specify the remote influx address. |
-| `--influx-port` | `<port>` | `8086` | `number` | Specify the remote influx port. |
-| `--influx-database` | `<database>` | `backtest` | `string` | Specify the influx database to use. |
-| `--influx-measurement` | `<measurement>` | `snapshots` |`string` | Specify the table name to use. |
-| `--influx-key` | `<key>` | `test` | `string` | Specify the unique key to use. **Previous data with the same key will be deleted!** |
-
 #### QuantStats
 
 Generate a tearsheet from the backtest data.
 
 | Option | Value | Default | Format | Description |
 | --- | --- | --- | --- | --- |
 | `--quantstats` | | `false` | | Enable the quantstats exporter. |
```

### Comparing `bktest-2.0.0/bktest/account.py` & `bktest-2.1.0/bktest/account.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/backtest.py` & `bktest-2.1.0/bktest/backtest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import sys
 import typing
 
 from .account import Account
+from .data.holidays import HolidayProvider, LegacyHolidayProvider
 from .data.source.base import DataSource
 from .export import Exporter, ExporterCollection
 from .fee import ConstantFeeModel, FeeModel
 from .order import Order, OrderProvider, ParallelOrderProvider, OrderResultCollection
 from .price_provider import PriceProvider, SymbolMapper
 from .iterator import DateIterator
 
@@ -145,16 +146,17 @@
         quantity_in_decimal: bool,
         data_source: DataSource,
         auto_close_others: bool = True,
         exporters_factory: typing.Callable[[int], typing.List[Exporter]] = lambda index: [],
         mapper: SymbolMapper = None,
         fee_model: FeeModel = ConstantFeeModel(0.0),
         caching=True,
-        weekends=False,
-        holidays=False,
+        allow_weekends=False,
+        allow_holidays=False,
+        holiday_provider: HolidayProvider = LegacyHolidayProvider(),
     ):
         self.order_provider = order_provider
         order_dates = order_provider.get_dates()
         start = max(next(iter(order_dates)), start) if len(order_dates) else None
 
         self.price_provider = PriceProvider(start, end, data_source, mapper, caching=caching)
 
@@ -175,16 +177,17 @@
         ]
 
         self.date_iterator = DateIterator(
             start,
             end,
             self.price_provider.is_closeable(),
             order_dates,
-            weekends,
-            holidays
+            holiday_provider,
+            allow_weekends,
+            allow_holidays
         )
 
     def update_price(self, date):
         cache = {}
 
         for pod in self.pods:
             for holding in pod.account.holdings:
@@ -222,20 +225,21 @@
                 pod.fire_snapshot(date, result)
 
         return result
 
     def run(self):
         self._fire_initialize()
 
-        for date, ordered, postponned in self.date_iterator:
-            for postpone in postponned:
+        for date, ordered, skips in self.date_iterator:
+            for skip in skips:
                 for pod in self.pods:
-                    pod.exporters.fire_skip(postpone.date, postpone.reason, True)
+                    pod.exporters.fire_skip(skip.date, skip.reason, skip.ordered)
 
-                self.order(postpone.date, price_date=date)
+                if skip.ordered:
+                    self.order(skip.date, price_date=date)
 
             self.update_price(date)
 
             if ordered:
                 self.order(date)
 
         self.price_provider.save()
@@ -261,16 +265,17 @@
         quantity_in_decimal: bool,
         data_source: DataSource,
         auto_close_others: bool = True,
         exporters: typing.List[Exporter] = [],
         mapper: SymbolMapper = None,
         fee_model: FeeModel = ConstantFeeModel(0.0),
         caching=True,
-        weekends=False,
-        holidays=False,
+        allow_weekends=False,
+        allow_holidays=False,
+        holiday_provider: HolidayProvider = LegacyHolidayProvider(),
     ):
         self.order_provider = order_provider
         order_dates = order_provider.get_dates()
         start = max(next(iter(order_dates)), start) if len(order_dates) else None
 
         self.price_provider = PriceProvider(start, end, data_source, mapper, caching=caching)
 
@@ -283,16 +288,17 @@
         )
 
         self.date_iterator = DateIterator(
             start,
             end,
             self.price_provider.is_closeable(),
             order_dates,
-            weekends,
-            holidays
+            holiday_provider,
+            allow_weekends,
+            allow_holidays,
         )
 
     def update_price(self, date):
         for holding in self.account.holdings:
             price = self.price_provider.get(date, holding.symbol)
 
             if price is None:
@@ -314,20 +320,21 @@
             orders,
             price_date
         )
 
     def run(self):
         self.exporters.fire_initialize()
 
-        for date, ordered, postponned in self.date_iterator:
-            for postpone in postponned:
-                self.exporters.fire_skip(postpone.date, postpone.reason, True)
-
-                result = self.order(postpone.date, price_date=date)
-                self.exporters.fire_snapshot(date, self.account, result, postponned=postpone.date)
+        for date, ordered, skips in self.date_iterator:
+            for skip in skips:
+                self.exporters.fire_skip(skip.date, skip.reason, skip.ordered)
+
+                if skip.ordered:
+                    result = self.order(skip.date, price_date=date)
+                    self.exporters.fire_snapshot(date, self.account, result, postponned=skip.date)
 
             self.update_price(date)
             self.exporters.fire_snapshot(date, self.account, None)
 
             if ordered:
                 result = self.order(date)
```

### Comparing `bktest-2.0.0/bktest/cli.py` & `bktest-2.1.0/bktest/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,104 +19,136 @@
 from .utils import is_number, use_attrs
 from . import constants
 
 dotenv.load_dotenv()
 
 
 @click.group(invoke_without_command=True)
+#
 @click.option('--start', type=click.DateTime(formats=["%Y-%m-%d"]), default=None, help="Start date.")
 @click.option('--end', type=click.DateTime(formats=["%Y-%m-%d"]), default=None, help="End date.")
-@click.option('--offset-before-trading', type=int, default=1, show_default=True, help="Number of day to offset to push the signal before trading it.")
+#
+@click.option('--offset-before-trading', type=int, default=0, show_default=True, help="Number of day to offset to push each date of the portfolio before trading it.")
 @click.option('--offset-before-ending', type=int, default=0, show_default=True, help="Number of day to continue the backtest after every orders.")
+#
 @click.option('--order-file', type=click.Path(exists=True, dir_okay=False), required=True, show_default=True, help="Specify an order file to use.")
 @click.option('--order-file-column-date', '--single-file-provider-column-date', type=str, default=constants.DEFAULT_DATE_COLUMN, show_default=True, help="Specify the date column name.")
 @click.option('--order-file-column-symbol', '--single-file-provider-column-symbol', type=str, default=constants.DEFAULT_SYMBOL_COLUMN, show_default=True, help="Specify the symbol column name.")
 @click.option('--order-file-column-quantity', '--single-file-provider-column-quantity', type=str, default=constants.DEFAULT_QUANTITY_COLUMN, show_default=True, help="Specify the quantity column name.")
+#
 @click.option('--initial-cash', type=int, default=100_000, show_default=True, help="Specify an initial cash amount.")
 @click.option('--quantity-mode', type=click.Choice(['percent', 'share']), default="percent", show_default=True, help="Use percent for weight and share for units.")
-@click.option('--auto-close-others', is_flag=True, help="Close the position that hasn't been provided after all of the order.")
+@click.option('--auto-close-others', is_flag=True, help="[deprecated] Close the position that hasn't been provided after all of the order.")
 @click.option('--weekends', is_flag=True, help="Include weekends?")
 @click.option('--holidays', is_flag=True, help="Include holidays?")
 @click.option('--symbol-mapping', type=str, required=False, help="Custom symbol mapping file enabling vendor-id translation.")
 @click.option('--no-caching', is_flag=True, help="Disable price caching.")
 @click.option('--fee-model', "fee_model_value", type=str, help="Specify a fee model. Must be a constant or an expression.")
+#
+@click.option('holiday_provider_name', '--holiday-provider', type=click.Choice(['legacy', 'nyse']), default="nyse", help="Specify the holiday provider to use.")
+#
 @click.option('--console', is_flag=True, help="Enable the console exporter.")
 @click.option('--console-format', type=click.Choice(['text', 'json']), default="text", show_default=True, help="Console output format.")
 @click.option('--console-file', type=click.Choice(['out', 'err']), default="out", show_default=True, help="Console output destination file.")
 @click.option('--console-hide-skips', is_flag=True, show_default=True, help="Should the console hide skipped days?")
 @click.option('--console-text-no-color', is_flag=True, help="Disable colors in the console output.")
+#
 @click.option('--dump', is_flag=True, help="Enable the dump exporter.")
 @click.option('--dump-output-file', type=str, default="dump.csv", show_default=True, help="Specify the output file.")
 @click.option('--dump-auto-delete', is_flag=True, help="Should conflicting files be automatically deleted?")
-@click.option('--influx', is_flag=True, help="Enable the influx exporter.")
-@click.option('--influx-host', type=str, default="localhost", show_default=True, help="Influx's database host.")
-@click.option('--influx-port', type=int, default=8086, show_default=True, help="Influx's database port.")
-@click.option('--influx-database', type=str, default="backtest", show_default=True, help="Influx's database name.")
-@click.option('--influx-measurement', type=str, default="snapshots", show_default=True, help="Influx's database table.")
-@click.option('--influx-key', type=str, default="test", show_default=True, help="Key to use to uniquely identify the exported values.")
+#
 @click.option('--quantstats', is_flag=True, help="Enable the quantstats exporter.")
 @click.option('--quantstats-output-file-html', type=str, default="report.html", show_default=True, help="Specify the output html file.")
 @click.option('--quantstats-output-file-csv', type=str, default="report.csv", show_default=True, help="Specify the output csv file.")
 @click.option('--quantstats-benchmark-ticker', type=str, default="SPY", show_default=True, help="Specify the symbol to use as a benchmark.")
 @click.option('--quantstats-auto-delete', is_flag=True, help="Should conflicting files be automatically deleted?")
+#
 @click.option('--pdf', is_flag=True, help="Enable the quantstats exporter.")
 @click.option('--pdf-template', type=str, default="tearsheet.sketch", show_default=True, help="Specify the template file.")
 @click.option('--pdf-output-file', type=str, default="report.pdf", show_default=True, help="Specify the output pdf file.")
 @click.option('--pdf-auto-delete', is_flag=True, help="Should aa conflicting file be automatically deleted?")
 @click.option('--pdf-debug', is_flag=True, help="Enable renderer debugging.")
 @click.option('--pdf-variable', "pdf_variables", nargs=2, multiple=True, type=(str, str), help="Specify custom variables.")
 @click.option('--pdf-user-script', "pdf_user_script_paths", multiple=True, type=str, help="Specify custom scripts.")
+#
 @click.option('--specific-return', type=str, help="Enable the specific return exporter by proving a .parquet.")
 @click.option('--specific-return-column-date', type=str, default="date", show_default=True, help="Specify the column name containing the dates.")
 @click.option('--specific-return-column-symbol', type=str, default="symbol", show_default=True, help="Specify the column name containing the symbols.")
 @click.option('--specific-return-column-value', type=str, default="specific_return", show_default=True, help="Specify the column name containing the value.")
 @click.option('--specific-return-output-file-html', type=str, default="sr-report.html", show_default=True, help="Specify the output html file.")
 @click.option('--specific-return-output-file-csv', type=str, default="sr-report.csv", show_default=True, help="Specify the output csv file.")
 @click.option('--specific-return-auto-delete', is_flag=True, help="Should conflicting files be automatically deleted?")
+#
 @click.option('--yahoo', is_flag=True, help="Use yahoo finance as the data source.")
+#
 @click.option('--coinmarketcap', is_flag=True, help="Use coin market cap as the data source.")
 @click.option('--coinmarketcap-force-mapping-refresh', is_flag=True, help="Force a mapping refresh.")
 @click.option('--coinmarketcap-page-size', default=10_000, help="Specify the query page size when building the mapping.")
+#
 @click.option('--factset', is_flag=True, help="Use factset prices as the data source.")
 @click.option('--factset-username-serial', type=str, envvar="FACTSET_USERNAME_SERIAL", help="Specify the factset username serial to use.")
 @click.option('--factset-api-key', type=str, envvar="FACTSET_API_KEY", help="Specify the factset api key to use.")
+#
 @click.option('--file-parquet', type=str, required=False, help="Use a .parquet file as the data source.")
 @click.option('--file-parquet-column-date', type=str, default="date", show_default=True, help="Specify the column name containing the dates.")
 @click.option('--file-parquet-column-symbol', type=str, default="symbol", show_default=True, help="Specify the column name containing the symbols.")
 @click.option('--file-parquet-column-price', type=str, default="price", show_default=True, help="Specify the column name containing the prices.")
+#
 @click.pass_context
 def cli(ctx: click.Context, **kwargs):
     if ctx.invoked_subcommand is None:
         main(**kwargs)
 
 
 def main(
-    start: datetime.datetime, end: datetime.datetime,
+    start: datetime.datetime,
+    end: datetime.datetime,
+    #
     offset_before_trading: int,
     offset_before_ending: int,
+    #
     order_file,
     order_file_column_date: str,
     order_file_column_symbol: str,
     order_file_column_quantity: str,
-    initial_cash, quantity_mode, auto_close_others,
-    weekends, holidays, symbol_mapping, no_caching,
+    #
+    initial_cash,
+    quantity_mode,
+    auto_close_others,
+    weekends,
+    holidays,
+    symbol_mapping,
+    no_caching,
     fee_model_value,
+    #
+    holiday_provider_name: str,
+    #
     console, console_format, console_file, console_hide_skips, console_text_no_color,
+    #
     dump: str, dump_output_file: str, dump_auto_delete: bool,
-    influx, influx_host, influx_port, influx_database, influx_measurement, influx_key,
+    #
     quantstats, quantstats_output_file_html, quantstats_output_file_csv, quantstats_benchmark_ticker, quantstats_auto_delete,
+    #
     pdf: bool, pdf_template: str, pdf_output_file: str, pdf_auto_delete: bool, pdf_debug: bool, pdf_variables: typing.Tuple[typing.Tuple[str, str]], pdf_user_script_paths: str,
+    #
     specific_return: str, specific_return_column_date: str, specific_return_column_symbol: str, specific_return_column_value: str, specific_return_output_file_html: str, specific_return_output_file_csv: str, specific_return_auto_delete: bool,
+    #
     yahoo,
+    #
     coinmarketcap, coinmarketcap_force_mapping_refresh, coinmarketcap_page_size,
+    #
     factset: bool, factset_username_serial: str, factset_api_key: str,
+    #
     file_parquet, file_parquet_column_date, file_parquet_column_symbol, file_parquet_column_price,
 ):
     logging.getLogger('matplotlib.font_manager').setLevel(logging.ERROR)
 
+    if auto_close_others:
+        print("[warning] `--auto-close-others` is deprecated and is forced to `true`", file=sys.stderr)
+
     now = datetime.date.today()
 
     quantity_in_decimal = quantity_mode == "percent"
 
     from .order import DataFrameOrderProvider
     order_provider = DataFrameOrderProvider(
         readwrite.read(order_file),
@@ -134,14 +166,20 @@
     end = end.date() if end is not None else dates[-1]
 
     end += datetime.timedelta(days=offset_before_ending)
     if end > now:
         end = now
 
         print(f"[warning] end is after today, using: {now}", file=sys.stderr)
+    
+    from .data.holidays import LegacyHolidayProvider, SimpleHolidayProvider
+    holiday_provider = ({
+        "legacy": lambda: LegacyHolidayProvider(),
+        "nyse": lambda: SimpleHolidayProvider.nyse()
+    }[holiday_provider_name])()
 
     data_source = None
     if yahoo:
         from .data.source import YahooDataSource
         data_source = YahooDataSource()
 
     if coinmarketcap:
@@ -228,24 +266,14 @@
     if dump:
         from .export import DumpExporter
         exporters.append(DumpExporter(
             output_file=dump_output_file,
             auto_delete=dump_auto_delete,
         ))
 
-    if influx:
-        from .export import InfluxExporter
-        exporters.append(InfluxExporter(
-            host=influx_host,
-            port=influx_port,
-            database=influx_database,
-            measurement=influx_measurement,
-            key=influx_key
-        ))
-
     if quantstats:
         from .export import QuantStatsExporter
         exporters.append(QuantStatsExporter(
             html_output_file=quantstats_output_file_html,
             csv_output_file=quantstats_output_file_csv,
             benchmark_ticker=quantstats_benchmark_ticker,
             auto_delete=quantstats_auto_delete,
@@ -296,22 +324,23 @@
     from .backtest import SimpleBacktester
     SimpleBacktester(
         start=start,
         end=end,
         order_provider=order_provider,
         initial_cash=initial_cash,
         quantity_in_decimal=quantity_in_decimal,
-        auto_close_others=auto_close_others,
+        auto_close_others=True,
         data_source=data_source,
         mapper=symbol_mapper,
         exporters=exporters,
         fee_model=fee_model,
         caching=not no_caching,
-        weekends=weekends,
-        holidays=holidays
+        allow_weekends=weekends,
+        allow_holidays=holidays,
+        holiday_provider=holiday_provider
     ).run()
 
 
 @cli.group(name="template")
 def template_group():
     pass
```

### Comparing `bktest-2.0.0/bktest/data/source/base.py` & `bktest-2.1.0/bktest/data/source/base.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/data/source/coinmarketcap.py` & `bktest-2.1.0/bktest/data/source/coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/data/source/dataframe.py` & `bktest-2.1.0/bktest/data/source/dataframe.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/data/source/delegate.py` & `bktest-2.1.0/bktest/data/source/delegate.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/data/source/factset.py` & `bktest-2.1.0/bktest/data/source/factset.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/export/base.py` & `bktest-2.1.0/bktest/export/base.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/export/console.py` & `bktest-2.1.0/bktest/export/console.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/export/dump.py` & `bktest-2.1.0/bktest/export/dump.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/export/model.py` & `bktest-2.1.0/bktest/export/model.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/export/pdf.py` & `bktest-2.1.0/bktest/export/pdf.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/export/quants.py` & `bktest-2.1.0/bktest/export/quants.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/export/specific_return.py` & `bktest-2.1.0/bktest/export/specific_return.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/fee.py` & `bktest-2.1.0/bktest/fee.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/holding.py` & `bktest-2.1.0/bktest/holding.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/iterator.py` & `bktest-2.1.0/bktest/iterator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,42 @@
+import dataclasses
 import datetime
 import typing
-import dataclasses
+
+from .data.holidays import HolidayProvider, LegacyHolidayProvider
 
 
 @dataclasses.dataclass()
-class Postpone:
-    
+class Skip:
+
     date: datetime.date
     reason: str
+    ordered: bool
 
 
 class DateIterator:
 
     def __init__(
         self,
         start: datetime.date,
         end: datetime.date,
         closable: bool,
         order_dates: typing.List[datetime.date],
+        holiday_provider: HolidayProvider = LegacyHolidayProvider(),
         allow_weekends=False,
-        allow_holidays=False
+        allow_holidays=False,
     ):
         self.start = start
         self.end = end
         self.closable = closable
         self.order_dates = order_dates
+        self.holiday_provider = holiday_provider
         self.allow_weekends = allow_weekends
         self.allow_holidays = allow_holidays
-        self.postponned = []
+        self.skips = []
 
         self._date = None
 
     def __iter__(self):
         if self.start is None:
             return iter([])
 
@@ -41,58 +46,56 @@
         self._date = self.start
         return self
 
     def _should_skip_weekends(
         self,
         date: datetime.date,
         ordered: bool,
-        postponned: typing.List[Postpone]
+        skips: typing.List[Skip]
     ) -> bool:
         if self.allow_weekends or date.weekday() <= 4:
             return False
 
-        if ordered:
-            postponned.append(Postpone(
-                date,
-                "weekend"
-            ))
+        skips.append(Skip(
+            date,
+            "weekend",
+            ordered
+        ))
 
         return True
 
     def _should_skip_holidays(
         self,
         date: datetime.date,
         ordered: bool,
-        postponned: typing.List[Postpone]
+        skips: typing.List[Skip]
     ) -> bool:
-        from .data.holidays import holidays as days
-        
-        if self.allow_holidays or date not in days:
+        if self.allow_holidays or not self.holiday_provider.is_holiday(date):
             return False
 
-        if ordered:
-            postponned.append(Postpone(
-                date,
-                "holiday"
-            ))
+        skips.append(Skip(
+            date,
+            "holiday",
+            ordered
+        ))
 
         return True
 
     def __next__(self):
-        postponned: typing.List[Postpone] = []
+        skips: typing.List[Skip] = []
 
         while self._date <= self.end:
-            date = self._date
+            date = datetime.date.fromisoformat(str(self._date))
             self._date += datetime.timedelta(days=1)
 
             ordered = date in self.order_dates
 
             if self.closable:
-                if self._should_skip_weekends(date, ordered, postponned):
+                if self._should_skip_weekends(date, ordered, skips):
                     continue
 
-                if self._should_skip_holidays(date, ordered, postponned):
+                if self._should_skip_holidays(date, ordered, skips):
                     continue
 
-            return date, ordered, postponned
+            return date, ordered, skips
 
         raise StopIteration
```

### Comparing `bktest-2.0.0/bktest/order.py` & `bktest-2.1.0/bktest/order.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/price_provider.py` & `bktest-2.1.0/bktest/price_provider.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/template/models.py` & `bktest-2.1.0/bktest/template/models.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/template/pdf.py` & `bktest-2.1.0/bktest/template/pdf.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/template/sketch.py` & `bktest-2.1.0/bktest/template/sketch.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/template/template.py` & `bktest-2.1.0/bktest/template/template.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest/utils.py` & `bktest-2.1.0/bktest/utils.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/bktest.egg-info/PKG-INFO` & `bktest-2.1.0/bktest.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: bktest
-Version: 2.0.0
+Version: 2.1.0
 Summary: bktest - A simple backtester by CrunchDAO
 Home-page: https://github.com/crunchdao/backtest
 Author: Enzo CACERES
 Author-email: enzo.caceres@crunchdao.com
 Keywords: package development template
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: click<8.1.2,>=8.0
 Requires-Dist: pandas<2.0.0,>=1.5
 Requires-Dist: python-dateutil<2.8.3,>=2.8.2
 Requires-Dist: tqdm<4.65.0,>=4.48.0
-Requires-Dist: influxdb<5.3.1,>=5.2.2
 Requires-Dist: numpy<1.25.0,>=1.23.0
 Requires-Dist: py_expression_eval<0.3.14,>=0.3.9
 Requires-Dist: pyarrow<12.0,>=11.0
 Requires-Dist: quantstats==0.0.62
 Requires-Dist: pytest<7.3.0,>=7.1.0
 Requires-Dist: yfinance<0.2.27,>=0.2.24
 Requires-Dist: python-dotenv<1.0.0,>=0.20
@@ -28,28 +27,28 @@
 Requires-Dist: python-slugify
 Requires-Dist: cached-property
 Requires-Dist: fpdf2==2.7.4
 Requires-Dist: contexttimer
 Requires-Dist: watchdog
 Requires-Dist: fastparquet
 Requires-Dist: readwrite
+Requires-Dist: holidays
 
 A small backtesting utility.
 
 ![image](https://user-images.githubusercontent.com/7386242/189368488-b0c30d48-9a1f-4362-9f78-10a451535682.png)
 
 [![PyTest](https://github.com/crunchdao/backtest/actions/workflows/pytest.yml/badge.svg)](https://github.com/crunchdao/backtest/actions/workflows/pytest.yml)
 
 - [Install](#install)
 - [Usage](#usage)
   - [Options](#options)
     - [Exporters](#exporters)
       - [Console](#console)
       - [Dump](#dump)
-      - [Influx](#influx)
       - [QuantStats](#quantstats)
       - [PDF](#pdf)
       - [Specific Return](#specific-return)
     - [Data Sources](#data-sources)
       - [Yahoo](#yahoo)
       - [CoinMarketCap](#coinmarketcap)
       - [FactSet](#factset)
@@ -70,31 +69,31 @@
 
 ## Options
 
 | Option | Value | Default | Format | Description |
 | --- | --- | --- | --- | --- |
 | `--start` | `<start date>` | `orders' first date` | `date` (ISO-8601) | The starting date of the backtesting. If the value is before the first ordering day, the value will be discarded. |
 | `--end` | `<end date>` | `orders' last date` | `date` (ISO-8601) | The ending date of the backtesting. If the value is after today, the value will be discarded. |
-| `--offset-before-trading` | `<days>` | `1` | `int` | Number of day to offset to push the signal before trading it. |
+| `--offset-before-trading` | `<days>` | `1` | `int` | Number of day to offset to push each date of the portfolio before trading it. |
 | `--offset-before-ending` | `<days>` | `0` | `int` | Number of day to continue the backtest after every orders. |
 | `--order-file` | `<file>` | | `path` | The single order file to use. The file must contain symbol, quantity and date information. |
 | `--single-file-provider-column-date` | `<column>` | `date` | `string` | Change the date column name to use. |
 | `--single-file-provider-column-symbol` | `<column>` | `symbol` | `string` | Change the symbol column name to use. |
 | `--single-file-provider-column-quantity` | `<column>` | `quantity` | `string` | Change the quantity column name to use. |
 | `--order-files` | `<directory>` | | `path` | The directory of order file to use. The filename must be a date. The file must contain symbol and quantity information. |
 | `--order-files-extension` | `<extension>` | `csv`  | `[csv, parquet, json]` | Change the file extension to use when listing for order files. |
 | `--initial-cash` | `<amount>` | `100_000` | `number` | Change the initial cash to use for the backtesting. |
 | `--quantity-mode` | `<mode>` | `percent` | `[percent, share]` | If the mode is `share`, all quantities will be interpreted as integers. If the mode is `percent`, all values will be multiplied by the current cash value. |
-| `--auto-close-others` | | `false` | | Should other position be closed after an ordering? |
 | `--weekends` | | `false` | | Enable ordering on weekends. |
 | `--holidays` | | `false` | | Enable ordering on holidays. |
 | `--symbol-mapping` | `<mapping>` | | `path` (.json) | Specify a custom symbol mapping file enabling vendor-id translation. |
 | `--no-caching` | | `false` | | Disable prices caching. |
 | `--fee-model` | `<model>` | | `expression` or `constant` | Specify a fee model to use. The value can be a `constant`. Or an expression that allow the usage of the `price` and `quantity` variable. <br /> Example: `abs(price * quantity) * 0.1` |
-| `--rfr-file` | `<directory>` | | `path` | The directory of rfr file to use. The file must contain a column with date information and a column with the rfr information in %. |
+| `--holiday-provider` | `<name>` | `nyse` | `[legacy, nyse]` | Specify which holiday provider to use. |
+| `--rfr-file` | `<directory>` |  | `path` | The directory of rfr file to use. The file must contain a column with date information and a column with the rfr information in %. |
 | `--rfr-file-column-date` | `<column>` | `date` | `string` | Change the date column name to use. |
 
 ### Exporters
 
 Multiple exporters can be enabled at one time.
 
 #### Console
@@ -115,28 +114,14 @@
 
 | Option | Value | Default | Format | Description |
 | --- | --- | --- | --- | --- |
 | `--dump` | | `false` | | Enable the dump exporter. |
 | `--dump-output-file` | `<file>` | `dump.csv` | `path` | Specify the output file. |
 | `--dump-auto-delete` | | `false` | | Automatically delete the previous dump file if it is present. |
 
-#### Influx
-
-Export the generated data to an Influx database. <br />
-Making it easier to plot the values using software like Grafana.
-
-| Option | Value | Default | Format | Description |
-| --- | --- | --- | --- | --- |
-| `--influx` | | `false` | | Enable the influx exporter. |
-| `--influx-host` | `<host>` | `localhost` | `string` | Specify the remote influx address. |
-| `--influx-port` | `<port>` | `8086` | `number` | Specify the remote influx port. |
-| `--influx-database` | `<database>` | `backtest` | `string` | Specify the influx database to use. |
-| `--influx-measurement` | `<measurement>` | `snapshots` |`string` | Specify the table name to use. |
-| `--influx-key` | `<key>` | `test` | `string` | Specify the unique key to use. **Previous data with the same key will be deleted!** |
-
 #### QuantStats
 
 Generate a tearsheet from the backtest data.
 
 | Option | Value | Default | Format | Description |
 | --- | --- | --- | --- | --- |
 | `--quantstats` | | `false` | | Enable the quantstats exporter. |
```

### Comparing `bktest-2.0.0/bktest.egg-info/SOURCES.txt` & `bktest-2.1.0/bktest.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 bktest/data/source/delegate.py
 bktest/data/source/factset.py
 bktest/data/source/yahoo.py
 bktest/export/__init__.py
 bktest/export/base.py
 bktest/export/console.py
 bktest/export/dump.py
-bktest/export/influx.py
 bktest/export/model.py
 bktest/export/pdf.py
 bktest/export/quants.py
 bktest/export/specific_return.py
 bktest/template/__init__.py
 bktest/template/models.py
 bktest/template/pdf.py
```

### Comparing `bktest-2.0.0/setup.py` & `bktest-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/tests/test_account.py` & `bktest-2.1.0/tests/test_account.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/tests/test_data_source.py` & `bktest-2.1.0/tests/test_data_source.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/tests/test_fee.py` & `bktest-2.1.0/tests/test_fee.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/tests/test_holdings.py` & `bktest-2.1.0/tests/test_holdings.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/tests/test_iterator.py` & `bktest-2.1.0/tests/test_iterator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import unittest
 
-from bktest.iterator import DateIterator, Postpone
+from bktest.iterator import DateIterator, Skip
 
 
 class DateIteratorTest(unittest.TestCase):
 
     def test_iter_empty(self):
         iterator = DateIterator(None, None, False, [])
         with self.assertRaises(StopIteration):
@@ -30,15 +30,15 @@
 
     def test_should_skip_weekends(self):
         iterator = DateIterator(None, None, False, [], allow_weekends=False)
         postponned = []
         date = datetime.date(2024, 1, 20)
 
         self.assertTrue(iterator._should_skip_weekends(date, True, postponned))
-        self.assertEqual(postponned, [Postpone(date, "weekend")])
+        self.assertEqual(postponned, [Skip(date, "weekend", True)])
 
     def test_should_skip_holidays_allow(self):
         iterator = DateIterator(None, None, False, [], allow_holidays=True)
         self.assertFalse(iterator._should_skip_holidays(datetime.date(2023, 12, 25), False, []))
 
     def test_should_skip_holidays_week(self):
         iterator = DateIterator(None, None, False, [], allow_holidays=False)
@@ -46,30 +46,30 @@
 
     def test_should_skip_holidays(self):
         iterator = DateIterator(None, None, False, [], allow_holidays=False)
         postponned = []
         date = datetime.date(2023, 12, 25)
 
         self.assertTrue(iterator._should_skip_holidays(date, True, postponned))
-        self.assertEqual(postponned, [Postpone(date, "holiday")])
+        self.assertEqual(postponned, [Skip(date, "holiday", True)])
 
     def test_next(self):
         iterator = iter(DateIterator(
             datetime.date(2024, 1, 1),
             datetime.date(2024, 1, 10),
             True,
             [
                 datetime.date(2024, 1, 1),
                 datetime.date(2024, 1, 4),
                 datetime.date(2024, 1, 7),
                 datetime.date(2024, 1, 9),
             ]
         ))
 
-        self.assertEqual(next(iterator), (datetime.date(2024, 1, 2), False, [Postpone(datetime.date(2024, 1, 1), "holiday")]))
+        self.assertEqual(next(iterator), (datetime.date(2024, 1, 2), False, [Skip(datetime.date(2024, 1, 1), "holiday", True)]))
         self.assertEqual(next(iterator), (datetime.date(2024, 1, 3), False, []))
         self.assertEqual(next(iterator), (datetime.date(2024, 1, 4), True, []))
         self.assertEqual(next(iterator), (datetime.date(2024, 1, 5), False, []))
-        self.assertEqual(next(iterator), (datetime.date(2024, 1, 8), False, [Postpone(datetime.date(2024, 1, 7), "weekend")]))
+        self.assertEqual(next(iterator), (datetime.date(2024, 1, 8), False, [Skip(datetime.date(2024, 1, 6), "weekend", False), Skip(datetime.date(2024, 1, 7), "weekend", True)]))
         self.assertEqual(next(iterator), (datetime.date(2024, 1, 9), True, []))
         self.assertEqual(next(iterator), (datetime.date(2024, 1, 10), False, []))
         self.assertRaises(StopIteration, lambda: next(iterator))
```

### Comparing `bktest-2.0.0/tests/test_order.py` & `bktest-2.1.0/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `bktest-2.0.0/tests/test_utils.py` & `bktest-2.1.0/tests/test_utils.py`

 * *Files identical despite different names*

