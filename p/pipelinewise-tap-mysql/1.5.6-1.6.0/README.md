# Comparing `tmp/pipelinewise-tap-mysql-1.5.6.tar.gz` & `tmp/pipelinewise_tap_mysql-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipelinewise-tap-mysql-1.5.6.tar", last modified: Thu Aug 10 16:03:03 2023, max compression
+gzip compressed data, was "pipelinewise_tap_mysql-1.6.0.tar", last modified: Thu May  9 14:27:50 2024, max compression
```

## Comparing `pipelinewise-tap-mysql-1.5.6.tar` & `pipelinewise_tap_mysql-1.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 16:03:03.815958 pipelinewise-tap-mysql-1.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-08-10 16:02:54.000000 pipelinewise-tap-mysql-1.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-08-10 16:03:03.815958 pipelinewise-tap-mysql-1.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22761 2023-08-10 16:02:54.000000 pipelinewise-tap-mysql-1.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 16:03:03.815958 pipelinewise-tap-mysql-1.5.6/pipelinewise_tap_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-08-10 16:03:03.000000 pipelinewise-tap-mysql-1.5.6/pipelinewise_tap_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-10 16:03:03.000000 pipelinewise-tap-mysql-1.5.6/pipelinewise_tap_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-10 16:03:03.000000 pipelinewise-tap-mysql-1.5.6/pipelinewise_tap_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-10 16:03:03.000000 pipelinewise-tap-mysql-1.5.6/pipelinewise_tap_mysql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-10 16:03:03.000000 pipelinewise-tap-mysql-1.5.6/pipelinewise_tap_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-10 16:03:03.000000 pipelinewise-tap-mysql-1.5.6/pipelinewise_tap_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-10 16:03:03.815958 pipelinewise-tap-mysql-1.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-10 16:02:54.000000 pipelinewise-tap-mysql-1.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 16:03:03.815958 pipelinewise-tap-mysql-1.5.6/tap_mysql/
--rw-r--r--   0 runner    (1001) docker     (123)    17929 2023-08-10 16:02:54.000000 pipelinewise-tap-mysql-1.5.6/tap_mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-08-10 16:02:54.000000 pipelinewise-tap-mysql-1.5.6/tap_mysql/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-08-10 16:02:54.000000 pipelinewise-tap-mysql-1.5.6/tap_mysql/discover_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-10 16:02:54.000000 pipelinewise-tap-mysql-1.5.6/tap_mysql/stream_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-10 16:03:03.815958 pipelinewise-tap-mysql-1.5.6/tap_mysql/sync_strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-10 16:02:54.000000 pipelinewise-tap-mysql-1.5.6/tap_mysql/sync_strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35179 2023-08-10 16:02:54.000000 pipelinewise-tap-mysql-1.5.6/tap_mysql/sync_strategies/binlog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-08-10 16:02:54.000000 pipelinewise-tap-mysql-1.5.6/tap_mysql/sync_strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-08-10 16:02:54.000000 pipelinewise-tap-mysql-1.5.6/tap_mysql/sync_strategies/full_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-08-10 16:02:54.000000 pipelinewise-tap-mysql-1.5.6/tap_mysql/sync_strategies/incremental.py
+drwxr-xr-x   0 louis.pieterse   (503) staff       (20)        0 2024-05-09 14:27:50.455164 pipelinewise_tap_mysql-1.6.0/
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)    32393 2024-05-09 13:12:03.000000 pipelinewise_tap_mysql-1.6.0/LICENSE
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)    23554 2024-05-09 14:27:50.454352 pipelinewise_tap_mysql-1.6.0/PKG-INFO
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)    22761 2024-05-09 13:12:03.000000 pipelinewise_tap_mysql-1.6.0/README.md
+drwxr-xr-x   0 louis.pieterse   (503) staff       (20)        0 2024-05-09 14:27:50.453115 pipelinewise_tap_mysql-1.6.0/pipelinewise_tap_mysql.egg-info/
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)    23554 2024-05-09 14:27:50.000000 pipelinewise_tap_mysql-1.6.0/pipelinewise_tap_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)      595 2024-05-09 14:27:50.000000 pipelinewise_tap_mysql-1.6.0/pipelinewise_tap_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)        1 2024-05-09 14:27:50.000000 pipelinewise_tap_mysql-1.6.0/pipelinewise_tap_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)       45 2024-05-09 14:27:50.000000 pipelinewise_tap_mysql-1.6.0/pipelinewise_tap_mysql.egg-info/entry_points.txt
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)      164 2024-05-09 14:27:50.000000 pipelinewise_tap_mysql-1.6.0/pipelinewise_tap_mysql.egg-info/requires.txt
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)       10 2024-05-09 14:27:50.000000 pipelinewise_tap_mysql-1.6.0/pipelinewise_tap_mysql.egg-info/top_level.txt
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)       38 2024-05-09 14:27:50.455271 pipelinewise_tap_mysql-1.6.0/setup.cfg
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)     1207 2024-05-09 13:36:58.000000 pipelinewise_tap_mysql-1.6.0/setup.py
+drwxr-xr-x   0 louis.pieterse   (503) staff       (20)        0 2024-05-09 14:27:50.448824 pipelinewise_tap_mysql-1.6.0/tap_mysql/
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)    17929 2024-05-09 13:12:03.000000 pipelinewise_tap_mysql-1.6.0/tap_mysql/__init__.py
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)     6570 2024-05-09 13:12:03.000000 pipelinewise_tap_mysql-1.6.0/tap_mysql/connection.py
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)    13865 2024-05-09 13:12:03.000000 pipelinewise_tap_mysql-1.6.0/tap_mysql/discover_utils.py
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)     1045 2024-05-09 13:12:03.000000 pipelinewise_tap_mysql-1.6.0/tap_mysql/stream_utils.py
+drwxr-xr-x   0 louis.pieterse   (503) staff       (20)        0 2024-05-09 14:27:50.452229 pipelinewise_tap_mysql-1.6.0/tap_mysql/sync_strategies/
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)        0 2024-05-09 13:12:03.000000 pipelinewise_tap_mysql-1.6.0/tap_mysql/sync_strategies/__init__.py
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)    35184 2024-05-09 13:12:03.000000 pipelinewise_tap_mysql-1.6.0/tap_mysql/sync_strategies/binlog.py
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)     7647 2024-05-09 13:12:03.000000 pipelinewise_tap_mysql-1.6.0/tap_mysql/sync_strategies/common.py
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)     6609 2024-05-09 13:12:03.000000 pipelinewise_tap_mysql-1.6.0/tap_mysql/sync_strategies/full_table.py
+-rw-r--r--   0 louis.pieterse   (503) staff       (20)     3051 2024-05-09 13:12:03.000000 pipelinewise_tap_mysql-1.6.0/tap_mysql/sync_strategies/incremental.py
```

### Comparing `pipelinewise-tap-mysql-1.5.6/LICENSE` & `pipelinewise_tap_mysql-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.6/PKG-INFO` & `pipelinewise_tap_mysql-1.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: pipelinewise-tap-mysql
-Version: 1.5.6
-Summary: Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible
-Home-page: https://github.com/transferwise/pipelinewise-tap-mysql
-Author: Wise
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Programming Language :: Python :: 3 :: Only
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # pipelinewise-tap-mysql
 
 [![PyPI version](https://badge.fury.io/py/pipelinewise-tap-mysql.svg)](https://badge.fury.io/py/pipelinewise-tap-mysql)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pipelinewise-tap-mysql.svg)](https://pypi.org/project/pipelinewise-tap-mysql/)
 [![License: MIT](https://img.shields.io/badge/License-GPLv3-yellow.svg)](https://opensource.org/licenses/GPL-3.0)
 
 [Singer](https://www.singer.io/) tap that extracts data from a [MySQL](https://www.mysql.com/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
```

### Comparing `pipelinewise-tap-mysql-1.5.6/README.md` & `pipelinewise_tap_mysql-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: pipelinewise-tap-mysql
+Version: 1.6.0
+Summary: Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible
+Home-page: https://github.com/transferwise/pipelinewise-tap-mysql
+Author: Wise
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3 :: Only
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pendulum==2.1.2
+Requires-Dist: pipelinewise-singer-python==1.*
+Requires-Dist: mysql-replication==0.43
+Requires-Dist: PyMySQL==1.1.*
+Requires-Dist: plpygis==0.2.1
+Requires-Dist: tzlocal==2.1
+Provides-Extra: test
+Requires-Dist: nose==1.3.*; extra == "test"
+Requires-Dist: pylint==2.13.2; extra == "test"
+Requires-Dist: nose-cov==1.6; extra == "test"
+
 # pipelinewise-tap-mysql
 
 [![PyPI version](https://badge.fury.io/py/pipelinewise-tap-mysql.svg)](https://badge.fury.io/py/pipelinewise-tap-mysql)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pipelinewise-tap-mysql.svg)](https://pypi.org/project/pipelinewise-tap-mysql/)
 [![License: MIT](https://img.shields.io/badge/License-GPLv3-yellow.svg)](https://opensource.org/licenses/GPL-3.0)
 
 [Singer](https://www.singer.io/) tap that extracts data from a [MySQL](https://www.mysql.com/) database and produces JSON-formatted data following the [Singer spec](https://github.com/singer-io/getting-started/blob/master/docs/SPEC.md).
```

### Comparing `pipelinewise-tap-mysql-1.5.6/pipelinewise_tap_mysql.egg-info/PKG-INFO` & `pipelinewise_tap_mysql-1.6.0/pipelinewise_tap_mysql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 Metadata-Version: 2.1
 Name: pipelinewise-tap-mysql
-Version: 1.5.6
+Version: 1.6.0
 Summary: Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible
 Home-page: https://github.com/transferwise/pipelinewise-tap-mysql
 Author: Wise
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: pendulum==2.1.2
+Requires-Dist: pipelinewise-singer-python==1.*
+Requires-Dist: mysql-replication==0.43
+Requires-Dist: PyMySQL==1.1.*
+Requires-Dist: plpygis==0.2.1
+Requires-Dist: tzlocal==2.1
+Provides-Extra: test
+Requires-Dist: nose==1.3.*; extra == "test"
+Requires-Dist: pylint==2.13.2; extra == "test"
+Requires-Dist: nose-cov==1.6; extra == "test"
 
 # pipelinewise-tap-mysql
 
 [![PyPI version](https://badge.fury.io/py/pipelinewise-tap-mysql.svg)](https://badge.fury.io/py/pipelinewise-tap-mysql)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pipelinewise-tap-mysql.svg)](https://pypi.org/project/pipelinewise-tap-mysql/)
 [![License: MIT](https://img.shields.io/badge/License-GPLv3-yellow.svg)](https://opensource.org/licenses/GPL-3.0)
```

### Comparing `pipelinewise-tap-mysql-1.5.6/pipelinewise_tap_mysql.egg-info/SOURCES.txt` & `pipelinewise_tap_mysql-1.6.0/pipelinewise_tap_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.6/setup.py` & `pipelinewise_tap_mysql-1.6.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='pipelinewise-tap-mysql',
-      version='1.5.6',
+      version='1.6.0',
       description='Singer.io tap for extracting data from MySQL & MariaDB - PipelineWise compatible',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Wise',
       url='https://github.com/transferwise/pipelinewise-tap-mysql',
       classifiers=[
           'License :: OSI Approved :: GNU Affero General Public License v3',
```

### Comparing `pipelinewise-tap-mysql-1.5.6/tap_mysql/__init__.py` & `pipelinewise_tap_mysql-1.6.0/tap_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.6/tap_mysql/connection.py` & `pipelinewise_tap_mysql-1.6.0/tap_mysql/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             "host": config["host"],
             "port": int(config["port"]),
             "cursorclass": config.get("cursorclass") or pymysql.cursors.SSCursor,
             "connect_timeout": CONNECT_TIMEOUT_SECONDS,
             "charset": "utf8",
         }
 
-        ssl_arg = None
+        ssl_arg = {"": True}
 
         if config.get("database"):
             args["database"] = config["database"]
 
         # Attempt self-signed SSL if config vars are present
         use_self_signed_ssl = config.get("ssl_ca") and config.get("ssl_cert") and config.get("ssl_key")
```

### Comparing `pipelinewise-tap-mysql-1.5.6/tap_mysql/discover_utils.py` & `pipelinewise_tap_mysql-1.6.0/tap_mysql/discover_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.6/tap_mysql/stream_utils.py` & `pipelinewise_tap_mysql-1.6.0/tap_mysql/stream_utils.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.6/tap_mysql/sync_strategies/binlog.py` & `pipelinewise_tap_mysql-1.6.0/tap_mysql/sync_strategies/binlog.py`

 * *Files 0% similar despite different names*

```diff
@@ -805,15 +805,15 @@
 
     Returns: Instance of BinlogStreamReader
     """
     if config.get('server_id'):
         server_id = int(config.get('server_id'))
         LOGGER.info("Using provided server_id=%s", server_id)
     else:
-        server_id = random.randint(1, 2 ^ 32)  # generate random server id for this slave
+        server_id = random.randint(1, 2 ** 32 - 1)  # generate random server id for this slave
         LOGGER.info("Using randomly generated server_id=%s", server_id)
 
     engine = config['engine']
 
     kwargs = {
         'connection_settings': {},
         'pymysql_wrapper': make_connection_wrapper(config),
```

### Comparing `pipelinewise-tap-mysql-1.5.6/tap_mysql/sync_strategies/common.py` & `pipelinewise_tap_mysql-1.6.0/tap_mysql/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.6/tap_mysql/sync_strategies/full_table.py` & `pipelinewise_tap_mysql-1.6.0/tap_mysql/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `pipelinewise-tap-mysql-1.5.6/tap_mysql/sync_strategies/incremental.py` & `pipelinewise_tap_mysql-1.6.0/tap_mysql/sync_strategies/incremental.py`

 * *Files identical despite different names*

