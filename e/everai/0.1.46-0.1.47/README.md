# Comparing `tmp/everai-0.1.46-py3-none-any.whl.zip` & `tmp/everai-0.1.47-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 436354 bytes, number of entries: 419
+Zip file size: 439582 bytes, number of entries: 423
 -rw-r--r--  2.0 unx       66 b- defN 24-Apr-24 07:43 everai/__init__.py
 -rw-r--r--  2.0 unx     1214 b- defN 24-Apr-28 08:33 everai/constants.py
--rw-r--r--  2.0 unx       23 b- defN 24-May-07 11:05 everai/version.py
+-rw-r--r--  2.0 unx       23 b- defN 24-May-09 06:59 everai/version.py
 -rw-r--r--  2.0 unx       40 b- defN 24-Mar-15 10:09 everai/api/__init__.py
--rw-r--r--  2.0 unx    15087 b- defN 24-May-06 13:23 everai/api/api.py
+-rw-r--r--  2.0 unx    15157 b- defN 24-May-09 04:23 everai/api/api.py
 -rw-r--r--  2.0 unx      208 b- defN 24-Apr-15 11:24 everai/app/__init__.py
 -rw-r--r--  2.0 unx     3732 b- defN 24-May-07 10:58 everai/app/app.py
 -rw-r--r--  2.0 unx    12389 b- defN 24-May-06 13:56 everai/app/app_manager.py
 -rw-r--r--  2.0 unx     1791 b- defN 24-Apr-24 07:37 everai/app/app_runner.py
 -rw-r--r--  2.0 unx     3486 b- defN 24-May-06 13:55 everai/app/app_runtime.py
 -rw-r--r--  2.0 unx     2568 b- defN 24-Apr-23 14:51 everai/app/app_setup.py
 -rw-r--r--  2.0 unx     1116 b- defN 24-Apr-24 04:14 everai/app/autocaling_handler.py
@@ -70,17 +70,18 @@
 -rw-r--r--  2.0 unx       66 b- defN 24-May-06 07:03 everai/commands/version/__init__.py
 -rw-r--r--  2.0 unx      561 b- defN 24-May-06 07:03 everai/commands/version/version.py
 -rw-r--r--  2.0 unx       63 b- defN 24-Apr-23 06:49 everai/commands/volume/__init__.py
 -rw-r--r--  2.0 unx      813 b- defN 24-Apr-23 07:08 everai/commands/volume/create.py
 -rw-r--r--  2.0 unx     1679 b- defN 24-May-07 10:51 everai/commands/volume/delete.py
 -rw-r--r--  2.0 unx      752 b- defN 24-Apr-23 07:09 everai/commands/volume/get.py
 -rw-r--r--  2.0 unx      747 b- defN 24-Apr-24 06:20 everai/commands/volume/list.py
+-rw-r--r--  2.0 unx      692 b- defN 24-May-09 04:35 everai/commands/volume/publish.py
 -rw-r--r--  2.0 unx     1507 b- defN 24-Apr-23 07:09 everai/commands/volume/pull.py
 -rw-r--r--  2.0 unx      753 b- defN 24-Apr-23 07:09 everai/commands/volume/push.py
--rw-r--r--  2.0 unx     1395 b- defN 24-Apr-24 06:24 everai/commands/volume/volume.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-09 04:17 everai/commands/volume/volume.py
 -rw-r--r--  2.0 unx       69 b- defN 24-Apr-23 04:08 everai/commands/worker/__init__.py
 -rw-r--r--  2.0 unx     1555 b- defN 24-Apr-25 10:30 everai/commands/worker/list.py
 -rw-r--r--  2.0 unx     1129 b- defN 24-Apr-25 10:26 everai/commands/worker/worker.py
 -rw-r--r--  2.0 unx      270 b- defN 24-Apr-24 10:07 everai/configmap/__init__.py
 -rw-r--r--  2.0 unx     1498 b- defN 24-Apr-23 13:52 everai/configmap/configmap.py
 -rw-r--r--  2.0 unx     1851 b- defN 24-May-06 09:09 everai/configmap/configmap_manager.py
 -rw-r--r--  2.0 unx      741 b- defN 24-Apr-24 10:33 everai/configmap/utils.py
@@ -113,141 +114,142 @@
 -rw-r--r--  2.0 unx     2518 b- defN 24-Apr-23 08:23 everai/utils/list.py
 -rw-r--r--  2.0 unx     1621 b- defN 24-Apr-25 11:57 everai/utils/show_mixin.py
 -rw-r--r--  2.0 unx      238 b- defN 24-Apr-24 05:08 everai/utils/singleton.py
 -rw-r--r--  2.0 unx      515 b- defN 24-Mar-28 11:33 everai/utils/size.py
 -rw-r--r--  2.0 unx      616 b- defN 24-Mar-07 07:12 everai/utils/utils.py
 -rw-r--r--  2.0 unx      153 b- defN 24-Mar-14 15:31 everai/utils/verbose.py
 -rw-r--r--  2.0 unx      107 b- defN 24-Apr-02 06:47 everai/volume/__init__.py
--rw-r--r--  2.0 unx     5148 b- defN 24-Apr-23 13:05 everai/volume/volume.py
--rw-r--r--  2.0 unx    14731 b- defN 24-Apr-23 08:23 everai/volume/volume_manager.py
+-rw-r--r--  2.0 unx     1922 b- defN 24-May-09 06:48 everai/volume/name_helper.py
+-rw-r--r--  2.0 unx     5555 b- defN 24-May-09 04:23 everai/volume/volume.py
+-rw-r--r--  2.0 unx    15081 b- defN 24-May-09 06:47 everai/volume/volume_manager.py
 -rw-r--r--  2.0 unx       55 b- defN 24-Apr-23 13:17 everai/worker/__init__.py
 -rw-r--r--  2.0 unx     3343 b- defN 24-May-07 10:58 everai/worker/worker.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-07 07:21 generated/__init__.py
--rw-r--r--  2.0 unx     1413 b- defN 24-May-07 07:21 generated/configmaps/__init__.py
--rw-r--r--  2.0 unx    29579 b- defN 24-May-07 07:21 generated/configmaps/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-May-07 07:21 generated/configmaps/api_response.py
--rw-r--r--  2.0 unx    14419 b- defN 24-May-07 07:21 generated/configmaps/configuration.py
--rw-r--r--  2.0 unx     5462 b- defN 24-May-07 07:21 generated/configmaps/exceptions.py
--rw-r--r--  2.0 unx    12966 b- defN 24-May-07 07:21 generated/configmaps/rest.py
--rw-r--r--  2.0 unx      127 b- defN 24-May-07 07:21 generated/configmaps/api/__init__.py
--rw-r--r--  2.0 unx    32156 b- defN 24-May-07 07:21 generated/configmaps/api/configmap_service_api.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-07 07:21 generated/configmaps/models/__init__.py
--rw-r--r--  2.0 unx     2555 b- defN 24-May-07 07:21 generated/configmaps/models/configmap_service_create_body.py
--rw-r--r--  2.0 unx     2555 b- defN 24-May-07 07:21 generated/configmaps/models/configmap_service_update_body.py
--rw-r--r--  2.0 unx     2764 b- defN 24-May-07 07:21 generated/configmaps/models/v1_configmap.py
--rw-r--r--  2.0 unx     2906 b- defN 24-May-07 07:21 generated/configmaps/models/v1_list_response.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-07 07:21 generated/configmaps/test/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 04:13 generated/__init__.py
+-rw-r--r--  2.0 unx     1413 b- defN 24-May-09 04:13 generated/configmaps/__init__.py
+-rw-r--r--  2.0 unx    29579 b- defN 24-May-09 04:13 generated/configmaps/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-May-09 04:13 generated/configmaps/api_response.py
+-rw-r--r--  2.0 unx    14419 b- defN 24-May-09 04:13 generated/configmaps/configuration.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-May-09 04:13 generated/configmaps/exceptions.py
+-rw-r--r--  2.0 unx    12966 b- defN 24-May-09 04:13 generated/configmaps/rest.py
+-rw-r--r--  2.0 unx      127 b- defN 24-May-09 04:13 generated/configmaps/api/__init__.py
+-rw-r--r--  2.0 unx    32156 b- defN 24-May-09 04:13 generated/configmaps/api/configmap_service_api.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-09 04:13 generated/configmaps/models/__init__.py
+-rw-r--r--  2.0 unx     2555 b- defN 24-May-09 04:13 generated/configmaps/models/configmap_service_create_body.py
+-rw-r--r--  2.0 unx     2555 b- defN 24-May-09 04:13 generated/configmaps/models/configmap_service_update_body.py
+-rw-r--r--  2.0 unx     2764 b- defN 24-May-09 04:13 generated/configmaps/models/v1_configmap.py
+-rw-r--r--  2.0 unx     2906 b- defN 24-May-09 04:13 generated/configmaps/models/v1_list_response.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 04:13 generated/configmaps/test/__init__.py
 -rw-r--r--  2.0 unx     1357 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_configmap_service_api.py
 -rw-r--r--  2.0 unx     1824 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_configmap_service_create_body.py
 -rw-r--r--  2.0 unx     1824 b- defN 24-Apr-24 09:52 generated/configmaps/test/test_configmap_service_update_body.py
 -rw-r--r--  2.0 unx     1775 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_v1_configmap.py
 -rw-r--r--  2.0 unx     1930 b- defN 24-Apr-23 13:37 generated/configmaps/test/test_v1_list_response.py
--rw-r--r--  2.0 unx     6829 b- defN 24-May-07 07:21 generated/schedulers/__init__.py
--rw-r--r--  2.0 unx    29587 b- defN 24-May-07 07:21 generated/schedulers/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-May-07 07:21 generated/schedulers/api_response.py
--rw-r--r--  2.0 unx    14427 b- defN 24-May-07 07:21 generated/schedulers/configuration.py
--rw-r--r--  2.0 unx     5470 b- defN 24-May-07 07:21 generated/schedulers/exceptions.py
--rw-r--r--  2.0 unx    12974 b- defN 24-May-07 07:21 generated/schedulers/rest.py
--rw-r--r--  2.0 unx      115 b- defN 24-May-07 07:21 generated/schedulers/api/__init__.py
--rw-r--r--  2.0 unx    84166 b- defN 24-May-07 07:21 generated/schedulers/api/app_service_api.py
--rw-r--r--  2.0 unx     6164 b- defN 24-May-07 07:21 generated/schedulers/models/__init__.py
--rw-r--r--  2.0 unx     2744 b- defN 24-May-07 07:21 generated/schedulers/models/app_service_create_body.py
+-rw-r--r--  2.0 unx     6829 b- defN 24-May-09 04:13 generated/schedulers/__init__.py
+-rw-r--r--  2.0 unx    29587 b- defN 24-May-09 04:13 generated/schedulers/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-May-09 04:13 generated/schedulers/api_response.py
+-rw-r--r--  2.0 unx    14427 b- defN 24-May-09 04:13 generated/schedulers/configuration.py
+-rw-r--r--  2.0 unx     5470 b- defN 24-May-09 04:13 generated/schedulers/exceptions.py
+-rw-r--r--  2.0 unx    12974 b- defN 24-May-09 04:13 generated/schedulers/rest.py
+-rw-r--r--  2.0 unx      115 b- defN 24-May-09 04:13 generated/schedulers/api/__init__.py
+-rw-r--r--  2.0 unx    84166 b- defN 24-May-09 04:13 generated/schedulers/api/app_service_api.py
+-rw-r--r--  2.0 unx     6164 b- defN 24-May-09 04:13 generated/schedulers/models/__init__.py
+-rw-r--r--  2.0 unx     2744 b- defN 24-May-09 04:13 generated/schedulers/models/app_service_create_body.py
 -rw-r--r--  2.0 unx     3417 b- defN 24-Apr-17 14:31 generated/schedulers/models/app_service_inference_body.py
 -rw-r--r--  2.0 unx     2962 b- defN 24-Apr-09 08:31 generated/schedulers/models/app_service_resources_body.py
--rw-r--r--  2.0 unx     2951 b- defN 24-May-07 07:21 generated/schedulers/models/app_service_setup_auto_scaling_policy_body.py
+-rw-r--r--  2.0 unx     2951 b- defN 24-May-09 04:13 generated/schedulers/models/app_service_setup_auto_scaling_policy_body.py
 -rw-r--r--  2.0 unx     2691 b- defN 24-Apr-02 07:19 generated/schedulers/models/app_service_setup_body.py
 -rw-r--r--  2.0 unx     2978 b- defN 24-Apr-09 08:31 generated/schedulers/models/app_service_setup_resource_body.py
--rw-r--r--  2.0 unx     2859 b- defN 24-May-07 07:21 generated/schedulers/models/app_service_setup_resources_body.py
--rw-r--r--  2.0 unx     2532 b- defN 24-May-07 07:21 generated/schedulers/models/app_service_setup_secrets_body.py
--rw-r--r--  2.0 unx     3023 b- defN 24-May-07 07:21 generated/schedulers/models/app_service_setup_volumes_body.py
+-rw-r--r--  2.0 unx     2859 b- defN 24-May-09 04:13 generated/schedulers/models/app_service_setup_resources_body.py
+-rw-r--r--  2.0 unx     2532 b- defN 24-May-09 04:13 generated/schedulers/models/app_service_setup_secrets_body.py
+-rw-r--r--  2.0 unx     3023 b- defN 24-May-09 04:13 generated/schedulers/models/app_service_setup_volumes_body.py
 -rw-r--r--  2.0 unx     2523 b- defN 24-Mar-29 07:39 generated/schedulers/models/appsv1_cpu.py
 -rw-r--r--  2.0 unx     2884 b- defN 24-Mar-29 07:39 generated/schedulers/models/appsv1_gpu.py
--rw-r--r--  2.0 unx     3074 b- defN 24-May-07 07:21 generated/schedulers/models/appsv1_setup_image.py
--rw-r--r--  2.0 unx     4049 b- defN 24-May-07 07:21 generated/schedulers/models/appsv1_worker.py
--rw-r--r--  2.0 unx     1146 b- defN 24-May-07 07:21 generated/schedulers/models/list_request_queues_response_queue_reason.py
--rw-r--r--  2.0 unx     2933 b- defN 24-May-07 07:21 generated/schedulers/models/list_request_queues_response_request_queue.py
--rw-r--r--  2.0 unx     6639 b- defN 24-May-07 07:21 generated/schedulers/models/protobuf_any.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-07 07:21 generated/schedulers/models/rule_behavior.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-May-09 04:13 generated/schedulers/models/appsv1_setup_image.py
+-rw-r--r--  2.0 unx     4049 b- defN 24-May-09 04:13 generated/schedulers/models/appsv1_worker.py
+-rw-r--r--  2.0 unx     1146 b- defN 24-May-09 04:13 generated/schedulers/models/list_request_queues_response_queue_reason.py
+-rw-r--r--  2.0 unx     2933 b- defN 24-May-09 04:13 generated/schedulers/models/list_request_queues_response_request_queue.py
+-rw-r--r--  2.0 unx     6639 b- defN 24-May-09 04:13 generated/schedulers/models/protobuf_any.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-09 04:13 generated/schedulers/models/rule_behavior.py
 -rw-r--r--  2.0 unx     2872 b- defN 24-Mar-29 07:39 generated/schedulers/models/schedulerv1_cpu.py
 -rw-r--r--  2.0 unx     3361 b- defN 24-Mar-29 07:39 generated/schedulers/models/schedulerv1_gpu.py
--rw-r--r--  2.0 unx     3551 b- defN 24-May-07 07:21 generated/schedulers/models/v1_app.py
--rw-r--r--  2.0 unx     2825 b- defN 24-May-07 07:21 generated/schedulers/models/v1_app_service_setup_image_body.py
--rw-r--r--  2.0 unx     1151 b- defN 24-May-07 07:21 generated/schedulers/models/v1_app_status.py
--rw-r--r--  2.0 unx     3371 b- defN 24-May-07 07:21 generated/schedulers/models/v1_autoscaling_policy.py
--rw-r--r--  2.0 unx     3073 b- defN 24-May-07 07:21 generated/schedulers/models/v1_bandwidth.py
--rw-r--r--  2.0 unx     2483 b- defN 24-May-07 07:21 generated/schedulers/models/v1_bandwidth_size.py
--rw-r--r--  2.0 unx     3086 b- defN 24-May-07 07:21 generated/schedulers/models/v1_basic_auth.py
+-rw-r--r--  2.0 unx     3551 b- defN 24-May-09 04:13 generated/schedulers/models/v1_app.py
+-rw-r--r--  2.0 unx     2825 b- defN 24-May-09 04:13 generated/schedulers/models/v1_app_service_setup_image_body.py
+-rw-r--r--  2.0 unx     1151 b- defN 24-May-09 04:13 generated/schedulers/models/v1_app_status.py
+-rw-r--r--  2.0 unx     3371 b- defN 24-May-09 04:13 generated/schedulers/models/v1_autoscaling_policy.py
+-rw-r--r--  2.0 unx     3073 b- defN 24-May-09 04:13 generated/schedulers/models/v1_bandwidth.py
+-rw-r--r--  2.0 unx     2483 b- defN 24-May-09 04:13 generated/schedulers/models/v1_bandwidth_size.py
+-rw-r--r--  2.0 unx     3086 b- defN 24-May-09 04:13 generated/schedulers/models/v1_basic_auth.py
 -rw-r--r--  2.0 unx     3086 b- defN 24-Apr-09 08:31 generated/schedulers/models/v1_build_in_policy.py
--rw-r--r--  2.0 unx     2965 b- defN 24-May-07 07:21 generated/schedulers/models/v1_built_in_policy.py
--rw-r--r--  2.0 unx     2836 b- defN 24-May-07 07:21 generated/schedulers/models/v1_cpu.py
--rw-r--r--  2.0 unx     2984 b- defN 24-May-07 07:21 generated/schedulers/models/v1_create_volume_request.py
--rw-r--r--  2.0 unx     2876 b- defN 24-May-07 07:21 generated/schedulers/models/v1_create_volume_response.py
--rw-r--r--  2.0 unx     2849 b- defN 24-May-07 07:21 generated/schedulers/models/v1_custom_policy.py
--rw-r--r--  2.0 unx     2987 b- defN 24-May-07 07:21 generated/schedulers/models/v1_delete_volume_request.py
+-rw-r--r--  2.0 unx     2965 b- defN 24-May-09 04:13 generated/schedulers/models/v1_built_in_policy.py
+-rw-r--r--  2.0 unx     2836 b- defN 24-May-09 04:13 generated/schedulers/models/v1_cpu.py
+-rw-r--r--  2.0 unx     2984 b- defN 24-May-09 04:13 generated/schedulers/models/v1_create_volume_request.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-May-09 04:13 generated/schedulers/models/v1_create_volume_response.py
+-rw-r--r--  2.0 unx     2849 b- defN 24-May-09 04:13 generated/schedulers/models/v1_custom_policy.py
+-rw-r--r--  2.0 unx     2987 b- defN 24-May-09 04:13 generated/schedulers/models/v1_delete_volume_request.py
 -rw-r--r--  2.0 unx     2612 b- defN 24-Mar-29 08:50 generated/schedulers/models/v1_delete_volume_response.py
--rw-r--r--  2.0 unx     4796 b- defN 24-May-07 07:21 generated/schedulers/models/v1_device_resource.py
--rw-r--r--  2.0 unx     2449 b- defN 24-May-07 07:21 generated/schedulers/models/v1_empty_response.py
--rw-r--r--  2.0 unx     2753 b- defN 24-May-07 07:21 generated/schedulers/models/v1_error_response.py
--rw-r--r--  2.0 unx     3247 b- defN 24-May-07 07:21 generated/schedulers/models/v1_filesystem.py
--rw-r--r--  2.0 unx     2546 b- defN 24-May-07 07:21 generated/schedulers/models/v1_get_image_request.py
--rw-r--r--  2.0 unx     2847 b- defN 24-May-07 07:21 generated/schedulers/models/v1_get_image_response.py
--rw-r--r--  2.0 unx     2624 b- defN 24-May-07 07:21 generated/schedulers/models/v1_get_volume_request.py
--rw-r--r--  2.0 unx     2864 b- defN 24-May-07 07:21 generated/schedulers/models/v1_get_volume_response.py
--rw-r--r--  2.0 unx     2518 b- defN 24-May-07 07:21 generated/schedulers/models/v1_get_worker_request.py
--rw-r--r--  2.0 unx     2900 b- defN 24-May-07 07:21 generated/schedulers/models/v1_get_worker_response.py
--rw-r--r--  2.0 unx     3325 b- defN 24-May-07 07:21 generated/schedulers/models/v1_gpu.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-07 07:21 generated/schedulers/models/v1_gpu_opts.py
--rw-r--r--  2.0 unx     2508 b- defN 24-May-07 07:21 generated/schedulers/models/v1_header_entry.py
--rw-r--r--  2.0 unx     3320 b- defN 24-May-07 07:21 generated/schedulers/models/v1_image.py
--rw-r--r--  2.0 unx     4574 b- defN 24-May-07 07:21 generated/schedulers/models/v1_image_request.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-07 07:21 generated/schedulers/models/v1_image_status.py
+-rw-r--r--  2.0 unx     4796 b- defN 24-May-09 04:13 generated/schedulers/models/v1_device_resource.py
+-rw-r--r--  2.0 unx     2449 b- defN 24-May-09 04:13 generated/schedulers/models/v1_empty_response.py
+-rw-r--r--  2.0 unx     2753 b- defN 24-May-09 04:13 generated/schedulers/models/v1_error_response.py
+-rw-r--r--  2.0 unx     3247 b- defN 24-May-09 04:13 generated/schedulers/models/v1_filesystem.py
+-rw-r--r--  2.0 unx     2546 b- defN 24-May-09 04:13 generated/schedulers/models/v1_get_image_request.py
+-rw-r--r--  2.0 unx     2847 b- defN 24-May-09 04:13 generated/schedulers/models/v1_get_image_response.py
+-rw-r--r--  2.0 unx     2624 b- defN 24-May-09 04:13 generated/schedulers/models/v1_get_volume_request.py
+-rw-r--r--  2.0 unx     2864 b- defN 24-May-09 04:13 generated/schedulers/models/v1_get_volume_response.py
+-rw-r--r--  2.0 unx     2518 b- defN 24-May-09 04:13 generated/schedulers/models/v1_get_worker_request.py
+-rw-r--r--  2.0 unx     2900 b- defN 24-May-09 04:13 generated/schedulers/models/v1_get_worker_response.py
+-rw-r--r--  2.0 unx     3325 b- defN 24-May-09 04:13 generated/schedulers/models/v1_gpu.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-09 04:13 generated/schedulers/models/v1_gpu_opts.py
+-rw-r--r--  2.0 unx     2508 b- defN 24-May-09 04:13 generated/schedulers/models/v1_header_entry.py
+-rw-r--r--  2.0 unx     3320 b- defN 24-May-09 04:13 generated/schedulers/models/v1_image.py
+-rw-r--r--  2.0 unx     4574 b- defN 24-May-09 04:13 generated/schedulers/models/v1_image_request.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-09 04:13 generated/schedulers/models/v1_image_status.py
 -rw-r--r--  2.0 unx     3436 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_inference_response.py
--rw-r--r--  2.0 unx     2924 b- defN 24-May-07 07:21 generated/schedulers/models/v1_list_image_request.py
--rw-r--r--  2.0 unx     3033 b- defN 24-May-07 07:21 generated/schedulers/models/v1_list_image_response.py
--rw-r--r--  2.0 unx     3038 b- defN 24-May-07 07:21 generated/schedulers/models/v1_list_request_queues_response.py
--rw-r--r--  2.0 unx     2836 b- defN 24-May-07 07:21 generated/schedulers/models/v1_list_response.py
--rw-r--r--  2.0 unx     2863 b- defN 24-May-07 07:21 generated/schedulers/models/v1_list_volume_request.py
--rw-r--r--  2.0 unx     3050 b- defN 24-May-07 07:21 generated/schedulers/models/v1_list_volume_response.py
--rw-r--r--  2.0 unx     2731 b- defN 24-May-07 07:21 generated/schedulers/models/v1_list_worker_request.py
--rw-r--r--  2.0 unx     3086 b- defN 24-May-07 07:21 generated/schedulers/models/v1_list_worker_response.py
--rw-r--r--  2.0 unx     3790 b- defN 24-May-07 07:21 generated/schedulers/models/v1_list_workers_response.py
--rw-r--r--  2.0 unx     3274 b- defN 24-May-07 07:21 generated/schedulers/models/v1_pull_image_request.py
--rw-r--r--  2.0 unx     2851 b- defN 24-May-07 07:21 generated/schedulers/models/v1_pull_image_response.py
--rw-r--r--  2.0 unx     2875 b- defN 24-May-07 07:21 generated/schedulers/models/v1_remove_image_request.py
--rw-r--r--  2.0 unx     3828 b- defN 24-May-07 07:21 generated/schedulers/models/v1_resource_claim.py
--rw-r--r--  2.0 unx     3190 b- defN 24-May-07 07:21 generated/schedulers/models/v1_resources.py
--rw-r--r--  2.0 unx     2616 b- defN 24-May-07 07:21 generated/schedulers/models/v1_restart_worker_request.py
--rw-r--r--  2.0 unx     4381 b- defN 24-May-07 07:21 generated/schedulers/models/v1_route_request.py
--rw-r--r--  2.0 unx     3056 b- defN 24-May-07 07:21 generated/schedulers/models/v1_rule.py
--rw-r--r--  2.0 unx     4243 b- defN 24-May-07 07:21 generated/schedulers/models/v1_run_worker_request.py
--rw-r--r--  2.0 unx     2924 b- defN 24-May-07 07:21 generated/schedulers/models/v1_run_worker_response.py
+-rw-r--r--  2.0 unx     2924 b- defN 24-May-09 04:13 generated/schedulers/models/v1_list_image_request.py
+-rw-r--r--  2.0 unx     3033 b- defN 24-May-09 04:13 generated/schedulers/models/v1_list_image_response.py
+-rw-r--r--  2.0 unx     3038 b- defN 24-May-09 04:13 generated/schedulers/models/v1_list_request_queues_response.py
+-rw-r--r--  2.0 unx     2836 b- defN 24-May-09 04:13 generated/schedulers/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2863 b- defN 24-May-09 04:13 generated/schedulers/models/v1_list_volume_request.py
+-rw-r--r--  2.0 unx     3050 b- defN 24-May-09 04:13 generated/schedulers/models/v1_list_volume_response.py
+-rw-r--r--  2.0 unx     2731 b- defN 24-May-09 04:13 generated/schedulers/models/v1_list_worker_request.py
+-rw-r--r--  2.0 unx     3086 b- defN 24-May-09 04:13 generated/schedulers/models/v1_list_worker_response.py
+-rw-r--r--  2.0 unx     3790 b- defN 24-May-09 04:13 generated/schedulers/models/v1_list_workers_response.py
+-rw-r--r--  2.0 unx     3274 b- defN 24-May-09 04:13 generated/schedulers/models/v1_pull_image_request.py
+-rw-r--r--  2.0 unx     2851 b- defN 24-May-09 04:13 generated/schedulers/models/v1_pull_image_response.py
+-rw-r--r--  2.0 unx     2875 b- defN 24-May-09 04:13 generated/schedulers/models/v1_remove_image_request.py
+-rw-r--r--  2.0 unx     3828 b- defN 24-May-09 04:13 generated/schedulers/models/v1_resource_claim.py
+-rw-r--r--  2.0 unx     3190 b- defN 24-May-09 04:13 generated/schedulers/models/v1_resources.py
+-rw-r--r--  2.0 unx     2616 b- defN 24-May-09 04:13 generated/schedulers/models/v1_restart_worker_request.py
+-rw-r--r--  2.0 unx     4381 b- defN 24-May-09 04:13 generated/schedulers/models/v1_route_request.py
+-rw-r--r--  2.0 unx     3056 b- defN 24-May-09 04:13 generated/schedulers/models/v1_rule.py
+-rw-r--r--  2.0 unx     4243 b- defN 24-May-09 04:13 generated/schedulers/models/v1_run_worker_request.py
+-rw-r--r--  2.0 unx     2924 b- defN 24-May-09 04:13 generated/schedulers/models/v1_run_worker_response.py
 -rw-r--r--  2.0 unx     4848 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setting.py
 -rw-r--r--  2.0 unx     3058 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_image.py
 -rw-r--r--  2.0 unx     2518 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_secrets.py
--rw-r--r--  2.0 unx     2764 b- defN 24-May-07 07:21 generated/schedulers/models/v1_setup_volume.py
+-rw-r--r--  2.0 unx     2764 b- defN 24-May-09 04:13 generated/schedulers/models/v1_setup_volume.py
 -rw-r--r--  2.0 unx     2925 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_volumes.py
 -rw-r--r--  2.0 unx     2890 b- defN 24-Apr-02 07:19 generated/schedulers/models/v1_setup_volumes_volume.py
--rw-r--r--  2.0 unx     2749 b- defN 24-May-07 07:21 generated/schedulers/models/v1_stop_worker_request.py
--rw-r--r--  2.0 unx     2475 b- defN 24-May-07 07:21 generated/schedulers/models/v1_storage_size.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-07 07:21 generated/schedulers/models/v1_sync_volume_request.py
+-rw-r--r--  2.0 unx     2749 b- defN 24-May-09 04:13 generated/schedulers/models/v1_stop_worker_request.py
+-rw-r--r--  2.0 unx     2475 b- defN 24-May-09 04:13 generated/schedulers/models/v1_storage_size.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-09 04:13 generated/schedulers/models/v1_sync_volume_request.py
 -rw-r--r--  2.0 unx     2604 b- defN 24-Mar-29 08:50 generated/schedulers/models/v1_sync_volume_response.py
--rw-r--r--  2.0 unx     2504 b- defN 24-May-07 07:21 generated/schedulers/models/v1_value_from_secret.py
--rw-r--r--  2.0 unx     3517 b- defN 24-May-07 07:21 generated/schedulers/models/v1_volume.py
--rw-r--r--  2.0 unx     2576 b- defN 24-May-07 07:21 generated/schedulers/models/v1_volume_mount.py
--rw-r--r--  2.0 unx     5229 b- defN 24-May-07 07:21 generated/schedulers/models/v1_volume_request.py
--rw-r--r--  2.0 unx      970 b- defN 24-May-07 07:21 generated/schedulers/models/v1_volume_status.py
+-rw-r--r--  2.0 unx     2504 b- defN 24-May-09 04:13 generated/schedulers/models/v1_value_from_secret.py
+-rw-r--r--  2.0 unx     3517 b- defN 24-May-09 04:13 generated/schedulers/models/v1_volume.py
+-rw-r--r--  2.0 unx     2576 b- defN 24-May-09 04:13 generated/schedulers/models/v1_volume_mount.py
+-rw-r--r--  2.0 unx     5229 b- defN 24-May-09 04:13 generated/schedulers/models/v1_volume_request.py
+-rw-r--r--  2.0 unx      970 b- defN 24-May-09 04:13 generated/schedulers/models/v1_volume_status.py
 -rw-r--r--  2.0 unx     3049 b- defN 24-Apr-17 14:31 generated/schedulers/models/v1_worker.py
--rw-r--r--  2.0 unx     5201 b- defN 24-May-07 07:21 generated/schedulers/models/v1_worker_request.py
+-rw-r--r--  2.0 unx     5201 b- defN 24-May-09 04:13 generated/schedulers/models/v1_worker_request.py
 -rw-r--r--  2.0 unx     1052 b- defN 24-Apr-23 13:37 generated/schedulers/models/v1_worker_status.py
--rw-r--r--  2.0 unx     1210 b- defN 24-May-07 07:21 generated/schedulers/models/v1_worker_worker_status.py
--rw-r--r--  2.0 unx     3106 b- defN 24-May-07 07:21 generated/schedulers/models/v1workersv1_worker.py
+-rw-r--r--  2.0 unx     1210 b- defN 24-May-09 04:13 generated/schedulers/models/v1_worker_worker_status.py
+-rw-r--r--  2.0 unx     3106 b- defN 24-May-09 04:13 generated/schedulers/models/v1workersv1_worker.py
 -rw-r--r--  2.0 unx     3439 b- defN 24-Apr-02 07:19 generated/schedulers/models/volumesv1_volume.py
--rw-r--r--  2.0 unx     1192 b- defN 24-May-07 07:21 generated/schedulers/models/worker_worker_detail_status.py
--rw-r--r--  2.0 unx     1073 b- defN 24-May-07 07:21 generated/schedulers/models/workersv1_worker_status.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-07 07:21 generated/schedulers/test/__init__.py
+-rw-r--r--  2.0 unx     1192 b- defN 24-May-09 04:13 generated/schedulers/models/worker_worker_detail_status.py
+-rw-r--r--  2.0 unx     1073 b- defN 24-May-09 04:13 generated/schedulers/models/workersv1_worker_status.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 04:13 generated/schedulers/test/__init__.py
 -rw-r--r--  2.0 unx     1668 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_api.py
 -rw-r--r--  2.0 unx     1602 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_create_body.py
 -rw-r--r--  2.0 unx     1763 b- defN 24-Apr-17 14:12 generated/schedulers/test/test_app_service_inference_body.py
 -rw-r--r--  2.0 unx     2887 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_resources_body.py
 -rw-r--r--  2.0 unx     3598 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_auto_scaling_policy_body.py
 -rw-r--r--  2.0 unx     7883 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_app_service_setup_body.py
 -rw-r--r--  2.0 unx     2936 b- defN 24-Apr-09 08:31 generated/schedulers/test/test_app_service_setup_resource_body.py
@@ -334,88 +336,90 @@
 -rw-r--r--  2.0 unx     2991 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker_request.py
 -rw-r--r--  2.0 unx      793 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_v1_worker_status.py
 -rw-r--r--  2.0 unx      836 b- defN 24-Apr-23 15:39 generated/schedulers/test/test_v1_worker_worker_status.py
 -rw-r--r--  2.0 unx     1999 b- defN 24-Apr-22 10:29 generated/schedulers/test/test_v1workersv1_worker.py
 -rw-r--r--  2.0 unx     1576 b- defN 24-Mar-29 07:39 generated/schedulers/test/test_volumesv1_volume.py
 -rw-r--r--  2.0 unx      864 b- defN 24-Apr-25 08:59 generated/schedulers/test/test_worker_worker_detail_status.py
 -rw-r--r--  2.0 unx      842 b- defN 24-Apr-23 15:39 generated/schedulers/test/test_workersv1_worker_status.py
--rw-r--r--  2.0 unx     1344 b- defN 24-May-07 07:21 generated/secrets/__init__.py
--rw-r--r--  2.0 unx    29558 b- defN 24-May-07 07:21 generated/secrets/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-May-07 07:21 generated/secrets/api_response.py
--rw-r--r--  2.0 unx    14413 b- defN 24-May-07 07:21 generated/secrets/configuration.py
--rw-r--r--  2.0 unx     5459 b- defN 24-May-07 07:21 generated/secrets/exceptions.py
--rw-r--r--  2.0 unx    12960 b- defN 24-May-07 07:21 generated/secrets/rest.py
--rw-r--r--  2.0 unx      118 b- defN 24-May-07 07:21 generated/secrets/api/__init__.py
--rw-r--r--  2.0 unx    31721 b- defN 24-May-07 07:21 generated/secrets/api/secret_service_api.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-07 07:21 generated/secrets/models/__init__.py
--rw-r--r--  2.0 unx     2540 b- defN 24-May-07 07:21 generated/secrets/models/secret_service_create_body.py
--rw-r--r--  2.0 unx     2540 b- defN 24-May-07 07:21 generated/secrets/models/secret_service_update_body.py
--rw-r--r--  2.0 unx     2861 b- defN 24-May-07 07:21 generated/secrets/models/v1_list_response.py
--rw-r--r--  2.0 unx     2749 b- defN 24-May-07 07:21 generated/secrets/models/v1_secret.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-07 07:21 generated/secrets/test/__init__.py
+-rw-r--r--  2.0 unx     1344 b- defN 24-May-09 04:13 generated/secrets/__init__.py
+-rw-r--r--  2.0 unx    29558 b- defN 24-May-09 04:13 generated/secrets/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-May-09 04:13 generated/secrets/api_response.py
+-rw-r--r--  2.0 unx    14413 b- defN 24-May-09 04:13 generated/secrets/configuration.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-May-09 04:13 generated/secrets/exceptions.py
+-rw-r--r--  2.0 unx    12960 b- defN 24-May-09 04:13 generated/secrets/rest.py
+-rw-r--r--  2.0 unx      118 b- defN 24-May-09 04:13 generated/secrets/api/__init__.py
+-rw-r--r--  2.0 unx    31721 b- defN 24-May-09 04:13 generated/secrets/api/secret_service_api.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-09 04:13 generated/secrets/models/__init__.py
+-rw-r--r--  2.0 unx     2540 b- defN 24-May-09 04:13 generated/secrets/models/secret_service_create_body.py
+-rw-r--r--  2.0 unx     2540 b- defN 24-May-09 04:13 generated/secrets/models/secret_service_update_body.py
+-rw-r--r--  2.0 unx     2861 b- defN 24-May-09 04:13 generated/secrets/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2749 b- defN 24-May-09 04:13 generated/secrets/models/v1_secret.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 04:13 generated/secrets/test/__init__.py
 -rw-r--r--  2.0 unx     1297 b- defN 24-Mar-28 14:39 generated/secrets/test/test_secret_service_api.py
 -rw-r--r--  2.0 unx     1680 b- defN 24-Mar-28 14:39 generated/secrets/test/test_secret_service_create_body.py
 -rw-r--r--  2.0 unx     1782 b- defN 24-Apr-24 09:52 generated/secrets/test/test_secret_service_update_body.py
 -rw-r--r--  2.0 unx     1845 b- defN 24-Mar-28 14:39 generated/secrets/test/test_v1_list_response.py
 -rw-r--r--  2.0 unx     1603 b- defN 24-Mar-28 14:39 generated/secrets/test/test_v1_secret.py
--rw-r--r--  2.0 unx     2928 b- defN 24-May-07 07:21 generated/volumes/__init__.py
--rw-r--r--  2.0 unx    29558 b- defN 24-May-07 07:21 generated/volumes/api_client.py
--rw-r--r--  2.0 unx      852 b- defN 24-May-07 07:21 generated/volumes/api_response.py
--rw-r--r--  2.0 unx    14413 b- defN 24-May-07 07:21 generated/volumes/configuration.py
--rw-r--r--  2.0 unx     5459 b- defN 24-May-07 07:21 generated/volumes/exceptions.py
--rw-r--r--  2.0 unx    12960 b- defN 24-May-07 07:21 generated/volumes/rest.py
--rw-r--r--  2.0 unx      118 b- defN 24-May-07 07:21 generated/volumes/api/__init__.py
--rw-r--r--  2.0 unx   119008 b- defN 24-May-07 07:21 generated/volumes/api/volume_service_api.py
--rw-r--r--  2.0 unx     2287 b- defN 24-May-07 07:21 generated/volumes/models/__init__.py
--rw-r--r--  2.0 unx     2991 b- defN 24-May-07 07:21 generated/volumes/models/file_information.py
--rw-r--r--  2.0 unx     2986 b- defN 24-May-07 07:21 generated/volumes/models/v1_file.py
--rw-r--r--  2.0 unx     2415 b- defN 24-May-07 07:21 generated/volumes/models/v1_header_value.py
--rw-r--r--  2.0 unx     2728 b- defN 24-May-07 07:21 generated/volumes/models/v1_initialize_multipart_upload_response.py
--rw-r--r--  2.0 unx     2855 b- defN 24-May-07 07:21 generated/volumes/models/v1_list_files_response.py
--rw-r--r--  2.0 unx     2855 b- defN 24-May-07 07:21 generated/volumes/models/v1_list_parts_response.py
--rw-r--r--  2.0 unx     2861 b- defN 24-May-07 07:21 generated/volumes/models/v1_list_response.py
--rw-r--r--  2.0 unx     2592 b- defN 24-May-07 07:21 generated/volumes/models/v1_part.py
--rw-r--r--  2.0 unx     2897 b- defN 24-May-07 07:21 generated/volumes/models/v1_revision.py
--rw-r--r--  2.0 unx     3193 b- defN 24-May-07 07:21 generated/volumes/models/v1_sign_response.py
--rw-r--r--  2.0 unx     2910 b- defN 24-May-07 07:21 generated/volumes/models/v1_sign_upload_response.py
--rw-r--r--  2.0 unx      901 b- defN 24-May-07 07:21 generated/volumes/models/v1_upload_action.py
--rw-r--r--  2.0 unx     3159 b- defN 24-May-07 07:21 generated/volumes/models/v1_volume.py
--rw-r--r--  2.0 unx     2517 b- defN 24-May-07 07:21 generated/volumes/models/volume_service_change_revision_body.py
--rw-r--r--  2.0 unx     2809 b- defN 24-May-07 07:21 generated/volumes/models/volume_service_commit_file_body.py
--rw-r--r--  2.0 unx     3055 b- defN 24-May-07 07:21 generated/volumes/models/volume_service_commit_file_body_file.py
--rw-r--r--  2.0 unx     2876 b- defN 24-May-07 07:21 generated/volumes/models/volume_service_commit_revision_body.py
--rw-r--r--  2.0 unx     3092 b- defN 24-May-07 07:21 generated/volumes/models/volume_service_complete_multipart_upload_body.py
--rw-r--r--  2.0 unx     2464 b- defN 24-May-07 07:21 generated/volumes/models/volume_service_create_body.py
--rw-r--r--  2.0 unx     2801 b- defN 24-May-07 07:21 generated/volumes/models/volume_service_initialize_multipart_upload_body.py
--rw-r--r--  2.0 unx     2527 b- defN 24-May-07 07:21 generated/volumes/models/volume_service_sign_multipart_upload_body.py
--rw-r--r--  2.0 unx     2741 b- defN 24-May-07 07:21 generated/volumes/models/volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-07 07:21 generated/volumes/test/__init__.py
+-rw-r--r--  2.0 unx     2997 b- defN 24-May-09 04:13 generated/volumes/__init__.py
+-rw-r--r--  2.0 unx    29558 b- defN 24-May-09 04:13 generated/volumes/api_client.py
+-rw-r--r--  2.0 unx      852 b- defN 24-May-09 04:13 generated/volumes/api_response.py
+-rw-r--r--  2.0 unx    14413 b- defN 24-May-09 04:13 generated/volumes/configuration.py
+-rw-r--r--  2.0 unx     5459 b- defN 24-May-09 04:13 generated/volumes/exceptions.py
+-rw-r--r--  2.0 unx    12960 b- defN 24-May-09 04:13 generated/volumes/rest.py
+-rw-r--r--  2.0 unx      118 b- defN 24-May-09 04:13 generated/volumes/api/__init__.py
+-rw-r--r--  2.0 unx   143619 b- defN 24-May-09 04:13 generated/volumes/api/volume_service_api.py
+-rw-r--r--  2.0 unx     2356 b- defN 24-May-09 04:13 generated/volumes/models/__init__.py
+-rw-r--r--  2.0 unx     2991 b- defN 24-May-09 04:13 generated/volumes/models/file_information.py
+-rw-r--r--  2.0 unx     2986 b- defN 24-May-09 04:13 generated/volumes/models/v1_file.py
+-rw-r--r--  2.0 unx     2415 b- defN 24-May-09 04:13 generated/volumes/models/v1_header_value.py
+-rw-r--r--  2.0 unx     2728 b- defN 24-May-09 04:13 generated/volumes/models/v1_initialize_multipart_upload_response.py
+-rw-r--r--  2.0 unx     2855 b- defN 24-May-09 04:13 generated/volumes/models/v1_list_files_response.py
+-rw-r--r--  2.0 unx     2855 b- defN 24-May-09 04:13 generated/volumes/models/v1_list_parts_response.py
+-rw-r--r--  2.0 unx     2861 b- defN 24-May-09 04:13 generated/volumes/models/v1_list_response.py
+-rw-r--r--  2.0 unx     2592 b- defN 24-May-09 04:13 generated/volumes/models/v1_part.py
+-rw-r--r--  2.0 unx     2897 b- defN 24-May-09 04:13 generated/volumes/models/v1_revision.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-May-09 04:13 generated/volumes/models/v1_sign_response.py
+-rw-r--r--  2.0 unx     2910 b- defN 24-May-09 04:13 generated/volumes/models/v1_sign_upload_response.py
+-rw-r--r--  2.0 unx      901 b- defN 24-May-09 04:13 generated/volumes/models/v1_upload_action.py
+-rw-r--r--  2.0 unx     3323 b- defN 24-May-09 04:13 generated/volumes/models/v1_volume.py
+-rw-r--r--  2.0 unx      951 b- defN 24-May-09 04:13 generated/volumes/models/v1_volume_status.py
+-rw-r--r--  2.0 unx     2517 b- defN 24-May-09 04:13 generated/volumes/models/volume_service_change_revision_body.py
+-rw-r--r--  2.0 unx     2809 b- defN 24-May-09 04:13 generated/volumes/models/volume_service_commit_file_body.py
+-rw-r--r--  2.0 unx     3055 b- defN 24-May-09 04:13 generated/volumes/models/volume_service_commit_file_body_file.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-May-09 04:13 generated/volumes/models/volume_service_commit_revision_body.py
+-rw-r--r--  2.0 unx     3092 b- defN 24-May-09 04:13 generated/volumes/models/volume_service_complete_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2464 b- defN 24-May-09 04:13 generated/volumes/models/volume_service_create_body.py
+-rw-r--r--  2.0 unx     2801 b- defN 24-May-09 04:13 generated/volumes/models/volume_service_initialize_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2527 b- defN 24-May-09 04:13 generated/volumes/models/volume_service_sign_multipart_upload_body.py
+-rw-r--r--  2.0 unx     2741 b- defN 24-May-09 04:13 generated/volumes/models/volume_service_sign_upload_body.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 04:13 generated/volumes/test/__init__.py
 -rw-r--r--  2.0 unx     1716 b- defN 24-Mar-28 14:39 generated/volumes/test/test_file_information.py
 -rw-r--r--  2.0 unx     1718 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_file.py
 -rw-r--r--  2.0 unx     1494 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_header_value.py
 -rw-r--r--  2.0 unx     1755 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_initialize_multipart_upload_response.py
 -rw-r--r--  2.0 unx     1949 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_files_response.py
 -rw-r--r--  2.0 unx     1721 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_parts_response.py
 -rw-r--r--  2.0 unx     2073 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_list_response.py
 -rw-r--r--  2.0 unx     1486 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_part.py
 -rw-r--r--  2.0 unx     1609 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_revision.py
 -rw-r--r--  2.0 unx     1722 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_sign_response.py
 -rw-r--r--  2.0 unx     1952 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_sign_upload_response.py
 -rw-r--r--  2.0 unx      779 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_upload_action.py
 -rw-r--r--  2.0 unx     1795 b- defN 24-Mar-28 14:39 generated/volumes/test/test_v1_volume.py
+-rw-r--r--  2.0 unx      779 b- defN 24-May-09 04:00 generated/volumes/test/test_v1_volume_status.py
 -rw-r--r--  2.0 unx     3607 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_api.py
 -rw-r--r--  2.0 unx     1712 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_change_revision_body.py
 -rw-r--r--  2.0 unx     2004 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_file_body.py
 -rw-r--r--  2.0 unx     1912 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_file_body_file.py
 -rw-r--r--  2.0 unx     2548 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_commit_revision_body.py
 -rw-r--r--  2.0 unx     2233 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1624 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_create_body.py
 -rw-r--r--  2.0 unx     2149 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1769 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 -rw-r--r--  2.0 unx     1968 b- defN 24-Mar-28 14:39 generated/volumes/test/test_volume_service_sign_upload_body.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-07 11:06 everai-0.1.46.dist-info/LICENSE
--rw-r--r--  2.0 unx     1951 b- defN 24-May-07 11:06 everai-0.1.46.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-07 11:06 everai-0.1.46.dist-info/WHEEL
--rw-r--r--  2.0 unx       98 b- defN 24-May-07 11:06 everai-0.1.46.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       17 b- defN 24-May-07 11:06 everai-0.1.46.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    41888 b- defN 24-May-07 11:06 everai-0.1.46.dist-info/RECORD
-419 files, 1352080 bytes uncompressed, 368124 bytes compressed:  72.8%
+-rw-r--r--  2.0 unx        0 b- defN 24-May-09 06:59 everai-0.1.47.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1951 b- defN 24-May-09 06:59 everai-0.1.47.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-09 06:59 everai-0.1.47.dist-info/WHEEL
+-rw-r--r--  2.0 unx       98 b- defN 24-May-09 06:59 everai-0.1.47.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-May-09 06:59 everai-0.1.47.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    42265 b- defN 24-May-09 06:59 everai-0.1.47.dist-info/RECORD
+423 files, 1382641 bytes uncompressed, 370744 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -219,14 +219,17 @@
 
 Filename: everai/commands/volume/get.py
 Comment: 
 
 Filename: everai/commands/volume/list.py
 Comment: 
 
+Filename: everai/commands/volume/publish.py
+Comment: 
+
 Filename: everai/commands/volume/pull.py
 Comment: 
 
 Filename: everai/commands/volume/push.py
 Comment: 
 
 Filename: everai/commands/volume/volume.py
@@ -348,14 +351,17 @@
 
 Filename: everai/utils/verbose.py
 Comment: 
 
 Filename: everai/volume/__init__.py
 Comment: 
 
+Filename: everai/volume/name_helper.py
+Comment: 
+
 Filename: everai/volume/volume.py
 Comment: 
 
 Filename: everai/volume/volume_manager.py
 Comment: 
 
 Filename: everai/worker/__init__.py
@@ -1134,14 +1140,17 @@
 
 Filename: generated/volumes/models/v1_upload_action.py
 Comment: 
 
 Filename: generated/volumes/models/v1_volume.py
 Comment: 
 
+Filename: generated/volumes/models/v1_volume_status.py
+Comment: 
+
 Filename: generated/volumes/models/volume_service_change_revision_body.py
 Comment: 
 
 Filename: generated/volumes/models/volume_service_commit_file_body.py
 Comment: 
 
 Filename: generated/volumes/models/volume_service_commit_file_body_file.py
@@ -1203,14 +1212,17 @@
 
 Filename: generated/volumes/test/test_v1_upload_action.py
 Comment: 
 
 Filename: generated/volumes/test/test_v1_volume.py
 Comment: 
 
+Filename: generated/volumes/test/test_v1_volume_status.py
+Comment: 
+
 Filename: generated/volumes/test/test_volume_service_api.py
 Comment: 
 
 Filename: generated/volumes/test/test_volume_service_change_revision_body.py
 Comment: 
 
 Filename: generated/volumes/test/test_volume_service_commit_file_body.py
@@ -1233,26 +1245,26 @@
 
 Filename: generated/volumes/test/test_volume_service_sign_multipart_upload_body.py
 Comment: 
 
 Filename: generated/volumes/test/test_volume_service_sign_upload_body.py
 Comment: 
 
-Filename: everai-0.1.46.dist-info/LICENSE
+Filename: everai-0.1.47.dist-info/LICENSE
 Comment: 
 
-Filename: everai-0.1.46.dist-info/METADATA
+Filename: everai-0.1.47.dist-info/METADATA
 Comment: 
 
-Filename: everai-0.1.46.dist-info/WHEEL
+Filename: everai-0.1.47.dist-info/WHEEL
 Comment: 
 
-Filename: everai-0.1.46.dist-info/entry_points.txt
+Filename: everai-0.1.47.dist-info/entry_points.txt
 Comment: 
 
-Filename: everai-0.1.46.dist-info/top_level.txt
+Filename: everai-0.1.47.dist-info/top_level.txt
 Comment: 
 
-Filename: everai-0.1.46.dist-info/RECORD
+Filename: everai-0.1.47.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## everai/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.46"
+__version__ = "0.1.47"
```

## everai/api/api.py

```diff
@@ -1,12 +1,10 @@
 import functools
 import typing
-import ssl
 
-from everai.logger import logger
 from everai.token_manager import TokenManager
 from generated.configmaps import (
     ApiClient as ConfigMapsClient,
     ConfigmapServiceApi, V1Configmap, ConfigmapServiceCreateBody, ConfigmapServiceUpdateBody
 )
 
 from generated.schedulers import (
@@ -235,14 +233,17 @@
                 sha256=file.sha256,
                 created_at=file.created_at,
                 modified_at=file.modified_at,
             ))
         )
         return
 
+    def publish_volume(self, name: str):
+        return self.volume_service_api.publish_volume(volume_name=name)
+
     def get_volume(self, name: str) -> V1Volume:
         return self.volume_service_api.get_volume(name)
 
     def delete_volume(self, name: str) -> None:
         self.volume_service_api.delete_volume(name)
 
     def list_volumes(self) -> typing.List[V1Volume]:
```

## everai/commands/volume/volume.py

```diff
@@ -1,13 +1,14 @@
 from everai.commands.command import ClientCommand, setup_subcommands
 from argparse import _SubParsersAction
 from everai.commands.volume.create import VolumeCreateCommand
 from everai.commands.volume.delete import VolumeDeleteCommand
 from everai.commands.volume.list import VolumeListCommand
 from everai.commands.volume.get import VolumeGetCommand
+from everai.commands.volume.publish import VolumePublishCommand
 from everai.commands.volume.pull import VolumePullCommand
 from everai.commands.volume.push import VolumePushCommand
 
 
 class VolumeCommand(ClientCommand):
     parser: _SubParsersAction = None
 
@@ -24,14 +25,15 @@
         setup_subcommands(volume_subparser, [
             VolumeCreateCommand,
             VolumeListCommand,
             VolumeDeleteCommand,
             VolumeGetCommand,
             VolumePullCommand,
             VolumePushCommand,
+            VolumePublishCommand,
         ])
 
         volume_parser.set_defaults(func=VolumeCommand)
         VolumeCommand.parser = volume_parser
 
     def run(self):
         VolumeCommand.parser.print_help()
```

## everai/volume/volume.py

```diff
@@ -13,54 +13,59 @@
 from types import SimpleNamespace
 import typing
 
 from everai.utils.datetime import format_datetime
 from everai.utils.list import ListUtils
 from everai.utils.show_mixin import ShowMixin, TableField
 from everai.utils.size import readable_size
+from generated.volumes import V1VolumeStatus
 from generated.volumes.models.v1_volume import V1Volume
 
 
 class Volume(ShowMixin):
     _id: str
     _name: str
     revision: str
     _path: typing.Optional[str]
     _created_at: datetime.datetime
     _modified_at: datetime.datetime
     _files: int
     _size: int
+    status: V1VolumeStatus
     _labels: typing.Optional[typing.Dict[str, str]]
 
     table_fields: typing.List[TableField] = [
         TableField('name'),
         TableField('revision'),
         TableField('created_at',
                    formatter=lambda dt: format_datetime(dt)),
         TableField('files'),
         TableField('size', formatter=lambda size: readable_size(size)),
+        TableField('status', formatter=lambda s: s.value.lstrip("STATUS_")),
     ]
 
     wide_table_extra_fields: typing.List[TableField] = [
         TableField('labels')
     ]
 
     def __init__(self, id: str = None, name: str = None, revision: str = None, path: str = None,
                  created_at: datetime.datetime = None, modified_at: datetime.datetime = None,
                  files: int = None, size: int = None,
+                 status: V1VolumeStatus = None,
                  labels: typing.Optional[typing.Dict[str, str]] = None):
         self._name = name
         self.revision = revision or '000000-000'
         self._id = id or ''
         self._created_at = created_at
         self._modified_at = modified_at
         self._labels = labels
         self._path = path or ''
         self._files = files or 0
         self._size = size or 0
+        self.status = status
         self.set_path(path)
 
     def __repr__(self):
         data = '<Volume: id: {}, name: {}, revision: {}, files: {}, size: {}>'.format(
             self.id,
             self.name,
             self.revision,
@@ -71,49 +76,53 @@
 
     def __eq__(self, obj):
         return (self.id == obj.id and
                 self._name == obj.name and
                 self.revision == obj.revision and
                 self.created_at == obj.created_at and
                 self.modified_at == obj.modified_at and
-                self.labels == obj.labels)
+                self.labels == obj.labels and
+                self.status == obj.status)
 
     def to_dict(self):
         return {
             'id': self.id,
             'name': self.name,
             'revision': self.revision,
             'files': self.files,
             'size': self.size,
             'labels': self.labels,
             'created_at': self.created_at,
             'modified_at': self.modified_at,
+            'status': self.status.value,
         }
 
     @staticmethod
     def from_json(data: str) -> Volume:
         x = json.loads(data, object_hook=lambda d: SimpleNamespace(**d))
         return Volume(
             id=x.id if hasattr(x, 'revision') else None,
             name=x.name if hasattr(x, 'revision') else None,
             revision=x.revision if hasattr(x, 'revision') else None,
             created_at=x.created_at if hasattr(x, 'created_at') else None,
-            modified_at=x.created_at if hasattr(x, 'modified_at') else None
+            modified_at=x.created_at if hasattr(x, 'modified_at') else None,
+            status=x.status if hasattr(x, 'status') else None
         )
 
     @staticmethod
     def from_proto(obj: V1Volume) -> Volume:
         return Volume(
             id=obj.id,
             name=obj.name,
             revision=obj.revision,
             files=int(obj.files),
             size=int(obj.size),
             created_at=obj.created_at,
             modified_at=obj.modified_at,
+            status=obj.status,
         )
 
     @staticmethod
     def from_path(path: str) -> typing.Optional[Volume]:
         if not os.path.exists(path):
             return None
```

## everai/volume/volume_manager.py

```diff
@@ -6,14 +6,15 @@
 
 from everai.volume import Volume
 from everai.api import API
 import typing
 from everai.utils.file import FileUtils, DirUtils
 from everai.constants import *
 from everai.utils.list import ListUtils
+from everai.volume.name_helper import myself_volume_name, regular_volume_name
 from generated.volumes import V1File, V1Part
 
 UpdateFileFunction = typing.Callable[[str, str, dict, bool], None]
 GetUpdateFileUrlFunction = typing.Callable[[str, str], tuple[str, str, dict]]
 
 INITIAL_REVISION = '000000-000'
 
@@ -146,22 +147,24 @@
 
         # if is_sync be set, remote local extra files
         if is_sync:
             for delete_file in compare_result.local_only_files:
                 FileUtils(self.join(volume_path, delete_file)).delete()
         return volume
 
+    @myself_volume_name
     def upload_single_file(self, volume_name: str, revision_name: str, file: V1File,
                            file_utils: FileUtils) -> tuple[bool, V1File]:
         should_upload, method, url, headers = self.api.sign_upload(volume_name, revision_name, file.path, file.size,
                                                                    file.sha256)
         if should_upload:
             file_utils.upload_file(method, url, headers)
         return should_upload, file
 
+    @myself_volume_name
     def upload_multipart_file(self, volume_name: str, revision_name: str, file: V1File,
                               file_utils: FileUtils) -> tuple[bool, V1File]:
         should_upload, upload_id = self.api.init_multipart_upload(volume_name, revision_name, file.path, int(file.size),
                                                                   file.sha256)
         if not should_upload:
             return should_upload, file
 
@@ -200,15 +203,16 @@
 
         parts = [x.lstrip('/') for x in args[1:]]
         return str(os.path.join(args[0], *parts))
 
     def file_path(self, volume_id: str, file_path: str) -> str:
         return self.join(self.volume_path(volume_id), file_path)
 
-    def upload_file(self, volume_id: str, volume_name: str, revision_name: str, volume_path: str,
+    @myself_volume_name
+    def upload_file(self, volume_name: str, revision_name: str, volume_path: str,
                     file: str or V1File) -> V1File:
         upload_file_metadata: V1File
         file_utils: FileUtils
         if isinstance(file, str):
             file_path = self.join(volume_path, file)
             file_utils = FileUtils(file_path)
             size = file_utils.get_size()
@@ -226,14 +230,15 @@
             should_commit, result = self.upload_single_file(volume_name, revision_name, upload_file_metadata,
                                                             file_utils)
 
         if should_commit:
             self.api.commit_file(volume_name, revision_name, result)
         return result
 
+    @myself_volume_name
     def push(self, name: str) -> Volume:
         volume = self.get(name)
         volume_path = self.volume_path(volume.id)
         volume.set_path(volume_path)
 
         compare_result = self.compare_files(name, volume_path)
         """
@@ -251,20 +256,20 @@
         # create new revision
         revision = self.api.create_revision(name)
 
         commit_files: typing.List[V1File] = compare_result.consistent_files
 
         # upload missed file
         for file in compare_result.local_only_files:
-            f = self.upload_file(volume.id, name, revision.name, volume_path, file)
+            f = self.upload_file(name, revision.name, volume_path, file)
             commit_files.append(f)
 
         # upload inconsistent files
         for local, cloud in compare_result.inconsistent_files:
-            f = self.upload_file(volume.id, name, revision.name, volume_path, local)
+            f = self.upload_file(name, revision.name, volume_path, local)
             commit_files.append(f)
 
         # commit revision
         self.api.commit_revision(name, revision.name, commit_files)
 
         # change local path to correct revision
         volume.revision = revision.name
@@ -272,14 +277,15 @@
 
         return volume
 
     # use volume id to avoid volume name conflict if more than one user use this machine
     def volume_path(self, volume_id: str) -> str:
         return os.path.join(self.volume_root, volume_id)
 
+    @myself_volume_name
     def create_volume(self, name: str) -> Volume:
         v1_volume = self.api.create_volume(name)
 
         volume = Volume.from_proto(v1_volume)
         assert volume.revision is not None
         volume_path = self.volume_path(volume.id)
         volume.set_path(volume_path)
@@ -296,33 +302,36 @@
             with open(metadata_file, 'r') as f:
                 data = f.read()
                 v = jsonpickle.loads(data, classes=Volume)
                 if v.name == name and (return_value is None or return_value.revision < v.revision):
                     return_value = v
         return return_value
 
+    @myself_volume_name
     def delete_cloud_volume(self, volume_name: str):
         self.api.delete_volume(volume_name)
 
     def delete_local_volume(self, volume_name: str):
         volume = self.from_name(volume_name)
         volume_path = self.volume_path(volume.id)
         shutil.rmtree(volume_path, ignore_errors=True)
 
+    @myself_volume_name
     def delete_volume(self, volume_name: str, local: bool = False, cloud: bool = False) -> None:
         if not local and not cloud:
             raise ValueError('need one of local and cloud or both them to delete volume')
 
         if local:
             self.delete_local_volume(volume_name)
 
         if cloud:
             self.delete_cloud_volume(volume_name)
         return
 
+    @regular_volume_name
     def get(self, volume_name: str) -> Volume:
         volume = self.api.get_volume(volume_name)
         return Volume.from_proto(volume)
 
     def list_local_volumes(self) -> typing.List[Volume]:
         metadata_files = glob.glob(f'{self.volume_root}/*/.metadata', recursive=True)
         volumes: typing.Dict[str, Volume] = {}
@@ -352,7 +361,11 @@
     def list_volumes(self, local: bool = False) -> typing.List[Volume]:
         """
         list volumes
         argument local means list local cache of volumes
         the opposite means list all the volumes in cloud
         """
         return self.list_local_volumes() if local else self.list_cloud_volumes()
+
+    @myself_volume_name
+    def publish_volume(self, name: str):
+        self.api.publish_volume(name)
```

## generated/volumes/__init__.py

```diff
@@ -40,14 +40,15 @@
 from generated.volumes.models.v1_list_response import V1ListResponse
 from generated.volumes.models.v1_part import V1Part
 from generated.volumes.models.v1_revision import V1Revision
 from generated.volumes.models.v1_sign_response import V1SignResponse
 from generated.volumes.models.v1_sign_upload_response import V1SignUploadResponse
 from generated.volumes.models.v1_upload_action import V1UploadAction
 from generated.volumes.models.v1_volume import V1Volume
+from generated.volumes.models.v1_volume_status import V1VolumeStatus
 from generated.volumes.models.volume_service_change_revision_body import VolumeServiceChangeRevisionBody
 from generated.volumes.models.volume_service_commit_file_body import VolumeServiceCommitFileBody
 from generated.volumes.models.volume_service_commit_file_body_file import VolumeServiceCommitFileBodyFile
 from generated.volumes.models.volume_service_commit_revision_body import VolumeServiceCommitRevisionBody
 from generated.volumes.models.volume_service_complete_multipart_upload_body import VolumeServiceCompleteMultipartUploadBody
 from generated.volumes.models.volume_service_create_body import VolumeServiceCreateBody
 from generated.volumes.models.volume_service_initialize_multipart_upload_body import VolumeServiceInitializeMultipartUploadBody
```

## generated/volumes/api/volume_service_api.py

```diff
@@ -1579,27 +1579,27 @@
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     def get_volume(
         self,
-        volume_name: Annotated[StrictStr, Field(description="volume name")],
+        volume_name_1: Annotated[StrictStr, Field(description="volume name")],
         **kwargs,
     ) -> V1Volume:
         """Get a volume metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_volume(volume_name, async_req=True)
+        >>> thread = api.get_volume(volume_name_1, async_req=True)
         >>> result = thread.get()
 
-        :param volume_name: volume name (required)
-        :type volume_name: str
+        :param volume_name_1: volume name (required)
+        :type volume_name_1: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
@@ -1609,30 +1609,179 @@
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the get_volume_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
 
         return self.get_volume_with_http_info(
-            volume_name,
+            volume_name_1,
             **kwargs,
         )
 
     @validate_call
     def get_volume_with_http_info(
         self,
-        volume_name: Annotated[StrictStr, Field(description="volume name")],
+        volume_name_1: Annotated[StrictStr, Field(description="volume name")],
+        **kwargs,
+    ) -> ApiResponse:
+        """Get a volume metadata  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_volume_with_http_info(volume_name_1, async_req=True)
+        >>> result = thread.get()
+
+        :param volume_name_1: volume name (required)
+        :type volume_name_1: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(V1Volume, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'volume_name_1'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_volume" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats: Dict[str, str] = {}
+
+        # process the path parameters
+        _path_params: Dict[str, str] = {}
+        if _params['volume_name_1'] is not None:
+            _path_params['volumeName_1'] = _params['volume_name_1']
+
+
+        # process the query parameters
+        _query_params: List[Tuple[str, str]] = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings: List[str] = []  # noqa: E501
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1Volume",
+        }
+
+        return self.api_client.call_api(
+            '/api/volumes/v1/{volumeName_1}', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    def get_volume_0(
+        self,
+        volume_name: Annotated[str, Field(strict=True, description="volume name")],
+        **kwargs,
+    ) -> V1Volume:
+        """Get a volume metadata  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_volume_0(volume_name, async_req=True)
+        >>> result = thread.get()
+
+        :param volume_name: volume name (required)
+        :type volume_name: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: V1Volume
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the get_volume_0_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+
+        return self.get_volume_0_with_http_info(
+            volume_name,
+            **kwargs,
+        )
+
+    @validate_call
+    def get_volume_0_with_http_info(
+        self,
+        volume_name: Annotated[str, Field(strict=True, description="volume name")],
         **kwargs,
     ) -> ApiResponse:
         """Get a volume metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_volume_with_http_info(volume_name, async_req=True)
+        >>> thread = api.get_volume_0_with_http_info(volume_name, async_req=True)
         >>> result = thread.get()
 
         :param volume_name: volume name (required)
         :type volume_name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
@@ -1676,15 +1825,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_volume" % _key
+                    " to method get_volume_0" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats: Dict[str, str] = {}
 
         # process the path parameters
@@ -1917,27 +2066,27 @@
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     def list_files(
         self,
-        volume_name: Annotated[StrictStr, Field(description="volume name")],
+        volume_name_1: Annotated[StrictStr, Field(description="volume name")],
         **kwargs,
     ) -> V1ListFilesResponse:
         """List files in a persistence volume of current revision  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_files(volume_name, async_req=True)
+        >>> thread = api.list_files(volume_name_1, async_req=True)
         >>> result = thread.get()
 
-        :param volume_name: volume name (required)
-        :type volume_name: str
+        :param volume_name_1: volume name (required)
+        :type volume_name_1: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request.
                If one number provided, it will be total request
                timeout. It can also be a pair (tuple) of
                (connection, read) timeouts.
         :return: Returns the result object.
@@ -1947,30 +2096,179 @@
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the list_files_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
 
         return self.list_files_with_http_info(
-            volume_name,
+            volume_name_1,
             **kwargs,
         )
 
     @validate_call
     def list_files_with_http_info(
         self,
-        volume_name: Annotated[StrictStr, Field(description="volume name")],
+        volume_name_1: Annotated[StrictStr, Field(description="volume name")],
+        **kwargs,
+    ) -> ApiResponse:
+        """List files in a persistence volume of current revision  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_files_with_http_info(volume_name_1, async_req=True)
+        >>> result = thread.get()
+
+        :param volume_name_1: volume name (required)
+        :type volume_name_1: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(V1ListFilesResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'volume_name_1'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method list_files" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats: Dict[str, str] = {}
+
+        # process the path parameters
+        _path_params: Dict[str, str] = {}
+        if _params['volume_name_1'] is not None:
+            _path_params['volumeName_1'] = _params['volume_name_1']
+
+
+        # process the query parameters
+        _query_params: List[Tuple[str, str]] = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings: List[str] = []  # noqa: E501
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1ListFilesResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/volumes/v1/{volumeName_1}/files', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    def list_files_0(
+        self,
+        volume_name: Annotated[str, Field(strict=True, description="volume name")],
+        **kwargs,
+    ) -> V1ListFilesResponse:
+        """List files in a persistence volume of current revision  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_files_0(volume_name, async_req=True)
+        >>> result = thread.get()
+
+        :param volume_name: volume name (required)
+        :type volume_name: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: V1ListFilesResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the list_files_0_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+
+        return self.list_files_0_with_http_info(
+            volume_name,
+            **kwargs,
+        )
+
+    @validate_call
+    def list_files_0_with_http_info(
+        self,
+        volume_name: Annotated[str, Field(strict=True, description="volume name")],
         **kwargs,
     ) -> ApiResponse:
         """List files in a persistence volume of current revision  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_files_with_http_info(volume_name, async_req=True)
+        >>> thread = api.list_files_0_with_http_info(volume_name, async_req=True)
         >>> result = thread.get()
 
         :param volume_name: volume name (required)
         :type volume_name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
@@ -2014,15 +2312,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_files" % _key
+                    " to method list_files_0" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats: Dict[str, str] = {}
 
         # process the path parameters
@@ -2373,26 +2671,335 @@
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
+    def publish_volume(
+        self,
+        volume_name: StrictStr,
+        **kwargs,
+    ) -> object:
+        """Publish volume  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.publish_volume(volume_name, async_req=True)
+        >>> result = thread.get()
+
+        :param volume_name: (required)
+        :type volume_name: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: object
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the publish_volume_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+
+        return self.publish_volume_with_http_info(
+            volume_name,
+            **kwargs,
+        )
+
+    @validate_call
+    def publish_volume_with_http_info(
+        self,
+        volume_name: StrictStr,
+        **kwargs,
+    ) -> ApiResponse:
+        """Publish volume  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.publish_volume_with_http_info(volume_name, async_req=True)
+        >>> result = thread.get()
+
+        :param volume_name: (required)
+        :type volume_name: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'volume_name'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method publish_volume" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats: Dict[str, str] = {}
+
+        # process the path parameters
+        _path_params: Dict[str, str] = {}
+        if _params['volume_name'] is not None:
+            _path_params['volumeName'] = _params['volume_name']
+
+
+        # process the query parameters
+        _query_params: List[Tuple[str, str]] = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings: List[str] = []  # noqa: E501
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "object",
+        }
+
+        return self.api_client.call_api(
+            '/api/volumes/v1/{volumeName}/publish', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
     def sign_download(
         self,
+        volume_name_1: Annotated[str, Field(strict=True, description="volume name")],
+        path: Annotated[str, Field(strict=True, description="file path")],
+        **kwargs,
+    ) -> V1SignResponse:
+        """Sign for download of a file  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.sign_download(volume_name_1, path, async_req=True)
+        >>> result = thread.get()
+
+        :param volume_name_1: volume name (required)
+        :type volume_name_1: str
+        :param path: file path (required)
+        :type path: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: V1SignResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the sign_download_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+
+        return self.sign_download_with_http_info(
+            volume_name_1,
+            path,
+            **kwargs,
+        )
+
+    @validate_call
+    def sign_download_with_http_info(
+        self,
+        volume_name_1: Annotated[str, Field(strict=True, description="volume name")],
+        path: Annotated[str, Field(strict=True, description="file path")],
+        **kwargs,
+    ) -> ApiResponse:
+        """Sign for download of a file  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.sign_download_with_http_info(volume_name_1, path, async_req=True)
+        >>> result = thread.get()
+
+        :param volume_name_1: volume name (required)
+        :type volume_name_1: str
+        :param path: file path (required)
+        :type path: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(V1SignResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'volume_name_1',
+            'path'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method sign_download" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats: Dict[str, str] = {}
+
+        # process the path parameters
+        _path_params: Dict[str, str] = {}
+        if _params['volume_name_1'] is not None:
+            _path_params['volumeName_1'] = _params['volume_name_1']
+
+        if _params['path'] is not None:
+            _path_params['path'] = _params['path']
+
+
+        # process the query parameters
+        _query_params: List[Tuple[str, str]] = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params: List[Tuple[str, str]] = []
+        _files: Dict[str, str] = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings: List[str] = []  # noqa: E501
+
+        _response_types_map: Dict[str, Optional[str]] = {
+            '200': "V1SignResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/volumes/v1/{volumeName_1}/files/{path}', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    def sign_download_0(
+        self,
         volume_name: Annotated[StrictStr, Field(description="volume name")],
         path: Annotated[str, Field(strict=True, description="file path")],
         **kwargs,
     ) -> V1SignResponse:
         """Sign for download of a file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.sign_download(volume_name, path, async_req=True)
+        >>> thread = api.sign_download_0(volume_name, path, async_req=True)
         >>> result = thread.get()
 
         :param volume_name: volume name (required)
         :type volume_name: str
         :param path: file path (required)
         :type path: str
         :param async_req: Whether to execute the request asynchronously.
@@ -2404,36 +3011,36 @@
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: V1SignResponse
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
-            message = "Error! Please call the sign_download_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            message = "Error! Please call the sign_download_0_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
 
-        return self.sign_download_with_http_info(
+        return self.sign_download_0_with_http_info(
             volume_name,
             path,
             **kwargs,
         )
 
     @validate_call
-    def sign_download_with_http_info(
+    def sign_download_0_with_http_info(
         self,
         volume_name: Annotated[StrictStr, Field(description="volume name")],
         path: Annotated[str, Field(strict=True, description="file path")],
         **kwargs,
     ) -> ApiResponse:
         """Sign for download of a file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.sign_download_with_http_info(volume_name, path, async_req=True)
+        >>> thread = api.sign_download_0_with_http_info(volume_name, path, async_req=True)
         >>> result = thread.get()
 
         :param volume_name: volume name (required)
         :type volume_name: str
         :param path: file path (required)
         :type path: str
         :param async_req: Whether to execute the request asynchronously.
@@ -2480,15 +3087,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method sign_download" % _key
+                    " to method sign_download_0" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats: Dict[str, str] = {}
 
         # process the path parameters
```

## generated/volumes/models/__init__.py

```diff
@@ -23,14 +23,15 @@
 from generated.volumes.models.v1_list_response import V1ListResponse
 from generated.volumes.models.v1_part import V1Part
 from generated.volumes.models.v1_revision import V1Revision
 from generated.volumes.models.v1_sign_response import V1SignResponse
 from generated.volumes.models.v1_sign_upload_response import V1SignUploadResponse
 from generated.volumes.models.v1_upload_action import V1UploadAction
 from generated.volumes.models.v1_volume import V1Volume
+from generated.volumes.models.v1_volume_status import V1VolumeStatus
 from generated.volumes.models.volume_service_change_revision_body import VolumeServiceChangeRevisionBody
 from generated.volumes.models.volume_service_commit_file_body import VolumeServiceCommitFileBody
 from generated.volumes.models.volume_service_commit_file_body_file import VolumeServiceCommitFileBodyFile
 from generated.volumes.models.volume_service_commit_revision_body import VolumeServiceCommitRevisionBody
 from generated.volumes.models.volume_service_complete_multipart_upload_body import VolumeServiceCompleteMultipartUploadBody
 from generated.volumes.models.volume_service_create_body import VolumeServiceCreateBody
 from generated.volumes.models.volume_service_initialize_multipart_upload_body import VolumeServiceInitializeMultipartUploadBody
```

## generated/volumes/models/v1_volume.py

```diff
@@ -17,14 +17,15 @@
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Dict, Optional
 from pydantic import BaseModel, StrictStr
 from pydantic import Field
+from generated.volumes.models.v1_volume_status import V1VolumeStatus
 from typing import Dict, Any
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 class V1Volume(BaseModel):
@@ -35,15 +36,16 @@
     name: Optional[StrictStr] = None
     revision: Optional[StrictStr] = None
     created_at: Optional[datetime] = Field(default=None, alias="createdAt")
     modified_at: Optional[datetime] = Field(default=None, alias="modifiedAt")
     labels: Optional[Dict[str, StrictStr]] = None
     size: Optional[StrictStr] = None
     files: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["id", "name", "revision", "createdAt", "modifiedAt", "labels", "size", "files"]
+    status: Optional[V1VolumeStatus] = None
+    __properties: ClassVar[List[str]] = ["id", "name", "revision", "createdAt", "modifiedAt", "labels", "size", "files", "status"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -92,12 +94,13 @@
             "id": obj.get("id"),
             "name": obj.get("name"),
             "revision": obj.get("revision"),
             "createdAt": obj.get("createdAt"),
             "modifiedAt": obj.get("modifiedAt"),
             "labels": obj.get("labels"),
             "size": obj.get("size"),
-            "files": obj.get("files")
+            "files": obj.get("files"),
+            "status": obj.get("status")
         })
         return _obj
```

## Comparing `everai-0.1.46.dist-info/METADATA` & `everai-0.1.47.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everai
-Version: 0.1.46
+Version: 0.1.47
 Summary: Client library to manage everai infrastructure
 Author-email: mc <mc@expvent.com>
 Maintainer-email: mc <mc@expvent.com>
 Project-URL: Homepage, https://everai.expvent.com
 Project-URL: Documentation, https://everai.expvent.com
 Project-URL: Repository, https://github.com/expvent/everai
 Project-URL: Issues, https://github.com/expvent/everai/issues
```

## Comparing `everai-0.1.46.dist-info/RECORD` & `everai-0.1.47.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 everai/__init__.py,sha256=AbgR3tVRy6TETgwXyJITEnET1TSFpEAEqQJJqzReYqQ,66
 everai/constants.py,sha256=6tvPKHYvL1H5ippD2YkwCerLhKftIiOg-SVtFLtVYN4,1214
-everai/version.py,sha256=X3e_85I7oZGwZD8nW9SBKEUbQU7-_3W9FXuicrfxHjc,23
+everai/version.py,sha256=BqdH88p7_x5NtwJCtqUPLKt1fAJF1mVKUoKH7vlX5dQ,23
 everai/api/__init__.py,sha256=2WLrQ_PpJ35__yOVHC89MhILujyGioyaGir-5n6hxCc,40
-everai/api/api.py,sha256=9xem34hxwiTxQfS_japWMHPxC-Oby5pEwHbEQ1A8LYQ,15087
+everai/api/api.py,sha256=FQ8HIdmKfY0ZOVhsToIvE_1yhy2-2eJxHl33oCCyeyo,15157
 everai/app/__init__.py,sha256=A-USWcj6TDAW_hxG6wT3Qb8m3d5Tq733WWC9McNhlGI,208
 everai/app/app.py,sha256=z9B48uwKAJHHW7OfF_rcVmhxR74Y2JAw4n5AApmMLEI,3732
 everai/app/app_manager.py,sha256=-ZLsk8-Ln2NUyipyvxMRH9EgkHLy9KBw56GH68wtEuI,12389
 everai/app/app_runner.py,sha256=HVlOLweFX-C2kBbgyVwuDz4vfGzQ6uzHpNVzikQhRfA,1791
 everai/app/app_runtime.py,sha256=2wFrZLtfNgG6uPR5LP4ID6XlNTOOu0Cy7nHT0wbvWlQ,3486
 everai/app/app_setup.py,sha256=CLXAC83OyTqEjAEKNLHQaCT3UPhvw149mD1VQr-AEEg,2568
 everai/app/autocaling_handler.py,sha256=Exsdti0N16GlcqXIILJ1qa6_DN9cBwzWpahukDKiqEo,1116
@@ -69,17 +69,18 @@
 everai/commands/version/__init__.py,sha256=gTsFsCRNV8TvUgZ0Vbvqi_7RQ6mChgi9Wf5o-EBBdUo,66
 everai/commands/version/version.py,sha256=Y98SgjQ21-wwve8wZVhDZDtfwaQfpp3n5X0cM72_S7g,561
 everai/commands/volume/__init__.py,sha256=UlxXpx7spko6zt5QASgQf3FvKMFWVDs0z6kc9ET_Z3M,63
 everai/commands/volume/create.py,sha256=zX4Jnx81NQjK82tZsatl-ZCtQKKf5mcMz2TTRmg4Szo,813
 everai/commands/volume/delete.py,sha256=zoc6YW4z0X7AlUfU04mcNhyiAMPgYUS1Ex2F7DCoIMA,1679
 everai/commands/volume/get.py,sha256=ruLx6zRKnmUZdpXhxHF2C1XIVgGaa1zLlnfU-nX0bfE,752
 everai/commands/volume/list.py,sha256=YmjnCWIl3pyDxE-F7rOmhDZu2PrlGFsR6MacnJlOFmY,747
+everai/commands/volume/publish.py,sha256=qzjePA3wuRrtKuemsRBQViVtrzqeCponbuY2ll6ir7A,692
 everai/commands/volume/pull.py,sha256=sJKByR1qWxCreb6BMj3kfbhM7w2UuO5eKySDMPtp7lQ,1507
 everai/commands/volume/push.py,sha256=lH_EB0joXOKGY4lPalWkmAPnCesDiytfhzfW_0E4jQA,753
-everai/commands/volume/volume.py,sha256=k6aTAZBo1TZGoTRRJUhVMaWglUey5nTJQm94m8-FBz8,1395
+everai/commands/volume/volume.py,sha256=DfyxbwAZ4UUYightWyu6Kz7zpc77FmT5KUxdWEcXis0,1495
 everai/commands/worker/__init__.py,sha256=8Sswddw1RHWdpl7AHrktEodBITDspvtESL0GnPI0Oo0,69
 everai/commands/worker/list.py,sha256=-9bgexlf0sChB4gjg8aL0jLIg0jKe0YPo0yX1r45L14,1555
 everai/commands/worker/worker.py,sha256=riUtg-KtxLAGwZAJqtB4SfUGwfPZOUGION9EWg3ITOY,1129
 everai/configmap/__init__.py,sha256=xKvP74DWxu5UrMrLiI1_9S1AfqZErlRotGnShY_5cec,270
 everai/configmap/configmap.py,sha256=zZnYKH7aZd2DCeGSyu9kEExwTI5bpXlcQjufDk5e1-g,1498
 everai/configmap/configmap_manager.py,sha256=EV001VUX3VmryImWeKDzty_HLooxs7CqbmlGdUvEGIg,1851
 everai/configmap/utils.py,sha256=OCaJQbnQ810Vs-gjmJnjkT9ibhsQfuLUBlS7Yzdqnjk,741
@@ -112,16 +113,17 @@
 everai/utils/list.py,sha256=zmPSWbdwvarZk4drh98VrTLqIgRh5-s4uWQEieanPLI,2518
 everai/utils/show_mixin.py,sha256=9FQY3Yns49-0Nm1ib_3yucTYi77m3UG2RdyiIXhdzi8,1621
 everai/utils/singleton.py,sha256=OGYIM0bx1kjg71dJK_X9LdFijE1PUKpJzvmcpP0puY8,238
 everai/utils/size.py,sha256=z1WQblKfACpj2wT6Wn-yzjBgklhStiOoJ9cxUgCp-Zw,515
 everai/utils/utils.py,sha256=bo-H50MC67Xs-F-64pAqEIF2epuTy8KkzdMKm2W_-W4,616
 everai/utils/verbose.py,sha256=aQ-nRJaMvhAia7Id_kM-2d5CHij4vudJdKSfyiSnHlw,153
 everai/volume/__init__.py,sha256=_nJ-S-Sgec1jY6byu-u9EOYE7-_1iaMj-kcM-v6pTaY,107
-everai/volume/volume.py,sha256=lW0-z0eIFhMKcz1dSPKMBNMXuQq_a17lTph6gO3Xh0Y,5148
-everai/volume/volume_manager.py,sha256=TZabXDog9dP8-QxsT7yBzBvsnuSEXiT7WM7aHba3qkU,14731
+everai/volume/name_helper.py,sha256=y9wrrRdzpFcLUsTo7bQRUOqWoY_SP-jV6Az1vKAKG7s,1922
+everai/volume/volume.py,sha256=5G7xIXA0PERp-M9RzqIdzFKn8a_XQeU0-5km1G2YFCQ,5555
+everai/volume/volume_manager.py,sha256=OcbH34OFFmhnFQmnT56u3JGrvZbcmOHmcXJDKYMUJl4,15081
 everai/worker/__init__.py,sha256=J8ziddB4caVoslM3FG445bwHAjl9donqX3Bcn7yX3ts,55
 everai/worker/worker.py,sha256=lArNkPO37botGe4oGMSYf5shiztkiz59i0mp0T5eQfs,3343
 generated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 generated/configmaps/__init__.py,sha256=qMsKjxY-Pzah_zlnImcqfkzzTxxl0fSKQst-JyMkhrE,1413
 generated/configmaps/api_client.py,sha256=MAq1ipqq9qhlpjWTF-fjisZeKXnVoCEmly2RJu00geM,29579
 generated/configmaps/api_response.py,sha256=uCehWdXXDnAO2HAHGKe0SgpQ_mJiGDbcu-BHDF3n_IM,852
 generated/configmaps/configuration.py,sha256=eF8KQFEyVDwkTOUtAC8O6Eq4XYMKhYOCtnuwpE7CXKU,14419
@@ -352,36 +354,37 @@
 generated/secrets/models/v1_secret.py,sha256=yAi4mA-i_TDykKBDi21SKHhNHYdL9DHi02e-Crvvaic,2749
 generated/secrets/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 generated/secrets/test/test_secret_service_api.py,sha256=GIFO1TTZ5MGvP4XnTWpahK3RcdW8vR_3iswq9-Zxk5M,1297
 generated/secrets/test/test_secret_service_create_body.py,sha256=eeuiYfAQkguxgQGD3mUcmWMz4sJNL-MhOLkxv-BXepo,1680
 generated/secrets/test/test_secret_service_update_body.py,sha256=CIBEh3HEo-AJ_yy0PQgkRUu9t3TK5D2dxidq1THryNk,1782
 generated/secrets/test/test_v1_list_response.py,sha256=wsZUJa8-6SBoDNh2Unq2Yvit7g9EL_uVbm1OS5o4lhQ,1845
 generated/secrets/test/test_v1_secret.py,sha256=sp1Zw1rraRdo4U3YhwKTCgQbjfqrZ3v1R5EKMGfOhJE,1603
-generated/volumes/__init__.py,sha256=HxwVvzZ7fTycXxp6w4M7Ig_Y0i5FK0HhJVj__E_fVps,2928
+generated/volumes/__init__.py,sha256=sTqKj4X9YbmrjXgOdtNXdFi55GciLqbWKgOHzRmfJB4,2997
 generated/volumes/api_client.py,sha256=leHtpUUBjAKU9ltZhZWmlk_EIDkXRymy6jZFvTNd9FA,29558
 generated/volumes/api_response.py,sha256=uCehWdXXDnAO2HAHGKe0SgpQ_mJiGDbcu-BHDF3n_IM,852
 generated/volumes/configuration.py,sha256=npRZ4V64YFnkCj2tkjEmUyfryXu0VBEqLj-xpeGAq-I,14413
 generated/volumes/exceptions.py,sha256=8d40RdHzGPWJrid1jnWmwfN-AzUUQV9hHPTojnZXugY,5459
 generated/volumes/rest.py,sha256=_7CowOCcyE3qysIrbVkO9g27MKWO2Slmldf0nQ7-JE4,12960
 generated/volumes/api/__init__.py,sha256=Y7InOiJOhJAe8RskibSuV9Pi13cIpxJVr4mv-dk0jzw,118
-generated/volumes/api/volume_service_api.py,sha256=3esRrguSuDyBhcSU4eOrD9Dg3TtBny4KnuNhbSs6TaQ,119008
-generated/volumes/models/__init__.py,sha256=-q6BH8uGeyCJnUML5OUM3xvH5BPOdaoPWppDZYjFPIc,2287
+generated/volumes/api/volume_service_api.py,sha256=2kimuHZVYUH-0rrDosBT1VGdRikSL4IEhK7lsINoDCE,143619
+generated/volumes/models/__init__.py,sha256=pwJq_0BYHPBYIJQsIEH1WuVNIp3Tgwtkmj4NyTQKnI0,2356
 generated/volumes/models/file_information.py,sha256=FHZLXyE4BdY_ZuJXxCeFSIdU4Q3yiICjNiJH9LLeuZc,2991
 generated/volumes/models/v1_file.py,sha256=ldVcpgue_3j7X3mp0l6kTMZ6_D5seUQDeuMRxJqLuks,2986
 generated/volumes/models/v1_header_value.py,sha256=eUx1lDR6LsuPaatYU0MmcFmn74uE2BnNork0EZw-7fA,2415
 generated/volumes/models/v1_initialize_multipart_upload_response.py,sha256=YXVQFfc4C2sJFflFHfJj_3cLeAopYNx3sgXWXKYhjic,2728
 generated/volumes/models/v1_list_files_response.py,sha256=tHDzLYRcUrGXRFyDF_oQLCjtbTfHb6PpRLE9unrtj3k,2855
 generated/volumes/models/v1_list_parts_response.py,sha256=CXsGn7ThemNN3VwfPesYWOPlNDLOn2s-R3zkOedKlfY,2855
 generated/volumes/models/v1_list_response.py,sha256=8Mj5F2zFVaPDug18nJlvHtFr2_soU55yE4lVTgg3XPs,2861
 generated/volumes/models/v1_part.py,sha256=TDIkr88H6p8rLwEre6KwNJMqZ4ENP_35_Z8wuUtZt_0,2592
 generated/volumes/models/v1_revision.py,sha256=bo9EKzTNmhoo2RgVcHBZWQeNqzNdRf9AVYFt_T8x-2I,2897
 generated/volumes/models/v1_sign_response.py,sha256=a9C8mRrXpNVAuAuiV6GB8oUJS-eK2YTifVGNs2mqATQ,3193
 generated/volumes/models/v1_sign_upload_response.py,sha256=DaYcpfaNHJUA9KRgle-SpNjC_-jR7etqXKx7HrmQ45w,2910
 generated/volumes/models/v1_upload_action.py,sha256=achr4vzd1aUrGsvO-60rL_cjDjtXDnr9978-mwvgxco,901
-generated/volumes/models/v1_volume.py,sha256=HHYS2CiUmiIa8ovkvnw2Do_f4Jk0bxo6u4QtqtKPUg8,3159
+generated/volumes/models/v1_volume.py,sha256=KZYCKznCxGoaBs73VBldqPM08XUGMZPHdpogRYgXZP0,3323
+generated/volumes/models/v1_volume_status.py,sha256=89HA9MRA0wASEx-zZBAvIu-iG4CqYk8BJwkx6-qmv7E,951
 generated/volumes/models/volume_service_change_revision_body.py,sha256=Yrja2cZ7LJsvS8VwE_xOvM3Unci4yqGbY23B3eX7lZU,2517
 generated/volumes/models/volume_service_commit_file_body.py,sha256=P9_TNgTOZ9uqhiI7rSmN1hOrMgZ6aDhKfrhMi-7UmV0,2809
 generated/volumes/models/volume_service_commit_file_body_file.py,sha256=Tv4l_uFW6bi0zPF3c4pc7_DbeOsxKbsnZoyCUgAKxRc,3055
 generated/volumes/models/volume_service_commit_revision_body.py,sha256=u9fiWxIWUCvaixLBHvdzTB_EMN4pq4cJtjgq7vhXaVg,2876
 generated/volumes/models/volume_service_complete_multipart_upload_body.py,sha256=V9helU9BPDjtaKvqPt4gYDz18rYAXsq_gDPTgXICWOs,3092
 generated/volumes/models/volume_service_create_body.py,sha256=ueROsf7ugT3Jt0rLnsb6j4RU6AHqz6D8nwwLkCOhvn8,2464
 generated/volumes/models/volume_service_initialize_multipart_upload_body.py,sha256=JVwsxNKH-DI9BpOQuDlvFvSEGHXnDKn7KmmGRaxc1KI,2801
@@ -397,23 +400,24 @@
 generated/volumes/test/test_v1_list_response.py,sha256=DSBBxq6iTS83YvgokiQ2feX9TB0VmQ0impRGnJY4-aI,2073
 generated/volumes/test/test_v1_part.py,sha256=eNdcJAgDmARSEPVEd3f4fKnu7_-jvLT3egCLkLwu3Rg,1486
 generated/volumes/test/test_v1_revision.py,sha256=8FcKpKHZ0XlRfzob7nc97q7aHw7rdW_sJ4FLwvvIeb4,1609
 generated/volumes/test/test_v1_sign_response.py,sha256=vS6QYPcpRH8pPSlE99xSG9f1qQlrW1z6NylOzgyDJ4A,1722
 generated/volumes/test/test_v1_sign_upload_response.py,sha256=wDYzXY_GfpnKsFYdo7SRcJU2HZtjUAA98q1w4btVkNE,1952
 generated/volumes/test/test_v1_upload_action.py,sha256=dQbCBFuGKce38jSeOkpeyH0xF5iopXJ0lvj3sd6Lo0U,779
 generated/volumes/test/test_v1_volume.py,sha256=AIju8B0JDFJIY78kHusiAZUSayGYUdnE-qNgcRlFnUo,1795
+generated/volumes/test/test_v1_volume_status.py,sha256=wo0T1jPXj2FnWugeIEs7RQdQG2PlzjbXrwlPsMGFM0k,779
 generated/volumes/test/test_volume_service_api.py,sha256=rEvl4U6iWHSOtMe82jrYKFK60Sris6cq7EBYf6f4cVw,3607
 generated/volumes/test/test_volume_service_change_revision_body.py,sha256=XUw55YHlM24Q_g0ma0W3lHzJ6qhKyys0meMS2srnLqQ,1712
 generated/volumes/test/test_volume_service_commit_file_body.py,sha256=y0k41kmE_g0xrWhuYI1A3P6C-z6g7adIDnZ7syiZiQ0,2004
 generated/volumes/test/test_volume_service_commit_file_body_file.py,sha256=F4jWVTlpo82x5j68w3hYpaHvaUZhCiFrmBSo1SVZOu0,1912
 generated/volumes/test/test_volume_service_commit_revision_body.py,sha256=UizO6O0rY4b9isgc_d2lKBUwTlCn0kiefccAD86nCcs,2548
 generated/volumes/test/test_volume_service_complete_multipart_upload_body.py,sha256=Ek6ZP78kDn1ol-guEmhm2zA42c_6XkArQf8G-_L5MgI,2233
 generated/volumes/test/test_volume_service_create_body.py,sha256=2MA4PEVNwPpMGuvpwMu4qeYvDAjrZjyUaeuo9p3qJ1c,1624
 generated/volumes/test/test_volume_service_initialize_multipart_upload_body.py,sha256=G58739S9489bMEXfaefcWch_GqgV-PTw4QCewOzxhSs,2149
 generated/volumes/test/test_volume_service_sign_multipart_upload_body.py,sha256=3b5ULrWgH38nEWU0s_MISEyj4j6LV8doFAx3CfQ6XjY,1769
 generated/volumes/test/test_volume_service_sign_upload_body.py,sha256=xX2B1LCvIu0OHX0AkyL8dXPClBTDgmZwmgPJOjjz96g,1968
-everai-0.1.46.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-everai-0.1.46.dist-info/METADATA,sha256=o8GsLyvM25hp3OMgKq8WmkmrniojE96eDYAFIpehUc8,1951
-everai-0.1.46.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-everai-0.1.46.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
-everai-0.1.46.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
-everai-0.1.46.dist-info/RECORD,,
+everai-0.1.47.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+everai-0.1.47.dist-info/METADATA,sha256=sLWiJ_yhBHebDOIdtAPQm14RLufCq06a94EsBMiAxL8,1951
+everai-0.1.47.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+everai-0.1.47.dist-info/entry_points.txt,sha256=JB8rwg4N4ctezo4f9O0QbWJkivM_s-wUhOn0mPM9xug,98
+everai-0.1.47.dist-info/top_level.txt,sha256=UNE90t4nA-FVpeYLiqPcJVSFyaKbZ-ERHUNI0Qd6co8,17
+everai-0.1.47.dist-info/RECORD,,
```

