# Comparing `tmp/jy_lib-0.7.3.tar.gz` & `tmp/jy_lib-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jy_lib-0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "jy_lib-0.7.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `jy_lib-0.7.3.tar` & `jy_lib-0.7.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2083 2024-05-04 10:16:37.911987 jy_lib-0.7.3/.gitignore
--rw-r--r--   0        0        0      285 2024-05-04 10:16:37.912391 jy_lib-0.7.3/.pypirc
--rw-r--r--   0        0        0     1073 2024-05-04 10:16:37.912678 jy_lib-0.7.3/LICENSE
--rw-r--r--   0        0        0      573 2024-05-04 10:16:37.912981 jy_lib-0.7.3/Pipfile
--rw-r--r--   0        0        0    40838 2024-05-04 10:16:37.913598 jy_lib-0.7.3/Pipfile.lock
--rw-r--r--   0        0        0       10 2024-05-04 10:16:37.914070 jy_lib-0.7.3/README.md
--rw-r--r--   0        0        0      469 2024-05-04 10:16:37.914438 jy_lib-0.7.3/README_Project.md
--rw-r--r--   0        0        0      518 2024-05-04 10:20:58.713262 jy_lib-0.7.3/jy_lib/__init__.py
--rw-r--r--   0        0        0     7230 2024-05-04 10:16:37.915485 jy_lib-0.7.3/jy_lib/auth_client.py
--rw-r--r--   0        0        0    10531 2024-05-04 10:16:37.915923 jy_lib-0.7.3/jy_lib/bank.py
--rw-r--r--   0        0        0      809 2024-05-04 10:16:37.916235 jy_lib-0.7.3/jy_lib/base.py
--rw-r--r--   0        0        0    14155 2024-05-04 10:16:37.916568 jy_lib-0.7.3/jy_lib/cache.py
--rw-r--r--   0        0        0    11966 2024-05-04 10:16:37.916925 jy_lib-0.7.3/jy_lib/clickhouse.py
--rw-r--r--   0        0        0     4411 2024-05-04 10:16:37.917240 jy_lib-0.7.3/jy_lib/compressor.py
--rw-r--r--   0        0        0    21765 2024-05-04 10:16:37.917634 jy_lib-0.7.3/jy_lib/country.py
--rw-r--r--   0        0        0    10928 2024-05-04 10:16:37.918037 jy_lib-0.7.3/jy_lib/currency.py
--rw-r--r--   0        0        0     2399 2024-05-04 10:16:37.918334 jy_lib-0.7.3/jy_lib/date.py
--rw-r--r--   0        0        0      931 2024-05-04 10:16:37.918666 jy_lib-0.7.3/jy_lib/decorator.py
--rw-r--r--   0        0        0     5916 2024-05-04 10:16:37.918991 jy_lib-0.7.3/jy_lib/exchange.py
--rw-r--r--   0        0        0      602 2024-05-04 10:16:37.919292 jy_lib-0.7.3/jy_lib/interrupt_protect.py
--rw-r--r--   0        0        0     2151 2024-05-04 10:16:37.919587 jy_lib-0.7.3/jy_lib/lock.py
--rw-r--r--   0        0        0      707 2024-05-04 10:16:37.919884 jy_lib-0.7.3/jy_lib/math.py
--rw-r--r--   0        0        0     5926 2024-05-04 10:16:37.920296 jy_lib-0.7.3/jy_lib/nav.py
--rw-r--r--   0        0        0     2194 2024-05-04 10:16:37.920783 jy_lib-0.7.3/jy_lib/reader.py
--rw-r--r--   0        0        0    18478 2024-05-04 10:16:37.921224 jy_lib-0.7.3/jy_lib/smb_client.py
--rw-r--r--   0        0        0    22173 2024-05-04 10:16:37.921846 jy_lib-0.7.3/jy_lib/symbol.py
--rw-r--r--   0        0        0    20726 2024-05-04 10:16:37.922441 jy_lib-0.7.3/jy_lib/symbol_em.py
--rw-r--r--   0        0        0      577 2024-05-04 10:16:37.922948 jy_lib-0.7.3/jy_lib/time.py
--rw-r--r--   0        0        0       67 2024-05-04 10:16:37.923293 jy_lib-0.7.3/publish-jypi.sh
--rw-r--r--   0        0        0       67 2024-05-04 10:16:37.923609 jy_lib-0.7.3/publish-pypi.sh
--rw-r--r--   0        0        0       67 2024-05-04 10:16:37.923903 jy_lib-0.7.3/publish-test.sh
--rw-r--r--   0        0        0      639 2024-05-04 10:16:37.924216 jy_lib-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      117 2024-05-04 10:16:37.924494 jy_lib-0.7.3/requirements.txt
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     2083 2023-10-19 03:06:08.475402 jy_lib-0.7.4/.gitignore
+-rw-r--r--   0        0        0      285 2023-10-23 02:58:33.543130 jy_lib-0.7.4/.pypirc
+-rw-r--r--   0        0        0     1073 2023-10-19 06:46:25.394076 jy_lib-0.7.4/LICENSE
+-rw-r--r--   0        0        0      573 2024-04-11 01:31:08.426951 jy_lib-0.7.4/Pipfile
+-rw-r--r--   0        0        0    40838 2023-02-28 09:06:11.940000 jy_lib-0.7.4/Pipfile.lock
+-rw-r--r--   0        0        0       10 2023-10-19 06:54:49.519221 jy_lib-0.7.4/README.md
+-rw-r--r--   0        0        0      469 2023-10-19 08:27:51.652921 jy_lib-0.7.4/README_Project.md
+-rw-r--r--   0        0        0      518 2024-05-09 07:54:59.347608 jy_lib-0.7.4/jy_lib/__init__.py
+-rw-r--r--   0        0        0     7230 2023-10-25 01:56:08.575822 jy_lib-0.7.4/jy_lib/auth_client.py
+-rw-r--r--   0        0        0    10531 2023-10-25 08:34:10.093160 jy_lib-0.7.4/jy_lib/bank.py
+-rw-r--r--   0        0        0      809 2023-10-23 02:40:21.784597 jy_lib-0.7.4/jy_lib/base.py
+-rw-r--r--   0        0        0    14155 2024-05-06 01:36:59.153706 jy_lib-0.7.4/jy_lib/cache.py
+-rw-r--r--   0        0        0    11966 2024-05-06 01:34:15.372137 jy_lib-0.7.4/jy_lib/clickhouse.py
+-rw-r--r--   0        0        0     4411 2024-04-11 01:28:25.533046 jy_lib-0.7.4/jy_lib/compressor.py
+-rw-r--r--   0        0        0    21765 2023-10-25 08:34:10.093378 jy_lib-0.7.4/jy_lib/country.py
+-rw-r--r--   0        0        0    10928 2023-10-25 08:34:10.093573 jy_lib-0.7.4/jy_lib/currency.py
+-rw-r--r--   0        0        0     2399 2024-01-16 00:58:10.482893 jy_lib-0.7.4/jy_lib/date.py
+-rw-r--r--   0        0        0      931 2023-10-27 09:01:08.015737 jy_lib-0.7.4/jy_lib/decorator.py
+-rw-r--r--   0        0        0     5916 2024-04-24 02:27:16.042289 jy_lib-0.7.4/jy_lib/exchange.py
+-rw-r--r--   0        0        0      602 2024-03-26 02:17:46.967953 jy_lib-0.7.4/jy_lib/interrupt_protect.py
+-rw-r--r--   0        0        0     2151 2023-10-25 05:47:55.730076 jy_lib-0.7.4/jy_lib/lock.py
+-rw-r--r--   0        0        0      707 2024-01-17 07:58:34.306588 jy_lib-0.7.4/jy_lib/math.py
+-rw-r--r--   0        0        0     5926 2023-12-21 06:12:51.186402 jy_lib-0.7.4/jy_lib/nav.py
+-rw-r--r--   0        0        0     2194 2024-05-06 01:34:15.372232 jy_lib-0.7.4/jy_lib/reader.py
+-rw-r--r--   0        0        0    18478 2024-04-17 00:51:09.235795 jy_lib-0.7.4/jy_lib/smb_client.py
+-rw-r--r--   0        0        0    22189 2024-05-09 07:54:46.613755 jy_lib-0.7.4/jy_lib/symbol.py
+-rw-r--r--   0        0        0    20726 2024-03-23 07:36:23.764234 jy_lib-0.7.4/jy_lib/symbol_em.py
+-rw-r--r--   0        0        0      577 2023-11-03 01:23:44.753118 jy_lib-0.7.4/jy_lib/time.py
+-rw-r--r--   0        0        0       67 2023-10-19 06:54:09.145568 jy_lib-0.7.4/publish-jypi.sh
+-rw-r--r--   0        0        0       67 2023-10-19 06:53:07.001372 jy_lib-0.7.4/publish-pypi.sh
+-rw-r--r--   0        0        0       67 2023-10-19 06:54:14.808768 jy_lib-0.7.4/publish-test.sh
+-rw-r--r--   0        0        0      639 2024-04-11 07:52:56.404049 jy_lib-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      117 2024-04-15 07:06:48.431549 jy_lib-0.7.4/requirements.txt
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 jy_lib-0.7.4/PKG-INFO
```

### Comparing `jy_lib-0.7.3/.gitignore` & `jy_lib-0.7.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/LICENSE` & `jy_lib-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/Pipfile` & `jy_lib-0.7.4/Pipfile`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/Pipfile.lock` & `jy_lib-0.7.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/__init__.py` & `jy_lib-0.7.4/jy_lib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     SymbolFlag,
     SymbolSubType,
     SymbolType,
     WarrantsType,
 )
 from .symbol_em import EMParser, KLineRecord, TrendRecord
 
-__version__ = "0.7.3"
+__version__ = "0.7.4"
```

### Comparing `jy_lib-0.7.3/jy_lib/auth_client.py` & `jy_lib-0.7.4/jy_lib/auth_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/bank.py` & `jy_lib-0.7.4/jy_lib/bank.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/base.py` & `jy_lib-0.7.4/jy_lib/base.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/cache.py` & `jy_lib-0.7.4/jy_lib/cache.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/clickhouse.py` & `jy_lib-0.7.4/jy_lib/clickhouse.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/compressor.py` & `jy_lib-0.7.4/jy_lib/compressor.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/country.py` & `jy_lib-0.7.4/jy_lib/country.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/currency.py` & `jy_lib-0.7.4/jy_lib/currency.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/date.py` & `jy_lib-0.7.4/jy_lib/date.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/decorator.py` & `jy_lib-0.7.4/jy_lib/decorator.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/exchange.py` & `jy_lib-0.7.4/jy_lib/exchange.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/interrupt_protect.py` & `jy_lib-0.7.4/jy_lib/interrupt_protect.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/lock.py` & `jy_lib-0.7.4/jy_lib/lock.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/math.py` & `jy_lib-0.7.4/jy_lib/math.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/nav.py` & `jy_lib-0.7.4/jy_lib/nav.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/reader.py` & `jy_lib-0.7.4/jy_lib/reader.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/smb_client.py` & `jy_lib-0.7.4/jy_lib/smb_client.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/symbol.py` & `jy_lib-0.7.4/jy_lib/symbol.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
                 instrument_type = SymbolType.OPTIONS
             elif l_iid == 6 and iid.startswith('000'):
                 instrument_type = SymbolType.INDEX
             elif l_iid == 6 and iid.startswith('5'):
                 instrument_type = SymbolType.FUND
             elif l_iid == 6 and iid.startswith(('6', '9')):
                 instrument_type = SymbolType.STOCK
-            elif l_iid == 6 and iid.startswith(('100', '11', '204')):
+            elif l_iid == 6 and iid.startswith(('100', '11', '204', '1260')):
                 instrument_type = SymbolType.BOND
             else:
                 return
             return SymbolDetail(
                 original_symbol_id=original_symbol_id,
                 exchange=exchange,
                 instrument_id=iid,
@@ -217,15 +217,15 @@
                 instrument_type = SymbolType.OPTIONS
             elif l_iid == 6 and iid.startswith('399'):
                 instrument_type = SymbolType.INDEX
             elif l_iid == 6 and iid.startswith(('15', '16', '18')):
                 instrument_type = SymbolType.FUND
             elif l_iid == 6 and iid.startswith(('2', '0', '3')):
                 instrument_type = SymbolType.STOCK
-            elif l_iid == 6 and iid.startswith(('12', '131')):
+            elif l_iid == 6 and iid.startswith(('12', '131', '1150')):
                 instrument_type = SymbolType.BOND
             else:
                 return
             return SymbolDetail(
                 original_symbol_id=original_symbol_id,
                 exchange=exchange,
                 instrument_id=iid,
```

### Comparing `jy_lib-0.7.3/jy_lib/symbol_em.py` & `jy_lib-0.7.4/jy_lib/symbol_em.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/jy_lib/time.py` & `jy_lib-0.7.4/jy_lib/time.py`

 * *Files identical despite different names*

### Comparing `jy_lib-0.7.3/pyproject.toml` & `jy_lib-0.7.4/pyproject.toml`

 * *Files identical despite different names*

