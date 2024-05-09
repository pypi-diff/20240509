# Comparing `tmp/th2_data_services-2.0.0.dev8981619855.tar.gz` & `tmp/th2_data_services-2.0.0.dev9014376771.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "th2_data_services-2.0.0.dev8981619855.tar", last modified: Tue May  7 07:49:32 2024, max compression
+gzip compressed data, was "th2_data_services-2.0.0.dev9014376771.tar", last modified: Thu May  9 08:12:23 2024, max compression
```

## Comparing `th2_data_services-2.0.0.dev8981619855.tar` & `th2_data_services-2.0.0.dev9014376771.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.102081 th2_data_services-2.0.0.dev8981619855/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-05-07 07:49:32.102081 th2_data_services-2.0.0.dev8981619855/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 07:49:20.000000 th2_data_services-2.0.0.dev8981619855/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:49:32.102081 th2_data_services-2.0.0.dev8981619855/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.094081 th2_data_services-2.0.0.dev8981619855/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.098080 th2_data_services-2.0.0.dev8981619855/th2_data_services/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/_internal/perf_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.098080 th2_data_services-2.0.0.dev8981619855/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    41867 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.098080 th2_data_services-2.0.0.dev8981619855/th2_data_services/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/dummy/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.098080 th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.098080 th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.098080 th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.102081 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/_is_sorted_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.102081 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.102081 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22097 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/path_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/sse_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.102081 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/stream_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/stream_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/stream_utils/stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.102081 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-07 07:48:19.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:49:32.098080 th2_data_services-2.0.0.dev8981619855/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-05-07 07:49:31.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-07 07:49:32.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:49:31.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-07 07:49:31.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 07:49:31.000000 th2_data_services-2.0.0.dev8981619855/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.292359 th2_data_services-2.0.0.dev9014376771/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-05-09 08:12:23.288359 th2_data_services-2.0.0.dev9014376771/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35047 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 08:12:15.000000 th2_data_services-2.0.0.dev9014376771/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:12:23.292359 th2_data_services-2.0.0.dev9014376771/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.280359 th2_data_services-2.0.0.dev9014376771/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.284359 th2_data_services-2.0.0.dev9014376771/th2_data_services/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/_internal/perf_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.284359 th2_data_services-2.0.0.dev9014376771/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41867 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.284359 th2_data_services-2.0.0.dev9014376771/th2_data_services/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/dummy/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.284359 th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16239 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26246 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.284359 th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.284359 th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.288359 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/_is_sorted_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16455 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.288359 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11641 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8434 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12146 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16194 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.288359 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22097 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/path_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/sse_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.288359 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/stream_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/stream_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/stream_utils/stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7498 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.288359 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-05-09 08:11:26.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:12:23.284359 th2_data_services-2.0.0.dev9014376771/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42588 2024-05-09 08:12:23.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-09 08:12:23.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:12:23.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-09 08:12:23.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 08:12:23.000000 th2_data_services-2.0.0.dev9014376771/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev8981619855/LICENSE` & `th2_data_services-2.0.0.dev9014376771/LICENSE`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/PKG-INFO` & `th2_data_services-2.0.0.dev9014376771/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3839 3831 3631 3938 3535 0a53 756d 6d61  8981619855.Summa
+00000040: 3930 3134 3337 3637 3731 0a53 756d 6d61  9014376771.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev8981619855/README.md` & `th2_data_services-2.0.0.dev9014376771/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/setup.py` & `th2_data_services-2.0.0.dev9014376771/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/_internal/__init__.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/_internal/perf_tests.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/_internal/perf_tests.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/data.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/dummy/__init__.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/dummy/data_source.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/dummy/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/utils/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,44 +80,59 @@
         seconds, nanoseconds = cls.parse_timestamp_int(timestamp)
         nanoseconds_str = f"{nanoseconds:0>9}"
         microseconds = nanoseconds_str[:-3]
         ts = float(str(seconds) + "." + microseconds)
         return datetime.utcfromtimestamp(ts)
 
     @classmethod
-    def to_microseconds(cls, timestamp: TimestampType) -> int:
-        """Converts timestamp to microseconds.
+    def to_seconds(cls, timestamp: TimestampType):
+        """Converts timestamp to seconds.
 
         If your timestamp has nanoseconds, they will be just cut (not rounding).
 
         Args:
             timestamp: TimestampType object to convert.
 
         Returns:
-            int: Timestamp in microseconds format.
+            int: Timestamp in seconds format.
         """
         seconds, nanoseconds = cls.parse_timestamp(timestamp)
-        return int(f"{seconds}{nanoseconds[:-3]}")
+        return int(seconds)
 
     @classmethod
-    def to_milliseconds(cls, timestamp: TimestampType):
+    def to_milliseconds(cls, timestamp: TimestampType) -> int:
         """Converts timestamp to milliseconds.
 
         If your timestamp has nanoseconds, they will be just cut (not rounding).
 
         Args:
             timestamp: TimestampType object to convert.
 
         Returns:
             int: Timestamp in microseconds format.
         """
         seconds, nanoseconds = cls.parse_timestamp(timestamp)
         return int(f"{seconds}{nanoseconds[:-6]}")
 
     @classmethod
+    def to_microseconds(cls, timestamp: TimestampType) -> int:
+        """Converts timestamp to microseconds.
+
+        If your timestamp has nanoseconds, they will be just cut (not rounding).
+
+        Args:
+            timestamp: TimestampType object to convert.
+
+        Returns:
+            int: Timestamp in microseconds format.
+        """
+        seconds, nanoseconds = cls.parse_timestamp(timestamp)
+        return int(f"{seconds}{nanoseconds[:-3]}")
+
+    @classmethod
     def to_nanoseconds(cls, timestamp: TimestampType) -> int:
         """Converts timestamp to nanoseconds.
 
         Args:
             timestamp: TimestampType object to convert.
 
         Returns:
```

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/_is_sorted_result.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/_is_sorted_result.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,29 @@
 
     @classmethod
     def parse_timestamp_int(cls, timestamp: dict) -> (int, int):
         seconds, nanoseconds = timestamp["epochSecond"], timestamp["nano"]
         return seconds, nanoseconds
 
     @classmethod
+    def to_seconds(cls, timestamp: TimestampType):
+        """Converts timestamp to seconds.
+
+        If your timestamp has nanoseconds, they will be just cut (not rounding).
+
+        Args:
+            timestamp: TimestampType object to convert.
+
+        Returns:
+            int: Timestamp in seconds format.
+        """
+        seconds, nanoseconds = cls.parse_timestamp_int(timestamp)
+        return seconds
+
+    @classmethod
     def to_microseconds(cls, timestamp: TimestampType) -> int:
         """Converts timestamp to microseconds.
 
         If your timestamp has nanoseconds, they will be just cut (not rounding).
 
         Args:
             timestamp: TimestampType object to convert.
```

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/data_utils.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/experimental.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 from typing import List
 
-from th2_data_services.provider.v5.commands import http
-from th2_data_services.provider.v5.data_source import HTTPProvider5DataSource
-
 import th2_data_services.utils
 from th2_data_services.config import options
 from th2_data_services.utils.converters import flatten_dict
 from th2_data_services.utils.message_utils import message_utils
 
 
 def prepare_story_from_storage(
```

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/path_utils.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/path_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     # -2 because we also have to add '/' symbol and at least 1 symbol for filename
     if parent_path_len >= options.MAX_PATH - 2:
         raise ValueError(
             f"It's impossible to create valid path for provided one: {filepath}. "
             f"Because its parent part is longer than Max possible OS path. {parent_path_len} >= {options.MAX_PATH-2}."
         )
 
-    max_filename_len = path_len - parent_path_len
+    max_filename_len = options.MAX_PATH - parent_path_len
     valid_filename = transform_filename_to_valid(filepath.name)[:max_filename_len]
 
     return filepath.parent / valid_filename
 
 
 def check_if_filename_valid(filename: str):
     """Returns status and reason string.
```

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/stream_utils/__init__.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/stream_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/stream_utils/stream_utils.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/stream_utils/stream_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  limitations under the License.
 
 from datetime import datetime, timezone
 from functools import wraps, partial
 from typing import Dict, Union, Callable
 from deprecated.classic import deprecated
 import time as time_
-from th2_data_services.utils.converters import Th2TimestampConverter
+from th2_data_services.utils.converters import Th2TimestampConverter, DatetimeConverter
 
 
 def extract_timestamp(timestamp_element: Dict) -> str:
     """Returns datetime string in the format: 2023-10-02T10:47:20.413072000."""
     return Th2TimestampConverter.to_datetime_str(timestamp_element)
 
 
@@ -72,32 +72,42 @@
     et_seconds, et_nanoseconds = Th2TimestampConverter.parse_timestamp_int(end_timestamp)
 
     seconds_delta = (et_seconds - st_seconds) * 1000000
     nano_delta = (et_nanoseconds - st_nanoseconds) / 1000
     return seconds_delta + nano_delta
 
 
-# TODO - looks ok, but we need to think about unified timestamps
 def time_slice_object_filter(
     timestamp_field: str, start_timestamp_iso: str, duration_seconds: int
 ) -> Callable:  # noqa
-    """Filter elements that from time moment `A` to `A+duration_seconds`.
+    """Returns filter function for `Data.filter` method.
+
+    Filter elements that from time moment `A` to `A+duration_seconds`.
 
     Args:
         timestamp_field: expects the field name that contains ProtobufTimestamp
             It usually 'timestamp' field.
         start_timestamp_iso: string in the ISO 8601 format.
             Example: 2009-05-28T16:15:00 or 2021-12-25
             Note: It cannot take strings with `Z` in the end.
         duration_seconds: seconds.
 
     Returns:
         Filter function.
+
+    Examples:
+        1. data.filter(time_slice_object_filter('startTimestamp', '2009-05-28T16:15:00, 300))
     """
-    ts1 = datetime.fromisoformat(start_timestamp_iso).timestamp()
+    # TODO
+    #   1. looks ok, but we need to think about unified timestamps
+    # FixMe
+    #   1. timestamp_field -- the problem here if the field is placed not in the root of the dict.
+    #   2. it expects, that `obj[timestamp_field]` == Th2Timestamp
+
+    ts1 = DatetimeConverter.to_seconds(datetime.fromisoformat(start_timestamp_iso))
     ts2 = ts1 + duration_seconds
 
     # FIXME
     #   time_interval_filter_seconds_precision require ProtobufTimestamp var as
     #   a first argument now.
     #
     #   TODO - We should do our methods universal!
```

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev9014376771/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev9014376771/th2_data_services.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3839 3831 3631 3938 3535 0a53 756d 6d61  8981619855.Summa
+00000040: 3930 3134 3337 3637 3731 0a53 756d 6d61  9014376771.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev9014376771/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev8981619855/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev9014376771/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

