# Comparing `tmp/vayu_client-1.0.6.tar.gz` & `tmp/vayu_client-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vayu_client-1.0.6.tar", last modified: Thu May  9 13:42:36 2024, max compression
+gzip compressed data, was "vayu_client-1.0.7.tar", last modified: Thu May  9 13:53:14 2024, max compression
```

## Comparing `vayu_client-1.0.6.tar` & `vayu_client-1.0.7.tar`

### file list

```diff
@@ -1,101 +1,105 @@
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 13:42:36.479429 vayu_client-1.0.6/
--rw-r--r--   0 shaigross   (501) staff       (20)     2539 2024-05-09 13:42:36.479524 vayu_client-1.0.6/PKG-INFO
--rw-r--r--   0 shaigross   (501) staff       (20)      481 2024-05-08 15:19:35.000000 vayu_client-1.0.6/README.md
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 13:42:36.468229 vayu_client-1.0.6/entity_clients/
--rw-r--r--   0 shaigross   (501) staff       (20)       46 2024-05-08 13:47:16.000000 vayu_client-1.0.6/entity_clients/__init__.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1178 2024-05-09 10:52:12.000000 vayu_client-1.0.6/entity_clients/contracts_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1295 2024-05-09 10:52:16.000000 vayu_client-1.0.6/entity_clients/customers_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1413 2024-05-08 14:59:08.000000 vayu_client-1.0.6/entity_clients/events_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)      517 2024-05-09 10:52:12.000000 vayu_client-1.0.6/entity_clients/invoices_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1807 2024-05-09 10:52:12.000000 vayu_client-1.0.6/entity_clients/meters_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)      561 2024-05-09 10:52:12.000000 vayu_client-1.0.6/entity_clients/plans_client.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 13:42:36.469207 vayu_client-1.0.6/openapi_client/
--rw-r--r--   0 shaigross   (501) staff       (20)     6948 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/__init__.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 13:42:36.470384 vayu_client-1.0.6/openapi_client/api/
--rw-r--r--   0 shaigross   (501) staff       (20)      422 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/api/__init__.py
--rw-r--r--   0 shaigross   (501) staff       (20)    12591 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/api/auth_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    43742 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/api/contracts_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    55565 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/api/customers_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    61236 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/api/events_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    22281 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/api/invoices_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    43924 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/api/meters_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    32198 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/api/plans_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    26550 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/api_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)      652 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/api_response.py
--rw-r--r--   0 shaigross   (501) staff       (20)    15152 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/configuration.py
--rw-r--r--   0 shaigross   (501) staff       (20)     6180 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/exceptions.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 13:42:36.478716 vayu_client-1.0.6/openapi_client/models/
--rw-r--r--   0 shaigross   (501) staff       (20)     6030 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/__init__.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3340 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/aggregation_method.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1161 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/aggregation_operator.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1052 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/billing_interval.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3214 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/condition.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4112 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/create_contract_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/create_contract_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3084 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/create_customer_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/create_customer_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3889 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/create_customer_response_schema_customer.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3034 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/criterion.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1202 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/criterion_operator.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/delete_contract_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/delete_customer_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3134 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/delete_event_by_ref_id_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4983 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/delete_event_by_ref_id_response_schema_event.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3063 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/delete_meter_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3042 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/delete_plan_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4127 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/event.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3243 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/events_dry_run_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4380 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/events_dry_run_response_schema_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3921 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/events_dry_run_response_schema_inner_event.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4556 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3461 2024-05-08 11:11:33.000000 vayu_client-1.0.6/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3477 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/filter.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3114 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/get_contract_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4858 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/get_contract_response_schema_contract.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/get_customer_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3110 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/get_event_by_ref_id_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4861 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/get_event_by_ref_id_response_schema_event.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3093 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/get_invoice_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     6159 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/get_invoice_response_schema_invoice.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3515 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3051 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/get_meter_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4720 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/get_meter_response_schema_meter.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3030 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/get_plan_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4195 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/get_plan_response_schema_plan.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3737 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/list_contracts_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4766 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/list_contracts_response_schema_contracts_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3737 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/list_customers_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3785 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/list_customers_response_schema_customers_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3716 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/list_invoices_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     6067 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/list_invoices_response_schema_invoices_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3674 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/list_meters_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4628 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/list_meters_response_schema_meters_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3653 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/list_plans_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4103 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/list_plans_response_schema_plans_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/login_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2870 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/login_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/period.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3483 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/plan_billing_data.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1023 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/plan_status.py
--rw-r--r--   0 shaigross   (501) staff       (20)      947 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/plan_type.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3353 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/query_events_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4866 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/query_events_response_schema_events_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3235 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/send_events_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4230 2024-05-08 14:01:03.000000 vayu_client-1.0.6/openapi_client/models/send_events_request_schema_events_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4212 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/send_events_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3218 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/send_events_response_schema_invalid_events_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3108 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/update_customer_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/update_customer_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4011 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/update_meter_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3063 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/models/update_meter_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     9616 2024-05-09 12:38:25.000000 vayu_client-1.0.6/openapi_client/rest.py
--rw-r--r--   0 shaigross   (501) staff       (20)      420 2024-05-09 13:42:36.479779 vayu_client-1.0.6/setup.cfg
--rw-r--r--   0 shaigross   (501) staff       (20)      296 2024-01-24 16:49:22.000000 vayu_client-1.0.6/setup.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2208 2024-05-09 13:41:05.000000 vayu_client-1.0.6/vayu.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 13:42:36.479283 vayu_client-1.0.6/vayu_client.egg-info/
--rw-r--r--   0 shaigross   (501) staff       (20)     2539 2024-05-09 13:42:36.000000 vayu_client-1.0.6/vayu_client.egg-info/PKG-INFO
--rw-r--r--   0 shaigross   (501) staff       (20)     4400 2024-05-09 13:42:36.000000 vayu_client-1.0.6/vayu_client.egg-info/SOURCES.txt
--rw-r--r--   0 shaigross   (501) staff       (20)        1 2024-05-09 13:42:36.000000 vayu_client-1.0.6/vayu_client.egg-info/dependency_links.txt
--rw-r--r--   0 shaigross   (501) staff       (20)      102 2024-05-09 13:42:36.000000 vayu_client-1.0.6/vayu_client.egg-info/requires.txt
--rw-r--r--   0 shaigross   (501) staff       (20)       47 2024-05-09 13:42:36.000000 vayu_client-1.0.6/vayu_client.egg-info/top_level.txt
--rw-r--r--   0 shaigross   (501) staff       (20)       41 2024-05-09 13:41:17.000000 vayu_client-1.0.6/vayu_consts.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 13:53:14.578782 vayu_client-1.0.7/
+-rw-r--r--   0 shaigross   (501) staff       (20)     2539 2024-05-09 13:53:14.578863 vayu_client-1.0.7/PKG-INFO
+-rw-r--r--   0 shaigross   (501) staff       (20)      481 2024-05-08 15:19:35.000000 vayu_client-1.0.7/README.md
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 13:53:14.565917 vayu_client-1.0.7/entity_clients/
+-rw-r--r--   0 shaigross   (501) staff       (20)       46 2024-05-08 13:47:16.000000 vayu_client-1.0.7/entity_clients/__init__.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1178 2024-05-09 10:52:12.000000 vayu_client-1.0.7/entity_clients/contracts_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1295 2024-05-09 10:52:16.000000 vayu_client-1.0.7/entity_clients/customers_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1413 2024-05-08 14:59:08.000000 vayu_client-1.0.7/entity_clients/events_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      517 2024-05-09 10:52:12.000000 vayu_client-1.0.7/entity_clients/invoices_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1807 2024-05-09 10:52:12.000000 vayu_client-1.0.7/entity_clients/meters_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      561 2024-05-09 10:52:12.000000 vayu_client-1.0.7/entity_clients/plans_client.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 13:53:14.567078 vayu_client-1.0.7/openapi_client/
+-rw-r--r--   0 shaigross   (501) staff       (20)     6785 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/__init__.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 13:53:14.568470 vayu_client-1.0.7/openapi_client/api/
+-rw-r--r--   0 shaigross   (501) staff       (20)      422 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/api/__init__.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    12591 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/api/auth_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    43742 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/api/contracts_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    55565 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/api/customers_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    61236 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/api/events_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    22281 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/api/invoices_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    43924 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/api/meters_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    32198 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/api/plans_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    26550 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/api_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      652 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/api_response.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    15152 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/configuration.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     6180 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/exceptions.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 13:53:14.577867 vayu_client-1.0.7/openapi_client/models/
+-rw-r--r--   0 shaigross   (501) staff       (20)     5867 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/__init__.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3340 2024-05-09 13:52:51.000000 vayu_client-1.0.7/openapi_client/models/aggregation_method.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1161 2024-05-09 13:52:51.000000 vayu_client-1.0.7/openapi_client/models/aggregation_operator.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1052 2024-05-09 13:52:51.000000 vayu_client-1.0.7/openapi_client/models/billing_interval.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3214 2024-05-09 13:52:51.000000 vayu_client-1.0.7/openapi_client/models/condition.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4112 2024-05-09 13:52:51.000000 vayu_client-1.0.7/openapi_client/models/create_contract_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/create_contract_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3084 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/create_customer_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/create_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3765 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/create_customer_response_schema_customer.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3034 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/criterion.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1202 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/criterion_operator.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/delete_contract_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4870 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/delete_contract_response_schema_contract.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/delete_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3889 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/delete_customer_response_schema_customer.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3134 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/delete_event_by_ref_id_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4983 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/delete_event_by_ref_id_response_schema_event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3075 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/delete_meter_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4732 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/delete_meter_response_schema_meter.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3054 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/delete_plan_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4207 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/delete_plan_response_schema_plan.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4127 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3243 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/events_dry_run_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4380 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/events_dry_run_response_schema_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3921 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/events_dry_run_response_schema_inner_event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4556 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3461 2024-05-08 11:11:33.000000 vayu_client-1.0.7/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3477 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/filter.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3114 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/get_contract_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4734 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/get_contract_response_schema_contract.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/get_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3110 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/get_event_by_ref_id_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4861 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/get_event_by_ref_id_response_schema_event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3093 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/get_invoice_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     6035 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/get_invoice_response_schema_invoice.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3515 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3051 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/get_meter_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4596 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/get_meter_response_schema_meter.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3030 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/get_plan_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4071 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/get_plan_response_schema_plan.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3704 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/list_contracts_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4766 2024-05-09 12:38:25.000000 vayu_client-1.0.7/openapi_client/models/list_contracts_response_schema_contracts_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3716 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/list_customers_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3785 2024-05-09 12:38:25.000000 vayu_client-1.0.7/openapi_client/models/list_customers_response_schema_customers_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3683 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/list_invoices_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     6067 2024-05-09 12:38:25.000000 vayu_client-1.0.7/openapi_client/models/list_invoices_response_schema_invoices_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3641 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/list_meters_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4628 2024-05-09 12:38:25.000000 vayu_client-1.0.7/openapi_client/models/list_meters_response_schema_meters_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3620 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/list_plans_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4103 2024-05-09 12:38:25.000000 vayu_client-1.0.7/openapi_client/models/list_plans_response_schema_plans_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/login_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2870 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/login_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/period.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3483 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/plan_billing_data.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1023 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/plan_status.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      947 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/plan_type.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3353 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/query_events_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4866 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/query_events_response_schema_events_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3235 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/send_events_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4230 2024-05-08 14:01:03.000000 vayu_client-1.0.7/openapi_client/models/send_events_request_schema_events_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4212 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/send_events_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3218 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/send_events_response_schema_invalid_events_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3108 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/update_customer_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/update_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4011 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/update_meter_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3063 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/models/update_meter_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     9616 2024-05-09 13:52:52.000000 vayu_client-1.0.7/openapi_client/rest.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      420 2024-05-09 13:53:14.579114 vayu_client-1.0.7/setup.cfg
+-rw-r--r--   0 shaigross   (501) staff       (20)      296 2024-01-24 16:49:22.000000 vayu_client-1.0.7/setup.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2208 2024-05-09 13:41:05.000000 vayu_client-1.0.7/vayu.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 13:53:14.578668 vayu_client-1.0.7/vayu_client.egg-info/
+-rw-r--r--   0 shaigross   (501) staff       (20)     2539 2024-05-09 13:53:14.000000 vayu_client-1.0.7/vayu_client.egg-info/PKG-INFO
+-rw-r--r--   0 shaigross   (501) staff       (20)     4650 2024-05-09 13:53:14.000000 vayu_client-1.0.7/vayu_client.egg-info/SOURCES.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)        1 2024-05-09 13:53:14.000000 vayu_client-1.0.7/vayu_client.egg-info/dependency_links.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)      102 2024-05-09 13:53:14.000000 vayu_client-1.0.7/vayu_client.egg-info/requires.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)       47 2024-05-09 13:53:14.000000 vayu_client-1.0.7/vayu_client.egg-info/top_level.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)       41 2024-05-09 13:41:17.000000 vayu_client-1.0.7/vayu_consts.py
```

### Comparing `vayu_client-1.0.6/PKG-INFO` & `vayu_client-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vayu_client
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple and easy to use python package for utilizing vayu billing system
 Home-page: https://withvayu.com
 Author: Vayu, Inc.
 Author-email: team@withvayu.com
 Keywords: vayu,billing,events,python,sdk
 Requires-Python: ==3.7.*
 Description-Content-Type: text/markdown
```

### Comparing `vayu_client-1.0.6/entity_clients/contracts_client.py` & `vayu_client-1.0.7/entity_clients/contracts_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/entity_clients/customers_client.py` & `vayu_client-1.0.7/entity_clients/customers_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/entity_clients/events_client.py` & `vayu_client-1.0.7/entity_clients/events_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/entity_clients/invoices_client.py` & `vayu_client-1.0.7/entity_clients/invoices_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/entity_clients/meters_client.py` & `vayu_client-1.0.7/entity_clients/meters_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/entity_clients/plans_client.py` & `vayu_client-1.0.7/entity_clients/plans_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/__init__.py` & `vayu_client-1.0.7/openapi_client/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,19 +46,23 @@
 from openapi_client.models.create_contract_response_schema import CreateContractResponseSchema
 from openapi_client.models.create_customer_request_schema import CreateCustomerRequestSchema
 from openapi_client.models.create_customer_response_schema import CreateCustomerResponseSchema
 from openapi_client.models.create_customer_response_schema_customer import CreateCustomerResponseSchemaCustomer
 from openapi_client.models.criterion import Criterion
 from openapi_client.models.criterion_operator import CriterionOperator
 from openapi_client.models.delete_contract_response_schema import DeleteContractResponseSchema
+from openapi_client.models.delete_contract_response_schema_contract import DeleteContractResponseSchemaContract
 from openapi_client.models.delete_customer_response_schema import DeleteCustomerResponseSchema
+from openapi_client.models.delete_customer_response_schema_customer import DeleteCustomerResponseSchemaCustomer
 from openapi_client.models.delete_event_by_ref_id_response_schema import DeleteEventByRefIdResponseSchema
 from openapi_client.models.delete_event_by_ref_id_response_schema_event import DeleteEventByRefIdResponseSchemaEvent
 from openapi_client.models.delete_meter_response_schema import DeleteMeterResponseSchema
+from openapi_client.models.delete_meter_response_schema_meter import DeleteMeterResponseSchemaMeter
 from openapi_client.models.delete_plan_response_schema import DeletePlanResponseSchema
+from openapi_client.models.delete_plan_response_schema_plan import DeletePlanResponseSchemaPlan
 from openapi_client.models.event import Event
 from openapi_client.models.events_dry_run_request_schema import EventsDryRunRequestSchema
 from openapi_client.models.events_dry_run_response_schema_inner import EventsDryRunResponseSchemaInner
 from openapi_client.models.events_dry_run_response_schema_inner_event import EventsDryRunResponseSchemaInnerEvent
 from openapi_client.models.events_dry_run_response_schema_inner_meter_with_values_inner import EventsDryRunResponseSchemaInnerMeterWithValuesInner
 from openapi_client.models.filter import Filter
 from openapi_client.models.get_contract_response_schema import GetContractResponseSchema
@@ -70,23 +74,18 @@
 from openapi_client.models.get_invoice_response_schema_invoice import GetInvoiceResponseSchemaInvoice
 from openapi_client.models.get_invoice_response_schema_invoice_line_items_inner import GetInvoiceResponseSchemaInvoiceLineItemsInner
 from openapi_client.models.get_meter_response_schema import GetMeterResponseSchema
 from openapi_client.models.get_meter_response_schema_meter import GetMeterResponseSchemaMeter
 from openapi_client.models.get_plan_response_schema import GetPlanResponseSchema
 from openapi_client.models.get_plan_response_schema_plan import GetPlanResponseSchemaPlan
 from openapi_client.models.list_contracts_response_schema import ListContractsResponseSchema
-from openapi_client.models.list_contracts_response_schema_contracts_inner import ListContractsResponseSchemaContractsInner
 from openapi_client.models.list_customers_response_schema import ListCustomersResponseSchema
-from openapi_client.models.list_customers_response_schema_customers_inner import ListCustomersResponseSchemaCustomersInner
 from openapi_client.models.list_invoices_response_schema import ListInvoicesResponseSchema
-from openapi_client.models.list_invoices_response_schema_invoices_inner import ListInvoicesResponseSchemaInvoicesInner
 from openapi_client.models.list_meters_response_schema import ListMetersResponseSchema
-from openapi_client.models.list_meters_response_schema_meters_inner import ListMetersResponseSchemaMetersInner
 from openapi_client.models.list_plans_response_schema import ListPlansResponseSchema
-from openapi_client.models.list_plans_response_schema_plans_inner import ListPlansResponseSchemaPlansInner
 from openapi_client.models.login_request_schema import LoginRequestSchema
 from openapi_client.models.login_response_schema import LoginResponseSchema
 from openapi_client.models.period import Period
 from openapi_client.models.plan_billing_data import PlanBillingData
 from openapi_client.models.plan_status import PlanStatus
 from openapi_client.models.plan_type import PlanType
 from openapi_client.models.query_events_response_schema import QueryEventsResponseSchema
```

### Comparing `vayu_client-1.0.6/openapi_client/api/auth_api.py` & `vayu_client-1.0.7/openapi_client/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/api/contracts_api.py` & `vayu_client-1.0.7/openapi_client/api/contracts_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/api/customers_api.py` & `vayu_client-1.0.7/openapi_client/api/customers_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/api/events_api.py` & `vayu_client-1.0.7/openapi_client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/api/invoices_api.py` & `vayu_client-1.0.7/openapi_client/api/invoices_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/api/meters_api.py` & `vayu_client-1.0.7/openapi_client/api/meters_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/api/plans_api.py` & `vayu_client-1.0.7/openapi_client/api/plans_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/api_client.py` & `vayu_client-1.0.7/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/api_response.py` & `vayu_client-1.0.7/openapi_client/api_response.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/configuration.py` & `vayu_client-1.0.7/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/exceptions.py` & `vayu_client-1.0.7/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/__init__.py` & `vayu_client-1.0.7/openapi_client/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,19 +23,23 @@
 from openapi_client.models.create_contract_response_schema import CreateContractResponseSchema
 from openapi_client.models.create_customer_request_schema import CreateCustomerRequestSchema
 from openapi_client.models.create_customer_response_schema import CreateCustomerResponseSchema
 from openapi_client.models.create_customer_response_schema_customer import CreateCustomerResponseSchemaCustomer
 from openapi_client.models.criterion import Criterion
 from openapi_client.models.criterion_operator import CriterionOperator
 from openapi_client.models.delete_contract_response_schema import DeleteContractResponseSchema
+from openapi_client.models.delete_contract_response_schema_contract import DeleteContractResponseSchemaContract
 from openapi_client.models.delete_customer_response_schema import DeleteCustomerResponseSchema
+from openapi_client.models.delete_customer_response_schema_customer import DeleteCustomerResponseSchemaCustomer
 from openapi_client.models.delete_event_by_ref_id_response_schema import DeleteEventByRefIdResponseSchema
 from openapi_client.models.delete_event_by_ref_id_response_schema_event import DeleteEventByRefIdResponseSchemaEvent
 from openapi_client.models.delete_meter_response_schema import DeleteMeterResponseSchema
+from openapi_client.models.delete_meter_response_schema_meter import DeleteMeterResponseSchemaMeter
 from openapi_client.models.delete_plan_response_schema import DeletePlanResponseSchema
+from openapi_client.models.delete_plan_response_schema_plan import DeletePlanResponseSchemaPlan
 from openapi_client.models.event import Event
 from openapi_client.models.events_dry_run_request_schema import EventsDryRunRequestSchema
 from openapi_client.models.events_dry_run_response_schema_inner import EventsDryRunResponseSchemaInner
 from openapi_client.models.events_dry_run_response_schema_inner_event import EventsDryRunResponseSchemaInnerEvent
 from openapi_client.models.events_dry_run_response_schema_inner_meter_with_values_inner import EventsDryRunResponseSchemaInnerMeterWithValuesInner
 from openapi_client.models.filter import Filter
 from openapi_client.models.get_contract_response_schema import GetContractResponseSchema
@@ -47,23 +51,18 @@
 from openapi_client.models.get_invoice_response_schema_invoice import GetInvoiceResponseSchemaInvoice
 from openapi_client.models.get_invoice_response_schema_invoice_line_items_inner import GetInvoiceResponseSchemaInvoiceLineItemsInner
 from openapi_client.models.get_meter_response_schema import GetMeterResponseSchema
 from openapi_client.models.get_meter_response_schema_meter import GetMeterResponseSchemaMeter
 from openapi_client.models.get_plan_response_schema import GetPlanResponseSchema
 from openapi_client.models.get_plan_response_schema_plan import GetPlanResponseSchemaPlan
 from openapi_client.models.list_contracts_response_schema import ListContractsResponseSchema
-from openapi_client.models.list_contracts_response_schema_contracts_inner import ListContractsResponseSchemaContractsInner
 from openapi_client.models.list_customers_response_schema import ListCustomersResponseSchema
-from openapi_client.models.list_customers_response_schema_customers_inner import ListCustomersResponseSchemaCustomersInner
 from openapi_client.models.list_invoices_response_schema import ListInvoicesResponseSchema
-from openapi_client.models.list_invoices_response_schema_invoices_inner import ListInvoicesResponseSchemaInvoicesInner
 from openapi_client.models.list_meters_response_schema import ListMetersResponseSchema
-from openapi_client.models.list_meters_response_schema_meters_inner import ListMetersResponseSchemaMetersInner
 from openapi_client.models.list_plans_response_schema import ListPlansResponseSchema
-from openapi_client.models.list_plans_response_schema_plans_inner import ListPlansResponseSchemaPlansInner
 from openapi_client.models.login_request_schema import LoginRequestSchema
 from openapi_client.models.login_response_schema import LoginResponseSchema
 from openapi_client.models.period import Period
 from openapi_client.models.plan_billing_data import PlanBillingData
 from openapi_client.models.plan_status import PlanStatus
 from openapi_client.models.plan_type import PlanType
 from openapi_client.models.query_events_response_schema import QueryEventsResponseSchema
```

### Comparing `vayu_client-1.0.6/openapi_client/models/aggregation_method.py` & `vayu_client-1.0.7/openapi_client/models/aggregation_method.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/aggregation_operator.py` & `vayu_client-1.0.7/openapi_client/models/aggregation_operator.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/billing_interval.py` & `vayu_client-1.0.7/openapi_client/models/billing_interval.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/condition.py` & `vayu_client-1.0.7/openapi_client/models/condition.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/create_contract_request_schema.py` & `vayu_client-1.0.7/openapi_client/models/create_contract_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/create_contract_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/create_contract_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/create_customer_request_schema.py` & `vayu_client-1.0.7/openapi_client/models/create_customer_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/create_customer_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/create_customer_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/create_customer_response_schema_customer.py` & `vayu_client-1.0.7/openapi_client/models/delete_customer_response_schema_customer.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 from datetime import datetime
 from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateCustomerResponseSchemaCustomer(BaseModel):
+class DeleteCustomerResponseSchemaCustomer(BaseModel):
     """
-    CreateCustomerResponseSchemaCustomer
+    DeleteCustomerResponseSchemaCustomer
     """ # noqa: E501
     name: Annotated[str, Field(min_length=1, strict=True)] = Field(description="The name of the customer")
     alias: Optional[Annotated[str, Field(min_length=1, strict=True)]] = Field(default=None, description="The alias of the customer used to match events to the customer.")
     id: Annotated[str, Field(strict=True)]
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
     deleted_at: StrictStr = Field(alias="deletedAt")
@@ -58,15 +58,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateCustomerResponseSchemaCustomer from a JSON string"""
+        """Create an instance of DeleteCustomerResponseSchemaCustomer from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -83,15 +83,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateCustomerResponseSchemaCustomer from a dict"""
+        """Create an instance of DeleteCustomerResponseSchemaCustomer from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `vayu_client-1.0.6/openapi_client/models/criterion.py` & `vayu_client-1.0.7/openapi_client/models/criterion.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/criterion_operator.py` & `vayu_client-1.0.7/openapi_client/models/criterion_operator.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/delete_contract_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/delete_contract_response_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from openapi_client.models.get_contract_response_schema_contract import GetContractResponseSchemaContract
+from openapi_client.models.delete_contract_response_schema_contract import DeleteContractResponseSchemaContract
 from typing import Optional, Set
 from typing_extensions import Self
 
 class DeleteContractResponseSchema(BaseModel):
     """
     DeleteContractResponseSchema
     """ # noqa: E501
-    contract: GetContractResponseSchemaContract
+    contract: DeleteContractResponseSchemaContract
     __properties: ClassVar[List[str]] = ["contract"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -81,12 +81,12 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "contract": GetContractResponseSchemaContract.from_dict(obj["contract"]) if obj.get("contract") is not None else None
+            "contract": DeleteContractResponseSchemaContract.from_dict(obj["contract"]) if obj.get("contract") is not None else None
         })
         return _obj
```

### Comparing `vayu_client-1.0.6/openapi_client/models/delete_customer_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/get_customer_response_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
 from openapi_client.models.create_customer_response_schema_customer import CreateCustomerResponseSchemaCustomer
 from typing import Optional, Set
 from typing_extensions import Self
 
-class DeleteCustomerResponseSchema(BaseModel):
+class GetCustomerResponseSchema(BaseModel):
     """
-    DeleteCustomerResponseSchema
+    GetCustomerResponseSchema
     """ # noqa: E501
     customer: CreateCustomerResponseSchemaCustomer
     __properties: ClassVar[List[str]] = ["customer"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of DeleteCustomerResponseSchema from a JSON string"""
+        """Create an instance of GetCustomerResponseSchema from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -73,15 +73,15 @@
         # override the default output from pydantic by calling `to_dict()` of customer
         if self.customer:
             _dict['customer'] = self.customer.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of DeleteCustomerResponseSchema from a dict"""
+        """Create an instance of GetCustomerResponseSchema from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `vayu_client-1.0.6/openapi_client/models/delete_event_by_ref_id_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/delete_event_by_ref_id_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/delete_event_by_ref_id_response_schema_event.py` & `vayu_client-1.0.7/openapi_client/models/delete_event_by_ref_id_response_schema_event.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/delete_meter_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/delete_meter_response_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from openapi_client.models.get_meter_response_schema_meter import GetMeterResponseSchemaMeter
+from openapi_client.models.delete_meter_response_schema_meter import DeleteMeterResponseSchemaMeter
 from typing import Optional, Set
 from typing_extensions import Self
 
 class DeleteMeterResponseSchema(BaseModel):
     """
     DeleteMeterResponseSchema
     """ # noqa: E501
-    meter: GetMeterResponseSchemaMeter
+    meter: DeleteMeterResponseSchemaMeter
     __properties: ClassVar[List[str]] = ["meter"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -81,12 +81,12 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "meter": GetMeterResponseSchemaMeter.from_dict(obj["meter"]) if obj.get("meter") is not None else None
+            "meter": DeleteMeterResponseSchemaMeter.from_dict(obj["meter"]) if obj.get("meter") is not None else None
         })
         return _obj
```

### Comparing `vayu_client-1.0.6/openapi_client/models/delete_plan_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/delete_plan_response_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from openapi_client.models.get_plan_response_schema_plan import GetPlanResponseSchemaPlan
+from openapi_client.models.delete_plan_response_schema_plan import DeletePlanResponseSchemaPlan
 from typing import Optional, Set
 from typing_extensions import Self
 
 class DeletePlanResponseSchema(BaseModel):
     """
     DeletePlanResponseSchema
     """ # noqa: E501
-    plan: GetPlanResponseSchemaPlan
+    plan: DeletePlanResponseSchemaPlan
     __properties: ClassVar[List[str]] = ["plan"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -81,12 +81,12 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "plan": GetPlanResponseSchemaPlan.from_dict(obj["plan"]) if obj.get("plan") is not None else None
+            "plan": DeletePlanResponseSchemaPlan.from_dict(obj["plan"]) if obj.get("plan") is not None else None
         })
         return _obj
```

### Comparing `vayu_client-1.0.6/openapi_client/models/event.py` & `vayu_client-1.0.7/openapi_client/models/event.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/events_dry_run_request_schema.py` & `vayu_client-1.0.7/openapi_client/models/events_dry_run_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/events_dry_run_response_schema_inner.py` & `vayu_client-1.0.7/openapi_client/models/events_dry_run_response_schema_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/events_dry_run_response_schema_inner_event.py` & `vayu_client-1.0.7/openapi_client/models/events_dry_run_response_schema_inner_event.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py` & `vayu_client-1.0.7/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py` & `vayu_client-1.0.7/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/filter.py` & `vayu_client-1.0.7/openapi_client/models/filter.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/get_contract_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/get_contract_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/get_contract_response_schema_contract.py` & `vayu_client-1.0.7/openapi_client/models/get_contract_response_schema_contract.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
 class GetContractResponseSchemaContract(BaseModel):
     """
@@ -32,16 +32,15 @@
     start_date: datetime = Field(description="The start date of the contract", alias="startDate")
     end_date: Optional[datetime] = Field(default=None, description="The end date of the contract", alias="endDate")
     customer_id: Annotated[str, Field(strict=True)] = Field(description="The id of the customer that the contract is associated with", alias="customerId")
     plan_id: Annotated[str, Field(strict=True)] = Field(description="The id of the plan that the contract is associated with", alias="planId")
     id: Annotated[str, Field(strict=True)]
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
-    deleted_at: StrictStr = Field(alias="deletedAt")
-    __properties: ClassVar[List[str]] = ["startDate", "endDate", "customerId", "planId", "id", "createdAt", "updatedAt", "deletedAt"]
+    __properties: ClassVar[List[str]] = ["startDate", "endDate", "customerId", "planId", "id", "createdAt", "updatedAt"]
 
     @field_validator('customer_id')
     def customer_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if not re.match(r"^[0-9a-fA-F]{24}$", value):
             raise ValueError(r"must validate the regular expression /^[0-9a-fA-F]{24}$/")
         return value
@@ -113,13 +112,12 @@
         _obj = cls.model_validate({
             "startDate": obj.get("startDate"),
             "endDate": obj.get("endDate"),
             "customerId": obj.get("customerId"),
             "planId": obj.get("planId"),
             "id": obj.get("id"),
             "createdAt": obj.get("createdAt"),
-            "updatedAt": obj.get("updatedAt"),
-            "deletedAt": obj.get("deletedAt")
+            "updatedAt": obj.get("updatedAt")
         })
         return _obj
```

### Comparing `vayu_client-1.0.6/openapi_client/models/get_customer_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/delete_customer_response_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from openapi_client.models.create_customer_response_schema_customer import CreateCustomerResponseSchemaCustomer
+from openapi_client.models.delete_customer_response_schema_customer import DeleteCustomerResponseSchemaCustomer
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GetCustomerResponseSchema(BaseModel):
+class DeleteCustomerResponseSchema(BaseModel):
     """
-    GetCustomerResponseSchema
+    DeleteCustomerResponseSchema
     """ # noqa: E501
-    customer: CreateCustomerResponseSchemaCustomer
+    customer: DeleteCustomerResponseSchemaCustomer
     __properties: ClassVar[List[str]] = ["customer"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -45,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GetCustomerResponseSchema from a JSON string"""
+        """Create an instance of DeleteCustomerResponseSchema from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -73,20 +73,20 @@
         # override the default output from pydantic by calling `to_dict()` of customer
         if self.customer:
             _dict['customer'] = self.customer.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GetCustomerResponseSchema from a dict"""
+        """Create an instance of DeleteCustomerResponseSchema from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "customer": CreateCustomerResponseSchemaCustomer.from_dict(obj["customer"]) if obj.get("customer") is not None else None
+            "customer": DeleteCustomerResponseSchemaCustomer.from_dict(obj["customer"]) if obj.get("customer") is not None else None
         })
         return _obj
```

### Comparing `vayu_client-1.0.6/openapi_client/models/get_event_by_ref_id_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/get_event_by_ref_id_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/get_event_by_ref_id_response_schema_event.py` & `vayu_client-1.0.7/openapi_client/models/get_event_by_ref_id_response_schema_event.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/get_invoice_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/get_invoice_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/get_invoice_response_schema_invoice.py` & `vayu_client-1.0.7/openapi_client/models/get_invoice_response_schema_invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, field_validator
 from typing import Any, ClassVar, Dict, List, Optional, Union
 from typing_extensions import Annotated
 from openapi_client.models.get_invoice_response_schema_invoice_line_items_inner import GetInvoiceResponseSchemaInvoiceLineItemsInner
 from openapi_client.models.period import Period
 from typing import Optional, Set
 from typing_extensions import Self
 
@@ -36,16 +36,15 @@
     amount: Union[StrictFloat, StrictInt] = Field(description="The amount to be charged in the invoice")
     name: Annotated[str, Field(min_length=1, strict=True)] = Field(description="The name of the invoice, usually a description of the billing period")
     billing_cycle: Period = Field(alias="billingCycle")
     line_items: List[GetInvoiceResponseSchemaInvoiceLineItemsInner] = Field(alias="lineItems")
     id: Annotated[str, Field(strict=True)]
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
-    deleted_at: StrictStr = Field(alias="deletedAt")
-    __properties: ClassVar[List[str]] = ["customerId", "contractId", "amount", "name", "billingCycle", "lineItems", "id", "createdAt", "updatedAt", "deletedAt"]
+    __properties: ClassVar[List[str]] = ["customerId", "contractId", "amount", "name", "billingCycle", "lineItems", "id", "createdAt", "updatedAt"]
 
     @field_validator('customer_id')
     def customer_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if not re.match(r"^[0-9a-fA-F]{24}$", value):
             raise ValueError(r"must validate the regular expression /^[0-9a-fA-F]{24}$/")
         return value
@@ -132,13 +131,12 @@
             "contractId": obj.get("contractId"),
             "amount": obj.get("amount"),
             "name": obj.get("name"),
             "billingCycle": Period.from_dict(obj["billingCycle"]) if obj.get("billingCycle") is not None else None,
             "lineItems": [GetInvoiceResponseSchemaInvoiceLineItemsInner.from_dict(_item) for _item in obj["lineItems"]] if obj.get("lineItems") is not None else None,
             "id": obj.get("id"),
             "createdAt": obj.get("createdAt"),
-            "updatedAt": obj.get("updatedAt"),
-            "deletedAt": obj.get("deletedAt")
+            "updatedAt": obj.get("updatedAt")
         })
         return _obj
```

### Comparing `vayu_client-1.0.6/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py` & `vayu_client-1.0.7/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/get_meter_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/get_meter_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/get_meter_response_schema_meter.py` & `vayu_client-1.0.7/openapi_client/models/delete_meter_response_schema_meter.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from openapi_client.models.aggregation_method import AggregationMethod
 from openapi_client.models.filter import Filter
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GetMeterResponseSchemaMeter(BaseModel):
+class DeleteMeterResponseSchemaMeter(BaseModel):
     """
-    GetMeterResponseSchemaMeter
+    DeleteMeterResponseSchemaMeter
     """ # noqa: E501
     name: Annotated[str, Field(min_length=1, strict=True)] = Field(description="The name of the meter")
     event_name: Annotated[str, Field(min_length=1, strict=True)] = Field(description="The name of the event that the meter is tracking.", alias="eventName")
     aggregation_method: AggregationMethod = Field(alias="aggregationMethod")
     filter: Optional[Filter] = None
     id: Annotated[str, Field(strict=True)]
     created_at: datetime = Field(alias="createdAt")
@@ -62,15 +62,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GetMeterResponseSchemaMeter from a JSON string"""
+        """Create an instance of DeleteMeterResponseSchemaMeter from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -93,15 +93,15 @@
         # override the default output from pydantic by calling `to_dict()` of filter
         if self.filter:
             _dict['filter'] = self.filter.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GetMeterResponseSchemaMeter from a dict"""
+        """Create an instance of DeleteMeterResponseSchemaMeter from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `vayu_client-1.0.6/openapi_client/models/get_plan_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/get_plan_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/get_plan_response_schema_plan.py` & `vayu_client-1.0.7/openapi_client/models/get_plan_response_schema_plan.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, field_validator
 from typing import Any, ClassVar, Dict, List
 from typing_extensions import Annotated
 from openapi_client.models.plan_billing_data import PlanBillingData
 from openapi_client.models.plan_status import PlanStatus
 from typing import Optional, Set
 from typing_extensions import Self
 
@@ -33,16 +33,15 @@
     """ # noqa: E501
     name: Annotated[str, Field(min_length=1, strict=True)] = Field(description="The name of the plan")
     status: PlanStatus
     billing_data: PlanBillingData = Field(alias="billingData")
     id: Annotated[str, Field(strict=True)]
     created_at: datetime = Field(alias="createdAt")
     updated_at: datetime = Field(alias="updatedAt")
-    deleted_at: StrictStr = Field(alias="deletedAt")
-    __properties: ClassVar[List[str]] = ["name", "status", "billingData", "id", "createdAt", "updatedAt", "deletedAt"]
+    __properties: ClassVar[List[str]] = ["name", "status", "billingData", "id", "createdAt", "updatedAt"]
 
     @field_validator('id')
     def id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if not re.match(r"^[0-9a-fA-F]{24}$", value):
             raise ValueError(r"must validate the regular expression /^[0-9a-fA-F]{24}$/")
         return value
@@ -102,13 +101,12 @@
 
         _obj = cls.model_validate({
             "name": obj.get("name"),
             "status": obj.get("status"),
             "billingData": PlanBillingData.from_dict(obj["billingData"]) if obj.get("billingData") is not None else None,
             "id": obj.get("id"),
             "createdAt": obj.get("createdAt"),
-            "updatedAt": obj.get("updatedAt"),
-            "deletedAt": obj.get("deletedAt")
+            "updatedAt": obj.get("updatedAt")
         })
         return _obj
```

### Comparing `vayu_client-1.0.6/openapi_client/models/list_contracts_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/list_contracts_response_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from openapi_client.models.list_contracts_response_schema_contracts_inner import ListContractsResponseSchemaContractsInner
+from openapi_client.models.get_contract_response_schema_contract import GetContractResponseSchemaContract
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ListContractsResponseSchema(BaseModel):
     """
     ListContractsResponseSchema
     """ # noqa: E501
-    contracts: List[ListContractsResponseSchemaContractsInner]
+    contracts: List[GetContractResponseSchemaContract]
     total: Union[StrictFloat, StrictInt]
     has_more: StrictBool = Field(alias="hasMore")
     next_cursor: Optional[StrictStr] = Field(default=None, alias="nextCursor")
     __properties: ClassVar[List[str]] = ["contracts", "total", "hasMore", "nextCursor"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -88,15 +88,15 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "contracts": [ListContractsResponseSchemaContractsInner.from_dict(_item) for _item in obj["contracts"]] if obj.get("contracts") is not None else None,
+            "contracts": [GetContractResponseSchemaContract.from_dict(_item) for _item in obj["contracts"]] if obj.get("contracts") is not None else None,
             "total": obj.get("total"),
             "hasMore": obj.get("hasMore"),
             "nextCursor": obj.get("nextCursor")
         })
         return _obj
```

### Comparing `vayu_client-1.0.6/openapi_client/models/list_contracts_response_schema_contracts_inner.py` & `vayu_client-1.0.7/openapi_client/models/list_contracts_response_schema_contracts_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/list_customers_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/list_customers_response_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from openapi_client.models.list_customers_response_schema_customers_inner import ListCustomersResponseSchemaCustomersInner
+from openapi_client.models.create_customer_response_schema_customer import CreateCustomerResponseSchemaCustomer
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ListCustomersResponseSchema(BaseModel):
     """
     ListCustomersResponseSchema
     """ # noqa: E501
-    customers: List[ListCustomersResponseSchemaCustomersInner]
+    customers: List[CreateCustomerResponseSchemaCustomer]
     total: Union[StrictFloat, StrictInt]
     has_more: StrictBool = Field(alias="hasMore")
     next_cursor: Optional[StrictStr] = Field(default=None, alias="nextCursor")
     __properties: ClassVar[List[str]] = ["customers", "total", "hasMore", "nextCursor"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -88,15 +88,15 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "customers": [ListCustomersResponseSchemaCustomersInner.from_dict(_item) for _item in obj["customers"]] if obj.get("customers") is not None else None,
+            "customers": [CreateCustomerResponseSchemaCustomer.from_dict(_item) for _item in obj["customers"]] if obj.get("customers") is not None else None,
             "total": obj.get("total"),
             "hasMore": obj.get("hasMore"),
             "nextCursor": obj.get("nextCursor")
         })
         return _obj
```

### Comparing `vayu_client-1.0.6/openapi_client/models/list_customers_response_schema_customers_inner.py` & `vayu_client-1.0.7/openapi_client/models/list_customers_response_schema_customers_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/list_invoices_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/list_invoices_response_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from openapi_client.models.list_invoices_response_schema_invoices_inner import ListInvoicesResponseSchemaInvoicesInner
+from openapi_client.models.get_invoice_response_schema_invoice import GetInvoiceResponseSchemaInvoice
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ListInvoicesResponseSchema(BaseModel):
     """
     ListInvoicesResponseSchema
     """ # noqa: E501
-    invoices: List[ListInvoicesResponseSchemaInvoicesInner]
+    invoices: List[GetInvoiceResponseSchemaInvoice]
     total: Union[StrictFloat, StrictInt]
     has_more: StrictBool = Field(alias="hasMore")
     next_cursor: Optional[StrictStr] = Field(default=None, alias="nextCursor")
     __properties: ClassVar[List[str]] = ["invoices", "total", "hasMore", "nextCursor"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -88,15 +88,15 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "invoices": [ListInvoicesResponseSchemaInvoicesInner.from_dict(_item) for _item in obj["invoices"]] if obj.get("invoices") is not None else None,
+            "invoices": [GetInvoiceResponseSchemaInvoice.from_dict(_item) for _item in obj["invoices"]] if obj.get("invoices") is not None else None,
             "total": obj.get("total"),
             "hasMore": obj.get("hasMore"),
             "nextCursor": obj.get("nextCursor")
         })
         return _obj
```

### Comparing `vayu_client-1.0.6/openapi_client/models/list_invoices_response_schema_invoices_inner.py` & `vayu_client-1.0.7/openapi_client/models/list_invoices_response_schema_invoices_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/list_meters_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/list_meters_response_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from openapi_client.models.list_meters_response_schema_meters_inner import ListMetersResponseSchemaMetersInner
+from openapi_client.models.get_meter_response_schema_meter import GetMeterResponseSchemaMeter
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ListMetersResponseSchema(BaseModel):
     """
     ListMetersResponseSchema
     """ # noqa: E501
-    meters: List[ListMetersResponseSchemaMetersInner]
+    meters: List[GetMeterResponseSchemaMeter]
     total: Union[StrictFloat, StrictInt]
     has_more: StrictBool = Field(alias="hasMore")
     next_cursor: Optional[StrictStr] = Field(default=None, alias="nextCursor")
     __properties: ClassVar[List[str]] = ["meters", "total", "hasMore", "nextCursor"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -88,15 +88,15 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "meters": [ListMetersResponseSchemaMetersInner.from_dict(_item) for _item in obj["meters"]] if obj.get("meters") is not None else None,
+            "meters": [GetMeterResponseSchemaMeter.from_dict(_item) for _item in obj["meters"]] if obj.get("meters") is not None else None,
             "total": obj.get("total"),
             "hasMore": obj.get("hasMore"),
             "nextCursor": obj.get("nextCursor")
         })
         return _obj
```

### Comparing `vayu_client-1.0.6/openapi_client/models/list_meters_response_schema_meters_inner.py` & `vayu_client-1.0.7/openapi_client/models/list_meters_response_schema_meters_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/list_plans_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/list_plans_response_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from openapi_client.models.list_plans_response_schema_plans_inner import ListPlansResponseSchemaPlansInner
+from openapi_client.models.get_plan_response_schema_plan import GetPlanResponseSchemaPlan
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ListPlansResponseSchema(BaseModel):
     """
     ListPlansResponseSchema
     """ # noqa: E501
-    plans: List[ListPlansResponseSchemaPlansInner]
+    plans: List[GetPlanResponseSchemaPlan]
     total: Union[StrictFloat, StrictInt]
     has_more: StrictBool = Field(alias="hasMore")
     next_cursor: Optional[StrictStr] = Field(default=None, alias="nextCursor")
     __properties: ClassVar[List[str]] = ["plans", "total", "hasMore", "nextCursor"]
 
     model_config = ConfigDict(
         populate_by_name=True,
@@ -88,15 +88,15 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "plans": [ListPlansResponseSchemaPlansInner.from_dict(_item) for _item in obj["plans"]] if obj.get("plans") is not None else None,
+            "plans": [GetPlanResponseSchemaPlan.from_dict(_item) for _item in obj["plans"]] if obj.get("plans") is not None else None,
             "total": obj.get("total"),
             "hasMore": obj.get("hasMore"),
             "nextCursor": obj.get("nextCursor")
         })
         return _obj
```

### Comparing `vayu_client-1.0.6/openapi_client/models/list_plans_response_schema_plans_inner.py` & `vayu_client-1.0.7/openapi_client/models/list_plans_response_schema_plans_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/login_request_schema.py` & `vayu_client-1.0.7/openapi_client/models/login_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/login_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/login_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/period.py` & `vayu_client-1.0.7/openapi_client/models/period.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/plan_billing_data.py` & `vayu_client-1.0.7/openapi_client/models/plan_billing_data.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/plan_status.py` & `vayu_client-1.0.7/openapi_client/models/plan_status.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/plan_type.py` & `vayu_client-1.0.7/openapi_client/models/plan_type.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/query_events_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/query_events_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/query_events_response_schema_events_inner.py` & `vayu_client-1.0.7/openapi_client/models/query_events_response_schema_events_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/send_events_request_schema.py` & `vayu_client-1.0.7/openapi_client/models/send_events_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/send_events_request_schema_events_inner.py` & `vayu_client-1.0.7/openapi_client/models/send_events_request_schema_events_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/send_events_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/send_events_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/send_events_response_schema_invalid_events_inner.py` & `vayu_client-1.0.7/openapi_client/models/send_events_response_schema_invalid_events_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/update_customer_request_schema.py` & `vayu_client-1.0.7/openapi_client/models/update_customer_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/update_customer_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/update_customer_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/update_meter_request_schema.py` & `vayu_client-1.0.7/openapi_client/models/update_meter_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/models/update_meter_response_schema.py` & `vayu_client-1.0.7/openapi_client/models/update_meter_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/openapi_client/rest.py` & `vayu_client-1.0.7/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/vayu.py` & `vayu_client-1.0.7/vayu.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.6/vayu_client.egg-info/PKG-INFO` & `vayu_client-1.0.7/vayu_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vayu-client
-Version: 1.0.6
+Version: 1.0.7
 Summary: Simple and easy to use python package for utilizing vayu billing system
 Home-page: https://withvayu.com
 Author: Vayu, Inc.
 Author-email: team@withvayu.com
 Keywords: vayu,billing,events,python,sdk
 Requires-Python: ==3.7.*
 Description-Content-Type: text/markdown
```

### Comparing `vayu_client-1.0.6/vayu_client.egg-info/SOURCES.txt` & `vayu_client-1.0.7/vayu_client.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -33,19 +33,23 @@
 openapi_client/models/create_contract_response_schema.py
 openapi_client/models/create_customer_request_schema.py
 openapi_client/models/create_customer_response_schema.py
 openapi_client/models/create_customer_response_schema_customer.py
 openapi_client/models/criterion.py
 openapi_client/models/criterion_operator.py
 openapi_client/models/delete_contract_response_schema.py
+openapi_client/models/delete_contract_response_schema_contract.py
 openapi_client/models/delete_customer_response_schema.py
+openapi_client/models/delete_customer_response_schema_customer.py
 openapi_client/models/delete_event_by_ref_id_response_schema.py
 openapi_client/models/delete_event_by_ref_id_response_schema_event.py
 openapi_client/models/delete_meter_response_schema.py
+openapi_client/models/delete_meter_response_schema_meter.py
 openapi_client/models/delete_plan_response_schema.py
+openapi_client/models/delete_plan_response_schema_plan.py
 openapi_client/models/event.py
 openapi_client/models/events_dry_run_request_schema.py
 openapi_client/models/events_dry_run_response_schema_inner.py
 openapi_client/models/events_dry_run_response_schema_inner_event.py
 openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py
 openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py
 openapi_client/models/filter.py
```

