# Comparing `tmp/levo-0.4.9.tar.gz` & `tmp/levo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "levo-0.4.9.tar", max compression
+gzip compressed data, was "levo-1.0.0.tar", last modified: Thu May  9 09:49:02 2024, max compression
```

## Comparing `levo-0.4.9.tar` & `levo-1.0.0.tar`

### file list

```diff
@@ -1,58 +1,14 @@
--rw-r--r--   0        0        0     1176 2022-02-07 21:44:17.163610 levo-0.4.9/pyproject.toml
--rw-r--r--   0        0        0       22 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/__init__.py
--rw-r--r--   0        0        0       61 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/__main__.py
--rw-r--r--   0        0        0        0 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/apitesting/__init__.py
--rw-r--r--   0        0        0    18672 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/apitesting/common_pb2.py
--rw-r--r--   0        0        0      158 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/apitesting/common_pb2_grpc.py
--rw-r--r--   0        0        0     4195 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/apitesting/levo_testplans_service_pb2.py
--rw-r--r--   0        0        0     3072 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/apitesting/levo_testplans_service_pb2_grpc.py
--rw-r--r--   0        0        0        0 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/apitesting/runs/__init__.py
--rw-r--r--   0        0        0    56648 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/apitesting/runs/api_test_runs_pb2.py
--rw-r--r--   0        0        0     4992 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/apitesting/runs/api_test_runs_pb2_grpc.py
--rw-r--r--   0        0        0     5163 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/callbacks.py
--rw-r--r--   0        0        0     4617 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/cli.py
--rw-r--r--   0        0        0        0 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/commands/__init__.py
--rw-r--r--   0        0        0     1348 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/commands/constants.py
--rw-r--r--   0        0        0    11432 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/commands/image.py
--rw-r--r--   0        0        0     9255 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/commands/test_plan.py
--rw-r--r--   0        0        0     1651 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/commands/testplan_callbacks.py
--rw-r--r--   0        0        0     2396 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/config.py
--rw-r--r--   0        0        0     2594 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/config_file.py
--rwxr-xr-x   0        0        0     3288 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/docker_api/docker_api.py
--rw-r--r--   0        0        0     3035 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/docker_utils.py
--rw-r--r--   0        0        0     2275 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/env_constants.py
--rw-r--r--   0        0        0      729 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/errors.py
--rw-r--r--   0        0        0     2692 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/events.py
--rw-r--r--   0        0        0       69 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/handlers/__init__.py
--rw-r--r--   0        0        0      255 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/handlers/base.py
--rw-r--r--   0        0        0      566 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/handlers/debug.py
--rw-r--r--   0        0        0     2895 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/logger.py
--rw-r--r--   0        0        0    11397 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/login.py
--rw-r--r--   0        0        0       39 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/__init__.py
--rw-r--r--   0        0        0    10926 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/__init__.py
--rw-r--r--   0        0        0     2353 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/context.py
--rw-r--r--   0        0        0     1982 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/event_handler.py
--rw-r--r--   0        0        0     1575 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/local.py
--rw-r--r--   0        0        0     1518 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/logging.py
--rw-r--r--   0        0        0      314 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/models.py
--rw-r--r--   0        0        0      537 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/modules/__init__.py
--rw-r--r--   0        0        0      218 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/modules/bespoke/__init__.py
--rw-r--r--   0        0        0      223 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/modules/schemathesis/__init__.py
--rw-r--r--   0        0        0     2435 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/modules/zaproxy/__init__.py
--rw-r--r--   0        0        0     5577 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/remote.py
--rw-r--r--   0        0        0        0 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/reporters/__init__.py
--rw-r--r--   0        0        0    12418 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/reporters/default.py
--rw-r--r--   0        0        0    16845 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/levo_plans/reporters/report_portal.py
--rw-r--r--   0        0        0     4341 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/schemathesis/__init__.py
--rw-r--r--   0        0        0     6895 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/schemathesis/adapter.py
--rw-r--r--   0        0        0     1946 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/schemathesis/config.py
--rw-r--r--   0        0        0     2277 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/schemathesis/context.py
--rw-r--r--   0        0        0     5458 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/schemathesis/models.py
--rw-r--r--   0        0        0      200 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/schemathesis/reporters/__init__.py
--rw-r--r--   0        0        0    20984 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/schemathesis/reporters/default.py
--rw-r--r--   0        0        0    18875 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/schemathesis/reporters/report_portal.py
--rw-r--r--   0        0        0     2375 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/schemathesis/reporters/short.py
--rw-r--r--   0        0        0     2966 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/runners/utils.py
--rw-r--r--   0        0        0     5028 2022-02-07 21:44:17.167610 levo-0.4.9/src/levocli/utils.py
--rw-r--r--   0        0        0     1986 2022-02-07 21:44:24.576034 levo-0.4.9/setup.py
--rw-r--r--   0        0        0     1426 2022-02-07 21:44:24.576391 levo-0.4.9/PKG-INFO
+drwxr-xr-x   0 ricekot   (1000) ricekot   (1000)        0 2024-05-09 09:49:02.562237 levo-1.0.0/
+-rw-r--r--   0 ricekot   (1000) ricekot   (1000)      425 2024-05-09 09:49:02.562237 levo-1.0.0/PKG-INFO
+-rw-r--r--   0 ricekot   (1000) ricekot   (1000)       88 2024-05-09 09:48:57.000000 levo-1.0.0/README.md
+-rw-r--r--   0 ricekot   (1000) ricekot   (1000)      470 2024-05-09 09:48:57.000000 levo-1.0.0/pyproject.toml
+-rw-r--r--   0 ricekot   (1000) ricekot   (1000)       38 2024-05-09 09:49:02.562237 levo-1.0.0/setup.cfg
+drwxr-xr-x   0 ricekot   (1000) ricekot   (1000)        0 2024-05-09 09:49:02.562237 levo-1.0.0/src/
+drwxr-xr-x   0 ricekot   (1000) ricekot   (1000)        0 2024-05-09 09:49:02.562237 levo-1.0.0/src/levo/
+-rw-r--r--   0 ricekot   (1000) ricekot   (1000)       62 2024-05-09 09:19:09.000000 levo-1.0.0/src/levo/config.py
+-rw-r--r--   0 ricekot   (1000) ricekot   (1000)      230 2024-05-09 09:24:38.000000 levo-1.0.0/src/levo/iam.py
+drwxr-xr-x   0 ricekot   (1000) ricekot   (1000)        0 2024-05-09 09:49:02.562237 levo-1.0.0/src/levo.egg-info/
+-rw-r--r--   0 ricekot   (1000) ricekot   (1000)      425 2024-05-09 09:49:02.000000 levo-1.0.0/src/levo.egg-info/PKG-INFO
+-rw-r--r--   0 ricekot   (1000) ricekot   (1000)      187 2024-05-09 09:49:02.000000 levo-1.0.0/src/levo.egg-info/SOURCES.txt
+-rw-r--r--   0 ricekot   (1000) ricekot   (1000)        1 2024-05-09 09:49:02.000000 levo-1.0.0/src/levo.egg-info/dependency_links.txt
+-rw-r--r--   0 ricekot   (1000) ricekot   (1000)        5 2024-05-09 09:49:02.000000 levo-1.0.0/src/levo.egg-info/top_level.txt
```

