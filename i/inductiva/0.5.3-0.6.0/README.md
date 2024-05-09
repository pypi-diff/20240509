# Comparing `tmp/inductiva-0.5.3.tar.gz` & `tmp/inductiva-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inductiva-0.5.3.tar", last modified: Wed Mar 27 17:33:17 2024, max compression
+gzip compressed data, was "inductiva-0.6.0.tar", last modified: Thu May  9 12:13:45 2024, max compression
```

## Comparing `inductiva-0.5.3.tar` & `inductiva-0.6.0.tar`

### file list

```diff
@@ -1,319 +1,374 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.678771 inductiva-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 17:33:05.000000 inductiva-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-27 17:33:05.000000 inductiva-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-27 17:33:17.678771 inductiva-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-03-27 17:33:05.000000 inductiva-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.638771 inductiva-0.5.3/inductiva/
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.642771 inductiva-0.5.3/inductiva/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/ansi_pager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.642771 inductiva-0.5.3/inductiva/_cli/cmd_autocomplete/
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_autocomplete/enable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.642771 inductiva-0.5.3/inductiva/_cli/cmd_logs/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_logs/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.642771 inductiva-0.5.3/inductiva/_cli/cmd_resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_resources/_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_resources/cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_resources/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_resources/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.642771 inductiva-0.5.3/inductiva/_cli/cmd_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_storage/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_storage/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_storage/storage_size.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.642771 inductiva-0.5.3/inductiva/_cli/cmd_tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_tasks/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_tasks/kill.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/cmd_tasks/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.642771 inductiva-0.5.3/inductiva/api/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/api/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.642771 inductiva-0.5.3/inductiva/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.634771 inductiva-0.5.3/inductiva/assets/completions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.642771 inductiva-0.5.3/inductiva/assets/completions/zsh/
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-03-27 17:33:15.000000 inductiva-0.5.3/inductiva/assets/completions/zsh/_inductiva
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/assets/inductiva-setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.646771 inductiva-0.5.3/inductiva/client/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    60864 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.646771 inductiva-0.5.3/inductiva/client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/path_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.650771 inductiva-0.5.3/inductiva/client/apis/paths/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/compute_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/compute_group_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/compute_group_mg_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/compute_group_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/compute_group_start.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/compute_group_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/compute_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/compute_machine_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/compute_price.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/compute_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/storage_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/storage_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/tasks_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/tasks_submit.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/tasks_task_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/tasks_task_id_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/tasks_task_id_kill.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/tasks_task_id_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/tasks_task_id_output_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/tasks_task_id_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/paths/version_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/tag_to_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.650771 inductiva-0.5.3/inductiva/client/apis/tags/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/tags/compute_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/tags/storage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/tags/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/apis/tags/version_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.658771 inductiva-0.5.3/inductiva/client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/backend_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/backend_version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/base_machine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/base_machine_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    37681 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/base_vm_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    29853 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/base_vm_group.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/body_upload_task_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/body_upload_task_input.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/default_machine_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/default_machine_group.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/executer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/executer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/executer_tracker_api_connection_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/executer_tracker_api_connection_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12191 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/executer_tracker_register_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/executer_tracker_register_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/file_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/http_validation_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/machine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/machine_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/output_archive_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/output_archive_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/providers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9920 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/quota.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    30945 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    24900 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/task.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/task_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/task_request.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/task_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/task_status.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/task_status_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/task_status_code.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/user.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/user_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/user_api_key.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/user_create.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/validation_error.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/version_comparison_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/version_comparison_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    45303 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/vm_group_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    35961 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/vm_group_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/vm_group_lifecycle_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/model/vm_group_lifecycle_config.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.658771 inductiva-0.5.3/inductiva/client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.658771 inductiva-0.5.3/inductiva/client/paths/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.658771 inductiva-0.5.3/inductiva/client/paths/compute_group/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group/post.py
--rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.658771 inductiva-0.5.3/inductiva/client/paths/compute_group_machine/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_machine/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_machine/delete.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.658771 inductiva-0.5.3/inductiva/client/paths/compute_group_mg_id/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_mg_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_mg_id/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)    14053 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_mg_id/patch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.658771 inductiva-0.5.3/inductiva/client/paths/compute_group_name/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_name/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_name/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_name/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.662771 inductiva-0.5.3/inductiva/client/paths/compute_group_start/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_start/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12718 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_start/post.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_start/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.662771 inductiva-0.5.3/inductiva/client/paths/compute_group_status/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11184 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_status/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_group_status/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.662771 inductiva-0.5.3/inductiva/client/paths/compute_groups/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_groups/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_groups/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.662771 inductiva-0.5.3/inductiva/client/paths/compute_machine_types/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_machine_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_machine_types/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_machine_types/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.662771 inductiva-0.5.3/inductiva/client/paths/compute_price/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_price/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_price/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_price/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.662771 inductiva-0.5.3/inductiva/client/paths/compute_type/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14836 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_type/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/compute_type/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.662771 inductiva-0.5.3/inductiva/client/paths/storage_contents/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/storage_contents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/storage_contents/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/storage_contents/delete.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/storage_contents/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/storage_contents/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.662771 inductiva-0.5.3/inductiva/client/paths/storage_size/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/storage_size/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/storage_size/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/storage_size/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.666771 inductiva-0.5.3/inductiva/client/paths/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12094 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    11522 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.666771 inductiva-0.5.3/inductiva/client/paths/tasks_auth/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_auth/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_auth/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.666771 inductiva-0.5.3/inductiva/client/paths/tasks_submit/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_submit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_submit/post.py
--rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_submit/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.666771 inductiva-0.5.3/inductiva/client/paths/tasks_task_id/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.666771 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_input/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_input/post.py
--rw-r--r--   0 runner    (1001) docker     (127)    14575 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_input/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.666771 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_kill/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_kill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_kill/post.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_kill/post.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.666771 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_output/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_output/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13737 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_output/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_output/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.666771 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_output_list/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_output_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_output_list/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_output_list/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.666771 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_status/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_status/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    10161 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/tasks_task_id_status/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.670771 inductiva-0.5.3/inductiva/client/paths/version/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/version/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/version/get.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.670771 inductiva-0.5.3/inductiva/client/paths/version_check/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/version_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/version_check/get.py
--rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/paths/version_check/get.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)   103945 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/client/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.670771 inductiva-0.5.3/inductiva/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/commands/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.670771 inductiva-0.5.3/inductiva/localization/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/localization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/localization/localization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.670771 inductiva-0.5.3/inductiva/localization/translations/
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/localization/translations/en.json
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/localization/translations/pt.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.670771 inductiva-0.5.3/inductiva/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/logs/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.670771 inductiva-0.5.3/inductiva/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/resources/machine_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/resources/machine_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/resources/machine_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/resources/machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    11433 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/resources/machines_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.674771 inductiva-0.5.3/inductiva/simulators/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/dualsphysics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/dummy_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/fds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/fenicsx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/gromacs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/openfoam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/reef3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/schism.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/simsopt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/splishsplash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/swan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/swash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/simulators/xbeach.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.674771 inductiva-0.5.3/inductiva/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/storage/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.674771 inductiva-0.5.3/inductiva/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/tasks/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/tasks/run_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/tasks/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)    18773 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/tasks/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.674771 inductiva-0.5.3/inductiva/templating/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/templating/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/templating/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/templating/renderers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.638771 inductiva-0.5.3/inductiva/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.638771 inductiva-0.5.3/inductiva/tests/templating/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.674771 inductiva-0.5.3/inductiva/tests/templating/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.674771 inductiva-0.5.3/inductiva/tests/templating/assets/folder/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/tests/templating/assets/folder/nested_template.txt.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/tests/templating/assets/template.txt.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.638771 inductiva-0.5.3/inductiva/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.674771 inductiva-0.5.3/inductiva/tests/utils/assets/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/tests/utils/assets/template.yaml.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/tests/utils/assets/template_file.txt.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.678771 inductiva-0.5.3/inductiva/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/utils/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/utils/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/utils/input_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/utils/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/utils/output_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-27 17:33:06.000000 inductiva-0.5.3/inductiva/utils/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 17:33:17.678771 inductiva-0.5.3/inductiva.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-03-27 17:33:17.000000 inductiva-0.5.3/inductiva.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-03-27 17:33:17.000000 inductiva-0.5.3/inductiva.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 17:33:17.000000 inductiva-0.5.3/inductiva.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-27 17:33:17.000000 inductiva-0.5.3/inductiva.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-27 17:33:17.000000 inductiva-0.5.3/inductiva.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-27 17:33:17.000000 inductiva-0.5.3/inductiva.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-27 17:33:06.000000 inductiva-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-27 17:33:17.678771 inductiva-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-27 17:33:06.000000 inductiva-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:45.002517 inductiva-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 12:13:08.000000 inductiva-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-09 12:13:08.000000 inductiva-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-09 12:13:45.002517 inductiva-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-09 12:13:08.000000 inductiva-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.958517 inductiva-0.6.0/inductiva/
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.958517 inductiva-0.6.0/inductiva/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13085 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/ansi_pager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.958517 inductiva-0.6.0/inductiva/_cli/cmd_autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_autocomplete/enable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.958517 inductiva-0.6.0/inductiva/_cli/cmd_logs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_logs/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.958517 inductiva-0.6.0/inductiva/_cli/cmd_quotas/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_quotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_quotas/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.958517 inductiva-0.6.0/inductiva/_cli/cmd_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_resources/_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_resources/cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_resources/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_resources/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.962517 inductiva-0.6.0/inductiva/_cli/cmd_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_storage/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_storage/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_storage/storage_size.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.962517 inductiva-0.6.0/inductiva/_cli/cmd_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_tasks/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_tasks/kill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/cmd_tasks/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.962517 inductiva-0.6.0/inductiva/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16072 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/api/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.962517 inductiva-0.6.0/inductiva/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.950517 inductiva-0.6.0/inductiva/assets/completions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.962517 inductiva-0.6.0/inductiva/assets/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (127)    12754 2024-05-09 12:13:42.000000 inductiva-0.6.0/inductiva/assets/completions/zsh/_inductiva
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/assets/inductiva-setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.962517 inductiva-0.6.0/inductiva/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60864 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.962517 inductiva-0.6.0/inductiva/client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/path_to_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.966517 inductiva-0.6.0/inductiva/client/apis/paths/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/compute_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/compute_group_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/compute_group_mg_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/compute_group_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/compute_group_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/compute_group_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/compute_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/compute_machine_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/compute_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/compute_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/projects_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/storage_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/storage_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/tasks_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/tasks_submit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/tasks_task_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/tasks_task_id_disable_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/tasks_task_id_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/tasks_task_id_input_upload_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/tasks_task_id_input_uploaded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/tasks_task_id_kill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/tasks_task_id_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/tasks_task_id_output_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/tasks_task_id_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/users_quotas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/paths/version_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/tag_to_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.970517 inductiva-0.6.0/inductiva/client/apis/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/tags/compute_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/tags/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/tags/storage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/tags/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/tags/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/apis/tags/version_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16772 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.978517 inductiva-0.6.0/inductiva/client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/autoscale_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/autoscale_policy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/backend_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/backend_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    42300 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/base_vm_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33358 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/base_vm_group.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/default_machine_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/default_machine_group.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7458 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/executer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/executer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/executer_tracker_api_connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/executer_tracker_api_connection_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/executer_tracker_register_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/executer_tracker_register_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/file_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/http_validation_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/machine_group_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/machine_group_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14170 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/machine_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/output_archive_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/output_archive_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/project.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/project_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/project_create.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/providers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9920 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/quota.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/storage_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/storage_file_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    34908 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28038 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/task.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/task_input_upload_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/task_input_upload_url.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23797 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/task_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19086 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/task_request.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/task_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/task_status.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/task_status_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/task_status_code.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/user_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/user_api_key.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/user_create.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/validation_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/version_comparison_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/version_comparison_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    53226 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/vm_group_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42024 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/vm_group_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/vm_group_lifecycle_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/model/vm_group_lifecycle_config.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.978517 inductiva-0.6.0/inductiva/client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.978517 inductiva-0.6.0/inductiva/client/paths/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.978517 inductiva-0.6.0/inductiva/client/paths/compute_group/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12738 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11964 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group/delete.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group/post.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.978517 inductiva-0.6.0/inductiva/client/paths/compute_group_machine/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11581 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_machine/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_machine/delete.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.982517 inductiva-0.6.0/inductiva/client/paths/compute_group_mg_id/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_mg_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_mg_id/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14053 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_mg_id/patch.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.982517 inductiva-0.6.0/inductiva/client/paths/compute_group_name/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10590 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_name/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_name/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.982517 inductiva-0.6.0/inductiva/client/paths/compute_group_start/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_start/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12718 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_start/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_start/post.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.982517 inductiva-0.6.0/inductiva/client/paths/compute_group_status/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11184 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_status/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10653 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_group_status/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.982517 inductiva-0.6.0/inductiva/client/paths/compute_groups/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_groups/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_groups/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.982517 inductiva-0.6.0/inductiva/client/paths/compute_machine_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_machine_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12652 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_machine_types/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_machine_types/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.982517 inductiva-0.6.0/inductiva/client/paths/compute_price/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_price/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11261 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_price/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10730 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_price/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.982517 inductiva-0.6.0/inductiva/client/paths/compute_type/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_type/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13425 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/compute_type/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.986517 inductiva-0.6.0/inductiva/client/paths/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/projects/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11290 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/projects/get.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/projects/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/projects/post.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.986517 inductiva-0.6.0/inductiva/client/paths/projects_name/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/projects_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10647 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/projects_name/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10086 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/projects_name/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.986517 inductiva-0.6.0/inductiva/client/paths/storage_contents/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/storage_contents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/storage_contents/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/storage_contents/delete.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/storage_contents/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12888 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/storage_contents/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.986517 inductiva-0.6.0/inductiva/client/paths/storage_size/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/storage_size/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/storage_size/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/storage_size/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.986517 inductiva-0.6.0/inductiva/client/paths/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11851 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.986517 inductiva-0.6.0/inductiva/client/paths/tasks_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_auth/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_auth/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.986517 inductiva-0.6.0/inductiva/client/paths/tasks_submit/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_submit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12945 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_submit/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_submit/post.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.986517 inductiva-0.6.0/inductiva/client/paths/tasks_task_id/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10596 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.990517 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_disable_logs/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_disable_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10523 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_disable_logs/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_disable_logs/post.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.990517 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16193 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input/put.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14856 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input/put.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.990517 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input_upload_url/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input_upload_url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input_upload_url/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input_upload_url/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.990517 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input_uploaded/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input_uploaded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input_uploaded/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input_uploaded/post.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.990517 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_kill/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_kill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_kill/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_kill/post.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.990517 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_output/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_output/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13737 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_output/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13175 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_output/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.990517 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_output_list/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_output_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_output_list/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_output_list/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.990517 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_status/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10540 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_status/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10161 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/tasks_task_id_status/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.990517 inductiva-0.6.0/inductiva/client/paths/users_quotas/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/users_quotas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8477 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/users_quotas/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/users_quotas/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.994517 inductiva-0.6.0/inductiva/client/paths/version/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/version/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/version/get.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.994517 inductiva-0.6.0/inductiva/client/paths/version_check/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/version_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/version_check/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/paths/version_check/get.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103945 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/client/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.994517 inductiva-0.6.0/inductiva/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/commands/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.994517 inductiva-0.6.0/inductiva/localization/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/localization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/localization/localization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.994517 inductiva-0.6.0/inductiva/localization/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/localization/translations/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/localization/translations/pt.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.994517 inductiva-0.6.0/inductiva/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/logs/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.994517 inductiva-0.6.0/inductiva/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/resources/machine_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/resources/machine_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/resources/machine_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/resources/machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11450 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/resources/machines_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.998517 inductiva-0.6.0/inductiva/simulators/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/amr_wind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/cans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/dualsphysics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/dummy_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/fds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/fenicsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/gromacs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/openfast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/openfoam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/reef3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/schism.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/simsopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/splishsplash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/swan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/swash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/simulators/xbeach.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.998517 inductiva-0.6.0/inductiva/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/storage/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.998517 inductiva-0.6.0/inductiva/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/tasks/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/tasks/run_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11144 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/tasks/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18773 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/tasks/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.998517 inductiva-0.6.0/inductiva/templating/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/templating/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8967 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/templating/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/templating/renderers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.954517 inductiva-0.6.0/inductiva/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.954517 inductiva-0.6.0/inductiva/tests/templating/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.998517 inductiva-0.6.0/inductiva/tests/templating/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.998517 inductiva-0.6.0/inductiva/tests/templating/assets/folder/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/tests/templating/assets/folder/nested_template.txt.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/tests/templating/assets/template.txt.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.954517 inductiva-0.6.0/inductiva/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:44.998517 inductiva-0.6.0/inductiva/tests/utils/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/tests/utils/assets/template.yaml.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/tests/utils/assets/template_file.txt.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:45.002517 inductiva-0.6.0/inductiva/users/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/users/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:45.002517 inductiva-0.6.0/inductiva/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/utils/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/utils/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/utils/input_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/utils/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/utils/output_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-09 12:13:09.000000 inductiva-0.6.0/inductiva/utils/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:45.002517 inductiva-0.6.0/inductiva.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-09 12:13:44.000000 inductiva-0.6.0/inductiva.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12551 2024-05-09 12:13:44.000000 inductiva-0.6.0/inductiva.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 12:13:44.000000 inductiva-0.6.0/inductiva.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 12:13:44.000000 inductiva-0.6.0/inductiva.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-09 12:13:44.000000 inductiva-0.6.0/inductiva.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-09 12:13:44.000000 inductiva-0.6.0/inductiva.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-09 12:13:09.000000 inductiva-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-09 12:13:45.002517 inductiva-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 12:13:09.000000 inductiva-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:45.002517 inductiva-0.6.0/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 12:13:09.000000 inductiva-0.6.0/tutorials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-09 12:13:09.000000 inductiva-0.6.0/tutorials/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-09 12:13:09.000000 inductiva-0.6.0/tutorials/conftest.py
```

### Comparing `inductiva-0.5.3/LICENSE` & `inductiva-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/PKG-INFO` & `inductiva-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inductiva
-Version: 0.5.3
+Version: 0.6.0
 Summary: Python client for the Inductiva API
 Home-page: https://github.com/inductiva/inductiva
 Author: Inductiva Research Labs
 Author-email: contact@inductiva.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -22,15 +22,15 @@
 Requires-Dist: tqdm
 Requires-Dist: websocket-client
 Requires-Dist: pyyaml
 
 
 [![Python package](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml/badge.svg)](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml) [![Python version](https://img.shields.io/pypi/pyversions/inductiva.svg)](https://www.python.org/downloads/) [![Documentation](https://img.shields.io/badge/Documentation-blue.svg)](https://docs.inductiva.ai/en/latest/) [![Benchmarks](https://img.shields.io/badge/Benchmarks-blue.svg)](https://benchmarks.inductiva.ai) <a href="https://pypi.org/project/inductiva/"><img src="https://img.shields.io/pypi/v/inductiva" alt="pypi version"></a> ![coverage badge](https://raw.githubusercontent.com/inductiva/inductiva/Inductiva-badges/badges/cov.svg)
 
-![linkedin_header](https://user-images.githubusercontent.com/104431973/231184851-0ce34289-593e-4832-aaa2-9aae652113f5.jpg)
+![inductiva_banner](https://github.com/inductiva/inductiva/assets/7538022/85569dd8-3beb-4ac3-8cbe-78e300a28fde)
 
 # Inductiva: a Python package for scaling simulations on the Cloud
 
 Welcome to the official Python library for the Inductiva API version **0.5**. 
 The Inductiva API allows running a set of open-source physical
 simulators on the cloud, easily parallelizing simulations, each running
 on hundreds of CPU cores.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inductiva Version: 0.5.3 Summary: Python client for
+Metadata-Version: 2.1 Name: inductiva Version: 0.6.0 Summary: Python client for
 the Inductiva API Home-page: https://github.com/inductiva/inductiva Author:
 Inductiva Research Labs Author-email: contact@inductiva.ai Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: certifi>=14.5.14 Requires-Dist:
 frozendict~=2.3.4 Requires-Dist: setuptools>=21.0.0 Requires-Dist: typing-
 extensions~=4.3.0 Requires-Dist: urllib3~=1.26.7 Requires-Dist: python-dateutil
@@ -12,22 +12,21 @@
 package.yml/badge.svg)](https://github.com/inductiva/inductiva/actions/
 workflows/python-package.yml) [![Python version](https://img.shields.io/pypi/
 pyversions/inductiva.svg)](https://www.python.org/downloads/) [![Documentation]
 (https://img.shields.io/badge/Documentation-blue.svg)](https://
 docs.inductiva.ai/en/latest/) [![Benchmarks](https://img.shields.io/badge/
 Benchmarks-blue.svg)](https://benchmarks.inductiva.ai) _[_p_y_p_i_ _v_e_r_s_i_o_n_]![coverage
 badge](https://raw.githubusercontent.com/inductiva/inductiva/Inductiva-badges/
-badges/cov.svg) ![linkedin_header](https://user-images.githubusercontent.com/
-104431973/231184851-0ce34289-593e-4832-aaa2-9aae652113f5.jpg) # Inductiva: a
-Python package for scaling simulations on the Cloud Welcome to the official
-Python library for the Inductiva API version **0.5**. The Inductiva API allows
-running a set of open-source physical simulators on the cloud, easily
-parallelizing simulations, each running on hundreds of CPU cores. Inductiva
-simplifies the complexities of cloud resource management, and software
-configuration, offering a straightforward Python interface for running
-simulations on state-of-the-art hardware. This allows scientists and engineers
-to focus their time and energy on what matters: running simulations that solve
-real problems. To find out more, check our [documentation](https://
-docs.inductiva.ai/). If you have any questions or suggestions about the API
-please [open an issue on the inductivaâs API Client GitHub repo](https://
-github.com/inductiva/inductiva/issues), or contact us via
-[support@inductiva.ai](mailto:support@inductiva.ai).
+badges/cov.svg) ![inductiva_banner](https://github.com/inductiva/inductiva/
+assets/7538022/85569dd8-3beb-4ac3-8cbe-78e300a28fde) # Inductiva: a Python
+package for scaling simulations on the Cloud Welcome to the official Python
+library for the Inductiva API version **0.5**. The Inductiva API allows running
+a set of open-source physical simulators on the cloud, easily parallelizing
+simulations, each running on hundreds of CPU cores. Inductiva simplifies the
+complexities of cloud resource management, and software configuration, offering
+a straightforward Python interface for running simulations on state-of-the-art
+hardware. This allows scientists and engineers to focus their time and energy
+on what matters: running simulations that solve real problems. To find out
+more, check our [documentation](https://docs.inductiva.ai/). If you have any
+questions or suggestions about the API please [open an issue on the
+inductivaâs API Client GitHub repo](https://github.com/inductiva/inductiva/
+issues), or contact us via [support@inductiva.ai](mailto:support@inductiva.ai).
```

### Comparing `inductiva-0.5.3/README.md` & `inductiva-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [![Python package](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml/badge.svg)](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml) [![Python version](https://img.shields.io/pypi/pyversions/inductiva.svg)](https://www.python.org/downloads/) [![Documentation](https://img.shields.io/badge/Documentation-blue.svg)](https://docs.inductiva.ai/en/latest/) [![Benchmarks](https://img.shields.io/badge/Benchmarks-blue.svg)](https://benchmarks.inductiva.ai) <a href="https://pypi.org/project/inductiva/"><img src="https://img.shields.io/pypi/v/inductiva" alt="pypi version"></a> ![coverage badge](https://raw.githubusercontent.com/inductiva/inductiva/Inductiva-badges/badges/cov.svg)
 
-![linkedin_header](https://user-images.githubusercontent.com/104431973/231184851-0ce34289-593e-4832-aaa2-9aae652113f5.jpg)
+![inductiva_banner](https://github.com/inductiva/inductiva/assets/7538022/85569dd8-3beb-4ac3-8cbe-78e300a28fde)
 
 # Inductiva: a Python package for scaling simulations on the Cloud
 
 Welcome to the official Python library for the Inductiva API version **0.5**. 
 The Inductiva API allows running a set of open-source physical
 simulators on the cloud, easily parallelizing simulations, each running
 on hundreds of CPU cores.
```

#### html2text {}

```diff
@@ -2,22 +2,21 @@
 python-package.yml/badge.svg)](https://github.com/inductiva/inductiva/actions/
 workflows/python-package.yml) [![Python version](https://img.shields.io/pypi/
 pyversions/inductiva.svg)](https://www.python.org/downloads/) [![Documentation]
 (https://img.shields.io/badge/Documentation-blue.svg)](https://
 docs.inductiva.ai/en/latest/) [![Benchmarks](https://img.shields.io/badge/
 Benchmarks-blue.svg)](https://benchmarks.inductiva.ai) _[_p_y_p_i_ _v_e_r_s_i_o_n_]![coverage
 badge](https://raw.githubusercontent.com/inductiva/inductiva/Inductiva-badges/
-badges/cov.svg) ![linkedin_header](https://user-images.githubusercontent.com/
-104431973/231184851-0ce34289-593e-4832-aaa2-9aae652113f5.jpg) # Inductiva: a
-Python package for scaling simulations on the Cloud Welcome to the official
-Python library for the Inductiva API version **0.5**. The Inductiva API allows
-running a set of open-source physical simulators on the cloud, easily
-parallelizing simulations, each running on hundreds of CPU cores. Inductiva
-simplifies the complexities of cloud resource management, and software
-configuration, offering a straightforward Python interface for running
-simulations on state-of-the-art hardware. This allows scientists and engineers
-to focus their time and energy on what matters: running simulations that solve
-real problems. To find out more, check our [documentation](https://
-docs.inductiva.ai/). If you have any questions or suggestions about the API
-please [open an issue on the inductivaâs API Client GitHub repo](https://
-github.com/inductiva/inductiva/issues), or contact us via
-[support@inductiva.ai](mailto:support@inductiva.ai).
+badges/cov.svg) ![inductiva_banner](https://github.com/inductiva/inductiva/
+assets/7538022/85569dd8-3beb-4ac3-8cbe-78e300a28fde) # Inductiva: a Python
+package for scaling simulations on the Cloud Welcome to the official Python
+library for the Inductiva API version **0.5**. The Inductiva API allows running
+a set of open-source physical simulators on the cloud, easily parallelizing
+simulations, each running on hundreds of CPU cores. Inductiva simplifies the
+complexities of cloud resource management, and software configuration, offering
+a straightforward Python interface for running simulations on state-of-the-art
+hardware. This allows scientists and engineers to focus their time and energy
+on what matters: running simulations that solve real problems. To find out
+more, check our [documentation](https://docs.inductiva.ai/). If you have any
+questions or suggestions about the API please [open an issue on the
+inductivaâs API Client GitHub repo](https://github.com/inductiva/inductiva/
+issues), or contact us via [support@inductiva.ai](mailto:support@inductiva.ai).
```

### Comparing `inductiva-0.5.3/inductiva/__init__.py` & `inductiva-0.6.0/inductiva/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from . import api
 from . import simulators
 from . import resources
 from . import storage
 from . import utils
 from . import tasks
+from . import users
 from . import logs
 from .templating import TemplateManager
 
 logs.setup()
 
 api_url = os.environ.get("INDUCTIVA_API_URL", "https://api.inductiva.ai")
 _output_dir = contextvars.ContextVar("INDUCTIVA_OUTPUT_DIR")
@@ -26,15 +27,15 @@
 absl.logging.set_verbosity(absl.logging.INFO)
 
 # Disable urllib3 warnings.
 # TODO: Verify and fix the appearance of this warning.
 urllib3_logger = logging.getLogger("urllib3.connectionpool")
 urllib3_logger.setLevel(logging.CRITICAL)
 
-__version__ = "0.5.3"
+__version__ = "0.6.0"
 
 
 def set_output_dir(new_output_dir):
     """Sets the value of `inductiva._output_dir` to `new_output_dir`"""
     _output_dir.set(new_output_dir)
```

### Comparing `inductiva-0.5.3/inductiva/_cli/ansi_pager.py` & `inductiva-0.6.0/inductiva/_cli/ansi_pager.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_autocomplete/__init__.py` & `inductiva-0.6.0/inductiva/_cli/cmd_autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_autocomplete/enable.py` & `inductiva-0.6.0/inductiva/_cli/cmd_autocomplete/enable.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_logs/__init__.py` & `inductiva-0.6.0/inductiva/_cli/cmd_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_logs/logs.py` & `inductiva-0.6.0/inductiva/_cli/cmd_logs/logs.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_resources/__init__.py` & `inductiva-0.6.0/inductiva/_cli/cmd_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_resources/_start.py` & `inductiva-0.6.0/inductiva/_cli/cmd_resources/_start.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_resources/cost.py` & `inductiva-0.6.0/inductiva/_cli/cmd_resources/cost.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_resources/list.py` & `inductiva-0.6.0/inductiva/_cli/cmd_resources/list.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_resources/terminate.py` & `inductiva-0.6.0/inductiva/_cli/cmd_resources/terminate.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_storage/__init__.py` & `inductiva-0.6.0/inductiva/_cli/cmd_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_storage/list.py` & `inductiva-0.6.0/inductiva/_cli/cmd_storage/list.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_storage/remove.py` & `inductiva-0.6.0/inductiva/_cli/cmd_storage/remove.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_storage/storage_size.py` & `inductiva-0.6.0/inductiva/_cli/cmd_storage/storage_size.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_tasks/__init__.py` & `inductiva-0.6.0/inductiva/_cli/cmd_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_tasks/download.py` & `inductiva-0.6.0/inductiva/_cli/cmd_tasks/download.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_tasks/kill.py` & `inductiva-0.6.0/inductiva/_cli/cmd_tasks/kill.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/cmd_tasks/list.py` & `inductiva-0.6.0/inductiva/_cli/cmd_tasks/list.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/loader.py` & `inductiva-0.6.0/inductiva/_cli/loader.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/main.py` & `inductiva-0.6.0/inductiva/_cli/main.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/_cli/utils.py` & `inductiva-0.6.0/inductiva/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/api/methods.py` & `inductiva-0.6.0/inductiva/api/methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,39 +5,43 @@
 """
 import os
 import pathlib
 import signal
 import time
 from urllib3.exceptions import MaxRetryError, NewConnectionError
 from contextlib import contextmanager
+import tqdm
+import tqdm.utils
+import urllib3
+import urllib3.request
 from typing import Any, Dict, List, Optional, Tuple, Type
 
 from absl import logging
 
 import inductiva
 from inductiva.client import ApiClient, ApiException, Configuration
 from inductiva.client.apis.tags.tasks_api import TasksApi
 from inductiva.client.apis.tags.version_api import VersionApi
-from inductiva.client.models import (BodyUploadTaskInput, TaskRequest,
-                                     TaskStatus)
+from inductiva.client.models import TaskRequest, TaskStatus
 from inductiva import types, constants
+from inductiva.resources.machine_types import ProviderType
 from inductiva.utils.data import (extract_output, get_validate_request_params,
                                   pack_input)
 from inductiva.utils import format_utils, files
 
 
 def validate_api_key(api_key: Optional[str]) -> Configuration:
     """Validates the API key and returns API configuration"""
     if inductiva.api_key is None:
         # pylint: disable=line-too-long
         raise ValueError(
             "No API Key specified. "
             "Please set the INDUCTIVA_API_KEY environment variable.\n"
             "More infomation at:"
-            "https://docs.inductiva.ai/")
+            "https://docs.inductiva.ai/en/latest/get_started/installation.html")
     # pylint: enable=line-too-long
 
     # Perform version check only on first invocation
     if not hasattr(validate_api_key, "version_checked"):
         compare_client_and_backend_versions(inductiva.__version__)
         validate_api_key.version_checked = True
 
@@ -92,27 +96,75 @@
                  format_utils.bytes_formatter(inputs_size))
     input_zip_path = pack_input(
         params=original_params,
         type_annotations=type_annotations,
         zip_name=task_id,
     )
 
+    zip_file_size = os.path.getsize(input_zip_path)
+    logging.info("Input archive size: %s",
+                 format_utils.bytes_formatter(zip_file_size))
+
+    logging.info("Uploading input archive...")
+
     try:
-        with open(input_zip_path, "rb") as zip_fp:
-            _ = api_instance.upload_task_input(
-                path_params={"task_id": task_id},
-                body=BodyUploadTaskInput(file=zip_fp),
+        api_response = api_instance.get_input_upload_url(
+            path_params={"task_id": task_id})
+
+        method = api_response.body["method"]
+        url = api_response.body["url"]
+        headers = {
+            "Content-Type":
+                "application/octet-stream",
+            "X-API-Key":
+                (api_instance.api_client.configuration.api_key["APIKeyHeader"])
+        }
+        logging.debug("Upload URL: %s", url)
+
+        with open(input_zip_path, "rb") as zip_fp, tqdm.tqdm(
+                total=zip_file_size,
+                unit="B",
+                unit_scale=True,
+                unit_divisor=1000,
+        ) as progress_bar:
+            # Wrap the file object so that the progress bar is updated every
+            # time a chunk is read.
+            wrapped_file = tqdm.utils.CallbackIOWrapper(
+                progress_bar.update,
+                zip_fp,
+                "read",
             )
+
+            # Use the pool_manager from the API client to send the request
+            # instead of using the generated client. This is because the
+            # generated client implementation does not support streaming
+            # the file and does not provide a way to update the progress bar.
+            pool_manager: urllib3.PoolManager = (
+                api_instance.api_client.rest_client.pool_manager)
+
+            resp = pool_manager.request(
+                method,
+                url,
+                body=wrapped_file,
+                headers=headers,
+            )
+            if resp.status != 200:
+                raise ApiException(
+                    status=resp.status,
+                    reason=resp.reason,
+                )
+
+            api_response = api_instance.notify_input_uploaded(
+                path_params={"task_id": task_id})
     except ApiException as e:
-        logging.exception(
-            "Exception when calling TasksApi->upload_task_inputs: %s", e)
+        logging.exception("Exception while uploading local input directory: %s",
+                          e)
         raise e
 
     logging.info("Local input directory successfully uploaded.")
-
     os.remove(input_zip_path)
 
 
 def download_output(
         api_instance: TasksApi,
         task_id,
         output_dir: Optional[types.Path] = None) -> Tuple[List, pathlib.Path]:
@@ -272,25 +324,27 @@
         logging.info(" >> %s", resource_pool)
     else:
         logging.info(" >> Default queue with %s machines.",
                      constants.DEFAULT_QUEUE_MACHINE_TYPE)
 
 
 def submit_task(api_instance, method_name, request_params, resource_pool,
-                storage_path_prefix, params, type_annotations):
+                storage_path_prefix, params, type_annotations,
+                provider_id: ProviderType):
     """Submit a task and send input files to the API."""
 
     resource_pool_id = None
     if resource_pool is not None:
         resource_pool_id = resource_pool.id
 
     task_request = TaskRequest(method=method_name,
                                params=request_params,
                                resource_pool=resource_pool_id,
-                               storage_path_prefix=storage_path_prefix)
+                               storage_path_prefix=storage_path_prefix,
+                               provider_id=provider_id.value)
     task = submit_request(
         api_instance=api_instance,
         request=task_request,
     )
 
     task_id = task["id"]
     log_task_info(task_id, method_name, params, resource_pool)
@@ -308,15 +362,16 @@
 
 
 def invoke_async_api(method_name: str,
                      params,
                      type_annotations: Dict[Any, Type],
                      resource_pool: Optional[
                          types.ComputationalResources] = None,
-                     storage_path_prefix: Optional[str] = "") -> str:
+                     storage_path_prefix: Optional[str] = "",
+                     provider_id: ProviderType = ProviderType.GCP) -> str:
     """Perform a task asyc and remotely via Inductiva's Web API.
 
     Submits a simulation async to the API and returns the task id.
     The flow is summarized as follows:
         1. Transform request params into the params used to
         validate permission to execute the request.
         2. Submit task via the "POST task/submit" endpoint.
@@ -328,14 +383,15 @@
             "POST task/{task_id}/input".
         4. Return task_id and leaves the simulation on the queue until resources
             become available.
 
     Args:
         request: Request sent to the API for validation.
         input_dir: Directory containing the input files to be uploaded.
+        provider_id: The provider id to use for the simulation (GCP or ICE).
 
     Return:
         Returns the task id.
     """
 
     api_config = validate_api_key(inductiva.api_key)
 
@@ -349,14 +405,15 @@
 
         task_id = submit_task(api_instance=api_instance,
                               method_name=method_name,
                               request_params=request_params,
                               resource_pool=resource_pool,
                               storage_path_prefix=storage_path_prefix,
                               params=params,
+                              provider_id=provider_id,
                               type_annotations=type_annotations)
 
     return task_id
 
 
 def compare_client_and_backend_versions(client_version: str):
     """ Compares the provided client version 7with the backend API version.
```

### Comparing `inductiva-0.5.3/inductiva/assets/completions/zsh/_inductiva` & `inductiva-0.6.0/inductiva/assets/completions/zsh/_inductiva`

 * *Files 8% similar despite different names*

```diff
@@ -3,28 +3,36 @@
 # AUTOMATICALLY GENERATED by `shtab`
 
 
 _shtab_inductiva_commands() {
   local _commands=(
     "autocomplete:Controls the autocomplete behavior for the inductiva package."
     "logs:Stream the STDOUT of a running task."
+    "quotas:Quotas management utilities."
     "resources:Computational resource management utilities."
     "storage:Remote storage management utilities."
     "tasks:Task management utilities."
   )
   _describe 'inductiva commands' _commands
 }
 
 _shtab_inductiva_autocomplete_commands() {
   local _commands=(
     "enable:Enables autocomplete for shell commands."
   )
   _describe 'inductiva autocomplete commands' _commands
 }
 
+_shtab_inductiva_quotas_commands() {
+  local _commands=(
+    "list:The \`inductiva quotas list\` command provides an overview of your quotas."
+  )
+  _describe 'inductiva quotas commands' _commands
+}
+
 _shtab_inductiva_resources_commands() {
   local _commands=(
     "available:The \`inductiva available\` command provides a utility for listing the"
     "cost:The \`inductiva cost\` command provides a utility for estimating the cost"
     "list:The \`inductiva resources list\` command provides a snapshot of your active computational resources."
     "ls:The \`inductiva resources list\` command provides a snapshot of your active computational resources."
     "terminate:The \`inductiva resources terminate\` command provides a utility for terminating"
@@ -68,14 +76,23 @@
 )
 
 _shtab_inductiva_logs_options=(
   "(- : *)"{-h,--help}"[show this help message and exit]"
   ":ID of the task for which to consume the stream.:"
 )
 
+_shtab_inductiva_quotas_options=(
+  "(- : *)"{-h,--help}"[show this help message and exit]"
+)
+
+_shtab_inductiva_quotas_list_options=(
+  "(- : *)"{-h,--help}"[show this help message and exit]"
+  {-w,--watch}"[Prompt the command every N seconds.]:watch:"
+)
+
 _shtab_inductiva_resources_options=(
   "(- : *)"{-h,--help}"[show this help message and exit]"
 )
 
 _shtab_inductiva_resources_available_options=(
   "(- : *)"{-h,--help}"[show this help message and exit]"
   {-p,--provider}"[Filter the available types by provider.]:provider:(GCP ICE)"
@@ -183,14 +200,15 @@
     inductiva)
       words=($line[1] "${words[@]}")
       (( CURRENT += 1 ))
       curcontext="${curcontext%:*:*}:_shtab_inductiva-$line[1]:"
       case $line[1] in
         autocomplete) _shtab_inductiva_autocomplete ;;
         logs) _arguments -C -s $_shtab_inductiva_logs_options ;;
+        quotas) _shtab_inductiva_quotas ;;
         resources) _shtab_inductiva_resources ;;
         storage) _shtab_inductiva_storage ;;
         tasks) _shtab_inductiva_tasks ;;
       esac
   esac
 }
 
@@ -209,14 +227,33 @@
       curcontext="${curcontext%:*:*}:_shtab_inductiva_autocomplete-$line[1]:"
       case $line[1] in
         enable) _arguments -C -s $_shtab_inductiva_autocomplete_enable_options ;;
       esac
   esac
 }
 
+_shtab_inductiva_quotas() {
+  local context state line curcontext="$curcontext" one_or_more='(-)*' remainder='(*)'
+
+  if ((${_shtab_inductiva_quotas_options[(I)${(q)one_or_more}*]} + ${_shtab_inductiva_quotas_options[(I)${(q)remainder}*]} == 0)); then  # noqa: E501
+    _shtab_inductiva_quotas_options+=(': :_shtab_inductiva_quotas_commands' '*::: :->quotas')
+  fi
+  _arguments -C -s $_shtab_inductiva_quotas_options
+
+  case $state in
+    quotas)
+      words=($line[1] "${words[@]}")
+      (( CURRENT += 1 ))
+      curcontext="${curcontext%:*:*}:_shtab_inductiva_quotas-$line[1]:"
+      case $line[1] in
+        list) _arguments -C -s $_shtab_inductiva_quotas_list_options ;;
+      esac
+  esac
+}
+
 _shtab_inductiva_resources() {
   local context state line curcontext="$curcontext" one_or_more='(-)*' remainder='(*)'
 
   if ((${_shtab_inductiva_resources_options[(I)${(q)one_or_more}*]} + ${_shtab_inductiva_resources_options[(I)${(q)remainder}*]} == 0)); then  # noqa: E501
     _shtab_inductiva_resources_options+=(': :_shtab_inductiva_resources_commands' '*::: :->resources')
   fi
   _arguments -C -s $_shtab_inductiva_resources_options
```

### Comparing `inductiva-0.5.3/inductiva/client/__init__.py` & `inductiva-0.6.0/inductiva/client/__init__.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/api_client.py` & `inductiva-0.6.0/inductiva/client/api_client.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/apis/path_to_api.py` & `inductiva-0.6.0/inductiva/client/apis/path_to_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import typing_extensions
 
 from inductiva.client.paths import PathValues
 from inductiva.client.apis.paths.tasks_auth import TasksAuth
 from inductiva.client.apis.paths.tasks_submit import TasksSubmit
+from inductiva.client.apis.paths.tasks_task_id_input_upload_url import TasksTaskIdInputUploadUrl
+from inductiva.client.apis.paths.tasks_task_id_input_uploaded import TasksTaskIdInputUploaded
 from inductiva.client.apis.paths.tasks_task_id_input import TasksTaskIdInput
 from inductiva.client.apis.paths.tasks_task_id import TasksTaskId
 from inductiva.client.apis.paths.tasks import Tasks
 from inductiva.client.apis.paths.tasks_task_id_status import TasksTaskIdStatus
 from inductiva.client.apis.paths.tasks_task_id_output_list import TasksTaskIdOutputList
 from inductiva.client.apis.paths.tasks_task_id_output import TasksTaskIdOutput
 from inductiva.client.apis.paths.tasks_task_id_kill import TasksTaskIdKill
+from inductiva.client.apis.paths.tasks_task_id_disable_logs import TasksTaskIdDisableLogs
 from inductiva.client.apis.paths.admin_users import AdminUsers
 from inductiva.client.apis.paths.admin_users_email_api_key import AdminUsersEmailApiKey
 from inductiva.client.apis.paths.admin_users_email import AdminUsersEmail
 from inductiva.client.apis.paths.admin_users_email_expiry_ts import AdminUsersEmailExpiryTs
 from inductiva.client.apis.paths.admin_users_username_tasks import AdminUsersUsernameTasks
 from inductiva.client.apis.paths.admin_groups import AdminGroups
 from inductiva.client.apis.paths.admin_groups_active import AdminGroupsActive
@@ -34,35 +37,43 @@
 from inductiva.client.apis.paths.compute_group_machine import ComputeGroupMachine
 from inductiva.client.apis.paths.compute_group_name import ComputeGroupName
 from inductiva.client.apis.paths.storage_size import StorageSize
 from inductiva.client.apis.paths.storage_contents import StorageContents
 from inductiva.client.apis.paths.version import Version
 from inductiva.client.apis.paths.version_check import VersionCheck
 from inductiva.client.apis.paths.users_quotas import UsersQuotas
+from inductiva.client.apis.paths.projects import Projects
+from inductiva.client.apis.paths.projects_name import ProjectsName
 
 PathToApi = typing_extensions.TypedDict(
     'PathToApi', {
         PathValues.TASKS_AUTH:
             TasksAuth,
         PathValues.TASKS_SUBMIT:
             TasksSubmit,
+        PathValues.TASKS_TASK_ID_INPUT_UPLOAD_URL:
+            TasksTaskIdInputUploadUrl,
+        PathValues.TASKS_TASK_ID_INPUT_UPLOADED:
+            TasksTaskIdInputUploaded,
         PathValues.TASKS_TASK_ID_INPUT:
             TasksTaskIdInput,
         PathValues.TASKS_TASK_ID:
             TasksTaskId,
         PathValues.TASKS:
             Tasks,
         PathValues.TASKS_TASK_ID_STATUS:
             TasksTaskIdStatus,
         PathValues.TASKS_TASK_ID_OUTPUT_LIST:
             TasksTaskIdOutputList,
         PathValues.TASKS_TASK_ID_OUTPUT:
             TasksTaskIdOutput,
         PathValues.TASKS_TASK_ID_KILL:
             TasksTaskIdKill,
+        PathValues.TASKS_TASK_ID_DISABLE_LOGS:
+            TasksTaskIdDisableLogs,
         PathValues.ADMIN_USERS:
             AdminUsers,
         PathValues.ADMIN_USERS_EMAIL_API_KEY:
             AdminUsersEmailApiKey,
         PathValues.ADMIN_USERS_EMAIL:
             AdminUsersEmail,
         PathValues.ADMIN_USERS_EMAIL_EXPIRY_TS:
@@ -111,35 +122,45 @@
             StorageContents,
         PathValues.VERSION:
             Version,
         PathValues.VERSIONCHECK:
             VersionCheck,
         PathValues.USERS_QUOTAS:
             UsersQuotas,
+        PathValues.PROJECTS:
+            Projects,
+        PathValues.PROJECTS_NAME:
+            ProjectsName,
     })
 
 path_to_api = PathToApi({
     PathValues.TASKS_AUTH:
         TasksAuth,
     PathValues.TASKS_SUBMIT:
         TasksSubmit,
+    PathValues.TASKS_TASK_ID_INPUT_UPLOAD_URL:
+        TasksTaskIdInputUploadUrl,
+    PathValues.TASKS_TASK_ID_INPUT_UPLOADED:
+        TasksTaskIdInputUploaded,
     PathValues.TASKS_TASK_ID_INPUT:
         TasksTaskIdInput,
     PathValues.TASKS_TASK_ID:
         TasksTaskId,
     PathValues.TASKS:
         Tasks,
     PathValues.TASKS_TASK_ID_STATUS:
         TasksTaskIdStatus,
     PathValues.TASKS_TASK_ID_OUTPUT_LIST:
         TasksTaskIdOutputList,
     PathValues.TASKS_TASK_ID_OUTPUT:
         TasksTaskIdOutput,
     PathValues.TASKS_TASK_ID_KILL:
         TasksTaskIdKill,
+    PathValues.TASKS_TASK_ID_DISABLE_LOGS:
+        TasksTaskIdDisableLogs,
     PathValues.ADMIN_USERS:
         AdminUsers,
     PathValues.ADMIN_USERS_EMAIL_API_KEY:
         AdminUsersEmailApiKey,
     PathValues.ADMIN_USERS_EMAIL:
         AdminUsersEmail,
     PathValues.ADMIN_USERS_EMAIL_EXPIRY_TS:
@@ -188,8 +209,12 @@
         StorageContents,
     PathValues.VERSION:
         Version,
     PathValues.VERSIONCHECK:
         VersionCheck,
     PathValues.USERS_QUOTAS:
         UsersQuotas,
+    PathValues.PROJECTS:
+        Projects,
+    PathValues.PROJECTS_NAME:
+        ProjectsName,
 })
```

### Comparing `inductiva-0.5.3/inductiva/client/apis/tag_to_api.py` & `inductiva-0.6.0/inductiva/client/apis/tag_to_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import typing_extensions
 
 from inductiva.client.apis.tags import TagValues
 from inductiva.client.apis.tags.compute_api import ComputeApi
+from inductiva.client.apis.tags.projects_api import ProjectsApi
 from inductiva.client.apis.tags.storage_api import StorageApi
 from inductiva.client.apis.tags.tasks_api import TasksApi
+from inductiva.client.apis.tags.users_api import UsersApi
 from inductiva.client.apis.tags.version_api import VersionApi
 
 TagToApi = typing_extensions.TypedDict(
     'TagToApi', {
         TagValues.COMPUTE: ComputeApi,
+        TagValues.PROJECTS: ProjectsApi,
         TagValues.STORAGE: StorageApi,
         TagValues.TASKS: TasksApi,
+        TagValues.USERS: UsersApi,
         TagValues.VERSION: VersionApi,
     })
 
 tag_to_api = TagToApi({
     TagValues.COMPUTE: ComputeApi,
+    TagValues.PROJECTS: ProjectsApi,
     TagValues.STORAGE: StorageApi,
     TagValues.TASKS: TasksApi,
+    TagValues.USERS: UsersApi,
     TagValues.VERSION: VersionApi,
 })
```

### Comparing `inductiva-0.5.3/inductiva/client/apis/tags/compute_api.py` & `inductiva-0.6.0/inductiva/client/apis/tags/compute_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/apis/tags/storage_api.py` & `inductiva-0.6.0/inductiva/client/apis/tags/storage_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/apis/tags/tasks_api.py` & `inductiva-0.6.0/inductiva/client/apis/tags/tasks_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,33 +4,39 @@
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
 """
 
+from inductiva.client.paths.tasks_task_id_disable_logs.post import DisableTaskLogs
 from inductiva.client.paths.tasks_task_id_output.get import DownloadTaskOutput
+from inductiva.client.paths.tasks_task_id_input_upload_url.get import GetInputUploadUrl
 from inductiva.client.paths.tasks_task_id_output_list.get import GetOutputsList
 from inductiva.client.paths.tasks_task_id.get import GetTask
 from inductiva.client.paths.tasks_task_id_status.get import GetTaskStatus
 from inductiva.client.paths.tasks.get import GetUserTasks
 from inductiva.client.paths.tasks_task_id_kill.post import KillTask
 from inductiva.client.paths.tasks_auth.get import LoggingAuthCheck
+from inductiva.client.paths.tasks_task_id_input_uploaded.post import NotifyInputUploaded
 from inductiva.client.paths.tasks_submit.post import SubmitTask
-from inductiva.client.paths.tasks_task_id_input.post import UploadTaskInput
+from inductiva.client.paths.tasks_task_id_input.put import UploadTaskInput
 
 
 class TasksApi(
+        DisableTaskLogs,
         DownloadTaskOutput,
+        GetInputUploadUrl,
         GetOutputsList,
         GetTask,
         GetTaskStatus,
         GetUserTasks,
         KillTask,
         LoggingAuthCheck,
+        NotifyInputUploaded,
         SubmitTask,
         UploadTaskInput,
 ):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `inductiva-0.5.3/inductiva/client/apis/tags/version_api.py` & `inductiva-0.6.0/inductiva/client/apis/tags/version_api.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/configuration.py` & `inductiva-0.6.0/inductiva/client/configuration.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/exceptions.py` & `inductiva-0.6.0/inductiva/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/backend_version.py` & `inductiva-0.6.0/inductiva/client/model/backend_version.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/backend_version.pyi` & `inductiva-0.6.0/inductiva/client/model/backend_version.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/base_machine_type.py` & `inductiva-0.6.0/inductiva/client/model/user.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,191 +18,172 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class BaseMachineType(schemas.DictSchema):
+class User(schemas.DictSchema):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     class MetaOapg:
         required = {
-            "machine_type",
-            "num_cpus",
-            "price",
-            "ram_gb",
+            "bucket_name",
+            "expiry_ts",
+            "email",
+            "username",
         }
 
         class properties:
-            machine_type = schemas.StrSchema
-            num_cpus = schemas.IntSchema
-            ram_gb = schemas.IntSchema
-            price = schemas.NumberSchema
-
-            class provider(schemas.EnumBase, schemas.StrSchema):
-
-                class MetaOapg:
-                    enum_value_to_name = {
-                        "GCP": "GCP",
-                        "ICE": "ICE",
-                    }
-
-                @schemas.classproperty
-                def GCP(cls):
-                    return cls("GCP")
-
-                @schemas.classproperty
-                def ICE(cls):
-                    return cls("ICE")
-
+            email = schemas.StrSchema
+            username = schemas.StrSchema
+            bucket_name = schemas.StrSchema
+            expiry_ts = schemas.DateTimeSchema
+            is_admin = schemas.BoolSchema
             __annotations__ = {
-                "machine_type": machine_type,
-                "num_cpus": num_cpus,
-                "ram_gb": ram_gb,
-                "price": price,
-                "provider": provider,
+                "email": email,
+                "username": username,
+                "bucket_name": bucket_name,
+                "expiry_ts": expiry_ts,
+                "is_admin": is_admin,
             }
 
-    machine_type: MetaOapg.properties.machine_type
-    num_cpus: MetaOapg.properties.num_cpus
-    price: MetaOapg.properties.price
-    ram_gb: MetaOapg.properties.ram_gb
+    bucket_name: MetaOapg.properties.bucket_name
+    expiry_ts: MetaOapg.properties.expiry_ts
+    email: MetaOapg.properties.email
+    username: MetaOapg.properties.username
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["machine_type"]
-    ) -> MetaOapg.properties.machine_type:
+            self, name: typing_extensions.Literal["email"]
+    ) -> MetaOapg.properties.email:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["num_cpus"]
-    ) -> MetaOapg.properties.num_cpus:
+        self, name: typing_extensions.Literal["username"]
+    ) -> MetaOapg.properties.username:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["ram_gb"]
-    ) -> MetaOapg.properties.ram_gb:
+        self, name: typing_extensions.Literal["bucket_name"]
+    ) -> MetaOapg.properties.bucket_name:
         ...
 
     @typing.overload
     def __getitem__(
-            self, name: typing_extensions.Literal["price"]
-    ) -> MetaOapg.properties.price:
+        self, name: typing_extensions.Literal["expiry_ts"]
+    ) -> MetaOapg.properties.expiry_ts:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["provider"]
-    ) -> MetaOapg.properties.provider:
+        self, name: typing_extensions.Literal["is_admin"]
+    ) -> MetaOapg.properties.is_admin:
         ...
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
     def __getitem__(self, name: typing.Union[typing_extensions.Literal[
-        "machine_type",
-        "num_cpus",
-        "ram_gb",
-        "price",
-        "provider",
+        "email",
+        "username",
+        "bucket_name",
+        "expiry_ts",
+        "is_admin",
     ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["machine_type"]
-    ) -> MetaOapg.properties.machine_type:
+            self, name: typing_extensions.Literal["email"]
+    ) -> MetaOapg.properties.email:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["num_cpus"]
-    ) -> MetaOapg.properties.num_cpus:
+        self, name: typing_extensions.Literal["username"]
+    ) -> MetaOapg.properties.username:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["ram_gb"]
-    ) -> MetaOapg.properties.ram_gb:
+        self, name: typing_extensions.Literal["bucket_name"]
+    ) -> MetaOapg.properties.bucket_name:
         ...
 
     @typing.overload
     def get_item_oapg(
-            self, name: typing_extensions.Literal["price"]
-    ) -> MetaOapg.properties.price:
+        self, name: typing_extensions.Literal["expiry_ts"]
+    ) -> MetaOapg.properties.expiry_ts:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["provider"]
-    ) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]:
+        self, name: typing_extensions.Literal["is_admin"]
+    ) -> typing.Union[MetaOapg.properties.is_admin, schemas.Unset]:
         ...
 
     @typing.overload
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
     def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
-        "machine_type",
-        "num_cpus",
-        "ram_gb",
-        "price",
-        "provider",
+        "email",
+        "username",
+        "bucket_name",
+        "expiry_ts",
+        "is_admin",
     ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *_args: typing.Union[
             dict,
             frozendict.frozendict,
         ],
-        machine_type: typing.Union[
-            MetaOapg.properties.machine_type,
+        bucket_name: typing.Union[
+            MetaOapg.properties.bucket_name,
             str,
         ],
-        num_cpus: typing.Union[
-            MetaOapg.properties.num_cpus,
-            decimal.Decimal,
-            int,
+        expiry_ts: typing.Union[
+            MetaOapg.properties.expiry_ts,
+            str,
+            datetime,
         ],
-        price: typing.Union[
-            MetaOapg.properties.price,
-            decimal.Decimal,
-            int,
-            float,
+        email: typing.Union[
+            MetaOapg.properties.email,
+            str,
         ],
-        ram_gb: typing.Union[
-            MetaOapg.properties.ram_gb,
-            decimal.Decimal,
-            int,
+        username: typing.Union[
+            MetaOapg.properties.username,
+            str,
         ],
-        provider: typing.Union[MetaOapg.properties.provider, str,
+        is_admin: typing.Union[MetaOapg.properties.is_admin, bool,
                                schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
-    ) -> 'BaseMachineType':
+    ) -> 'User':
         return super().__new__(
             cls,
             *_args,
-            machine_type=machine_type,
-            num_cpus=num_cpus,
-            price=price,
-            ram_gb=ram_gb,
-            provider=provider,
+            bucket_name=bucket_name,
+            expiry_ts=expiry_ts,
+            email=email,
+            username=username,
+            is_admin=is_admin,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/client/model/base_machine_type.pyi` & `inductiva-0.6.0/inductiva/client/model/output_archive_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # coding: utf-8
-
 """
     InductivaWebAPI
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
@@ -19,124 +18,135 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class BaseMachineType(
-    schemas.DictSchema
-):
+class OutputArchiveInfo(schemas.DictSchema):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
-
     class MetaOapg:
         required = {
-            "machine_type",
-            "num_cpus",
-            "price",
-            "ram_gb",
+            "size",
+            "contents",
         }
-        
+
         class properties:
-            machine_type = schemas.StrSchema
-            num_cpus = schemas.IntSchema
-            ram_gb = schemas.IntSchema
-            price = schemas.NumberSchema
-            
-            
-            class provider(
-                schemas.EnumBase,
-                schemas.StrSchema
-            ):
-                
-                @schemas.classproperty
-                def GCP(cls):
-                    return cls("GCP")
-                
-                @schemas.classproperty
-                def ICE(cls):
-                    return cls("ICE")
+            size = schemas.IntSchema
+
+            class contents(schemas.ListSchema):
+
+                class MetaOapg:
+
+                    @staticmethod
+                    def items() -> typing.Type['FileInfo']:
+                        return FileInfo
+
+                def __new__(
+                    cls,
+                    _arg: typing.Union[typing.Tuple['FileInfo'],
+                                       typing.List['FileInfo']],
+                    _configuration: typing.Optional[
+                        schemas.Configuration] = None,
+                ) -> 'contents':
+                    return super().__new__(
+                        cls,
+                        _arg,
+                        _configuration=_configuration,
+                    )
+
+                def __getitem__(self, i: int) -> 'FileInfo':
+                    return super().__getitem__(i)
+
             __annotations__ = {
-                "machine_type": machine_type,
-                "num_cpus": num_cpus,
-                "ram_gb": ram_gb,
-                "price": price,
-                "provider": provider,
+                "size": size,
+                "contents": contents,
             }
-    
-    machine_type: MetaOapg.properties.machine_type
-    num_cpus: MetaOapg.properties.num_cpus
-    price: MetaOapg.properties.price
-    ram_gb: MetaOapg.properties.ram_gb
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["machine_type"]) -> MetaOapg.properties.machine_type: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["num_cpus"]) -> MetaOapg.properties.num_cpus: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["ram_gb"]) -> MetaOapg.properties.ram_gb: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["price"]) -> MetaOapg.properties.price: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["machine_type", "num_cpus", "ram_gb", "price", "provider", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["machine_type"]) -> MetaOapg.properties.machine_type: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["num_cpus"]) -> MetaOapg.properties.num_cpus: ...
-    
+
+    size: MetaOapg.properties.size
+    contents: MetaOapg.properties.contents
+
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["ram_gb"]) -> MetaOapg.properties.ram_gb: ...
-    
+    def __getitem__(
+            self, name: typing_extensions.Literal["size"]
+    ) -> MetaOapg.properties.size:
+        ...
+
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["price"]) -> MetaOapg.properties.price: ...
-    
+    def __getitem__(
+        self, name: typing_extensions.Literal["contents"]
+    ) -> MetaOapg.properties.contents:
+        ...
+
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
-    
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
+        ...
+
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal[
+        "size",
+        "contents",
+    ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+
     @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["machine_type", "num_cpus", "ram_gb", "price", "provider", ], str]):
+    def get_item_oapg(
+            self, name: typing_extensions.Literal["size"]
+    ) -> MetaOapg.properties.size:
+        ...
+
+    @typing.overload
+    def get_item_oapg(
+        self, name: typing_extensions.Literal["contents"]
+    ) -> MetaOapg.properties.contents:
+        ...
+
+    @typing.overload
+    def get_item_oapg(
+            self, name: str
+    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+        ...
+
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
+        "size",
+        "contents",
+    ], str]):
         return super().get_item_oapg(name)
-    
 
     def __new__(
         cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        machine_type: typing.Union[MetaOapg.properties.machine_type, str, ],
-        num_cpus: typing.Union[MetaOapg.properties.num_cpus, decimal.Decimal, int, ],
-        price: typing.Union[MetaOapg.properties.price, decimal.Decimal, int, float, ],
-        ram_gb: typing.Union[MetaOapg.properties.ram_gb, decimal.Decimal, int, ],
-        provider: typing.Union[MetaOapg.properties.provider, str, schemas.Unset] = schemas.unset,
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        size: typing.Union[
+            MetaOapg.properties.size,
+            decimal.Decimal,
+            int,
+        ],
+        contents: typing.Union[
+            MetaOapg.properties.contents,
+            list,
+            tuple,
+        ],
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'BaseMachineType':
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
+                               frozendict.frozendict, str, date, datetime,
+                               uuid.UUID, int, float, decimal.Decimal, None,
+                               list, tuple, bytes],
+    ) -> 'OutputArchiveInfo':
         return super().__new__(
             cls,
             *_args,
-            machine_type=machine_type,
-            num_cpus=num_cpus,
-            price=price,
-            ram_gb=ram_gb,
-            provider=provider,
+            size=size,
+            contents=contents,
             _configuration=_configuration,
             **kwargs,
         )
+
+
+from inductiva.client.model.file_info import FileInfo
```

### Comparing `inductiva-0.5.3/inductiva/client/model/base_vm_group.py` & `inductiva-0.6.0/inductiva/client/model/base_vm_group.py`

 * *Files 7% similar despite different names*

```diff
@@ -614,64 +614,137 @@
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
 
-            class type(schemas.EnumBase, schemas.StrSchema):
+            class type(
+                    schemas.ComposedSchema,):
 
                 class MetaOapg:
-                    enum_value_to_name = {
-                        "standard": "STANDARD",
-                        "mpi": "MPI",
-                        "elastic": "ELASTIC",
-                    }
-
-                @schemas.classproperty
-                def STANDARD(cls):
-                    return cls("standard")
-
-                @schemas.classproperty
-                def MPI(cls):
-                    return cls("mpi")
-
-                @schemas.classproperty
-                def ELASTIC(cls):
-                    return cls("elastic")
 
-            class provider_id(schemas.EnumBase, schemas.StrSchema):
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            MachineGroupType,
+                        ]
+
+                def __new__(
+                    cls,
+                    *_args: typing.Union[
+                        dict,
+                        frozendict.frozendict,
+                        str,
+                        date,
+                        datetime,
+                        uuid.UUID,
+                        int,
+                        float,
+                        decimal.Decimal,
+                        bool,
+                        None,
+                        list,
+                        tuple,
+                        bytes,
+                        io.FileIO,
+                        io.BufferedReader,
+                    ],
+                    _configuration: typing.Optional[
+                        schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
+                                           frozendict.frozendict, str, date,
+                                           datetime, uuid.UUID, int, float,
+                                           decimal.Decimal, None, list, tuple,
+                                           bytes],
+                ) -> 'type':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+
+            class provider_id(
+                    schemas.ComposedSchema,):
 
                 class MetaOapg:
-                    enum_value_to_name = {
-                        "GCP": "GCP",
-                        "ICE": "ICE",
-                    }
-
-                @schemas.classproperty
-                def GCP(cls):
-                    return cls("GCP")
-
-                @schemas.classproperty
-                def ICE(cls):
-                    return cls("ICE")
 
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            Providers,
+                        ]
+
+                def __new__(
+                    cls,
+                    *_args: typing.Union[
+                        dict,
+                        frozendict.frozendict,
+                        str,
+                        date,
+                        datetime,
+                        uuid.UUID,
+                        int,
+                        float,
+                        decimal.Decimal,
+                        bool,
+                        None,
+                        list,
+                        tuple,
+                        bytes,
+                        io.FileIO,
+                        io.BufferedReader,
+                    ],
+                    _configuration: typing.Optional[
+                        schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
+                                           frozendict.frozendict, str, date,
+                                           datetime, uuid.UUID, int, float,
+                                           decimal.Decimal, None, list, tuple,
+                                           bytes],
+                ) -> 'provider_id':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+
+            started = schemas.BoolSchema
             __annotations__ = {
                 "max_idle_time": max_idle_time,
                 "auto_terminate_ts": auto_terminate_ts,
                 "id": id,
                 "name": name,
                 "machine_type": machine_type,
                 "disk_size_gb": disk_size_gb,
                 "num_vms": num_vms,
                 "idle_seconds": idle_seconds,
                 "creation_timestamp": creation_timestamp,
                 "deletion_timestamp": deletion_timestamp,
                 "type": type,
                 "provider_id": provider_id,
+                "started": started,
             }
 
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["max_idle_time"]
     ) -> MetaOapg.properties.max_idle_time:
         ...
@@ -739,14 +812,20 @@
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["provider_id"]
     ) -> MetaOapg.properties.provider_id:
         ...
 
     @typing.overload
+    def __getitem__(
+        self, name: typing_extensions.Literal["started"]
+    ) -> MetaOapg.properties.started:
+        ...
+
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
     def __getitem__(self, name: typing.Union[typing_extensions.Literal[
         "max_idle_time",
         "auto_terminate_ts",
         "id",
@@ -755,14 +834,15 @@
         "disk_size_gb",
         "num_vms",
         "idle_seconds",
         "creation_timestamp",
         "deletion_timestamp",
         "type",
         "provider_id",
+        "started",
     ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["max_idle_time"]
@@ -833,14 +913,20 @@
     def get_item_oapg(
         self, name: typing_extensions.Literal["provider_id"]
     ) -> typing.Union[MetaOapg.properties.provider_id, schemas.Unset]:
         ...
 
     @typing.overload
     def get_item_oapg(
+        self, name: typing_extensions.Literal["started"]
+    ) -> typing.Union[MetaOapg.properties.started, schemas.Unset]:
+        ...
+
+    @typing.overload
+    def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
     def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
         "max_idle_time",
         "auto_terminate_ts",
@@ -850,14 +936,15 @@
         "disk_size_gb",
         "num_vms",
         "idle_seconds",
         "creation_timestamp",
         "deletion_timestamp",
         "type",
         "provider_id",
+        "started",
     ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *_args: typing.Union[
             dict,
@@ -919,18 +1006,27 @@
         deletion_timestamp: typing.Union[MetaOapg.properties.deletion_timestamp,
                                          dict, frozendict.frozendict, str, date,
                                          datetime, uuid.UUID, int, float,
                                          decimal.Decimal, bool, None, list,
                                          tuple, bytes, io.FileIO,
                                          io.BufferedReader,
                                          schemas.Unset] = schemas.unset,
-        type: typing.Union[MetaOapg.properties.type, str,
+        type: typing.Union[MetaOapg.properties.type, dict,
+                           frozendict.frozendict, str, date, datetime,
+                           uuid.UUID, int, float, decimal.Decimal, bool, None,
+                           list, tuple, bytes, io.FileIO, io.BufferedReader,
                            schemas.Unset] = schemas.unset,
-        provider_id: typing.Union[MetaOapg.properties.provider_id, str,
+        provider_id: typing.Union[MetaOapg.properties.provider_id, dict,
+                                  frozendict.frozendict, str, date, datetime,
+                                  uuid.UUID, int, float, decimal.Decimal, bool,
+                                  None, list, tuple, bytes, io.FileIO,
+                                  io.BufferedReader,
                                   schemas.Unset] = schemas.unset,
+        started: typing.Union[MetaOapg.properties.started, bool,
+                              schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
     ) -> 'BaseVMGroup':
         return super().__new__(
@@ -944,10 +1040,15 @@
             disk_size_gb=disk_size_gb,
             num_vms=num_vms,
             idle_seconds=idle_seconds,
             creation_timestamp=creation_timestamp,
             deletion_timestamp=deletion_timestamp,
             type=type,
             provider_id=provider_id,
+            started=started,
             _configuration=_configuration,
             **kwargs,
         )
+
+
+from inductiva.client.model.machine_group_type import MachineGroupType
+from inductiva.client.model.providers import Providers
```

### Comparing `inductiva-0.5.3/inductiva/client/model/base_vm_group.pyi` & `inductiva-0.6.0/inductiva/client/model/base_vm_group.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -436,56 +436,98 @@
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             
             
             class type(
-                schemas.EnumBase,
-                schemas.StrSchema
+                schemas.ComposedSchema,
             ):
-                
-                @schemas.classproperty
-                def STANDARD(cls):
-                    return cls("standard")
-                
-                @schemas.classproperty
-                def MPI(cls):
-                    return cls("mpi")
-                
-                @schemas.classproperty
-                def ELASTIC(cls):
-                    return cls("elastic")
+            
+            
+                class MetaOapg:
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            MachineGroupType,
+                        ]
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'type':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
             
             
             class provider_id(
-                schemas.EnumBase,
-                schemas.StrSchema
+                schemas.ComposedSchema,
             ):
-                
-                @schemas.classproperty
-                def GCP(cls):
-                    return cls("GCP")
-                
-                @schemas.classproperty
-                def ICE(cls):
-                    return cls("ICE")
+            
+            
+                class MetaOapg:
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            Providers,
+                        ]
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'provider_id':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+            started = schemas.BoolSchema
             __annotations__ = {
                 "max_idle_time": max_idle_time,
                 "auto_terminate_ts": auto_terminate_ts,
                 "id": id,
                 "name": name,
                 "machine_type": machine_type,
                 "disk_size_gb": disk_size_gb,
                 "num_vms": num_vms,
                 "idle_seconds": idle_seconds,
                 "creation_timestamp": creation_timestamp,
                 "deletion_timestamp": deletion_timestamp,
                 "type": type,
                 "provider_id": provider_id,
+                "started": started,
             }
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["max_idle_time"]) -> MetaOapg.properties.max_idle_time: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["auto_terminate_ts"]) -> MetaOapg.properties.auto_terminate_ts: ...
@@ -517,17 +559,20 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider_id"]) -> MetaOapg.properties.provider_id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["started"]) -> MetaOapg.properties.started: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["max_idle_time", "auto_terminate_ts", "id", "name", "machine_type", "disk_size_gb", "num_vms", "idle_seconds", "creation_timestamp", "deletion_timestamp", "type", "provider_id", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["max_idle_time", "auto_terminate_ts", "id", "name", "machine_type", "disk_size_gb", "num_vms", "idle_seconds", "creation_timestamp", "deletion_timestamp", "type", "provider_id", "started", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["max_idle_time"]) -> typing.Union[MetaOapg.properties.max_idle_time, schemas.Unset]: ...
     
@@ -561,17 +606,20 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> typing.Union[MetaOapg.properties.type, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider_id"]) -> typing.Union[MetaOapg.properties.provider_id, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["started"]) -> typing.Union[MetaOapg.properties.started, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["max_idle_time", "auto_terminate_ts", "id", "name", "machine_type", "disk_size_gb", "num_vms", "idle_seconds", "creation_timestamp", "deletion_timestamp", "type", "provider_id", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["max_idle_time", "auto_terminate_ts", "id", "name", "machine_type", "disk_size_gb", "num_vms", "idle_seconds", "creation_timestamp", "deletion_timestamp", "type", "provider_id", "started", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         max_idle_time: typing.Union[MetaOapg.properties.max_idle_time, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
@@ -580,16 +628,17 @@
         name: typing.Union[MetaOapg.properties.name, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         machine_type: typing.Union[MetaOapg.properties.machine_type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         disk_size_gb: typing.Union[MetaOapg.properties.disk_size_gb, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         num_vms: typing.Union[MetaOapg.properties.num_vms, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         idle_seconds: typing.Union[MetaOapg.properties.idle_seconds, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         creation_timestamp: typing.Union[MetaOapg.properties.creation_timestamp, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         deletion_timestamp: typing.Union[MetaOapg.properties.deletion_timestamp, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        type: typing.Union[MetaOapg.properties.type, str, schemas.Unset] = schemas.unset,
-        provider_id: typing.Union[MetaOapg.properties.provider_id, str, schemas.Unset] = schemas.unset,
+        type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        provider_id: typing.Union[MetaOapg.properties.provider_id, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        started: typing.Union[MetaOapg.properties.started, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'BaseVMGroup':
         return super().__new__(
             cls,
             *_args,
             max_idle_time=max_idle_time,
@@ -600,10 +649,14 @@
             disk_size_gb=disk_size_gb,
             num_vms=num_vms,
             idle_seconds=idle_seconds,
             creation_timestamp=creation_timestamp,
             deletion_timestamp=deletion_timestamp,
             type=type,
             provider_id=provider_id,
+            started=started,
             _configuration=_configuration,
             **kwargs,
         )
+
+from inductiva.client.model.machine_group_type import MachineGroupType
+from inductiva.client.model.providers import Providers
```

### Comparing `inductiva-0.5.3/inductiva/client/model/body_upload_task_input.py` & `inductiva-0.6.0/inductiva/client/model/user_api_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,87 +18,85 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class BodyUploadTaskInput(schemas.DictSchema):
+class UserApiKey(schemas.DictSchema):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     class MetaOapg:
         required = {
-            "file",
+            "api_key",
         }
 
         class properties:
-            file = schemas.BinarySchema
+            api_key = schemas.StrSchema
             __annotations__ = {
-                "file": file,
+                "api_key": api_key,
             }
 
-    file: MetaOapg.properties.file
+    api_key: MetaOapg.properties.api_key
 
     @typing.overload
     def __getitem__(
-            self, name: typing_extensions.Literal["file"]
-    ) -> MetaOapg.properties.file:
+        self, name: typing_extensions.Literal["api_key"]
+    ) -> MetaOapg.properties.api_key:
         ...
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
     def __getitem__(self,
                     name: typing.Union[typing_extensions.Literal[
-                        "file",
+                        "api_key",
                     ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
-            self, name: typing_extensions.Literal["file"]
-    ) -> MetaOapg.properties.file:
+        self, name: typing_extensions.Literal["api_key"]
+    ) -> MetaOapg.properties.api_key:
         ...
 
     @typing.overload
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
     def get_item_oapg(self,
                       name: typing.Union[typing_extensions.Literal[
-                          "file",
+                          "api_key",
                       ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *_args: typing.Union[
             dict,
             frozendict.frozendict,
         ],
-        file: typing.Union[
-            MetaOapg.properties.file,
-            bytes,
-            io.FileIO,
-            io.BufferedReader,
+        api_key: typing.Union[
+            MetaOapg.properties.api_key,
+            str,
         ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
-    ) -> 'BodyUploadTaskInput':
+    ) -> 'UserApiKey':
         return super().__new__(
             cls,
             *_args,
-            file=file,
+            api_key=api_key,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/client/model/body_upload_task_input.pyi` & `inductiva-0.6.0/inductiva/client/model/project_create.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -19,65 +19,70 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class BodyUploadTaskInput(
+class ProjectCreate(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
         required = {
-            "file",
+            "name",
         }
         
         class properties:
-            file = schemas.BinarySchema
+            
+            
+            class name(
+                schemas.StrSchema
+            ):
+                pass
             __annotations__ = {
-                "file": file,
+                "name": name,
             }
     
-    file: MetaOapg.properties.file
+    name: MetaOapg.properties.name
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["file"]) -> MetaOapg.properties.file: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["file", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["file"]) -> MetaOapg.properties.file: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["file", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        file: typing.Union[MetaOapg.properties.file, bytes, io.FileIO, io.BufferedReader, ],
+        name: typing.Union[MetaOapg.properties.name, str, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'BodyUploadTaskInput':
+    ) -> 'ProjectCreate':
         return super().__new__(
             cls,
             *_args,
-            file=file,
+            name=name,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/client/model/default_machine_group.py` & `inductiva-0.6.0/inductiva/client/model/default_machine_group.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/default_machine_group.pyi` & `inductiva-0.6.0/inductiva/client/model/default_machine_group.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/executer.py` & `inductiva-0.6.0/inductiva/client/model/executer.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/executer.pyi` & `inductiva-0.6.0/inductiva/client/model/executer.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/executer_tracker_api_connection_info.py` & `inductiva-0.6.0/inductiva/client/model/executer_tracker_api_connection_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,72 +30,46 @@
 
     Information sent to the executer tracker after registration.
     """
 
     class MetaOapg:
         required = {
             "redis_consumer_group",
+            "redis_stream",
             "redis_consumer_name",
-            "redis_streams",
             "uuid",
         }
 
         class properties:
             uuid = schemas.StrSchema
-
-            class redis_streams(schemas.ListSchema):
-
-                class MetaOapg:
-                    items = schemas.StrSchema
-
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[
-                        MetaOapg.items,
-                        str,
-                    ]], typing.List[typing.Union[
-                        MetaOapg.items,
-                        str,
-                    ]]],
-                    _configuration: typing.Optional[
-                        schemas.Configuration] = None,
-                ) -> 'redis_streams':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-
+            redis_stream = schemas.StrSchema
             redis_consumer_name = schemas.StrSchema
             redis_consumer_group = schemas.StrSchema
             __annotations__ = {
                 "uuid": uuid,
-                "redis_streams": redis_streams,
+                "redis_stream": redis_stream,
                 "redis_consumer_name": redis_consumer_name,
                 "redis_consumer_group": redis_consumer_group,
             }
 
     redis_consumer_group: MetaOapg.properties.redis_consumer_group
+    redis_stream: MetaOapg.properties.redis_stream
     redis_consumer_name: MetaOapg.properties.redis_consumer_name
-    redis_streams: MetaOapg.properties.redis_streams
     uuid: MetaOapg.properties.uuid
 
     @typing.overload
     def __getitem__(
             self, name: typing_extensions.Literal["uuid"]
     ) -> MetaOapg.properties.uuid:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["redis_streams"]
-    ) -> MetaOapg.properties.redis_streams:
+        self, name: typing_extensions.Literal["redis_stream"]
+    ) -> MetaOapg.properties.redis_stream:
         ...
 
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["redis_consumer_name"]
     ) -> MetaOapg.properties.redis_consumer_name:
         ...
@@ -108,31 +82,31 @@
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
     def __getitem__(self, name: typing.Union[typing_extensions.Literal[
         "uuid",
-        "redis_streams",
+        "redis_stream",
         "redis_consumer_name",
         "redis_consumer_group",
     ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
             self, name: typing_extensions.Literal["uuid"]
     ) -> MetaOapg.properties.uuid:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["redis_streams"]
-    ) -> MetaOapg.properties.redis_streams:
+        self, name: typing_extensions.Literal["redis_stream"]
+    ) -> MetaOapg.properties.redis_stream:
         ...
 
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["redis_consumer_name"]
     ) -> MetaOapg.properties.redis_consumer_name:
         ...
@@ -147,15 +121,15 @@
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
     def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
         "uuid",
-        "redis_streams",
+        "redis_stream",
         "redis_consumer_name",
         "redis_consumer_group",
     ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
@@ -163,36 +137,35 @@
             dict,
             frozendict.frozendict,
         ],
         redis_consumer_group: typing.Union[
             MetaOapg.properties.redis_consumer_group,
             str,
         ],
+        redis_stream: typing.Union[
+            MetaOapg.properties.redis_stream,
+            str,
+        ],
         redis_consumer_name: typing.Union[
             MetaOapg.properties.redis_consumer_name,
             str,
         ],
-        redis_streams: typing.Union[
-            MetaOapg.properties.redis_streams,
-            list,
-            tuple,
-        ],
         uuid: typing.Union[
             MetaOapg.properties.uuid,
             str,
         ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
     ) -> 'ExecuterTrackerAPIConnectionInfo':
         return super().__new__(
             cls,
             *_args,
             redis_consumer_group=redis_consumer_group,
+            redis_stream=redis_stream,
             redis_consumer_name=redis_consumer_name,
-            redis_streams=redis_streams,
             uuid=uuid,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/client/model/executer_tracker_api_connection_info.pyi` & `inductiva-0.6.0/inductiva/client/model/user.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -19,125 +19,111 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class ExecuterTrackerAPIConnectionInfo(
+class User(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
-
-    Information sent to the executer tracker after registration.
     """
 
 
     class MetaOapg:
         required = {
-            "redis_consumer_group",
-            "redis_consumer_name",
-            "redis_streams",
-            "uuid",
+            "bucket_name",
+            "expiry_ts",
+            "email",
+            "username",
         }
         
         class properties:
-            uuid = schemas.StrSchema
-            
-            
-            class redis_streams(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    items = schemas.StrSchema
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'redis_streams':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-            redis_consumer_name = schemas.StrSchema
-            redis_consumer_group = schemas.StrSchema
+            email = schemas.StrSchema
+            username = schemas.StrSchema
+            bucket_name = schemas.StrSchema
+            expiry_ts = schemas.DateTimeSchema
+            is_admin = schemas.BoolSchema
             __annotations__ = {
-                "uuid": uuid,
-                "redis_streams": redis_streams,
-                "redis_consumer_name": redis_consumer_name,
-                "redis_consumer_group": redis_consumer_group,
+                "email": email,
+                "username": username,
+                "bucket_name": bucket_name,
+                "expiry_ts": expiry_ts,
+                "is_admin": is_admin,
             }
     
-    redis_consumer_group: MetaOapg.properties.redis_consumer_group
-    redis_consumer_name: MetaOapg.properties.redis_consumer_name
-    redis_streams: MetaOapg.properties.redis_streams
-    uuid: MetaOapg.properties.uuid
+    bucket_name: MetaOapg.properties.bucket_name
+    expiry_ts: MetaOapg.properties.expiry_ts
+    email: MetaOapg.properties.email
+    username: MetaOapg.properties.username
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["email"]) -> MetaOapg.properties.email: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["uuid"]) -> MetaOapg.properties.uuid: ...
+    def __getitem__(self, name: typing_extensions.Literal["username"]) -> MetaOapg.properties.username: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["redis_streams"]) -> MetaOapg.properties.redis_streams: ...
+    def __getitem__(self, name: typing_extensions.Literal["bucket_name"]) -> MetaOapg.properties.bucket_name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["redis_consumer_name"]) -> MetaOapg.properties.redis_consumer_name: ...
+    def __getitem__(self, name: typing_extensions.Literal["expiry_ts"]) -> MetaOapg.properties.expiry_ts: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["redis_consumer_group"]) -> MetaOapg.properties.redis_consumer_group: ...
+    def __getitem__(self, name: typing_extensions.Literal["is_admin"]) -> MetaOapg.properties.is_admin: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["uuid", "redis_streams", "redis_consumer_name", "redis_consumer_group", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["email", "username", "bucket_name", "expiry_ts", "is_admin", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["uuid"]) -> MetaOapg.properties.uuid: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["email"]) -> MetaOapg.properties.email: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["username"]) -> MetaOapg.properties.username: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["redis_streams"]) -> MetaOapg.properties.redis_streams: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["bucket_name"]) -> MetaOapg.properties.bucket_name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["redis_consumer_name"]) -> MetaOapg.properties.redis_consumer_name: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["expiry_ts"]) -> MetaOapg.properties.expiry_ts: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["redis_consumer_group"]) -> MetaOapg.properties.redis_consumer_group: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["is_admin"]) -> typing.Union[MetaOapg.properties.is_admin, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["uuid", "redis_streams", "redis_consumer_name", "redis_consumer_group", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["email", "username", "bucket_name", "expiry_ts", "is_admin", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        redis_consumer_group: typing.Union[MetaOapg.properties.redis_consumer_group, str, ],
-        redis_consumer_name: typing.Union[MetaOapg.properties.redis_consumer_name, str, ],
-        redis_streams: typing.Union[MetaOapg.properties.redis_streams, list, tuple, ],
-        uuid: typing.Union[MetaOapg.properties.uuid, str, ],
+        bucket_name: typing.Union[MetaOapg.properties.bucket_name, str, ],
+        expiry_ts: typing.Union[MetaOapg.properties.expiry_ts, str, datetime, ],
+        email: typing.Union[MetaOapg.properties.email, str, ],
+        username: typing.Union[MetaOapg.properties.username, str, ],
+        is_admin: typing.Union[MetaOapg.properties.is_admin, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ExecuterTrackerAPIConnectionInfo':
+    ) -> 'User':
         return super().__new__(
             cls,
             *_args,
-            redis_consumer_group=redis_consumer_group,
-            redis_consumer_name=redis_consumer_name,
-            redis_streams=redis_streams,
-            uuid=uuid,
+            bucket_name=bucket_name,
+            expiry_ts=expiry_ts,
+            email=email,
+            username=username,
+            is_admin=is_admin,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/client/model/executer_tracker_register_info.py` & `inductiva-0.6.0/inductiva/client/model/executer_tracker_register_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,46 +35,18 @@
         required = {
             "vm_id",
             "memory",
             "create_time",
             "cpu_count_logical",
             "cpu_count_physical",
             "vm_name",
-            "supported_executer_types",
         }
 
         class properties:
             create_time = schemas.DateTimeSchema
-
-            class supported_executer_types(schemas.ListSchema):
-
-                class MetaOapg:
-                    items = schemas.StrSchema
-
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[
-                        MetaOapg.items,
-                        str,
-                    ]], typing.List[typing.Union[
-                        MetaOapg.items,
-                        str,
-                    ]]],
-                    _configuration: typing.Optional[
-                        schemas.Configuration] = None,
-                ) -> 'supported_executer_types':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
-
             cpu_count_logical = schemas.IntSchema
             cpu_count_physical = schemas.IntSchema
             memory = schemas.IntSchema
             vm_name = schemas.StrSchema
             vm_id = schemas.StrSchema
 
             class machine_group_id(
@@ -136,15 +108,14 @@
                         _configuration=_configuration,
                         **kwargs,
                     )
 
             mpi_cluster = schemas.BoolSchema
             __annotations__ = {
                 "create_time": create_time,
-                "supported_executer_types": supported_executer_types,
                 "cpu_count_logical": cpu_count_logical,
                 "cpu_count_physical": cpu_count_physical,
                 "memory": memory,
                 "vm_name": vm_name,
                 "vm_id": vm_id,
                 "machine_group_id": machine_group_id,
                 "mpi_cluster": mpi_cluster,
@@ -152,30 +123,23 @@
 
     vm_id: MetaOapg.properties.vm_id
     memory: MetaOapg.properties.memory
     create_time: MetaOapg.properties.create_time
     cpu_count_logical: MetaOapg.properties.cpu_count_logical
     cpu_count_physical: MetaOapg.properties.cpu_count_physical
     vm_name: MetaOapg.properties.vm_name
-    supported_executer_types: MetaOapg.properties.supported_executer_types
 
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["create_time"]
     ) -> MetaOapg.properties.create_time:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["supported_executer_types"]
-    ) -> MetaOapg.properties.supported_executer_types:
-        ...
-
-    @typing.overload
-    def __getitem__(
         self, name: typing_extensions.Literal["cpu_count_logical"]
     ) -> MetaOapg.properties.cpu_count_logical:
         ...
 
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["cpu_count_physical"]
@@ -214,15 +178,14 @@
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
     def __getitem__(self, name: typing.Union[typing_extensions.Literal[
         "create_time",
-        "supported_executer_types",
         "cpu_count_logical",
         "cpu_count_physical",
         "memory",
         "vm_name",
         "vm_id",
         "machine_group_id",
         "mpi_cluster",
@@ -234,20 +197,14 @@
     def get_item_oapg(
         self, name: typing_extensions.Literal["create_time"]
     ) -> MetaOapg.properties.create_time:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["supported_executer_types"]
-    ) -> MetaOapg.properties.supported_executer_types:
-        ...
-
-    @typing.overload
-    def get_item_oapg(
         self, name: typing_extensions.Literal["cpu_count_logical"]
     ) -> MetaOapg.properties.cpu_count_logical:
         ...
 
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["cpu_count_physical"]
@@ -288,15 +245,14 @@
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
     def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
         "create_time",
-        "supported_executer_types",
         "cpu_count_logical",
         "cpu_count_physical",
         "memory",
         "vm_name",
         "vm_id",
         "machine_group_id",
         "mpi_cluster",
@@ -333,19 +289,14 @@
             decimal.Decimal,
             int,
         ],
         vm_name: typing.Union[
             MetaOapg.properties.vm_name,
             str,
         ],
-        supported_executer_types: typing.Union[
-            MetaOapg.properties.supported_executer_types,
-            list,
-            tuple,
-        ],
         machine_group_id: typing.Union[MetaOapg.properties.machine_group_id,
                                        dict, frozendict.frozendict, str, date,
                                        datetime, uuid.UUID, int, float,
                                        decimal.Decimal, bool, None, list, tuple,
                                        bytes, io.FileIO, io.BufferedReader,
                                        schemas.Unset] = schemas.unset,
         mpi_cluster: typing.Union[MetaOapg.properties.mpi_cluster, bool,
@@ -361,13 +312,12 @@
             *_args,
             vm_id=vm_id,
             memory=memory,
             create_time=create_time,
             cpu_count_logical=cpu_count_logical,
             cpu_count_physical=cpu_count_physical,
             vm_name=vm_name,
-            supported_executer_types=supported_executer_types,
             machine_group_id=machine_group_id,
             mpi_cluster=mpi_cluster,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/client/model/executer_tracker_register_info.pyi` & `inductiva-0.6.0/inductiva/client/model/executer_tracker_register_info.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -39,42 +39,18 @@
         required = {
             "vm_id",
             "memory",
             "create_time",
             "cpu_count_logical",
             "cpu_count_physical",
             "vm_name",
-            "supported_executer_types",
         }
         
         class properties:
             create_time = schemas.DateTimeSchema
-            
-            
-            class supported_executer_types(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    items = schemas.StrSchema
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple[typing.Union[MetaOapg.items, str, ]], typing.List[typing.Union[MetaOapg.items, str, ]]],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'supported_executer_types':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> MetaOapg.items:
-                    return super().__getitem__(i)
             cpu_count_logical = schemas.IntSchema
             cpu_count_physical = schemas.IntSchema
             memory = schemas.IntSchema
             vm_name = schemas.StrSchema
             vm_id = schemas.StrSchema
             
             
@@ -116,15 +92,14 @@
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             mpi_cluster = schemas.BoolSchema
             __annotations__ = {
                 "create_time": create_time,
-                "supported_executer_types": supported_executer_types,
                 "cpu_count_logical": cpu_count_logical,
                 "cpu_count_physical": cpu_count_physical,
                 "memory": memory,
                 "vm_name": vm_name,
                 "vm_id": vm_id,
                 "machine_group_id": machine_group_id,
                 "mpi_cluster": mpi_cluster,
@@ -132,23 +107,19 @@
     
     vm_id: MetaOapg.properties.vm_id
     memory: MetaOapg.properties.memory
     create_time: MetaOapg.properties.create_time
     cpu_count_logical: MetaOapg.properties.cpu_count_logical
     cpu_count_physical: MetaOapg.properties.cpu_count_physical
     vm_name: MetaOapg.properties.vm_name
-    supported_executer_types: MetaOapg.properties.supported_executer_types
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["create_time"]) -> MetaOapg.properties.create_time: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["supported_executer_types"]) -> MetaOapg.properties.supported_executer_types: ...
-    
-    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["cpu_count_logical"]) -> MetaOapg.properties.cpu_count_logical: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["cpu_count_physical"]) -> MetaOapg.properties.cpu_count_physical: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["memory"]) -> MetaOapg.properties.memory: ...
@@ -164,26 +135,23 @@
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["mpi_cluster"]) -> MetaOapg.properties.mpi_cluster: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["create_time", "supported_executer_types", "cpu_count_logical", "cpu_count_physical", "memory", "vm_name", "vm_id", "machine_group_id", "mpi_cluster", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["create_time", "cpu_count_logical", "cpu_count_physical", "memory", "vm_name", "vm_id", "machine_group_id", "mpi_cluster", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["create_time"]) -> MetaOapg.properties.create_time: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["supported_executer_types"]) -> MetaOapg.properties.supported_executer_types: ...
-    
-    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["cpu_count_logical"]) -> MetaOapg.properties.cpu_count_logical: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["cpu_count_physical"]) -> MetaOapg.properties.cpu_count_physical: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["memory"]) -> MetaOapg.properties.memory: ...
@@ -199,41 +167,39 @@
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["mpi_cluster"]) -> typing.Union[MetaOapg.properties.mpi_cluster, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["create_time", "supported_executer_types", "cpu_count_logical", "cpu_count_physical", "memory", "vm_name", "vm_id", "machine_group_id", "mpi_cluster", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["create_time", "cpu_count_logical", "cpu_count_physical", "memory", "vm_name", "vm_id", "machine_group_id", "mpi_cluster", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         vm_id: typing.Union[MetaOapg.properties.vm_id, str, ],
         memory: typing.Union[MetaOapg.properties.memory, decimal.Decimal, int, ],
         create_time: typing.Union[MetaOapg.properties.create_time, str, datetime, ],
         cpu_count_logical: typing.Union[MetaOapg.properties.cpu_count_logical, decimal.Decimal, int, ],
         cpu_count_physical: typing.Union[MetaOapg.properties.cpu_count_physical, decimal.Decimal, int, ],
         vm_name: typing.Union[MetaOapg.properties.vm_name, str, ],
-        supported_executer_types: typing.Union[MetaOapg.properties.supported_executer_types, list, tuple, ],
         machine_group_id: typing.Union[MetaOapg.properties.machine_group_id, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         mpi_cluster: typing.Union[MetaOapg.properties.mpi_cluster, bool, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'ExecuterTrackerRegisterInfo':
         return super().__new__(
             cls,
             *_args,
             vm_id=vm_id,
             memory=memory,
             create_time=create_time,
             cpu_count_logical=cpu_count_logical,
             cpu_count_physical=cpu_count_physical,
             vm_name=vm_name,
-            supported_executer_types=supported_executer_types,
             machine_group_id=machine_group_id,
             mpi_cluster=mpi_cluster,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/client/model/file_info.py` & `inductiva-0.6.0/inductiva/client/model/file_info.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/file_info.pyi` & `inductiva-0.6.0/inductiva/client/model/file_info.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/http_validation_error.py` & `inductiva-0.6.0/inductiva/client/model/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/http_validation_error.pyi` & `inductiva-0.6.0/inductiva/client/model/http_validation_error.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/machine_type.py` & `inductiva-0.6.0/inductiva/client/model/project.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,237 +18,220 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class MachineType(schemas.DictSchema):
+class Project(schemas.DictSchema):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     class MetaOapg:
         required = {
-            "machine_type",
-            "num_cpus",
-            "price",
-            "spot",
-            "region",
-            "ram_gb",
+            "num_tasks",
+            "name",
+            "created_at",
+            "id",
         }
 
         class properties:
-            machine_type = schemas.StrSchema
-            num_cpus = schemas.IntSchema
-            ram_gb = schemas.IntSchema
-            price = schemas.NumberSchema
-            spot = schemas.BoolSchema
-            region = schemas.StrSchema
 
-            class provider(schemas.EnumBase, schemas.StrSchema):
+            class name(schemas.StrSchema):
 
                 class MetaOapg:
-                    enum_value_to_name = {
-                        "GCP": "GCP",
-                        "ICE": "ICE",
-                    }
-
-                @schemas.classproperty
-                def GCP(cls):
-                    return cls("GCP")
-
-                @schemas.classproperty
-                def ICE(cls):
-                    return cls("ICE")
+                    max_length = 128
+                    min_length = 1
 
-            __annotations__ = {
-                "machine_type": machine_type,
-                "num_cpus": num_cpus,
-                "ram_gb": ram_gb,
-                "price": price,
-                "spot": spot,
-                "region": region,
-                "provider": provider,
-            }
+            id = schemas.UUIDSchema
+            created_at = schemas.DateTimeSchema
+            num_tasks = schemas.IntSchema
 
-    machine_type: MetaOapg.properties.machine_type
-    num_cpus: MetaOapg.properties.num_cpus
-    price: MetaOapg.properties.price
-    spot: MetaOapg.properties.spot
-    region: MetaOapg.properties.region
-    ram_gb: MetaOapg.properties.ram_gb
+            class task_status_overview(schemas.DictSchema):
 
-    @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["machine_type"]
-    ) -> MetaOapg.properties.machine_type:
-        ...
+                class MetaOapg:
+                    additional_properties = schemas.IntSchema
 
-    @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["num_cpus"]
-    ) -> MetaOapg.properties.num_cpus:
-        ...
+                def __getitem__(
+                        self, name: typing.Union[
+                            str,
+                        ]) -> MetaOapg.additional_properties:
+                    # dict_instance[name] accessor
+                    return super().__getitem__(name)
+
+                def get_item_oapg(
+                        self, name: typing.Union[
+                            str,
+                        ]) -> MetaOapg.additional_properties:
+                    return super().get_item_oapg(name)
+
+                def __new__(
+                    cls,
+                    *_args: typing.Union[
+                        dict,
+                        frozendict.frozendict,
+                    ],
+                    _configuration: typing.Optional[
+                        schemas.Configuration] = None,
+                    **kwargs: typing.Union[
+                        MetaOapg.additional_properties,
+                        decimal.Decimal,
+                        int,
+                    ],
+                ) -> 'task_status_overview':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+
+            __annotations__ = {
+                "name": name,
+                "id": id,
+                "created_at": created_at,
+                "num_tasks": num_tasks,
+                "task_status_overview": task_status_overview,
+            }
+
+    num_tasks: MetaOapg.properties.num_tasks
+    name: MetaOapg.properties.name
+    created_at: MetaOapg.properties.created_at
+    id: MetaOapg.properties.id
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["ram_gb"]
-    ) -> MetaOapg.properties.ram_gb:
+            self, name: typing_extensions.Literal["name"]
+    ) -> MetaOapg.properties.name:
         ...
 
     @typing.overload
     def __getitem__(
-            self, name: typing_extensions.Literal["price"]
-    ) -> MetaOapg.properties.price:
+            self,
+            name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id:
         ...
 
     @typing.overload
     def __getitem__(
-            self, name: typing_extensions.Literal["spot"]
-    ) -> MetaOapg.properties.spot:
+        self, name: typing_extensions.Literal["created_at"]
+    ) -> MetaOapg.properties.created_at:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["region"]
-    ) -> MetaOapg.properties.region:
+        self, name: typing_extensions.Literal["num_tasks"]
+    ) -> MetaOapg.properties.num_tasks:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["provider"]
-    ) -> MetaOapg.properties.provider:
+        self, name: typing_extensions.Literal["task_status_overview"]
+    ) -> MetaOapg.properties.task_status_overview:
         ...
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
     def __getitem__(self, name: typing.Union[typing_extensions.Literal[
-        "machine_type",
-        "num_cpus",
-        "ram_gb",
-        "price",
-        "spot",
-        "region",
-        "provider",
+        "name",
+        "id",
+        "created_at",
+        "num_tasks",
+        "task_status_overview",
     ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["machine_type"]
-    ) -> MetaOapg.properties.machine_type:
-        ...
-
-    @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["num_cpus"]
-    ) -> MetaOapg.properties.num_cpus:
-        ...
-
-    @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["ram_gb"]
-    ) -> MetaOapg.properties.ram_gb:
+            self, name: typing_extensions.Literal["name"]
+    ) -> MetaOapg.properties.name:
         ...
 
     @typing.overload
     def get_item_oapg(
-            self, name: typing_extensions.Literal["price"]
-    ) -> MetaOapg.properties.price:
+            self,
+            name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id:
         ...
 
     @typing.overload
     def get_item_oapg(
-            self, name: typing_extensions.Literal["spot"]
-    ) -> MetaOapg.properties.spot:
+        self, name: typing_extensions.Literal["created_at"]
+    ) -> MetaOapg.properties.created_at:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["region"]
-    ) -> MetaOapg.properties.region:
+        self, name: typing_extensions.Literal["num_tasks"]
+    ) -> MetaOapg.properties.num_tasks:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["provider"]
-    ) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]:
+        self, name: typing_extensions.Literal["task_status_overview"]
+    ) -> typing.Union[MetaOapg.properties.task_status_overview, schemas.Unset]:
         ...
 
     @typing.overload
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
     def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
-        "machine_type",
-        "num_cpus",
-        "ram_gb",
-        "price",
-        "spot",
-        "region",
-        "provider",
+        "name",
+        "id",
+        "created_at",
+        "num_tasks",
+        "task_status_overview",
     ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *_args: typing.Union[
             dict,
             frozendict.frozendict,
         ],
-        machine_type: typing.Union[
-            MetaOapg.properties.machine_type,
-            str,
-        ],
-        num_cpus: typing.Union[
-            MetaOapg.properties.num_cpus,
+        num_tasks: typing.Union[
+            MetaOapg.properties.num_tasks,
             decimal.Decimal,
             int,
         ],
-        price: typing.Union[
-            MetaOapg.properties.price,
-            decimal.Decimal,
-            int,
-            float,
-        ],
-        spot: typing.Union[
-            MetaOapg.properties.spot,
-            bool,
+        name: typing.Union[
+            MetaOapg.properties.name,
+            str,
         ],
-        region: typing.Union[
-            MetaOapg.properties.region,
+        created_at: typing.Union[
+            MetaOapg.properties.created_at,
             str,
+            datetime,
         ],
-        ram_gb: typing.Union[
-            MetaOapg.properties.ram_gb,
-            decimal.Decimal,
-            int,
+        id: typing.Union[
+            MetaOapg.properties.id,
+            str,
+            uuid.UUID,
         ],
-        provider: typing.Union[MetaOapg.properties.provider, str,
-                               schemas.Unset] = schemas.unset,
+        task_status_overview: typing.Union[
+            MetaOapg.properties.task_status_overview, dict,
+            frozendict.frozendict, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
-    ) -> 'MachineType':
+    ) -> 'Project':
         return super().__new__(
             cls,
             *_args,
-            machine_type=machine_type,
-            num_cpus=num_cpus,
-            price=price,
-            spot=spot,
-            region=region,
-            ram_gb=ram_gb,
-            provider=provider,
+            num_tasks=num_tasks,
+            name=name,
+            created_at=created_at,
+            id=id,
+            task_status_overview=task_status_overview,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/client/model/machine_type.pyi` & `inductiva-0.6.0/inductiva/client/model/project.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -19,148 +19,144 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class MachineType(
+class Project(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
         required = {
-            "machine_type",
-            "num_cpus",
-            "price",
-            "spot",
-            "region",
-            "ram_gb",
+            "num_tasks",
+            "name",
+            "created_at",
+            "id",
         }
         
         class properties:
-            machine_type = schemas.StrSchema
-            num_cpus = schemas.IntSchema
-            ram_gb = schemas.IntSchema
-            price = schemas.NumberSchema
-            spot = schemas.BoolSchema
-            region = schemas.StrSchema
             
             
-            class provider(
-                schemas.EnumBase,
+            class name(
                 schemas.StrSchema
             ):
+                pass
+            id = schemas.UUIDSchema
+            created_at = schemas.DateTimeSchema
+            num_tasks = schemas.IntSchema
+            
+            
+            class task_status_overview(
+                schemas.DictSchema
+            ):
+            
+            
+                class MetaOapg:
+                    additional_properties = schemas.IntSchema
                 
-                @schemas.classproperty
-                def GCP(cls):
-                    return cls("GCP")
+                def __getitem__(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
+                    # dict_instance[name] accessor
+                    return super().__getitem__(name)
                 
-                @schemas.classproperty
-                def ICE(cls):
-                    return cls("ICE")
+                def get_item_oapg(self, name: typing.Union[str, ]) -> MetaOapg.additional_properties:
+                    return super().get_item_oapg(name)
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[dict, frozendict.frozendict, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[MetaOapg.additional_properties, decimal.Decimal, int, ],
+                ) -> 'task_status_overview':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
             __annotations__ = {
-                "machine_type": machine_type,
-                "num_cpus": num_cpus,
-                "ram_gb": ram_gb,
-                "price": price,
-                "spot": spot,
-                "region": region,
-                "provider": provider,
+                "name": name,
+                "id": id,
+                "created_at": created_at,
+                "num_tasks": num_tasks,
+                "task_status_overview": task_status_overview,
             }
     
-    machine_type: MetaOapg.properties.machine_type
-    num_cpus: MetaOapg.properties.num_cpus
-    price: MetaOapg.properties.price
-    spot: MetaOapg.properties.spot
-    region: MetaOapg.properties.region
-    ram_gb: MetaOapg.properties.ram_gb
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["machine_type"]) -> MetaOapg.properties.machine_type: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["num_cpus"]) -> MetaOapg.properties.num_cpus: ...
+    num_tasks: MetaOapg.properties.num_tasks
+    name: MetaOapg.properties.name
+    created_at: MetaOapg.properties.created_at
+    id: MetaOapg.properties.id
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["ram_gb"]) -> MetaOapg.properties.ram_gb: ...
+    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["price"]) -> MetaOapg.properties.price: ...
+    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["spot"]) -> MetaOapg.properties.spot: ...
+    def __getitem__(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["region"]) -> MetaOapg.properties.region: ...
+    def __getitem__(self, name: typing_extensions.Literal["num_tasks"]) -> MetaOapg.properties.num_tasks: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["provider"]) -> MetaOapg.properties.provider: ...
+    def __getitem__(self, name: typing_extensions.Literal["task_status_overview"]) -> MetaOapg.properties.task_status_overview: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["machine_type", "num_cpus", "ram_gb", "price", "spot", "region", "provider", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", "id", "created_at", "num_tasks", "task_status_overview", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["machine_type"]) -> MetaOapg.properties.machine_type: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["num_cpus"]) -> MetaOapg.properties.num_cpus: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["ram_gb"]) -> MetaOapg.properties.ram_gb: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["price"]) -> MetaOapg.properties.price: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["spot"]) -> MetaOapg.properties.spot: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["created_at"]) -> MetaOapg.properties.created_at: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["region"]) -> MetaOapg.properties.region: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["num_tasks"]) -> MetaOapg.properties.num_tasks: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["provider"]) -> typing.Union[MetaOapg.properties.provider, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["task_status_overview"]) -> typing.Union[MetaOapg.properties.task_status_overview, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["machine_type", "num_cpus", "ram_gb", "price", "spot", "region", "provider", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", "id", "created_at", "num_tasks", "task_status_overview", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        machine_type: typing.Union[MetaOapg.properties.machine_type, str, ],
-        num_cpus: typing.Union[MetaOapg.properties.num_cpus, decimal.Decimal, int, ],
-        price: typing.Union[MetaOapg.properties.price, decimal.Decimal, int, float, ],
-        spot: typing.Union[MetaOapg.properties.spot, bool, ],
-        region: typing.Union[MetaOapg.properties.region, str, ],
-        ram_gb: typing.Union[MetaOapg.properties.ram_gb, decimal.Decimal, int, ],
-        provider: typing.Union[MetaOapg.properties.provider, str, schemas.Unset] = schemas.unset,
+        num_tasks: typing.Union[MetaOapg.properties.num_tasks, decimal.Decimal, int, ],
+        name: typing.Union[MetaOapg.properties.name, str, ],
+        created_at: typing.Union[MetaOapg.properties.created_at, str, datetime, ],
+        id: typing.Union[MetaOapg.properties.id, str, uuid.UUID, ],
+        task_status_overview: typing.Union[MetaOapg.properties.task_status_overview, dict, frozendict.frozendict, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'MachineType':
+    ) -> 'Project':
         return super().__new__(
             cls,
             *_args,
-            machine_type=machine_type,
-            num_cpus=num_cpus,
-            price=price,
-            spot=spot,
-            region=region,
-            ram_gb=ram_gb,
-            provider=provider,
+            num_tasks=num_tasks,
+            name=name,
+            created_at=created_at,
+            id=id,
+            task_status_overview=task_status_overview,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/client/model/output_archive_info.py` & `inductiva-0.6.0/inductiva/client/model/output_archive_info.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # coding: utf-8
+
 """
     InductivaWebAPI
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
@@ -18,135 +19,104 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class OutputArchiveInfo(schemas.DictSchema):
+class OutputArchiveInfo(
+    schemas.DictSchema
+):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
+
     class MetaOapg:
         required = {
             "size",
             "contents",
         }
-
+        
         class properties:
             size = schemas.IntSchema
-
-            class contents(schemas.ListSchema):
-
+            
+            
+            class contents(
+                schemas.ListSchema
+            ):
+            
+            
                 class MetaOapg:
-
+                    
                     @staticmethod
                     def items() -> typing.Type['FileInfo']:
                         return FileInfo
-
+            
                 def __new__(
                     cls,
-                    _arg: typing.Union[typing.Tuple['FileInfo'],
-                                       typing.List['FileInfo']],
-                    _configuration: typing.Optional[
-                        schemas.Configuration] = None,
+                    _arg: typing.Union[typing.Tuple['FileInfo'], typing.List['FileInfo']],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
                 ) -> 'contents':
                     return super().__new__(
                         cls,
                         _arg,
                         _configuration=_configuration,
                     )
-
+            
                 def __getitem__(self, i: int) -> 'FileInfo':
                     return super().__getitem__(i)
-
             __annotations__ = {
                 "size": size,
                 "contents": contents,
             }
-
+    
     size: MetaOapg.properties.size
     contents: MetaOapg.properties.contents
-
+    
     @typing.overload
-    def __getitem__(
-            self, name: typing_extensions.Literal["size"]
-    ) -> MetaOapg.properties.size:
-        ...
-
+    def __getitem__(self, name: typing_extensions.Literal["size"]) -> MetaOapg.properties.size: ...
+    
     @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["contents"]
-    ) -> MetaOapg.properties.contents:
-        ...
-
+    def __getitem__(self, name: typing_extensions.Literal["contents"]) -> MetaOapg.properties.contents: ...
+    
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
-        ...
-
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal[
-        "size",
-        "contents",
-    ], str]):
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["size", "contents", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
-
+    
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["size"]) -> MetaOapg.properties.size: ...
+    
     @typing.overload
-    def get_item_oapg(
-            self, name: typing_extensions.Literal["size"]
-    ) -> MetaOapg.properties.size:
-        ...
-
-    @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["contents"]
-    ) -> MetaOapg.properties.contents:
-        ...
-
-    @typing.overload
-    def get_item_oapg(
-            self, name: str
-    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
-        ...
-
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
-        "size",
-        "contents",
-    ], str]):
+    def get_item_oapg(self, name: typing_extensions.Literal["contents"]) -> MetaOapg.properties.contents: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["size", "contents", ], str]):
         return super().get_item_oapg(name)
+    
 
     def __new__(
         cls,
-        *_args: typing.Union[
-            dict,
-            frozendict.frozendict,
-        ],
-        size: typing.Union[
-            MetaOapg.properties.size,
-            decimal.Decimal,
-            int,
-        ],
-        contents: typing.Union[
-            MetaOapg.properties.contents,
-            list,
-            tuple,
-        ],
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, ],
+        contents: typing.Union[MetaOapg.properties.contents, list, tuple, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
-                               frozendict.frozendict, str, date, datetime,
-                               uuid.UUID, int, float, decimal.Decimal, None,
-                               list, tuple, bytes],
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'OutputArchiveInfo':
         return super().__new__(
             cls,
             *_args,
             size=size,
             contents=contents,
             _configuration=_configuration,
             **kwargs,
         )
 
-
 from inductiva.client.model.file_info import FileInfo
```

### Comparing `inductiva-0.5.3/inductiva/client/model/output_archive_info.pyi` & `inductiva-0.6.0/inductiva/client/model/task_input_upload_url.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # coding: utf-8
-
 """
     InductivaWebAPI
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
@@ -19,104 +18,108 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class OutputArchiveInfo(
-    schemas.DictSchema
-):
+class TaskInputUploadUrl(schemas.DictSchema):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
-
     class MetaOapg:
         required = {
-            "size",
-            "contents",
+            "method",
+            "url",
         }
-        
+
         class properties:
-            size = schemas.IntSchema
-            
-            
-            class contents(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['FileInfo']:
-                        return FileInfo
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple['FileInfo'], typing.List['FileInfo']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'contents':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'FileInfo':
-                    return super().__getitem__(i)
+            url = schemas.StrSchema
+            method = schemas.StrSchema
             __annotations__ = {
-                "size": size,
-                "contents": contents,
+                "url": url,
+                "method": method,
             }
-    
-    size: MetaOapg.properties.size
-    contents: MetaOapg.properties.contents
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["size"]) -> MetaOapg.properties.size: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["contents"]) -> MetaOapg.properties.contents: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["size", "contents", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
+
+    method: MetaOapg.properties.method
+    url: MetaOapg.properties.url
+
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["size"]) -> MetaOapg.properties.size: ...
-    
+    def __getitem__(
+            self,
+            name: typing_extensions.Literal["url"]) -> MetaOapg.properties.url:
+        ...
+
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["contents"]) -> MetaOapg.properties.contents: ...
-    
+    def __getitem__(
+        self, name: typing_extensions.Literal["method"]
+    ) -> MetaOapg.properties.method:
+        ...
+
     @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["size", "contents", ], str]):
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
+        ...
+
+    def __getitem__(self,
+                    name: typing.Union[typing_extensions.Literal[
+                        "url",
+                        "method",
+                    ], str]):
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+
+    @typing.overload
+    def get_item_oapg(
+            self,
+            name: typing_extensions.Literal["url"]) -> MetaOapg.properties.url:
+        ...
+
+    @typing.overload
+    def get_item_oapg(
+        self, name: typing_extensions.Literal["method"]
+    ) -> MetaOapg.properties.method:
+        ...
+
+    @typing.overload
+    def get_item_oapg(
+            self, name: str
+    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
+        ...
+
+    def get_item_oapg(self,
+                      name: typing.Union[typing_extensions.Literal[
+                          "url",
+                          "method",
+                      ], str]):
         return super().get_item_oapg(name)
-    
 
     def __new__(
         cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        size: typing.Union[MetaOapg.properties.size, decimal.Decimal, int, ],
-        contents: typing.Union[MetaOapg.properties.contents, list, tuple, ],
+        *_args: typing.Union[
+            dict,
+            frozendict.frozendict,
+        ],
+        method: typing.Union[
+            MetaOapg.properties.method,
+            str,
+        ],
+        url: typing.Union[
+            MetaOapg.properties.url,
+            str,
+        ],
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'OutputArchiveInfo':
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
+                               frozendict.frozendict, str, date, datetime,
+                               uuid.UUID, int, float, decimal.Decimal, None,
+                               list, tuple, bytes],
+    ) -> 'TaskInputUploadUrl':
         return super().__new__(
             cls,
             *_args,
-            size=size,
-            contents=contents,
+            method=method,
+            url=url,
             _configuration=_configuration,
             **kwargs,
         )
-
-from inductiva.client.model.file_info import FileInfo
```

### Comparing `inductiva-0.5.3/inductiva/client/model/provider.py` & `inductiva-0.6.0/inductiva/client/model/provider.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/provider.pyi` & `inductiva-0.6.0/inductiva/client/model/provider.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/providers.py` & `inductiva-0.6.0/inductiva/client/model/autoscale_policy.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,29 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class Providers(schemas.EnumBase, schemas.StrSchema):
+class AutoscalePolicy(schemas.EnumBase, schemas.StrSchema):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     An enumeration.
     """
 
     class MetaOapg:
         enum_value_to_name = {
-            "GCP": "GCP",
-            "ICE": "ICE",
+            "cpu": "CPU",
+            "task_in_queue": "TASK_IN_QUEUE",
         }
 
     @schemas.classproperty
-    def GCP(cls):
-        return cls("GCP")
+    def CPU(cls):
+        return cls("cpu")
 
     @schemas.classproperty
-    def ICE(cls):
-        return cls("ICE")
+    def TASK_IN_QUEUE(cls):
+        return cls("task_in_queue")
```

### Comparing `inductiva-0.5.3/inductiva/client/model/providers.pyi` & `inductiva-0.6.0/inductiva/client/model/autoscale_policy.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -19,26 +19,26 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class Providers(
+class AutoscalePolicy(
     schemas.EnumBase,
     schemas.StrSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     An enumeration.
     """
     
     @schemas.classproperty
-    def GCP(cls):
-        return cls("GCP")
+    def CPU(cls):
+        return cls("cpu")
     
     @schemas.classproperty
-    def ICE(cls):
-        return cls("ICE")
+    def TASK_IN_QUEUE(cls):
+        return cls("task_in_queue")
```

### Comparing `inductiva-0.5.3/inductiva/client/model/quota.py` & `inductiva-0.6.0/inductiva/client/model/quota.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/quota.pyi` & `inductiva-0.6.0/inductiva/client/model/quota.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/task.py` & `inductiva-0.6.0/inductiva/client/model/task.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,26 +28,28 @@
 
     Do not edit the class manually.
     """
 
     class MetaOapg:
         required = {
             "method_name",
+            "project",
             "task_id",
             "status",
         }
 
         class properties:
             task_id = schemas.StrSchema
 
             @staticmethod
             def status() -> typing.Type['TaskStatusCode']:
                 return TaskStatusCode
 
             method_name = schemas.StrSchema
+            project = schemas.StrSchema
 
             class create_time(
                     schemas.DateTimeBase,
                     schemas.ComposedSchema,
             ):
 
                 class MetaOapg:
@@ -514,29 +516,89 @@
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
 
+            class container_image(
+                    schemas.ComposedSchema,):
+
+                class MetaOapg:
+                    any_of_0 = schemas.StrSchema
+                    any_of_1 = schemas.NoneSchema
+
+                    @classmethod
+                    @functools.lru_cache()
+                    def any_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            cls.any_of_0,
+                            cls.any_of_1,
+                        ]
+
+                def __new__(
+                    cls,
+                    *_args: typing.Union[
+                        dict,
+                        frozendict.frozendict,
+                        str,
+                        date,
+                        datetime,
+                        uuid.UUID,
+                        int,
+                        float,
+                        decimal.Decimal,
+                        bool,
+                        None,
+                        list,
+                        tuple,
+                        bytes,
+                        io.FileIO,
+                        io.BufferedReader,
+                    ],
+                    _configuration: typing.Optional[
+                        schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
+                                           frozendict.frozendict, str, date,
+                                           datetime, uuid.UUID, int, float,
+                                           decimal.Decimal, None, list, tuple,
+                                           bytes],
+                ) -> 'container_image':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+
             __annotations__ = {
                 "task_id": task_id,
                 "status": status,
                 "method_name": method_name,
+                "project": project,
                 "create_time": create_time,
                 "input_submit_time": input_submit_time,
                 "start_time": start_time,
                 "computation_start_time": computation_start_time,
                 "computation_end_time": computation_end_time,
                 "end_time": end_time,
                 "executer": executer,
                 "storage_path": storage_path,
+                "container_image": container_image,
             }
 
     method_name: MetaOapg.properties.method_name
+    project: MetaOapg.properties.project
     task_id: MetaOapg.properties.task_id
     status: 'TaskStatusCode'
 
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["task_id"]
     ) -> MetaOapg.properties.task_id:
@@ -552,14 +614,20 @@
     def __getitem__(
         self, name: typing_extensions.Literal["method_name"]
     ) -> MetaOapg.properties.method_name:
         ...
 
     @typing.overload
     def __getitem__(
+        self, name: typing_extensions.Literal["project"]
+    ) -> MetaOapg.properties.project:
+        ...
+
+    @typing.overload
+    def __getitem__(
         self, name: typing_extensions.Literal["create_time"]
     ) -> MetaOapg.properties.create_time:
         ...
 
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["input_submit_time"]
@@ -599,29 +667,37 @@
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["storage_path"]
     ) -> MetaOapg.properties.storage_path:
         ...
 
     @typing.overload
+    def __getitem__(
+        self, name: typing_extensions.Literal["container_image"]
+    ) -> MetaOapg.properties.container_image:
+        ...
+
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
     def __getitem__(self, name: typing.Union[typing_extensions.Literal[
         "task_id",
         "status",
         "method_name",
+        "project",
         "create_time",
         "input_submit_time",
         "start_time",
         "computation_start_time",
         "computation_end_time",
         "end_time",
         "executer",
         "storage_path",
+        "container_image",
     ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["task_id"]
@@ -638,14 +714,20 @@
     def get_item_oapg(
         self, name: typing_extensions.Literal["method_name"]
     ) -> MetaOapg.properties.method_name:
         ...
 
     @typing.overload
     def get_item_oapg(
+        self, name: typing_extensions.Literal["project"]
+    ) -> MetaOapg.properties.project:
+        ...
+
+    @typing.overload
+    def get_item_oapg(
         self, name: typing_extensions.Literal["create_time"]
     ) -> typing.Union[MetaOapg.properties.create_time, schemas.Unset]:
         ...
 
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["input_submit_time"]
@@ -687,43 +769,55 @@
     def get_item_oapg(
         self, name: typing_extensions.Literal["storage_path"]
     ) -> typing.Union[MetaOapg.properties.storage_path, schemas.Unset]:
         ...
 
     @typing.overload
     def get_item_oapg(
+        self, name: typing_extensions.Literal["container_image"]
+    ) -> typing.Union[MetaOapg.properties.container_image, schemas.Unset]:
+        ...
+
+    @typing.overload
+    def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
     def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
         "task_id",
         "status",
         "method_name",
+        "project",
         "create_time",
         "input_submit_time",
         "start_time",
         "computation_start_time",
         "computation_end_time",
         "end_time",
         "executer",
         "storage_path",
+        "container_image",
     ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *_args: typing.Union[
             dict,
             frozendict.frozendict,
         ],
         method_name: typing.Union[
             MetaOapg.properties.method_name,
             str,
         ],
+        project: typing.Union[
+            MetaOapg.properties.project,
+            str,
+        ],
         task_id: typing.Union[
             MetaOapg.properties.task_id,
             str,
         ],
         status: 'TaskStatusCode',
         create_time: typing.Union[MetaOapg.properties.create_time, dict,
                                   frozendict.frozendict, str, date, datetime,
@@ -768,34 +862,42 @@
                                schemas.Unset] = schemas.unset,
         storage_path: typing.Union[MetaOapg.properties.storage_path, dict,
                                    frozendict.frozendict, str, date, datetime,
                                    uuid.UUID, int, float, decimal.Decimal, bool,
                                    None, list, tuple, bytes, io.FileIO,
                                    io.BufferedReader,
                                    schemas.Unset] = schemas.unset,
+        container_image: typing.Union[MetaOapg.properties.container_image, dict,
+                                      frozendict.frozendict, str, date,
+                                      datetime, uuid.UUID, int, float,
+                                      decimal.Decimal, bool, None, list, tuple,
+                                      bytes, io.FileIO, io.BufferedReader,
+                                      schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
     ) -> 'Task':
         return super().__new__(
             cls,
             *_args,
             method_name=method_name,
+            project=project,
             task_id=task_id,
             status=status,
             create_time=create_time,
             input_submit_time=input_submit_time,
             start_time=start_time,
             computation_start_time=computation_start_time,
             computation_end_time=computation_end_time,
             end_time=end_time,
             executer=executer,
             storage_path=storage_path,
+            container_image=container_image,
             _configuration=_configuration,
             **kwargs,
         )
 
 
 from inductiva.client.model.executer import Executer
 from inductiva.client.model.task_status_code import TaskStatusCode
```

### Comparing `inductiva-0.5.3/inductiva/client/model/task.pyi` & `inductiva-0.6.0/inductiva/client/model/task.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -32,25 +32,27 @@
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
         required = {
             "method_name",
+            "project",
             "task_id",
             "status",
         }
         
         class properties:
             task_id = schemas.StrSchema
         
             @staticmethod
             def status() -> typing.Type['TaskStatusCode']:
                 return TaskStatusCode
             method_name = schemas.StrSchema
+            project = schemas.StrSchema
             
             
             class create_time(
                 schemas.DateTimeBase,
                 schemas.ComposedSchema,
             ):
             
@@ -366,42 +368,87 @@
                 ) -> 'storage_path':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+            
+            
+            class container_image(
+                schemas.ComposedSchema,
+            ):
+            
+            
+                class MetaOapg:
+                    any_of_0 = schemas.StrSchema
+                    any_of_1 = schemas.NoneSchema
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def any_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            cls.any_of_0,
+                            cls.any_of_1,
+                        ]
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'container_image':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
             __annotations__ = {
                 "task_id": task_id,
                 "status": status,
                 "method_name": method_name,
+                "project": project,
                 "create_time": create_time,
                 "input_submit_time": input_submit_time,
                 "start_time": start_time,
                 "computation_start_time": computation_start_time,
                 "computation_end_time": computation_end_time,
                 "end_time": end_time,
                 "executer": executer,
                 "storage_path": storage_path,
+                "container_image": container_image,
             }
     
     method_name: MetaOapg.properties.method_name
+    project: MetaOapg.properties.project
     task_id: MetaOapg.properties.task_id
     status: 'TaskStatusCode'
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["task_id"]) -> MetaOapg.properties.task_id: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["status"]) -> 'TaskStatusCode': ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["method_name"]) -> MetaOapg.properties.method_name: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["create_time"]) -> MetaOapg.properties.create_time: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["input_submit_time"]) -> MetaOapg.properties.input_submit_time: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["start_time"]) -> MetaOapg.properties.start_time: ...
@@ -418,31 +465,37 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["executer"]) -> MetaOapg.properties.executer: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["storage_path"]) -> MetaOapg.properties.storage_path: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["container_image"]) -> MetaOapg.properties.container_image: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["task_id", "status", "method_name", "create_time", "input_submit_time", "start_time", "computation_start_time", "computation_end_time", "end_time", "executer", "storage_path", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["task_id", "status", "method_name", "project", "create_time", "input_submit_time", "start_time", "computation_start_time", "computation_end_time", "end_time", "executer", "storage_path", "container_image", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["task_id"]) -> MetaOapg.properties.task_id: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["status"]) -> 'TaskStatusCode': ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["method_name"]) -> MetaOapg.properties.method_name: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["project"]) -> MetaOapg.properties.project: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["create_time"]) -> typing.Union[MetaOapg.properties.create_time, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["input_submit_time"]) -> typing.Union[MetaOapg.properties.input_submit_time, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["start_time"]) -> typing.Union[MetaOapg.properties.start_time, schemas.Unset]: ...
@@ -459,50 +512,57 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["executer"]) -> typing.Union[MetaOapg.properties.executer, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["storage_path"]) -> typing.Union[MetaOapg.properties.storage_path, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["container_image"]) -> typing.Union[MetaOapg.properties.container_image, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["task_id", "status", "method_name", "create_time", "input_submit_time", "start_time", "computation_start_time", "computation_end_time", "end_time", "executer", "storage_path", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["task_id", "status", "method_name", "project", "create_time", "input_submit_time", "start_time", "computation_start_time", "computation_end_time", "end_time", "executer", "storage_path", "container_image", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         method_name: typing.Union[MetaOapg.properties.method_name, str, ],
+        project: typing.Union[MetaOapg.properties.project, str, ],
         task_id: typing.Union[MetaOapg.properties.task_id, str, ],
         status: 'TaskStatusCode',
         create_time: typing.Union[MetaOapg.properties.create_time, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         input_submit_time: typing.Union[MetaOapg.properties.input_submit_time, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         start_time: typing.Union[MetaOapg.properties.start_time, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         computation_start_time: typing.Union[MetaOapg.properties.computation_start_time, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         computation_end_time: typing.Union[MetaOapg.properties.computation_end_time, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         end_time: typing.Union[MetaOapg.properties.end_time, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         executer: typing.Union[MetaOapg.properties.executer, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         storage_path: typing.Union[MetaOapg.properties.storage_path, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        container_image: typing.Union[MetaOapg.properties.container_image, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'Task':
         return super().__new__(
             cls,
             *_args,
             method_name=method_name,
+            project=project,
             task_id=task_id,
             status=status,
             create_time=create_time,
             input_submit_time=input_submit_time,
             start_time=start_time,
             computation_start_time=computation_start_time,
             computation_end_time=computation_end_time,
             end_time=end_time,
             executer=executer,
             storage_path=storage_path,
+            container_image=container_image,
             _configuration=_configuration,
             **kwargs,
         )
 
 from inductiva.client.model.executer import Executer
 from inductiva.client.model.task_status_code import TaskStatusCode
```

### Comparing `inductiva-0.5.3/inductiva/client/model/task_request.py` & `inductiva-0.6.0/inductiva/client/model/machine_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,52 +18,52 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class TaskRequest(schemas.DictSchema):
+class MachineType(schemas.DictSchema):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     class MetaOapg:
         required = {
-            "method",
-            "params",
+            "machine_type",
+            "num_cpus",
+            "price",
+            "ram_gb",
         }
 
         class properties:
-            method = schemas.StrSchema
-            params = schemas.DictSchema
+            machine_type = schemas.StrSchema
+            num_cpus = schemas.IntSchema
+            ram_gb = schemas.IntSchema
+            price = schemas.NumberSchema
 
-            class resource_pool(
+            class provider_id(
                     schemas.ComposedSchema,):
 
                 class MetaOapg:
-                    format = 'uuid4'
-                    any_of_0 = schemas.StrSchema
-                    any_of_1 = schemas.NoneSchema
 
                     @classmethod
                     @functools.lru_cache()
-                    def any_of(cls):
+                    def all_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            cls.any_of_0,
-                            cls.any_of_1,
+                            Providers,
                         ]
 
                 def __new__(
                     cls,
                     *_args: typing.Union[
                         dict,
                         frozendict.frozendict,
@@ -85,27 +85,27 @@
                     _configuration: typing.Optional[
                         schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                            frozendict.frozendict, str, date,
                                            datetime, uuid.UUID, int, float,
                                            decimal.Decimal, None, list, tuple,
                                            bytes],
-                ) -> 'resource_pool':
+                ) -> 'provider_id':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
 
-            class client_version(
+            class spot(
                     schemas.ComposedSchema,):
 
                 class MetaOapg:
-                    any_of_0 = schemas.StrSchema
+                    any_of_0 = schemas.BoolSchema
                     any_of_1 = schemas.NoneSchema
 
                     @classmethod
                     @functools.lru_cache()
                     def any_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
@@ -142,23 +142,23 @@
                     _configuration: typing.Optional[
                         schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                            frozendict.frozendict, str, date,
                                            datetime, uuid.UUID, int, float,
                                            decimal.Decimal, None, list, tuple,
                                            bytes],
-                ) -> 'client_version':
+                ) -> 'spot':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
 
-            class scenario_name(
+            class region(
                     schemas.ComposedSchema,):
 
                 class MetaOapg:
                     any_of_0 = schemas.StrSchema
                     any_of_1 = schemas.NoneSchema
 
                     @classmethod
@@ -199,220 +199,211 @@
                     _configuration: typing.Optional[
                         schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                            frozendict.frozendict, str, date,
                                            datetime, uuid.UUID, int, float,
                                            decimal.Decimal, None, list, tuple,
                                            bytes],
-                ) -> 'scenario_name':
+                ) -> 'region':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
 
-            storage_path_prefix = schemas.StrSchema
-
-            class provider_id(schemas.EnumBase, schemas.StrSchema):
-
-                class MetaOapg:
-                    enum_value_to_name = {
-                        "GCP": "GCP",
-                        "ICE": "ICE",
-                    }
-
-                @schemas.classproperty
-                def GCP(cls):
-                    return cls("GCP")
-
-                @schemas.classproperty
-                def ICE(cls):
-                    return cls("ICE")
-
             __annotations__ = {
-                "method": method,
-                "params": params,
-                "resource_pool": resource_pool,
-                "client_version": client_version,
-                "scenario_name": scenario_name,
-                "storage_path_prefix": storage_path_prefix,
+                "machine_type": machine_type,
+                "num_cpus": num_cpus,
+                "ram_gb": ram_gb,
+                "price": price,
                 "provider_id": provider_id,
+                "spot": spot,
+                "region": region,
             }
 
-    method: MetaOapg.properties.method
-    params: MetaOapg.properties.params
+    machine_type: MetaOapg.properties.machine_type
+    num_cpus: MetaOapg.properties.num_cpus
+    price: MetaOapg.properties.price
+    ram_gb: MetaOapg.properties.ram_gb
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["method"]
-    ) -> MetaOapg.properties.method:
+        self, name: typing_extensions.Literal["machine_type"]
+    ) -> MetaOapg.properties.machine_type:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["params"]
-    ) -> MetaOapg.properties.params:
+        self, name: typing_extensions.Literal["num_cpus"]
+    ) -> MetaOapg.properties.num_cpus:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["resource_pool"]
-    ) -> MetaOapg.properties.resource_pool:
+        self, name: typing_extensions.Literal["ram_gb"]
+    ) -> MetaOapg.properties.ram_gb:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["client_version"]
-    ) -> MetaOapg.properties.client_version:
+            self, name: typing_extensions.Literal["price"]
+    ) -> MetaOapg.properties.price:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["scenario_name"]
-    ) -> MetaOapg.properties.scenario_name:
+        self, name: typing_extensions.Literal["provider_id"]
+    ) -> MetaOapg.properties.provider_id:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["storage_path_prefix"]
-    ) -> MetaOapg.properties.storage_path_prefix:
+            self, name: typing_extensions.Literal["spot"]
+    ) -> MetaOapg.properties.spot:
         ...
 
     @typing.overload
     def __getitem__(
-        self, name: typing_extensions.Literal["provider_id"]
-    ) -> MetaOapg.properties.provider_id:
+        self, name: typing_extensions.Literal["region"]
+    ) -> MetaOapg.properties.region:
         ...
 
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
     def __getitem__(self, name: typing.Union[typing_extensions.Literal[
-        "method",
-        "params",
-        "resource_pool",
-        "client_version",
-        "scenario_name",
-        "storage_path_prefix",
+        "machine_type",
+        "num_cpus",
+        "ram_gb",
+        "price",
         "provider_id",
+        "spot",
+        "region",
     ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["method"]
-    ) -> MetaOapg.properties.method:
+        self, name: typing_extensions.Literal["machine_type"]
+    ) -> MetaOapg.properties.machine_type:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["params"]
-    ) -> MetaOapg.properties.params:
+        self, name: typing_extensions.Literal["num_cpus"]
+    ) -> MetaOapg.properties.num_cpus:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["resource_pool"]
-    ) -> typing.Union[MetaOapg.properties.resource_pool, schemas.Unset]:
+        self, name: typing_extensions.Literal["ram_gb"]
+    ) -> MetaOapg.properties.ram_gb:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["client_version"]
-    ) -> typing.Union[MetaOapg.properties.client_version, schemas.Unset]:
+            self, name: typing_extensions.Literal["price"]
+    ) -> MetaOapg.properties.price:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["scenario_name"]
-    ) -> typing.Union[MetaOapg.properties.scenario_name, schemas.Unset]:
+        self, name: typing_extensions.Literal["provider_id"]
+    ) -> typing.Union[MetaOapg.properties.provider_id, schemas.Unset]:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["storage_path_prefix"]
-    ) -> typing.Union[MetaOapg.properties.storage_path_prefix, schemas.Unset]:
+        self, name: typing_extensions.Literal["spot"]
+    ) -> typing.Union[MetaOapg.properties.spot, schemas.Unset]:
         ...
 
     @typing.overload
     def get_item_oapg(
-        self, name: typing_extensions.Literal["provider_id"]
-    ) -> typing.Union[MetaOapg.properties.provider_id, schemas.Unset]:
+        self, name: typing_extensions.Literal["region"]
+    ) -> typing.Union[MetaOapg.properties.region, schemas.Unset]:
         ...
 
     @typing.overload
     def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
     def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
-        "method",
-        "params",
-        "resource_pool",
-        "client_version",
-        "scenario_name",
-        "storage_path_prefix",
+        "machine_type",
+        "num_cpus",
+        "ram_gb",
+        "price",
         "provider_id",
+        "spot",
+        "region",
     ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *_args: typing.Union[
             dict,
             frozendict.frozendict,
         ],
-        method: typing.Union[
-            MetaOapg.properties.method,
+        machine_type: typing.Union[
+            MetaOapg.properties.machine_type,
             str,
         ],
-        params: typing.Union[
-            MetaOapg.properties.params,
-            dict,
-            frozendict.frozendict,
+        num_cpus: typing.Union[
+            MetaOapg.properties.num_cpus,
+            decimal.Decimal,
+            int,
+        ],
+        price: typing.Union[
+            MetaOapg.properties.price,
+            decimal.Decimal,
+            int,
+            float,
         ],
-        resource_pool: typing.Union[MetaOapg.properties.resource_pool, dict,
-                                    frozendict.frozendict, str, date, datetime,
-                                    uuid.UUID, int, float, decimal.Decimal,
-                                    bool, None, list, tuple, bytes, io.FileIO,
-                                    io.BufferedReader,
-                                    schemas.Unset] = schemas.unset,
-        client_version: typing.Union[MetaOapg.properties.client_version, dict,
-                                     frozendict.frozendict, str, date, datetime,
-                                     uuid.UUID, int, float, decimal.Decimal,
-                                     bool, None, list, tuple, bytes, io.FileIO,
-                                     io.BufferedReader,
-                                     schemas.Unset] = schemas.unset,
-        scenario_name: typing.Union[MetaOapg.properties.scenario_name, dict,
-                                    frozendict.frozendict, str, date, datetime,
-                                    uuid.UUID, int, float, decimal.Decimal,
-                                    bool, None, list, tuple, bytes, io.FileIO,
-                                    io.BufferedReader,
-                                    schemas.Unset] = schemas.unset,
-        storage_path_prefix: typing.Union[
-            MetaOapg.properties.storage_path_prefix, str,
-            schemas.Unset] = schemas.unset,
-        provider_id: typing.Union[MetaOapg.properties.provider_id, str,
+        ram_gb: typing.Union[
+            MetaOapg.properties.ram_gb,
+            decimal.Decimal,
+            int,
+        ],
+        provider_id: typing.Union[MetaOapg.properties.provider_id, dict,
+                                  frozendict.frozendict, str, date, datetime,
+                                  uuid.UUID, int, float, decimal.Decimal, bool,
+                                  None, list, tuple, bytes, io.FileIO,
+                                  io.BufferedReader,
                                   schemas.Unset] = schemas.unset,
+        spot: typing.Union[MetaOapg.properties.spot, dict,
+                           frozendict.frozendict, str, date, datetime,
+                           uuid.UUID, int, float, decimal.Decimal, bool, None,
+                           list, tuple, bytes, io.FileIO, io.BufferedReader,
+                           schemas.Unset] = schemas.unset,
+        region: typing.Union[MetaOapg.properties.region, dict,
+                             frozendict.frozendict, str, date, datetime,
+                             uuid.UUID, int, float, decimal.Decimal, bool, None,
+                             list, tuple, bytes, io.FileIO, io.BufferedReader,
+                             schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
-    ) -> 'TaskRequest':
+    ) -> 'MachineType':
         return super().__new__(
             cls,
             *_args,
-            method=method,
-            params=params,
-            resource_pool=resource_pool,
-            client_version=client_version,
-            scenario_name=scenario_name,
-            storage_path_prefix=storage_path_prefix,
+            machine_type=machine_type,
+            num_cpus=num_cpus,
+            price=price,
+            ram_gb=ram_gb,
             provider_id=provider_id,
+            spot=spot,
+            region=region,
             _configuration=_configuration,
             **kwargs,
         )
+
+
+from inductiva.client.model.providers import Providers
```

### Comparing `inductiva-0.5.3/inductiva/client/model/task_request.pyi` & `inductiva-0.6.0/inductiva/client/model/machine_type.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -19,82 +19,82 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class TaskRequest(
+class MachineType(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
         required = {
-            "method",
-            "params",
+            "machine_type",
+            "num_cpus",
+            "price",
+            "ram_gb",
         }
         
         class properties:
-            method = schemas.StrSchema
-            params = schemas.DictSchema
+            machine_type = schemas.StrSchema
+            num_cpus = schemas.IntSchema
+            ram_gb = schemas.IntSchema
+            price = schemas.NumberSchema
             
             
-            class resource_pool(
+            class provider_id(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    format = 'uuid4'
-                    any_of_0 = schemas.StrSchema
-                    any_of_1 = schemas.NoneSchema
                     
                     @classmethod
                     @functools.lru_cache()
-                    def any_of(cls):
+                    def all_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
                         # when we invoke this method. If we kept this at the class
                         # level we would get an error because the class level
                         # code would be run when this module is imported, and these composed
                         # classes don't exist yet because their module has not finished
                         # loading
                         return [
-                            cls.any_of_0,
-                            cls.any_of_1,
+                            Providers,
                         ]
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'resource_pool':
+                ) -> 'provider_id':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             
             
-            class client_version(
+            class spot(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
-                    any_of_0 = schemas.StrSchema
+                    any_of_0 = schemas.BoolSchema
                     any_of_1 = schemas.NoneSchema
                     
                     @classmethod
                     @functools.lru_cache()
                     def any_of(cls):
                         # we need this here to make our import statements work
                         # we must store _composed_schemas in here so the code is only run
@@ -110,24 +110,24 @@
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'client_version':
+                ) -> 'spot':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             
             
-            class scenario_name(
+            class region(
                 schemas.ComposedSchema,
             ):
             
             
                 class MetaOapg:
                     any_of_0 = schemas.StrSchema
                     any_of_1 = schemas.NoneSchema
@@ -149,125 +149,114 @@
             
             
                 def __new__(
                     cls,
                     *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
                     _configuration: typing.Optional[schemas.Configuration] = None,
                     **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-                ) -> 'scenario_name':
+                ) -> 'region':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
-            storage_path_prefix = schemas.StrSchema
-            
-            
-            class provider_id(
-                schemas.EnumBase,
-                schemas.StrSchema
-            ):
-                
-                @schemas.classproperty
-                def GCP(cls):
-                    return cls("GCP")
-                
-                @schemas.classproperty
-                def ICE(cls):
-                    return cls("ICE")
             __annotations__ = {
-                "method": method,
-                "params": params,
-                "resource_pool": resource_pool,
-                "client_version": client_version,
-                "scenario_name": scenario_name,
-                "storage_path_prefix": storage_path_prefix,
+                "machine_type": machine_type,
+                "num_cpus": num_cpus,
+                "ram_gb": ram_gb,
+                "price": price,
                 "provider_id": provider_id,
+                "spot": spot,
+                "region": region,
             }
     
-    method: MetaOapg.properties.method
-    params: MetaOapg.properties.params
+    machine_type: MetaOapg.properties.machine_type
+    num_cpus: MetaOapg.properties.num_cpus
+    price: MetaOapg.properties.price
+    ram_gb: MetaOapg.properties.ram_gb
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["method"]) -> MetaOapg.properties.method: ...
+    def __getitem__(self, name: typing_extensions.Literal["machine_type"]) -> MetaOapg.properties.machine_type: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["params"]) -> MetaOapg.properties.params: ...
+    def __getitem__(self, name: typing_extensions.Literal["num_cpus"]) -> MetaOapg.properties.num_cpus: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["resource_pool"]) -> MetaOapg.properties.resource_pool: ...
+    def __getitem__(self, name: typing_extensions.Literal["ram_gb"]) -> MetaOapg.properties.ram_gb: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["client_version"]) -> MetaOapg.properties.client_version: ...
+    def __getitem__(self, name: typing_extensions.Literal["price"]) -> MetaOapg.properties.price: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["scenario_name"]) -> MetaOapg.properties.scenario_name: ...
+    def __getitem__(self, name: typing_extensions.Literal["provider_id"]) -> MetaOapg.properties.provider_id: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["storage_path_prefix"]) -> MetaOapg.properties.storage_path_prefix: ...
+    def __getitem__(self, name: typing_extensions.Literal["spot"]) -> MetaOapg.properties.spot: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["provider_id"]) -> MetaOapg.properties.provider_id: ...
+    def __getitem__(self, name: typing_extensions.Literal["region"]) -> MetaOapg.properties.region: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["method", "params", "resource_pool", "client_version", "scenario_name", "storage_path_prefix", "provider_id", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["machine_type", "num_cpus", "ram_gb", "price", "provider_id", "spot", "region", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["method"]) -> MetaOapg.properties.method: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["machine_type"]) -> MetaOapg.properties.machine_type: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["params"]) -> MetaOapg.properties.params: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["num_cpus"]) -> MetaOapg.properties.num_cpus: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["resource_pool"]) -> typing.Union[MetaOapg.properties.resource_pool, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["ram_gb"]) -> MetaOapg.properties.ram_gb: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["client_version"]) -> typing.Union[MetaOapg.properties.client_version, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["price"]) -> MetaOapg.properties.price: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["scenario_name"]) -> typing.Union[MetaOapg.properties.scenario_name, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["provider_id"]) -> typing.Union[MetaOapg.properties.provider_id, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["storage_path_prefix"]) -> typing.Union[MetaOapg.properties.storage_path_prefix, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["spot"]) -> typing.Union[MetaOapg.properties.spot, schemas.Unset]: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["provider_id"]) -> typing.Union[MetaOapg.properties.provider_id, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["region"]) -> typing.Union[MetaOapg.properties.region, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["method", "params", "resource_pool", "client_version", "scenario_name", "storage_path_prefix", "provider_id", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["machine_type", "num_cpus", "ram_gb", "price", "provider_id", "spot", "region", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        method: typing.Union[MetaOapg.properties.method, str, ],
-        params: typing.Union[MetaOapg.properties.params, dict, frozendict.frozendict, ],
-        resource_pool: typing.Union[MetaOapg.properties.resource_pool, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        client_version: typing.Union[MetaOapg.properties.client_version, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        scenario_name: typing.Union[MetaOapg.properties.scenario_name, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        storage_path_prefix: typing.Union[MetaOapg.properties.storage_path_prefix, str, schemas.Unset] = schemas.unset,
-        provider_id: typing.Union[MetaOapg.properties.provider_id, str, schemas.Unset] = schemas.unset,
+        machine_type: typing.Union[MetaOapg.properties.machine_type, str, ],
+        num_cpus: typing.Union[MetaOapg.properties.num_cpus, decimal.Decimal, int, ],
+        price: typing.Union[MetaOapg.properties.price, decimal.Decimal, int, float, ],
+        ram_gb: typing.Union[MetaOapg.properties.ram_gb, decimal.Decimal, int, ],
+        provider_id: typing.Union[MetaOapg.properties.provider_id, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        spot: typing.Union[MetaOapg.properties.spot, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        region: typing.Union[MetaOapg.properties.region, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'TaskRequest':
+    ) -> 'MachineType':
         return super().__new__(
             cls,
             *_args,
-            method=method,
-            params=params,
-            resource_pool=resource_pool,
-            client_version=client_version,
-            scenario_name=scenario_name,
-            storage_path_prefix=storage_path_prefix,
+            machine_type=machine_type,
+            num_cpus=num_cpus,
+            price=price,
+            ram_gb=ram_gb,
             provider_id=provider_id,
+            spot=spot,
+            region=region,
             _configuration=_configuration,
             **kwargs,
         )
+
+from inductiva.client.model.providers import Providers
```

### Comparing `inductiva-0.5.3/inductiva/client/model/task_status.py` & `inductiva-0.6.0/inductiva/client/model/task_status.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/task_status.pyi` & `inductiva-0.6.0/inductiva/client/model/task_status.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/task_status_code.py` & `inductiva-0.6.0/inductiva/client/model/task_status_code.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/task_status_code.pyi` & `inductiva-0.6.0/inductiva/client/model/task_status_code.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/user.pyi` & `inductiva-0.6.0/inductiva/client/model/version_comparison_result.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -19,111 +19,89 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class User(
+class VersionComparisonResult(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
         required = {
-            "bucket_name",
-            "expiry_ts",
-            "email",
-            "username",
+            "is_valid",
+            "client_version",
+            "server_version",
         }
         
         class properties:
-            email = schemas.StrSchema
-            username = schemas.StrSchema
-            bucket_name = schemas.StrSchema
-            expiry_ts = schemas.DateTimeSchema
-            is_admin = schemas.BoolSchema
+            is_valid = schemas.BoolSchema
+            client_version = schemas.StrSchema
+            server_version = schemas.StrSchema
             __annotations__ = {
-                "email": email,
-                "username": username,
-                "bucket_name": bucket_name,
-                "expiry_ts": expiry_ts,
-                "is_admin": is_admin,
+                "is_valid": is_valid,
+                "client_version": client_version,
+                "server_version": server_version,
             }
     
-    bucket_name: MetaOapg.properties.bucket_name
-    expiry_ts: MetaOapg.properties.expiry_ts
-    email: MetaOapg.properties.email
-    username: MetaOapg.properties.username
+    is_valid: MetaOapg.properties.is_valid
+    client_version: MetaOapg.properties.client_version
+    server_version: MetaOapg.properties.server_version
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["email"]) -> MetaOapg.properties.email: ...
+    def __getitem__(self, name: typing_extensions.Literal["is_valid"]) -> MetaOapg.properties.is_valid: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["username"]) -> MetaOapg.properties.username: ...
+    def __getitem__(self, name: typing_extensions.Literal["client_version"]) -> MetaOapg.properties.client_version: ...
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["bucket_name"]) -> MetaOapg.properties.bucket_name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["expiry_ts"]) -> MetaOapg.properties.expiry_ts: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["is_admin"]) -> MetaOapg.properties.is_admin: ...
+    def __getitem__(self, name: typing_extensions.Literal["server_version"]) -> MetaOapg.properties.server_version: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["email", "username", "bucket_name", "expiry_ts", "is_admin", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["is_valid", "client_version", "server_version", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["email"]) -> MetaOapg.properties.email: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["username"]) -> MetaOapg.properties.username: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["bucket_name"]) -> MetaOapg.properties.bucket_name: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["is_valid"]) -> MetaOapg.properties.is_valid: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["expiry_ts"]) -> MetaOapg.properties.expiry_ts: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["client_version"]) -> MetaOapg.properties.client_version: ...
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["is_admin"]) -> typing.Union[MetaOapg.properties.is_admin, schemas.Unset]: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["server_version"]) -> MetaOapg.properties.server_version: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["email", "username", "bucket_name", "expiry_ts", "is_admin", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["is_valid", "client_version", "server_version", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        bucket_name: typing.Union[MetaOapg.properties.bucket_name, str, ],
-        expiry_ts: typing.Union[MetaOapg.properties.expiry_ts, str, datetime, ],
-        email: typing.Union[MetaOapg.properties.email, str, ],
-        username: typing.Union[MetaOapg.properties.username, str, ],
-        is_admin: typing.Union[MetaOapg.properties.is_admin, bool, schemas.Unset] = schemas.unset,
+        is_valid: typing.Union[MetaOapg.properties.is_valid, bool, ],
+        client_version: typing.Union[MetaOapg.properties.client_version, str, ],
+        server_version: typing.Union[MetaOapg.properties.server_version, str, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'User':
+    ) -> 'VersionComparisonResult':
         return super().__new__(
             cls,
             *_args,
-            bucket_name=bucket_name,
-            expiry_ts=expiry_ts,
-            email=email,
-            username=username,
-            is_admin=is_admin,
+            is_valid=is_valid,
+            client_version=client_version,
+            server_version=server_version,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/client/model/user_api_key.py` & `inductiva-0.6.0/inductiva/client/model/user_api_key.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # coding: utf-8
+
 """
     InductivaWebAPI
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     The version of the OpenAPI document: 0.1.0
     Generated by: https://openapi-generator.tech
@@ -18,84 +19,64 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class UserApiKey(schemas.DictSchema):
+class UserApiKey(
+    schemas.DictSchema
+):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
+
     class MetaOapg:
         required = {
             "api_key",
         }
-
+        
         class properties:
             api_key = schemas.StrSchema
             __annotations__ = {
                 "api_key": api_key,
             }
-
+    
     api_key: MetaOapg.properties.api_key
-
+    
     @typing.overload
-    def __getitem__(
-        self, name: typing_extensions.Literal["api_key"]
-    ) -> MetaOapg.properties.api_key:
-        ...
-
+    def __getitem__(self, name: typing_extensions.Literal["api_key"]) -> MetaOapg.properties.api_key: ...
+    
     @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
-        ...
-
-    def __getitem__(self,
-                    name: typing.Union[typing_extensions.Literal[
-                        "api_key",
-                    ], str]):
+    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
+    
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["api_key", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
-
+    
+    
     @typing.overload
-    def get_item_oapg(
-        self, name: typing_extensions.Literal["api_key"]
-    ) -> MetaOapg.properties.api_key:
-        ...
-
+    def get_item_oapg(self, name: typing_extensions.Literal["api_key"]) -> MetaOapg.properties.api_key: ...
+    
     @typing.overload
-    def get_item_oapg(
-            self, name: str
-    ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
-        ...
-
-    def get_item_oapg(self,
-                      name: typing.Union[typing_extensions.Literal[
-                          "api_key",
-                      ], str]):
+    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
+    
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["api_key", ], str]):
         return super().get_item_oapg(name)
+    
 
     def __new__(
         cls,
-        *_args: typing.Union[
-            dict,
-            frozendict.frozendict,
-        ],
-        api_key: typing.Union[
-            MetaOapg.properties.api_key,
-            str,
-        ],
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        api_key: typing.Union[MetaOapg.properties.api_key, str, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
-                               frozendict.frozendict, str, date, datetime,
-                               uuid.UUID, int, float, decimal.Decimal, None,
-                               list, tuple, bytes],
+        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'UserApiKey':
         return super().__new__(
             cls,
             *_args,
             api_key=api_key,
             _configuration=_configuration,
             **kwargs,
```

### Comparing `inductiva-0.5.3/inductiva/client/model/user_api_key.pyi` & `inductiva-0.6.0/inductiva/client/model/task_input_upload_url.pyi`

 * *Files 27% similar despite different names*

```diff
@@ -19,65 +19,77 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 
-class UserApiKey(
+class TaskInputUploadUrl(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
 
     class MetaOapg:
         required = {
-            "api_key",
+            "method",
+            "url",
         }
         
         class properties:
-            api_key = schemas.StrSchema
+            url = schemas.StrSchema
+            method = schemas.StrSchema
             __annotations__ = {
-                "api_key": api_key,
+                "url": url,
+                "method": method,
             }
     
-    api_key: MetaOapg.properties.api_key
+    method: MetaOapg.properties.method
+    url: MetaOapg.properties.url
     
     @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["api_key"]) -> MetaOapg.properties.api_key: ...
+    def __getitem__(self, name: typing_extensions.Literal["url"]) -> MetaOapg.properties.url: ...
+    
+    @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["method"]) -> MetaOapg.properties.method: ...
     
     @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["api_key", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["url", "method", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["api_key"]) -> MetaOapg.properties.api_key: ...
+    def get_item_oapg(self, name: typing_extensions.Literal["url"]) -> MetaOapg.properties.url: ...
+    
+    @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["method"]) -> MetaOapg.properties.method: ...
     
     @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["api_key", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["url", "method", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
-        api_key: typing.Union[MetaOapg.properties.api_key, str, ],
+        method: typing.Union[MetaOapg.properties.method, str, ],
+        url: typing.Union[MetaOapg.properties.url, str, ],
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'UserApiKey':
+    ) -> 'TaskInputUploadUrl':
         return super().__new__(
             cls,
             *_args,
-            api_key=api_key,
+            method=method,
+            url=url,
             _configuration=_configuration,
             **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/client/model/user_create.py` & `inductiva-0.6.0/inductiva/client/model/user_create.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/user_create.pyi` & `inductiva-0.6.0/inductiva/client/model/user_create.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/validation_error.py` & `inductiva-0.6.0/inductiva/client/model/validation_error.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/validation_error.pyi` & `inductiva-0.6.0/inductiva/client/model/validation_error.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/version_comparison_result.py` & `inductiva-0.6.0/inductiva/client/model/version_comparison_result.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/vm_group_config.py` & `inductiva-0.6.0/inductiva/client/model/vm_group_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -620,50 +620,123 @@
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
 
-            class type(schemas.EnumBase, schemas.StrSchema):
+            class type(
+                    schemas.ComposedSchema,):
 
                 class MetaOapg:
-                    enum_value_to_name = {
-                        "standard": "STANDARD",
-                        "mpi": "MPI",
-                        "elastic": "ELASTIC",
-                    }
-
-                @schemas.classproperty
-                def STANDARD(cls):
-                    return cls("standard")
-
-                @schemas.classproperty
-                def MPI(cls):
-                    return cls("mpi")
-
-                @schemas.classproperty
-                def ELASTIC(cls):
-                    return cls("elastic")
 
-            class provider_id(schemas.EnumBase, schemas.StrSchema):
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            MachineGroupType,
+                        ]
+
+                def __new__(
+                    cls,
+                    *_args: typing.Union[
+                        dict,
+                        frozendict.frozendict,
+                        str,
+                        date,
+                        datetime,
+                        uuid.UUID,
+                        int,
+                        float,
+                        decimal.Decimal,
+                        bool,
+                        None,
+                        list,
+                        tuple,
+                        bytes,
+                        io.FileIO,
+                        io.BufferedReader,
+                    ],
+                    _configuration: typing.Optional[
+                        schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
+                                           frozendict.frozendict, str, date,
+                                           datetime, uuid.UUID, int, float,
+                                           decimal.Decimal, None, list, tuple,
+                                           bytes],
+                ) -> 'type':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+
+            class provider_id(
+                    schemas.ComposedSchema,):
 
                 class MetaOapg:
-                    enum_value_to_name = {
-                        "GCP": "GCP",
-                        "ICE": "ICE",
-                    }
-
-                @schemas.classproperty
-                def GCP(cls):
-                    return cls("GCP")
-
-                @schemas.classproperty
-                def ICE(cls):
-                    return cls("ICE")
+
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            Providers,
+                        ]
+
+                def __new__(
+                    cls,
+                    *_args: typing.Union[
+                        dict,
+                        frozendict.frozendict,
+                        str,
+                        date,
+                        datetime,
+                        uuid.UUID,
+                        int,
+                        float,
+                        decimal.Decimal,
+                        bool,
+                        None,
+                        list,
+                        tuple,
+                        bytes,
+                        io.FileIO,
+                        io.BufferedReader,
+                    ],
+                    _configuration: typing.Optional[
+                        schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
+                                           frozendict.frozendict, str, date,
+                                           datetime, uuid.UUID, int, float,
+                                           decimal.Decimal, None, list, tuple,
+                                           bytes],
+                ) -> 'provider_id':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+
+            started = schemas.BoolSchema
 
             class min_vms(
                     schemas.ComposedSchema,):
 
                 class MetaOapg:
                     any_of_0 = schemas.IntSchema
                     any_of_1 = schemas.NoneSchema
@@ -771,14 +844,68 @@
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
 
+            class autoscale_policy(
+                    schemas.ComposedSchema,):
+
+                class MetaOapg:
+
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            AutoscalePolicy,
+                        ]
+
+                def __new__(
+                    cls,
+                    *_args: typing.Union[
+                        dict,
+                        frozendict.frozendict,
+                        str,
+                        date,
+                        datetime,
+                        uuid.UUID,
+                        int,
+                        float,
+                        decimal.Decimal,
+                        bool,
+                        None,
+                        list,
+                        tuple,
+                        bytes,
+                        io.FileIO,
+                        io.BufferedReader,
+                    ],
+                    _configuration: typing.Optional[
+                        schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
+                                           frozendict.frozendict, str, date,
+                                           datetime, uuid.UUID, int, float,
+                                           decimal.Decimal, None, list, tuple,
+                                           bytes],
+                ) -> 'autoscale_policy':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+
             __annotations__ = {
                 "spot": spot,
                 "is_elastic": is_elastic,
                 "max_idle_time": max_idle_time,
                 "auto_terminate_ts": auto_terminate_ts,
                 "id": id,
                 "name": name,
@@ -786,16 +913,18 @@
                 "disk_size_gb": disk_size_gb,
                 "num_vms": num_vms,
                 "idle_seconds": idle_seconds,
                 "creation_timestamp": creation_timestamp,
                 "deletion_timestamp": deletion_timestamp,
                 "type": type,
                 "provider_id": provider_id,
+                "started": started,
                 "min_vms": min_vms,
                 "max_vms": max_vms,
+                "autoscale_policy": autoscale_policy,
             }
 
     spot: MetaOapg.properties.spot
     is_elastic: MetaOapg.properties.is_elastic
 
     @typing.overload
     def __getitem__(
@@ -879,25 +1008,37 @@
     def __getitem__(
         self, name: typing_extensions.Literal["provider_id"]
     ) -> MetaOapg.properties.provider_id:
         ...
 
     @typing.overload
     def __getitem__(
+        self, name: typing_extensions.Literal["started"]
+    ) -> MetaOapg.properties.started:
+        ...
+
+    @typing.overload
+    def __getitem__(
         self, name: typing_extensions.Literal["min_vms"]
     ) -> MetaOapg.properties.min_vms:
         ...
 
     @typing.overload
     def __getitem__(
         self, name: typing_extensions.Literal["max_vms"]
     ) -> MetaOapg.properties.max_vms:
         ...
 
     @typing.overload
+    def __getitem__(
+        self, name: typing_extensions.Literal["autoscale_policy"]
+    ) -> MetaOapg.properties.autoscale_policy:
+        ...
+
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema:
         ...
 
     def __getitem__(self, name: typing.Union[typing_extensions.Literal[
         "spot",
         "is_elastic",
         "max_idle_time",
@@ -908,16 +1049,18 @@
         "disk_size_gb",
         "num_vms",
         "idle_seconds",
         "creation_timestamp",
         "deletion_timestamp",
         "type",
         "provider_id",
+        "started",
         "min_vms",
         "max_vms",
+        "autoscale_policy",
     ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
 
     @typing.overload
     def get_item_oapg(
             self, name: typing_extensions.Literal["spot"]
@@ -1000,26 +1143,38 @@
     def get_item_oapg(
         self, name: typing_extensions.Literal["provider_id"]
     ) -> typing.Union[MetaOapg.properties.provider_id, schemas.Unset]:
         ...
 
     @typing.overload
     def get_item_oapg(
+        self, name: typing_extensions.Literal["started"]
+    ) -> typing.Union[MetaOapg.properties.started, schemas.Unset]:
+        ...
+
+    @typing.overload
+    def get_item_oapg(
         self, name: typing_extensions.Literal["min_vms"]
     ) -> typing.Union[MetaOapg.properties.min_vms, schemas.Unset]:
         ...
 
     @typing.overload
     def get_item_oapg(
         self, name: typing_extensions.Literal["max_vms"]
     ) -> typing.Union[MetaOapg.properties.max_vms, schemas.Unset]:
         ...
 
     @typing.overload
     def get_item_oapg(
+        self, name: typing_extensions.Literal["autoscale_policy"]
+    ) -> typing.Union[MetaOapg.properties.autoscale_policy, schemas.Unset]:
+        ...
+
+    @typing.overload
+    def get_item_oapg(
             self, name: str
     ) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]:
         ...
 
     def get_item_oapg(self, name: typing.Union[typing_extensions.Literal[
         "spot",
         "is_elastic",
@@ -1031,16 +1186,18 @@
         "disk_size_gb",
         "num_vms",
         "idle_seconds",
         "creation_timestamp",
         "deletion_timestamp",
         "type",
         "provider_id",
+        "started",
         "min_vms",
         "max_vms",
+        "autoscale_policy",
     ], str]):
         return super().get_item_oapg(name)
 
     def __new__(
         cls,
         *_args: typing.Union[
             dict,
@@ -1110,28 +1267,43 @@
         deletion_timestamp: typing.Union[MetaOapg.properties.deletion_timestamp,
                                          dict, frozendict.frozendict, str, date,
                                          datetime, uuid.UUID, int, float,
                                          decimal.Decimal, bool, None, list,
                                          tuple, bytes, io.FileIO,
                                          io.BufferedReader,
                                          schemas.Unset] = schemas.unset,
-        type: typing.Union[MetaOapg.properties.type, str,
+        type: typing.Union[MetaOapg.properties.type, dict,
+                           frozendict.frozendict, str, date, datetime,
+                           uuid.UUID, int, float, decimal.Decimal, bool, None,
+                           list, tuple, bytes, io.FileIO, io.BufferedReader,
                            schemas.Unset] = schemas.unset,
-        provider_id: typing.Union[MetaOapg.properties.provider_id, str,
+        provider_id: typing.Union[MetaOapg.properties.provider_id, dict,
+                                  frozendict.frozendict, str, date, datetime,
+                                  uuid.UUID, int, float, decimal.Decimal, bool,
+                                  None, list, tuple, bytes, io.FileIO,
+                                  io.BufferedReader,
                                   schemas.Unset] = schemas.unset,
+        started: typing.Union[MetaOapg.properties.started, bool,
+                              schemas.Unset] = schemas.unset,
         min_vms: typing.Union[MetaOapg.properties.min_vms, dict,
                               frozendict.frozendict, str, date, datetime,
                               uuid.UUID, int, float, decimal.Decimal, bool,
                               None, list, tuple, bytes, io.FileIO,
                               io.BufferedReader, schemas.Unset] = schemas.unset,
         max_vms: typing.Union[MetaOapg.properties.max_vms, dict,
                               frozendict.frozendict, str, date, datetime,
                               uuid.UUID, int, float, decimal.Decimal, bool,
                               None, list, tuple, bytes, io.FileIO,
                               io.BufferedReader, schemas.Unset] = schemas.unset,
+        autoscale_policy: typing.Union[MetaOapg.properties.autoscale_policy,
+                                       dict, frozendict.frozendict, str, date,
+                                       datetime, uuid.UUID, int, float,
+                                       decimal.Decimal, bool, None, list, tuple,
+                                       bytes, io.FileIO, io.BufferedReader,
+                                       schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict,
                                frozendict.frozendict, str, date, datetime,
                                uuid.UUID, int, float, decimal.Decimal, None,
                                list, tuple, bytes],
     ) -> 'VMGroupConfig':
         return super().__new__(
@@ -1147,12 +1319,19 @@
             disk_size_gb=disk_size_gb,
             num_vms=num_vms,
             idle_seconds=idle_seconds,
             creation_timestamp=creation_timestamp,
             deletion_timestamp=deletion_timestamp,
             type=type,
             provider_id=provider_id,
+            started=started,
             min_vms=min_vms,
             max_vms=max_vms,
+            autoscale_policy=autoscale_policy,
             _configuration=_configuration,
             **kwargs,
         )
+
+
+from inductiva.client.model.autoscale_policy import AutoscalePolicy
+from inductiva.client.model.machine_group_type import MachineGroupType
+from inductiva.client.model.providers import Providers
```

### Comparing `inductiva-0.5.3/inductiva/client/model/vm_group_config.pyi` & `inductiva-0.6.0/inductiva/client/model/vm_group_config.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -442,43 +442,84 @@
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
             
             
             class type(
-                schemas.EnumBase,
-                schemas.StrSchema
+                schemas.ComposedSchema,
             ):
-                
-                @schemas.classproperty
-                def STANDARD(cls):
-                    return cls("standard")
-                
-                @schemas.classproperty
-                def MPI(cls):
-                    return cls("mpi")
-                
-                @schemas.classproperty
-                def ELASTIC(cls):
-                    return cls("elastic")
+            
+            
+                class MetaOapg:
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            MachineGroupType,
+                        ]
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'type':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
             
             
             class provider_id(
-                schemas.EnumBase,
-                schemas.StrSchema
+                schemas.ComposedSchema,
             ):
-                
-                @schemas.classproperty
-                def GCP(cls):
-                    return cls("GCP")
-                
-                @schemas.classproperty
-                def ICE(cls):
-                    return cls("ICE")
+            
+            
+                class MetaOapg:
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            Providers,
+                        ]
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'provider_id':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
+            started = schemas.BoolSchema
             
             
             class min_vms(
                 schemas.ComposedSchema,
             ):
             
             
@@ -549,14 +590,50 @@
                 ) -> 'max_vms':
                     return super().__new__(
                         cls,
                         *_args,
                         _configuration=_configuration,
                         **kwargs,
                     )
+            
+            
+            class autoscale_policy(
+                schemas.ComposedSchema,
+            ):
+            
+            
+                class MetaOapg:
+                    
+                    @classmethod
+                    @functools.lru_cache()
+                    def all_of(cls):
+                        # we need this here to make our import statements work
+                        # we must store _composed_schemas in here so the code is only run
+                        # when we invoke this method. If we kept this at the class
+                        # level we would get an error because the class level
+                        # code would be run when this module is imported, and these composed
+                        # classes don't exist yet because their module has not finished
+                        # loading
+                        return [
+                            AutoscalePolicy,
+                        ]
+            
+            
+                def __new__(
+                    cls,
+                    *_args: typing.Union[dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, ],
+                    _configuration: typing.Optional[schemas.Configuration] = None,
+                    **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
+                ) -> 'autoscale_policy':
+                    return super().__new__(
+                        cls,
+                        *_args,
+                        _configuration=_configuration,
+                        **kwargs,
+                    )
             __annotations__ = {
                 "spot": spot,
                 "is_elastic": is_elastic,
                 "max_idle_time": max_idle_time,
                 "auto_terminate_ts": auto_terminate_ts,
                 "id": id,
                 "name": name,
@@ -564,16 +641,18 @@
                 "disk_size_gb": disk_size_gb,
                 "num_vms": num_vms,
                 "idle_seconds": idle_seconds,
                 "creation_timestamp": creation_timestamp,
                 "deletion_timestamp": deletion_timestamp,
                 "type": type,
                 "provider_id": provider_id,
+                "started": started,
                 "min_vms": min_vms,
                 "max_vms": max_vms,
+                "autoscale_policy": autoscale_policy,
             }
     
     spot: MetaOapg.properties.spot
     is_elastic: MetaOapg.properties.is_elastic
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["spot"]) -> MetaOapg.properties.spot: ...
@@ -614,23 +693,29 @@
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["type"]) -> MetaOapg.properties.type: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["provider_id"]) -> MetaOapg.properties.provider_id: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["started"]) -> MetaOapg.properties.started: ...
+    
+    @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["min_vms"]) -> MetaOapg.properties.min_vms: ...
     
     @typing.overload
     def __getitem__(self, name: typing_extensions.Literal["max_vms"]) -> MetaOapg.properties.max_vms: ...
     
     @typing.overload
+    def __getitem__(self, name: typing_extensions.Literal["autoscale_policy"]) -> MetaOapg.properties.autoscale_policy: ...
+    
+    @typing.overload
     def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
     
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["spot", "is_elastic", "max_idle_time", "auto_terminate_ts", "id", "name", "machine_type", "disk_size_gb", "num_vms", "idle_seconds", "creation_timestamp", "deletion_timestamp", "type", "provider_id", "min_vms", "max_vms", ], str]):
+    def __getitem__(self, name: typing.Union[typing_extensions.Literal["spot", "is_elastic", "max_idle_time", "auto_terminate_ts", "id", "name", "machine_type", "disk_size_gb", "num_vms", "idle_seconds", "creation_timestamp", "deletion_timestamp", "type", "provider_id", "started", "min_vms", "max_vms", "autoscale_policy", ], str]):
         # dict_instance[name] accessor
         return super().__getitem__(name)
     
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["spot"]) -> MetaOapg.properties.spot: ...
     
@@ -670,23 +755,29 @@
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["type"]) -> typing.Union[MetaOapg.properties.type, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["provider_id"]) -> typing.Union[MetaOapg.properties.provider_id, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["started"]) -> typing.Union[MetaOapg.properties.started, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["min_vms"]) -> typing.Union[MetaOapg.properties.min_vms, schemas.Unset]: ...
     
     @typing.overload
     def get_item_oapg(self, name: typing_extensions.Literal["max_vms"]) -> typing.Union[MetaOapg.properties.max_vms, schemas.Unset]: ...
     
     @typing.overload
+    def get_item_oapg(self, name: typing_extensions.Literal["autoscale_policy"]) -> typing.Union[MetaOapg.properties.autoscale_policy, schemas.Unset]: ...
+    
+    @typing.overload
     def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
     
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["spot", "is_elastic", "max_idle_time", "auto_terminate_ts", "id", "name", "machine_type", "disk_size_gb", "num_vms", "idle_seconds", "creation_timestamp", "deletion_timestamp", "type", "provider_id", "min_vms", "max_vms", ], str]):
+    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["spot", "is_elastic", "max_idle_time", "auto_terminate_ts", "id", "name", "machine_type", "disk_size_gb", "num_vms", "idle_seconds", "creation_timestamp", "deletion_timestamp", "type", "provider_id", "started", "min_vms", "max_vms", "autoscale_policy", ], str]):
         return super().get_item_oapg(name)
     
 
     def __new__(
         cls,
         *_args: typing.Union[dict, frozendict.frozendict, ],
         spot: typing.Union[MetaOapg.properties.spot, bool, ],
@@ -697,18 +788,20 @@
         name: typing.Union[MetaOapg.properties.name, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         machine_type: typing.Union[MetaOapg.properties.machine_type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         disk_size_gb: typing.Union[MetaOapg.properties.disk_size_gb, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         num_vms: typing.Union[MetaOapg.properties.num_vms, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         idle_seconds: typing.Union[MetaOapg.properties.idle_seconds, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         creation_timestamp: typing.Union[MetaOapg.properties.creation_timestamp, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         deletion_timestamp: typing.Union[MetaOapg.properties.deletion_timestamp, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
-        type: typing.Union[MetaOapg.properties.type, str, schemas.Unset] = schemas.unset,
-        provider_id: typing.Union[MetaOapg.properties.provider_id, str, schemas.Unset] = schemas.unset,
+        type: typing.Union[MetaOapg.properties.type, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        provider_id: typing.Union[MetaOapg.properties.provider_id, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        started: typing.Union[MetaOapg.properties.started, bool, schemas.Unset] = schemas.unset,
         min_vms: typing.Union[MetaOapg.properties.min_vms, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         max_vms: typing.Union[MetaOapg.properties.max_vms, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
+        autoscale_policy: typing.Union[MetaOapg.properties.autoscale_policy, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, bool, None, list, tuple, bytes, io.FileIO, io.BufferedReader, schemas.Unset] = schemas.unset,
         _configuration: typing.Optional[schemas.Configuration] = None,
         **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
     ) -> 'VMGroupConfig':
         return super().__new__(
             cls,
             *_args,
             spot=spot,
@@ -721,12 +814,18 @@
             disk_size_gb=disk_size_gb,
             num_vms=num_vms,
             idle_seconds=idle_seconds,
             creation_timestamp=creation_timestamp,
             deletion_timestamp=deletion_timestamp,
             type=type,
             provider_id=provider_id,
+            started=started,
             min_vms=min_vms,
             max_vms=max_vms,
+            autoscale_policy=autoscale_policy,
             _configuration=_configuration,
             **kwargs,
         )
+
+from inductiva.client.model.autoscale_policy import AutoscalePolicy
+from inductiva.client.model.machine_group_type import MachineGroupType
+from inductiva.client.model.providers import Providers
```

### Comparing `inductiva-0.5.3/inductiva/client/model/vm_group_lifecycle_config.py` & `inductiva-0.6.0/inductiva/client/model/vm_group_lifecycle_config.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/model/vm_group_lifecycle_config.pyi` & `inductiva-0.6.0/inductiva/client/model/vm_group_lifecycle_config.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/models/__init__.py` & `inductiva-0.6.0/inductiva/client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,34 @@
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
 # from inductiva.client.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
+from inductiva.client.model.autoscale_policy import AutoscalePolicy
 from inductiva.client.model.backend_version import BackendVersion
-from inductiva.client.model.base_machine_type import BaseMachineType
 from inductiva.client.model.base_vm_group import BaseVMGroup
-from inductiva.client.model.body_upload_task_input import BodyUploadTaskInput
 from inductiva.client.model.default_machine_group import DefaultMachineGroup
 from inductiva.client.model.executer import Executer
 from inductiva.client.model.executer_tracker_api_connection_info import ExecuterTrackerAPIConnectionInfo
 from inductiva.client.model.executer_tracker_register_info import ExecuterTrackerRegisterInfo
 from inductiva.client.model.file_info import FileInfo
 from inductiva.client.model.http_validation_error import HTTPValidationError
+from inductiva.client.model.machine_group_type import MachineGroupType
 from inductiva.client.model.machine_type import MachineType
 from inductiva.client.model.output_archive_info import OutputArchiveInfo
+from inductiva.client.model.project import Project
+from inductiva.client.model.project_create import ProjectCreate
 from inductiva.client.model.provider import Provider
 from inductiva.client.model.providers import Providers
 from inductiva.client.model.quota import Quota
+from inductiva.client.model.storage_file_info import StorageFileInfo
 from inductiva.client.model.task import Task
+from inductiva.client.model.task_input_upload_url import TaskInputUploadUrl
 from inductiva.client.model.task_request import TaskRequest
 from inductiva.client.model.task_status import TaskStatus
 from inductiva.client.model.task_status_code import TaskStatusCode
 from inductiva.client.model.user import User
 from inductiva.client.model.user_api_key import UserApiKey
 from inductiva.client.model.user_create import UserCreate
 from inductiva.client.model.vm_group_config import VMGroupConfig
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/__init__.py` & `inductiva-0.6.0/inductiva/client/paths/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 
 import enum
 
 
 class PathValues(str, enum.Enum):
     TASKS_AUTH = "/tasks/auth"
     TASKS_SUBMIT = "/tasks/submit"
+    TASKS_TASK_ID_INPUT_UPLOAD_URL = "/tasks/{task_id}/input_upload_url"
+    TASKS_TASK_ID_INPUT_UPLOADED = "/tasks/{task_id}/input_uploaded"
     TASKS_TASK_ID_INPUT = "/tasks/{task_id}/input"
     TASKS_TASK_ID = "/tasks/{task_id}"
     TASKS = "/tasks"
     TASKS_TASK_ID_STATUS = "/tasks/{task_id}/status"
     TASKS_TASK_ID_OUTPUT_LIST = "/tasks/{task_id}/output/list"
     TASKS_TASK_ID_OUTPUT = "/tasks/{task_id}/output"
     TASKS_TASK_ID_KILL = "/tasks/{task_id}/kill"
+    TASKS_TASK_ID_DISABLE_LOGS = "/tasks/{task_id}/disable_logs"
     ADMIN_USERS = "/admin/users"
     ADMIN_USERS_EMAIL_API_KEY = "/admin/users/{email}/api_key"
     ADMIN_USERS_EMAIL = "/admin/users/{email}"
     ADMIN_USERS_EMAIL_EXPIRY_TS = "/admin/users/{email}/expiry_ts"
     ADMIN_USERS_USERNAME_TASKS = "/admin/users/{username}/tasks"
     ADMIN_GROUPS = "/admin/groups"
     ADMIN_GROUPS_ACTIVE = "/admin/groups/active"
@@ -39,7 +42,9 @@
     COMPUTE_GROUP_MACHINE = "/compute/group/machine"
     COMPUTE_GROUP_NAME = "/compute/group/{name}"
     STORAGE_SIZE = "/storage/size"
     STORAGE_CONTENTS = "/storage/contents"
     VERSION = "/version"
     VERSIONCHECK = "/version-check"
     USERS_QUOTAS = "/users/quotas"
+    PROJECTS = "/projects"
+    PROJECTS_NAME = "/projects/{name}"
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group/delete.py` & `inductiva-0.6.0/inductiva/client/paths/compute_group/delete.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group/delete.pyi` & `inductiva-0.6.0/inductiva/client/paths/compute_group/delete.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group/post.py` & `inductiva-0.6.0/inductiva/client/paths/compute_group/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group/post.pyi` & `inductiva-0.6.0/inductiva/client/paths/compute_group/post.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group_machine/delete.py` & `inductiva-0.6.0/inductiva/client/paths/compute_group_machine/delete.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group_machine/delete.pyi` & `inductiva-0.6.0/inductiva/client/paths/compute_group_machine/delete.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group_mg_id/patch.py` & `inductiva-0.6.0/inductiva/client/paths/compute_group_mg_id/patch.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group_mg_id/patch.pyi` & `inductiva-0.6.0/inductiva/client/paths/compute_group_mg_id/patch.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group_name/get.py` & `inductiva-0.6.0/inductiva/client/paths/compute_group_name/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group_name/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/compute_group_name/get.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group_start/post.py` & `inductiva-0.6.0/inductiva/client/paths/compute_group_start/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group_start/post.pyi` & `inductiva-0.6.0/inductiva/client/paths/compute_group_start/post.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group_status/get.py` & `inductiva-0.6.0/inductiva/client/paths/compute_group_status/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_group_status/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/compute_group_status/get.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_groups/get.py` & `inductiva-0.6.0/inductiva/client/paths/compute_groups/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_groups/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/compute_groups/get.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_machine_types/get.py` & `inductiva-0.6.0/inductiva/client/paths/compute_machine_types/get.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # coding: utf-8
+
 """
 
 
     Generated by: https://openapi-generator.tech
 """
 
 from dataclasses import dataclass
@@ -24,68 +25,80 @@
 
 from inductiva.client import schemas  # noqa: F401
 
 from inductiva.client.model.providers import Providers
 from inductiva.client.model.http_validation_error import HTTPValidationError
 from inductiva.client.model.machine_type import MachineType
 
-from . import path
-
 # Query params
 MachineFamilySchema = schemas.StrSchema
+SpotSchema = schemas.BoolSchema
+RegionSchema = schemas.StrSchema
 ProviderIdSchema = Providers
 RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams', {})
+    'RequestRequiredQueryParams',
+    {
+    }
+)
 RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams', {
-        'machine_family': typing.Union[
-            MachineFamilySchema,
-            str,
-        ],
-        'provider_id': typing.Union[
-            ProviderIdSchema,
-        ],
+    'RequestOptionalQueryParams',
+    {
+        'machine_family': typing.Union[MachineFamilySchema, str, ],
+        'spot': typing.Union[SpotSchema, bool, ],
+        'region': typing.Union[RegionSchema, str, ],
+        'provider_id': typing.Union[ProviderIdSchema, ],
     },
-    total=False)
+    total=False
+)
 
 
-class RequestQueryParams(RequestRequiredQueryParams,
-                         RequestOptionalQueryParams):
+class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
 request_query_machine_family = api_client.QueryParameter(
     name="machine_family",
     style=api_client.ParameterStyle.FORM,
     schema=MachineFamilySchema,
     explode=True,
 )
+request_query_spot = api_client.QueryParameter(
+    name="spot",
+    style=api_client.ParameterStyle.FORM,
+    schema=SpotSchema,
+    explode=True,
+)
+request_query_region = api_client.QueryParameter(
+    name="region",
+    style=api_client.ParameterStyle.FORM,
+    schema=RegionSchema,
+    explode=True,
+)
 request_query_provider_id = api_client.QueryParameter(
     name="provider_id",
     style=api_client.ParameterStyle.FORM,
     schema=ProviderIdSchema,
     explode=True,
 )
-_auth = [
-    'APIKeyHeader',
-]
 
 
-class SchemaFor200ResponseBodyApplicationJson(schemas.ListSchema):
+class SchemaFor200ResponseBodyApplicationJson(
+    schemas.ListSchema
+):
 
-    class MetaOapg:
 
+    class MetaOapg:
+        
         @staticmethod
         def items() -> typing.Type['MachineType']:
             return MachineType
 
     def __new__(
         cls,
-        _arg: typing.Union[typing.Tuple['MachineType'],
-                           typing.List['MachineType']],
+        _arg: typing.Union[typing.Tuple['MachineType'], typing.List['MachineType']],
         _configuration: typing.Optional[schemas.Configuration] = None,
     ) -> 'SchemaFor200ResponseBodyApplicationJson':
         return super().__new__(
             cls,
             _arg,
             _configuration=_configuration,
         )
@@ -102,17 +115,16 @@
     ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
-        'application/json':
-            api_client.MediaType(schema=SchemaFor200ResponseBodyApplicationJson
-                                ),
+        'application/json': api_client.MediaType(
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationError
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
@@ -122,65 +134,58 @@
     ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_422 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor422,
     content={
-        'application/json':
-            api_client.MediaType(schema=SchemaFor422ResponseBodyApplicationJson
-                                ),
+        'application/json': api_client.MediaType(
+            schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
-_all_accept_content_types = ('application/json',)
+_all_accept_content_types = (
+    'application/json',
+)
 
 
 class BaseApi(api_client.Api):
-
     @typing.overload
     def _list_available_machine_types_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-    ]:
-        ...
+        ApiResponseFor200,
+    ]: ...
 
     @typing.overload
     def _list_available_machine_types_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization:
-        ...
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def _list_available_machine_types_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-            api_client.ApiResponseWithoutDeserialization,
-    ]:
-        ...
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
 
     def _list_available_machine_types_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
@@ -193,25 +198,25 @@
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
 
         prefix_separator_iterator = None
         for parameter in (
-                request_query_machine_family,
-                request_query_provider_id,
+            request_query_machine_family,
+            request_query_spot,
+            request_query_region,
+            request_query_provider_id,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator(
-                )
-            serialized_data = parameter.serialize(parameter_data,
-                                                  prefix_separator_iterator)
+                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
+            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
             for serialized_value in serialized_data.values():
                 used_path += serialized_value
 
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
@@ -223,30 +228,28 @@
             headers=_headers,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
-            api_response = api_client.ApiResponseWithoutDeserialization(
-                response=response)
+            api_response = api_client.ApiResponseWithoutDeserialization(response=response)
         else:
-            response_for_status = _status_code_to_response.get(
-                str(response.status))
+            response_for_status = _status_code_to_response.get(str(response.status))
             if response_for_status:
-                api_response = response_for_status.deserialize(
-                    response, self.api_client.configuration)
+                api_response = response_for_status.deserialize(response, self.api_client.configuration)
             else:
-                api_response = api_client.ApiResponseWithoutDeserialization(
-                    response=response)
+                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
 
         if not 200 <= response.status <= 299:
-            raise exceptions.ApiException(status=response.status,
-                                          reason=response.reason,
-                                          api_response=api_response)
+            raise exceptions.ApiException(
+                status=response.status,
+                reason=response.reason,
+                api_response=api_response
+            )
 
         return api_response
 
 
 class ListAvailableMachineTypes(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
@@ -255,107 +258,105 @@
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-    ]:
-        ...
+        ApiResponseFor200,
+    ]: ...
 
     @typing.overload
     def list_available_machine_types(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization:
-        ...
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def list_available_machine_types(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-            api_client.ApiResponseWithoutDeserialization,
-    ]:
-        ...
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
 
     def list_available_machine_types(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._list_available_machine_types_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization)
+            skip_deserialization=skip_deserialization
+        )
 
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-    ]:
-        ...
+        ApiResponseFor200,
+    ]: ...
 
     @typing.overload
     def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization:
-        ...
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-            api_client.ApiResponseWithoutDeserialization,
-    ]:
-        ...
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
 
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._list_available_machine_types_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization)
+            skip_deserialization=skip_deserialization
+        )
+
+
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_machine_types/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/compute_machine_types/get.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # coding: utf-8
-
 """
 
 
     Generated by: https://openapi-generator.tech
 """
 
 from dataclasses import dataclass
@@ -25,64 +24,90 @@
 
 from inductiva.client import schemas  # noqa: F401
 
 from inductiva.client.model.providers import Providers
 from inductiva.client.model.http_validation_error import HTTPValidationError
 from inductiva.client.model.machine_type import MachineType
 
+from . import path
+
 # Query params
 MachineFamilySchema = schemas.StrSchema
+SpotSchema = schemas.BoolSchema
+RegionSchema = schemas.StrSchema
 ProviderIdSchema = Providers
 RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams',
-    {
-    }
-)
+    'RequestRequiredQueryParams', {})
 RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams',
-    {
-        'machine_family': typing.Union[MachineFamilySchema, str, ],
-        'provider_id': typing.Union[ProviderIdSchema, ],
+    'RequestOptionalQueryParams', {
+        'machine_family': typing.Union[
+            MachineFamilySchema,
+            str,
+        ],
+        'spot': typing.Union[
+            SpotSchema,
+            bool,
+        ],
+        'region': typing.Union[
+            RegionSchema,
+            str,
+        ],
+        'provider_id': typing.Union[
+            ProviderIdSchema,
+        ],
     },
-    total=False
-)
+    total=False)
 
 
-class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
+class RequestQueryParams(RequestRequiredQueryParams,
+                         RequestOptionalQueryParams):
     pass
 
 
 request_query_machine_family = api_client.QueryParameter(
     name="machine_family",
     style=api_client.ParameterStyle.FORM,
     schema=MachineFamilySchema,
     explode=True,
 )
+request_query_spot = api_client.QueryParameter(
+    name="spot",
+    style=api_client.ParameterStyle.FORM,
+    schema=SpotSchema,
+    explode=True,
+)
+request_query_region = api_client.QueryParameter(
+    name="region",
+    style=api_client.ParameterStyle.FORM,
+    schema=RegionSchema,
+    explode=True,
+)
 request_query_provider_id = api_client.QueryParameter(
     name="provider_id",
     style=api_client.ParameterStyle.FORM,
     schema=ProviderIdSchema,
     explode=True,
 )
+_auth = [
+    'APIKeyHeader',
+]
 
 
-class SchemaFor200ResponseBodyApplicationJson(
-    schemas.ListSchema
-):
-
+class SchemaFor200ResponseBodyApplicationJson(schemas.ListSchema):
 
     class MetaOapg:
-        
+
         @staticmethod
         def items() -> typing.Type['MachineType']:
             return MachineType
 
     def __new__(
         cls,
-        _arg: typing.Union[typing.Tuple['MachineType'], typing.List['MachineType']],
+        _arg: typing.Union[typing.Tuple['MachineType'],
+                           typing.List['MachineType']],
         _configuration: typing.Optional[schemas.Configuration] = None,
     ) -> 'SchemaFor200ResponseBodyApplicationJson':
         return super().__new__(
             cls,
             _arg,
             _configuration=_configuration,
         )
@@ -99,16 +124,17 @@
     ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+        'application/json':
+            api_client.MediaType(schema=SchemaFor200ResponseBodyApplicationJson
+                                ),
     },
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationError
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
@@ -118,58 +144,65 @@
     ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_422 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor422,
     content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor422ResponseBodyApplicationJson),
+        'application/json':
+            api_client.MediaType(schema=SchemaFor422ResponseBodyApplicationJson
+                                ),
     },
 )
-_all_accept_content_types = (
-    'application/json',
-)
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
+_all_accept_content_types = ('application/json',)
 
 
 class BaseApi(api_client.Api):
+
     @typing.overload
     def _list_available_machine_types_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+            ApiResponseFor200,
+    ]:
+        ...
 
     @typing.overload
     def _list_available_machine_types_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    ) -> api_client.ApiResponseWithoutDeserialization:
+        ...
 
     @typing.overload
     def _list_available_machine_types_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-        api_client.ApiResponseWithoutDeserialization,
-    ]: ...
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
+        ...
 
     def _list_available_machine_types_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
@@ -182,23 +215,27 @@
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
 
         prefix_separator_iterator = None
         for parameter in (
-            request_query_machine_family,
-            request_query_provider_id,
+                request_query_machine_family,
+                request_query_spot,
+                request_query_region,
+                request_query_provider_id,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
-            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
+                prefix_separator_iterator = parameter.get_prefix_separator_iterator(
+                )
+            serialized_data = parameter.serialize(parameter_data,
+                                                  prefix_separator_iterator)
             for serialized_value in serialized_data.values():
                 used_path += serialized_value
 
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
@@ -210,28 +247,30 @@
             headers=_headers,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
-            api_response = api_client.ApiResponseWithoutDeserialization(response=response)
+            api_response = api_client.ApiResponseWithoutDeserialization(
+                response=response)
         else:
-            response_for_status = _status_code_to_response.get(str(response.status))
+            response_for_status = _status_code_to_response.get(
+                str(response.status))
             if response_for_status:
-                api_response = response_for_status.deserialize(response, self.api_client.configuration)
+                api_response = response_for_status.deserialize(
+                    response, self.api_client.configuration)
             else:
-                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
+                api_response = api_client.ApiResponseWithoutDeserialization(
+                    response=response)
 
         if not 200 <= response.status <= 299:
-            raise exceptions.ApiException(
-                status=response.status,
-                reason=response.reason,
-                api_response=api_response
-            )
+            raise exceptions.ApiException(status=response.status,
+                                          reason=response.reason,
+                                          api_response=api_response)
 
         return api_response
 
 
 class ListAvailableMachineTypes(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
@@ -240,105 +279,107 @@
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+            ApiResponseFor200,
+    ]:
+        ...
 
     @typing.overload
     def list_available_machine_types(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    ) -> api_client.ApiResponseWithoutDeserialization:
+        ...
 
     @typing.overload
     def list_available_machine_types(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-        api_client.ApiResponseWithoutDeserialization,
-    ]: ...
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
+        ...
 
     def list_available_machine_types(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._list_available_machine_types_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization
-        )
+            skip_deserialization=skip_deserialization)
 
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+            ApiResponseFor200,
+    ]:
+        ...
 
     @typing.overload
     def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    ) -> api_client.ApiResponseWithoutDeserialization:
+        ...
 
     @typing.overload
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-        api_client.ApiResponseWithoutDeserialization,
-    ]: ...
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
+        ...
 
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._list_available_machine_types_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization
-        )
-
-
+            skip_deserialization=skip_deserialization)
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_price/get.py` & `inductiva-0.6.0/inductiva/client/paths/compute_price/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_price/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/compute_price/get.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_type/get.py` & `inductiva-0.6.0/inductiva/client/paths/compute_type/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
-from inductiva.client.model.base_machine_type import BaseMachineType
 from inductiva.client.model.providers import Providers
 from inductiva.client.model.http_validation_error import HTTPValidationError
+from inductiva.client.model.machine_type import MachineType
 
 from . import path
 
 # Query params
 NumCpusSchema = schemas.IntSchema
 
 
@@ -195,15 +195,15 @@
     style=api_client.ParameterStyle.FORM,
     schema=ProviderIdSchema,
     explode=True,
 )
 _auth = [
     'APIKeyHeader',
 ]
-SchemaFor200ResponseBodyApplicationJson = BaseMachineType
+SchemaFor200ResponseBodyApplicationJson = MachineType
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/compute_type/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/compute_type/get.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
-from inductiva.client.model.base_machine_type import BaseMachineType
 from inductiva.client.model.providers import Providers
 from inductiva.client.model.http_validation_error import HTTPValidationError
+from inductiva.client.model.machine_type import MachineType
 
 # Query params
 NumCpusSchema = schemas.IntSchema
 
 
 class SpotSchema(
     schemas.ComposedSchema,
@@ -141,15 +141,15 @@
 )
 request_query_provider_id = api_client.QueryParameter(
     name="provider_id",
     style=api_client.ParameterStyle.FORM,
     schema=ProviderIdSchema,
     explode=True,
 )
-SchemaFor200ResponseBodyApplicationJson = BaseMachineType
+SchemaFor200ResponseBodyApplicationJson = MachineType
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/storage_contents/delete.py` & `inductiva-0.6.0/inductiva/client/paths/storage_contents/delete.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/storage_contents/delete.pyi` & `inductiva-0.6.0/inductiva/client/paths/storage_contents/delete.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/storage_contents/get.py` & `inductiva-0.6.0/inductiva/client/paths/projects/get.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # coding: utf-8
+
 """
 
 
     Generated by: https://openapi-generator.tech
 """
 
 from dataclasses import dataclass
@@ -20,143 +21,103 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
-from inductiva.client.model.providers import Providers
+from inductiva.client.model.project import Project
 from inductiva.client.model.http_validation_error import HTTPValidationError
 
-from . import path
-
 # Query params
-MaxResultsSchema = schemas.IntSchema
-
-
-class SortBySchema(schemas.EnumBase, schemas.StrSchema):
-
-    class MetaOapg:
-        enum_value_to_name = {
-            "size": "SIZE",
-            "creation_time": "CREATION_TIME",
-        }
-
-    @schemas.classproperty
-    def SIZE(cls):
-        return cls("size")
-
-    @schemas.classproperty
-    def CREATION_TIME(cls):
-        return cls("creation_time")
-
 
-class OrderSchema(schemas.EnumBase, schemas.StrSchema):
 
-    class MetaOapg:
-        enum_value_to_name = {
-            "asc": "ASC",
-            "desc": "DESC",
-        }
-
-    @schemas.classproperty
-    def ASC(cls):
-        return cls("asc")
-
-    @schemas.classproperty
-    def DESC(cls):
-        return cls("desc")
+class PageSchema(
+    schemas.IntSchema
+):
+    pass
 
 
-PathSchema = schemas.StrSchema
-ProviderIdSchema = Providers
+class PerPageSchema(
+    schemas.IntSchema
+):
+    pass
 RequestRequiredQueryParams = typing_extensions.TypedDict(
-    'RequestRequiredQueryParams', {})
+    'RequestRequiredQueryParams',
+    {
+    }
+)
 RequestOptionalQueryParams = typing_extensions.TypedDict(
-    'RequestOptionalQueryParams', {
-        'max_results': typing.Union[
-            MaxResultsSchema,
-            decimal.Decimal,
-            int,
-        ],
-        'sort_by': typing.Union[
-            SortBySchema,
-            str,
-        ],
-        'order': typing.Union[
-            OrderSchema,
-            str,
-        ],
-        'path': typing.Union[
-            PathSchema,
-            str,
-        ],
-        'provider_id': typing.Union[
-            ProviderIdSchema,
-        ],
+    'RequestOptionalQueryParams',
+    {
+        'page': typing.Union[PageSchema, decimal.Decimal, int, ],
+        'per_page': typing.Union[PerPageSchema, decimal.Decimal, int, ],
     },
-    total=False)
+    total=False
+)
 
 
-class RequestQueryParams(RequestRequiredQueryParams,
-                         RequestOptionalQueryParams):
+class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
 
 
-request_query_max_results = api_client.QueryParameter(
-    name="max_results",
-    style=api_client.ParameterStyle.FORM,
-    schema=MaxResultsSchema,
-    explode=True,
-)
-request_query_sort_by = api_client.QueryParameter(
-    name="sort_by",
-    style=api_client.ParameterStyle.FORM,
-    schema=SortBySchema,
-    explode=True,
-)
-request_query_order = api_client.QueryParameter(
-    name="order",
-    style=api_client.ParameterStyle.FORM,
-    schema=OrderSchema,
-    explode=True,
-)
-request_query_path = api_client.QueryParameter(
-    name="path",
+request_query_page = api_client.QueryParameter(
+    name="page",
     style=api_client.ParameterStyle.FORM,
-    schema=PathSchema,
+    schema=PageSchema,
     explode=True,
 )
-request_query_provider_id = api_client.QueryParameter(
-    name="provider_id",
+request_query_per_page = api_client.QueryParameter(
+    name="per_page",
     style=api_client.ParameterStyle.FORM,
-    schema=ProviderIdSchema,
+    schema=PerPageSchema,
     explode=True,
 )
-_auth = [
-    'APIKeyHeader',
-]
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+
+
+class SchemaFor200ResponseBodyApplicationJson(
+    schemas.ListSchema
+):
+
+
+    class MetaOapg:
+        
+        @staticmethod
+        def items() -> typing.Type['Project']:
+            return Project
+
+    def __new__(
+        cls,
+        _arg: typing.Union[typing.Tuple['Project'], typing.List['Project']],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+    ) -> 'SchemaFor200ResponseBodyApplicationJson':
+        return super().__new__(
+            cls,
+            _arg,
+            _configuration=_configuration,
+        )
+
+    def __getitem__(self, i: int) -> 'Project':
+        return super().__getitem__(i)
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
-        'application/json':
-            api_client.MediaType(schema=SchemaFor200ResponseBodyApplicationJson
-                                ),
+        'application/json': api_client.MediaType(
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationError
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
@@ -166,99 +127,87 @@
     ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_422 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor422,
     content={
-        'application/json':
-            api_client.MediaType(schema=SchemaFor422ResponseBodyApplicationJson
-                                ),
+        'application/json': api_client.MediaType(
+            schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
-_all_accept_content_types = ('application/json',)
+_all_accept_content_types = (
+    'application/json',
+)
 
 
 class BaseApi(api_client.Api):
-
     @typing.overload
-    def _list_storage_contents_oapg(
+    def _get_user_projects_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-    ]:
-        ...
+        ApiResponseFor200,
+    ]: ...
 
     @typing.overload
-    def _list_storage_contents_oapg(
+    def _get_user_projects_oapg(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization:
-        ...
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def _list_storage_contents_oapg(
+    def _get_user_projects_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-            api_client.ApiResponseWithoutDeserialization,
-    ]:
-        ...
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
 
-    def _list_storage_contents_oapg(
+    def _get_user_projects_oapg(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        List Storage Contents
+        Get User Projects
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestQueryParams, query_params)
         used_path = path.value
 
         prefix_separator_iterator = None
         for parameter in (
-                request_query_max_results,
-                request_query_sort_by,
-                request_query_order,
-                request_query_path,
-                request_query_provider_id,
+            request_query_page,
+            request_query_per_page,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
-                prefix_separator_iterator = parameter.get_prefix_separator_iterator(
-                )
-            serialized_data = parameter.serialize(parameter_data,
-                                                  prefix_separator_iterator)
+                prefix_separator_iterator = parameter.get_prefix_separator_iterator()
+            serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
             for serialized_value in serialized_data.values():
                 used_path += serialized_value
 
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
@@ -270,139 +219,135 @@
             headers=_headers,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
-            api_response = api_client.ApiResponseWithoutDeserialization(
-                response=response)
+            api_response = api_client.ApiResponseWithoutDeserialization(response=response)
         else:
-            response_for_status = _status_code_to_response.get(
-                str(response.status))
+            response_for_status = _status_code_to_response.get(str(response.status))
             if response_for_status:
-                api_response = response_for_status.deserialize(
-                    response, self.api_client.configuration)
+                api_response = response_for_status.deserialize(response, self.api_client.configuration)
             else:
-                api_response = api_client.ApiResponseWithoutDeserialization(
-                    response=response)
+                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
 
         if not 200 <= response.status <= 299:
-            raise exceptions.ApiException(status=response.status,
-                                          reason=response.reason,
-                                          api_response=api_response)
+            raise exceptions.ApiException(
+                status=response.status,
+                reason=response.reason,
+                api_response=api_response
+            )
 
         return api_response
 
 
-class ListStorageContents(BaseApi):
+class GetUserProjects(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def list_storage_contents(
+    def get_user_projects(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-    ]:
-        ...
+        ApiResponseFor200,
+    ]: ...
 
     @typing.overload
-    def list_storage_contents(
+    def get_user_projects(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization:
-        ...
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def list_storage_contents(
+    def get_user_projects(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-            api_client.ApiResponseWithoutDeserialization,
-    ]:
-        ...
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
 
-    def list_storage_contents(
+    def get_user_projects(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_storage_contents_oapg(
+        return self._get_user_projects_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization)
+            skip_deserialization=skip_deserialization
+        )
 
 
 class ApiForget(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-    ]:
-        ...
+        ApiResponseFor200,
+    ]: ...
 
     @typing.overload
     def get(
         self,
         skip_deserialization: typing_extensions.Literal[True],
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization:
-        ...
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-            api_client.ApiResponseWithoutDeserialization,
-    ]:
-        ...
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
 
     def get(
         self,
         query_params: RequestQueryParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._list_storage_contents_oapg(
+        return self._get_user_projects_oapg(
             query_params=query_params,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization)
+            skip_deserialization=skip_deserialization
+        )
+
+
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/storage_contents/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/storage_contents/get.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
 from inductiva.client.model.providers import Providers
+from inductiva.client.model.storage_file_info import StorageFileInfo
 from inductiva.client.model.http_validation_error import HTTPValidationError
 
 # Query params
 MaxResultsSchema = schemas.IntSchema
 
 
 class SortBySchema(
@@ -108,15 +109,46 @@
 )
 request_query_provider_id = api_client.QueryParameter(
     name="provider_id",
     style=api_client.ParameterStyle.FORM,
     schema=ProviderIdSchema,
     explode=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+
+
+class SchemaFor200ResponseBodyApplicationJson(
+    schemas.DictSchema
+):
+
+
+    class MetaOapg:
+        
+        @staticmethod
+        def additional_properties() -> typing.Type['StorageFileInfo']:
+            return StorageFileInfo
+    
+    def __getitem__(self, name: typing.Union[str, ]) -> 'StorageFileInfo':
+        # dict_instance[name] accessor
+        return super().__getitem__(name)
+    
+    def get_item_oapg(self, name: typing.Union[str, ]) -> 'StorageFileInfo':
+        return super().get_item_oapg(name)
+
+    def __new__(
+        cls,
+        *_args: typing.Union[dict, frozendict.frozendict, ],
+        _configuration: typing.Optional[schemas.Configuration] = None,
+        **kwargs: 'StorageFileInfo',
+    ) -> 'SchemaFor200ResponseBodyApplicationJson':
+        return super().__new__(
+            cls,
+            *_args,
+            _configuration=_configuration,
+            **kwargs,
+        )
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/storage_size/get.py` & `inductiva-0.6.0/inductiva/client/paths/storage_size/get.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     style=api_client.ParameterStyle.FORM,
     schema=ProviderIdSchema,
     explode=True,
 )
 _auth = [
     'APIKeyHeader',
 ]
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+SchemaFor200ResponseBodyApplicationJson = schemas.IntSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/storage_size/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/storage_size/get.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 request_query_provider_id = api_client.QueryParameter(
     name="provider_id",
     style=api_client.ParameterStyle.FORM,
     schema=ProviderIdSchema,
     explode=True,
 )
-SchemaFor200ResponseBodyApplicationJson = schemas.AnyTypeSchema
+SchemaFor200ResponseBodyApplicationJson = schemas.IntSchema
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks/get.py` & `inductiva-0.6.0/inductiva/client/paths/tasks/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,31 @@
 from inductiva.client.model.task_status_code import TaskStatusCode
 from inductiva.client.model.task import Task
 from inductiva.client.model.http_validation_error import HTTPValidationError
 
 from . import path
 
 # Query params
-PageSchema = schemas.IntSchema
-PerPageSchema = schemas.IntSchema
+
+
+class PageSchema(schemas.IntSchema):
+
+    class MetaOapg:
+        inclusive_minimum = 1
+
+
+class PerPageSchema(schemas.IntSchema):
+
+    class MetaOapg:
+        inclusive_maximum = 500
+        inclusive_minimum = 1
+
+
 StatusSchema = TaskStatusCode
+ProjectSchema = schemas.StrSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams', {})
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams', {
         'page': typing.Union[
             PageSchema,
             decimal.Decimal,
@@ -47,14 +61,18 @@
             PerPageSchema,
             decimal.Decimal,
             int,
         ],
         'status': typing.Union[
             StatusSchema,
         ],
+        'project': typing.Union[
+            ProjectSchema,
+            str,
+        ],
     },
     total=False)
 
 
 class RequestQueryParams(RequestRequiredQueryParams,
                          RequestOptionalQueryParams):
     pass
@@ -74,14 +92,20 @@
 )
 request_query_status = api_client.QueryParameter(
     name="status",
     style=api_client.ParameterStyle.FORM,
     schema=StatusSchema,
     explode=True,
 )
+request_query_project = api_client.QueryParameter(
+    name="project",
+    style=api_client.ParameterStyle.FORM,
+    schema=ProjectSchema,
+    explode=True,
+)
 _auth = [
     'APIKeyHeader',
 ]
 
 
 class SchemaFor200ResponseBodyApplicationJson(schemas.ListSchema):
 
@@ -208,14 +232,15 @@
         used_path = path.value
 
         prefix_separator_iterator = None
         for parameter in (
                 request_query_page,
                 request_query_per_page,
                 request_query_status,
+                request_query_project,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator(
                 )
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/tasks/get.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,28 +26,40 @@
 from inductiva.client import schemas  # noqa: F401
 
 from inductiva.client.model.task_status_code import TaskStatusCode
 from inductiva.client.model.task import Task
 from inductiva.client.model.http_validation_error import HTTPValidationError
 
 # Query params
-PageSchema = schemas.IntSchema
-PerPageSchema = schemas.IntSchema
+
+
+class PageSchema(
+    schemas.IntSchema
+):
+    pass
+
+
+class PerPageSchema(
+    schemas.IntSchema
+):
+    pass
 StatusSchema = TaskStatusCode
+ProjectSchema = schemas.StrSchema
 RequestRequiredQueryParams = typing_extensions.TypedDict(
     'RequestRequiredQueryParams',
     {
     }
 )
 RequestOptionalQueryParams = typing_extensions.TypedDict(
     'RequestOptionalQueryParams',
     {
         'page': typing.Union[PageSchema, decimal.Decimal, int, ],
         'per_page': typing.Union[PerPageSchema, decimal.Decimal, int, ],
         'status': typing.Union[StatusSchema, ],
+        'project': typing.Union[ProjectSchema, str, ],
     },
     total=False
 )
 
 
 class RequestQueryParams(RequestRequiredQueryParams, RequestOptionalQueryParams):
     pass
@@ -67,14 +79,20 @@
 )
 request_query_status = api_client.QueryParameter(
     name="status",
     style=api_client.ParameterStyle.FORM,
     schema=StatusSchema,
     explode=True,
 )
+request_query_project = api_client.QueryParameter(
+    name="project",
+    style=api_client.ParameterStyle.FORM,
+    schema=ProjectSchema,
+    explode=True,
+)
 
 
 class SchemaFor200ResponseBodyApplicationJson(
     schemas.ListSchema
 ):
 
 
@@ -193,14 +211,15 @@
         used_path = path.value
 
         prefix_separator_iterator = None
         for parameter in (
             request_query_page,
             request_query_per_page,
             request_query_status,
+            request_query_project,
         ):
             parameter_data = query_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             if prefix_separator_iterator is None:
                 prefix_separator_iterator = parameter.get_prefix_separator_iterator()
             serialized_data = parameter.serialize(parameter_data, prefix_separator_iterator)
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_auth/get.py` & `inductiva-0.6.0/inductiva/client/paths/tasks_auth/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_auth/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/tasks_auth/get.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_submit/post.py` & `inductiva-0.6.0/inductiva/client/paths/tasks_submit/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_submit/post.pyi` & `inductiva-0.6.0/inductiva/client/paths/tasks_submit/post.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_task_id/get.py` & `inductiva-0.6.0/inductiva/client/paths/tasks_task_id/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_task_id/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/tasks_task_id/get.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_task_id_input/post.py` & `inductiva-0.6.0/inductiva/client/paths/tasks_task_id_input/put.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # coding: utf-8
+
 """
 
 
     Generated by: https://openapi-generator.tech
 """
 
 from dataclasses import dataclass
@@ -20,53 +21,54 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
-from inductiva.client.model.body_upload_task_input import BodyUploadTaskInput
 from inductiva.client.model.task_status import TaskStatus
 from inductiva.client.model.http_validation_error import HTTPValidationError
 
-from . import path
-
 # Path params
 TaskIdSchema = schemas.StrSchema
 RequestRequiredPathParams = typing_extensions.TypedDict(
-    'RequestRequiredPathParams', {
-        'task_id': typing.Union[
-            TaskIdSchema,
-            str,
-        ],
-    })
+    'RequestRequiredPathParams',
+    {
+        'task_id': typing.Union[TaskIdSchema, str, ],
+    }
+)
 RequestOptionalPathParams = typing_extensions.TypedDict(
-    'RequestOptionalPathParams', {}, total=False)
+    'RequestOptionalPathParams',
+    {
+    },
+    total=False
+)
 
 
 class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
     pass
 
 
 request_path_task_id = api_client.PathParameter(
     name="task_id",
     style=api_client.ParameterStyle.SIMPLE,
     schema=TaskIdSchema,
     required=True,
 )
 # body param
-SchemaForRequestBodyMultipartFormData = BodyUploadTaskInput
+SchemaForRequestBodyApplicationOctetStream = schemas.BinarySchema
+
 
-request_body_body = api_client.RequestBody(content={
-    'multipart/form-data':
-        api_client.MediaType(schema=SchemaForRequestBodyMultipartFormData),
-},)
-_auth = [
-    'APIKeyHeader',
-]
+request_body_body = api_client.RequestBody(
+    content={
+        'application/octet-stream': api_client.MediaType(
+            schema=SchemaForRequestBodyApplicationOctetStream),
+    },
+    required=True,
+)
 SchemaFor200ResponseBodyApplicationJson = TaskStatus
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
@@ -74,17 +76,16 @@
     ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
-        'application/json':
-            api_client.MediaType(schema=SchemaFor200ResponseBodyApplicationJson
-                                ),
+        'application/json': api_client.MediaType(
+            schema=SchemaFor200ResponseBodyApplicationJson),
     },
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationError
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
@@ -94,96 +95,84 @@
     ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_422 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor422,
     content={
-        'application/json':
-            api_client.MediaType(schema=SchemaFor422ResponseBodyApplicationJson
-                                ),
+        'application/json': api_client.MediaType(
+            schema=SchemaFor422ResponseBodyApplicationJson),
     },
 )
-_status_code_to_response = {
-    '200': _response_for_200,
-    '422': _response_for_422,
-}
-_all_accept_content_types = ('application/json',)
+_all_accept_content_types = (
+    'application/json',
+)
 
 
 class BaseApi(api_client.Api):
-
     @typing.overload
     def _upload_task_input_oapg(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
+        content_type: typing_extensions.Literal["application/octet-stream"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-    ]:
-        ...
+        ApiResponseFor200,
+    ]: ...
 
     @typing.overload
     def _upload_task_input_oapg(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-    ]:
-        ...
+        ApiResponseFor200,
+    ]: ...
+
 
     @typing.overload
     def _upload_task_input_oapg(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization:
-        ...
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def _upload_task_input_oapg(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-            api_client.ApiResponseWithoutDeserialization,
-    ]:
-        ...
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
 
     def _upload_task_input_oapg(
         self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
+        content_type: str = 'application/octet-stream',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
@@ -192,15 +181,17 @@
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
         self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
         _path_params = {}
-        for parameter in (request_path_task_id,):
+        for parameter in (
+            request_path_task_id,
+        ):
             parameter_data = path_params.get(parameter.name, schemas.unset)
             if parameter_data is schemas.unset:
                 continue
             serialized_data = parameter.serialize(parameter_data)
             _path_params.update(serialized_data)
 
         for k, v in _path_params.items():
@@ -208,220 +199,208 @@
 
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead')
         _fields = None
         _body = None
-        if body is not schemas.unset:
-            serialized_data = request_body_body.serialize(body, content_type)
-            _headers.add('Content-Type', content_type)
-            if 'fields' in serialized_data:
-                _fields = serialized_data['fields']
-            elif 'body' in serialized_data:
-                _body = serialized_data['body']
+        serialized_data = request_body_body.serialize(body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
-            method='post'.upper(),
+            method='put'.upper(),
             headers=_headers,
             fields=_fields,
             body=_body,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
-            api_response = api_client.ApiResponseWithoutDeserialization(
-                response=response)
+            api_response = api_client.ApiResponseWithoutDeserialization(response=response)
         else:
-            response_for_status = _status_code_to_response.get(
-                str(response.status))
+            response_for_status = _status_code_to_response.get(str(response.status))
             if response_for_status:
-                api_response = response_for_status.deserialize(
-                    response, self.api_client.configuration)
+                api_response = response_for_status.deserialize(response, self.api_client.configuration)
             else:
-                api_response = api_client.ApiResponseWithoutDeserialization(
-                    response=response)
+                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
 
         if not 200 <= response.status <= 299:
-            raise exceptions.ApiException(status=response.status,
-                                          reason=response.reason,
-                                          api_response=api_response)
+            raise exceptions.ApiException(
+                status=response.status,
+                reason=response.reason,
+                api_response=api_response
+            )
 
         return api_response
 
 
 class UploadTaskInput(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
     def upload_task_input(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
+        content_type: typing_extensions.Literal["application/octet-stream"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-    ]:
-        ...
+        ApiResponseFor200,
+    ]: ...
 
     @typing.overload
     def upload_task_input(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-    ]:
-        ...
+        ApiResponseFor200,
+    ]: ...
+
 
     @typing.overload
     def upload_task_input(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization:
-        ...
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
     def upload_task_input(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-            api_client.ApiResponseWithoutDeserialization,
-    ]:
-        ...
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
 
     def upload_task_input(
         self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
+        content_type: str = 'application/octet-stream',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._upload_task_input_oapg(
             body=body,
             path_params=path_params,
             content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization)
+            skip_deserialization=skip_deserialization
+        )
 
 
-class ApiForpost(BaseApi):
+class ApiForput(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
-    def post(
+    def put(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
+        content_type: typing_extensions.Literal["application/octet-stream"] = ...,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-    ]:
-        ...
+        ApiResponseFor200,
+    ]: ...
 
     @typing.overload
-    def post(
+    def put(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-    ]:
-        ...
+        ApiResponseFor200,
+    ]: ...
+
 
     @typing.overload
-    def post(
+    def put(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization:
-        ...
+    ) -> api_client.ApiResponseWithoutDeserialization: ...
 
     @typing.overload
-    def post(
+    def put(
         self,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-            ApiResponseFor200,
-            api_client.ApiResponseWithoutDeserialization,
-    ]:
-        ...
-
-    def post(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData,
-                           schemas.Unset] = schemas.unset,
+        ApiResponseFor200,
+        api_client.ApiResponseWithoutDeserialization,
+    ]: ...
+
+    def put(
+        self,
+        body: typing.Union[SchemaForRequestBodyApplicationOctetStream,bytes, io.FileIO, io.BufferedReader, ],
+        content_type: str = 'application/octet-stream',
         path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         return self._upload_task_input_oapg(
             body=body,
             path_params=path_params,
             content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization)
+            skip_deserialization=skip_deserialization
+        )
+
+
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_task_id_input/post.pyi` & `inductiva-0.6.0/inductiva/client/paths/projects/post.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # coding: utf-8
-
 """
 
 
     Generated by: https://openapi-generator.tech
 """
 
 from dataclasses import dataclass
@@ -21,71 +20,51 @@
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
 from inductiva.client import schemas  # noqa: F401
 
-from inductiva.client.model.body_upload_task_input import BodyUploadTaskInput
-from inductiva.client.model.task_status import TaskStatus
+from inductiva.client.model.project import Project
+from inductiva.client.model.project_create import ProjectCreate
 from inductiva.client.model.http_validation_error import HTTPValidationError
 
-# Path params
-TaskIdSchema = schemas.StrSchema
-RequestRequiredPathParams = typing_extensions.TypedDict(
-    'RequestRequiredPathParams',
-    {
-        'task_id': typing.Union[TaskIdSchema, str, ],
-    }
-)
-RequestOptionalPathParams = typing_extensions.TypedDict(
-    'RequestOptionalPathParams',
-    {
-    },
-    total=False
-)
-
-
-class RequestPathParams(RequestRequiredPathParams, RequestOptionalPathParams):
-    pass
+from . import path
 
-
-request_path_task_id = api_client.PathParameter(
-    name="task_id",
-    style=api_client.ParameterStyle.SIMPLE,
-    schema=TaskIdSchema,
-    required=True,
-)
 # body param
-SchemaForRequestBodyMultipartFormData = BodyUploadTaskInput
+SchemaForRequestBodyApplicationJson = ProjectCreate
 
-
-request_body_body = api_client.RequestBody(
+request_body_project_create = api_client.RequestBody(
     content={
-        'multipart/form-data': api_client.MediaType(
-            schema=SchemaForRequestBodyMultipartFormData),
+        'application/json':
+            api_client.MediaType(schema=SchemaForRequestBodyApplicationJson),
     },
+    required=True,
 )
-SchemaFor200ResponseBodyApplicationJson = TaskStatus
+_auth = [
+    'APIKeyHeader',
+]
+SchemaFor200ResponseBodyApplicationJson = Project
 
 
 @dataclass
 class ApiResponseFor200(api_client.ApiResponse):
     response: urllib3.HTTPResponse
     body: typing.Union[
         SchemaFor200ResponseBodyApplicationJson,
     ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_200 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor200,
     content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor200ResponseBodyApplicationJson),
+        'application/json':
+            api_client.MediaType(schema=SchemaFor200ResponseBodyApplicationJson
+                                ),
     },
 )
 SchemaFor422ResponseBodyApplicationJson = HTTPValidationError
 
 
 @dataclass
 class ApiResponseFor422(api_client.ApiResponse):
@@ -95,310 +74,324 @@
     ]
     headers: schemas.Unset = schemas.unset
 
 
 _response_for_422 = api_client.OpenApiResponse(
     response_cls=ApiResponseFor422,
     content={
-        'application/json': api_client.MediaType(
-            schema=SchemaFor422ResponseBodyApplicationJson),
+        'application/json':
+            api_client.MediaType(schema=SchemaFor422ResponseBodyApplicationJson
+                                ),
     },
 )
-_all_accept_content_types = (
-    'application/json',
-)
+_status_code_to_response = {
+    '200': _response_for_200,
+    '422': _response_for_422,
+}
+_all_accept_content_types = ('application/json',)
 
 
 class BaseApi(api_client.Api):
+
     @typing.overload
-    def _upload_task_input_oapg(
+    def _create_project_oapg(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
+        content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+            ApiResponseFor200,
+    ]:
+        ...
 
     @typing.overload
-    def _upload_task_input_oapg(
+    def _create_project_oapg(
         self,
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
+            ApiResponseFor200,
+    ]:
+        ...
 
     @typing.overload
-    def _upload_task_input_oapg(
+    def _create_project_oapg(
         self,
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    ) -> api_client.ApiResponseWithoutDeserialization:
+        ...
 
     @typing.overload
-    def _upload_task_input_oapg(
+    def _create_project_oapg(
         self,
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-        api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def _upload_task_input_oapg(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
+        ...
+
+    def _create_project_oapg(
+        self,
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
+        content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
         """
-        Upload Task Input
+        Create Project
         :param skip_deserialization: If true then api_response.response will be set but
             api_response.body and api_response.headers will not be deserialized into schema
             class instances
         """
-        self._verify_typed_dict_inputs_oapg(RequestPathParams, path_params)
         used_path = path.value
 
-        _path_params = {}
-        for parameter in (
-            request_path_task_id,
-        ):
-            parameter_data = path_params.get(parameter.name, schemas.unset)
-            if parameter_data is schemas.unset:
-                continue
-            serialized_data = parameter.serialize(parameter_data)
-            _path_params.update(serialized_data)
-
-        for k, v in _path_params.items():
-            used_path = used_path.replace('{%s}' % k, v)
-
         _headers = HTTPHeaderDict()
         # TODO add cookie handling
         if accept_content_types:
             for accept_content_type in accept_content_types:
                 _headers.add('Accept', accept_content_type)
 
+        if body is schemas.unset:
+            raise exceptions.ApiValueError(
+                'The required body parameter has an invalid value of: unset. Set a valid value instead'
+            )
         _fields = None
         _body = None
-        if body is not schemas.unset:
-            serialized_data = request_body_body.serialize(body, content_type)
-            _headers.add('Content-Type', content_type)
-            if 'fields' in serialized_data:
-                _fields = serialized_data['fields']
-            elif 'body' in serialized_data:
-                _body = serialized_data['body']
+        serialized_data = request_body_project_create.serialize(
+            body, content_type)
+        _headers.add('Content-Type', content_type)
+        if 'fields' in serialized_data:
+            _fields = serialized_data['fields']
+        elif 'body' in serialized_data:
+            _body = serialized_data['body']
         response = self.api_client.call_api(
             resource_path=used_path,
             method='post'.upper(),
             headers=_headers,
             fields=_fields,
             body=_body,
             auth_settings=_auth,
             stream=stream,
             timeout=timeout,
         )
 
         if skip_deserialization:
-            api_response = api_client.ApiResponseWithoutDeserialization(response=response)
+            api_response = api_client.ApiResponseWithoutDeserialization(
+                response=response)
         else:
-            response_for_status = _status_code_to_response.get(str(response.status))
+            response_for_status = _status_code_to_response.get(
+                str(response.status))
             if response_for_status:
-                api_response = response_for_status.deserialize(response, self.api_client.configuration)
+                api_response = response_for_status.deserialize(
+                    response, self.api_client.configuration)
             else:
-                api_response = api_client.ApiResponseWithoutDeserialization(response=response)
+                api_response = api_client.ApiResponseWithoutDeserialization(
+                    response=response)
 
         if not 200 <= response.status <= 299:
-            raise exceptions.ApiException(
-                status=response.status,
-                reason=response.reason,
-                api_response=api_response
-            )
+            raise exceptions.ApiException(status=response.status,
+                                          reason=response.reason,
+                                          api_response=api_response)
 
         return api_response
 
 
-class UploadTaskInput(BaseApi):
+class CreateProject(BaseApi):
     # this class is used by api classes that refer to endpoints with operationId fn names
 
     @typing.overload
-    def upload_task_input(
+    def create_project(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
+        content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+            ApiResponseFor200,
+    ]:
+        ...
 
     @typing.overload
-    def upload_task_input(
+    def create_project(
         self,
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
+            ApiResponseFor200,
+    ]:
+        ...
 
     @typing.overload
-    def upload_task_input(
+    def create_project(
         self,
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    ) -> api_client.ApiResponseWithoutDeserialization:
+        ...
 
     @typing.overload
-    def upload_task_input(
+    def create_project(
         self,
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-        api_client.ApiResponseWithoutDeserialization,
-    ]: ...
-
-    def upload_task_input(
-        self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
+        ...
+
+    def create_project(
+        self,
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
+        content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._upload_task_input_oapg(
+        return self._create_project_oapg(
             body=body,
-            path_params=path_params,
             content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization
-        )
+            skip_deserialization=skip_deserialization)
 
 
 class ApiForpost(BaseApi):
     # this class is used by api classes that refer to endpoints by path and http method names
 
     @typing.overload
     def post(
         self,
-        content_type: typing_extensions.Literal["multipart/form-data"] = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
+        content_type: typing_extensions.Literal["application/json"] = ...,
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
+            ApiResponseFor200,
+    ]:
+        ...
 
     @typing.overload
     def post(
         self,
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: typing_extensions.Literal[False] = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-    ]: ...
-
+            ApiResponseFor200,
+    ]:
+        ...
 
     @typing.overload
     def post(
         self,
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         skip_deserialization: typing_extensions.Literal[True],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
-    ) -> api_client.ApiResponseWithoutDeserialization: ...
+    ) -> api_client.ApiResponseWithoutDeserialization:
+        ...
 
     @typing.overload
     def post(
         self,
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
         content_type: str = ...,
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = ...,
     ) -> typing.Union[
-        ApiResponseFor200,
-        api_client.ApiResponseWithoutDeserialization,
-    ]: ...
+            ApiResponseFor200,
+            api_client.ApiResponseWithoutDeserialization,
+    ]:
+        ...
 
     def post(
         self,
-        content_type: str = 'multipart/form-data',
-        body: typing.Union[SchemaForRequestBodyMultipartFormData, schemas.Unset] = schemas.unset,
-        path_params: RequestPathParams = frozendict.frozendict(),
+        body: typing.Union[
+            SchemaForRequestBodyApplicationJson,
+        ],
+        content_type: str = 'application/json',
         accept_content_types: typing.Tuple[str] = _all_accept_content_types,
         stream: bool = False,
         timeout: typing.Optional[typing.Union[int, typing.Tuple]] = None,
         skip_deserialization: bool = False,
     ):
-        return self._upload_task_input_oapg(
+        return self._create_project_oapg(
             body=body,
-            path_params=path_params,
             content_type=content_type,
             accept_content_types=accept_content_types,
             stream=stream,
             timeout=timeout,
-            skip_deserialization=skip_deserialization
-        )
-
-
+            skip_deserialization=skip_deserialization)
```

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_task_id_kill/post.py` & `inductiva-0.6.0/inductiva/client/paths/tasks_task_id_kill/post.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_task_id_kill/post.pyi` & `inductiva-0.6.0/inductiva/client/paths/tasks_task_id_kill/post.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_task_id_output/get.py` & `inductiva-0.6.0/inductiva/client/paths/tasks_task_id_output/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_task_id_output/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/tasks_task_id_output/get.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_task_id_output_list/get.py` & `inductiva-0.6.0/inductiva/client/paths/tasks_task_id_output_list/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_task_id_output_list/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/tasks_task_id_output_list/get.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_task_id_status/get.py` & `inductiva-0.6.0/inductiva/client/paths/tasks_task_id_status/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/tasks_task_id_status/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/tasks_task_id_status/get.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/version/get.py` & `inductiva-0.6.0/inductiva/client/paths/version/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/version/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/version/get.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/version_check/get.py` & `inductiva-0.6.0/inductiva/client/paths/version_check/get.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/paths/version_check/get.pyi` & `inductiva-0.6.0/inductiva/client/paths/version_check/get.pyi`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/rest.py` & `inductiva-0.6.0/inductiva/client/rest.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/client/schemas.py` & `inductiva-0.6.0/inductiva/client/schemas.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/commands/commands.py` & `inductiva-0.6.0/inductiva/commands/commands.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/localization/localization.py` & `inductiva-0.6.0/inductiva/localization/localization.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/localization/translations/en.json` & `inductiva-0.6.0/inductiva/localization/translations/en.json`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/logs/log.py` & `inductiva-0.6.0/inductiva/logs/log.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/resources/machine_cluster.py` & `inductiva-0.6.0/inductiva/resources/machine_cluster.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/resources/machine_groups.py` & `inductiva-0.6.0/inductiva/resources/machine_groups.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/resources/machine_types.py` & `inductiva-0.6.0/inductiva/resources/machine_types.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/resources/machines.py` & `inductiva-0.6.0/inductiva/resources/machines.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/resources/machines_base.py` & `inductiva-0.6.0/inductiva/resources/machines_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             data_disk_gb=resp["disk_size_gb"],
             register=False,
         )
         machine_group._id = resp["id"]
         machine_group.provider = resp["provider_id"]
         machine_group._name = resp["name"]
         machine_group.create_time = resp["creation_timestamp"]
-        machine_group._started = True
+        machine_group._started = bool(resp["started"])
 
         return machine_group
 
     def update_termination_timers(self,
                                   max_idle_time: datetime.timedelta = None,
                                   auto_terminate_ts: datetime.datetime = None):
         """Update the termination timers of a machine group.
```

### Comparing `inductiva-0.5.3/inductiva/simulators/dualsphysics.py` & `inductiva-0.6.0/inductiva/simulators/dualsphysics.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     def run(
         self,
         input_dir: types.Path,
         commands: types.Commands,
         on: Optional[types.ComputationalResources] = None,
         storage_dir: Optional[types.Path] = "",
         extra_metadata: Optional[dict] = None,
+        **kwargs,
     ) -> tasks.Task:
         """Executes a DualSPHysics simulation.
 
         Args:
             input_dir: Directory with simulation input files.
             sim_config_filename: Simulation config file.
             on: The computational resource to launch the simulation on. If None
@@ -32,8 +33,9 @@
         Returns:
             tasks.Task: An object representing the simulation task.
         """
         return super().run(input_dir,
                            on=on,
                            commands=commands,
                            storage_dir=storage_dir,
-                           extra_metadata=extra_metadata)
+                           extra_metadata=extra_metadata,
+                           **kwargs)
```

### Comparing `inductiva-0.5.3/inductiva/simulators/dummy_simulator.py` & `inductiva-0.6.0/inductiva/simulators/dummy_simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,23 +18,25 @@
 
     def run(self,
             input_dir: types.Path,
             input_filename: str,
             sleep_time: Optional[float] = 1,
             on: Optional[types.ComputationalResources] = None,
             storage_dir: Optional[types.Path] = "",
-            extra_metadata: Optional[dict] = None) -> tasks.Task:
+            extra_metadata: Optional[dict] = None,
+            **kwargs) -> tasks.Task:
         """Run a dummy simulation that echo's to a file.
         
         Args: 
             input_dir: Path to directory with simulation input files.
             input_filename: Name of the test input file.
             sleep_time: Time to sleep before running the commands.
             extra_metadata: Extra metadata to be sent to the backend.
         """
 
         return super().run(input_dir,
                            on=on,
                            input_filename=input_filename,
                            sleep_time=sleep_time,
                            storage_dir=storage_dir,
-                           extra_metadata=extra_metadata)
+                           extra_metadata=extra_metadata,
+                           **kwargs)
```

### Comparing `inductiva-0.5.3/inductiva/simulators/fds.py` & `inductiva-0.6.0/inductiva/simulators/amr_wind.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,45 @@
-"""FDS simulator module of the API."""
-
+"""AmrWind module of the API for numerical simulations of fluid flows."""
 from typing import Optional
 
 from inductiva import types, tasks, simulators
-from inductiva.utils import meta
 
 
-class FDS(simulators.Simulator):
-    """Class to invoke a generic FDS simulation on the API."""
+@simulators.simulator.mpi_enabled
+class AmrWind(simulators.Simulator):
+    """Class to invoke a generic AmrWind simulation on the API.
+    """
 
     def __init__(self):
+
         super().__init__()
-        self.api_method_name = "fdm.fds.run_simulation"
+        self.api_method_name = "amrWind.amrWind.run_simulation"
 
-    @meta.deprecated_arg(n_cores="n_vcpus")
     def run(self,
             input_dir: types.Path,
             sim_config_filename: str,
-            n_vcpus: Optional[int] = None,
             use_hwthread: bool = True,
-            post_processing_filename: str = None,
-            on: Optional[types.ComputationalResources] = None,
-            storage_dir: Optional[types.Path] = "",
+            n_vcpus: Optional[int] = None,
             extra_metadata: Optional[dict] = None,
+            storage_dir: Optional[types.Path] = "",
+            on: Optional[types.ComputationalResources] = None,
             **kwargs) -> tasks.Task:
         """Run the simulation.
-
         Args:
             input_dir: Path to the directory of the simulation input files.
-            sim_config_filename: Name of the simulation configuration file.
             n_vcpus: Number of vCPUs to use in the simulation. If not provided
             (default), all vCPUs will be used.
             use_hwthread: If specified Open MPI will attempt to discover the
             number of hardware threads on the node, and use that as the
             number of slots available.
             on: The computational resource to launch the simulation on. If None
                 the simulation is submitted to a machine in the default pool.
             other arguments: See the documentation of the base class.
         """
         return super().run(input_dir,
                            on=on,
-                           input_filename=sim_config_filename,
-                           post_processing_config=post_processing_filename,
-                           storage_dir=storage_dir,
                            n_vcpus=n_vcpus,
+                           storage_dir=storage_dir,
                            use_hwthread=use_hwthread,
-                           extra_metadata=extra_metadata)
+                           extra_metadata=extra_metadata,
+                           input_filename=sim_config_filename,
+                           **kwargs)
```

### Comparing `inductiva-0.5.3/inductiva/simulators/fenicsx.py` & `inductiva-0.6.0/inductiva/simulators/fenicsx.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,16 @@
                 - mesh_element_order (int): Order of the mesh element.
                 - mesh_quadrature_rule (str): Mesh quadrature rule.
                 - mesh_quadrature_degree (int): Mesh quadrature degree.
             other arguments: See the documentation of the base class.
         """
 
         return super().run(input_dir,
-                           on=on,
-                           geometry_filename=geometry_filename,
-                           bcs_filename=bcs_filename,
+                           mesh_info_filename=mesh_info_filename,
                            material_filename=material_filename,
+                           geometry_filename=geometry_filename,
+                           extra_metadata=extra_metadata,
                            mesh_filename=mesh_filename,
-                           mesh_info_filename=mesh_info_filename,
+                           bcs_filename=bcs_filename,
                            storage_dir=storage_dir,
-                           extra_metadata=extra_metadata,
+                           on=on,
                            **kwargs)
```

### Comparing `inductiva-0.5.3/inductiva/simulators/gromacs.py` & `inductiva-0.6.0/inductiva/simulators/openfast.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-"""GROMACS module of the API"""
-
+"""OpenFAST module of the API for wind turbine simulations."""
 from typing import Optional
 
 from inductiva import types, tasks, simulators
 
 
-class GROMACS(simulators.Simulator):
-    """Class to invoke any GROMACS command on the API."""
+class OpenFAST(simulators.Simulator):
+    """Class to invoke a generic OpenFAST simulation on the API.
+
+    """
 
     def __init__(self):
+
         super().__init__()
-        self.api_method_name = "md.gromacs.run_simulation"
+        self.api_method_name = "openfast.openfast.run_simulation"
 
-    def run(
-        self,
-        input_dir: types.Path,
-        commands: types.Commands,
-        on: Optional[types.ComputationalResources] = None,
-        storage_dir: Optional[types.Path] = "",
-        extra_metadata: Optional[dict] = None,
-    ) -> tasks.Task:
-        """Run a list of GROMACS commands.
+    def run(self,
+            input_dir: types.Path,
+            commands: types.Commands,
+            on: Optional[types.ComputationalResources] = None,
+            storage_dir: Optional[types.Path] = "",
+            extra_metadata: Optional[dict] = None,
+            **kwargs) -> tasks.Task:
+        """Run the simulation.
 
         Args:
-            input_dir: Path to the directory containing the input files.
-            commands: List of commands to run using the GROMACS simulator.
+            input_dir: Path to the directory of the simulation input files.
+            commands: List of commands to run using the OpenFAST simulator.
             on: The computational resource to launch the simulation on. If None
                 the simulation is submitted to a machine in the default pool.
-            storage_dir: Parent directory for storing simulation
-                               results.
+            other arguments: See the documentation of the base class.
         """
-
         return super().run(input_dir,
                            on=on,
                            commands=commands,
                            storage_dir=storage_dir,
-                           extra_metadata=extra_metadata)
+                           extra_metadata=extra_metadata,
+                           **kwargs)
```

### Comparing `inductiva-0.5.3/inductiva/simulators/openfoam.py` & `inductiva-0.6.0/inductiva/simulators/openfoam.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,8 +48,9 @@
         """
         return super().run(input_dir,
                            on=on,
                            commands=commands,
                            storage_dir=storage_dir,
                            n_vcpus=n_vcpus,
                            use_hwthread=use_hwthread,
-                           extra_metadata=extra_metadata)
+                           extra_metadata=extra_metadata,
+                           **kwargs)
```

### Comparing `inductiva-0.5.3/inductiva/simulators/reef3d.py` & `inductiva-0.6.0/inductiva/simulators/swash.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,45 @@
-"""Reef3D simulator module of the API."""
-
+"""SWASH module of the API."""
 from typing import Optional
 
-from inductiva import simulators, types, tasks
+from inductiva import types, tasks, simulators
 
 
 @simulators.simulator.mpi_enabled
-class REEF3D(simulators.Simulator):
-    """Class to invoke a generic FDS simulation on the API."""
+class SWASH(simulators.Simulator):
+    """Class to invoke a generic SWASH simulation on the API."""
 
     def __init__(self):
         super().__init__()
-        self.api_method_name = "reef3d.reef3d.run_simulation"
+        self.api_method_name = "sw.swash.run_simulation"
 
     def run(self,
             input_dir: types.Path,
+            sim_config_filename: str,
             n_vcpus: Optional[int] = None,
             use_hwthread: bool = True,
             on: Optional[types.ComputationalResources] = None,
             storage_dir: Optional[types.Path] = "",
             extra_metadata: Optional[dict] = None,
             **kwargs) -> tasks.Task:
         """Run the simulation.
 
         Args:
             input_dir: Path to the directory of the simulation input files.
+            sim_config_filename: Name of the simulation configuration file.
             n_vcpus: Number of vCPUs to use in the simulation. If not provided
             (default), all vCPUs will be used.
             use_hwthread: If specified Open MPI will attempt to discover the
             number of hardware threads on the node, and use that as the
             number of slots available.
-            sim_config_filename: Name of the simulation configuration file.
             on: The computational resource to launch the simulation on. If None
                 the simulation is submitted to a machine in the default pool.
-            other arguments: See the documentation of the base class.
+            storage_dir: Directory for storing simulation results.
         """
         return super().run(input_dir,
                            on=on,
+                           input_filename=sim_config_filename,
                            storage_dir=storage_dir,
                            n_vcpus=n_vcpus,
                            use_hwthread=use_hwthread,
-                           extra_metadata=extra_metadata)
+                           extra_metadata=extra_metadata,
+                           **kwargs)
```

### Comparing `inductiva-0.5.3/inductiva/simulators/schism.py` & `inductiva-0.6.0/inductiva/simulators/schism.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,16 @@
     def run(self,
             input_dir: types.Path,
             num_scribes: int = 1,
             on: Optional[types.ComputationalResources] = None,
             storage_dir: Optional[types.Path] = "",
             use_hwthread: bool = True,
             extra_metadata: Optional[dict] = None,
-            n_vcpus: int = None) -> tasks.Task:
+            n_vcpus: int = None,
+            **kwargs) -> tasks.Task:
         """Run the simulation.
         Args:
             input_dir: Path to the directory of the simulation input files.
             num_scribes: The num_scribes as per the simulator documentation.
             # pylint: disable=line-too-long
             https://schism-dev.github.io/schism/master/getting-started/running-model.html
             # pylint: enable=line-too-long
@@ -37,8 +38,9 @@
         """
         return super().run(input_dir,
                            on=on,
                            num_scribes=num_scribes,
                            storage_dir=storage_dir,
                            n_vcpus=n_vcpus,
                            use_hwthread=use_hwthread,
-                           extra_metadata=extra_metadata)
+                           extra_metadata=extra_metadata,
+                           **kwargs)
```

### Comparing `inductiva-0.5.3/inductiva/simulators/simsopt.py` & `inductiva-0.6.0/inductiva/simulators/simsopt.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         num_iterations: int,
         num_samples: int,
         sigma_scaling_factor: float,
         objectives_weights_filename: str,
         on: Optional[types.ComputationalResources] = None,
         storage_dir: Optional[types.Path] = "",
         extra_metadata: Optional[dict] = None,
+        **kwargs,
     ) -> tasks.Task:
         """Run the simulation.
 
         Args:
             coil_coefficients_filename: Name of the file with the Fourier
               Series coefficients of the coils.
             coil_currents_filename: Name of the file with the current in each
@@ -54,19 +55,20 @@
               each objective function used in the construction of the total
               objective.
             storage_dir: Directory for storing results.
             other arguments: See the documentation of the base class.
         """
         return super().run(
             input_dir,
-            on=on,
+            objectives_weights_filename=objectives_weights_filename,
             coil_coefficients_filename=coil_coefficients_filename,
-            coil_currents_filename=coil_currents_filename,
             plasma_surface_filename=plasma_surface_filename,
+            coil_currents_filename=coil_currents_filename,
+            sigma_scaling_factor=sigma_scaling_factor,
             num_field_periods=num_field_periods,
             num_iterations=num_iterations,
+            extra_metadata=extra_metadata,
             num_samples=num_samples,
-            sigma_scaling_factor=sigma_scaling_factor,
-            objectives_weights_filename=objectives_weights_filename,
             storage_dir=storage_dir,
-            extra_metadata=extra_metadata,
+            on=on,
+            **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/simulators/simulator.py` & `inductiva-0.6.0/inductiva/simulators/simulator.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/simulators/splishsplash.py` & `inductiva-0.6.0/inductiva/simulators/splishsplash.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,26 +14,28 @@
     def run(
         self,
         input_dir: types.Path,
         sim_config_filename: str,
         on: Optional[types.ComputationalResources] = None,
         storage_dir: Optional[types.Path] = "",
         extra_metadata: Optional[dict] = None,
+        **kwargs,
     ) -> tasks.Task:
         """Run the SPlisHSPlasH simulation.
 
         Args:
             input_dir: Path to the directory of the simulation input files.
             sim_config_filename: Name of the simulation configuration file.
             on: The computational resource to launch the simulation on. If None
                 the simulation is submitted to a machine in the default pool.
             storage_dir: Directory for storing simulation results.
         Returns:
             Task object representing the simulation task.
         """
         return super().run(
             input_dir,
-            on=on,
             input_filename=sim_config_filename,
-            storage_dir=storage_dir,
             extra_metadata=extra_metadata,
+            storage_dir=storage_dir,
+            on=on,
+            **kwargs,
         )
```

### Comparing `inductiva-0.5.3/inductiva/simulators/swan.py` & `inductiva-0.6.0/inductiva/simulators/swan.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         input_dir: types.Path,
         sim_config_filename: str,
         n_vcpus: Optional[int] = None,
         use_hwthread: bool = True,
         on: Optional[types.ComputationalResources] = None,
         storage_dir: Optional[types.Path] = "",
         extra_metadata: Optional[dict] = None,
+        **kwargs,
     ) -> tasks.Task:
         """Run the simulation.
 
         Args:
             input_dir: Path to the directory of the simulation input files.
             sim_config_filename: Name of the simulation configuration file.
             n_vcpus: Number of vCPUs to use in the simulation. If not provided
@@ -38,8 +39,9 @@
         """
         return super().run(input_dir,
                            on=on,
                            input_filename=sim_config_filename,
                            storage_dir=storage_dir,
                            n_vcpus=n_vcpus,
                            use_hwthread=use_hwthread,
-                           extra_metadata=extra_metadata)
+                           extra_metadata=extra_metadata,
+                           **kwargs)
```

### Comparing `inductiva-0.5.3/inductiva/simulators/swash.py` & `inductiva-0.6.0/inductiva/simulators/fds.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-"""SWASH module of the API."""
+"""FDS simulator module of the API."""
+
 from typing import Optional
 
 from inductiva import types, tasks, simulators
+from inductiva.utils import meta
 
 
-@simulators.simulator.mpi_enabled
-class SWASH(simulators.Simulator):
-    """Class to invoke a generic SWASH simulation on the API."""
+class FDS(simulators.Simulator):
+    """Class to invoke a generic FDS simulation on the API."""
 
     def __init__(self):
         super().__init__()
-        self.api_method_name = "sw.swash.run_simulation"
+        self.api_method_name = "fdm.fds.run_simulation"
 
+    @meta.deprecated_arg(n_cores="n_vcpus")
     def run(self,
             input_dir: types.Path,
             sim_config_filename: str,
             n_vcpus: Optional[int] = None,
             use_hwthread: bool = True,
+            post_processing_filename: str = None,
             on: Optional[types.ComputationalResources] = None,
             storage_dir: Optional[types.Path] = "",
             extra_metadata: Optional[dict] = None,
             **kwargs) -> tasks.Task:
         """Run the simulation.
 
         Args:
@@ -29,16 +32,18 @@
             n_vcpus: Number of vCPUs to use in the simulation. If not provided
             (default), all vCPUs will be used.
             use_hwthread: If specified Open MPI will attempt to discover the
             number of hardware threads on the node, and use that as the
             number of slots available.
             on: The computational resource to launch the simulation on. If None
                 the simulation is submitted to a machine in the default pool.
-            storage_dir: Directory for storing simulation results.
+            other arguments: See the documentation of the base class.
         """
         return super().run(input_dir,
                            on=on,
                            input_filename=sim_config_filename,
+                           post_processing_config=post_processing_filename,
                            storage_dir=storage_dir,
                            n_vcpus=n_vcpus,
                            use_hwthread=use_hwthread,
-                           extra_metadata=extra_metadata)
+                           extra_metadata=extra_metadata,
+                           **kwargs)
```

### Comparing `inductiva-0.5.3/inductiva/simulators/xbeach.py` & `inductiva-0.6.0/inductiva/simulators/xbeach.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,8 +38,9 @@
         """
         return super().run(input_dir,
                            input_filename=sim_config_filename,
                            on=on,
                            storage_dir=storage_dir,
                            n_vcpus=n_vcpus,
                            use_hwthread=use_hwthread,
-                           extra_metadata=extra_metadata)
+                           extra_metadata=extra_metadata,
+                           **kwargs)
```

### Comparing `inductiva-0.5.3/inductiva/storage/storage.py` & `inductiva-0.6.0/inductiva/storage/storage.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/tasks/methods.py` & `inductiva-0.6.0/inductiva/tasks/methods.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/tasks/run_simulation.py` & `inductiva-0.6.0/inductiva/tasks/run_simulation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """Functions for running simulations via Inductiva Web API."""
 import os
 
 import pathlib
-from typing import Any, Optional
+from typing import Any, Optional, Union
 import json
 import threading
 
 from absl import logging
 
 from inductiva import tasks, types
 from inductiva.api import methods
 from inductiva.utils import format_utils, files
+from inductiva.resources.machine_types import ProviderType
 
 TASK_METADATA_FILENAME = "task_metadata.json"
 
 _metadata_lock = threading.RLock()
 
 
 def run_simulation(
     api_method_name: str,
     input_dir: pathlib.Path,
     computational_resources: Optional[types.ComputationalResources] = None,
+    provider_id: Optional[Union[ProviderType, str]] = ProviderType.GCP,
     storage_dir: Optional[types.Path] = "",
     api_invoker=None,
     extra_metadata=None,
     **kwargs: Any,
 ) -> tasks.Task:
     """Run a simulation via Inductiva Web API."""
 
@@ -35,21 +37,23 @@
     type_annotations = {
         "sim_dir": pathlib.Path,
     }
 
     if api_invoker is None:
         api_invoker = methods.invoke_async_api
 
-    task_id = api_invoker(
-        api_method_name,
-        params,
-        type_annotations,
-        resource_pool=computational_resources,
-        storage_path_prefix=storage_dir,
-    )
+    if provider_id is not None:
+        provider_id = ProviderType(provider_id)
+
+    task_id = api_invoker(api_method_name,
+                          params,
+                          type_annotations,
+                          resource_pool=computational_resources,
+                          storage_path_prefix=storage_dir,
+                          provider_id=provider_id)
 
     if computational_resources is not None:
         logging.info("Task %s submitted to the queue of the %s.", task_id,
                      computational_resources)
     else:
         logging.info("Task %s submitted to the default queue.", task_id)
```

### Comparing `inductiva-0.5.3/inductiva/tasks/streams.py` & `inductiva-0.6.0/inductiva/tasks/streams.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/tasks/task.py` & `inductiva-0.6.0/inductiva/tasks/task.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/templating/manager.py` & `inductiva-0.6.0/inductiva/templating/manager.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/templating/renderers.py` & `inductiva-0.6.0/inductiva/templating/renderers.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/types.py` & `inductiva-0.6.0/inductiva/types.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/utils/data.py` & `inductiva-0.6.0/inductiva/utils/data.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/utils/file_manager.py` & `inductiva-0.6.0/inductiva/utils/file_manager.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/utils/files.py` & `inductiva-0.6.0/inductiva/utils/files.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/utils/format_utils.py` & `inductiva-0.6.0/inductiva/utils/format_utils.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/utils/input_functions.py` & `inductiva-0.6.0/inductiva/utils/input_functions.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/utils/meta.py` & `inductiva-0.6.0/inductiva/utils/meta.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/utils/output_contents.py` & `inductiva-0.6.0/inductiva/utils/output_contents.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva/utils/scheduler.py` & `inductiva-0.6.0/inductiva/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `inductiva-0.5.3/inductiva.egg-info/PKG-INFO` & `inductiva-0.6.0/inductiva.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inductiva
-Version: 0.5.3
+Version: 0.6.0
 Summary: Python client for the Inductiva API
 Home-page: https://github.com/inductiva/inductiva
 Author: Inductiva Research Labs
 Author-email: contact@inductiva.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -22,15 +22,15 @@
 Requires-Dist: tqdm
 Requires-Dist: websocket-client
 Requires-Dist: pyyaml
 
 
 [![Python package](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml/badge.svg)](https://github.com/inductiva/inductiva/actions/workflows/python-package.yml) [![Python version](https://img.shields.io/pypi/pyversions/inductiva.svg)](https://www.python.org/downloads/) [![Documentation](https://img.shields.io/badge/Documentation-blue.svg)](https://docs.inductiva.ai/en/latest/) [![Benchmarks](https://img.shields.io/badge/Benchmarks-blue.svg)](https://benchmarks.inductiva.ai) <a href="https://pypi.org/project/inductiva/"><img src="https://img.shields.io/pypi/v/inductiva" alt="pypi version"></a> ![coverage badge](https://raw.githubusercontent.com/inductiva/inductiva/Inductiva-badges/badges/cov.svg)
 
-![linkedin_header](https://user-images.githubusercontent.com/104431973/231184851-0ce34289-593e-4832-aaa2-9aae652113f5.jpg)
+![inductiva_banner](https://github.com/inductiva/inductiva/assets/7538022/85569dd8-3beb-4ac3-8cbe-78e300a28fde)
 
 # Inductiva: a Python package for scaling simulations on the Cloud
 
 Welcome to the official Python library for the Inductiva API version **0.5**. 
 The Inductiva API allows running a set of open-source physical
 simulators on the cloud, easily parallelizing simulations, each running
 on hundreds of CPU cores.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inductiva Version: 0.5.3 Summary: Python client for
+Metadata-Version: 2.1 Name: inductiva Version: 0.6.0 Summary: Python client for
 the Inductiva API Home-page: https://github.com/inductiva/inductiva Author:
 Inductiva Research Labs Author-email: contact@inductiva.ai Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: certifi>=14.5.14 Requires-Dist:
 frozendict~=2.3.4 Requires-Dist: setuptools>=21.0.0 Requires-Dist: typing-
 extensions~=4.3.0 Requires-Dist: urllib3~=1.26.7 Requires-Dist: python-dateutil
@@ -12,22 +12,21 @@
 package.yml/badge.svg)](https://github.com/inductiva/inductiva/actions/
 workflows/python-package.yml) [![Python version](https://img.shields.io/pypi/
 pyversions/inductiva.svg)](https://www.python.org/downloads/) [![Documentation]
 (https://img.shields.io/badge/Documentation-blue.svg)](https://
 docs.inductiva.ai/en/latest/) [![Benchmarks](https://img.shields.io/badge/
 Benchmarks-blue.svg)](https://benchmarks.inductiva.ai) _[_p_y_p_i_ _v_e_r_s_i_o_n_]![coverage
 badge](https://raw.githubusercontent.com/inductiva/inductiva/Inductiva-badges/
-badges/cov.svg) ![linkedin_header](https://user-images.githubusercontent.com/
-104431973/231184851-0ce34289-593e-4832-aaa2-9aae652113f5.jpg) # Inductiva: a
-Python package for scaling simulations on the Cloud Welcome to the official
-Python library for the Inductiva API version **0.5**. The Inductiva API allows
-running a set of open-source physical simulators on the cloud, easily
-parallelizing simulations, each running on hundreds of CPU cores. Inductiva
-simplifies the complexities of cloud resource management, and software
-configuration, offering a straightforward Python interface for running
-simulations on state-of-the-art hardware. This allows scientists and engineers
-to focus their time and energy on what matters: running simulations that solve
-real problems. To find out more, check our [documentation](https://
-docs.inductiva.ai/). If you have any questions or suggestions about the API
-please [open an issue on the inductivaâs API Client GitHub repo](https://
-github.com/inductiva/inductiva/issues), or contact us via
-[support@inductiva.ai](mailto:support@inductiva.ai).
+badges/cov.svg) ![inductiva_banner](https://github.com/inductiva/inductiva/
+assets/7538022/85569dd8-3beb-4ac3-8cbe-78e300a28fde) # Inductiva: a Python
+package for scaling simulations on the Cloud Welcome to the official Python
+library for the Inductiva API version **0.5**. The Inductiva API allows running
+a set of open-source physical simulators on the cloud, easily parallelizing
+simulations, each running on hundreds of CPU cores. Inductiva simplifies the
+complexities of cloud resource management, and software configuration, offering
+a straightforward Python interface for running simulations on state-of-the-art
+hardware. This allows scientists and engineers to focus their time and energy
+on what matters: running simulations that solve real problems. To find out
+more, check our [documentation](https://docs.inductiva.ai/). If you have any
+questions or suggestions about the API please [open an issue on the
+inductivaâs API Client GitHub repo](https://github.com/inductiva/inductiva/
+issues), or contact us via [support@inductiva.ai](mailto:support@inductiva.ai).
```

### Comparing `inductiva-0.5.3/inductiva.egg-info/SOURCES.txt` & `inductiva-0.6.0/inductiva.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 inductiva/_cli/loader.py
 inductiva/_cli/main.py
 inductiva/_cli/utils.py
 inductiva/_cli/cmd_autocomplete/__init__.py
 inductiva/_cli/cmd_autocomplete/enable.py
 inductiva/_cli/cmd_logs/__init__.py
 inductiva/_cli/cmd_logs/logs.py
+inductiva/_cli/cmd_quotas/__init__.py
+inductiva/_cli/cmd_quotas/list.py
 inductiva/_cli/cmd_resources/__init__.py
 inductiva/_cli/cmd_resources/_start.py
 inductiva/_cli/cmd_resources/cost.py
 inductiva/_cli/cmd_resources/list.py
 inductiva/_cli/cmd_resources/terminate.py
 inductiva/_cli/cmd_storage/__init__.py
 inductiva/_cli/cmd_storage/list.py
@@ -55,65 +57,81 @@
 inductiva/client/apis/paths/compute_group_name.py
 inductiva/client/apis/paths/compute_group_start.py
 inductiva/client/apis/paths/compute_group_status.py
 inductiva/client/apis/paths/compute_groups.py
 inductiva/client/apis/paths/compute_machine_types.py
 inductiva/client/apis/paths/compute_price.py
 inductiva/client/apis/paths/compute_type.py
+inductiva/client/apis/paths/projects.py
+inductiva/client/apis/paths/projects_name.py
 inductiva/client/apis/paths/storage_contents.py
 inductiva/client/apis/paths/storage_size.py
 inductiva/client/apis/paths/tasks.py
 inductiva/client/apis/paths/tasks_auth.py
 inductiva/client/apis/paths/tasks_submit.py
 inductiva/client/apis/paths/tasks_task_id.py
+inductiva/client/apis/paths/tasks_task_id_disable_logs.py
 inductiva/client/apis/paths/tasks_task_id_input.py
+inductiva/client/apis/paths/tasks_task_id_input_upload_url.py
+inductiva/client/apis/paths/tasks_task_id_input_uploaded.py
 inductiva/client/apis/paths/tasks_task_id_kill.py
 inductiva/client/apis/paths/tasks_task_id_output.py
 inductiva/client/apis/paths/tasks_task_id_output_list.py
 inductiva/client/apis/paths/tasks_task_id_status.py
+inductiva/client/apis/paths/users_quotas.py
 inductiva/client/apis/paths/version.py
 inductiva/client/apis/paths/version_check.py
 inductiva/client/apis/tags/__init__.py
 inductiva/client/apis/tags/compute_api.py
+inductiva/client/apis/tags/projects_api.py
 inductiva/client/apis/tags/storage_api.py
 inductiva/client/apis/tags/tasks_api.py
+inductiva/client/apis/tags/users_api.py
 inductiva/client/apis/tags/version_api.py
 inductiva/client/model/__init__.py
+inductiva/client/model/autoscale_policy.py
+inductiva/client/model/autoscale_policy.pyi
 inductiva/client/model/backend_version.py
 inductiva/client/model/backend_version.pyi
-inductiva/client/model/base_machine_type.py
-inductiva/client/model/base_machine_type.pyi
 inductiva/client/model/base_vm_group.py
 inductiva/client/model/base_vm_group.pyi
-inductiva/client/model/body_upload_task_input.py
-inductiva/client/model/body_upload_task_input.pyi
 inductiva/client/model/default_machine_group.py
 inductiva/client/model/default_machine_group.pyi
 inductiva/client/model/executer.py
 inductiva/client/model/executer.pyi
 inductiva/client/model/executer_tracker_api_connection_info.py
 inductiva/client/model/executer_tracker_api_connection_info.pyi
 inductiva/client/model/executer_tracker_register_info.py
 inductiva/client/model/executer_tracker_register_info.pyi
 inductiva/client/model/file_info.py
 inductiva/client/model/file_info.pyi
 inductiva/client/model/http_validation_error.py
 inductiva/client/model/http_validation_error.pyi
+inductiva/client/model/machine_group_type.py
+inductiva/client/model/machine_group_type.pyi
 inductiva/client/model/machine_type.py
 inductiva/client/model/machine_type.pyi
 inductiva/client/model/output_archive_info.py
 inductiva/client/model/output_archive_info.pyi
+inductiva/client/model/project.py
+inductiva/client/model/project.pyi
+inductiva/client/model/project_create.py
+inductiva/client/model/project_create.pyi
 inductiva/client/model/provider.py
 inductiva/client/model/provider.pyi
 inductiva/client/model/providers.py
 inductiva/client/model/providers.pyi
 inductiva/client/model/quota.py
 inductiva/client/model/quota.pyi
+inductiva/client/model/storage_file_info.py
+inductiva/client/model/storage_file_info.pyi
 inductiva/client/model/task.py
 inductiva/client/model/task.pyi
+inductiva/client/model/task_input_upload_url.py
+inductiva/client/model/task_input_upload_url.pyi
 inductiva/client/model/task_request.py
 inductiva/client/model/task_request.pyi
 inductiva/client/model/task_status.py
 inductiva/client/model/task_status.pyi
 inductiva/client/model/task_status_code.py
 inductiva/client/model/task_status_code.pyi
 inductiva/client/model/user.py
@@ -160,14 +178,22 @@
 inductiva/client/paths/compute_machine_types/get.pyi
 inductiva/client/paths/compute_price/__init__.py
 inductiva/client/paths/compute_price/get.py
 inductiva/client/paths/compute_price/get.pyi
 inductiva/client/paths/compute_type/__init__.py
 inductiva/client/paths/compute_type/get.py
 inductiva/client/paths/compute_type/get.pyi
+inductiva/client/paths/projects/__init__.py
+inductiva/client/paths/projects/get.py
+inductiva/client/paths/projects/get.pyi
+inductiva/client/paths/projects/post.py
+inductiva/client/paths/projects/post.pyi
+inductiva/client/paths/projects_name/__init__.py
+inductiva/client/paths/projects_name/get.py
+inductiva/client/paths/projects_name/get.pyi
 inductiva/client/paths/storage_contents/__init__.py
 inductiva/client/paths/storage_contents/delete.py
 inductiva/client/paths/storage_contents/delete.pyi
 inductiva/client/paths/storage_contents/get.py
 inductiva/client/paths/storage_contents/get.pyi
 inductiva/client/paths/storage_size/__init__.py
 inductiva/client/paths/storage_size/get.py
@@ -180,29 +206,41 @@
 inductiva/client/paths/tasks_auth/get.pyi
 inductiva/client/paths/tasks_submit/__init__.py
 inductiva/client/paths/tasks_submit/post.py
 inductiva/client/paths/tasks_submit/post.pyi
 inductiva/client/paths/tasks_task_id/__init__.py
 inductiva/client/paths/tasks_task_id/get.py
 inductiva/client/paths/tasks_task_id/get.pyi
+inductiva/client/paths/tasks_task_id_disable_logs/__init__.py
+inductiva/client/paths/tasks_task_id_disable_logs/post.py
+inductiva/client/paths/tasks_task_id_disable_logs/post.pyi
 inductiva/client/paths/tasks_task_id_input/__init__.py
-inductiva/client/paths/tasks_task_id_input/post.py
-inductiva/client/paths/tasks_task_id_input/post.pyi
+inductiva/client/paths/tasks_task_id_input/put.py
+inductiva/client/paths/tasks_task_id_input/put.pyi
+inductiva/client/paths/tasks_task_id_input_upload_url/__init__.py
+inductiva/client/paths/tasks_task_id_input_upload_url/get.py
+inductiva/client/paths/tasks_task_id_input_upload_url/get.pyi
+inductiva/client/paths/tasks_task_id_input_uploaded/__init__.py
+inductiva/client/paths/tasks_task_id_input_uploaded/post.py
+inductiva/client/paths/tasks_task_id_input_uploaded/post.pyi
 inductiva/client/paths/tasks_task_id_kill/__init__.py
 inductiva/client/paths/tasks_task_id_kill/post.py
 inductiva/client/paths/tasks_task_id_kill/post.pyi
 inductiva/client/paths/tasks_task_id_output/__init__.py
 inductiva/client/paths/tasks_task_id_output/get.py
 inductiva/client/paths/tasks_task_id_output/get.pyi
 inductiva/client/paths/tasks_task_id_output_list/__init__.py
 inductiva/client/paths/tasks_task_id_output_list/get.py
 inductiva/client/paths/tasks_task_id_output_list/get.pyi
 inductiva/client/paths/tasks_task_id_status/__init__.py
 inductiva/client/paths/tasks_task_id_status/get.py
 inductiva/client/paths/tasks_task_id_status/get.pyi
+inductiva/client/paths/users_quotas/__init__.py
+inductiva/client/paths/users_quotas/get.py
+inductiva/client/paths/users_quotas/get.pyi
 inductiva/client/paths/version/__init__.py
 inductiva/client/paths/version/get.py
 inductiva/client/paths/version/get.pyi
 inductiva/client/paths/version_check/__init__.py
 inductiva/client/paths/version_check/get.py
 inductiva/client/paths/version_check/get.pyi
 inductiva/commands/__init__.py
@@ -216,19 +254,22 @@
 inductiva/resources/__init__.py
 inductiva/resources/machine_cluster.py
 inductiva/resources/machine_groups.py
 inductiva/resources/machine_types.py
 inductiva/resources/machines.py
 inductiva/resources/machines_base.py
 inductiva/simulators/__init__.py
+inductiva/simulators/amr_wind.py
+inductiva/simulators/cans.py
 inductiva/simulators/dualsphysics.py
 inductiva/simulators/dummy_simulator.py
 inductiva/simulators/fds.py
 inductiva/simulators/fenicsx.py
 inductiva/simulators/gromacs.py
+inductiva/simulators/openfast.py
 inductiva/simulators/openfoam.py
 inductiva/simulators/reef3d.py
 inductiva/simulators/schism.py
 inductiva/simulators/simsopt.py
 inductiva/simulators/simulator.py
 inductiva/simulators/splishsplash.py
 inductiva/simulators/swan.py
@@ -244,16 +285,21 @@
 inductiva/templating/__init__.py
 inductiva/templating/manager.py
 inductiva/templating/renderers.py
 inductiva/tests/templating/assets/template.txt.jinja
 inductiva/tests/templating/assets/folder/nested_template.txt.jinja
 inductiva/tests/utils/assets/template.yaml.jinja
 inductiva/tests/utils/assets/template_file.txt.jinja
+inductiva/users/__init__.py
+inductiva/users/methods.py
 inductiva/utils/__init__.py
 inductiva/utils/data.py
 inductiva/utils/file_manager.py
 inductiva/utils/files.py
 inductiva/utils/format_utils.py
 inductiva/utils/input_functions.py
 inductiva/utils/meta.py
 inductiva/utils/output_contents.py
-inductiva/utils/scheduler.py
+inductiva/utils/scheduler.py
+tutorials/__init__.py
+tutorials/conf.py
+tutorials/conftest.py
```

### Comparing `inductiva-0.5.3/setup.cfg` & `inductiva-0.6.0/setup.cfg`

 * *Files identical despite different names*

