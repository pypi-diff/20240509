# Comparing `tmp/bttc-0.0.77.3.tar.gz` & `tmp/bttc-0.0.77.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.77.3.tar", last modified: Mon May  6 14:51:46 2024, max compression
+gzip compressed data, was "bttc-0.0.77.4.tar", last modified: Thu May  9 02:38:52 2024, max compression
```

## Comparing `bttc-0.0.77.3.tar` & `bttc-0.0.77.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.257136 bttc-0.0.77.3/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.77.3/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2160 2024-05-06 14:51:46.257136 bttc-0.0.77.3/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1430 2024-05-06 13:58:19.000000 bttc-0.0.77.3/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.249136 bttc-0.0.77.3/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6838 2024-05-06 14:51:31.000000 bttc-0.0.77.3/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.77.3/bttc/apk_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.77.3/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.77.3/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.77.3/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4211 2024-05-05 01:21:12.000000 bttc-0.0.77.3/bttc/general_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    36150 2024-05-06 14:42:05.000000 bttc-0.0.77.3/bttc/general_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/mc_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/mc_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.249136 bttc-0.0.77.3/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.77.3/bttc/utils/device_factory.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2336 2024-05-06 07:32:12.000000 bttc-0.0.77.3/bttc/utils/dialer_simulator.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.77.3/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    10543 2024-05-05 01:21:12.000000 bttc-0.0.77.3/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/utils/logcat.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.257136 bttc-0.0.77.3/bttc/utils/media_player/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/utils/media_player/media_player_agent_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5331 2024-05-06 13:58:19.000000 bttc-0.0.77.3/bttc/utils/media_player/yt_player_agent.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/utils/typing_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.257136 bttc-0.0.77.3/bttc/utils/ui_pages/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/utils/ui_pages/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.77.3/bttc/utils/ui_pages/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    17093 2024-05-06 13:58:19.000000 bttc-0.0.77.3/bttc/utils/ui_pages/ui_core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/utils/ui_pages/ui_node.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/utils/ui_pages/utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.77.3/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.77.3/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-06 14:51:46.253136 bttc-0.0.77.3/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2160 2024-05-06 14:51:46.000000 bttc-0.0.77.3/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1618 2024-05-06 14:51:46.000000 bttc-0.0.77.3/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-05-06 14:51:46.000000 bttc-0.0.77.3/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-05-06 14:51:46.000000 bttc-0.0.77.3/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-05-06 14:51:46.000000 bttc-0.0.77.3/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-05-06 14:51:46.257136 bttc-0.0.77.3/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.77.3/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.019067 bttc-0.0.77.4/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.77.4/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2160 2024-05-09 02:38:52.019067 bttc-0.0.77.4/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1430 2024-05-06 13:58:19.000000 bttc-0.0.77.4/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.015067 bttc-0.0.77.4/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6838 2024-05-09 02:38:42.000000 bttc-0.0.77.4/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9617 2024-04-15 06:13:29.000000 bttc-0.0.77.4/bttc/apk_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-04-08 13:33:17.000000 bttc-0.0.77.4/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16481 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.015067 bttc-0.0.77.4/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-10 06:01:48.000000 bttc-0.0.77.4/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22596 2024-04-15 06:24:35.000000 bttc-0.0.77.4/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3956 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4489 2024-05-08 02:00:40.000000 bttc-0.0.77.4/bttc/general_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    36150 2024-05-06 14:42:05.000000 bttc-0.0.77.4/bttc/general_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1062 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/mc_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5053 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/mc_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.015067 bttc-0.0.77.4/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.015067 bttc-0.0.77.4/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.011067 bttc-0.0.77.4/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.015067 bttc-0.0.77.4/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.019067 bttc-0.0.77.4/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     9130 2024-05-09 02:36:08.000000 bttc-0.0.77.4/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6497 2024-05-09 02:35:18.000000 bttc-0.0.77.4/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.019067 bttc-0.0.77.4/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3932 2024-04-15 06:13:29.000000 bttc-0.0.77.4/bttc/utils/device_factory.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2238 2024-05-07 06:26:37.000000 bttc-0.0.77.4/bttc/utils/dialer_simulator.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.019067 bttc-0.0.77.4/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5893 2024-05-05 01:21:12.000000 bttc-0.0.77.4/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    11329 2024-05-08 03:08:22.000000 bttc-0.0.77.4/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/utils/logcat.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.019067 bttc-0.0.77.4/bttc/utils/media_player/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1227 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/utils/media_player/media_player_agent_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5331 2024-05-06 13:58:19.000000 bttc-0.0.77.4/bttc/utils/media_player/yt_player_agent.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/utils/typing_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.019067 bttc-0.0.77.4/bttc/utils/ui_pages/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3877 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/utils/ui_pages/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1677 2024-04-29 08:53:55.000000 bttc-0.0.77.4/bttc/utils/ui_pages/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    17093 2024-05-06 13:58:19.000000 bttc-0.0.77.4/bttc/utils/ui_pages/ui_core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7585 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/utils/ui_pages/ui_node.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2320 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/utils/ui_pages/utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2960 2024-04-28 06:22:01.000000 bttc-0.0.77.4/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.77.4/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-05-09 02:38:52.015067 bttc-0.0.77.4/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2160 2024-05-09 02:38:51.000000 bttc-0.0.77.4/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1618 2024-05-09 02:38:51.000000 bttc-0.0.77.4/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-05-09 02:38:51.000000 bttc-0.0.77.4/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      185 2024-05-09 02:38:51.000000 bttc-0.0.77.4/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-05-09 02:38:51.000000 bttc-0.0.77.4/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-05-09 02:38:52.023067 bttc-0.0.77.4/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1772 2024-04-28 06:22:01.000000 bttc-0.0.77.4/setup.py
```

### Comparing `bttc-0.0.77.3/LICENSE` & `bttc-0.0.77.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/PKG-INFO` & `bttc-0.0.77.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.77.3
+Version: 0.0.77.4
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.77.3/README.md` & `bttc-0.0.77.4/README.md`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/__init__.py` & `bttc-0.0.77.4/bttc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 import shlex
 from typing import Callable, TypeAlias
 
 
-__version__ = '0.0.77.3'
+__version__ = '0.0.77.4'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.77.3/bttc/apk_utils.py` & `bttc-0.0.77.4/bttc/apk_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/ble_data.py` & `bttc-0.0.77.4/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/ble_utils.py` & `bttc-0.0.77.4/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/bt_data.py` & `bttc-0.0.77.4/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/bt_utils.py` & `bttc-0.0.77.4/bttc/bt_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/cli/__init__.py` & `bttc-0.0.77.4/bttc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/cli/constants.py` & `bttc-0.0.77.4/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/cli/main.py` & `bttc-0.0.77.4/bttc/cli/main.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/common_data.py` & `bttc-0.0.77.4/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/constants.py` & `bttc-0.0.77.4/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/core.py` & `bttc-0.0.77.4/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/errors.py` & `bttc-0.0.77.4/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/general_data.py` & `bttc-0.0.77.4/bttc/general_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,23 @@
     Min: 1
     Max: 7
     streamVolume:5
     Current: 1 (earpiece): 5, 80 (bt_a2dp): 5, 40000000 (default): 5
     Devices: earpiece(1)
     Volume Group: AUDIO_STREAM_VOICE_CALL
   ```
+
+  Attributes:
+    name: Name of audio stream.
+    is_muted: True iff the audio is muted.
+    min_level: Minimum of volume level.
+    max_level: Maximum of volume level.
+    stream_volume_level: Stream volume level.
+    current: Current device.
+    devices: Device information.
   """
 
   name: str
   is_muted: bool = False
   min_level: int = -1
   max_level: int = -1
   stream_volume_level: int = -1
```

### Comparing `bttc-0.0.77.3/bttc/general_utils.py` & `bttc-0.0.77.4/bttc/general_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/mc_data.py` & `bttc-0.0.77.4/bttc/mc_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/mc_utils.py` & `bttc-0.0.77.4/bttc/mc_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.77.4/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.77.4/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.77.4/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.77.4/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.77.4/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.77.4/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.77.4/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/profiles/avrcp/errors.py` & `bttc-0.0.77.4/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/profiles/hfp/__init__.py` & `bttc-0.0.77.4/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/profiles/hfp/constants.py` & `bttc-0.0.77.4/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/profiles/hfp/errors.py` & `bttc-0.0.77.4/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.77.4/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.77.4/bttc/profiles/hfp/hfp_devices.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """Phone implementation from HFP interface PhoneDevice."""
 
 import shlex
 import time
 
 from mobly.controllers.android_device_lib import adb
 
-from bttc import general_utils
+from bttc.utils import dialer_simulator
 from bttc.utils import key_events_handler
 from bttc.utils import retry
 from bttc.utils import typing_utils
 from bttc.profiles.hfp import constants
 from bttc.profiles.hfp import errors
 from bttc.profiles.hfp import hfp_data
 from bttc.profiles.hfp import hfp_facade
@@ -40,15 +40,15 @@
 
 class AndroidPhone(hfp_facade.PhoneDevice):
   """Android phone device."""
 
   def __init__(self, device: typing_utils.AndroidLike,
                phone_number: str):
     super().__init__(phone_number, device.log)
-    self._device = general_utils.bind(device)
+    self._device = device
     self._key_event_handler = (
         key_events_handler.KeyEventHandler(self._device))
 
   def to_phone_device(self) -> hfp_facade.PhoneDevice:
     """Translates into phone device.
 
     Returns:
@@ -240,7 +240,38 @@
   def set_call_audio_route(self, audio_route: constants.AudioRoute):
     """Sets call audio route.
 
     Args:
       audio_route: Audio route to switch to.
     """
     self._device.sl4a.telecomCallSetAudioRoute(audio_route.value)
+
+
+class AndroidPhoneWithDialerSimulator(AndroidPhone):
+  """Android with dialer simulator apk installed."""
+
+  def __init__(self, device: typing_utils.AndroidLike,
+               phone_number: str | None = None):
+    super().__init__(device, phone_number)
+    self._ds = dialer_simulator.DialerSimulator(device)
+
+  @property
+  def ds(self) -> dialer_simulator.DialerSimulator:
+    return self._ds
+
+  def outgoing_call(self) -> hfp_facade.CallResult:
+    """Makes simulated outgoing call.
+
+    Returns:
+      dataclass CallResult to represent calling result.
+    """
+    self.ds.make_outgoing_call()
+    return hfp_facade.CallResult(self, None)
+
+  def incoming_call(self) -> hfp_facade.CallResult:
+    """Makes simulated incoming call.
+
+    Returns:
+      dataclass CallResult to represent calling result.
+    """
+    self.ds.make_incoming_call()
+    return hfp_facade.CallResult(None, self)
```

### Comparing `bttc-0.0.77.3/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.77.4/bttc/profiles/hfp/hfp_facade.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """HFP Facade module."""
 
 from __future__ import annotations
 
 import abc
 import dataclasses
-from typing import Optional, Protocol
+from typing import Protocol
 
 from bttc.profiles.hfp import constants
 from bttc.profiles.hfp import hfp_data
 from bttc.utils import typing_utils
 
 
 _CALL_IDLE = hfp_data.CallStateEnum.IDLE
@@ -36,14 +36,18 @@
     log: Logger object.
   """
 
   def __init__(self, phone_number: str, log: typing_utils.LogProtocol):
     self.phone_number = phone_number
     self.log = log
 
+  @property
+  def call_state(self) -> hfp_data.CallStateEnum:
+    return self.get_call_state()
+
   def is_incall(self) -> bool:
     """Checks if the device is in call or not.
 
     Returns
       True iff the device is in call.
     """
     raise NotImplementedError(
@@ -75,14 +79,34 @@
     Raises:
       BrokenPipeError: If called while the socket is disconnected.
       jsonrpc_client_base.Error: Something wrong with SL4A API call.
     """
     raise NotImplementedError(
         f'Subclass={self} should implement `wait_for_call_state`!')
 
+  def incoming_call(self) -> CallResult:
+    """Simulates incoming call.
+
+    This method is only valid with dialer simulator available in DUT.
+
+    Returns:
+      dataclass CallResult to represent calling result.
+    """
+    raise NotImplementedError('`incoming_call` is not implemented!')
+
+  def outgoing_call(self) -> CallResult:
+    """Simulates outgoing call.
+
+    This method is only valid with dialer simulator available in DUT.
+
+    Returns:
+      dataclass CallResult to represent calling result.
+    """
+    raise NotImplementedError('`outgoing_call` is not implemented!')
+
   def call(self, callee: PhoneDevice) -> CallResult:
     """Calls the target device.
 
     Args:
       callee: The target device to call.
 
     Returns:
@@ -157,17 +181,17 @@
     """
     ...
 
 
 @dataclasses.dataclass
 class CallResult:
   """Result of a call between two devices."""
-  caller: PhoneDevice
-  callee: PhoneDevice
-  error: Optional[str] = None
+  caller: PhoneDevice | None
+  callee: PhoneDevice | None
+  error: str | None = None
 
 
 class HFPFacade:
   """HFP Facade class."""
 
   def __init__(self, caller_device: PhoneDevice, callee_device: PhoneDevice):
     self._caller_device = caller_device
```

### Comparing `bttc-0.0.77.3/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.77.4/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/strategy.py` & `bttc-0.0.77.4/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/ad_checker.py` & `bttc-0.0.77.4/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/device_factory.py` & `bttc-0.0.77.4/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/dialer_simulator.py` & `bttc-0.0.77.4/bttc/utils/dialer_simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,19 +32,17 @@
         ['dumpsys', 'package', DIALER_PACKAGE_NAME, '|', 'grep', '-E',
          '"versionName=(.+)"', '||', 'echo  ']).decode('utf-8').strip()
     version = re.findall(r'versionName=(.+)', output)
     if not version:
       raise Error(self._device, 'Dialer app is not installed.')
     self._device.log.debug('Dialer Simulator Version: %s', version)
     if 'dogfood' not in version[0]:
-      # raise Error(
-      #     self._device,
-      #     f'Dialer app is not dogfood version: {version}')
-      self._device.log.warning(
-          'Dialer app version is not dogfood: %s', version)
+      raise Error(
+          self._device,
+          f'Dialer app is not dogfood version: {version}')
 
   def execute_command(self, *cmd_args: str) -> None:
     """Executes a command.
 
     Args:
       *cmd_args: Arguments for the command.
     """
```

### Comparing `bttc-0.0.77.3/bttc/utils/iperf/__init__.py` & `bttc-0.0.77.4/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/iperf/errors.py` & `bttc-0.0.77.4/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/key_events_handler.py` & `bttc-0.0.77.4/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/log_parser.py` & `bttc-0.0.77.4/bttc/utils/log_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,48 @@
 DeviceInfo = ble_data.DeviceInfo
 StateMachineLog = ble_data.StateMachineLog
 LeAudioStateMachine = ble_data.LeAudioStateMachine
 
 
 def parse_audio_dump_for_volume_info(
     log_content: str) -> dict[str, general_data.AudioStreamVolume]:
-  """Parses the audio dumps to retrieve the volume information."""
+  """Parses the audio dumps to retrieve the volume information.
+
+  `log_content` is expected to collect from below command in DUT:
+  ```
+  $ dumpsys audio
+  ...
+  Stream volumes (device: index)
+  - STREAM_VOICE_CALL:
+    Muted: false
+    Muted Internally: false
+    Min: 1
+    Max: 7
+    streamVolume:5
+    Current: 1 (earpiece): 4, 10 (bt_sco): 5, 80 (bt_a2dp): 5, ...(default): 5
+    Devices: bt_a2dp(80)
+    Volume Group: AUDIO_STREAM_VOICE_CALL
+  ...
+  ```
+
+  Args:
+    log_content: Log content to parse.
+
+  Returns:
+    dict object with key as name of audo stream and value as corresponding
+    parsing result.
+
+  Raises:
+    ValueError: Unexpected log content.
+  """
   stream_header_pattern = re.compile('STREAM_([_A-Z0-9]+)')
   log_lines = log_content.split('\n')
   current_volume_setting_record: general_data.AudioStreamVolume | None = None
   collected_volume_info: dict[str, general_data.AudioStreamVolume] = {}
+  is_parse_done = False
   for i, line in enumerate(log_lines):
     if line.startswith('Stream volumes'):
       # Start parsing
       for line in log_lines[i+1:]:
         line = line.strip()
         if line.startswith('- '):
           # New volume type. e.g.:
@@ -81,21 +110,28 @@
         elif line.startswith('Devices:'):
           current_volume_setting_record.devices = line.split(':')[1].strip()
         elif line.startswith('Current:'):
           current_volume_setting_record.current = (
               int(line.split(':')[1].strip().split()[0]))
         elif line == '':
           if current_volume_setting_record is None:
+            is_parse_done = True
             break
 
           # Save the parsing record
           collected_volume_info[current_volume_setting_record.name] = (
               current_volume_setting_record)
           current_volume_setting_record = None
 
+      if is_parse_done:
+        break
+
+  if not is_parse_done:
+    raise ValueError('Audio stream content is not found!')
+
   return collected_volume_info
 
 
 def parse_bluetooth_crash_info(log_content: str) -> Sequence[str]:
   """Parses the BT manager log to collect crash information.
 
   For this function to work, we expect below log snippet from given log content:
```

### Comparing `bttc-0.0.77.3/bttc/utils/logcat.py` & `bttc-0.0.77.4/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/media_player/media_player_agent_facade.py` & `bttc-0.0.77.4/bttc/utils/media_player/media_player_agent_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/media_player/yt_player_agent.py` & `bttc-0.0.77.4/bttc/utils/media_player/yt_player_agent.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/retry.py` & `bttc-0.0.77.4/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/typing_utils.py` & `bttc-0.0.77.4/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/ui_pages/__init__.py` & `bttc-0.0.77.4/bttc/utils/ui_pages/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/ui_pages/errors.py` & `bttc-0.0.77.4/bttc/utils/ui_pages/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/ui_pages/ui_core.py` & `bttc-0.0.77.4/bttc/utils/ui_pages/ui_core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/ui_pages/ui_node.py` & `bttc-0.0.77.4/bttc/utils/ui_pages/ui_node.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils/ui_pages/utils.py` & `bttc-0.0.77.4/bttc/utils/ui_pages/utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/utils_loader.py` & `bttc-0.0.77.4/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc/wifi_utils.py` & `bttc-0.0.77.4/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/bttc.egg-info/PKG-INFO` & `bttc-0.0.77.4/bttc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.77.3
+Version: 0.0.77.4
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bttc-0.0.77.3/bttc.egg-info/SOURCES.txt` & `bttc-0.0.77.4/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.77.3/setup.py` & `bttc-0.0.77.4/setup.py`

 * *Files identical despite different names*

