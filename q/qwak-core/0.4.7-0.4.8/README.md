# Comparing `tmp/qwak_core-0.4.7.tar.gz` & `tmp/qwak_core-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.4.7.tar", max compression
+gzip compressed data, was "qwak_core-0.4.8.tar", max compression
```

## Comparing `qwak_core-0.4.7.tar` & `qwak_core-0.4.8.tar`

### file list

```diff
@@ -1,818 +1,818 @@
--rw-r--r--   0        0        0      264 2024-05-08 11:46:13.386486 qwak_core-0.4.7/README.md
--rw-r--r--   0        0        0        0 2024-05-08 11:48:53.312527 qwak_core-0.4.7/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5877 2024-05-08 11:48:53.340526 qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     7824 2024-05-08 11:48:22.453680 qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.344526 qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0    12703 2024-05-08 11:48:53.344526 qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py
--rw-r--r--   0        0        0    10914 2024-05-08 11:48:22.657673 qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi
--rw-r--r--   0        0        0    14681 2024-05-08 11:48:53.344526 qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2024-05-08 11:48:53.336526 qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2024-05-08 11:48:22.049695 qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.336526 qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2024-05-08 11:48:53.340526 qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2024-05-08 11:48:22.249688 qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.340526 qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2024-05-08 11:48:53.328526 qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2024-05-08 11:48:21.437718 qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2024-05-08 11:48:53.332526 qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2024-05-08 11:48:53.332526 qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2024-05-08 11:48:21.641711 qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.332526 qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4901 2024-05-08 11:48:53.336526 qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5995 2024-05-08 11:48:21.841703 qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.336526 qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2024-05-08 11:48:53.312527 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2024-05-08 11:48:21.233726 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2024-05-08 11:48:53.316527 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     7360 2024-05-08 11:48:53.316527 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0    11651 2024-05-08 11:48:22.865665 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.316527 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     5029 2024-05-08 11:48:53.320527 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     6943 2024-05-08 11:48:23.309648 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.324526 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2024-05-08 11:48:53.324526 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2024-05-08 11:48:23.521641 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2024-05-08 11:48:53.324526 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2024-05-08 11:48:53.320527 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2024-05-08 11:48:23.069657 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.320527 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6541 2024-05-08 11:48:53.328526 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10595 2024-05-08 11:48:23.757632 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.328526 qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0    15382 2024-05-08 11:48:53.380524 qwak_core-0.4.7/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    20668 2024-05-08 11:48:26.693522 qwak_core-0.4.7/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.384524 qwak_core-0.4.7/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2024-05-08 11:48:53.384524 qwak_core-0.4.7/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2024-05-08 11:48:26.905515 qwak_core-0.4.7/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2024-05-08 11:48:53.384524 qwak_core-0.4.7/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7616 2024-05-08 11:48:53.512519 qwak_core-0.4.7/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11995 2024-05-08 11:48:37.037134 qwak_core-0.4.7/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.512519 qwak_core-0.4.7/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0    14893 2024-05-08 11:48:53.512519 qwak_core-0.4.7/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0    11812 2024-05-08 11:48:37.265125 qwak_core-0.4.7/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    19155 2024-05-08 11:48:53.512519 qwak_core-0.4.7/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2024-05-08 11:48:53.516519 qwak_core-0.4.7/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2024-05-08 11:48:38.625074 qwak_core-0.4.7/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2024-05-08 11:48:53.520519 qwak_core-0.4.7/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8864 2024-05-08 11:48:53.516519 qwak_core-0.4.7/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13789 2024-05-08 11:48:38.413082 qwak_core-0.4.7/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.516519 qwak_core-0.4.7/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5777 2024-05-08 11:48:53.520519 qwak_core-0.4.7/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8264 2024-05-08 11:48:38.853065 qwak_core-0.4.7/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.524519 qwak_core-0.4.7/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2024-05-08 11:48:53.524519 qwak_core-0.4.7/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2024-05-08 11:48:39.069057 qwak_core-0.4.7/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2024-05-08 11:48:53.524519 qwak_core-0.4.7/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    14053 2024-05-08 11:48:53.644514 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    20860 2024-05-08 11:48:49.320675 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.644514 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5775 2024-05-08 11:48:53.636515 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     8308 2024-05-08 11:48:48.908691 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.640515 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3954 2024-05-08 11:48:53.640515 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     5309 2024-05-08 11:48:49.108683 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.640515 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    21176 2024-05-08 11:48:53.632515 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    15049 2024-05-08 11:48:48.496706 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    25475 2024-05-08 11:48:53.632515 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2024-05-08 11:48:53.636515 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2024-05-08 11:48:48.704698 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.636515 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2024-05-08 11:48:53.648514 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2024-05-08 11:48:49.924653 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.652514 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2024-05-08 11:48:53.648514 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2024-05-08 11:48:49.720661 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.648514 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2024-05-08 11:48:53.644514 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2024-05-08 11:48:49.520668 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.644514 qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    11218 2024-05-08 11:48:53.628515 qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    15584 2024-05-08 11:48:48.172718 qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.632515 qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2083 2024-05-08 11:48:53.624515 qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1977 2024-05-08 11:48:47.708735 qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.624515 qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    46028 2024-05-08 11:48:53.624515 qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    60013 2024-05-08 11:48:47.972725 qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    32008 2024-05-08 11:48:53.628515 qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    29124 2024-05-08 11:48:53.560518 qwak_core-0.4.7/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    24434 2024-05-08 11:48:41.300974 qwak_core-0.4.7/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    27837 2024-05-08 11:48:53.560518 qwak_core-0.4.7/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    33279 2024-05-08 11:48:53.556518 qwak_core-0.4.7/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    52325 2024-05-08 11:48:40.848991 qwak_core-0.4.7/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.556518 qwak_core-0.4.7/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0     5757 2024-05-08 11:48:53.564518 qwak_core-0.4.7/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py
--rw-r--r--   0        0        0     4013 2024-05-08 11:48:42.016947 qwak_core-0.4.7/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi
--rw-r--r--   0        0        0     6783 2024-05-08 11:48:53.564518 qwak_core-0.4.7/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py
--rw-r--r--   0        0        0     6016 2024-05-08 11:48:53.560518 qwak_core-0.4.7/_qwak_proto/qwak/build_settings/build_settings_pb2.py
--rw-r--r--   0        0        0     7049 2024-05-08 11:48:41.784956 qwak_core-0.4.7/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.564518 qwak_core-0.4.7/_qwak_proto/qwak/build_settings/build_settings_pb2_grpc.py
--rw-r--r--   0        0        0    14991 2024-05-08 11:48:53.544518 qwak_core-0.4.7/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    24472 2024-05-08 11:48:40.616999 qwak_core-0.4.7/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.544518 qwak_core-0.4.7/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     5552 2024-05-08 11:48:53.544518 qwak_core-0.4.7/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     7299 2024-05-08 11:48:41.064983 qwak_core-0.4.7/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.548518 qwak_core-0.4.7/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    15672 2024-05-08 11:48:53.548518 qwak_core-0.4.7/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0    12741 2024-05-08 11:48:41.536965 qwak_core-0.4.7/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    16925 2024-05-08 11:48:53.548518 qwak_core-0.4.7/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38491 2024-05-08 11:48:53.552518 qwak_core-0.4.7/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    53557 2024-05-08 11:48:42.748920 qwak_core-0.4.7/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2024-05-08 11:48:53.556518 qwak_core-0.4.7/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     3508 2024-05-08 11:48:53.552518 qwak_core-0.4.7/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     2300 2024-05-08 11:48:42.240939 qwak_core-0.4.7/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0     3101 2024-05-08 11:48:53.552518 qwak_core-0.4.7/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0     2270 2024-05-08 11:48:53.572517 qwak_core-0.4.7/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     2697 2024-05-08 11:48:43.240902 qwak_core-0.4.7/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.572517 qwak_core-0.4.7/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4458 2024-05-08 11:48:53.572517 qwak_core-0.4.7/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     3113 2024-05-08 11:48:43.468893 qwak_core-0.4.7/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2024-05-08 11:48:53.576517 qwak_core-0.4.7/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2024-05-08 11:48:53.536519 qwak_core-0.4.7/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2024-05-08 11:48:39.977023 qwak_core-0.4.7/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.536519 qwak_core-0.4.7/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11871 2024-05-08 11:48:53.536519 qwak_core-0.4.7/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     8790 2024-05-08 11:48:40.181016 qwak_core-0.4.7/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2024-05-08 11:48:53.540518 qwak_core-0.4.7/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2024-05-08 11:48:53.528519 qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2024-05-08 11:48:39.525040 qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.532519 qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    50041 2024-05-08 11:48:53.528519 qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    74372 2024-05-08 11:48:39.297048 qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.528519 qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    46309 2024-05-08 11:48:53.532519 qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    40356 2024-05-08 11:48:39.761031 qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    27756 2024-05-08 11:48:53.532519 qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     3345 2024-05-08 11:48:53.368525 qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     4098 2024-05-08 11:48:25.649561 qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.368525 qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12707 2024-05-08 11:48:53.372525 qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    13800 2024-05-08 11:48:25.857554 qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.372525 qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    17949 2024-05-08 11:48:53.372525 qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    18562 2024-05-08 11:48:26.065546 qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    12833 2024-05-08 11:48:53.376525 qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     6463 2024-05-08 11:48:53.464521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/backfill_pb2.py
--rw-r--r--   0        0        0     7945 2024-05-08 11:48:32.069321 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.464521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/backfill_pb2_grpc.py
--rw-r--r--   0        0        0     2971 2024-05-08 11:48:53.468521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/batch_pb2.py
--rw-r--r--   0        0        0     3266 2024-05-08 11:48:32.273314 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.468521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/batch_pb2_grpc.py
--rw-r--r--   0        0        0     2210 2024-05-08 11:48:53.468521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/deletion_pb2.py
--rw-r--r--   0        0        0     1540 2024-05-08 11:48:32.485306 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.472521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/deletion_pb2_grpc.py
--rw-r--r--   0        0        0     5793 2024-05-08 11:48:53.472521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/execution_pb2.py
--rw-r--r--   0        0        0     7373 2024-05-08 11:48:32.693298 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.472521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/execution_pb2_grpc.py
--rw-r--r--   0        0        0    14900 2024-05-08 11:48:53.472521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/execution_service_pb2.py
--rw-r--r--   0        0        0    11103 2024-05-08 11:48:32.897290 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi
--rw-r--r--   0        0        0    17220 2024-05-08 11:48:53.476521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py
--rw-r--r--   0        0        0     7695 2024-05-08 11:48:53.480521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py
--rw-r--r--   0        0        0    14959 2024-05-08 11:48:33.309275 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.480521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0    19304 2024-05-08 11:48:53.480521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py
--rw-r--r--   0        0        0    16916 2024-05-08 11:48:33.517267 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    21145 2024-05-08 11:48:53.484521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     8440 2024-05-08 11:48:53.476521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py
--rw-r--r--   0        0        0    13312 2024-05-08 11:48:33.101282 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.476521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     2051 2024-05-08 11:48:53.484521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py
--rw-r--r--   0        0        0     1952 2024-05-08 11:48:33.721259 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.484521 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/execution_state_pb2_grpc.py
--rw-r--r--   0        0        0    12222 2024-05-08 11:48:53.488520 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py
--rw-r--r--   0        0        0     7930 2024-05-08 11:48:33.929251 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi
--rw-r--r--   0        0        0    14212 2024-05-08 11:48:53.488520 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py
--rw-r--r--   0        0        0     1685 2024-05-08 11:48:53.488520 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py
--rw-r--r--   0        0        0     1272 2024-05-08 11:48:34.137243 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.492520 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2_grpc.py
--rw-r--r--   0        0        0     6198 2024-05-08 11:48:53.492520 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py
--rw-r--r--   0        0        0     7677 2024-05-08 11:48:34.393234 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.492520 qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2024-05-08 11:48:53.440522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2024-05-08 11:48:31.861329 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.440522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2024-05-08 11:48:53.436522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2024-05-08 11:48:31.653337 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2024-05-08 11:48:53.436522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0    11432 2024-05-08 11:48:53.408523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    12882 2024-05-08 11:48:29.393422 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.408523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0    13825 2024-05-08 11:48:53.420523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/deployment_pb2.py
--rw-r--r--   0        0        0    19227 2024-05-08 11:48:30.413384 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.420523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/deployment_pb2_grpc.py
--rw-r--r--   0        0        0     3307 2024-05-08 11:48:53.424523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py
--rw-r--r--   0        0        0     1637 2024-05-08 11:48:30.613376 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi
--rw-r--r--   0        0        0     3293 2024-05-08 11:48:53.424523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     5303 2024-05-08 11:48:53.404523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8604 2024-05-08 11:48:29.189429 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.404523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2024-05-08 11:48:53.396524 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2024-05-08 11:48:28.557453 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.396524 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    28920 2024-05-08 11:48:53.400524 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20665 2024-05-08 11:48:28.989437 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    35307 2024-05-08 11:48:53.404523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2024-05-08 11:48:53.408523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2024-05-08 11:48:29.593414 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.412523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2024-05-08 11:48:53.412523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2024-05-08 11:48:29.797407 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2024-05-08 11:48:53.412523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    26853 2024-05-08 11:48:53.400524 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    39247 2024-05-08 11:48:28.773445 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.400524 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2024-05-08 11:48:53.416523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2024-05-08 11:48:29.997399 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.416523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0    13240 2024-05-08 11:48:53.416523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
--rw-r--r--   0        0        0    18420 2024-05-08 11:48:30.205392 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.420523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2024-05-08 11:48:53.440522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2024-05-08 11:48:52.148570 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.440522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2024-05-08 11:48:53.444522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2024-05-08 11:48:52.420560 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2024-05-08 11:48:53.444522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     4308 2024-05-08 11:48:53.444522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     7410 2024-05-08 11:48:36.377159 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.448522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    15316 2024-05-08 11:48:53.448522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    14087 2024-05-08 11:48:36.609150 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    18465 2024-05-08 11:48:53.448522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2024-05-08 11:48:53.452522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2024-05-08 11:48:36.825142 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.452522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     5111 2024-05-08 11:48:53.460521 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/management_pb2.py
--rw-r--r--   0        0        0     2739 2024-05-08 11:48:38.197090 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi
--rw-r--r--   0        0        0     5436 2024-05-08 11:48:53.464521 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py
--rw-r--r--   0        0        0     5385 2024-05-08 11:48:53.456522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     7551 2024-05-08 11:48:37.729107 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.456522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    17474 2024-05-08 11:48:53.452522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2024-05-08 11:48:37.497116 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2024-05-08 11:48:53.456522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2024-05-08 11:48:53.460521 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2024-05-08 11:48:37.957099 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.460521 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    27355 2024-05-08 11:48:53.424523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    43393 2024-05-08 11:48:30.825369 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.428523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5147 2024-05-08 11:48:53.428523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6208 2024-05-08 11:48:31.033361 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.428523 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2024-05-08 11:48:53.432522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2024-05-08 11:48:31.241353 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2024-05-08 11:48:53.432522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11049 2024-05-08 11:48:53.432522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15942 2024-05-08 11:48:31.449345 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.436522 qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2024-05-08 11:48:53.660514 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2024-05-08 11:48:50.788621 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.660514 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2024-05-08 11:48:53.664514 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2024-05-08 11:48:51.012612 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2024-05-08 11:48:53.664514 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2024-05-08 11:48:53.664514 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2024-05-08 11:48:51.224604 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.668514 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2024-05-08 11:48:53.668514 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2024-05-08 11:48:51.456596 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2024-05-08 11:48:53.668514 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0    10469 2024-05-08 11:48:53.672514 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0    11719 2024-05-08 11:48:51.692587 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     9458 2024-05-08 11:48:53.672514 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     5302 2024-05-08 11:48:53.672514 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     5484 2024-05-08 11:48:51.896580 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.676513 qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2975 2024-05-08 11:48:53.576517 qwak_core-0.4.7/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     4026 2024-05-08 11:48:43.688885 qwak_core-0.4.7/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.576517 qwak_core-0.4.7/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4455 2024-05-08 11:48:53.580517 qwak_core-0.4.7/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     3113 2024-05-08 11:48:43.912876 qwak_core-0.4.7/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2024-05-08 11:48:53.580517 qwak_core-0.4.7/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6950 2024-05-08 11:48:53.384524 qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    11560 2024-05-08 11:48:27.725484 qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.388524 qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     3442 2024-05-08 11:48:53.388524 qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     5719 2024-05-08 11:48:27.929476 qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.388524 qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2024-05-08 11:48:53.392524 qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2024-05-08 11:48:28.133469 qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2024-05-08 11:48:53.392524 qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8504 2024-05-08 11:48:53.392524 qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12440 2024-05-08 11:48:28.333461 qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.396524 qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2024-05-08 11:48:53.540518 qwak_core-0.4.7/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2024-05-08 11:48:40.389008 qwak_core-0.4.7/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2024-05-08 11:48:53.540518 qwak_core-0.4.7/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     3876 2024-05-08 11:48:53.580517 qwak_core-0.4.7/_qwak_proto/qwak/instance_template/instance_template_pb2.py
--rw-r--r--   0        0        0     4658 2024-05-08 11:48:44.124869 qwak_core-0.4.7/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.584517 qwak_core-0.4.7/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
--rw-r--r--   0        0        0     4722 2024-05-08 11:48:53.584517 qwak_core-0.4.7/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
--rw-r--r--   0        0        0     3245 2024-05-08 11:48:44.336861 qwak_core-0.4.7/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
--rw-r--r--   0        0        0     5240 2024-05-08 11:48:53.584517 qwak_core-0.4.7/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2024-05-08 11:48:53.600516 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2024-05-08 11:48:45.684811 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.600516 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2024-05-08 11:48:53.604516 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2024-05-08 11:48:45.900802 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.604516 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    25218 2024-05-08 11:48:53.604516 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    31280 2024-05-08 11:48:46.120794 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.604516 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13432 2024-05-08 11:48:53.608516 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    22974 2024-05-08 11:48:46.336786 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.608516 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12784 2024-05-08 11:48:53.608516 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16585 2024-05-08 11:48:46.564778 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.612516 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    51171 2024-05-08 11:48:53.612516 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    40800 2024-05-08 11:48:46.812769 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    73869 2024-05-08 11:48:53.616515 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2024-05-08 11:48:53.616515 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2024-05-08 11:48:47.016761 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.616515 qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2024-05-08 11:48:53.588517 qwak_core-0.4.7/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2024-05-08 11:48:44.780844 qwak_core-0.4.7/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.592517 qwak_core-0.4.7/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2024-05-08 11:48:53.596516 qwak_core-0.4.7/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2024-05-08 11:48:45.436820 qwak_core-0.4.7/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.600516 qwak_core-0.4.7/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2024-05-08 11:48:53.592517 qwak_core-0.4.7/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2024-05-08 11:48:45.032835 qwak_core-0.4.7/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2024-05-08 11:48:53.592517 qwak_core-0.4.7/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0    10138 2024-05-08 11:48:53.596516 qwak_core-0.4.7/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    14337 2024-05-08 11:48:45.236827 qwak_core-0.4.7/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.596516 qwak_core-0.4.7/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    27866 2024-05-08 11:48:53.568517 qwak_core-0.4.7/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    32184 2024-05-08 11:48:43.000911 qwak_core-0.4.7/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    19830 2024-05-08 11:48:53.568517 qwak_core-0.4.7/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2024-05-08 11:48:53.364525 qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2024-05-08 11:48:27.313499 qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2024-05-08 11:48:53.364525 qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2024-05-08 11:48:53.360525 qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2024-05-08 11:48:27.109507 qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.360525 qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2024-05-08 11:48:53.364525 qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2024-05-08 11:48:27.517492 qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2024-05-08 11:48:53.368525 qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     1598 2024-05-08 11:48:53.652514 qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py
--rw-r--r--   0        0        0     1221 2024-05-08 11:48:50.160644 qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.652514 qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2_grpc.py
--rw-r--r--   0        0        0    11437 2024-05-08 11:48:53.656514 qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py
--rw-r--r--   0        0        0    12170 2024-05-08 11:48:50.580628 qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi
--rw-r--r--   0        0        0     9793 2024-05-08 11:48:53.660514 qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4060 2024-05-08 11:48:53.656514 qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/population_pb2.py
--rw-r--r--   0        0        0     3906 2024-05-08 11:48:50.368636 qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.656514 qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/population_pb2_grpc.py
--rw-r--r--   0        0        0    10804 2024-05-08 11:48:53.564518 qwak_core-0.4.7/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0    12120 2024-05-08 11:48:42.504929 qwak_core-0.4.7/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     9642 2024-05-08 11:48:53.568517 qwak_core-0.4.7/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2024-05-08 11:48:53.588517 qwak_core-0.4.7/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2024-05-08 11:48:44.552853 qwak_core-0.4.7/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2024-05-08 11:48:53.588517 qwak_core-0.4.7/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0    10718 2024-05-08 11:48:53.356525 qwak_core-0.4.7/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0    12627 2024-05-08 11:48:24.825592 qwak_core-0.4.7/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.360525 qwak_core-0.4.7/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    19751 2024-05-08 11:48:53.356525 qwak_core-0.4.7/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    13467 2024-05-08 11:48:24.609600 qwak_core-0.4.7/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    24352 2024-05-08 11:48:53.356525 qwak_core-0.4.7/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2024-05-08 11:48:53.348526 qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2024-05-08 11:48:23.965624 qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.348526 qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2477 2024-05-08 11:48:53.348526 qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2679 2024-05-08 11:48:24.169616 qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.352525 qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2024-05-08 11:48:53.352525 qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2024-05-08 11:48:24.393608 qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2024-05-08 11:48:53.352525 qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6909 2024-05-08 11:48:53.620515 qwak_core-0.4.7/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     5186 2024-05-08 11:48:47.480744 qwak_core-0.4.7/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2024-05-08 11:48:53.620515 qwak_core-0.4.7/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7868 2024-05-08 11:48:53.616515 qwak_core-0.4.7/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    12177 2024-05-08 11:48:47.256752 qwak_core-0.4.7/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.620515 qwak_core-0.4.7/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0    11396 2024-05-08 11:48:53.376525 qwak_core-0.4.7/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0    15139 2024-05-08 11:48:26.269538 qwak_core-0.4.7/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.376525 qwak_core-0.4.7/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     3645 2024-05-08 11:48:53.380524 qwak_core-0.4.7/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2983 2024-05-08 11:48:26.473531 qwak_core-0.4.7/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.380524 qwak_core-0.4.7/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     8648 2024-05-08 11:48:53.496520 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py
--rw-r--r--   0        0        0    12852 2024-05-08 11:48:34.845217 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.500520 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/collection_pb2_grpc.py
--rw-r--r--   0        0        0    13830 2024-05-08 11:48:53.500520 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py
--rw-r--r--   0        0        0    10297 2024-05-08 11:48:35.065208 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi
--rw-r--r--   0        0        0    17183 2024-05-08 11:48:53.500520 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py
--rw-r--r--   0        0        0     1873 2024-05-08 11:48:53.496520 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py
--rw-r--r--   0        0        0     1550 2024-05-08 11:48:34.625225 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.496520 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2_grpc.py
--rw-r--r--   0        0        0     8996 2024-05-08 11:48:53.504520 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/filters_pb2.py
--rw-r--r--   0        0        0    11380 2024-05-08 11:48:35.281200 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.504520 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/filters_pb2_grpc.py
--rw-r--r--   0        0        0     4533 2024-05-08 11:48:53.504520 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/vector_pb2.py
--rw-r--r--   0        0        0     6103 2024-05-08 11:48:35.497192 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.508520 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/vector_pb2_grpc.py
--rw-r--r--   0        0        0     9738 2024-05-08 11:48:53.508520 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py
--rw-r--r--   0        0        0    10977 2024-05-08 11:48:35.709184 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi
--rw-r--r--   0        0        0    10157 2024-05-08 11:48:53.508520 qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py
--rw-r--r--   0        0        0    10852 2024-05-08 11:48:53.676513 qwak_core-0.4.7/_qwak_proto/qwak/workspace/workspace_pb2.py
--rw-r--r--   0        0        0    17043 2024-05-08 11:48:52.688550 qwak_core-0.4.7/_qwak_proto/qwak/workspace/workspace_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-08 11:48:53.676513 qwak_core-0.4.7/_qwak_proto/qwak/workspace/workspace_pb2_grpc.py
--rw-r--r--   0        0        0    21429 2024-05-08 11:48:53.680513 qwak_core-0.4.7/_qwak_proto/qwak/workspace/workspace_service_pb2.py
--rw-r--r--   0        0        0    13726 2024-05-08 11:48:52.916542 qwak_core-0.4.7/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi
--rw-r--r--   0        0        0    27193 2024-05-08 11:48:53.680513 qwak_core-0.4.7/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py
--rw-r--r--   0        0        0     3696 2024-05-08 11:49:03.064164 qwak_core-0.4.7/pyproject.toml
--rw-r--r--   0        0        0      585 2024-05-08 11:49:03.064164 qwak_core-0.4.7/qwak/__init__.py
--rw-r--r--   0        0        0     1522 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3228 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    12456 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/automations/automations.py
--rw-r--r--   0        0        0    12907 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/automations/batch_execution_action.py
--rw-r--r--   0        0        0    26800 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/automations/build_and_deploy_action.py
--rw-r--r--   0        0        0     2404 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/automations/common.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/_inner/__init__.py
--rw-r--r--   0        0        0      849 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/_inner/edge_communications.py
--rw-r--r--   0        0        0      224 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5340 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       43 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/alerts_registry/__init__.py
--rw-r--r--   0        0        0     4040 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/alerts_registry/channel.py
--rw-r--r--   0        0        0     5355 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/alerts_registry/client.py
--rw-r--r--   0        0        0       42 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     9034 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2024-05-08 11:46:13.390485 qwak_core-0.4.7/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    21054 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6882 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4209 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0      105 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0     5110 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/build_orchestrator/build_model_request_getter.py
--rw-r--r--   0        0        0    16148 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0     3981 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/build_orchestrator/internal_client.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     2401 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0      885 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/data_versioning/data_tag_filter.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6806 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     4051 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/feature_store/execution_management_client.py
--rw-r--r--   0        0        0     2635 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    16056 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     8022 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/feature_store/offline_serving_client.py
--rw-r--r--   0        0        0     5811 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     2505 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0      885 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/file_versioning/file_tag_filter.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/instance_template/__init__.py
--rw-r--r--   0        0        0     2509 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/instance_template/client.py
--rw-r--r--   0        0        0       41 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9308 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     4431 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3581 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      102 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/vector_store/__init__.py
--rw-r--r--   0        0        0     4247 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/vector_store/management_client.py
--rw-r--r--   0        0        0     5293 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/vector_store/serving_client.py
--rw-r--r--   0        0        0       43 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/workspace_manager/__init__.py
--rw-r--r--   0        0        0     8136 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/clients/workspace_manager/client.py
--rw-r--r--   0        0        0      790 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      192 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      424 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/qwak_general_build_exception.py
--rw-r--r--   0        0        0      579 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0       54 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/qwak_load_configuration_exception.py
--rw-r--r--   0        0        0      274 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      137 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/qwak_remote_build_failed.py
--rw-r--r--   0        0        0      746 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/exceptions/qwak_suggestion_exception.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     1977 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/_common/artifact_utils.py
--rw-r--r--   0        0        0     7046 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/_common/feature_set_utils.py
--rw-r--r--   0        0        0     4707 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     6680 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/_common/packaging.py
--rw-r--r--   0        0        0     2316 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0     2694 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/base.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/__init__.py
--rw-r--r--   0        0        0      197 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/_batch.py
--rw-r--r--   0        0        0      658 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/_jdbc.py
--rw-r--r--   0        0        0    10805 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/athena.py
--rw-r--r--   0        0        0     3022 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/big_query.py
--rw-r--r--   0        0        0     2063 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/clickhouse.py
--rw-r--r--   0        0        0     1981 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/csv.py
--rw-r--r--   0        0        0     2130 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/elastic_search.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/filesystem/__init__.py
--rw-r--r--   0        0        0     2828 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/filesystem/aws.py
--rw-r--r--   0        0        0      245 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/filesystem/base_config.py
--rw-r--r--   0        0        0     1572 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/filesystem/gcp.py
--rw-r--r--   0        0        0     1874 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/filesystem/utils.py
--rw-r--r--   0        0        0     1921 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/mongodb.py
--rw-r--r--   0        0        0     1595 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/mysql.py
--rw-r--r--   0        0        0     1867 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/parquet.py
--rw-r--r--   0        0        0     1648 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/postgres.py
--rw-r--r--   0        0        0     3114 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/redshift.py
--rw-r--r--   0        0        0     2579 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/snowflake.py
--rw-r--r--   0        0        0     1830 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/batch/vertica.py
--rw-r--r--   0        0        0      895 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/source_authentication.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/streaming/__init__.py
--rw-r--r--   0        0        0      181 2024-05-08 11:46:13.394485 qwak_core-0.4.7/qwak/feature_store/data_sources/streaming/_streaming.py
--rw-r--r--   0        0        0      649 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/data_sources/streaming/kafka/__init__.py
--rw-r--r--   0        0        0     3959 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/data_sources/streaming/kafka/authentication.py
--rw-r--r--   0        0        0     3510 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/data_sources/streaming/kafka/deserialization.py
--rw-r--r--   0        0        0     4398 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/data_sources/streaming/kafka/kafka.py
--rw-r--r--   0        0        0     5984 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/data_sources/time_partition_columns.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     2313 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/execution/__init__.py
--rw-r--r--   0        0        0     6470 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/execution/backfill.py
--rw-r--r--   0        0        0    21243 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/execution/execution.py
--rw-r--r--   0        0        0     3564 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/execution/execution_query.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1636 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/_utils/_featureset_utils.py
--rw-r--r--   0        0        0     1979 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0     5285 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/base_feature_set.py
--rw-r--r--   0        0        0    16910 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1670 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0     1155 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0    23233 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/streaming.py
--rw-r--r--   0        0        0     9584 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/streaming_backfill.py
--rw-r--r--   0        0        0      733 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/aggregations/__init__.py
--rw-r--r--   0        0        0    14117 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py
--rw-r--r--   0        0        0     2253 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/aggregations/windows.py
--rw-r--r--   0        0        0      281 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/functions/__init__.py
--rw-r--r--   0        0        0     2425 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py
--rw-r--r--   0        0        0     1156 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/functions/schema.py
--rw-r--r--   0        0        0     9659 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/transformations.py
--rw-r--r--   0        0        0      173 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0     1216 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/offline/_offline_serving_validations.py
--rw-r--r--   0        0        0      738 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28651 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0    12597 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/offline/client_v2.py
--rw-r--r--   0        0        0      739 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/offline/feature_set_features.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0    11144 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0     2210 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/online/endpoint_utils.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/validations/__init__.py
--rw-r--r--   0        0        0     2656 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/validations/validation_options.py
--rw-r--r--   0        0        0     3783 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/validations/validation_response.py
--rw-r--r--   0        0        0     3864 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/feature_store/validations/validator.py
--rw-r--r--   0        0        0      226 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_config/__init__.py
--rw-r--r--   0        0        0    11174 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_config/build_config_v1.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/build_loggers/__init__.py
--rw-r--r--   0        0        0     1426 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/build_loggers/trigger_build_logger.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/constants/__init__.py
--rw-r--r--   0        0        0      209 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/constants/dependencies.py
--rw-r--r--   0        0        0      131 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/constants/host_resource.py
--rw-r--r--   0        0        0       94 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/constants/messages.py
--rw-r--r--   0        0        0       36 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/constants/temp_dir.py
--rw-r--r--   0        0        0      279 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/constants/upload_tag.py
--rw-r--r--   0        0        0      116 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/dependency_manager_type.py
--rw-r--r--   0        0        0     2299 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/execute_build_pipeline.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/interface/__init__.py
--rw-r--r--   0        0        0      528 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/interface/build_logger_interface.py
--rw-r--r--   0        0        0      675 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/interface/build_phase.py
--rw-r--r--   0        0        0     2247 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/interface/context_interface.py
--rw-r--r--   0        0        0     1723 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/interface/phase_run_handler.py
--rw-r--r--   0        0        0      718 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/interface/step_inteface.py
--rw-r--r--   0        0        0      585 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/interface/time_source.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/__init__.py
--rw-r--r--   0        0        0     1895 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/__init__.py
--rw-r--r--   0        0        0      953 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py
--rw-r--r--   0        0        0     2067 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/__init__.py
--rw-r--r--   0        0        0     5057 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/__init__.py
--rw-r--r--   0        0        0     5944 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py
--rw-r--r--   0        0        0     1424 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/__init__.py
--rw-r--r--   0        0        0     2258 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py
--rw-r--r--   0        0        0     5399 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py
--rw-r--r--   0        0        0    10894 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py
--rw-r--r--   0        0        0     1186 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.398485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/__init__.py
--rw-r--r--   0        0        0      618 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py
--rw-r--r--   0        0        0     1599 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py
--rw-r--r--   0        0        0     9553 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py
--rw-r--r--   0        0        0     1244 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/build_logic/phases/phases_pipeline.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/build_logic/run_handlers/__init__.py
--rw-r--r--   0        0        0     3484 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/build_logic/tools/__init__.py
--rw-r--r--   0        0        0     2498 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/build_logic/tools/dependencies_tools.py
--rw-r--r--   0        0        0     8228 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/build_logic/tools/files.py
--rw-r--r--   0        0        0      750 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/build_logic/tools/ignore_files.py
--rw-r--r--   0        0        0      188 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/build_logic/tools/text.py
--rw-r--r--   0        0        0      200 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/build_logic/trigger_build_context.py
--rw-r--r--   0        0        0     1084 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/const.py
--rw-r--r--   0        0        0     1595 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0      242 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0     1136 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      414 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/instance_template/__init__.py
--rw-r--r--   0        0        0     1916 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/instance_template/verify_template_id.py
--rw-r--r--   0        0        0     2933 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0       70 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/provider.py
--rw-r--r--   0        0        0      281 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      545 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3830 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      361 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     6897 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      422 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0     1686 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/tool/protobuf_factory.py
--rw-r--r--   0        0        0      435 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      275 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     4200 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     7722 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/__init__.py
--rw-r--r--   0        0        0     4762 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/_entity_extraction.py
--rw-r--r--   0        0        0     1739 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      322 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      321 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/base.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1938 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/decorators/api.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/decorators/impl/__init__.py
--rw-r--r--   0        0        0      993 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/decorators/impl/api_implementation.py
--rw-r--r--   0        0        0      215 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/decorators/impl/timer_implementation.py
--rw-r--r--   0        0        0      739 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/decorators/timer.py
--rw-r--r--   0        0        0     1503 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0     1981 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/schema.py
--rw-r--r--   0        0        0     2411 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      786 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     2176 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0     1560 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2712 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      798 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0     2289 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2938 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5472 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0     1757 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/qwak_client/batch_jobs/execution.py
--rw-r--r--   0        0        0     1531 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/qwak_client/batch_jobs/task.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/qwak_client/build_api_helpers/__init__.py
--rw-r--r--   0        0        0     1886 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/qwak_client/build_api_helpers/build_api_steps.py
--rw-r--r--   0        0        0      184 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/qwak_client/build_api_helpers/messages.py
--rw-r--r--   0        0        0     2355 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/qwak_client/build_api_helpers/trigger_build_api.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.402485 qwak_core-0.4.7/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    26693 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/data_versioning/__init__.py
--rw-r--r--   0        0        0      806 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/data_versioning/data_tag.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13288 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/file_versioning/__init__.py
--rw-r--r--   0        0        0      806 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/file_versioning/file_tag.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0     1191 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2247 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9598 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/utils/__init__.py
--rw-r--r--   0        0        0      581 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/utils/datetime_utils.py
--rw-r--r--   0        0        0      120 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/vector_store/__init__.py
--rw-r--r--   0        0        0     6040 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/vector_store/client.py
--rw-r--r--   0        0        0    16916 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/vector_store/collection.py
--rw-r--r--   0        0        0     8209 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/vector_store/filters.py
--rw-r--r--   0        0        0     3711 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/vector_store/inference_client.py
--rw-r--r--   0        0        0     2658 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/vector_store/rest_helpers.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/vector_store/utils/__init__.py
--rw-r--r--   0        0        0      837 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/vector_store/utils/filter_utils.py
--rw-r--r--   0        0        0     7459 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak/vector_store/utils/upsert_utils.py
--rw-r--r--   0        0        0       46 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2263 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/alert_registry_service_api.py
--rw-r--r--   0        0        0     2129 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1189 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    13129 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3686 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     4984 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     1264 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py
--rw-r--r--   0        0        0     5226 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     2453 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    20753 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1608 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0      886 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/execution_management_service.py
--rw-r--r--   0        0        0     3207 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     3400 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3712 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     6800 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     2592 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     1635 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/fs_offline_serving_service.py
--rw-r--r--   0        0        0     4567 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/instance_template_management_service.py
--rw-r--r--   0        0        0     1046 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/internal_build_orchestrator_service.py
--rw-r--r--   0        0        0     2696 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     4153 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     5500 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0     5722 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/vector_serving_api.py
--rw-r--r--   0        0        0     3594 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/vectors_management_api.py
--rw-r--r--   0        0        0     7591 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/mocks/workspace_manager_service_mock.py
--rw-r--r--   0        0        0    17551 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2024-05-08 11:46:13.406485 qwak_core-0.4.7/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     7299 1970-01-01 00:00:00.000000 qwak_core-0.4.7/setup.py
--rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 qwak_core-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0      264 2024-05-08 13:07:26.534485 qwak_core-0.4.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 13:09:46.510589 qwak_core-0.4.8/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5877 2024-05-08 13:09:46.542591 qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     7824 2024-05-08 13:09:19.641029 qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.542591 qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0    12703 2024-05-08 13:09:46.546591 qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py
+-rw-r--r--   0        0        0    10914 2024-05-08 13:09:19.801038 qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi
+-rw-r--r--   0        0        0    14681 2024-05-08 13:09:46.546591 qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2024-05-08 13:09:46.534591 qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2024-05-08 13:09:19.317010 qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.538591 qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2024-05-08 13:09:46.538591 qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2024-05-08 13:09:19.473019 qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.542591 qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2024-05-08 13:09:46.526590 qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2024-05-08 13:09:18.824982 qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2024-05-08 13:09:46.530590 qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2024-05-08 13:09:46.530590 qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2024-05-08 13:09:18.988991 qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.530590 qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4901 2024-05-08 13:09:46.534591 qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5995 2024-05-08 13:09:19.149000 qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.534591 qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2024-05-08 13:09:46.510589 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2024-05-08 13:09:18.628970 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2024-05-08 13:09:46.514589 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7360 2024-05-08 13:09:46.514589 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0    11651 2024-05-08 13:09:19.965047 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.514589 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     5029 2024-05-08 13:09:46.518590 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     6943 2024-05-08 13:09:20.289066 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.522590 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2024-05-08 13:09:46.522590 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2024-05-08 13:09:20.461076 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2024-05-08 13:09:46.522590 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2024-05-08 13:09:46.514589 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2024-05-08 13:09:20.129057 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.518590 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6541 2024-05-08 13:09:46.526590 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10595 2024-05-08 13:09:20.629086 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.526590 qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0    15382 2024-05-08 13:09:46.582593 qwak_core-0.4.8/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    20668 2024-05-08 13:09:23.193234 qwak_core-0.4.8/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.586593 qwak_core-0.4.8/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2024-05-08 13:09:46.586593 qwak_core-0.4.8/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2024-05-08 13:09:23.361244 qwak_core-0.4.8/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2024-05-08 13:09:46.586593 qwak_core-0.4.8/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7616 2024-05-08 13:09:46.814607 qwak_core-0.4.8/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11995 2024-05-08 13:09:33.525832 qwak_core-0.4.8/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.818607 qwak_core-0.4.8/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0    14893 2024-05-08 13:09:46.818607 qwak_core-0.4.8/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0    11812 2024-05-08 13:09:33.713843 qwak_core-0.4.8/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    19155 2024-05-08 13:09:46.818607 qwak_core-0.4.8/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2024-05-08 13:09:46.822607 qwak_core-0.4.8/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2024-05-08 13:09:34.753904 qwak_core-0.4.8/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2024-05-08 13:09:46.826607 qwak_core-0.4.8/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8864 2024-05-08 13:09:46.822607 qwak_core-0.4.8/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13789 2024-05-08 13:09:34.577894 qwak_core-0.4.8/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.822607 qwak_core-0.4.8/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5777 2024-05-08 13:09:46.826607 qwak_core-0.4.8/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8264 2024-05-08 13:09:34.925914 qwak_core-0.4.8/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.826607 qwak_core-0.4.8/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2024-05-08 13:09:46.830608 qwak_core-0.4.8/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2024-05-08 13:09:35.089923 qwak_core-0.4.8/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2024-05-08 13:09:46.830608 qwak_core-0.4.8/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    14053 2024-05-08 13:09:46.950615 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    20860 2024-05-08 13:09:43.106391 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.950615 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5775 2024-05-08 13:09:46.946614 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     8308 2024-05-08 13:09:42.774371 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.946614 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3954 2024-05-08 13:09:46.946614 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     5309 2024-05-08 13:09:42.938381 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.950615 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    21176 2024-05-08 13:09:46.938614 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    15049 2024-05-08 13:09:42.422351 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    25475 2024-05-08 13:09:46.942614 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2024-05-08 13:09:46.942614 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2024-05-08 13:09:42.610362 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.942614 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2024-05-08 13:09:46.958615 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2024-05-08 13:09:43.598420 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.958615 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2024-05-08 13:09:46.954615 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2024-05-08 13:09:43.434410 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.954615 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2024-05-08 13:09:46.950615 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2024-05-08 13:09:43.274401 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.954615 qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    11218 2024-05-08 13:09:46.938614 qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    15584 2024-05-08 13:09:42.174337 qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.938614 qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2083 2024-05-08 13:09:46.930613 qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1977 2024-05-08 13:09:41.818316 qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.934614 qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    46028 2024-05-08 13:09:46.934614 qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    60013 2024-05-08 13:09:42.010327 qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    32008 2024-05-08 13:09:46.934614 qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    29124 2024-05-08 13:09:46.862609 qwak_core-0.4.8/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    24434 2024-05-08 13:09:36.862027 qwak_core-0.4.8/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    27837 2024-05-08 13:09:46.866610 qwak_core-0.4.8/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    33279 2024-05-08 13:09:46.862609 qwak_core-0.4.8/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    52325 2024-05-08 13:09:36.510006 qwak_core-0.4.8/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.862609 qwak_core-0.4.8/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0     5757 2024-05-08 13:09:46.870610 qwak_core-0.4.8/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py
+-rw-r--r--   0        0        0     4013 2024-05-08 13:09:37.378057 qwak_core-0.4.8/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi
+-rw-r--r--   0        0        0     6783 2024-05-08 13:09:46.870610 qwak_core-0.4.8/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py
+-rw-r--r--   0        0        0     6016 2024-05-08 13:09:46.866610 qwak_core-0.4.8/_qwak_proto/qwak/build_settings/build_settings_pb2.py
+-rw-r--r--   0        0        0     7049 2024-05-08 13:09:37.202046 qwak_core-0.4.8/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.870610 qwak_core-0.4.8/_qwak_proto/qwak/build_settings/build_settings_pb2_grpc.py
+-rw-r--r--   0        0        0    14991 2024-05-08 13:09:46.846608 qwak_core-0.4.8/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    24472 2024-05-08 13:09:36.329996 qwak_core-0.4.8/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.850609 qwak_core-0.4.8/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     5552 2024-05-08 13:09:46.850609 qwak_core-0.4.8/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     7299 2024-05-08 13:09:36.678016 qwak_core-0.4.8/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.850609 qwak_core-0.4.8/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    15672 2024-05-08 13:09:46.854609 qwak_core-0.4.8/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0    12741 2024-05-08 13:09:37.034037 qwak_core-0.4.8/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    16925 2024-05-08 13:09:46.854609 qwak_core-0.4.8/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38491 2024-05-08 13:09:46.858609 qwak_core-0.4.8/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    53557 2024-05-08 13:09:37.934089 qwak_core-0.4.8/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2024-05-08 13:09:46.858609 qwak_core-0.4.8/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     3508 2024-05-08 13:09:46.854609 qwak_core-0.4.8/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     2300 2024-05-08 13:09:37.550067 qwak_core-0.4.8/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0     3101 2024-05-08 13:09:46.858609 qwak_core-0.4.8/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2270 2024-05-08 13:09:46.878610 qwak_core-0.4.8/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     2697 2024-05-08 13:09:38.302111 qwak_core-0.4.8/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.878610 qwak_core-0.4.8/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4458 2024-05-08 13:09:46.878610 qwak_core-0.4.8/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     3113 2024-05-08 13:09:38.462120 qwak_core-0.4.8/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2024-05-08 13:09:46.882611 qwak_core-0.4.8/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2024-05-08 13:09:46.838608 qwak_core-0.4.8/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2024-05-08 13:09:35.825966 qwak_core-0.4.8/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.842608 qwak_core-0.4.8/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11871 2024-05-08 13:09:46.842608 qwak_core-0.4.8/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     8790 2024-05-08 13:09:35.993976 qwak_core-0.4.8/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2024-05-08 13:09:46.842608 qwak_core-0.4.8/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2024-05-08 13:09:46.834608 qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2024-05-08 13:09:35.481946 qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.834608 qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    50041 2024-05-08 13:09:46.830608 qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    74372 2024-05-08 13:09:35.301936 qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.834608 qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    46309 2024-05-08 13:09:46.838608 qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    40356 2024-05-08 13:09:35.661957 qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    27756 2024-05-08 13:09:46.838608 qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3345 2024-05-08 13:09:46.570592 qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     4098 2024-05-08 13:09:22.189176 qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.570592 qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12707 2024-05-08 13:09:46.574593 qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    13800 2024-05-08 13:09:22.393188 qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.574593 qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    17949 2024-05-08 13:09:46.574593 qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    18562 2024-05-08 13:09:22.605200 qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    12833 2024-05-08 13:09:46.578593 qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6463 2024-05-08 13:09:46.766604 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/backfill_pb2.py
+-rw-r--r--   0        0        0     7945 2024-05-08 13:09:28.929565 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.770604 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/backfill_pb2_grpc.py
+-rw-r--r--   0        0        0     2971 2024-05-08 13:09:46.770604 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/batch_pb2.py
+-rw-r--r--   0        0        0     3266 2024-05-08 13:09:29.097575 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.770604 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     2210 2024-05-08 13:09:46.774604 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/deletion_pb2.py
+-rw-r--r--   0        0        0     1540 2024-05-08 13:09:29.261584 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.774604 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/deletion_pb2_grpc.py
+-rw-r--r--   0        0        0     5793 2024-05-08 13:09:46.774604 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/execution_pb2.py
+-rw-r--r--   0        0        0     7373 2024-05-08 13:09:29.421594 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.778605 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    14900 2024-05-08 13:09:46.778605 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/execution_service_pb2.py
+-rw-r--r--   0        0        0    11103 2024-05-08 13:09:29.597604 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi
+-rw-r--r--   0        0        0    17220 2024-05-08 13:09:46.778605 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7695 2024-05-08 13:09:46.782605 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py
+-rw-r--r--   0        0        0    14959 2024-05-08 13:09:30.557659 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.786605 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0    19304 2024-05-08 13:09:46.786605 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0    16916 2024-05-08 13:09:30.737670 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    21145 2024-05-08 13:09:46.786605 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8440 2024-05-08 13:09:46.782605 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py
+-rw-r--r--   0        0        0    13312 2024-05-08 13:09:30.341647 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.782605 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     2051 2024-05-08 13:09:46.790605 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py
+-rw-r--r--   0        0        0     1952 2024-05-08 13:09:30.937681 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.790605 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/execution_state_pb2_grpc.py
+-rw-r--r--   0        0        0    12222 2024-05-08 13:09:46.790605 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py
+-rw-r--r--   0        0        0     7930 2024-05-08 13:09:31.121692 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi
+-rw-r--r--   0        0        0    14212 2024-05-08 13:09:46.794606 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1685 2024-05-08 13:09:46.794606 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py
+-rw-r--r--   0        0        0     1272 2024-05-08 13:09:31.285701 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.794606 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2_grpc.py
+-rw-r--r--   0        0        0     6198 2024-05-08 13:09:46.798606 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py
+-rw-r--r--   0        0        0     7677 2024-05-08 13:09:31.441711 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.798606 qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2024-05-08 13:09:46.738602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2024-05-08 13:09:28.765556 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.742602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2024-05-08 13:09:46.734602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2024-05-08 13:09:28.605546 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2024-05-08 13:09:46.738602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11432 2024-05-08 13:09:46.706601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    12882 2024-05-08 13:09:26.209408 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.706601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0    13825 2024-05-08 13:09:46.718601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/deployment_pb2.py
+-rw-r--r--   0        0        0    19227 2024-05-08 13:09:27.521484 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.722601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     3307 2024-05-08 13:09:46.722601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py
+-rw-r--r--   0        0        0     1637 2024-05-08 13:09:27.725496 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0     3293 2024-05-08 13:09:46.722601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5303 2024-05-08 13:09:46.702600 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8604 2024-05-08 13:09:25.997396 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.702600 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2024-05-08 13:09:46.694600 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2024-05-08 13:09:25.465365 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.694600 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    28920 2024-05-08 13:09:46.698600 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20665 2024-05-08 13:09:25.837386 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    35307 2024-05-08 13:09:46.698600 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2024-05-08 13:09:46.706601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2024-05-08 13:09:26.837444 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.710601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2024-05-08 13:09:46.710601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2024-05-08 13:09:27.025455 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2024-05-08 13:09:46.710601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    26853 2024-05-08 13:09:46.694600 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    39247 2024-05-08 13:09:25.641375 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.698600 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2024-05-08 13:09:46.714601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2024-05-08 13:09:27.185464 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.714601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0    13240 2024-05-08 13:09:46.714601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py
+-rw-r--r--   0        0        0    18420 2024-05-08 13:09:27.361475 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.718601 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2024-05-08 13:09:46.742602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2024-05-08 13:09:45.386524 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.742602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2024-05-08 13:09:46.746603 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2024-05-08 13:09:45.646539 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2024-05-08 13:09:46.746603 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4308 2024-05-08 13:09:46.746603 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     7410 2024-05-08 13:09:33.005802 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.750603 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    15316 2024-05-08 13:09:46.750603 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    14087 2024-05-08 13:09:33.173812 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    18465 2024-05-08 13:09:46.750603 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2024-05-08 13:09:46.754603 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2024-05-08 13:09:33.341821 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.754603 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     5111 2024-05-08 13:09:46.766604 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/management_pb2.py
+-rw-r--r--   0        0        0     2739 2024-05-08 13:09:34.401883 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi
+-rw-r--r--   0        0        0     5436 2024-05-08 13:09:46.766604 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py
+-rw-r--r--   0        0        0     5385 2024-05-08 13:09:46.758603 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     7551 2024-05-08 13:09:34.049863 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.758603 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    17474 2024-05-08 13:09:46.754603 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2024-05-08 13:09:33.877853 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2024-05-08 13:09:46.758603 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2024-05-08 13:09:46.762604 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2024-05-08 13:09:34.217872 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.762604 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    27355 2024-05-08 13:09:46.726602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    43393 2024-05-08 13:09:27.893505 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.726602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5147 2024-05-08 13:09:46.726602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6208 2024-05-08 13:09:28.065515 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.730602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2024-05-08 13:09:46.730602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2024-05-08 13:09:28.237525 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2024-05-08 13:09:46.730602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11049 2024-05-08 13:09:46.734602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15942 2024-05-08 13:09:28.409535 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.734602 qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2024-05-08 13:09:46.966616 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2024-05-08 13:09:44.294460 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.970616 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2024-05-08 13:09:46.970616 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2024-05-08 13:09:44.474471 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2024-05-08 13:09:46.970616 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2024-05-08 13:09:46.974616 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2024-05-08 13:09:44.646481 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.974616 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2024-05-08 13:09:46.974616 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2024-05-08 13:09:44.822491 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2024-05-08 13:09:46.978616 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10469 2024-05-08 13:09:46.978616 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0    11719 2024-05-08 13:09:45.022503 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     9458 2024-05-08 13:09:46.978616 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5302 2024-05-08 13:09:46.982616 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     5484 2024-05-08 13:09:45.190513 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.982616 qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2975 2024-05-08 13:09:46.882611 qwak_core-0.4.8/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     4026 2024-05-08 13:09:38.638130 qwak_core-0.4.8/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.886611 qwak_core-0.4.8/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4455 2024-05-08 13:09:46.886611 qwak_core-0.4.8/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     3113 2024-05-08 13:09:38.814141 qwak_core-0.4.8/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2024-05-08 13:09:46.886611 qwak_core-0.4.8/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6950 2024-05-08 13:09:46.590594 qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    11560 2024-05-08 13:09:24.509310 qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.590594 qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     3442 2024-05-08 13:09:46.650597 qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     5719 2024-05-08 13:09:24.689320 qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.654597 qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2024-05-08 13:09:46.654597 qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2024-05-08 13:09:24.889332 qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2024-05-08 13:09:46.654597 qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8504 2024-05-08 13:09:46.658598 qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12440 2024-05-08 13:09:25.049341 qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.690600 qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2024-05-08 13:09:46.846608 qwak_core-0.4.8/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2024-05-08 13:09:36.161986 qwak_core-0.4.8/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2024-05-08 13:09:46.846608 qwak_core-0.4.8/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     3876 2024-05-08 13:09:46.890611 qwak_core-0.4.8/_qwak_proto/qwak/instance_template/instance_template_pb2.py
+-rw-r--r--   0        0        0     4658 2024-05-08 13:09:39.002152 qwak_core-0.4.8/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.890611 qwak_core-0.4.8/_qwak_proto/qwak/instance_template/instance_template_pb2_grpc.py
+-rw-r--r--   0        0        0     4722 2024-05-08 13:09:46.890611 qwak_core-0.4.8/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py
+-rw-r--r--   0        0        0     3245 2024-05-08 13:09:39.166161 qwak_core-0.4.8/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi
+-rw-r--r--   0        0        0     5240 2024-05-08 13:09:46.894611 qwak_core-0.4.8/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2024-05-08 13:09:46.906612 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2024-05-08 13:09:40.210222 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.910612 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2024-05-08 13:09:46.910612 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2024-05-08 13:09:40.374231 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.910612 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    25218 2024-05-08 13:09:46.914612 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    31280 2024-05-08 13:09:40.566243 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.914612 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13432 2024-05-08 13:09:46.914612 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    22974 2024-05-08 13:09:40.738253 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.918613 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12784 2024-05-08 13:09:46.918613 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16585 2024-05-08 13:09:40.910263 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.918613 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    51171 2024-05-08 13:09:46.922613 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    40800 2024-05-08 13:09:41.138276 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    73869 2024-05-08 13:09:46.922613 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2024-05-08 13:09:46.922613 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2024-05-08 13:09:41.302286 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.926613 qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2024-05-08 13:09:46.898611 qwak_core-0.4.8/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2024-05-08 13:09:39.502181 qwak_core-0.4.8/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.898611 qwak_core-0.4.8/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2024-05-08 13:09:46.906612 qwak_core-0.4.8/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2024-05-08 13:09:40.026211 qwak_core-0.4.8/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.906612 qwak_core-0.4.8/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2024-05-08 13:09:46.898611 qwak_core-0.4.8/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2024-05-08 13:09:39.694192 qwak_core-0.4.8/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2024-05-08 13:09:46.902612 qwak_core-0.4.8/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10138 2024-05-08 13:09:46.902612 qwak_core-0.4.8/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    14337 2024-05-08 13:09:39.862202 qwak_core-0.4.8/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.902612 qwak_core-0.4.8/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    27866 2024-05-08 13:09:46.874610 qwak_core-0.4.8/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    32184 2024-05-08 13:09:38.118100 qwak_core-0.4.8/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    19830 2024-05-08 13:09:46.874610 qwak_core-0.4.8/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2024-05-08 13:09:46.562592 qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2024-05-08 13:09:23.925276 qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2024-05-08 13:09:46.566592 qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2024-05-08 13:09:46.562592 qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2024-05-08 13:09:23.621259 qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.562592 qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2024-05-08 13:09:46.566592 qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2024-05-08 13:09:24.269296 qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2024-05-08 13:09:46.566592 qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1598 2024-05-08 13:09:46.958615 qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py
+-rw-r--r--   0        0        0     1221 2024-05-08 13:09:43.778430 qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.962615 qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2_grpc.py
+-rw-r--r--   0        0        0    11437 2024-05-08 13:09:46.966616 qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py
+-rw-r--r--   0        0        0    12170 2024-05-08 13:09:44.118450 qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi
+-rw-r--r--   0        0        0     9793 2024-05-08 13:09:46.966616 qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4060 2024-05-08 13:09:46.962615 qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/population_pb2.py
+-rw-r--r--   0        0        0     3906 2024-05-08 13:09:43.946440 qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.962615 qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/population_pb2_grpc.py
+-rw-r--r--   0        0        0    10804 2024-05-08 13:09:46.870610 qwak_core-0.4.8/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0    12120 2024-05-08 13:09:37.754079 qwak_core-0.4.8/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     9642 2024-05-08 13:09:46.874610 qwak_core-0.4.8/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2024-05-08 13:09:46.894611 qwak_core-0.4.8/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2024-05-08 13:09:39.342171 qwak_core-0.4.8/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2024-05-08 13:09:46.894611 qwak_core-0.4.8/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10718 2024-05-08 13:09:46.558592 qwak_core-0.4.8/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0    12627 2024-05-08 13:09:21.485135 qwak_core-0.4.8/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.558592 qwak_core-0.4.8/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    19751 2024-05-08 13:09:46.554592 qwak_core-0.4.8/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    13467 2024-05-08 13:09:21.317125 qwak_core-0.4.8/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    24352 2024-05-08 13:09:46.558592 qwak_core-0.4.8/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2024-05-08 13:09:46.546591 qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2024-05-08 13:09:20.793095 qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.550591 qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2477 2024-05-08 13:09:46.550591 qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2679 2024-05-08 13:09:20.957105 qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.550591 qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2024-05-08 13:09:46.554592 qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2024-05-08 13:09:21.117114 qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2024-05-08 13:09:46.554592 qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6909 2024-05-08 13:09:46.930613 qwak_core-0.4.8/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     5186 2024-05-08 13:09:41.642305 qwak_core-0.4.8/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2024-05-08 13:09:46.930613 qwak_core-0.4.8/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7868 2024-05-08 13:09:46.926613 qwak_core-0.4.8/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    12177 2024-05-08 13:09:41.478296 qwak_core-0.4.8/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.926613 qwak_core-0.4.8/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0    11396 2024-05-08 13:09:46.578593 qwak_core-0.4.8/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0    15139 2024-05-08 13:09:22.813212 qwak_core-0.4.8/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.578593 qwak_core-0.4.8/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     3645 2024-05-08 13:09:46.582593 qwak_core-0.4.8/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2983 2024-05-08 13:09:23.021224 qwak_core-0.4.8/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.582593 qwak_core-0.4.8/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     8648 2024-05-08 13:09:46.802606 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py
+-rw-r--r--   0        0        0    12852 2024-05-08 13:09:31.777730 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.802606 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/collection_pb2_grpc.py
+-rw-r--r--   0        0        0    13830 2024-05-08 13:09:46.806606 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py
+-rw-r--r--   0        0        0    10297 2024-05-08 13:09:31.949740 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi
+-rw-r--r--   0        0        0    17183 2024-05-08 13:09:46.806606 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1873 2024-05-08 13:09:46.798606 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py
+-rw-r--r--   0        0        0     1550 2024-05-08 13:09:31.609720 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.802606 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2_grpc.py
+-rw-r--r--   0        0        0     8996 2024-05-08 13:09:46.806606 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/filters_pb2.py
+-rw-r--r--   0        0        0    11380 2024-05-08 13:09:32.133751 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.810606 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/filters_pb2_grpc.py
+-rw-r--r--   0        0        0     4533 2024-05-08 13:09:46.810606 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/vector_pb2.py
+-rw-r--r--   0        0        0     6103 2024-05-08 13:09:32.309761 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.810606 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/vector_pb2_grpc.py
+-rw-r--r--   0        0        0     9738 2024-05-08 13:09:46.814607 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py
+-rw-r--r--   0        0        0    10977 2024-05-08 13:09:32.481771 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi
+-rw-r--r--   0        0        0    10157 2024-05-08 13:09:46.814607 qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10852 2024-05-08 13:09:46.982616 qwak_core-0.4.8/_qwak_proto/qwak/workspace/workspace_pb2.py
+-rw-r--r--   0        0        0    17043 2024-05-08 13:09:45.886553 qwak_core-0.4.8/_qwak_proto/qwak/workspace/workspace_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-08 13:09:46.986617 qwak_core-0.4.8/_qwak_proto/qwak/workspace/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0    21429 2024-05-08 13:09:46.986617 qwak_core-0.4.8/_qwak_proto/qwak/workspace/workspace_service_pb2.py
+-rw-r--r--   0        0        0    13726 2024-05-08 13:09:46.078564 qwak_core-0.4.8/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi
+-rw-r--r--   0        0        0    27193 2024-05-08 13:09:46.986617 qwak_core-0.4.8/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3696 2024-05-08 13:09:58.787298 qwak_core-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0      585 2024-05-08 13:09:58.791298 qwak_core-0.4.8/qwak/__init__.py
+-rw-r--r--   0        0        0     1522 2024-05-08 13:07:26.534485 qwak_core-0.4.8/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3228 2024-05-08 13:07:26.534485 qwak_core-0.4.8/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    12456 2024-05-08 13:07:26.534485 qwak_core-0.4.8/qwak/automations/automations.py
+-rw-r--r--   0        0        0    12907 2024-05-08 13:07:26.534485 qwak_core-0.4.8/qwak/automations/batch_execution_action.py
+-rw-r--r--   0        0        0    26800 2024-05-08 13:07:26.534485 qwak_core-0.4.8/qwak/automations/build_and_deploy_action.py
+-rw-r--r--   0        0        0     2404 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/automations/common.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/_inner/__init__.py
+-rw-r--r--   0        0        0      849 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/_inner/edge_communications.py
+-rw-r--r--   0        0        0      224 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5340 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       43 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/alerts_registry/__init__.py
+-rw-r--r--   0        0        0     4040 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/alerts_registry/channel.py
+-rw-r--r--   0        0        0     5355 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/alerts_registry/client.py
+-rw-r--r--   0        0        0       42 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     9034 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    21054 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6882 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4209 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0      105 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0     5119 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/build_orchestrator/build_model_request_getter.py
+-rw-r--r--   0        0        0    16148 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0     3981 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/build_orchestrator/internal_client.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     2401 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0      885 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/data_versioning/data_tag_filter.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6806 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     4051 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/feature_store/execution_management_client.py
+-rw-r--r--   0        0        0     2635 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    16056 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     8022 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/feature_store/offline_serving_client.py
+-rw-r--r--   0        0        0     5811 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     2505 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0      885 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/file_versioning/file_tag_filter.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/instance_template/__init__.py
+-rw-r--r--   0        0        0     2509 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/instance_template/client.py
+-rw-r--r--   0        0        0       41 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9308 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     4431 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3581 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      102 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/vector_store/__init__.py
+-rw-r--r--   0        0        0     4247 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/vector_store/management_client.py
+-rw-r--r--   0        0        0     5293 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/vector_store/serving_client.py
+-rw-r--r--   0        0        0       43 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/workspace_manager/__init__.py
+-rw-r--r--   0        0        0     8136 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/clients/workspace_manager/client.py
+-rw-r--r--   0        0        0      790 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      192 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      424 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/qwak_general_build_exception.py
+-rw-r--r--   0        0        0      579 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0       54 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/qwak_load_configuration_exception.py
+-rw-r--r--   0        0        0      274 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      137 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/qwak_remote_build_failed.py
+-rw-r--r--   0        0        0      746 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/exceptions/qwak_suggestion_exception.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     1977 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/feature_store/_common/artifact_utils.py
+-rw-r--r--   0        0        0     7046 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/feature_store/_common/feature_set_utils.py
+-rw-r--r--   0        0        0     4707 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     6680 2024-05-08 13:07:26.538485 qwak_core-0.4.8/qwak/feature_store/_common/packaging.py
+-rw-r--r--   0        0        0     2316 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0     2694 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/base.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/_batch.py
+-rw-r--r--   0        0        0      658 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/_jdbc.py
+-rw-r--r--   0        0        0    10805 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/athena.py
+-rw-r--r--   0        0        0     3022 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/big_query.py
+-rw-r--r--   0        0        0     2063 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/clickhouse.py
+-rw-r--r--   0        0        0     1981 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/csv.py
+-rw-r--r--   0        0        0     2130 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/elastic_search.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/filesystem/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/filesystem/aws.py
+-rw-r--r--   0        0        0      245 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/filesystem/base_config.py
+-rw-r--r--   0        0        0     1572 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/filesystem/gcp.py
+-rw-r--r--   0        0        0     1874 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/filesystem/utils.py
+-rw-r--r--   0        0        0     1921 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/mongodb.py
+-rw-r--r--   0        0        0     1595 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/mysql.py
+-rw-r--r--   0        0        0     1867 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/parquet.py
+-rw-r--r--   0        0        0     1648 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/postgres.py
+-rw-r--r--   0        0        0     3114 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/redshift.py
+-rw-r--r--   0        0        0     2579 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/snowflake.py
+-rw-r--r--   0        0        0     1830 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/batch/vertica.py
+-rw-r--r--   0        0        0      895 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/source_authentication.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/streaming/__init__.py
+-rw-r--r--   0        0        0      181 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/streaming/_streaming.py
+-rw-r--r--   0        0        0      649 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/streaming/kafka/__init__.py
+-rw-r--r--   0        0        0     3959 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/streaming/kafka/authentication.py
+-rw-r--r--   0        0        0     3510 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/streaming/kafka/deserialization.py
+-rw-r--r--   0        0        0     4398 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/streaming/kafka/kafka.py
+-rw-r--r--   0        0        0     5984 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/data_sources/time_partition_columns.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     2313 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/execution/__init__.py
+-rw-r--r--   0        0        0     6470 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/execution/backfill.py
+-rw-r--r--   0        0        0    21243 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/execution/execution.py
+-rw-r--r--   0        0        0     3564 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/execution/execution_query.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1636 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/_utils/_featureset_utils.py
+-rw-r--r--   0        0        0     1979 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0     5285 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/base_feature_set.py
+-rw-r--r--   0        0        0    16910 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1670 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0     1155 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0    23233 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/streaming.py
+-rw-r--r--   0        0        0     9584 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/streaming_backfill.py
+-rw-r--r--   0        0        0      733 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/aggregations/__init__.py
+-rw-r--r--   0        0        0    14117 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py
+-rw-r--r--   0        0        0     2253 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/aggregations/windows.py
+-rw-r--r--   0        0        0      281 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/functions/__init__.py
+-rw-r--r--   0        0        0     2425 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py
+-rw-r--r--   0        0        0     1156 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/functions/schema.py
+-rw-r--r--   0        0        0     9659 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/transformations.py
+-rw-r--r--   0        0        0      173 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0     1216 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/offline/_offline_serving_validations.py
+-rw-r--r--   0        0        0      738 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28651 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0    12597 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/offline/client_v2.py
+-rw-r--r--   0        0        0      739 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/offline/feature_set_features.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0    11144 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0     2210 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/online/endpoint_utils.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/validations/__init__.py
+-rw-r--r--   0        0        0     2656 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/validations/validation_options.py
+-rw-r--r--   0        0        0     3783 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/validations/validation_response.py
+-rw-r--r--   0        0        0     3864 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/feature_store/validations/validator.py
+-rw-r--r--   0        0        0      226 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_config/__init__.py
+-rw-r--r--   0        0        0    11232 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_config/build_config_v1.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/build_loggers/__init__.py
+-rw-r--r--   0        0        0     1426 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/build_loggers/trigger_build_logger.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/constants/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/constants/dependencies.py
+-rw-r--r--   0        0        0      131 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/constants/host_resource.py
+-rw-r--r--   0        0        0       94 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/constants/messages.py
+-rw-r--r--   0        0        0       36 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/constants/temp_dir.py
+-rw-r--r--   0        0        0      279 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/constants/upload_tag.py
+-rw-r--r--   0        0        0      116 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/dependency_manager_type.py
+-rw-r--r--   0        0        0     2299 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/execute_build_pipeline.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/interface/__init__.py
+-rw-r--r--   0        0        0      528 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/interface/build_logger_interface.py
+-rw-r--r--   0        0        0      675 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/interface/build_phase.py
+-rw-r--r--   0        0        0     2247 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/interface/context_interface.py
+-rw-r--r--   0        0        0     1723 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/interface/phase_run_handler.py
+-rw-r--r--   0        0        0      718 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/interface/step_inteface.py
+-rw-r--r--   0        0        0      585 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/interface/time_source.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/phases/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.542485 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/__init__.py
+-rw-r--r--   0        0        0     1895 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/__init__.py
+-rw-r--r--   0        0        0      953 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py
+-rw-r--r--   0        0        0     2067 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/__init__.py
+-rw-r--r--   0        0        0     5057 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/__init__.py
+-rw-r--r--   0        0        0     5944 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py
+-rw-r--r--   0        0        0     1424 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/__init__.py
+-rw-r--r--   0        0        0     2258 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py
+-rw-r--r--   0        0        0     5399 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py
+-rw-r--r--   0        0        0    10894 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py
+-rw-r--r--   0        0        0     1186 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/__init__.py
+-rw-r--r--   0        0        0      618 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py
+-rw-r--r--   0        0        0     1599 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py
+-rw-r--r--   0        0        0     9553 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py
+-rw-r--r--   0        0        0     1244 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/phases/phases_pipeline.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/run_handlers/__init__.py
+-rw-r--r--   0        0        0     3484 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/tools/__init__.py
+-rw-r--r--   0        0        0     2498 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/tools/dependencies_tools.py
+-rw-r--r--   0        0        0     8228 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/tools/files.py
+-rw-r--r--   0        0        0      750 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/tools/ignore_files.py
+-rw-r--r--   0        0        0      188 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/tools/text.py
+-rw-r--r--   0        0        0      200 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/build_logic/trigger_build_context.py
+-rw-r--r--   0        0        0     1084 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/const.py
+-rw-r--r--   0        0        0     1595 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0      242 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0     1136 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      414 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/instance_template/__init__.py
+-rw-r--r--   0        0        0     1916 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/instance_template/verify_template_id.py
+-rw-r--r--   0        0        0     2933 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0       70 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/provider.py
+-rw-r--r--   0        0        0      281 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      545 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3830 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      361 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     6897 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      422 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0     1686 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/tool/protobuf_factory.py
+-rw-r--r--   0        0        0      435 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      275 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     4200 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     7722 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/__init__.py
+-rw-r--r--   0        0        0     4762 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/_entity_extraction.py
+-rw-r--r--   0        0        0     1739 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      322 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      321 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1938 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/decorators/impl/__init__.py
+-rw-r--r--   0        0        0      993 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/decorators/impl/api_implementation.py
+-rw-r--r--   0        0        0      215 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/decorators/impl/timer_implementation.py
+-rw-r--r--   0        0        0      739 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/decorators/timer.py
+-rw-r--r--   0        0        0     1503 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0     1981 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/schema.py
+-rw-r--r--   0        0        0     2411 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      786 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     2176 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0     1560 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2712 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      798 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0     2289 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2938 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5472 2024-05-08 13:07:26.546486 qwak_core-0.4.8/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0     1757 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/batch_jobs/execution.py
+-rw-r--r--   0        0        0     1531 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/batch_jobs/task.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/build_api_helpers/__init__.py
+-rw-r--r--   0        0        0     1886 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/build_api_helpers/build_api_steps.py
+-rw-r--r--   0        0        0      184 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/build_api_helpers/messages.py
+-rw-r--r--   0        0        0     2355 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/build_api_helpers/trigger_build_api.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    26693 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/data_versioning/__init__.py
+-rw-r--r--   0        0        0      806 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/data_versioning/data_tag.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13288 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/file_versioning/__init__.py
+-rw-r--r--   0        0        0      806 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/file_versioning/file_tag.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0     1191 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/utils/__init__.py
+-rw-r--r--   0        0        0      581 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/utils/datetime_utils.py
+-rw-r--r--   0        0        0      120 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/vector_store/__init__.py
+-rw-r--r--   0        0        0     6040 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/vector_store/client.py
+-rw-r--r--   0        0        0    16916 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/vector_store/collection.py
+-rw-r--r--   0        0        0     8209 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/vector_store/filters.py
+-rw-r--r--   0        0        0     3711 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/vector_store/inference_client.py
+-rw-r--r--   0        0        0     2658 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/vector_store/rest_helpers.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/vector_store/utils/__init__.py
+-rw-r--r--   0        0        0      837 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/vector_store/utils/filter_utils.py
+-rw-r--r--   0        0        0     7459 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak/vector_store/utils/upsert_utils.py
+-rw-r--r--   0        0        0       46 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2263 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/alert_registry_service_api.py
+-rw-r--r--   0        0        0     2129 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1189 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    13129 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3686 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     4984 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     1264 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py
+-rw-r--r--   0        0        0     5226 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     2453 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    20753 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1608 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0      886 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/execution_management_service.py
+-rw-r--r--   0        0        0     3207 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     3400 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3712 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     6800 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     2592 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     1635 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/fs_offline_serving_service.py
+-rw-r--r--   0        0        0     4567 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/instance_template_management_service.py
+-rw-r--r--   0        0        0     1046 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/internal_build_orchestrator_service.py
+-rw-r--r--   0        0        0     2696 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     4153 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     5500 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0     5722 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/vector_serving_api.py
+-rw-r--r--   0        0        0     3594 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/vectors_management_api.py
+-rw-r--r--   0        0        0     7591 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/mocks/workspace_manager_service_mock.py
+-rw-r--r--   0        0        0    17551 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2024-05-08 13:07:26.550486 qwak_core-0.4.8/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     7299 1970-01-01 00:00:00.000000 qwak_core-0.4.8/setup.py
+-rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 qwak_core-0.4.8/PKG-INFO
```

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/build_settings/build_settings_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/build_settings/build_settings_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/build_settings/build_settings_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/build_settings/build_settings_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/build_settings/build_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/build_settings/build_settings_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/builds/internal_builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/backfill_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/backfill_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/backfill_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/batch_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/batch_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/deletion_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/deletion_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/deletion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/execution_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/execution_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/execution_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/execution_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/execution_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/execution_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/jobs/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/execution_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/execution_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/featureset_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/execution/v1/state/spark_execution_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/deployment_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/features/real_time_feature_extractor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/management_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/management_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/management_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/management_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/instance_template/instance_template_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/instance_template/instance_template_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/instance_template/instance_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/instance_template/instance_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/instance_template/instance_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/instance_template/instance_template_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/feature_values_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/offline_serving_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/population_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/population_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/offline/serving/v1/population_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/collection_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/collection_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/collection/event/collection_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/filters_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/filters_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/filters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/vector_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/vector_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/vector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/vector_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/vector_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/vectors/v1/vector_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/workspace/workspace_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/workspace/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/workspace/workspace_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/workspace/workspace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/workspace/workspace_service_pb2.py` & `qwak_core-0.4.8/_qwak_proto/qwak/workspace/workspace_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi` & `qwak_core-0.4.8/_qwak_proto/qwak/workspace/workspace_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py` & `qwak_core-0.4.8/_qwak_proto/qwak/workspace/workspace_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/pyproject.toml` & `qwak_core-0.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.4.7"
+version = "0.4.8"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.4.7/qwak/__init__.py` & `qwak_core-0.4.8/qwak/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for qwak-core."""
 
 __author__ = "Qwak.ai"
-__version__ = "0.4.7"
+__version__ = "0.4.8"
 
 from qwak.inner.di_configuration import wire_dependencies
 from qwak.model.experiment_tracking import log_metric, log_param
 from qwak.model_loggers.artifact_logger import load_file, log_file
 from qwak.model_loggers.data_logger import load_data, log_data
 from qwak.model_loggers.model_logger import load_model, log_model
```

### Comparing `qwak_core-0.4.7/qwak/automations/__init__.py` & `qwak_core-0.4.8/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/automations/automation_executions.py` & `qwak_core-0.4.8/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/automations/automations.py` & `qwak_core-0.4.8/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/automations/batch_execution_action.py` & `qwak_core-0.4.8/qwak/automations/batch_execution_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/automations/build_and_deploy_action.py` & `qwak_core-0.4.8/qwak/automations/build_and_deploy_action.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/automations/common.py` & `qwak_core-0.4.8/qwak/automations/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/_inner/edge_communications.py` & `qwak_core-0.4.8/qwak/clients/_inner/edge_communications.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.4.8/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/administration/authentication/client.py` & `qwak_core-0.4.8/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.4.8/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/administration/environment/client.py` & `qwak_core-0.4.8/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/administration/self_service/client.py` & `qwak_core-0.4.8/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/alert_management/client.py` & `qwak_core-0.4.8/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/alerts_registry/channel.py` & `qwak_core-0.4.8/qwak/clients/alerts_registry/channel.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/alerts_registry/client.py` & `qwak_core-0.4.8/qwak/clients/alerts_registry/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/analytics/client.py` & `qwak_core-0.4.8/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/audience/client.py` & `qwak_core-0.4.8/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/automation_management/client.py` & `qwak_core-0.4.8/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/autoscaling/client.py` & `qwak_core-0.4.8/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/batch_job_management/client.py` & `qwak_core-0.4.8/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.4.8/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/batch_job_management/results.py` & `qwak_core-0.4.8/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/build_management/client.py` & `qwak_core-0.4.8/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/build_orchestrator/build_model_request_getter.py` & `qwak_core-0.4.8/qwak/clients/build_orchestrator/build_model_request_getter.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             build_config_url=build_config_url,
             qwak_sdk_wheel_url=qwak_sdk_wheel_url,
             qwak_sdk_version_url=qwak_sdk_version_url,
         ),
         build_v1_flag=build_v1_flag,
         build_steps=build_steps,
         purchase_option=_purchase_option_to_enum(build_conf.purchase_option),
-        provision_instance_timeout=build_conf.provision_timeout,
+        provision_instance_timeout=build_conf.provision_instance_timeout,
     )
 
     if build_conf.build_env.remote.resources.instance:
         build_spec.client_pod_compute_resources.template_spec.CopyFrom(
             PodComputeResourceTemplateSpec(
                 template_id=build_conf.build_env.remote.resources.instance
             )
```

### Comparing `qwak_core-0.4.7/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.4.8/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/build_orchestrator/internal_client.py` & `qwak_core-0.4.8/qwak/clients/build_orchestrator/internal_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/data_versioning/client.py` & `qwak_core-0.4.8/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/data_versioning/data_tag_filter.py` & `qwak_core-0.4.8/qwak/clients/data_versioning/data_tag_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/deployment/client.py` & `qwak_core-0.4.8/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/feature_store/execution_management_client.py` & `qwak_core-0.4.8/qwak/clients/feature_store/execution_management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.4.8/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/feature_store/management_client.py` & `qwak_core-0.4.8/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/feature_store/offline_serving_client.py` & `qwak_core-0.4.8/qwak/clients/feature_store/offline_serving_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.4.8/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/file_versioning/client.py` & `qwak_core-0.4.8/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/file_versioning/file_tag_filter.py` & `qwak_core-0.4.8/qwak/clients/file_versioning/file_tag_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/instance_template/client.py` & `qwak_core-0.4.8/qwak/clients/instance_template/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.4.8/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/logging_client/client.py` & `qwak_core-0.4.8/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/model_management/client.py` & `qwak_core-0.4.8/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/project/client.py` & `qwak_core-0.4.8/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/secret_service/client.py` & `qwak_core-0.4.8/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/user_application_instance/client.py` & `qwak_core-0.4.8/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/vector_store/management_client.py` & `qwak_core-0.4.8/qwak/clients/vector_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/vector_store/serving_client.py` & `qwak_core-0.4.8/qwak/clients/vector_store/serving_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/clients/workspace_manager/client.py` & `qwak_core-0.4.8/qwak/clients/workspace_manager/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/exceptions/__init__.py` & `qwak_core-0.4.8/qwak/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/exceptions/quiet_error.py` & `qwak_core-0.4.8/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.4.8/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/exceptions/qwak_suggestion_exception.py` & `qwak_core-0.4.8/qwak/exceptions/qwak_suggestion_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/_common/artifact_utils.py` & `qwak_core-0.4.8/qwak/feature_store/_common/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/_common/feature_set_utils.py` & `qwak_core-0.4.8/qwak/feature_store/_common/feature_set_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.4.8/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/_common/functions.py` & `qwak_core-0.4.8/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/_common/packaging.py` & `qwak_core-0.4.8/qwak/feature_store/_common/packaging.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/base.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/_jdbc.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/athena.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/athena.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/big_query.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/clickhouse.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/clickhouse.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/csv.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/elastic_search.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/filesystem/aws.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/filesystem/aws.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/filesystem/gcp.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/filesystem/gcp.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/filesystem/utils.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/filesystem/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/mongodb.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/mysql.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/parquet.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/postgres.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/redshift.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/snowflake.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/batch/vertica.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/batch/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/source_authentication.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/source_authentication.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/streaming/kafka/__init__.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/streaming/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/streaming/kafka/authentication.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/streaming/kafka/authentication.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/streaming/kafka/deserialization.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/streaming/kafka/deserialization.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/streaming/kafka/kafka.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/streaming/kafka/kafka.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/data_sources/time_partition_columns.py` & `qwak_core-0.4.8/qwak/feature_store/data_sources/time_partition_columns.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/entities/entity.py` & `qwak_core-0.4.8/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/execution/backfill.py` & `qwak_core-0.4.8/qwak/feature_store/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/execution/execution.py` & `qwak_core-0.4.8/qwak/feature_store/execution/execution.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/execution/execution_query.py` & `qwak_core-0.4.8/qwak/feature_store/execution/execution_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/_utils/_featureset_utils.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/_utils/_featureset_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/base_feature_set.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/base_feature_set.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/streaming.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/streaming.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/streaming_backfill.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/streaming_backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/__init__.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/aggregations/aggregations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/aggregations/windows.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/aggregations/windows.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/functions/qwak_pandas.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/functions/schema.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/functions/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/feature_sets/transformations/transformations.py` & `qwak_core-0.4.8/qwak/feature_store/feature_sets/transformations/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/offline/_offline_serving_validations.py` & `qwak_core-0.4.8/qwak/feature_store/offline/_offline_serving_validations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.4.8/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.4.8/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/offline/client.py` & `qwak_core-0.4.8/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/offline/client_v2.py` & `qwak_core-0.4.8/qwak/feature_store/offline/client_v2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/offline/feature_set_features.py` & `qwak_core-0.4.8/qwak/feature_store/offline/feature_set_features.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/online/client.py` & `qwak_core-0.4.8/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/online/endpoint_utils.py` & `qwak_core-0.4.8/qwak/feature_store/online/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/validations/validation_options.py` & `qwak_core-0.4.8/qwak/feature_store/validations/validation_options.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/validations/validation_response.py` & `qwak_core-0.4.8/qwak/feature_store/validations/validation_response.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/feature_store/validations/validator.py` & `qwak_core-0.4.8/qwak/feature_store/validations/validator.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_config/build_config_v1.py` & `qwak_core-0.4.8/qwak/inner/build_config/build_config_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,19 @@
     ),
     ConfigCliMap("instance", "build_env.remote.resources.instance", validate_string),
     # Verbosity level
     ConfigCliMap("verbose", "verbose", validate_int),
     ConfigCliMap("deploy", "deploy", validate_bool),
     ConfigCliMap("deployment_instance", "deployment_instance", validate_string),
     ConfigCliMap("purchase_option", "purchase_option", validate_purchase_option),
-    ConfigCliMap("provision_timeout", "provision_timeout", validate_positive_int),
+    ConfigCliMap(
+        "provision_instance_timeout",
+        "provision_instance_timeout",
+        validate_positive_int,
+    ),
 ]
 
 
 @protobuf_factory(Step)
 @dataclass
 class Step:
     validate_build_artifact: bool = field(default=True)
@@ -249,15 +253,15 @@
     build_env: Optional[BuildEnv] = field(default_factory=BuildEnv)
     pre_build: Optional[BuildEnv] = field(default=None)
     post_build: Optional[BuildEnv] = field(default=None)
     step: Step = field(default_factory=Step)
     deploy: bool = field(default=False)
     deployment_instance: Optional[str] = field(default=None)
     purchase_option: Optional[str] = field(default=None)
-    provision_timeout: Optional[int] = field(default=None)
+    provision_instance_timeout: Optional[int] = field(default=None)
     verbose: int = field(default=0)
     pre_built_model: Optional[QwakModel] = field(default=None, init=False)
 
     def _post_merge_cli(self):
         """Implementing post merge actions."""
         self.build_properties.model_id = self.build_properties.model_id.lower()
         self.build_properties.tags = list(self.build_properties.tags)
```

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/build_loggers/trigger_build_logger.py` & `qwak_core-0.4.8/qwak/inner/build_logic/build_loggers/trigger_build_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/execute_build_pipeline.py` & `qwak_core-0.4.8/qwak/inner/build_logic/execute_build_pipeline.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/interface/build_logger_interface.py` & `qwak_core-0.4.8/qwak/inner/build_logic/interface/build_logger_interface.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/interface/build_phase.py` & `qwak_core-0.4.8/qwak/inner/build_logic/interface/build_phase.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/interface/context_interface.py` & `qwak_core-0.4.8/qwak/inner/build_logic/interface/context_interface.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/interface/phase_run_handler.py` & `qwak_core-0.4.8/qwak/inner/build_logic/interface/phase_run_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/interface/step_inteface.py` & `qwak_core-0.4.8/qwak/inner/build_logic/interface/step_inteface.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/interface/time_source.py` & `qwak_core-0.4.8/qwak/inner/build_logic/interface/time_source.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_model_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/common.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/fetch_strategy_manager.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/folder/folder_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/git/git_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/fetch_strategy_manager/strategy/zip/zip_strategy.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/post_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/pre_fetch_validation_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_010_fetch_model/set_version_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/cleanup_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/start_remote_build_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phase_020_remote_register_qwak_build/upload_step.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/phases/phases_pipeline.py` & `qwak_core-0.4.8/qwak/inner/build_logic/phases/phases_pipeline.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py` & `qwak_core-0.4.8/qwak/inner/build_logic/run_handlers/programmatic_phase_run_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/tools/dependencies_tools.py` & `qwak_core-0.4.8/qwak/inner/build_logic/tools/dependencies_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/tools/files.py` & `qwak_core-0.4.8/qwak/inner/build_logic/tools/files.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/build_logic/tools/ignore_files.py` & `qwak_core-0.4.8/qwak/inner/build_logic/tools/ignore_files.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/const.py` & `qwak_core-0.4.8/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.4.8/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/di_configuration/account.py` & `qwak_core-0.4.8/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/di_configuration/containers.py` & `qwak_core-0.4.8/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/instance_template/verify_template_id.py` & `qwak_core-0.4.8/qwak/inner/instance_template/verify_template_id.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/model_loggers_utils.py` & `qwak_core-0.4.8/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/runtime_di/containers.py` & `qwak_core-0.4.8/qwak/inner/runtime_di/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/singleton_meta.py` & `qwak_core-0.4.8/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/tool/auth.py` & `qwak_core-0.4.8/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.4.8/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/tool/protobuf_factory.py` & `qwak_core-0.4.8/qwak/inner/tool/protobuf_factory.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/tool/run_config/base.py` & `qwak_core-0.4.8/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.4.8/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/_entity_extraction.py` & `qwak_core-0.4.8/qwak/model/_entity_extraction.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/adapters/__init__.py` & `qwak_core-0.4.8/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.4.8/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.4.8/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.4.8/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.4.8/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.4.8/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/base.py` & `qwak_core-0.4.8/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/decorators/api.py` & `qwak_core-0.4.8/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/decorators/impl/api_implementation.py` & `qwak_core-0.4.8/qwak/model/decorators/impl/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/decorators/timer.py` & `qwak_core-0.4.8/qwak/model/decorators/timer.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/experiment_tracking.py` & `qwak_core-0.4.8/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/schema.py` & `qwak_core-0.4.8/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/schema_entities.py` & `qwak_core-0.4.8/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/__init__.py` & `qwak_core-0.4.8/qwak/model/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.4.8/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/adapters/input.py` & `qwak_core-0.4.8/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.4.8/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/adapters/output.py` & `qwak_core-0.4.8/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.4.8/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.4.8/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.4.8/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.4.8/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model/tools/run_model_locally.py` & `qwak_core-0.4.8/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.4.8/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model_loggers/data_logger.py` & `qwak_core-0.4.8/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/model_loggers/model_logger.py` & `qwak_core-0.4.8/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/batch_jobs/execution.py` & `qwak_core-0.4.8/qwak/qwak_client/batch_jobs/execution.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/batch_jobs/task.py` & `qwak_core-0.4.8/qwak/qwak_client/batch_jobs/task.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/build_api_helpers/build_api_steps.py` & `qwak_core-0.4.8/qwak/qwak_client/build_api_helpers/build_api_steps.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/build_api_helpers/trigger_build_api.py` & `qwak_core-0.4.8/qwak/qwak_client/build_api_helpers/trigger_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/builds/build.py` & `qwak_core-0.4.8/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.4.8/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.4.8/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/client.py` & `qwak_core-0.4.8/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/data_versioning/data_tag.py` & `qwak_core-0.4.8/qwak/qwak_client/data_versioning/data_tag.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.4.8/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/file_versioning/file_tag.py` & `qwak_core-0.4.8/qwak/qwak_client/file_versioning/file_tag.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/models/model.py` & `qwak_core-0.4.8/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.4.8/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/qwak_client/projects/project.py` & `qwak_core-0.4.8/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/tools/logger/logger.py` & `qwak_core-0.4.8/qwak/tools/logger/logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/tools/logger/logging.yml` & `qwak_core-0.4.8/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/utils/datetime_utils.py` & `qwak_core-0.4.8/qwak/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/vector_store/client.py` & `qwak_core-0.4.8/qwak/vector_store/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/vector_store/collection.py` & `qwak_core-0.4.8/qwak/vector_store/collection.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/vector_store/filters.py` & `qwak_core-0.4.8/qwak/vector_store/filters.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/vector_store/inference_client.py` & `qwak_core-0.4.8/qwak/vector_store/inference_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/vector_store/rest_helpers.py` & `qwak_core-0.4.8/qwak/vector_store/rest_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/vector_store/utils/filter_utils.py` & `qwak_core-0.4.8/qwak/vector_store/utils/filter_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak/vector_store/utils/upsert_utils.py` & `qwak_core-0.4.8/qwak/vector_store/utils/upsert_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/alert_registry_service_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/alert_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/build_orchestrator_build_settings_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/execution_management_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/execution_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/fs_offline_serving_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/fs_offline_serving_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/instance_template_management_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/instance_template_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/internal_build_orchestrator_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/internal_build_orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/vector_serving_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/vector_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/vectors_management_api.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/vectors_management_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/mocks/workspace_manager_service_mock.py` & `qwak_core-0.4.8/qwak_services_mock/mocks/workspace_manager_service_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/qwak_services_mock/services_mock.py` & `qwak_core-0.4.8/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.4.7/setup.py` & `qwak_core-0.4.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 {':extra == "feature-store"': ['cloudpickle==2.2.1'],
  ':python_full_version >= "3.7.1" and python_version < "3.10"': ['protobuf>=3.10,<4'],
  ':python_version >= "3.10"': ['protobuf>=4.21.6'],
  'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.4.7',
+    'version': '0.4.8',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.4.7/PKG-INFO` & `qwak_core-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.4.7
+Version: 0.4.8
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```

