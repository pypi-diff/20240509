# Comparing `tmp/spaceone-notification-2.0.dev8.tar.gz` & `tmp/spaceone-notification-2.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-notification-2.0.dev8.tar", last modified: Mon Dec 25 10:31:52 2023, max compression
+gzip compressed data, was "spaceone-notification-2.0.dev9.tar", last modified: Mon Dec 25 12:00:29 2023, max compression
```

## Comparing `spaceone-notification-2.0.dev8.tar` & `spaceone-notification-2.0.dev9.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.855021 spaceone-notification-2.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-25 10:31:52.855021 spaceone-notification-2.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-25 10:31:52.855021 spaceone-notification-2.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.843021 spaceone-notification-2.0.dev8/spaceone/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.843021 spaceone-notification-2.0.dev8/spaceone/notification/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.843021 spaceone-notification-2.0.dev8/spaceone/notification/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/conf/global_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/conf/protocol_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.843021 spaceone-notification-2.0.dev8/spaceone/notification/connector/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/connector/identity_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/connector/notification_plugin_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/connector/plugin_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/connector/repository_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/connector/secret_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.843021 spaceone-notification-2.0.dev8/spaceone/notification/error/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/error/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/error/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/error/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/error/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/error/quota.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.847021 spaceone-notification-2.0.dev8/spaceone/notification/info/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/info/common_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/info/notification_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/info/project_channel_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/info/protocol_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/info/user_channel_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.847021 spaceone-notification-2.0.dev8/spaceone/notification/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.847021 spaceone-notification-2.0.dev8/spaceone/notification/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/interface/grpc/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/interface/grpc/project_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/interface/grpc/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/interface/grpc/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.847021 spaceone-notification-2.0.dev8/spaceone/notification/interface/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/interface/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.847021 spaceone-notification-2.0.dev8/spaceone/notification/interface/task/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/interface/task/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/interface/task/v1/delete_old_notification_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.847021 spaceone-notification-2.0.dev8/spaceone/notification/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/lib/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/lib/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.847021 spaceone-notification-2.0.dev8/spaceone/notification/manager/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/manager/identity_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/manager/notification_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/manager/notification_usage_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/manager/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/manager/project_channel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/manager/protocol_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/manager/repository_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/manager/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/manager/user_channel_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/manager/user_secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.851021 spaceone-notification-2.0.dev8/spaceone/notification/model/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/model/notification_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/model/notification_usage_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/model/project_channel_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/model/protocol_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/model/schedule_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/model/user_channel_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.851021 spaceone-notification-2.0.dev8/spaceone/notification/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.851021 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.851021 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.851021 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.851021 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/interface/grpc/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/interface/grpc/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.851021 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/lib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.851021 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/model/notification_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/model/protocol_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/model/protocol_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.851021 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/service/notification_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/service/protocol_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.851021 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/skeleton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/skeleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/skeleton/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.855021 spaceone-notification-2.0.dev8/spaceone/notification/service/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24935 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/service/notification_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14159 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/service/project_channel_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15671 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/service/protocol_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    11864 2023-12-25 10:31:44.000000 spaceone-notification-2.0.dev8/spaceone/notification/service/user_channel_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 10:31:52.855021 spaceone-notification-2.0.dev8/spaceone_notification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-25 10:31:52.000000 spaceone-notification-2.0.dev8/spaceone_notification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2023-12-25 10:31:52.000000 spaceone-notification-2.0.dev8/spaceone_notification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 10:31:52.000000 spaceone-notification-2.0.dev8/spaceone_notification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 10:31:52.000000 spaceone-notification-2.0.dev8/spaceone_notification.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-25 10:31:52.000000 spaceone-notification-2.0.dev8/spaceone_notification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-25 10:31:52.000000 spaceone-notification-2.0.dev8/spaceone_notification.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.451179 spaceone-notification-2.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-25 12:00:29.451179 spaceone-notification-2.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-25 12:00:29.451179 spaceone-notification-2.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.439179 spaceone-notification-2.0.dev9/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.439179 spaceone-notification-2.0.dev9/spaceone/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.439179 spaceone-notification-2.0.dev9/spaceone/notification/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/conf/global_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/conf/protocol_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.439179 spaceone-notification-2.0.dev9/spaceone/notification/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/connector/identity_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/connector/notification_plugin_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/connector/plugin_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/connector/repository_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/connector/secret_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.443179 spaceone-notification-2.0.dev9/spaceone/notification/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/error/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/error/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/error/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/error/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/error/quota.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.443179 spaceone-notification-2.0.dev9/spaceone/notification/info/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/info/common_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/info/notification_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/info/project_channel_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/info/protocol_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/info/user_channel_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.443179 spaceone-notification-2.0.dev9/spaceone/notification/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.443179 spaceone-notification-2.0.dev9/spaceone/notification/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/interface/grpc/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/interface/grpc/project_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/interface/grpc/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/interface/grpc/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.443179 spaceone-notification-2.0.dev9/spaceone/notification/interface/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/interface/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.443179 spaceone-notification-2.0.dev9/spaceone/notification/interface/task/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/interface/task/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/interface/task/v1/delete_old_notification_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.443179 spaceone-notification-2.0.dev9/spaceone/notification/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/lib/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/lib/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.447179 spaceone-notification-2.0.dev9/spaceone/notification/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/manager/identity_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/manager/notification_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/manager/notification_usage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/manager/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/manager/project_channel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/manager/protocol_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/manager/repository_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/manager/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/manager/user_channel_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/manager/user_secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.447179 spaceone-notification-2.0.dev9/spaceone/notification/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/model/notification_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/model/notification_usage_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/model/project_channel_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/model/protocol_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/model/schedule_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/model/user_channel_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.447179 spaceone-notification-2.0.dev9/spaceone/notification/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.447179 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.447179 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.447179 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.447179 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/interface/grpc/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/interface/grpc/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.447179 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/lib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.447179 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/model/notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/model/protocol_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/model/protocol_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.451179 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/service/notification_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/service/protocol_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.451179 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/skeleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/skeleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/skeleton/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.451179 spaceone-notification-2.0.dev9/spaceone/notification/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24935 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/service/notification_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14159 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/service/project_channel_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15668 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/service/protocol_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11864 2023-12-25 12:00:20.000000 spaceone-notification-2.0.dev9/spaceone/notification/service/user_channel_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-25 12:00:29.451179 spaceone-notification-2.0.dev9/spaceone_notification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2023-12-25 12:00:28.000000 spaceone-notification-2.0.dev9/spaceone_notification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2023-12-25 12:00:29.000000 spaceone-notification-2.0.dev9/spaceone_notification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 12:00:28.000000 spaceone-notification-2.0.dev9/spaceone_notification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-25 12:00:28.000000 spaceone-notification-2.0.dev9/spaceone_notification.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-25 12:00:28.000000 spaceone-notification-2.0.dev9/spaceone_notification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-25 12:00:28.000000 spaceone-notification-2.0.dev9/spaceone_notification.egg-info/top_level.txt
```

### Comparing `spaceone-notification-2.0.dev8/setup.py` & `spaceone-notification-2.0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/conf/global_conf.py` & `spaceone-notification-2.0.dev9/spaceone/notification/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/connector/identity_connector.py` & `spaceone-notification-2.0.dev9/spaceone/notification/connector/identity_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/connector/notification_plugin_connector.py` & `spaceone-notification-2.0.dev9/spaceone/notification/connector/notification_plugin_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/connector/plugin_connector.py` & `spaceone-notification-2.0.dev9/spaceone/notification/connector/plugin_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/connector/repository_connector.py` & `spaceone-notification-2.0.dev9/spaceone/notification/connector/repository_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/connector/secret_connector.py` & `spaceone-notification-2.0.dev9/spaceone/notification/connector/secret_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/error/channel.py` & `spaceone-notification-2.0.dev9/spaceone/notification/error/channel.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/error/plugin.py` & `spaceone-notification-2.0.dev9/spaceone/notification/error/plugin.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/error/protocol.py` & `spaceone-notification-2.0.dev9/spaceone/notification/error/protocol.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/info/notification_info.py` & `spaceone-notification-2.0.dev9/spaceone/notification/info/notification_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/info/project_channel_info.py` & `spaceone-notification-2.0.dev9/spaceone/notification/info/project_channel_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/info/protocol_info.py` & `spaceone-notification-2.0.dev9/spaceone/notification/info/protocol_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/info/user_channel_info.py` & `spaceone-notification-2.0.dev9/spaceone/notification/info/user_channel_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/interface/grpc/notification.py` & `spaceone-notification-2.0.dev9/spaceone/notification/interface/grpc/notification.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/interface/grpc/project_channel.py` & `spaceone-notification-2.0.dev9/spaceone/notification/interface/grpc/project_channel.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/interface/grpc/protocol.py` & `spaceone-notification-2.0.dev9/spaceone/notification/interface/grpc/protocol.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/interface/grpc/user_channel.py` & `spaceone-notification-2.0.dev9/spaceone/notification/interface/grpc/user_channel.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/interface/task/v1/delete_old_notification_scheduler.py` & `spaceone-notification-2.0.dev9/spaceone/notification/interface/task/v1/delete_old_notification_scheduler.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/lib/schedule.py` & `spaceone-notification-2.0.dev9/spaceone/notification/lib/schedule.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/manager/__init__.py` & `spaceone-notification-2.0.dev9/spaceone/notification/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/manager/identity_manager.py` & `spaceone-notification-2.0.dev9/spaceone/notification/manager/identity_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/manager/notification_manager.py` & `spaceone-notification-2.0.dev9/spaceone/notification/manager/notification_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/manager/notification_usage_manager.py` & `spaceone-notification-2.0.dev9/spaceone/notification/manager/notification_usage_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/manager/plugin_manager.py` & `spaceone-notification-2.0.dev9/spaceone/notification/manager/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/manager/project_channel_manager.py` & `spaceone-notification-2.0.dev9/spaceone/notification/manager/project_channel_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/manager/protocol_manager.py` & `spaceone-notification-2.0.dev9/spaceone/notification/manager/protocol_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/manager/repository_manager.py` & `spaceone-notification-2.0.dev9/spaceone/notification/manager/repository_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/manager/secret_manager.py` & `spaceone-notification-2.0.dev9/spaceone/notification/manager/secret_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/manager/user_channel_manager.py` & `spaceone-notification-2.0.dev9/spaceone/notification/manager/user_channel_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/manager/user_secret_manager.py` & `spaceone-notification-2.0.dev9/spaceone/notification/manager/user_secret_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/model/notification_model.py` & `spaceone-notification-2.0.dev9/spaceone/notification/model/notification_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/model/notification_usage_model.py` & `spaceone-notification-2.0.dev9/spaceone/notification/model/notification_usage_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/model/project_channel_model.py` & `spaceone-notification-2.0.dev9/spaceone/notification/model/project_channel_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/model/protocol_model.py` & `spaceone-notification-2.0.dev9/spaceone/notification/model/protocol_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/model/user_channel_model.py` & `spaceone-notification-2.0.dev9/spaceone/notification/model/user_channel_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/interface/grpc/notification.py` & `spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/interface/grpc/notification.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/interface/grpc/protocol.py` & `spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/interface/grpc/protocol.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/lib/server.py` & `spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/lib/server.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/model/notification_request.py` & `spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/model/notification_request.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/model/protocol_response.py` & `spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/model/protocol_response.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/service/notification_service.py` & `spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/service/notification_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/service/protocol_service.py` & `spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/service/protocol_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/plugin/protocol/skeleton/main.py` & `spaceone-notification-2.0.dev9/spaceone/notification/plugin/protocol/skeleton/main.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/service/notification_service.py` & `spaceone-notification-2.0.dev9/spaceone/notification/service/notification_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/service/project_channel_service.py` & `spaceone-notification-2.0.dev9/spaceone/notification/service/project_channel_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/service/protocol_service.py` & `spaceone-notification-2.0.dev9/spaceone/notification/service/protocol_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             request_plugin.update({"version": version})
 
         if "secret_data" in plugin_info:
             secret_mgr: SecretManager = self.locator.get_manager("SecretManager")
             secret_params = {
                 "name": utils.generate_id("secret-noti-proto", 4),
                 "data": plugin_info["secret_data"],
-                "resource_group": "WORKSPACE",
+                "resource_group": "DOMAIN",
             }
 
             # if schema_id := plugin_info.get("schema_id"):
             #     secret_params["schema_id"] = schema_id
             # if provider := plugin_info.get("provider"):
             #     secret_params["provider"] = provider
```

### Comparing `spaceone-notification-2.0.dev8/spaceone/notification/service/user_channel_service.py` & `spaceone-notification-2.0.dev9/spaceone/notification/service/user_channel_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-notification-2.0.dev8/spaceone_notification.egg-info/SOURCES.txt` & `spaceone-notification-2.0.dev9/spaceone_notification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

