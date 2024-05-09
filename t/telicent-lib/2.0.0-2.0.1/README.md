# Comparing `tmp/telicent_lib-2.0.0.tar.gz` & `tmp/telicent_lib-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telicent_lib-2.0.0.tar", last modified: Thu May  2 09:16:15 2024, max compression
+gzip compressed data, was "telicent_lib-2.0.1.tar", last modified: Thu May  9 13:18:46 2024, max compression
```

## Comparing `telicent_lib-2.0.0.tar` & `telicent_lib-2.0.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:16:15.365936 telicent_lib-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-05-02 09:16:15.365936 telicent_lib-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 09:16:15.365936 telicent_lib-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:16:15.353936 telicent_lib-2.0.0/telicent_lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:16:15.357936 telicent_lib-2.0.0/telicent_lib/access/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/access/edhv1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/access/edhv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/access/security_labels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:16:15.357936 telicent_lib-2.0.0/telicent_lib/access/ukihm/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/access/ukihm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/access/ukihm/edh_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    27204 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    10976 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:16:15.357936 telicent_lib-2.0.0/telicent_lib/config/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/config/configSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/config/configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:16:15.357936 telicent_lib-2.0.0/telicent_lib/middleware/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/middleware/decode_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     6256 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/projector.py
--rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/records.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:16:15.357936 telicent_lib-2.0.0/telicent_lib/sinks/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/sinks/dataSink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/sinks/dictSink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/sinks/kafkaSink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/sinks/listSink.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/sinks/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:16:15.357936 telicent_lib-2.0.0/telicent_lib/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/sources/dataSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/sources/deserializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/sources/dictSource.py
--rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/sources/kafkaSource.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/sources/listSource.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/telicent_lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:16:15.361936 telicent_lib-2.0.0/telicent_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-05-02 09:16:15.000000 telicent_lib-2.0.0/telicent_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-02 09:16:15.000000 telicent_lib-2.0.0/telicent_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 09:16:15.000000 telicent_lib-2.0.0/telicent_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-02 09:16:15.000000 telicent_lib-2.0.0/telicent_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-02 09:16:15.000000 telicent_lib-2.0.0/telicent_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 09:16:15.361936 telicent_lib-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_decode_token_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_edh_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_generate_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_projector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_protocol_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_security_labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_security_labels_edhv1.py
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_serdes.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_sinks.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-02 09:16:08.000000 telicent_lib-2.0.0/tests/test_sources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.592571 telicent_lib-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-05-09 13:18:46.592571 telicent_lib-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:18:46.592571 telicent_lib-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.580571 telicent_lib-2.0.1/telicent_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.584571 telicent_lib-2.0.1/telicent_lib/access/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/access/edhv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/access/edhv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/access/security_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.584571 telicent_lib-2.0.1/telicent_lib/access/ukihm/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/access/ukihm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/access/ukihm/edh_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27204 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.584571 telicent_lib-2.0.1/telicent_lib/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/config/configSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/config/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9160 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.584571 telicent_lib-2.0.1/telicent_lib/middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/middleware/decode_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/projector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.584571 telicent_lib-2.0.1/telicent_lib/sinks/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sinks/dataSink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sinks/dictSink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sinks/kafkaSink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sinks/listSink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sinks/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.588571 telicent_lib-2.0.1/telicent_lib/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sources/dataSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sources/deserializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sources/dictSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18619 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sources/kafkaSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/sources/listSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/telicent_lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.592571 telicent_lib-2.0.1/telicent_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-05-09 13:18:46.000000 telicent_lib-2.0.1/telicent_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-09 13:18:46.000000 telicent_lib-2.0.1/telicent_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:18:46.000000 telicent_lib-2.0.1/telicent_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-09 13:18:46.000000 telicent_lib-2.0.1/telicent_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-09 13:18:46.000000 telicent_lib-2.0.1/telicent_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:18:46.592571 telicent_lib-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_decode_token_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_edh_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_generate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_projector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_protocol_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13170 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_security_labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_security_labels_edhv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_serdes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_sinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-09 13:18:40.000000 telicent_lib-2.0.1/tests/test_sources.py
```

### Comparing `telicent_lib-2.0.0/LICENSE` & `telicent_lib-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/PKG-INFO` & `telicent_lib-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telicent-lib
-Version: 2.0.0
+Version: 2.0.1
 Summary: A helper package for building Adapters, Mappers and Projectors for Telicent Core
 Author-email: Telicent Ltd <admin@telicent.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `telicent_lib-2.0.0/README.md` & `telicent_lib-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/pyproject.toml` & `telicent_lib-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2.0", "wheel==0.41.3", "pip-tools==7.3.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "telicent-lib"
-version = "2.0.0"
+version = "2.0.1"
 authors = [{name = "Telicent Ltd", email = "admin@telicent.io"}]
 description = "A helper package for building Adapters, Mappers and Projectors for Telicent Core"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 readme = "README.md"
 dependencies = [
     "colored==1.4.4",
```

### Comparing `telicent_lib-2.0.0/telicent_lib/__init__.py` & `telicent_lib-2.0.1/telicent_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/access/__init__.py` & `telicent_lib-2.0.1/telicent_lib/access/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/access/edhv1.py` & `telicent_lib-2.0.1/telicent_lib/access/edhv1.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/access/edhv2.py` & `telicent_lib-2.0.1/telicent_lib/access/edhv2.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/access/security_labels.py` & `telicent_lib-2.0.1/telicent_lib/access/security_labels.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/access/ukihm/__init__.py` & `telicent_lib-2.0.1/telicent_lib/access/ukihm/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/access/ukihm/edh_model.py` & `telicent_lib-2.0.1/telicent_lib/access/ukihm/edh_model.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/action.py` & `telicent_lib-2.0.1/telicent_lib/action.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/adapter.py` & `telicent_lib-2.0.1/telicent_lib/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             self.print_coloured("Waiting for data from " + self.source_name +
                                 " - will write out to " + str(self.target))
         else:
             self.print_coloured("Waiting for data - will write out to " + str(self.target))
 
         if self.reporter is not None:
             self.reporter.run()
-            self.print_coloured(f"Telicent Live Reporter registered to send heartbeats to {self.reporter.target}")
+            self.print_coloured(f"Telicent Live Reporter registered to send heartbeats to {self.reporter.sink}")
 
         self.started()
 
     def finished(self) -> None:
         self.target.close()
         super().finished()
```

### Comparing `telicent_lib-2.0.0/telicent_lib/config/__init__.py` & `telicent_lib-2.0.1/telicent_lib/config/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/config/configSource.py` & `telicent_lib-2.0.1/telicent_lib/config/configSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/config/configurator.py` & `telicent_lib-2.0.1/telicent_lib/config/configurator.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/errors.py` & `telicent_lib-2.0.1/telicent_lib/errors.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/exceptions.py` & `telicent_lib-2.0.1/telicent_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/logging.py` & `telicent_lib-2.0.1/telicent_lib/logging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from __future__ import annotations
 
 import json
 import logging
-import sys
-import traceback
 from typing import Any, MutableMapping
 
 from confluent_kafka import KafkaException
 
 from telicent_lib import Record, RecordUtils
 from telicent_lib.sinks import KafkaSink
 
@@ -27,15 +25,14 @@
 limitations under the License.
 """
 
 
 class CoreLogFormats:
     BASIC = ['name', 'levelname', 'msg', 'created']
     CORE = ['name', 'log_type', 'levelname', 'msg', 'created']
-    UNHANDLED_EXCEPTION = ['name', 'log_type', 'levelname', 'msg', 'created', 'unhandled_info']
 
 
 MERGE = 0
 REPLACE = 1
 
 
 class CoreLoggerAdapter(logging.LoggerAdapter):
@@ -139,33 +136,8 @@
             fmt = CoreLogFormats.CORE
 
         handler.setFormatter(JSONFormatter(fmt))
 
         logger.addHandler(handler)
         core_logger = CoreLoggerAdapter(logger, headers=headers, log_type=log_type, header_method=header_method)
 
-        def handle_unhandled_exception(exc_type, exc_value, exc_traceback):
-            if issubclass(exc_type, KeyboardInterrupt):
-                sys.__excepthook__(exc_type, exc_value, exc_traceback)
-                return
-            traceback_info = traceback.extract_tb(exc_traceback)
-            if traceback_info:
-                filename, lineno, funcname, _ = traceback_info[-1]
-            else:
-                filename, lineno, funcname = "", "", ""
-
-            extra_info = {
-                'exception_type': str(exc_type),
-                'exception_value': str(exc_value),
-                'filename': filename,
-                'lineno': lineno,
-                'func': funcname
-            }
-            for _handler in filter(lambda h: isinstance(h, KafkaHandler), core_logger.logger.handlers):
-                _handler.setFormatter(JSONFormatter(CoreLogFormats.UNHANDLED_EXCEPTION))
-            core_logger.critical(
-                "Unhandled exception", extra={'unhandled_info': extra_info}, log_type='CRITICAL'
-            )
-
-        sys.excepthook = handle_unhandled_exception
-
         return core_logger
```

### Comparing `telicent_lib-2.0.0/telicent_lib/mapper.py` & `telicent_lib-2.0.1/telicent_lib/mapper.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/middleware/__init__.py` & `telicent_lib-2.0.1/telicent_lib/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/middleware/decode_token.py` & `telicent_lib-2.0.1/telicent_lib/middleware/decode_token.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 
 import jwt
 import requests
 from werkzeug.wrappers import Request, Response
 
-from telicent_lib.config import Configurator, OnError
 from telicent_lib.exceptions import ConfigurationException
 from telicent_lib.logging import CoreLoggerFactory
 
 __license__ = """
 Copyright (c) Telicent Ltd.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -43,18 +42,16 @@
         self.jwks_url = jwks_url
 
         self.public_key_url = public_key_url
         if isinstance(self.public_key_url, str):
             self.public_key_url = self.public_key_url.strip("/")
         self.jwt_header = jwt_header
         if logger is None:
-            conf = Configurator()
             self.logger = CoreLoggerFactory.get_logger(
                 'Authenticator',
-                conf.get("BOOTSTRAP_SERVERS", required=True, on_error=OnError.RAISE_EXCEPTION)
             )
         else:
             self.logger = logger
 
     def __call__(self, environ, start_response):
         request = Request(environ)
         if self.jwt_header not in request.headers:
```

### Comparing `telicent_lib-2.0.0/telicent_lib/projector.py` & `telicent_lib-2.0.1/telicent_lib/projector.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         need only call this.
         """
         self.display_startup_banner()
         self.print_coloured("Waiting for data from " + str(self.source) +
                             " - will write out to " + self.target_store)
         if self.reporter is not None:
             self.reporter.run()
-            self.print_coloured(f"Telicent Live Reporter registered to send heartbeats to {self.reporter.target}")
+            self.print_coloured(f"Telicent Live Reporter registered to send heartbeats to {self.reporter.sink}")
         with self.source:
             try:
                 self.started()
                 self.__print_source_status__(self.source)
                 for _, record in enumerate(self.source.data()):
                     try:
                         traceparent = list(RecordUtils.get_headers(record, 'traceparent'))[-1]
```

### Comparing `telicent_lib-2.0.0/telicent_lib/records.py` & `telicent_lib-2.0.1/telicent_lib/records.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/reporter.py` & `telicent_lib-2.0.1/telicent_lib/reporter.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/sinks/__init__.py` & `telicent_lib-2.0.1/telicent_lib/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/sinks/dataSink.py` & `telicent_lib-2.0.1/telicent_lib/sinks/dataSink.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/sinks/dictSink.py` & `telicent_lib-2.0.1/telicent_lib/sinks/dictSink.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/sinks/kafkaSink.py` & `telicent_lib-2.0.1/telicent_lib/sinks/kafkaSink.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/sinks/listSink.py` & `telicent_lib-2.0.1/telicent_lib/sinks/listSink.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/sinks/serializers.py` & `telicent_lib-2.0.1/telicent_lib/sinks/serializers.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/sources/dataSource.py` & `telicent_lib-2.0.1/telicent_lib/sources/dataSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/sources/deserializers.py` & `telicent_lib-2.0.1/telicent_lib/sources/deserializers.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/sources/dictSource.py` & `telicent_lib-2.0.1/telicent_lib/sources/dictSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/sources/kafkaSource.py` & `telicent_lib-2.0.1/telicent_lib/sources/kafkaSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/sources/listSource.py` & `telicent_lib-2.0.1/telicent_lib/sources/listSource.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/status.py` & `telicent_lib-2.0.1/telicent_lib/status.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib/utils.py` & `telicent_lib-2.0.1/telicent_lib/utils.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/telicent_lib.egg-info/PKG-INFO` & `telicent_lib-2.0.1/telicent_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telicent-lib
-Version: 2.0.0
+Version: 2.0.1
 Summary: A helper package for building Adapters, Mappers and Projectors for Telicent Core
 Author-email: Telicent Ltd <admin@telicent.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `telicent_lib-2.0.0/telicent_lib.egg-info/SOURCES.txt` & `telicent_lib-2.0.1/telicent_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_adapter.py` & `telicent_lib-2.0.1/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_decode_token_middleware.py` & `telicent_lib-2.0.1/tests/test_decode_token_middleware.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_edh_model.py` & `telicent_lib-2.0.1/tests/test_edh_model.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_error_handler.py` & `telicent_lib-2.0.1/tests/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_generate_ids.py` & `telicent_lib-2.0.1/tests/test_generate_ids.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_mapper.py` & `telicent_lib-2.0.1/tests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_projector.py` & `telicent_lib-2.0.1/tests/test_projector.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_protocol_validation.py` & `telicent_lib-2.0.1/tests/test_protocol_validation.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_records.py` & `telicent_lib-2.0.1/tests/test_records.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_reporter.py` & `telicent_lib-2.0.1/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_security_labels.py` & `telicent_lib-2.0.1/tests/test_security_labels.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_security_labels_edhv1.py` & `telicent_lib-2.0.1/tests/test_security_labels_edhv1.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_serdes.py` & `telicent_lib-2.0.1/tests/test_serdes.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_sinks.py` & `telicent_lib-2.0.1/tests/test_sinks.py`

 * *Files identical despite different names*

### Comparing `telicent_lib-2.0.0/tests/test_sources.py` & `telicent_lib-2.0.1/tests/test_sources.py`

 * *Files identical despite different names*

