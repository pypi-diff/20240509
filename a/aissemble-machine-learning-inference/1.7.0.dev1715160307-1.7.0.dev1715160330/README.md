# Comparing `tmp/aissemble_machine_learning_inference-1.7.0.dev1715160307.tar.gz` & `tmp/aissemble_machine_learning_inference-1.7.0.dev1715160330.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aissemble_machine_learning_inference-1.7.0.dev1715160307.tar", max compression
+gzip compressed data, was "aissemble_machine_learning_inference-1.7.0.dev1715160330.tar", max compression
```

## Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307.tar` & `aissemble_machine_learning_inference-1.7.0.dev1715160330.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     9580 2024-05-08 09:24:41.837360 aissemble_machine_learning_inference-1.7.0.dev1715160307/LICENSE
--rw-r--r--   0        0        0     1893 2024-05-08 09:25:07.826670 aissemble_machine_learning_inference-1.7.0.dev1715160307/pyproject.toml
--rw-r--r--   0        0        0      208 2024-05-08 09:24:41.797361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:24:41.717363 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/__init__.py.tmp
--rw-r--r--   0        0        0      208 2024-05-08 09:24:41.797361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:24:37.717469 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/__init__.py.tmp
--rw-r--r--   0        0        0     1460 2024-05-08 09:24:41.797361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py
--rw-r--r--   0        0        0     1252 2024-05-08 09:24:41.717363 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py.tmp
--rw-r--r--   0        0        0     1768 2024-05-08 09:24:41.787361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py
--rw-r--r--   0        0        0     1560 2024-05-08 09:24:41.707363 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py.tmp
--rw-r--r--   0        0        0     1661 2024-05-08 09:24:41.777361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py
--rw-r--r--   0        0        0     1453 2024-05-08 09:24:41.697364 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py.tmp
--rw-r--r--   0        0        0     1642 2024-05-08 09:24:41.787361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py
--rw-r--r--   0        0        0     1434 2024-05-08 09:24:41.707363 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py.tmp
--rw-r--r--   0        0        0     1680 2024-05-08 09:24:41.787361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py
--rw-r--r--   0        0        0     1472 2024-05-08 09:24:41.707363 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py.tmp
--rw-r--r--   0        0        0     1586 2024-05-08 09:24:41.787361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py
--rw-r--r--   0        0        0     1378 2024-05-08 09:24:41.707363 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py.tmp
--rw-r--r--   0        0        0      208 2024-05-08 09:24:41.767362 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:24:41.697364 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/__init__.py.tmp
--rw-r--r--   0        0        0      208 2024-05-08 09:24:41.777361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:24:41.737363 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/__init__.py.tmp
--rw-r--r--   0        0        0      208 2024-05-08 09:24:41.777361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:24:41.697364 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/__init__.py.tmp
--rw-r--r--   0        0        0     1640 2024-05-08 09:25:03.076796 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2.py
--rw-r--r--   0        0        0     1217 2024-05-08 09:25:03.076796 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2_grpc.py
--rw-r--r--   0        0        0     5696 2024-05-08 09:24:41.777361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py
--rw-r--r--   0        0        0     5487 2024-05-08 09:24:41.697364 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py.tmp
--rw-r--r--   0        0        0     2931 2024-05-08 09:25:03.076796 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2.py
--rw-r--r--   0        0        0     6582 2024-05-08 09:25:03.076796 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2_grpc.py
--rw-r--r--   0        0        0      208 2024-05-08 09:24:41.767362 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/rest/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:24:41.697364 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/rest/__init__.py.tmp
--rw-r--r--   0        0        0     2366 2024-05-08 09:24:41.767362 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py
--rw-r--r--   0        0        0     2158 2024-05-08 09:24:41.697364 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py.tmp
--rw-r--r--   0        0        0      208 2024-05-08 09:24:41.757362 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:24:37.677471 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/__init__.py.tmp
--rw-r--r--   0        0        0     3006 2024-05-08 09:24:41.767362 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py
--rw-r--r--   0        0        0     2798 2024-05-08 09:24:41.727363 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py.tmp
--rw-r--r--   0        0        0     2910 2024-05-08 09:24:41.757362 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py
--rw-r--r--   0        0        0     2702 2024-05-08 09:24:41.697364 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py.tmp
--rw-r--r--   0        0        0     6369 2024-05-08 09:24:41.767362 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py
--rw-r--r--   0        0        0     6161 2024-05-08 09:24:41.727363 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py.tmp
--rw-r--r--   0        0        0     2902 2024-05-08 09:24:41.757362 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py
--rw-r--r--   0        0        0     2694 2024-05-08 09:24:41.697364 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py.tmp
--rw-r--r--   0        0        0      208 2024-05-08 09:24:41.797361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/validation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 09:24:41.717363 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/validation/__init__.py.tmp
--rw-r--r--   0        0        0     1456 2024-05-08 09:24:41.797361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py
--rw-r--r--   0        0        0     1247 2024-05-08 09:24:41.717363 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py.tmp
--rw-r--r--   0        0        0     1748 2024-05-08 09:24:41.797361 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py
--rw-r--r--   0        0        0     1540 2024-05-08 09:24:41.717363 aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py.tmp
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 aissemble_machine_learning_inference-1.7.0.dev1715160307/PKG-INFO
+-rw-r--r--   0        0        0     9580 2024-05-08 09:25:01.791662 aissemble_machine_learning_inference-1.7.0.dev1715160330/LICENSE
+-rw-r--r--   0        0        0     1893 2024-05-08 09:25:30.826671 aissemble_machine_learning_inference-1.7.0.dev1715160330/pyproject.toml
+-rw-r--r--   0        0        0      208 2024-05-08 09:25:01.749662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:25:01.679662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/__init__.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-08 09:25:01.749662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:24:57.825661 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/__init__.py.tmp
+-rw-r--r--   0        0        0     1460 2024-05-08 09:25:01.749662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py
+-rw-r--r--   0        0        0     1252 2024-05-08 09:25:01.678662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py.tmp
+-rw-r--r--   0        0        0     1768 2024-05-08 09:25:01.741662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py
+-rw-r--r--   0        0        0     1560 2024-05-08 09:25:01.662662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py.tmp
+-rw-r--r--   0        0        0     1661 2024-05-08 09:25:01.739662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py
+-rw-r--r--   0        0        0     1453 2024-05-08 09:25:01.658662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py.tmp
+-rw-r--r--   0        0        0     1642 2024-05-08 09:25:01.743662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py
+-rw-r--r--   0        0        0     1434 2024-05-08 09:25:01.666662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py.tmp
+-rw-r--r--   0        0        0     1680 2024-05-08 09:25:01.745662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py
+-rw-r--r--   0        0        0     1472 2024-05-08 09:25:01.670662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py.tmp
+-rw-r--r--   0        0        0     1586 2024-05-08 09:25:01.747662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py
+-rw-r--r--   0        0        0     1378 2024-05-08 09:25:01.674662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-08 09:25:01.734662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:25:01.653662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/__init__.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-08 09:25:01.736662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:25:01.698662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/__init__.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-08 09:25:01.736662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:25:01.655662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/__init__.py.tmp
+-rw-r--r--   0        0        0     1640 2024-05-08 09:25:26.242670 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2.py
+-rw-r--r--   0        0        0     1217 2024-05-08 09:25:26.242670 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2_grpc.py
+-rw-r--r--   0        0        0     5696 2024-05-08 09:25:01.736662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py
+-rw-r--r--   0        0        0     5487 2024-05-08 09:25:01.654662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py.tmp
+-rw-r--r--   0        0        0     2931 2024-05-08 09:25:26.242670 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2.py
+-rw-r--r--   0        0        0     6582 2024-05-08 09:25:26.242670 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2_grpc.py
+-rw-r--r--   0        0        0      208 2024-05-08 09:25:01.731662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/rest/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:25:01.651662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/rest/__init__.py.tmp
+-rw-r--r--   0        0        0     2366 2024-05-08 09:25:01.733662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py
+-rw-r--r--   0        0        0     2158 2024-05-08 09:25:01.652662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-08 09:25:01.725662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:24:57.793661 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/__init__.py.tmp
+-rw-r--r--   0        0        0     3006 2024-05-08 09:25:01.728662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py
+-rw-r--r--   0        0        0     2798 2024-05-08 09:25:01.690662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py.tmp
+-rw-r--r--   0        0        0     2910 2024-05-08 09:25:01.723662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py
+-rw-r--r--   0        0        0     2702 2024-05-08 09:25:01.648662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py.tmp
+-rw-r--r--   0        0        0     6369 2024-05-08 09:25:01.731662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py
+-rw-r--r--   0        0        0     6161 2024-05-08 09:25:01.695662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py.tmp
+-rw-r--r--   0        0        0     2902 2024-05-08 09:25:01.725662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py
+-rw-r--r--   0        0        0     2694 2024-05-08 09:25:01.650662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py.tmp
+-rw-r--r--   0        0        0      208 2024-05-08 09:25:01.754662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/validation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 09:25:01.685662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/validation/__init__.py.tmp
+-rw-r--r--   0        0        0     1456 2024-05-08 09:25:01.752662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py
+-rw-r--r--   0        0        0     1247 2024-05-08 09:25:01.680662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py.tmp
+-rw-r--r--   0        0        0     1748 2024-05-08 09:25:01.754662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py
+-rw-r--r--   0        0        0     1540 2024-05-08 09:25:01.684662 aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py.tmp
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 aissemble_machine_learning_inference-1.7.0.dev1715160330/PKG-INFO
```

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/LICENSE` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/LICENSE`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/pyproject.toml` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # GENERATED STUB - PLEASE ***DO*** MODIFY
 # Originally generated from templates/inference/pyproject.toml.vm.
 
 [tool.poetry]
 name = "aissemble-machine-learning-inference"
-version = "1.7.0.dev1715160307"
+version = "1.7.0.dev1715160330"
 description = "Machine Learning Inference Test Module"
 authors = ["aiSSEMBLE Baseline Community <aissemble@bah.com>"]
 
 # Ensure that generated code is included in package archives
 include = ["src/aissemble_machine_learning_inference/generated/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/date_as_seconds_since_epoch_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/event_category_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/event_kind_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/event_outcome_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/ip_address_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/dictionary/port_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2_grpc.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/generated/inference_payload_definition_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_grpc_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2_grpc.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/grpc/inference_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/inference/rest/inference_payload_definition.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/adversarial_threat_prediction_field.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/event_log_entry_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/record/event_log_entry_field.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/validation/inference_message_definition_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py.tmp` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/src/aissemble_machine_learning_inference/generated/validation/inference_payload_definition_base.py.tmp`

 * *Files identical despite different names*

### Comparing `aissemble_machine_learning_inference-1.7.0.dev1715160307/PKG-INFO` & `aissemble_machine_learning_inference-1.7.0.dev1715160330/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aissemble-machine-learning-inference
-Version: 1.7.0.dev1715160307
+Version: 1.7.0.dev1715160330
 Summary: Machine Learning Inference Test Module
 Author: aiSSEMBLE Baseline Community
 Author-email: aissemble@bah.com
 Requires-Python: >=3.11.4,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aissemble-extensions-encryption-vault-python (==1.7.0.*)
```

