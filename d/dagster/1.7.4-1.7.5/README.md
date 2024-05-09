# Comparing `tmp/dagster-1.7.4.tar.gz` & `tmp/dagster-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.7.4.tar", last modified: Thu May  2 20:32:09 2024, max compression
+gzip compressed data, was "dagster-1.7.5.tar", last modified: Thu May  9 17:47:59 2024, max compression
```

## Comparing `dagster-1.7.4.tar` & `dagster-1.7.5.tar`

### file list

```diff
@@ -1,695 +1,714 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.169218 dagster-1.7.4/
--rw-r--r--   0 root         (0) root         (0)      553 2024-05-02 20:31:40.000000 dagster-1.7.4/COPYING
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-02 20:31:40.000000 dagster-1.7.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      533 2024-05-02 20:31:40.000000 dagster-1.7.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9867 2024-05-02 20:32:09.169218 dagster-1.7.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8153 2024-05-02 20:31:40.000000 dagster-1.7.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.049219 dagster-1.7.4/dagster/
--rw-r--r--   0 root         (0) root         (0)    29976 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)    20744 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.053219 dagster-1.7.4/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     3224 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5483 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3370 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.053219 dagster-1.7.4/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    52040 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.053219 dagster-1.7.4/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26898 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8030 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     8302 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3513 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     8134 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     6651 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    30542 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     9114 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5120 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19351 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15461 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4259 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.057219 dagster-1.7.4/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27910 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.057219 dagster-1.7.4/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15830 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18787 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    14918 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    19728 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9536 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.061219 dagster-1.7.4/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)     1394 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)    18114 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/config.py
--rw-r--r--   0 root         (0) root         (0)    11510 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    11583 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    41265 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/resource.py
--rw-r--r--   0 root         (0) root         (0)     1996 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/type_check_utils.py
--rw-r--r--   0 root         (0) root         (0)     8375 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)    12532 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3087 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17137 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.061219 dagster-1.7.4/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.065219 dagster-1.7.4/dagster/_core/asset_graph_view/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/asset_graph_view/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21047 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/asset_graph_view/asset_graph_view.py
--rw-r--r--   0 root         (0) root         (0)      994 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13427 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.065219 dagster-1.7.4/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     9665 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.081218 dagster-1.7.4/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7827 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4506 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_check_evaluation.py
--rw-r--r--   0 root         (0) root         (0)     7090 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_check_result.py
--rw-r--r--   0 root         (0) root         (0)     5628 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_check_spec.py
--rw-r--r--   0 root         (0) root         (0)     6113 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_checks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.081218 dagster-1.7.4/dagster/_core/definitions/asset_condition/
--rw-r--r--   0 root         (0) root         (0)       62 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_condition/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21109 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_condition/asset_condition.py
--rw-r--r--   0 root         (0) root         (0)    16731 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py
--rw-r--r--   0 root         (0) root         (0)    26314 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_daemon_context.py
--rw-r--r--   0 root         (0) root         (0)    10654 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_dep.py
--rw-r--r--   0 root         (0) root         (0)    10133 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     7696 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_graph_differ.py
--rw-r--r--   0 root         (0) root         (0)    16636 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3644 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    30136 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_job.py
--rw-r--r--   0 root         (0) root         (0)     6060 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_key.py
--rw-r--r--   0 root         (0) root         (0)    30355 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     6945 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    39535 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7444 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     6764 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_spec.py
--rw-r--r--   0 root         (0) root         (0)    10723 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/asset_subset.py
--rw-r--r--   0 root         (0) root         (0)    80227 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    13758 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    11477 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/auto_materialize_rule.py
--rw-r--r--   0 root         (0) root         (0)    21722 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/auto_materialize_rule_evaluation.py
--rw-r--r--   0 root         (0) root         (0)    46525 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/auto_materialize_rule_impls.py
--rw-r--r--   0 root         (0) root         (0)     2768 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/auto_materialize_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/backfill_policy.py
--rw-r--r--   0 root         (0) root         (0)    34599 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/base_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    16772 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    40623 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4278 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    14811 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    22990 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    30155 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.085218 dagster-1.7.4/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16572 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/asset_check_decorator.py
--rw-r--r--   0 root         (0) root         (0)    70075 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4907 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9077 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9353 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10815 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    19011 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    15668 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8718 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12463 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12664 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5267 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    23545 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    42243 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    26888 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21182 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)     9379 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/external_asset.py
--rw-r--r--   0 root         (0) root         (0)     9766 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_based_auto_materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.085218 dagster-1.7.4/dagster/_core/definitions/freshness_checks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5838 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_checks/last_update.py
--rw-r--r--   0 root         (0) root         (0)     7685 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_checks/sensor.py
--rw-r--r--   0 root         (0) root         (0)     9349 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_checks/shared_builder.py
--rw-r--r--   0 root         (0) root         (0)     4669 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_checks/time_partition.py
--rw-r--r--   0 root         (0) root         (0)    10454 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_checks/utils.py
--rw-r--r--   0 root         (0) root         (0)     8801 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16401 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    47569 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    21027 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     6410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    53689 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)     5693 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/load_asset_checks_from_modules.py
--rw-r--r--   0 root         (0) root         (0)    22306 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7171 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.085218 dagster-1.7.4/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    42277 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    57203 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    22029 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)      197 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11892 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8016 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2892 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    23078 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    23141 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7551 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    19237 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    50520 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47665 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    11087 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27733 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/reconstruct.py
--rw-r--r--   0 root         (0) root         (0)    21602 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/remote_asset_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.085218 dagster-1.7.4/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6024 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    21698 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    20892 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     8858 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1465 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    17900 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5382 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)    10320 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)     3383 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/result.py
--rw-r--r--   0 root         (0) root         (0)    23076 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    19555 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    44126 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    39363 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     6209 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/schema_change_checks.py
--rw-r--r--   0 root         (0) root         (0)     5134 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    14134 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    53797 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    19244 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)    22389 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)   102377 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15160 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)    11017 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3982 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    26986 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)    17452 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.085218 dagster-1.7.4/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    71913 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8142 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.093218 dagster-1.7.4/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38363 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    64654 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    17100 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6296 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.093218 dagster-1.7.4/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79687 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)     8657 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/data_version_cache.py
--rw-r--r--   0 root         (0) root         (0)    17598 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    29167 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    40124 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    37256 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    49252 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18837 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5135 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5897 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9633 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8602 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14247 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6723 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.097218 dagster-1.7.4/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26460 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     9850 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    17019 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16974 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    40707 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    11032 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    39260 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6251 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/instance_concurrency_context.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5706 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7326 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    61075 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    17174 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15985 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8230 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19141 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2100 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)     9950 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)    14043 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/submit_asset_runs.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.097218 dagster-1.7.4/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5989 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     3366 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15497 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.097218 dagster-1.7.4/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16894 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.097218 dagster-1.7.4/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.101218 dagster-1.7.4/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   132334 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15788 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24141 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     3899 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.101218 dagster-1.7.4/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3819 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6645 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1566 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    18041 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     6656 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/op_concurrency_limits_counter.py
--rw-r--r--   0 root         (0) root         (0)     3691 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.101218 dagster-1.7.4/dagster/_core/pipes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8974 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/pipes/client.py
--rw-r--r--   0 root         (0) root         (0)    18318 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/pipes/context.py
--rw-r--r--   0 root         (0) root         (0)     5648 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/pipes/subprocess.py
--rw-r--r--   0 root         (0) root         (0)    25661 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/pipes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.105218 dagster-1.7.4/dagster/_core/remote_representation/
--rw-r--r--   0 root         (0) root         (0)     2793 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36695 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    37482 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    83582 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/feature_flags.py
--rw-r--r--   0 root         (0) root         (0)    12429 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4356 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19669 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/remote_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.105218 dagster-1.7.4/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    13364 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.105218 dagster-1.7.4/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    28809 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)    10917 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.105218 dagster-1.7.4/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1801 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.105218 dagster-1.7.4/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18109 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.109218 dagster-1.7.4/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2842 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9302 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12155 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16934 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14185 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     3183 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.113218 dagster-1.7.4/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3058 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.113218 dagster-1.7.4/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6686 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.129218 dagster-1.7.4/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      312 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1486 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      599 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      635 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      958 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      499 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)     2359 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
--rw-r--r--   0 root         (0) root         (0)     1322 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3887 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/asset_check_execution_record.py
--rw-r--r--   0 root         (0) root         (0)     7301 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.129218 dagster-1.7.4/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8725 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16223 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9557 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    25652 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11187 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.129218 dagster-1.7.4/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19078 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3801 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7289 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     8037 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     9250 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)   121159 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.129218 dagster-1.7.4/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7508 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    22497 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10983 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13492 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8819 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10882 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    32629 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17558 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1167 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4355 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/migration/bigint_migration.py
--rw-r--r--   0 root         (0) root         (0)    15491 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3270 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    17398 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13903 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2452 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8716 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     6391 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    37611 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6310 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7236 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4133 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     4086 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    25146 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3684 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7691 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/sqlalchemy_compat.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4875 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1186 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    19138 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.133218 dagster-1.7.4/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13962 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15178 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    29921 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    22361 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.137218 dagster-1.7.4/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7042 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    36504 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3571 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4764 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3620 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     6652 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.137218 dagster-1.7.4/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3160 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/batch_asset_record_loader.py
--rw-r--r--   0 root         (0) root         (0)     3422 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    29210 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11852 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4721 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     3463 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1971 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)    42160 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7402 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9036 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     2665 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     5118 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19590 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    12497 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      320 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/monitoring/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     9904 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/monitoring/run_monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18725 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    39411 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/utils.py
--rw-r--r--   0 root         (0) root         (0)     4114 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2997 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.045219 dagster-1.7.4/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.141218 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      297 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.145218 dagster-1.7.4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.145218 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.145218 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.145218 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.145218 dagster-1.7.4/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.149218 dagster-1.7.4/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27262 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/__generated__/api_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    43164 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    22739 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3584 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    23173 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.149218 dagster-1.7.4/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5993 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    13431 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    60914 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5297 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    29291 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     3693 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.149218 dagster-1.7.4/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      180 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.149218 dagster-1.7.4/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_loggers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.149218 dagster-1.7.4/dagster/_model/
--rw-r--r--   0 root         (0) root         (0)     1491 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_model/pydantic_compat_layer.py
--rw-r--r--   0 root         (0) root         (0)     3269 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.149218 dagster-1.7.4/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42035 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1262 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.153218 dagster-1.7.4/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      701 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8916 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7292 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    43131 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.153218 dagster-1.7.4/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5455 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.153218 dagster-1.7.4/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.169218 dagster-1.7.4/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    26539 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9314 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     5536 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    42955 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     5865 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/concurrency.py
--rw-r--r--   0 root         (0) root         (0)    12887 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/container.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/env.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      745 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)    11214 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    33445 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/security.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.169218 dagster-1.7.4/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    13678 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7790 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/data_versions.py
--rw-r--r--   0 root         (0) root         (0)      119 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    36138 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.169218 dagster-1.7.4/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/typed_dict.py
--rw-r--r--   0 root         (0) root         (0)      170 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4740 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/warnings.py
--rw-r--r--   0 root         (0) root         (0)     4902 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-02 20:31:40.000000 dagster-1.7.4/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:32:09.049219 dagster-1.7.4/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9867 2024-05-02 20:32:08.000000 dagster-1.7.4/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    28135 2024-05-02 20:32:08.000000 dagster-1.7.4/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:32:08.000000 dagster-1.7.4/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2024-05-02 20:32:08.000000 dagster-1.7.4/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1467 2024-05-02 20:32:08.000000 dagster-1.7.4/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-02 20:32:08.000000 dagster-1.7.4/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2024-05-02 20:32:09.173218 dagster-1.7.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6847 2024-05-02 20:31:40.000000 dagster-1.7.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.447741 dagster-1.7.5/
+-rw-r--r--   0 root         (0) root         (0)      553 2024-05-09 17:47:35.000000 dagster-1.7.5/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-09 17:47:35.000000 dagster-1.7.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      533 2024-05-09 17:47:35.000000 dagster-1.7.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8928 2024-05-09 17:47:59.447741 dagster-1.7.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7214 2024-05-09 17:47:35.000000 dagster-1.7.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.367741 dagster-1.7.5/dagster/
+-rw-r--r--   0 root         (0) root         (0)    30128 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    20744 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.371741 dagster-1.7.5/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.371741 dagster-1.7.5/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    52040 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.371741 dagster-1.7.5/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26898 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8271 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     8302 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    30542 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     9114 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5120 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19351 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.371741 dagster-1.7.5/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27910 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.375741 dagster-1.7.5/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15830 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18787 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    14918 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    19728 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9536 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.375741 dagster-1.7.5/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)     1394 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)    18114 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/config.py
+-rw-r--r--   0 root         (0) root         (0)    11510 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    11583 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    41265 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/type_check_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8375 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17137 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.379741 dagster-1.7.5/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.379741 dagster-1.7.5/dagster/_core/asset_graph_view/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/asset_graph_view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22976 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/asset_graph_view/asset_graph_view.py
+-rw-r--r--   0 root         (0) root         (0)      994 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13427 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.379741 dagster-1.7.5/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     9665 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.391741 dagster-1.7.5/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7873 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_evaluation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.391741 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.391741 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12253 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py
+-rw-r--r--   0 root         (0) root         (0)     7692 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     9763 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py
+-rw-r--r--   0 root         (0) root         (0)     6122 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/schema_change_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11378 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/utils.py
+-rw-r--r--   0 root         (0) root         (0)     7090 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_result.py
+-rw-r--r--   0 root         (0) root         (0)     5628 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_spec.py
+-rw-r--r--   0 root         (0) root         (0)     6113 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)    28490 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_daemon_context.py
+-rw-r--r--   0 root         (0) root         (0)    10831 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_dep.py
+-rw-r--r--   0 root         (0) root         (0)    10133 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     7696 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_graph_differ.py
+-rw-r--r--   0 root         (0) root         (0)    16636 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    30136 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_job.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)    30355 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     6937 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    39535 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7444 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6756 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_spec.py
+-rw-r--r--   0 root         (0) root         (0)    10965 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_subset.py
+-rw-r--r--   0 root         (0) root         (0)    79051 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13969 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/auto_materialize_rule.py
+-rw-r--r--   0 root         (0) root         (0)    21722 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/auto_materialize_rule_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)    50726 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/auto_materialize_rule_impls.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/auto_materialize_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/backfill_policy.py
+-rw-r--r--   0 root         (0) root         (0)    34599 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/base_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    16772 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    40623 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4278 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    22990 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    30236 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.395741 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/README.md
+-rw-r--r--   0 root         (0) root         (0)      956 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.395741 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py
+-rw-r--r--   0 root         (0) root         (0)    16841 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.395741 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operands/
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.395741 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operators/
+-rw-r--r--   0 root         (0) root         (0)      280 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py
+-rw-r--r--   0 root         (0) root         (0)     3592 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py
+-rw-r--r--   0 root         (0) root         (0)     7206 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/scheduling_condition.py
+-rw-r--r--   0 root         (0) root         (0)     6430 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/scheduling_context.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py
+-rw-r--r--   0 root         (0) root         (0)    10067 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/serialized_objects.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.395741 dagster-1.7.5/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16572 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/asset_check_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    70075 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9077 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9353 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10815 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    19011 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    15668 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8718 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12656 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    23545 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    42243 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    27649 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21182 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9379 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/external_asset.py
+-rw-r--r--   0 root         (0) root         (0)     9808 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/freshness_based_auto_materialize.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16401 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    47569 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    21027 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    53689 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5693 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/load_asset_checks_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)    22306 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.395741 dagster-1.7.5/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)     9602 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5591 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/metadata/metadata_set.py
+-rw-r--r--   0 root         (0) root         (0)    31381 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/metadata/metadata_value.py
+-rw-r--r--   0 root         (0) root         (0)    12452 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    57203 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    22029 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8016 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    23078 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    23141 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7551 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    19237 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    50520 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47665 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    11087 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27690 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/reconstruct.py
+-rw-r--r--   0 root         (0) root         (0)    21602 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/remote_asset_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.399741 dagster-1.7.5/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    21698 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    20892 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     8858 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    17900 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    10320 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/result.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    19555 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    45639 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    39363 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    14134 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    53797 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19236 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)    22389 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)   102377 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    15160 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    11027 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    26986 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    17452 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.399741 dagster-1.7.5/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    71913 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.403741 dagster-1.7.5/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38363 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    65474 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    17100 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.403741 dagster-1.7.5/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79687 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)     8657 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/data_version_cache.py
+-rw-r--r--   0 root         (0) root         (0)    17598 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    29167 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    40124 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    37256 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    49252 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18837 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14247 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.407741 dagster-1.7.5/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26460 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    17062 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16974 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    40877 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    11032 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    39260 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/instance_concurrency_context.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    61075 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    17174 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15985 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8230 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19141 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)     9950 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)    15211 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/submit_asset_runs.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.407741 dagster-1.7.5/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15497 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.407741 dagster-1.7.5/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16894 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.407741 dagster-1.7.5/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   132334 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15788 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24141 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    18041 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     6656 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/op_concurrency_limits_counter.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/pipes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/pipes/client.py
+-rw-r--r--   0 root         (0) root         (0)    18318 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/pipes/context.py
+-rw-r--r--   0 root         (0) root         (0)     5648 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/pipes/subprocess.py
+-rw-r--r--   0 root         (0) root         (0)    25661 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/pipes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/remote_representation/
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36695 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    37482 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    83582 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/feature_flags.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19669 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    13364 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    28819 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)    10917 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18109 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.415741 dagster-1.7.5/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9302 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12155 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16934 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14185 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.419741 dagster-1.7.5/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.419741 dagster-1.7.5/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6686 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      312 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      599 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      635 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      958 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3872 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/asset_check_execution_record.py
+-rw-r--r--   0 root         (0) root         (0)     7301 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/base_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3320 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/batch_asset_record_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8725 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16223 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9557 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    25652 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11187 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20210 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7289 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     8037 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     9250 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)   121797 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7508 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    22497 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8819 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10882 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    32639 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17558 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/migration/bigint_migration.py
+-rw-r--r--   0 root         (0) root         (0)    15491 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    18101 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/root.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13903 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    37611 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6310 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     4086 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    25156 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7691 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/sqlalchemy_compat.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    19138 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    29921 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    22361 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7042 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    36504 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     6652 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    29231 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11852 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4721 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    42160 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9036 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     2665 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19590 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    12656 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/monitoring/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     9904 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/monitoring/run_monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18725 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39411 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.363741 dagster-1.7.5/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27262 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/__generated__/api_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    43164 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    22739 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    23173 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    13431 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    60914 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    29291 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     4748 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_loggers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_model/
+-rw-r--r--   0 root         (0) root         (0)     1491 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_model/pydantic_compat_layer.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42035 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      701 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8978 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7292 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    46494 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5455 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.443741 dagster-1.7.5/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    26539 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9314 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    44181 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     5865 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)    12887 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/container.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)    11214 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    33445 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/security.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.447741 dagster-1.7.5/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    13678 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7790 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/data_versions.py
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    36148 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.447741 dagster-1.7.5/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/typed_dict.py
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     4009 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4740 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/warnings.py
+-rw-r--r--   0 root         (0) root         (0)     4902 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.367741 dagster-1.7.5/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8928 2024-05-09 17:47:59.000000 dagster-1.7.5/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    29326 2024-05-09 17:47:59.000000 dagster-1.7.5/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:47:59.000000 dagster-1.7.5/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2024-05-09 17:47:59.000000 dagster-1.7.5/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1467 2024-05-09 17:47:59.000000 dagster-1.7.5/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:47:59.000000 dagster-1.7.5/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2024-05-09 17:47:59.447741 dagster-1.7.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6847 2024-05-09 17:47:35.000000 dagster-1.7.5/setup.py
```

### Comparing `dagster-1.7.4/COPYING` & `dagster-1.7.5/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/LICENSE` & `dagster-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/MANIFEST.in` & `dagster-1.7.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/PKG-INFO` & `dagster-1.7.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.4
+Version: 1.7.5
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
@@ -102,29 +102,14 @@
 
 <p align="center">
   <img width="100%" alt="An example asset graph as rendered in the Dagster UI" src="https://raw.githubusercontent.com/dagster-io/dagster/master/.github/example-lineage.png">
 </p>
 
 Dagster is built to be used at every stage of the data development lifecycle - local development, unit tests, integration tests, staging environments, all the way up to production.
 
-## Special Event: Introducing Dagster+
-
-<p align="center">
-  <img width="100%" alt="Join us on April 17 (12PM ET) for a special event introducing Dagster+" src="https://i.imgur.com/1r7hOep.png">
-</p>
-
-Join us on April 17 (12PM ET) for a special event introducing Dagster+. [Register for our Dagster+ launch event here](https://dagster.io/events/dagster-plus-launch-event)
-
-In addition to the core open-source project, we are excited to announce Dagster+, the next generation of Dagster's cloud offering.
-
-- Find out how to weave data reliability and quality checks into the execution of your data pipelines.
-- See how diff-based branch deployments will accelerate your development cycle and cut extraneous compute costs.
-- Get a deep understanding of what is driving the cost of your data pipelines, then optimize to get the best cost/performance outcomes.
-- Enjoy the benefits of built-in data cataloging, and asset-level rich metadata.
-
 ## Quick Start:
 
 If you're new to Dagster, we recommend reading about its [core concepts](https://docs.dagster.io/concepts) or learning with the hands-on [tutorial](https://docs.dagster.io/tutorial).
 
 Dagster is available on PyPI and officially supports Python 3.8 through Python 3.12.
 
 ```bash
```

### Comparing `dagster-1.7.4/README.md` & `dagster-1.7.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -62,29 +62,14 @@
 
 <p align="center">
   <img width="100%" alt="An example asset graph as rendered in the Dagster UI" src="https://raw.githubusercontent.com/dagster-io/dagster/master/.github/example-lineage.png">
 </p>
 
 Dagster is built to be used at every stage of the data development lifecycle - local development, unit tests, integration tests, staging environments, all the way up to production.
 
-## Special Event: Introducing Dagster+
-
-<p align="center">
-  <img width="100%" alt="Join us on April 17 (12PM ET) for a special event introducing Dagster+" src="https://i.imgur.com/1r7hOep.png">
-</p>
-
-Join us on April 17 (12PM ET) for a special event introducing Dagster+. [Register for our Dagster+ launch event here](https://dagster.io/events/dagster-plus-launch-event)
-
-In addition to the core open-source project, we are excited to announce Dagster+, the next generation of Dagster's cloud offering.
-
-- Find out how to weave data reliability and quality checks into the execution of your data pipelines.
-- See how diff-based branch deployments will accelerate your development cycle and cut extraneous compute costs.
-- Get a deep understanding of what is driving the cost of your data pipelines, then optimize to get the best cost/performance outcomes.
-- Enjoy the benefits of built-in data cataloging, and asset-level rich metadata.
-
 ## Quick Start:
 
 If you're new to Dagster, we recommend reading about its [core concepts](https://docs.dagster.io/concepts) or learning with the hands-on [tutorial](https://docs.dagster.io/tutorial).
 
 Dagster is available on PyPI and officially supports Python 3.8 through Python 3.12.
 
 ```bash
```

### Comparing `dagster-1.7.4/dagster/__init__.py` & `dagster-1.7.5/dagster/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,21 +107,32 @@
 )
 from dagster._config.source import (
     BoolSource as BoolSource,
     IntSource as IntSource,
     StringSource as StringSource,
 )
 from dagster._core.definitions import AssetCheckResult as AssetCheckResult
+from dagster._core.definitions.asset_check_factories.freshness_checks.last_update import (
+    build_last_update_freshness_checks as build_last_update_freshness_checks,
+)
+from dagster._core.definitions.asset_check_factories.freshness_checks.sensor import (
+    build_sensor_for_freshness_checks as build_sensor_for_freshness_checks,
+)
+from dagster._core.definitions.asset_check_factories.freshness_checks.time_partition import (
+    build_time_partition_freshness_checks as build_time_partition_freshness_checks,
+)
+from dagster._core.definitions.asset_check_factories.schema_change_checks import (
+    build_column_schema_change_checks as build_column_schema_change_checks,
+)
 from dagster._core.definitions.asset_check_spec import (
     AssetCheckKey as AssetCheckKey,
     AssetCheckSeverity as AssetCheckSeverity,
     AssetCheckSpec as AssetCheckSpec,
 )
 from dagster._core.definitions.asset_checks import AssetChecksDefinition as AssetChecksDefinition
-from dagster._core.definitions.asset_condition import AssetCondition as AssetCondition
 from dagster._core.definitions.asset_dep import AssetDep as AssetDep
 from dagster._core.definitions.asset_in import AssetIn as AssetIn
 from dagster._core.definitions.asset_out import AssetOut as AssetOut
 from dagster._core.definitions.asset_selection import AssetSelection as AssetSelection
 from dagster._core.definitions.asset_sensor_definition import (
     AssetSensorDefinition as AssetSensorDefinition,
 )
@@ -144,14 +155,18 @@
 from dagster._core.definitions.config import ConfigMapping as ConfigMapping
 from dagster._core.definitions.configurable import configured as configured
 from dagster._core.definitions.data_version import (
     DataProvenance as DataProvenance,
     DataVersion as DataVersion,
     DataVersionsByPartition as DataVersionsByPartition,
 )
+from dagster._core.definitions.declarative_scheduling import (
+    AssetCondition as AssetCondition,
+    SchedulingCondition as SchedulingCondition,
+)
 from dagster._core.definitions.decorators.asset_check_decorator import (
     asset_check as asset_check,
     multi_asset_check as multi_asset_check,
 )
 from dagster._core.definitions.decorators.asset_decorator import (
     asset as asset,
     graph_asset as graph_asset,
@@ -209,23 +224,14 @@
     multiple_process_executor_requirements as multiple_process_executor_requirements,
     multiprocess_executor as multiprocess_executor,
 )
 from dagster._core.definitions.external_asset import (
     external_asset_from_spec as external_asset_from_spec,
     external_assets_from_specs as external_assets_from_specs,
 )
-from dagster._core.definitions.freshness_checks.last_update import (
-    build_last_update_freshness_checks as build_last_update_freshness_checks,
-)
-from dagster._core.definitions.freshness_checks.sensor import (
-    build_sensor_for_freshness_checks as build_sensor_for_freshness_checks,
-)
-from dagster._core.definitions.freshness_checks.time_partition import (
-    build_time_partition_freshness_checks as build_time_partition_freshness_checks,
-)
 from dagster._core.definitions.freshness_policy import FreshnessPolicy as FreshnessPolicy
 from dagster._core.definitions.freshness_policy_sensor_definition import (
     FreshnessPolicySensorContext as FreshnessPolicySensorContext,
     FreshnessPolicySensorDefinition as FreshnessPolicySensorDefinition,
     build_freshness_policy_sensor_context as build_freshness_policy_sensor_context,
     freshness_policy_sensor as freshness_policy_sensor,
 )
@@ -373,17 +379,14 @@
 )
 from dagster._core.definitions.schedule_definition import (
     DefaultScheduleStatus as DefaultScheduleStatus,
     ScheduleDefinition as ScheduleDefinition,
     ScheduleEvaluationContext as ScheduleEvaluationContext,
     build_schedule_context as build_schedule_context,
 )
-from dagster._core.definitions.schema_change_checks import (
-    build_column_schema_change_checks as build_column_schema_change_checks,
-)
 from dagster._core.definitions.selector import (
     CodeLocationSelector as CodeLocationSelector,
     JobSelector as JobSelector,
     RepositorySelector as RepositorySelector,
 )
 from dagster._core.definitions.sensor_definition import (
     DefaultSensorStatus as DefaultSensorStatus,
```

### Comparing `dagster-1.7.4/dagster/_annotations.py` & `dagster-1.7.5/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_api/get_server_id.py` & `dagster-1.7.5/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_api/list_repositories.py` & `dagster-1.7.5/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_api/notebook_data.py` & `dagster-1.7.5/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_api/snapshot_execution_plan.py` & `dagster-1.7.5/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_api/snapshot_job.py` & `dagster-1.7.5/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_api/snapshot_partition.py` & `dagster-1.7.5/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_api/snapshot_repository.py` & `dagster-1.7.5/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_api/snapshot_schedule.py` & `dagster-1.7.5/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_api/snapshot_sensor.py` & `dagster-1.7.5/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_check/README.md` & `dagster-1.7.5/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_check/__init__.py` & `dagster-1.7.5/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/__init__.py` & `dagster-1.7.5/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/api.py` & `dagster-1.7.5/dagster/_cli/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/asset.py` & `dagster-1.7.5/dagster/_cli/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,19 @@
             implicit_job_def.asset_layer.get(asset_key).partitions_def is None
             for asset_key in asset_keys
         ):
             check.failed("Provided '--partition' option, but none of the assets are partitioned")
 
         tags = partitions_def.get_tags_for_partition_key(partition)
     else:
+        if any(
+            implicit_job_def.asset_layer.get(asset_key).partitions_def is not None
+            for asset_key in asset_keys
+        ):
+            check.failed("Asset has partitions, but no '--partition' option was provided")
         tags = {}
 
     result = execute_job(
         job=reconstructable_job, asset_selection=list(asset_keys), instance=instance, tags=tags
     )
     if not result.success:
         raise click.ClickException("Materialization failed.")
```

### Comparing `dagster-1.7.4/dagster/_cli/code_server.py` & `dagster-1.7.5/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/config_scaffolder.py` & `dagster-1.7.5/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/debug.py` & `dagster-1.7.5/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/dev.py` & `dagster-1.7.5/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/instance.py` & `dagster-1.7.5/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/job.py` & `dagster-1.7.5/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/load_handle.py` & `dagster-1.7.5/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/project.py` & `dagster-1.7.5/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/run.py` & `dagster-1.7.5/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/schedule.py` & `dagster-1.7.5/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/sensor.py` & `dagster-1.7.5/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/utils.py` & `dagster-1.7.5/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_cli/workspace/cli_target.py` & `dagster-1.7.5/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/__init__.py` & `dagster-1.7.5/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/config_schema.py` & `dagster-1.7.5/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/config_type.py` & `dagster-1.7.5/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/errors.py` & `dagster-1.7.5/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/evaluate_value_result.py` & `dagster-1.7.5/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/field.py` & `dagster-1.7.5/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/field_utils.py` & `dagster-1.7.5/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/post_process.py` & `dagster-1.7.5/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/primitive_mapping.py` & `dagster-1.7.5/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/pythonic_config/__init__.py` & `dagster-1.7.5/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.7.5/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/pythonic_config/config.py` & `dagster-1.7.5/dagster/_config/pythonic_config/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/pythonic_config/conversion_utils.py` & `dagster-1.7.5/dagster/_config/pythonic_config/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/pythonic_config/io_manager.py` & `dagster-1.7.5/dagster/_config/pythonic_config/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/pythonic_config/resource.py` & `dagster-1.7.5/dagster/_config/pythonic_config/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/pythonic_config/type_check_utils.py` & `dagster-1.7.5/dagster/_config/pythonic_config/type_check_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.7.5/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/snap.py` & `dagster-1.7.5/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/source.py` & `dagster-1.7.5/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/stack.py` & `dagster-1.7.5/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/traversal_context.py` & `dagster-1.7.5/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/type_printer.py` & `dagster-1.7.5/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_config/validate.py` & `dagster-1.7.5/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/asset_graph_view/asset_graph_view.py` & `dagster-1.7.5/dagster/_core/asset_graph_view/asset_graph_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Mapping,
     NamedTuple,
     NewType,
     Optional,
@@ -16,22 +16,20 @@
     MultiPartitionKey,
     MultiPartitionsDefinition,
     PartitionDimensionDefinition,
 )
 from dagster._core.definitions.partition import (
     AllPartitionsSubset,
     DefaultPartitionsSubset,
-    DynamicPartitionsDefinition,
-    StaticPartitionsDefinition,
 )
 from dagster._core.definitions.time_window_partitions import (
-    PartitionKeysTimeWindowPartitionsSubset,
+    BaseTimeWindowPartitionsSubset,
     TimeWindow,
     TimeWindowPartitionsDefinition,
-    TimeWindowPartitionsSubset,
+    get_time_partitions_def,
 )
 from dagster._utils.cached_method import cached_method
 
 if TYPE_CHECKING:
     from dagster._core.definitions.base_asset_graph import BaseAssetGraph, BaseAssetNode
     from dagster._core.definitions.data_version import CachingStaleStatusResolver
     from dagster._core.definitions.definitions_class import Definitions
@@ -157,28 +155,43 @@
     def compute_parent_slices(self) -> Mapping[AssetKey, "AssetSlice"]:
         return {ak: self.compute_parent_slice(ak) for ak in self.parent_keys}
 
     @cached_method
     def compute_child_slices(self) -> Mapping[AssetKey, "AssetSlice"]:
         return {ak: self.compute_child_slice(ak) for ak in self.child_keys}
 
+    def compute_difference(self, other: "AssetSlice") -> "AssetSlice":
+        return _slice_from_subset(
+            self._asset_graph_view, self._compatible_subset - other.convert_to_valid_asset_subset()
+        )
+
+    def compute_union(self, other: "AssetSlice") -> "AssetSlice":
+        return _slice_from_subset(
+            self._asset_graph_view, self._compatible_subset | other.convert_to_valid_asset_subset()
+        )
+
+    def compute_intersection(self, other: "AssetSlice") -> "AssetSlice":
+        return _slice_from_subset(
+            self._asset_graph_view, self._compatible_subset & other.convert_to_valid_asset_subset()
+        )
+
     def compute_intersection_with_partition_keys(
         self, partition_keys: AbstractSet[str]
     ) -> "AssetSlice":
         """Return a new AssetSlice with only the given partition keys if they are in the slice."""
         return self._asset_graph_view.compute_intersection_with_partition_keys(partition_keys, self)
 
     @property
     def time_windows(self) -> Sequence[TimeWindow]:
         """Get the time windows for the asset slice. Only supports explicitly time-windowed partitions for now."""
         tw_partitions_def = check.not_none(
             self._time_window_partitions_def_in_context(), "Must be time windowed."
         )
 
-        if isinstance(self._compatible_subset.subset_value, TimeWindowPartitionsSubset):
+        if isinstance(self._compatible_subset.subset_value, BaseTimeWindowPartitionsSubset):
             return self._compatible_subset.subset_value.included_time_windows
         elif isinstance(self._compatible_subset.subset_value, AllPartitionsSubset):
             last_tw = tw_partitions_def.get_last_partition_window(
                 self._asset_graph_view.effective_dt
             )
             return [TimeWindow(datetime.min, last_tw.end)] if last_tw else []
         elif isinstance(self._compatible_subset.subset_value, DefaultPartitionsSubset):
@@ -194,21 +207,17 @@
                 "Keys must be multi partition keys.",
             ):
                 tm_partition_key = next(iter(multi_partition_key.keys_by_dimension.values()))
                 tw_partition_keys.add(tm_partition_key)
 
             subset_from_tw = tw_partitions_def.subset_with_partition_keys(tw_partition_keys)
             check.inst(
-                subset_from_tw,
-                (TimeWindowPartitionsSubset, PartitionKeysTimeWindowPartitionsSubset),
-                "Must be time window subset.",
+                subset_from_tw, BaseTimeWindowPartitionsSubset, "Must be time window subset."
             )
-            if isinstance(subset_from_tw, TimeWindowPartitionsSubset):
-                return subset_from_tw.included_time_windows
-            elif isinstance(subset_from_tw, PartitionKeysTimeWindowPartitionsSubset):
+            if isinstance(subset_from_tw, BaseTimeWindowPartitionsSubset):
                 return subset_from_tw.included_time_windows
             else:
                 check.failed(
                     f"Unsupported subset value in generated subset {self._compatible_subset.subset_value} created by keys {tw_partition_keys}"
                 )
 
         check.failed(f"Unsupported subset value: {self._compatible_subset.subset_value}")
@@ -219,15 +228,15 @@
             return pd
         if isinstance(pd, MultiPartitionsDefinition):
             return pd.time_window_partitions_def if pd.has_time_window_dimension else None
         return None
 
     @property
     def is_empty(self) -> bool:
-        return self._compatible_subset.size == 0
+        return self._compatible_subset.is_empty
 
 
 class AssetGraphView:
     """The Asset Graph View. It is a view of the asset graph from the perspective of a specific
     temporal context.
 
     If the user wants to get a new view of the asset graph with a new effective date or last event
@@ -324,14 +333,44 @@
                 asset_key=asset_key,
                 partitions_def=self._get_partitions_def(asset_key),
                 dynamic_partitions_store=self._queryer,
                 current_time=self.effective_dt,
             ),
         )
 
+    def get_asset_slice_from_subset(self, subset: AssetSubset) -> "AssetSlice":
+        return _slice_from_subset(self, subset)
+
+    def compute_missing_subslice(
+        self, asset_key: "AssetKey", from_slice: "AssetSlice"
+    ) -> "AssetSlice":
+        """Returns a slice which is the subset of the input slice that has never been materialized
+        (if it is a materializable asset) or observered (if it is an observable asset).
+        """
+        # TODO: this logic should be simplified once we have a unified way of detecting both
+        # materializations and observations through the parittion status cache. at that point, the
+        # definition will slightly change to search for materializations and observations regardless
+        # of the materializability of the asset
+        if self.asset_graph.get(asset_key).is_materializable:
+            # cheap call which takes advantage of the partition status cache
+            materialized_subset = self._queryer.get_materialized_asset_subset(asset_key=asset_key)
+            materialized_slice = self.get_asset_slice_from_subset(materialized_subset)
+            return from_slice.compute_difference(materialized_slice)
+        else:
+            # more expensive call
+            missing_asset_partitions = {
+                ap
+                for ap in from_slice.convert_to_valid_asset_subset().asset_partitions
+                if not self._queryer.asset_partition_has_materialization_or_observation(ap)
+            }
+            missing_subset = ValidAssetSubset.from_asset_partitions_set(
+                asset_key, self._get_partitions_def(asset_key), missing_asset_partitions
+            )
+            return self.get_asset_slice_from_subset(missing_subset)
+
     def compute_parent_asset_slice(
         self, parent_asset_key: AssetKey, asset_slice: AssetSlice
     ) -> AssetSlice:
         return _slice_from_subset(
             self,
             self.asset_graph.get_parent_asset_subset(
                 dynamic_partitions_store=self._queryer,
@@ -350,14 +389,19 @@
                 dynamic_partitions_store=self._queryer,
                 child_asset_key=child_asset_key,
                 current_time=self.effective_dt,
                 parent_asset_subset=asset_slice.convert_to_valid_asset_subset(),
             ),
         )
 
+    def compute_in_progress_asset_slice(self, asset_key: "AssetKey") -> "AssetSlice":
+        return _slice_from_subset(
+            self, self._queryer.get_in_progress_asset_subset(asset_key=asset_key)
+        )
+
     def compute_intersection_with_partition_keys(
         self, partition_keys: AbstractSet[str], asset_slice: AssetSlice
     ) -> "AssetSlice":
         """Return a new AssetSlice with only the given partition keys if they are in the slice."""
         partitions_def = check.not_none(
             self._get_partitions_def(asset_slice.asset_key), "Must have partitions def"
         )
@@ -375,68 +419,54 @@
             self,
             asset_slice.convert_to_valid_asset_subset()
             & AssetSubset.from_partition_keys(
                 asset_slice.asset_key, partitions_def, partition_keys
             ),
         )
 
-    def create_from_time_window(self, asset_key: AssetKey, time_window: TimeWindow) -> AssetSlice:
-        return _slice_from_subset(
-            self,
-            AssetSubset(
-                asset_key=asset_key,
-                value=TimeWindowPartitionsSubset(
-                    partitions_def=_required_tw_partitions_def(self._get_partitions_def(asset_key)),
-                    num_partitions=None,
-                    included_time_windows=[time_window],
-                ),
-            ),
-        )
-
-    def create_latest_time_window_slice(self, asset_key: AssetKey) -> AssetSlice:
-        """If the underlying asset is time-window partitioned, this will return the latest complete
-        time window relative to the effective date. For example if it is daily partitioned starting
-        at midnight every day.  If the effective date is before the start of the partition definition, this will
-        return the empty time window (where both start and end are datetime.max).
-
-        If the underlying asset is unpartitioned or static partitioned and it is not empty,
-        this will return a time window from the beginning of time to the effective date. If
-        it is empty it will return the empty time window.
-
-        TODO: add language for multi-dimensional partitioning when we support it
-        TODO: add language for dynamic partitioning when we support it
+    def compute_latest_time_window_slice(
+        self, asset_key: AssetKey, lookback_delta: Optional[timedelta] = None
+    ) -> AssetSlice:
+        """Compute the slice of the asset which exists within the latest time partition window. If
+        the asset has no time dimension, this will always return the full slice. If
+        lookback_delta is provided, all partitions that are up to that timedelta before the
+        end of the latest time partition window will be included.
         """
         partitions_def = self._get_partitions_def(asset_key)
-        if partitions_def is None or isinstance(
-            partitions_def, (DynamicPartitionsDefinition, StaticPartitionsDefinition)
-        ):
+        time_partitions_def = get_time_partitions_def(partitions_def)
+        if time_partitions_def is None:
+            # if the asset has no time dimension, then return a full slice
             return self.get_asset_slice(asset_key)
 
-        if isinstance(partitions_def, TimeWindowPartitionsDefinition):
-            time_window = partitions_def.get_last_partition_window(self.effective_dt)
-            return (
-                self.create_from_time_window(asset_key, time_window)
-                if time_window
-                else self.create_empty_slice(asset_key)
+        latest_time_window = time_partitions_def.get_last_partition_window(self.effective_dt)
+        if latest_time_window is None:
+            return self.create_empty_slice(asset_key)
+
+        # the time window in which to look for partitions
+        time_window = (
+            TimeWindow(
+                start=max(
+                    # do not look before the start of the definition
+                    time_partitions_def.start,
+                    latest_time_window.end - lookback_delta,
+                ),
+                end=latest_time_window.end,
             )
+            if lookback_delta
+            else latest_time_window
+        )
 
-        if isinstance(partitions_def, MultiPartitionsDefinition):
-            if not partitions_def.has_time_window_dimension:
-                return self.get_asset_slice(asset_key)
-
-            multi_dim_info = self._get_multi_dim_info(asset_key)
-            last_tw = multi_dim_info.tw_partition_def.get_last_partition_window(self.effective_dt)
-            return (
-                self._build_multi_partition_slice(asset_key, multi_dim_info, last_tw)
-                if last_tw
-                else self.create_empty_slice(asset_key)
+        if isinstance(partitions_def, TimeWindowPartitionsDefinition):
+            return self._build_time_partition_slice(asset_key, partitions_def, time_window)
+        elif isinstance(partitions_def, MultiPartitionsDefinition):
+            return self._build_multi_partition_slice(
+                asset_key, self._get_multi_dim_info(asset_key), time_window
             )
-
-        # Need to handle dynamic partitioning
-        check.failed(f"Unsupported partitions_def: {partitions_def}")
+        else:
+            check.failed(f"Unsupported partitions_def: {partitions_def}")
 
     def create_empty_slice(self, asset_key: AssetKey) -> AssetSlice:
         return _slice_from_subset(
             self,
             AssetSubset.empty(asset_key, self._get_partitions_def(asset_key)),
         )
 
@@ -461,31 +491,41 @@
             MultiPartitionsDefinition,
         )
         return self.MultiDimInfo(
             tw_dim=partitions_def.time_window_dimension,
             secondary_dim=partitions_def.secondary_dimension,
         )
 
+    def _build_time_partition_slice(
+        self,
+        asset_key: AssetKey,
+        partitions_def: TimeWindowPartitionsDefinition,
+        time_window: TimeWindow,
+    ) -> "AssetSlice":
+        return self.get_asset_slice(asset_key).compute_intersection_with_partition_keys(
+            set(partitions_def.get_partition_keys_in_time_window(time_window))
+        )
+
     def _build_multi_partition_slice(
-        self, asset_key: AssetKey, multi_dim_info: MultiDimInfo, last_tw: TimeWindow
+        self, asset_key: AssetKey, multi_dim_info: MultiDimInfo, time_window: TimeWindow
     ) -> "AssetSlice":
         # Note: Potential perf improvement here. There is no way to encode a cartesian product
         # in the underlying PartitionsSet. We could add a specialized PartitionsSubset
         # subclass that itself composed two PartitionsSubset to avoid materializing the entire
         # partitions range.
         return self.get_asset_slice(asset_key).compute_intersection_with_partition_keys(
             {
                 MultiPartitionKey(
                     {
                         multi_dim_info.tw_dim.name: tw_pk,
                         multi_dim_info.secondary_dim.name: secondary_pk,
                     }
                 )
                 for tw_pk in multi_dim_info.tw_partition_def.get_partition_keys_in_time_window(
-                    last_tw
+                    time_window
                 )
                 for secondary_pk in multi_dim_info.secondary_partition_def.get_partition_keys(
                     current_time=self.effective_dt,
                     dynamic_partitions_store=self._queryer,
                 )
             }
         )
```

### Comparing `dagster-1.7.4/dagster/_core/assets.py` & `dagster-1.7.5/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/code_pointer.py` & `dagster-1.7.5/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/container_context/config.py` & `dagster-1.7.5/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/debug.py` & `dagster-1.7.5/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/decorator_utils.py` & `dagster-1.7.5/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/__init__.py` & `dagster-1.7.5/dagster/_core/definitions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .asset_check_result import (
     AssetCheckEvaluation as AssetCheckEvaluation,
     AssetCheckResult as AssetCheckResult,
+    AssetCheckSeverity as AssetCheckSeverity,
 )
 from .composition import PendingNodeInvocation as PendingNodeInvocation
 from .config import ConfigMapping as ConfigMapping
 from .dependency import (
     DependencyDefinition as DependencyDefinition,
     MultiDependencyDefinition as MultiDependencyDefinition,
     Node as Node,
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_check_evaluation.py` & `dagster-1.7.5/dagster/_core/definitions/asset_check_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_check_result.py` & `dagster-1.7.5/dagster/_core/definitions/asset_check_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_check_spec.py` & `dagster-1.7.5/dagster/_core/definitions/asset_check_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_checks.py` & `dagster-1.7.5/dagster/_core/definitions/asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_condition/asset_condition.py` & `dagster-1.7.5/dagster/_core/definitions/auto_materialize_rule_evaluation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,557 +1,549 @@
-import functools
-from abc import ABC, abstractmethod
-from dataclasses import dataclass
+from abc import ABC, abstractproperty
+from collections import defaultdict
+from enum import Enum
 from typing import (
-    TYPE_CHECKING,
     AbstractSet,
     Dict,
     FrozenSet,
-    List,
-    Mapping,
+    NamedTuple,
     Optional,
     Sequence,
     Tuple,
-    Type,
-    TypeVar,
     Union,
+    cast,
 )
 
-import pendulum
-
-from dagster._annotations import experimental
+import dagster._check as check
+from dagster._core.definitions.asset_subset import AssetSubset
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.metadata import MetadataMapping, MetadataValue
-from dagster._core.definitions.partition import AllPartitionsSubset
-from dagster._model import DagsterModel
-from dagster._serdes.serdes import PackableValue, whitelist_for_serdes
+from dagster._serdes.serdes import (
+    _WHITELIST_MAP,
+    NamedTupleSerializer,
+    PackableValue,
+    PydanticModelSerializer,
+    UnpackContext,
+    UnpackedValue,
+    WhitelistMap,
+    deserialize_value,
+    whitelist_for_serdes,
+)
 from dagster._utils.security import non_secure_md5_hash_str
 
-from ..asset_subset import AssetSubset, ValidAssetSubset
-from ..auto_materialize_rule import AutoMaterializeRule
-
-if TYPE_CHECKING:
-    from .asset_condition_evaluation_context import AssetConditionEvaluationContext
-
-
-T = TypeVar("T")
+from .declarative_scheduling.serialized_objects import (
+    AssetConditionEvaluation,
+    AssetConditionEvaluationWithRunIds,
+    AssetConditionSnapshot,
+    AssetSubsetWithMetadata,
+)
+from .partition import PartitionsDefinition, SerializedPartitionsSubset
 
 
 @whitelist_for_serdes
-class HistoricalAllPartitionsSubsetSentinel(DagsterModel):
-    """Serializable indicator that this value was an AllPartitionsSubset at serialization time, but
-    the partitions may have changed since that time.
+class AutoMaterializeDecisionType(Enum):
+    """Represents the set of results of the auto-materialize logic.
+
+    MATERIALIZE: The asset should be materialized by a run kicked off on this tick
+    SKIP: The asset should not be materialized by a run kicked off on this tick, because future
+        ticks are expected to materialize it.
+    DISCARD: The asset should not be materialized by a run kicked off on this tick, but future
+        ticks are not expected to materialize it.
     """
 
+    MATERIALIZE = "MATERIALIZE"
+    SKIP = "SKIP"
+    DISCARD = "DISCARD"
+
 
 @whitelist_for_serdes
-class AssetConditionSnapshot(DagsterModel):
-    """A serializable snapshot of a node in the AutomationCondition tree."""
+class AutoMaterializeRuleSnapshot(NamedTuple):
+    """A serializable snapshot of an AutoMaterializeRule for historical evaluations."""
 
     class_name: str
     description: str
-    unique_id: str
+    decision_type: AutoMaterializeDecisionType
 
 
-@whitelist_for_serdes
-class AssetSubsetWithMetadata(DagsterModel):
-    """An asset subset with metadata that corresponds to it."""
-
-    subset: AssetSubset
-    metadata: MetadataMapping
+class AutoMaterializeRuleEvaluationData(ABC):
+    @abstractproperty
+    def metadata(self) -> MetadataMapping:
+        raise NotImplementedError()
 
     @property
     def frozen_metadata(self) -> FrozenSet[Tuple[str, MetadataValue]]:
         return frozenset(self.metadata.items())
 
 
-def get_serializable_candidate_subset(
-    candidate_subset: Union[AssetSubset, HistoricalAllPartitionsSubsetSentinel],
-) -> Union[AssetSubset, HistoricalAllPartitionsSubsetSentinel]:
-    """Do not serialize the candidate subset directly if it is an AllPartitionsSubset."""
-    if isinstance(candidate_subset, AssetSubset) and isinstance(
-        candidate_subset.value, AllPartitionsSubset
-    ):
-        return HistoricalAllPartitionsSubsetSentinel()
-    return candidate_subset
-
-
 @whitelist_for_serdes
-class AssetConditionEvaluation(DagsterModel):
-    """Serializable representation of the results of evaluating a node in the evaluation tree."""
-
-    condition_snapshot: AssetConditionSnapshot
-    start_timestamp: Optional[float]
-    end_timestamp: Optional[float]
-
-    true_subset: AssetSubset
-    candidate_subset: Union[AssetSubset, HistoricalAllPartitionsSubsetSentinel]
-    subsets_with_metadata: Sequence[AssetSubsetWithMetadata]
-
-    child_evaluations: Sequence["AssetConditionEvaluation"]
-
+class TextRuleEvaluationData(
+    AutoMaterializeRuleEvaluationData,
+    NamedTuple("_TextRuleEvaluationData", [("text", str)]),
+):
     @property
-    def asset_key(self) -> AssetKey:
-        return self.true_subset.asset_key
-
-    @staticmethod
-    def from_result(result: "AssetConditionResult") -> "AssetConditionEvaluation":
-        return AssetConditionEvaluation(
-            condition_snapshot=result.condition.snapshot,
-            start_timestamp=result.start_timestamp,
-            end_timestamp=result.end_timestamp,
-            true_subset=result.true_subset,
-            candidate_subset=get_serializable_candidate_subset(result.candidate_subset),
-            subsets_with_metadata=result.subsets_with_metadata,
-            child_evaluations=[
-                AssetConditionEvaluation.from_result(child_result)
-                for child_result in result.child_results
-            ],
-        )
-
-    def equivalent_to_stored_evaluation(self, other: Optional["AssetConditionEvaluation"]) -> bool:
-        """Returns if this evaluation is functionally equivalent to the given stored evaluation.
-        This is used to determine if it is necessary to store this new evaluation in the database.
-        Noteably, the timestamps on successive evaluations will always be different, so a simple
-        equality check would be too strict.
-        """
-        return (
-            other is not None
-            and self.condition_snapshot == other.condition_snapshot
-            and self.true_subset == other.true_subset
-            # the candidate subset gets modified during serialization
-            and get_serializable_candidate_subset(self.candidate_subset)
-            == get_serializable_candidate_subset(other.candidate_subset)
-            and self.subsets_with_metadata == other.subsets_with_metadata
-            and len(self.child_evaluations) == len(other.child_evaluations)
-            and all(
-                self_child.equivalent_to_stored_evaluation(other_child)
-                for self_child, other_child in zip(self.child_evaluations, other.child_evaluations)
-            )
-        )
-
-    def discarded_subset(self) -> Optional[AssetSubset]:
-        """Returns the AssetSubset representing asset partitions that were discarded during this
-        evaluation. Note that 'discarding' is a deprecated concept that is only used for backwards
-        compatibility.
-        """
-        if len(self.child_evaluations) != 3:
-            return None
-        not_discard_evaluation = self.child_evaluations[-1]
-        discard_evaluation = not_discard_evaluation.child_evaluations[0]
-        return discard_evaluation.true_subset
-
-    def get_requested_or_discarded_subset(self) -> AssetSubset:
-        discarded_subset = self.discarded_subset()
-        if discarded_subset is None:
-            return self.true_subset
-        else:
-            # the true_subset and discarded_subset were created on the same tick, so they are
-            # guaranteed to be compatible with each other
-            return (
-                ValidAssetSubset(asset_key=self.asset_key, value=self.true_subset.value)
-                | discarded_subset
-            )
-
-    def for_child(self, child_condition: "AssetCondition") -> Optional["AssetConditionEvaluation"]:
-        """Returns the evaluation of a given child condition by finding the child evaluation that
-        has an identical hash to the given condition.
-        """
-        child_unique_id = child_condition.snapshot.unique_id
-        for child_evaluation in self.child_evaluations:
-            if child_evaluation.condition_snapshot.unique_id == child_unique_id:
-                return child_evaluation
-
-        return None
-
-    def with_run_ids(self, run_ids: AbstractSet[str]) -> "AssetConditionEvaluationWithRunIds":
-        return AssetConditionEvaluationWithRunIds(evaluation=self, run_ids=frozenset(run_ids))
-
-    def legacy_num_skipped(self) -> int:
-        if len(self.child_evaluations) < 2:
-            return 0
-
-        not_skip_evaluation = self.child_evaluations[-1]
-        skip_evaluation = not_skip_evaluation.child_evaluations[0]
-        return skip_evaluation.true_subset.size - self.legacy_num_discarded()
-
-    def legacy_num_discarded(self) -> int:
-        discarded_subset = self.discarded_subset()
-        if discarded_subset is None:
-            return 0
-        return discarded_subset.size
+    def metadata(self) -> MetadataMapping:
+        return {"text": MetadataValue.text(self.text)}
 
 
 @whitelist_for_serdes
-@dataclass(frozen=True)
-class AssetConditionEvaluationState:
-    """Incremental state calculated during the evaluation of an AssetCondition. This may be used
-    on the subsequent evaluation to make the computation more efficient.
-
-    Attributes:
-        previous_evaluation: The computed AssetConditionEvaluation.
-        previous_tick_evaluation_timestamp: The evaluation_timestamp at which the evaluation was performed.
-        max_storage_id: The maximum storage ID over all events used in this computation.
-        extra_state_by_unique_id: A mapping from the unique ID of each condition in the evaluation
-            tree to the extra state that was calculated for it, if any.
-    """
-
-    previous_evaluation: AssetConditionEvaluation
-    previous_tick_evaluation_timestamp: Optional[float]
-
-    max_storage_id: Optional[int]
-    extra_state_by_unique_id: Mapping[str, PackableValue]
-
-    @property
-    def asset_key(self) -> AssetKey:
-        return self.previous_evaluation.asset_key
-
-    @property
-    def true_subset(self) -> AssetSubset:
-        return self.previous_evaluation.true_subset
-
-    @staticmethod
-    def create(
-        context: "AssetConditionEvaluationContext", root_result: "AssetConditionResult"
-    ) -> "AssetConditionEvaluationState":
-        """Convenience constructor to generate an AssetConditionEvaluationState from the root result
-        and the context in which it was evaluated.
-        """
-
-        # flatten the extra state into a single dict
-        def _flatten_extra_state(
-            r: AssetConditionResult,
-        ) -> Mapping[str, PackableValue]:
-            extra_state: Dict[str, PackableValue] = (
-                {r.condition.unique_id: r.extra_state} if r.extra_state else {}
-            )
-            for child in r.child_results:
-                extra_state.update(_flatten_extra_state(child))
-            return extra_state
-
-        return AssetConditionEvaluationState(
-            previous_evaluation=AssetConditionEvaluation.from_result(root_result),
-            previous_tick_evaluation_timestamp=context.evaluation_time.timestamp(),
-            max_storage_id=context.new_max_storage_id,
-            extra_state_by_unique_id=_flatten_extra_state(root_result),
-        )
-
-    def get_extra_state(self, condition: "AssetCondition", as_type: Type[T]) -> Optional[T]:
-        """Returns the value from the extras dict for the given condition, if it exists and is of
-        the expected type. Otherwise, returns None.
-        """
-        extra_state = self.extra_state_by_unique_id.get(condition.unique_id)
-        if isinstance(extra_state, as_type):
-            return extra_state
-        return None
+class ParentUpdatedRuleEvaluationData(
+    AutoMaterializeRuleEvaluationData,
+    NamedTuple(
+        "_ParentUpdatedRuleEvaluationData",
+        [
+            ("updated_asset_keys", FrozenSet[AssetKey]),
+            ("will_update_asset_keys", FrozenSet[AssetKey]),
+        ],
+    ),
+):
+    @property
+    def metadata(self) -> MetadataMapping:
+        return {
+            **{
+                f"updated_parent_{i+1}": MetadataValue.asset(k)
+                for i, k in enumerate(sorted(self.updated_asset_keys))
+            },
+            **{
+                f"will_update_parent_{i+1}": MetadataValue.asset(k)
+                for i, k in enumerate(sorted(self.will_update_asset_keys))
+            },
+        }
 
 
 @whitelist_for_serdes
-class AssetConditionEvaluationWithRunIds(DagsterModel):
-    """A union of an AssetConditionEvaluation and the set of run IDs that have been launched in
-    response to it.
-    """
+class WaitingOnAssetsRuleEvaluationData(
+    AutoMaterializeRuleEvaluationData,
+    NamedTuple(
+        "_WaitingOnParentRuleEvaluationData",
+        [("waiting_on_asset_keys", FrozenSet[AssetKey])],
+    ),
+):
+    @property
+    def metadata(self) -> MetadataMapping:
+        return {
+            **{
+                f"waiting_on_ancestor_{i+1}": MetadataValue.asset(k)
+                for i, k in enumerate(sorted(self.waiting_on_asset_keys))
+            },
+        }
 
-    evaluation: AssetConditionEvaluation
-    run_ids: FrozenSet[str]
 
-    @property
-    def asset_key(self) -> AssetKey:
-        return self.evaluation.asset_key
+RuleEvaluations = Tuple[AssetSubset, Sequence["AssetSubsetWithMetadata"], PackableValue]
 
-    @property
-    def num_requested(self) -> int:
-        return self.evaluation.true_subset.size
 
+@whitelist_for_serdes
+class AutoMaterializeRuleEvaluation(NamedTuple):
+    rule_snapshot: AutoMaterializeRuleSnapshot
+    evaluation_data: Optional[AutoMaterializeRuleEvaluationData]
 
-class AssetCondition(ABC, DagsterModel):
-    """An AssetCondition represents some state of the world that can influence if an asset
-    partition should be materialized or not. AssetConditions can be combined to create
-    new conditions using the `&` (and), `|` (or), and `~` (not) operators.
 
-    Examples:
-        .. code-block:: python
+# BACKCOMPAT GRAVEYARD
 
-            from dagster import AssetCondition, AutoMaterializePolicy
 
-            # At least one parent is newer and no parent is missing.
-            my_policy = AutoMaterializePolicy(
-                asset_condition = AssetCondition.parent_newer() & ~AssetCondition.parent_missing()
-            )
+def deserialize_auto_materialize_asset_evaluation_to_asset_condition_evaluation_with_run_ids(
+    serialized_evaluation: str, partitions_def: Optional[PartitionsDefinition]
+) -> "AssetConditionEvaluationWithRunIds":
+    """Provides a backcompat layer to allow deserializing old AutoMaterializeAssetEvaluation
+    objects into the new AssetConditionEvaluationWithRunIds objects.
+    """
+    from .declarative_scheduling.serialized_objects import (
+        AssetConditionEvaluationWithRunIds,
+    )
+
+    class BackcompatDeserializer(BackcompatAutoMaterializeAssetEvaluationSerializer):
+        @property
+        def partitions_def(self) -> Optional[PartitionsDefinition]:
+            return partitions_def
+
+    # create a new WhitelistMap that can deserialize SerializedPartitionSubset objects stored
+    # on the old cursor format
+    whitelist_map = WhitelistMap(
+        object_serializers=_WHITELIST_MAP.object_serializers,
+        object_deserializers={
+            **_WHITELIST_MAP.object_deserializers,
+            "AutoMaterializeAssetEvaluation": BackcompatDeserializer(
+                klass=AssetConditionEvaluationWithRunIds
+            ),
+        },
+        enum_serializers=_WHITELIST_MAP.enum_serializers,
+    )
+
+    return deserialize_value(
+        serialized_evaluation, AssetConditionEvaluationWithRunIds, whitelist_map=whitelist_map
+    )
+
+
+def deserialize_serialized_partitions_subset_to_asset_subset(
+    serialized: SerializedPartitionsSubset,
+    asset_key: AssetKey,
+    partitions_def: Optional[PartitionsDefinition],
+) -> AssetSubset:
+    if partitions_def is None or not serialized.can_deserialize(partitions_def):
+        # partitions def has changed since storage time
+        return AssetSubset.empty(asset_key, partitions_def)
+
+    return AssetSubset(asset_key=asset_key, value=serialized.deserialize(partitions_def))
+
+
+class BackcompatAutoMaterializeAssetEvaluationSerializer(PydanticModelSerializer):
+    """This handles backcompat for the old AutoMaterializeAssetEvaluation objects, turning them into
+    AssetConditionEvaluationWithRunIds objects.
     """
 
     @property
-    def unique_id(self) -> str:
-        parts = [
-            self.__class__.__name__,
-            *[child.unique_id for child in self.children],
-        ]
-        return non_secure_md5_hash_str("".join(parts).encode())
-
-    @abstractmethod
-    def evaluate(self, context: "AssetConditionEvaluationContext") -> "AssetConditionResult":
-        raise NotImplementedError()
-
-    @property
-    @abstractmethod
-    def description(self) -> str:
-        raise NotImplementedError()
-
-    def __and__(self, other: "AssetCondition") -> "AssetCondition":
-        # group AndAssetConditions together
-        if isinstance(self, AndAssetCondition):
-            return AndAssetCondition(operands=[*self.operands, other])
-        return AndAssetCondition(operands=[self, other])
-
-    def __or__(self, other: "AssetCondition") -> "AssetCondition":
-        # group OrAssetConditions together
-        if isinstance(self, OrAssetCondition):
-            return OrAssetCondition(operands=[*self.operands, other])
-        return OrAssetCondition(operands=[self, other])
-
-    def __invert__(self) -> "AssetCondition":
-        return NotAssetCondition(operand=self)
-
-    @property
-    def is_legacy(self) -> bool:
-        """Returns if this condition is in the legacy format. This is used to determine if we can
-        do certain types of backwards-compatible operations on it.
+    def partitions_def(self) -> Optional[PartitionsDefinition]:
+        """This property gets overridden by subclasses at runtime, once the partitions_def for the
+        specific record we're deserializing is known.
         """
-        return (
-            isinstance(self, AndAssetCondition)
-            and len(self.children) in {2, 3}
-            and isinstance(self.children[0], OrAssetCondition)
-            and isinstance(self.children[1], NotAssetCondition)
-            # the third child is the discard condition, which is optional
-            and (len(self.children) == 2 or isinstance(self.children[2], NotAssetCondition))
-        )
+        raise NotImplementedError()
 
-    @property
-    def children(self) -> Sequence["AssetCondition"]:
-        return []
+    def deserialize_serialized_partitions_subset_or_none(
+        self,
+        asset_key: AssetKey,
+        serialized: Union[None, SerializedPartitionsSubset],
+    ) -> AssetSubset:
+        if serialized is None:
+            # Confusingly, we used `None` to indicate "all of an unpartitioned asset" in the old
+            # serialization scheme
+            return AssetSubset(asset_key=asset_key, value=True)
+        return deserialize_serialized_partitions_subset_to_asset_subset(
+            serialized, asset_key, self.partitions_def
+        )
+
+    def _asset_condition_snapshot_from_rule_snapshot(
+        self, rule_snapshot: AutoMaterializeRuleSnapshot
+    ) -> "AssetConditionSnapshot":
+        from .declarative_scheduling.legacy.rule_condition import RuleCondition
+        from .declarative_scheduling.serialized_objects import AssetConditionSnapshot
 
-    @property
-    def not_skip_condition(self) -> Optional["AssetCondition"]:
-        if not self.is_legacy:
-            return None
-        return self.children[1]
+        unique_id_parts = [rule_snapshot.class_name, rule_snapshot.description]
+        unique_id = non_secure_md5_hash_str("".join(unique_id_parts).encode())
 
-    @property
-    def not_discard_condition(self) -> Optional["AssetCondition"]:
-        if not self.is_legacy or not len(self.children) == 3:
-            return None
-        return self.children[-1]
-
-    @functools.cached_property
-    def snapshot(self) -> AssetConditionSnapshot:
-        """Returns a snapshot of this condition that can be used for serialization."""
         return AssetConditionSnapshot(
-            class_name=self.__class__.__name__,
-            description=self.description,
-            unique_id=self.unique_id,
-        )
-
-    @staticmethod
-    def parent_newer() -> "AssetCondition":
-        """Returns an AssetCondition that is true for an asset partition when at least one parent
-        asset partition is newer than it.
-        """
-        return RuleCondition(rule=AutoMaterializeRule.materialize_on_parent_updated())
-
-    @staticmethod
-    def missing() -> "AssetCondition":
-        """Returns an AssetCondition that is true for an asset partition when it has never been
-        materialized.
-        """
-        from ..auto_materialize_rule import AutoMaterializeRule
-
-        return RuleCondition(rule=AutoMaterializeRule.materialize_on_missing())
-
-    @staticmethod
-    def parent_missing() -> "AssetCondition":
-        """Returns an AssetCondition that is true for an asset partition when at least one parent
-        asset partition has never been materialized or observed.
-        """
-        from ..auto_materialize_rule import AutoMaterializeRule
-
-        return RuleCondition(rule=AutoMaterializeRule.skip_on_parent_missing())
-
-    @staticmethod
-    def updated_since_cron(cron_schedule: str, timezone: str = "UTC") -> "AssetCondition":
-        """Returns an AssetCondition that is true for an asset partition when it has been updated
-        since the latest tick of the given cron schedule. For partitioned assets with a time
-        component, this can only be true for the most recent partition.
-        """
-        from ..auto_materialize_rule import AutoMaterializeRule
-
-        return ~RuleCondition(rule=AutoMaterializeRule.materialize_on_cron(cron_schedule, timezone))
-
-    @staticmethod
-    def parents_updated_since_cron(cron_schedule: str, timezone: str = "UTC") -> "AssetCondition":
-        """Returns an AssetCondition that is true for an asset partition when all parent asset
-        partitions have been updated more recently than the latest tick of the given cron schedule.
-        """
-        from ..auto_materialize_rule import AutoMaterializeRule
+            class_name=RuleCondition.__name__,
+            description=rule_snapshot.description,
+            unique_id=unique_id,
+        )
+
+    def _get_child_rule_evaluation(
+        self,
+        asset_key: AssetKey,
+        partition_subsets_by_condition: Sequence[
+            Tuple["AutoMaterializeRuleEvaluation", Optional[SerializedPartitionsSubset]]
+        ],
+        is_partitioned: bool,
+        rule_snapshot: AutoMaterializeRuleSnapshot,
+    ) -> "AssetConditionEvaluation":
+        from .declarative_scheduling.serialized_objects import (
+            HistoricalAllPartitionsSubsetSentinel,
+        )
+
+        condition_snapshot = self._asset_condition_snapshot_from_rule_snapshot(rule_snapshot)
+
+        subsets_with_metadata = [
+            AssetSubsetWithMetadata(
+                subset=self.deserialize_serialized_partitions_subset_or_none(asset_key, serialized),
+                metadata=rule_evaluation.evaluation_data.metadata,
+            )
+            for rule_evaluation, serialized in partition_subsets_by_condition
+            if rule_evaluation.evaluation_data
+        ]
 
-        return ~RuleCondition(
-            rule=AutoMaterializeRule.skip_on_not_all_parents_updated_since_cron(
-                cron_schedule, timezone
+        true_subset = AssetSubset.empty(asset_key, self.partitions_def)
+        for _, serialized in partition_subsets_by_condition:
+            true_subset |= self.deserialize_serialized_partitions_subset_or_none(
+                asset_key, serialized
             )
-        )
 
+        return AssetConditionEvaluation(
+            condition_snapshot=condition_snapshot,
+            true_subset=true_subset,
+            candidate_subset=HistoricalAllPartitionsSubsetSentinel()
+            if is_partitioned
+            else AssetSubset.all(asset_key, None),
+            start_timestamp=None,
+            end_timestamp=None,
+            subsets_with_metadata=subsets_with_metadata,
+            child_evaluations=[],
+        )
 
-@experimental
-@whitelist_for_serdes
-class RuleCondition(AssetCondition):
-    """This class represents the condition that a particular AutoMaterializeRule is satisfied."""
+    def _get_child_decision_type_evaluation(
+        self,
+        asset_key: AssetKey,
+        partition_subsets_by_condition: Sequence[
+            Tuple["AutoMaterializeRuleEvaluation", Optional[SerializedPartitionsSubset]]
+        ],
+        rule_snapshots: Sequence[AutoMaterializeRuleSnapshot],
+        is_partitioned: bool,
+        decision_type: AutoMaterializeDecisionType,
+    ) -> Optional["AssetConditionEvaluation"]:
+        from .declarative_scheduling.operators.boolean_operators import (
+            NotAssetCondition,
+            OrAssetCondition,
+        )
+        from .declarative_scheduling.serialized_objects import (
+            HistoricalAllPartitionsSubsetSentinel,
+        )
+
+        partition_subsets_by_condition_by_rule_snapshot = defaultdict(list)
+        for elt in partition_subsets_by_condition:
+            partition_subsets_by_condition_by_rule_snapshot[elt[0].rule_snapshot].append(elt)
+
+        child_evaluations = [
+            self._get_child_rule_evaluation(
+                asset_key,
+                partition_subsets_by_condition_by_rule_snapshot[rule_snapshot],
+                is_partitioned,
+                rule_snapshot,
+            )
+            for rule_snapshot in (
+                set(rule_snapshots) | set(partition_subsets_by_condition_by_rule_snapshot.keys())
+            )
+            if rule_snapshot.decision_type == decision_type
+        ]
 
-    rule: AutoMaterializeRule
+        if decision_type == AutoMaterializeDecisionType.DISCARD:
+            # for the discard type, we don't have an OrAssetCondition
+            if len(child_evaluations) != 1:
+                return None
+            evaluation = child_evaluations[0]
+        else:
+            unique_id_parts = [
+                OrAssetCondition.__name__,
+                *[e.condition_snapshot.unique_id for e in child_evaluations],
+            ]
+            unique_id = non_secure_md5_hash_str("".join(unique_id_parts).encode())
+            decision_type_snapshot = AssetConditionSnapshot(
+                class_name=OrAssetCondition.__name__, description="Any of", unique_id=unique_id
+            )
+            true_subset = AssetSubset.empty(asset_key, self.partitions_def)
+            for e in child_evaluations:
+                true_subset |= e.true_subset
+            evaluation = AssetConditionEvaluation(
+                condition_snapshot=decision_type_snapshot,
+                true_subset=true_subset,
+                candidate_subset=HistoricalAllPartitionsSubsetSentinel()
+                if is_partitioned
+                else AssetSubset.all(asset_key, None),
+                subsets_with_metadata=[],
+                child_evaluations=child_evaluations,
+                start_timestamp=None,
+                end_timestamp=None,
+            )
 
-    @property
-    def unique_id(self) -> str:
-        parts = [self.rule.__class__.__name__, self.description]
-        return non_secure_md5_hash_str("".join(parts).encode())
+        if decision_type == AutoMaterializeDecisionType.MATERIALIZE:
+            return evaluation
 
-    @property
-    def description(self) -> str:
-        return self.rule.description
+        # non-materialize conditions are inverted
+        unique_id_parts = [
+            NotAssetCondition.__name__,
+            evaluation.condition_snapshot.unique_id,
+        ]
+        unique_id = non_secure_md5_hash_str("".join(unique_id_parts).encode())
 
-    def evaluate(self, context: "AssetConditionEvaluationContext") -> "AssetConditionResult":
-        context.root_context.daemon_context.logger.debug(
-            f"Evaluating rule: {self.rule.to_snapshot()}"
+        if is_partitioned:
+            # In reality, we'd like to invert the inner true_subset here, but this is an
+            # expensive operation, and error-prone as the set of all partitions may have changed
+            # since the evaluation was stored. Instead, we just use an empty subset.
+            true_subset = AssetSubset.empty(asset_key, self.partitions_def)
+        else:
+            true_subset = evaluation.true_subset.copy(
+                update={"value": not evaluation.true_subset.bool_value}
+            )
+        return AssetConditionEvaluation(
+            condition_snapshot=AssetConditionSnapshot(
+                class_name=NotAssetCondition.__name__, description="Not", unique_id=unique_id
+            ),
+            true_subset=true_subset,
+            candidate_subset=HistoricalAllPartitionsSubsetSentinel()
+            if is_partitioned
+            else AssetSubset.all(asset_key, None),
+            subsets_with_metadata=[],
+            child_evaluations=[evaluation],
+            start_timestamp=None,
+            end_timestamp=None,
+        )
+
+    def unpack(
+        self,
+        unpacked_dict: Dict[str, UnpackedValue],
+        whitelist_map: WhitelistMap,
+        context: UnpackContext,
+    ) -> "AssetConditionEvaluationWithRunIds":
+        from .declarative_scheduling.operators.boolean_operators import AndAssetCondition
+        from .declarative_scheduling.serialized_objects import (
+            HistoricalAllPartitionsSubsetSentinel,
+        )
+
+        asset_key = cast(AssetKey, unpacked_dict.get("asset_key"))
+        partition_subsets_by_condition = cast(
+            Sequence[Tuple[AutoMaterializeRuleEvaluation, Optional[SerializedPartitionsSubset]]],
+            unpacked_dict.get("partition_subsets_by_condition"),
+        )
+        rule_snapshots = (
+            cast(Sequence[AutoMaterializeRuleSnapshot], unpacked_dict.get("rule_snapshots", []))
+            or []
+        )
+        is_partitioned = (
+            any(tup[1] is not None for tup in partition_subsets_by_condition)
+            if partition_subsets_by_condition
+            # if we don't have any partition_subsets_by_condition to look at, we can't tell if this
+            # asset was partitioned at the time that the evaluation was stored, so instead we assume
+            # that its current partition status is the same as its partition status at storage time.
+            else self.partitions_def is not None
+        )
+
+        # get the sub-evaluations for each decision type
+        materialize_evaluation = check.not_none(
+            self._get_child_decision_type_evaluation(
+                asset_key,
+                partition_subsets_by_condition,
+                rule_snapshots,
+                is_partitioned,
+                AutoMaterializeDecisionType.MATERIALIZE,
+            )
         )
-        evaluation_result = self.rule.evaluate_for_asset(context)
-        context.root_context.daemon_context.logger.debug(
-            f"Rule returned {evaluation_result.true_subset.size} partitions "
-            f"({evaluation_result.end_timestamp - evaluation_result.start_timestamp:.2f} seconds)"
+        not_skip_evaluation = self._get_child_decision_type_evaluation(
+            asset_key,
+            partition_subsets_by_condition,
+            rule_snapshots,
+            is_partitioned,
+            AutoMaterializeDecisionType.SKIP,
+        )
+        not_discard_evaluation = self._get_child_decision_type_evaluation(
+            asset_key,
+            partition_subsets_by_condition,
+            rule_snapshots,
+            is_partitioned,
+            AutoMaterializeDecisionType.DISCARD,
+        )
+
+        # filter out any None evaluations (should realistically only happen for discard)
+        child_evaluations = list(
+            filter(None, [materialize_evaluation, not_skip_evaluation, not_discard_evaluation])
+        )
+
+        # the top level condition is the AND of all the sub-conditions
+        unique_id_parts = [
+            AndAssetCondition.__name__,
+            *[e.condition_snapshot.unique_id for e in child_evaluations],
+        ]
+        unique_id = non_secure_md5_hash_str("".join(unique_id_parts).encode())
+        condition_snapshot = AssetConditionSnapshot(
+            class_name=AndAssetCondition.__name__, description="All of", unique_id=unique_id
         )
-        return evaluation_result
-
 
-@experimental
-@whitelist_for_serdes
-class AndAssetCondition(AssetCondition):
-    """This class represents the condition that all of its children evaluate to true."""
+        # all AssetSubsets generated here are created using the current partitions_def, so they
+        # will be valid
+        true_subset = materialize_evaluation.true_subset.as_valid(self.partitions_def)
+        if not_skip_evaluation:
+            true_subset -= not_skip_evaluation.child_evaluations[0].true_subset
+        if not_discard_evaluation:
+            true_subset -= not_discard_evaluation.child_evaluations[0].true_subset
 
-    operands: Sequence[AssetCondition]
+        return AssetConditionEvaluation(
+            condition_snapshot=condition_snapshot,
+            true_subset=true_subset,
+            candidate_subset=HistoricalAllPartitionsSubsetSentinel()
+            if is_partitioned
+            else AssetSubset.all(asset_key, None),
+            subsets_with_metadata=[],
+            child_evaluations=child_evaluations,
+            start_timestamp=None,
+            end_timestamp=None,
+        ).with_run_ids(cast(AbstractSet[str], unpacked_dict.get("run_ids", set())))
 
-    @property
-    def children(self) -> Sequence[AssetCondition]:
-        return self.operands
 
-    @property
-    def description(self) -> str:
-        return "All of"
+class BackcompatAutoMaterializeConditionSerializer(NamedTupleSerializer):
+    """This handles backcompat for the old AutoMaterializeCondition objects, turning them into the
+    proper AutoMaterializeRuleEvaluation objects. This is necessary because old
+    AutoMaterializeAssetEvaluation objects will have serialized AutoMaterializeCondition objects,
+    and we need to be able to deserialize them.
 
-    def evaluate(self, context: "AssetConditionEvaluationContext") -> "AssetConditionResult":
-        child_results: List[AssetConditionResult] = []
-        true_subset = context.candidate_subset
-        for child in self.children:
-            child_context = context.for_child(condition=child, candidate_subset=true_subset)
-            child_result = child.evaluate(child_context)
-            child_results.append(child_result)
-            true_subset &= child_result.true_subset
-        return AssetConditionResult.create_from_children(context, true_subset, child_results)
+    In theory, as these serialized objects happen to be purged periodically, we can remove this
+    backcompat logic at some point in the future.
+    """
 
+    def unpack(
+        self,
+        unpacked_dict: Dict[str, UnpackedValue],
+        whitelist_map: WhitelistMap,
+        context: UnpackContext,
+    ) -> AutoMaterializeRuleEvaluation:
+        from .auto_materialize_rule import AutoMaterializeRule
+        from .auto_materialize_rule_impls import DiscardOnMaxMaterializationsExceededRule
+
+        if self.klass in (
+            FreshnessAutoMaterializeCondition,
+            DownstreamFreshnessAutoMaterializeCondition,
+        ):
+            return AutoMaterializeRuleEvaluation(
+                rule_snapshot=AutoMaterializeRule.materialize_on_required_for_freshness().to_snapshot(),
+                evaluation_data=None,
+            )
+        elif self.klass == MissingAutoMaterializeCondition:
+            return AutoMaterializeRuleEvaluation(
+                rule_snapshot=AutoMaterializeRule.materialize_on_missing().to_snapshot(),
+                evaluation_data=None,
+            )
+        elif self.klass == ParentMaterializedAutoMaterializeCondition:
+            updated_asset_keys = unpacked_dict.get("updated_asset_keys")
+            if isinstance(updated_asset_keys, set):
+                updated_asset_keys = cast(FrozenSet[AssetKey], frozenset(updated_asset_keys))
+            else:
+                updated_asset_keys = frozenset()
+            will_update_asset_keys = unpacked_dict.get("will_update_asset_keys")
+            if isinstance(will_update_asset_keys, set):
+                will_update_asset_keys = cast(
+                    FrozenSet[AssetKey], frozenset(will_update_asset_keys)
+                )
+            else:
+                will_update_asset_keys = frozenset()
+            return AutoMaterializeRuleEvaluation(
+                rule_snapshot=AutoMaterializeRule.materialize_on_parent_updated().to_snapshot(),
+                evaluation_data=ParentUpdatedRuleEvaluationData(
+                    updated_asset_keys=updated_asset_keys,
+                    will_update_asset_keys=will_update_asset_keys,
+                ),
+            )
+        elif self.klass == ParentOutdatedAutoMaterializeCondition:
+            waiting_on_asset_keys = unpacked_dict.get("waiting_on_asset_keys")
+            if isinstance(waiting_on_asset_keys, set):
+                waiting_on_asset_keys = cast(FrozenSet[AssetKey], frozenset(waiting_on_asset_keys))
+            else:
+                waiting_on_asset_keys = frozenset()
+            return AutoMaterializeRuleEvaluation(
+                rule_snapshot=AutoMaterializeRule.skip_on_parent_outdated().to_snapshot(),
+                evaluation_data=WaitingOnAssetsRuleEvaluationData(
+                    waiting_on_asset_keys=waiting_on_asset_keys
+                ),
+            )
+        elif self.klass == MaxMaterializationsExceededAutoMaterializeCondition:
+            return AutoMaterializeRuleEvaluation(
+                rule_snapshot=DiscardOnMaxMaterializationsExceededRule(limit=1).to_snapshot(),
+                evaluation_data=None,
+            )
+        check.failed(f"Unexpected class {self.klass}")
 
-@experimental
-@whitelist_for_serdes
-class OrAssetCondition(AssetCondition):
-    """This class represents the condition that any of its children evaluate to true."""
 
-    operands: Sequence[AssetCondition]
+@whitelist_for_serdes(serializer=BackcompatAutoMaterializeConditionSerializer)
+class FreshnessAutoMaterializeCondition(NamedTuple): ...
 
-    @property
-    def children(self) -> Sequence[AssetCondition]:
-        return self.operands
 
-    @property
-    def description(self) -> str:
-        return "Any of"
+@whitelist_for_serdes(serializer=BackcompatAutoMaterializeConditionSerializer)
+class DownstreamFreshnessAutoMaterializeCondition(NamedTuple): ...
 
-    def evaluate(self, context: "AssetConditionEvaluationContext") -> "AssetConditionResult":
-        child_results: List[AssetConditionResult] = []
-        true_subset = context.empty_subset()
-        for child in self.children:
-            child_context = context.for_child(
-                condition=child, candidate_subset=context.candidate_subset
-            )
-            child_result = child.evaluate(child_context)
-            child_results.append(child_result)
-            true_subset |= child_result.true_subset
-        return AssetConditionResult.create_from_children(context, true_subset, child_results)
 
+@whitelist_for_serdes(serializer=BackcompatAutoMaterializeConditionSerializer)
+class ParentMaterializedAutoMaterializeCondition(NamedTuple): ...
 
-@experimental
-@whitelist_for_serdes
-class NotAssetCondition(AssetCondition):
-    """This class represents the condition that none of its children evaluate to true."""
 
-    operand: AssetCondition
+@whitelist_for_serdes(serializer=BackcompatAutoMaterializeConditionSerializer)
+class MissingAutoMaterializeCondition(NamedTuple): ...
 
-    @property
-    def description(self) -> str:
-        return "Not"
 
-    @property
-    def children(self) -> Sequence[AssetCondition]:
-        return [self.operand]
+@whitelist_for_serdes(serializer=BackcompatAutoMaterializeConditionSerializer)
+class ParentOutdatedAutoMaterializeCondition(NamedTuple): ...
 
-    def evaluate(self, context: "AssetConditionEvaluationContext") -> "AssetConditionResult":
-        child_context = context.for_child(
-            condition=self.operand, candidate_subset=context.candidate_subset
-        )
-        child_result = self.operand.evaluate(child_context)
-        true_subset = context.candidate_subset - child_result.true_subset
-
-        return AssetConditionResult.create_from_children(context, true_subset, [child_result])
-
-
-@dataclass(frozen=True)
-class AssetConditionResult:
-    condition: AssetCondition
-    start_timestamp: float
-    end_timestamp: float
-
-    true_subset: AssetSubset
-    candidate_subset: AssetSubset
-    subsets_with_metadata: Sequence[AssetSubsetWithMetadata]
-
-    extra_state: PackableValue
-    child_results: Sequence["AssetConditionResult"]
-
-    @staticmethod
-    def create_from_children(
-        context: "AssetConditionEvaluationContext",
-        true_subset: AssetSubset,
-        child_results: Sequence["AssetConditionResult"],
-    ) -> "AssetConditionResult":
-        """Returns a new AssetConditionEvaluation from the given child results."""
-        return AssetConditionResult(
-            condition=context.condition,
-            start_timestamp=context.start_timestamp,
-            end_timestamp=pendulum.now("UTC").timestamp(),
-            true_subset=true_subset,
-            candidate_subset=context.candidate_subset,
-            subsets_with_metadata=[],
-            child_results=child_results,
-            extra_state=None,
-        )
 
-    @staticmethod
-    def create(
-        context: "AssetConditionEvaluationContext",
-        true_subset: AssetSubset,
-        subsets_with_metadata: Sequence[AssetSubsetWithMetadata] = [],
-        extra_state: PackableValue = None,
-    ) -> "AssetConditionResult":
-        """Returns a new AssetConditionEvaluation from the given parameters."""
-        return AssetConditionResult(
-            condition=context.condition,
-            start_timestamp=context.start_timestamp,
-            end_timestamp=pendulum.now("UTC").timestamp(),
-            true_subset=true_subset,
-            candidate_subset=context.candidate_subset,
-            subsets_with_metadata=subsets_with_metadata,
-            child_results=[],
-            extra_state=extra_state,
-        )
+@whitelist_for_serdes(serializer=BackcompatAutoMaterializeConditionSerializer)
+class MaxMaterializationsExceededAutoMaterializeCondition(NamedTuple): ...
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py` & `dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,36 +15,37 @@
     Sequence,
     Tuple,
     TypeVar,
 )
 
 import pendulum
 
-from dagster._core.definitions.asset_condition.asset_condition import (
+from dagster._core.definitions.declarative_scheduling.serialized_objects import (
     HistoricalAllPartitionsSubsetSentinel,
 )
-from dagster._core.definitions.data_time import CachingDataTimeResolver
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.metadata import MetadataValue
 from dagster._core.definitions.partition import PartitionsDefinition
 from dagster._core.definitions.partition_mapping import IdentityPartitionMapping
 from dagster._core.definitions.time_window_partition_mapping import TimeWindowPartitionMapping
-from dagster._utils.caching_instance_queryer import CachingInstanceQueryer
 
-from ..asset_subset import AssetSubset, ValidAssetSubset
-from ..base_asset_graph import BaseAssetGraph
+from ...asset_subset import AssetSubset, ValidAssetSubset
+from ..serialized_objects import (
+    AssetConditionEvaluation,
+    AssetConditionEvaluationState,
+    AssetSubsetWithMetadata,
+)
 
 if TYPE_CHECKING:
-    from ..asset_daemon_context import AssetDaemonContext
-    from .asset_condition import (
-        AssetCondition,
-        AssetConditionEvaluation,
-        AssetConditionEvaluationState,
-        AssetSubsetWithMetadata,
-    )
+    from dagster._core.definitions.data_time import CachingDataTimeResolver
+    from dagster._utils.caching_instance_queryer import CachingInstanceQueryer
+
+    from ...asset_daemon_context import AssetDaemonContext
+    from ...base_asset_graph import BaseAssetGraph
+    from ..scheduling_condition import SchedulingCondition
 
 T = TypeVar("T")
 
 
 def root_property(fn: Callable[[Any], T]) -> Callable[[Any], T]:
     """Ensures that a given property is always accessed via the root context, ensuring that any
     cached properties are accessed correctly.
@@ -53,49 +54,49 @@
     def wrapped(self: Any) -> Any:
         return fn(self.root_context)
 
     return wrapped
 
 
 @dataclass(frozen=True)
-class AssetConditionEvaluationContext:
+class LegacyRuleEvaluationContext:
     """Context object containing methods and properties used for evaluating the entire state of an
     asset's automation rules.
     """
 
     asset_key: AssetKey
-    condition: "AssetCondition"
-    previous_evaluation_state: Optional["AssetConditionEvaluationState"]
-    previous_evaluation: Optional["AssetConditionEvaluation"]
+    condition: "SchedulingCondition"
+    previous_evaluation_state: Optional[AssetConditionEvaluationState]
+    previous_evaluation: Optional[AssetConditionEvaluation]
     candidate_subset: ValidAssetSubset
 
-    instance_queryer: CachingInstanceQueryer
-    data_time_resolver: CachingDataTimeResolver
+    instance_queryer: "CachingInstanceQueryer"
+    data_time_resolver: "CachingDataTimeResolver"
     daemon_context: "AssetDaemonContext"
 
-    evaluation_state_by_key: Mapping[AssetKey, "AssetConditionEvaluationState"]
+    evaluation_state_by_key: Mapping[AssetKey, AssetConditionEvaluationState]
     expected_data_time_mapping: Mapping[AssetKey, Optional[datetime.datetime]]
 
     start_timestamp: float
-    root_ref: Optional["AssetConditionEvaluationContext"] = None
+    root_ref: Optional["LegacyRuleEvaluationContext"] = None
 
     @staticmethod
     def create(
         asset_key: AssetKey,
-        condition: "AssetCondition",
-        previous_evaluation_state: Optional["AssetConditionEvaluationState"],
-        instance_queryer: CachingInstanceQueryer,
-        data_time_resolver: CachingDataTimeResolver,
+        condition: "SchedulingCondition",
+        previous_evaluation_state: Optional[AssetConditionEvaluationState],
+        instance_queryer: "CachingInstanceQueryer",
+        data_time_resolver: "CachingDataTimeResolver",
         daemon_context: "AssetDaemonContext",
-        evaluation_state_by_key: Mapping[AssetKey, "AssetConditionEvaluationState"],
+        evaluation_state_by_key: Mapping[AssetKey, AssetConditionEvaluationState],
         expected_data_time_mapping: Mapping[AssetKey, Optional[datetime.datetime]],
-    ) -> "AssetConditionEvaluationContext":
+    ) -> "LegacyRuleEvaluationContext":
         partitions_def = instance_queryer.asset_graph.get(asset_key).partitions_def
 
-        return AssetConditionEvaluationContext(
+        return LegacyRuleEvaluationContext(
             asset_key=asset_key,
             condition=condition,
             previous_evaluation_state=previous_evaluation_state,
             previous_evaluation=previous_evaluation_state.previous_evaluation
             if previous_evaluation_state
             else None,
             candidate_subset=AssetSubset.all(
@@ -109,34 +110,37 @@
             daemon_context=daemon_context,
             evaluation_state_by_key=evaluation_state_by_key,
             expected_data_time_mapping=expected_data_time_mapping,
             start_timestamp=pendulum.now("UTC").timestamp(),
         )
 
     def for_child(
-        self, condition: "AssetCondition", candidate_subset: AssetSubset
-    ) -> "AssetConditionEvaluationContext":
+        self,
+        child_condition: "SchedulingCondition",
+        child_unique_id: str,
+        candidate_subset: AssetSubset,
+    ) -> "LegacyRuleEvaluationContext":
         return dataclasses.replace(
             self,
-            condition=condition,
-            previous_evaluation=self.previous_evaluation.for_child(condition)
+            condition=child_condition,
+            previous_evaluation=self.previous_evaluation.for_child(child_unique_id)
             if self.previous_evaluation
             else None,
             candidate_subset=candidate_subset,
             root_ref=self.root_context,
             start_timestamp=pendulum.now("UTC").timestamp(),
         )
 
     @property
-    def root_context(self) -> "AssetConditionEvaluationContext":
+    def root_context(self) -> "LegacyRuleEvaluationContext":
         """A reference to the context of the root condition for this evaluation."""
         return self.root_ref or self
 
     @property
-    def asset_graph(self) -> BaseAssetGraph:
+    def asset_graph(self) -> "BaseAssetGraph":
         return self.instance_queryer.asset_graph
 
     @property
     def partitions_def(self) -> Optional[PartitionsDefinition]:
         return self.asset_graph.get(self.asset_key).partitions_def
 
     @property
@@ -175,15 +179,15 @@
             return AssetSubset.all(
                 self.asset_key, self.partitions_def, self.instance_queryer, self.evaluation_time
             )
         else:
             return candidate_subset
 
     @property
-    def previous_subsets_with_metadata(self) -> Sequence["AssetSubsetWithMetadata"]:
+    def previous_subsets_with_metadata(self) -> Sequence[AssetSubsetWithMetadata]:
         if self.previous_evaluation is None:
             return []
         return self.previous_evaluation.subsets_with_metadata
 
     @functools.cached_property
     @root_property
     def parent_will_update_subset(self) -> ValidAssetSubset:
@@ -286,15 +290,15 @@
         return self.candidate_subset & self.parent_has_or_will_update_subset
 
     @property
     def candidates_not_evaluated_on_previous_tick_subset(self) -> ValidAssetSubset:
         """Returns the set of candidates for this tick which were not candidates on the previous
         tick.
         """
-        from .asset_condition import HistoricalAllPartitionsSubsetSentinel
+        from ..serialized_objects import HistoricalAllPartitionsSubsetSentinel
 
         if not self.previous_evaluation:
             return self.candidate_subset
         # when the candidate_subset is HistoricalAllPartitionsSubsetSentinel, this indicates that the
         # entire asset was evaluated for this condition on the previous tick, and so no candidates
         # were *not* evaluated on the previous tick
         elif isinstance(
@@ -357,25 +361,25 @@
 
     def add_evaluation_data_from_previous_tick(
         self,
         asset_partitions_by_frozen_metadata: Mapping[
             FrozenSet[Tuple[str, MetadataValue]], AbstractSet[AssetKeyPartitionKey]
         ],
         ignore_subset: AssetSubset,
-    ) -> Tuple[AssetSubset, Sequence["AssetSubsetWithMetadata"]]:
+    ) -> Tuple[ValidAssetSubset, Sequence[AssetSubsetWithMetadata]]:
         """Combines information calculated on this tick with information from the previous tick,
         returning a tuple of the combined true subset and the combined subsets with metadata.
 
         Args:
             asset_partitions_by_frozen_metadata: A mapping from metadata to the set of asset
                 partitions that the rule applies to.
             ignore_subset: An AssetSubset which represents information that we should *not* carry
                 forward from the previous tick.
         """
-        from .asset_condition import AssetSubsetWithMetadata
+        from ..serialized_objects import AssetSubsetWithMetadata
 
         mapping = defaultdict(lambda: self.empty_subset())
         has_new_metadata_subset = self.empty_subset()
         for frozen_metadata, asset_partitions in asset_partitions_by_frozen_metadata.items():
             mapping[frozen_metadata] = AssetSubset.from_asset_partitions_set(
                 self.asset_key, self.partitions_def, asset_partitions
             )
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_daemon_context.py` & `dagster-1.7.5/dagster/_core/definitions/asset_daemon_context.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,33 +18,44 @@
     Tuple,
     cast,
 )
 
 import pendulum
 
 import dagster._check as check
+from dagster._core.asset_graph_view.asset_graph_view import AssetGraphView, TemporalContext
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.data_time import CachingDataTimeResolver
+from dagster._core.definitions.data_version import CachingStaleStatusResolver
+from dagster._core.definitions.declarative_scheduling.scheduling_context import (
+    SchedulingContext,
+)
+from dagster._core.definitions.declarative_scheduling.scheduling_evaluation_info import (
+    SchedulingEvaluationInfo,
+)
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.run_request import RunRequest
 from dagster._core.definitions.time_window_partitions import (
     get_time_partitions_def,
 )
 from dagster._core.instance import DynamicPartitionsStore
 
 from ... import PartitionKeyRange
 from ..storage.tags import ASSET_PARTITION_RANGE_END_TAG, ASSET_PARTITION_RANGE_START_TAG
-from .asset_condition.asset_condition import AssetConditionEvaluation, AssetConditionEvaluationState
-from .asset_condition.asset_condition_evaluation_context import (
-    AssetConditionEvaluationContext,
-)
 from .asset_daemon_cursor import AssetDaemonCursor
 from .auto_materialize_rule import AutoMaterializeRule
 from .backfill_policy import BackfillPolicy, BackfillPolicyType
 from .base_asset_graph import BaseAssetGraph
+from .declarative_scheduling.legacy.legacy_context import (
+    LegacyRuleEvaluationContext,
+)
+from .declarative_scheduling.serialized_objects import (
+    AssetConditionEvaluation,
+    AssetConditionEvaluationState,
+)
 from .freshness_based_auto_materialize import get_expected_data_time_for_asset_key
 from .partition import PartitionsDefinition, ScheduleType
 
 if TYPE_CHECKING:
     from dagster._core.instance import DagsterInstance
     from dagster._utils.caching_instance_queryer import CachingInstanceQueryer  # expensive import
 
@@ -97,14 +108,27 @@
         from dagster._utils.caching_instance_queryer import CachingInstanceQueryer
 
         self._evaluation_id = evaluation_id
         self._instance_queryer = CachingInstanceQueryer(
             instance, asset_graph, evaluation_time=evaluation_time, logger=logger
         )
         self._data_time_resolver = CachingDataTimeResolver(self.instance_queryer)
+
+        stale_resolver = CachingStaleStatusResolver(
+            instance=instance, asset_graph=asset_graph, instance_queryer=self.instance_queryer
+        )
+        self._asset_graph_view = AssetGraphView(
+            temporal_context=TemporalContext(
+                effective_dt=self.instance_queryer.evaluation_time,
+                # TODO: we should eventually pass in an explicit last_event_id
+                last_event_id=None,
+            ),
+            stale_resolver=stale_resolver,
+        )
+        self._data_time_resolver = CachingDataTimeResolver(self.instance_queryer)
         self._cursor = cursor
         self._auto_materialize_asset_keys = auto_materialize_asset_keys or set()
         self._materialize_run_tags = materialize_run_tags
         self._observe_run_tags = observe_run_tags
         self._auto_observe_asset_keys = auto_observe_asset_keys or set()
         self._respect_materialization_data_versions = respect_materialization_data_versions
         self._logger = logger
@@ -121,14 +145,18 @@
         return self._instance_queryer
 
     @property
     def data_time_resolver(self) -> CachingDataTimeResolver:
         return self._data_time_resolver
 
     @property
+    def asset_graph_view(self) -> AssetGraphView:
+        return self._asset_graph_view
+
+    @property
     def cursor(self) -> AssetDaemonCursor:
         return self._cursor
 
     @property
     def asset_graph(self) -> BaseAssetGraph:
         return self.instance_queryer.asset_graph
 
@@ -171,14 +199,15 @@
         self._logger.info("Done prefetching asset records.")
 
     def evaluate_asset(
         self,
         asset_key: AssetKey,
         evaluation_state_by_key: Mapping[AssetKey, AssetConditionEvaluationState],
         expected_data_time_mapping: Mapping[AssetKey, Optional[datetime.datetime]],
+        current_evaluation_info_by_key: Mapping[AssetKey, SchedulingEvaluationInfo],
     ) -> Tuple[AssetConditionEvaluationState, Optional[datetime.datetime]]:
         """Evaluates the auto materialize policy of a given asset key.
 
         Params:
             - asset_key: The asset key to evaluate.
             - will_materialize_mapping: A mapping of AssetKey to the set of AssetKeyPartitionKeys
                 that will be materialized this tick. As this function is called in topological order,
@@ -187,44 +216,58 @@
                 asset after this tick. As this function is called in topological order, this mapping
                 will contain the expected data times of all upstream assets.
 
         """
         # convert the legacy AutoMaterializePolicy to an Evaluator
         asset_condition = check.not_none(
             self.asset_graph.get(asset_key).auto_materialize_policy
-        ).to_asset_condition()
+        ).to_scheduling_condition()
 
-        asset_cursor = self.cursor.get_previous_evaluation_state(asset_key)
+        previous_evaluation_state = self.cursor.get_previous_evaluation_state(asset_key)
 
-        context = AssetConditionEvaluationContext.create(
+        legacy_context = LegacyRuleEvaluationContext.create(
             asset_key=asset_key,
-            previous_evaluation_state=asset_cursor,
+            previous_evaluation_state=previous_evaluation_state,
             condition=asset_condition,
             instance_queryer=self.instance_queryer,
             data_time_resolver=self.data_time_resolver,
             daemon_context=self,
             evaluation_state_by_key=evaluation_state_by_key,
             expected_data_time_mapping=expected_data_time_mapping,
         )
 
+        context = SchedulingContext.create(
+            asset_key=asset_key,
+            asset_graph_view=self.asset_graph_view,
+            logger=self.logger,
+            current_tick_evaluation_info_by_key=current_evaluation_info_by_key,
+            previous_evaluation_info=SchedulingEvaluationInfo.from_asset_condition_evaluation_state(
+                self.asset_graph_view, previous_evaluation_state
+            )
+            if previous_evaluation_state
+            else None,
+            legacy_context=legacy_context,
+        )
+
         result = asset_condition.evaluate(context)
 
         expected_data_time = get_expected_data_time_for_asset_key(
-            context, will_materialize=result.true_subset.size > 0
+            legacy_context, will_materialize=result.true_subset.size > 0
         )
         return AssetConditionEvaluationState.create(context, result), expected_data_time
 
     def get_asset_condition_evaluations(
         self,
     ) -> Tuple[Sequence[AssetConditionEvaluationState], AbstractSet[AssetKeyPartitionKey]]:
         """Returns a mapping from asset key to the AutoMaterializeAssetEvaluation for that key, a
         sequence of new per-asset cursors, and the set of all asset partitions that should be
         materialized or discarded this tick.
         """
         evaluation_state_by_key: Dict[AssetKey, AssetConditionEvaluationState] = {}
+        current_evaluation_info_by_key: Dict[AssetKey, SchedulingEvaluationInfo] = {}
         expected_data_time_mapping: Dict[AssetKey, Optional[datetime.datetime]] = defaultdict()
         to_request: Set[AssetKeyPartitionKey] = set()
 
         num_checked_assets = 0
         num_auto_materialize_asset_keys = len(self.auto_materialize_asset_keys)
 
         for asset_key in self.asset_graph.toposorted_asset_keys:
@@ -237,15 +280,18 @@
             self._logger.debug(
                 "Evaluating asset"
                 f" {asset_key.to_user_string()} ({num_checked_assets}/{num_auto_materialize_asset_keys})"
             )
 
             try:
                 (evaluation_state, expected_data_time) = self.evaluate_asset(
-                    asset_key, evaluation_state_by_key, expected_data_time_mapping
+                    asset_key,
+                    evaluation_state_by_key,
+                    expected_data_time_mapping,
+                    current_evaluation_info_by_key,
                 )
             except Exception as e:
                 raise Exception(
                     f"Error while evaluating conditions for asset {asset_key.to_user_string()}"
                 ) from e
 
             num_requested = evaluation_state.true_subset.size
@@ -259,14 +305,19 @@
 
             log_fn(
                 f"Asset {asset_key.to_user_string()} evaluation result: {num_requested}"
                 f" requested ({to_request_str}) ({format(time.time()-start_time, '.3f')} seconds)"
             )
 
             evaluation_state_by_key[asset_key] = evaluation_state
+            current_evaluation_info_by_key[asset_key] = (
+                SchedulingEvaluationInfo.from_asset_condition_evaluation_state(
+                    self.asset_graph_view, evaluation_state
+                )
+            )
             expected_data_time_mapping[asset_key] = expected_data_time
 
             # if we need to materialize any partitions of a non-subsettable multi-asset, we need to
             # materialize all of them
             execution_set_keys = self.asset_graph.get(asset_key).execution_set_asset_keys
             if len(execution_set_keys) > 1 and num_requested > 0:
                 for neighbor_key in execution_set_keys:
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_daemon_cursor.py` & `dagster-1.7.5/dagster/_core/definitions/asset_daemon_cursor.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,19 +22,21 @@
     WhitelistMap,
     pack_value,
     unpack_value,
     whitelist_for_serdes,
 )
 
 from .base_asset_graph import BaseAssetGraph
+from .declarative_scheduling.serialized_objects import (
+    AssetConditionEvaluation,
+    AssetConditionEvaluationState,
+)
 
 if TYPE_CHECKING:
-    from .asset_condition.asset_condition import (
-        AssetConditionEvaluation,
-        AssetConditionEvaluationState,
+    from .declarative_scheduling.serialized_objects import (
         AssetConditionSnapshot,
     )
 
 
 @whitelist_for_serdes
 class AssetConditionCursorExtras(NamedTuple):
     """Represents additional state that may be optionally saved by an AssetCondition between
@@ -144,43 +146,47 @@
 def get_backcompat_asset_condition_evaluation_state(
     latest_evaluation: "AssetConditionEvaluation",
     latest_storage_id: Optional[int],
     latest_timestamp: Optional[float],
     handled_root_subset: Optional[AssetSubset],
 ) -> "AssetConditionEvaluationState":
     """Generates an AssetDaemonCursor from information available on the old cursor format."""
-    from dagster._core.definitions.asset_condition.asset_condition import (
-        AssetConditionEvaluationState,
+    from dagster._core.definitions.auto_materialize_rule_impls import MaterializeOnMissingRule
+    from dagster._core.definitions.declarative_scheduling.legacy.rule_condition import (
         RuleCondition,
     )
-    from dagster._core.definitions.auto_materialize_rule_impls import MaterializeOnMissingRule
+    from dagster._core.definitions.declarative_scheduling.serialized_objects import (
+        AssetConditionEvaluationState,
+    )
 
     return AssetConditionEvaluationState(
         previous_evaluation=latest_evaluation,
         previous_tick_evaluation_timestamp=latest_timestamp,
         max_storage_id=latest_storage_id,
         # the only information we need to preserve from the previous cursor is the handled subset
         extra_state_by_unique_id={
-            RuleCondition(rule=MaterializeOnMissingRule()).unique_id: handled_root_subset,
+            RuleCondition(rule=MaterializeOnMissingRule()).get_unique_id(None): handled_root_subset,
         }
         if handled_root_subset and handled_root_subset.size > 0
         else {},
     )
 
 
 def backcompat_deserialize_asset_daemon_cursor_str(
     cursor_str: str, asset_graph: Optional[BaseAssetGraph], default_evaluation_id: int
 ) -> AssetDaemonCursor:
     """This serves as a backcompat layer for deserializing the old cursor format. Some information
     is impossible to fully recover, this will recover enough to continue operating as normal.
     """
-    from .asset_condition.asset_condition import AssetConditionEvaluation, AssetConditionSnapshot
     from .auto_materialize_rule_evaluation import (
         deserialize_auto_materialize_asset_evaluation_to_asset_condition_evaluation_with_run_ids,
     )
+    from .declarative_scheduling.serialized_objects import (
+        AssetConditionSnapshot,
+    )
 
     data = json.loads(cursor_str)
 
     if isinstance(data, list):
         evaluation_id = data[0] if isinstance(data[0], int) else default_evaluation_id
         return AssetDaemonCursor.empty(evaluation_id)
     elif not isinstance(data, dict):
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_dep.py` & `dagster-1.7.5/dagster/_core/definitions/asset_dep.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_graph.py` & `dagster-1.7.5/dagster/_core/definitions/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_graph_differ.py` & `dagster-1.7.5/dagster/_core/definitions/asset_graph_differ.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.7.5/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_in.py` & `dagster-1.7.5/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_job.py` & `dagster-1.7.5/dagster/_core/definitions/asset_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_key.py` & `dagster-1.7.5/dagster/_core/definitions/asset_key.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,22 +53,18 @@
     def __repr__(self):
         return f"AssetKey({self.path})"
 
     def __hash__(self):
         return hash(tuple(self.path))
 
     def __eq__(self, other):
-        if not isinstance(other, AssetKey):
+        if other.__class__ is not self.__class__:
             return False
-        if len(self.path) != len(other.path):
-            return False
-        for i in range(0, len(self.path)):
-            if self.path[i] != other.path[i]:
-                return False
-        return True
+
+        return self.path == other.path
 
     def to_string(self) -> str:
         """E.g. '["first_component", "second_component"]'."""
         return seven.json.dumps(self.path)
 
     def to_user_string(self) -> str:
         """E.g. "first_component/second_component"."""
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_layer.py` & `dagster-1.7.5/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_out.py` & `dagster-1.7.5/dagster/_core/definitions/asset_out.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._core.definitions.input import NoValueSentinel
 from dagster._core.definitions.output import Out
 from dagster._core.definitions.utils import DEFAULT_IO_MANAGER_KEY
 from dagster._core.types.dagster_type import DagsterType, resolve_dagster_type
 
-from .utils import validate_definition_tags
+from .utils import validate_tags_strict
 
 
 @experimental_param(param="owners")
 @experimental_param(param="tags")
 class AssetOut(
     NamedTuple(
         "_AssetOut",
@@ -119,15 +119,15 @@
             auto_materialize_policy=check.opt_inst_param(
                 auto_materialize_policy, "auto_materialize_policy", AutoMaterializePolicy
             ),
             backfill_policy=check.opt_inst_param(
                 backfill_policy, "backfill_policy", BackfillPolicy
             ),
             owners=check.opt_sequence_param(owners, "owners", of_type=str),
-            tags=validate_definition_tags(tags),
+            tags=validate_tags_strict(tags),
         )
 
     def to_out(self) -> Out:
         return Out(
             dagster_type=self.dagster_type,
             description=self.description,
             metadata=self.metadata,
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_selection.py` & `dagster-1.7.5/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.7.5/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_spec.py` & `dagster-1.7.5/dagster/_core/definitions/asset_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from .auto_materialize_policy import AutoMaterializePolicy
 from .events import (
     AssetKey,
     CoercibleToAssetKey,
 )
 from .freshness_policy import FreshnessPolicy
-from .utils import validate_definition_tags
+from .utils import validate_tags_strict
 
 if TYPE_CHECKING:
     from dagster._core.definitions.asset_dep import AssetDep, CoercibleToAssetDep
 
 # SYSTEM_METADATA_KEY_ASSET_EXECUTION_TYPE lives on the metadata of an asset
 # (which currently ends up on the Output associated with the asset key)
 # whih encodes the execution type the of asset. "Unexecutable" assets are assets
@@ -139,9 +139,9 @@
             ),
             auto_materialize_policy=check.opt_inst_param(
                 auto_materialize_policy,
                 "auto_materialize_policy",
                 AutoMaterializePolicy,
             ),
             owners=check.opt_sequence_param(owners, "owners", of_type=str),
-            tags=validate_definition_tags(tags),
+            tags=validate_tags_strict(tags),
         )
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/asset_subset.py` & `dagster-1.7.5/dagster/_core/definitions/asset_subset.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,38 +81,45 @@
     @property
     def size(self) -> int:
         if not self.is_partitioned:
             return int(self.bool_value)
         else:
             return len(self.subset_value)
 
-    def _is_compatible_with_partitions_def(
+    @property
+    def is_empty(self) -> bool:
+        # avoid calculating the full size of the subset if it's an AllPartitionsSubset
+        if isinstance(self.value, AllPartitionsSubset):
+            return False
+        return self.size == 0
+
+    def is_compatible_with_partitions_def(
         self, partitions_def: Optional[PartitionsDefinition]
     ) -> bool:
         if self.is_partitioned:
             # for some PartitionSubset types, we have access to the underlying partitions
             # definitions, so we can ensure those are identical
             if isinstance(self.value, (BaseTimeWindowPartitionsSubset, AllPartitionsSubset)):
                 return self.value.partitions_def == partitions_def
             else:
                 return partitions_def is not None
         else:
             return partitions_def is None
 
     def _is_compatible_with_subset(self, other: "AssetSubset") -> bool:
         if isinstance(other.value, (BaseTimeWindowPartitionsSubset, AllPartitionsSubset)):
-            return self._is_compatible_with_partitions_def(other.value.partitions_def)
+            return self.is_compatible_with_partitions_def(other.value.partitions_def)
         else:
             return self.is_partitioned == other.is_partitioned
 
     def as_valid(self, partitions_def: Optional[PartitionsDefinition]) -> "ValidAssetSubset":
         """Converts this AssetSubset to a ValidAssetSubset by returning a copy of this AssetSubset
         if it is compatible with the given PartitionsDefinition, otherwise returns an empty subset.
         """
-        if self._is_compatible_with_partitions_def(partitions_def):
+        if self.is_compatible_with_partitions_def(partitions_def):
             return ValidAssetSubset(asset_key=self.asset_key, value=self.value)
         else:
             return ValidAssetSubset.empty(self.asset_key, partitions_def)
 
     @staticmethod
     def all(
         asset_key: AssetKey,
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/assets.py` & `dagster-1.7.5/dagster/_core/definitions/assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Iterator,
     List,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Set,
+    TypeVar,
     Union,
     cast,
 )
 
 import dagster._check as check
 from dagster._annotations import experimental_param, public
 from dagster._core.definitions.asset_check_spec import AssetCheckKey, AssetCheckSpec
@@ -67,15 +68,15 @@
 from .partition_mapping import (
     PartitionMapping,
     get_builtin_partition_mapping_types,
     infer_partition_mapping,
 )
 from .resource_definition import ResourceDefinition
 from .source_asset import SourceAsset
-from .utils import DEFAULT_GROUP_NAME, validate_definition_tags, validate_group_name
+from .utils import DEFAULT_GROUP_NAME, validate_group_name, validate_tags_strict
 
 if TYPE_CHECKING:
     from .base_asset_graph import AssetKeyOrCheckKey
     from .graph_definition import GraphDefinition
 
 ASSET_SUBSET_INPUT_PREFIX = "__subset_input__"
 
@@ -267,15 +268,15 @@
         self._metadata_by_key = dict(
             check.opt_mapping_param(
                 metadata_by_key, "metadata_by_key", key_type=AssetKey, value_type=dict
             )
         )
 
         for tags in (tags_by_key or {}).values():
-            validate_definition_tags(tags)
+            validate_tags_strict(tags)
         self._tags_by_key = tags_by_key or {}
 
         self._descriptions_by_key = dict(
             check.opt_mapping_param(
                 descriptions_by_key, "descriptions_by_key", key_type=AssetKey, value_type=str
             )
         )
@@ -638,15 +639,15 @@
             auto_materialize_policies_by_output_name=auto_materialize_policies_by_output_name,
             backfill_policy=backfill_policy,
             can_subset=can_subset,
         )
 
     @staticmethod
     def _from_node(
-        node_def: Union[OpDefinition, "GraphDefinition"],
+        node_def: NodeDefinition,
         *,
         keys_by_input_name: Optional[Mapping[str, AssetKey]] = None,
         keys_by_output_name: Optional[Mapping[str, AssetKey]] = None,
         key_prefix: Optional[CoercibleToAssetKeyPrefix] = None,
         internal_asset_deps: Optional[Mapping[str, Set[AssetKey]]] = None,
         partitions_def: Optional[PartitionsDefinition] = None,
         partition_mappings: Optional[Mapping[str, PartitionMapping]] = None,
@@ -714,30 +715,39 @@
         for output_name, key in keys_by_output_name.items():
             # add key_prefix to the beginning of each asset key
             key_with_key_prefix = AssetKey(
                 list(filter(None, [*(key_prefix_list or []), *key.path]))
             )
             keys_by_output_name_with_prefix[output_name] = key_with_key_prefix
 
+        T = TypeVar("T")
+
+        def _output_dict_to_asset_dict(
+            attr_by_output_name: Optional[Mapping[str, Optional[T]]],
+        ) -> Optional[Mapping[AssetKey, T]]:
+            if not attr_by_output_name:
+                return None
+            return {
+                keys_by_output_name_with_prefix[output_name]: attr
+                for output_name, attr in attr_by_output_name.items()
+                if attr is not None
+            }
+
         check.param_invariant(
             group_name is None or group_names_by_output_name is None,
             "group_name",
             "Cannot use both group_name and group_names_by_output_name",
         )
 
         if group_name is not None:
             group_names_by_key = {
                 asset_key: group_name for asset_key in keys_by_output_name_with_prefix.values()
             }
         elif group_names_by_output_name:
-            group_names_by_key = {
-                keys_by_output_name_with_prefix[output_name]: group_name
-                for output_name, group_name in group_names_by_output_name.items()
-                if group_name is not None
-            }
+            group_names_by_key = _output_dict_to_asset_dict(group_names_by_output_name)
         else:
             group_names_by_key = None
 
         return AssetsDefinition.dagster_internal_init(
             keys_by_input_name=keys_by_input_name,
             keys_by_output_name=keys_by_output_name_with_prefix,
             node_def=node_def,
@@ -753,62 +763,24 @@
                 {
                     keys_by_input_name[input_name]: partition_mapping
                     for input_name, partition_mapping in partition_mappings.items()
                 }
                 if partition_mappings
                 else None
             ),
-            metadata_by_key=(
-                {
-                    keys_by_output_name_with_prefix[output_name]: metadata
-                    for output_name, metadata in metadata_by_output_name.items()
-                    if metadata is not None
-                }
-                if metadata_by_output_name
-                else None
-            ),
-            tags_by_key=(
-                {
-                    keys_by_output_name_with_prefix[output_name]: tags
-                    for output_name, tags in tags_by_output_name.items()
-                    if tags is not None
-                }
-                if tags_by_output_name
-                else None
-            ),
-            freshness_policies_by_key=(
-                {
-                    keys_by_output_name_with_prefix[output_name]: freshness_policy
-                    for output_name, freshness_policy in freshness_policies_by_output_name.items()
-                    if freshness_policy is not None
-                }
-                if freshness_policies_by_output_name
-                else None
-            ),
-            auto_materialize_policies_by_key=(
-                {
-                    keys_by_output_name_with_prefix[output_name]: auto_materialize_policy
-                    for output_name, auto_materialize_policy in auto_materialize_policies_by_output_name.items()
-                    if auto_materialize_policy is not None
-                }
-                if auto_materialize_policies_by_output_name
-                else None
+            metadata_by_key=_output_dict_to_asset_dict(metadata_by_output_name),
+            tags_by_key=_output_dict_to_asset_dict(tags_by_output_name),
+            freshness_policies_by_key=_output_dict_to_asset_dict(freshness_policies_by_output_name),
+            auto_materialize_policies_by_key=_output_dict_to_asset_dict(
+                auto_materialize_policies_by_output_name
             ),
             backfill_policy=check.opt_inst_param(
                 backfill_policy, "backfill_policy", BackfillPolicy
             ),
-            descriptions_by_key=(
-                {
-                    keys_by_output_name_with_prefix[output_name]: description
-                    for output_name, description in descriptions_by_output_name.items()
-                    if description is not None
-                }
-                if descriptions_by_output_name
-                else None
-            ),
+            descriptions_by_key=_output_dict_to_asset_dict(descriptions_by_output_name),
             can_subset=can_subset,
             selected_asset_keys=None,  # node has no subselection info
             check_specs_by_output_name=check_specs_by_output_name,
             selected_asset_check_keys=None,
             is_subset=False,
             owners_by_key=owners_by_key,
         )
@@ -1583,15 +1555,15 @@
             selected_asset_check_keys=self._selected_asset_check_keys,
             owners_by_key=self._owners_by_key,
             tags_by_key=self._tags_by_key,
         )
 
 
 def _infer_keys_by_input_names(
-    node_def: Union["GraphDefinition", OpDefinition], keys_by_input_name: Mapping[str, AssetKey]
+    node_def: NodeDefinition, keys_by_input_name: Mapping[str, AssetKey]
 ) -> Mapping[str, AssetKey]:
     all_input_names = [input_def.name for input_def in node_def.input_defs]
     if keys_by_input_name:
         check.invariant(
             set(keys_by_input_name.keys()) == set(all_input_names),
             "The set of input names keys specified in the keys_by_input_name argument must "
             f"equal the set of asset keys inputted by '{node_def.name}'. \n"
@@ -1606,15 +1578,15 @@
         for input_name in all_input_names
     }
 
     return inferred_input_names_by_asset_key
 
 
 def _infer_keys_by_output_names(
-    node_def: Union["GraphDefinition", OpDefinition],
+    node_def: NodeDefinition,
     keys_by_output_name: Mapping[str, AssetKey],
     check_specs_by_output_name: Mapping[str, AssetCheckSpec],
 ) -> Mapping[str, AssetKey]:
     output_names = [output_def.name for output_def in node_def.output_defs]
     if keys_by_output_name:
         overlapping_asset_and_check_outputs = set(keys_by_output_name.keys()) & set(
             check_specs_by_output_name.keys()
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.7.5/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from enum import Enum
-from typing import AbstractSet, Dict, FrozenSet, NamedTuple, Optional, Sequence
+from typing import TYPE_CHECKING, AbstractSet, Dict, FrozenSet, NamedTuple, Optional, Sequence
 
 import dagster._check as check
 from dagster._annotations import deprecated, experimental, public
-from dagster._core.definitions.asset_condition.asset_condition import AssetCondition
-from dagster._core.definitions.auto_materialize_rule import (
-    AutoMaterializeRule,
-    AutoMaterializeRuleSnapshot,
+from dagster._core.definitions.declarative_scheduling.scheduling_condition import (
+    SchedulingCondition,
 )
 from dagster._serdes.serdes import (
     NamedTupleSerializer,
     UnpackContext,
     UnpackedValue,
     whitelist_for_serdes,
 )
 
+if TYPE_CHECKING:
+    from dagster._core.definitions.auto_materialize_rule import (
+        AutoMaterializeRule,
+        AutoMaterializeRuleSnapshot,
+    )
+
 
 class AutoMaterializePolicySerializer(NamedTupleSerializer):
     def before_unpack(
         self, context: UnpackContext, unpacked_dict: Dict[str, UnpackedValue]
     ) -> Dict[str, UnpackedValue]:
+        from dagster._core.definitions.auto_materialize_rule import AutoMaterializeRule
+
         backcompat_map = {
             "on_missing": AutoMaterializeRule.materialize_on_missing(),
             "on_new_parent_data": AutoMaterializeRule.materialize_on_parent_updated(),
             "for_freshness": AutoMaterializeRule.materialize_on_required_for_freshness(),
         }
 
         # determine if this namedtuple was serialized with the old format (booleans for rules)
@@ -53,17 +59,17 @@
     old_fields={"time_window_partition_scope_minutes": 1e-6},
     serializer=AutoMaterializePolicySerializer,
 )
 class AutoMaterializePolicy(
     NamedTuple(
         "_AutoMaterializePolicy",
         [
-            ("rules", FrozenSet[AutoMaterializeRule]),
+            ("rules", FrozenSet["AutoMaterializeRule"]),
             ("max_materializations_per_minute", Optional[int]),
-            ("asset_condition", Optional[AssetCondition]),
+            ("asset_condition", Optional[SchedulingCondition]),
         ],
     )
 ):
     """An AutoMaterializePolicy specifies how Dagster should attempt to keep an asset up-to-date.
 
     Each policy consists of a set of AutoMaterializeRules, which are used to determine whether an
     asset or a partition of an asset should or should not be auto-materialized.
@@ -118,15 +124,15 @@
 
     """
 
     def __new__(
         cls,
         rules: AbstractSet["AutoMaterializeRule"],
         max_materializations_per_minute: Optional[int] = 1,
-        asset_condition: Optional[AssetCondition] = None,
+        asset_condition: Optional[SchedulingCondition] = None,
     ):
         from dagster._core.definitions.auto_materialize_rule import AutoMaterializeRule
 
         check.invariant(
             max_materializations_per_minute is None or max_materializations_per_minute > 0,
             "max_materializations_per_minute must be positive. To disable rate-limiting, set it"
             " to None. To disable auto materializing, remove the policy.",
@@ -165,15 +171,15 @@
         from dagster._core.definitions.auto_materialize_rule import AutoMaterializeDecisionType
 
         return {
             rule for rule in self.rules if rule.decision_type == AutoMaterializeDecisionType.SKIP
         }
 
     @staticmethod
-    def from_asset_condition(asset_condition: AssetCondition) -> "AutoMaterializePolicy":
+    def from_asset_condition(asset_condition: SchedulingCondition) -> "AutoMaterializePolicy":
         """Constructs an AutoMaterializePolicy which will materialize an asset partition whenever
         the provided asset_condition evaluates to True.
 
         Args:
             asset_condition (AssetCondition): The condition which determines whether an asset
                 partition should be materialized.
         """
@@ -277,22 +283,22 @@
             return AutoMaterializePolicyType.EAGER
         return AutoMaterializePolicyType.LAZY
 
     @property
     def rule_snapshots(self) -> Sequence["AutoMaterializeRuleSnapshot"]:
         return [rule.to_snapshot() for rule in self.rules]
 
-    def to_asset_condition(self) -> AssetCondition:
+    def to_scheduling_condition(self) -> SchedulingCondition:
         """Converts a set of materialize / skip rules into a single binary expression."""
-        from .asset_condition.asset_condition import (
+        from .auto_materialize_rule_impls import DiscardOnMaxMaterializationsExceededRule
+        from .declarative_scheduling.operators.boolean_operators import (
             AndAssetCondition,
             NotAssetCondition,
             OrAssetCondition,
         )
-        from .auto_materialize_rule_impls import DiscardOnMaxMaterializationsExceededRule
 
         if self.asset_condition is not None:
             return self.asset_condition
 
         materialize_condition = OrAssetCondition(
             operands=[
                 rule.to_asset_condition()
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/auto_materialize_rule.py` & `dagster-1.7.5/dagster/_core/definitions/auto_materialize_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,34 +8,37 @@
 from dagster._core.definitions.auto_materialize_rule_evaluation import (
     AutoMaterializeDecisionType,
     AutoMaterializeRuleSnapshot,
 )
 from dagster._utils.schedules import is_valid_cron_string
 
 if TYPE_CHECKING:
-    from dagster._core.definitions.asset_condition.asset_condition import (
-        AssetCondition,
-        AssetConditionResult,
-    )
     from dagster._core.definitions.auto_materialize_rule_impls import (
         AutoMaterializeAssetPartitionsFilter,
         MaterializeOnCronRule,
         MaterializeOnMissingRule,
         MaterializeOnParentUpdatedRule,
         MaterializeOnRequiredForFreshnessRule,
         SkipOnBackfillInProgressRule,
         SkipOnNotAllParentsUpdatedRule,
         SkipOnNotAllParentsUpdatedSinceCronRule,
         SkipOnParentMissingRule,
         SkipOnParentOutdatedRule,
         SkipOnRequiredButNonexistentParentsRule,
         SkipOnRunInProgressRule,
     )
-
-    from .asset_condition.asset_condition_evaluation_context import AssetConditionEvaluationContext
+    from dagster._core.definitions.declarative_scheduling.legacy.asset_condition import (
+        AssetCondition,
+    )
+    from dagster._core.definitions.declarative_scheduling.scheduling_condition import (
+        SchedulingResult,
+    )
+    from dagster._core.definitions.declarative_scheduling.scheduling_context import (
+        SchedulingContext,
+    )
 
 
 class AutoMaterializeRule(ABC):
     """An AutoMaterializeRule defines a bit of logic which helps determine if a materialization
     should be kicked off for a given asset partition.
 
     Each rule can have one of two decision types, `MATERIALIZE` (indicating that an asset partition
@@ -56,22 +59,20 @@
         """A human-readable description of this rule. As a basic guideline, this string should
         complete the sentence: 'Indicates an asset should be (materialize/skipped) when ____'.
         """
         ...
 
     def to_asset_condition(self) -> "AssetCondition":
         """Converts this AutoMaterializeRule into an AssetCondition."""
-        from .asset_condition.asset_condition import RuleCondition
+        from .declarative_scheduling.legacy.rule_condition import RuleCondition
 
         return RuleCondition(rule=self)
 
     @abstractmethod
-    def evaluate_for_asset(
-        self, context: "AssetConditionEvaluationContext"
-    ) -> "AssetConditionResult":
+    def evaluate_for_asset(self, context: "SchedulingContext") -> "SchedulingResult":
         """The core evaluation function for the rule. This function takes in a context object and
         returns a mapping from evaluated rules to the set of asset partitions that the rule applies
         to.
         """
         ...
 
     @public
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/auto_materialize_sensor_definition.py` & `dagster-1.7.5/dagster/_core/definitions/auto_materialize_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/backfill_policy.py` & `dagster-1.7.5/dagster/_core/definitions/backfill_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/base_asset_graph.py` & `dagster-1.7.5/dagster/_core/definitions/base_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.7.5/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/composition.py` & `dagster-1.7.5/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/config.py` & `dagster-1.7.5/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/configurable.py` & `dagster-1.7.5/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/data_time.py` & `dagster-1.7.5/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/data_version.py` & `dagster-1.7.5/dagster/_core/definitions/data_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,19 +377,20 @@
     _asset_graph: Optional["BaseAssetGraph"]
     _asset_graph_load_fn: Optional[Callable[[], "BaseAssetGraph"]]
 
     def __init__(
         self,
         instance: "DagsterInstance",
         asset_graph: Union["BaseAssetGraph", Callable[[], "BaseAssetGraph"]],
+        instance_queryer: Optional["CachingInstanceQueryer"] = None,
     ):
         from dagster._core.definitions.base_asset_graph import BaseAssetGraph
 
         self._instance = instance
-        self._instance_queryer = None
+        self._instance_queryer = instance_queryer
         if isinstance(asset_graph, BaseAssetGraph):
             self._asset_graph = asset_graph
             self._asset_graph_load_fn = None
         else:
             self._asset_graph = None
             self._asset_graph_load_fn = asset_graph
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.7.5/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/decorators/asset_check_decorator.py` & `dagster-1.7.5/dagster/_core/definitions/decorators/asset_check_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.7.5/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 from ..partition import PartitionsDefinition
 from ..policy import RetryPolicy
 from ..resource_definition import ResourceDefinition
 from ..utils import (
     DEFAULT_IO_MANAGER_KEY,
     DEFAULT_OUTPUT,
     NoValueSentinel,
-    validate_definition_tags,
+    validate_tags_strict,
 )
 
 
 @overload
 def asset(
     compute_fn: Callable[..., Any],
 ) -> AssetsDefinition: ...
@@ -90,15 +90,15 @@
     auto_materialize_policy: Optional[AutoMaterializePolicy] = ...,
     backfill_policy: Optional[BackfillPolicy] = ...,
     retry_policy: Optional[RetryPolicy] = ...,
     code_version: Optional[str] = ...,
     key: Optional[CoercibleToAssetKey] = None,
     non_argument_deps: Optional[Union[Set[AssetKey], Set[str]]] = ...,
     check_specs: Optional[Sequence[AssetCheckSpec]] = ...,
-    owners: Optional[List[str]] = ...,
+    owners: Optional[Sequence[str]] = ...,
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]: ...
 
 
 @experimental_param(param="resource_defs")
 @experimental_param(param="io_manager_def")
 @experimental_param(param="auto_materialize_policy")
 @experimental_param(param="backfill_policy")
@@ -132,15 +132,15 @@
     auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
     backfill_policy: Optional[BackfillPolicy] = None,
     retry_policy: Optional[RetryPolicy] = None,
     code_version: Optional[str] = None,
     key: Optional[CoercibleToAssetKey] = None,
     non_argument_deps: Optional[Union[Set[AssetKey], Set[str]]] = None,
     check_specs: Optional[Sequence[AssetCheckSpec]] = None,
-    owners: Optional[List[str]] = None,
+    owners: Optional[Sequence[str]] = None,
 ) -> Union[AssetsDefinition, Callable[[Callable[..., Any]], AssetsDefinition]]:
     """Create a definition for how to compute an asset.
 
     A software-defined asset is the combination of:
       1. An asset key, e.g. the name of a table.
       2. A function, which can be run to compute the contents of the asset.
       3. A set of upstream assets that are provided as inputs to the function when computing the asset.
@@ -232,15 +232,15 @@
 
         return _Asset(
             name=cast(Optional[str], name),  # (mypy bug that it can't infer name is Optional[str])
             key_prefix=key_prefix,
             ins=ins,
             deps=upstream_asset_deps,
             metadata=metadata,
-            tags=validate_definition_tags(tags),
+            tags=validate_tags_strict(tags),
             description=description,
             config_schema=config_schema,
             required_resource_keys=required_resource_keys,
             resource_defs=resource_defs,
             io_manager_key=io_manager_key,
             io_manager_def=io_manager_def,
             compute_kind=check.opt_str_param(compute_kind, "compute_kind"),
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.7.5/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.7.5/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.7.5/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.7.5/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.7.5/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.7.5/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.7.5/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.7.5/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.7.5/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from dagster._core.definitions.metadata import (
     RawMetadataMapping,
 )
 from dagster._core.definitions.partition import PartitionsDefinition
 from dagster._core.definitions.resource_annotation import get_resource_args
 from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.source_asset import SourceAsset, SourceAssetObserveFunction
-from dagster._core.definitions.utils import validate_definition_tags
+from dagster._core.definitions.utils import validate_tags_strict
 
 
 @overload
 def observable_source_asset(observe_fn: SourceAssetObserveFunction) -> SourceAsset: ...
 
 
 @overload
@@ -127,15 +127,15 @@
         group_name,
         required_resource_keys,
         resource_defs,
         partitions_def,
         auto_observe_interval_minutes,
         freshness_policy,
         op_tags,
-        tags=validate_definition_tags(tags),
+        tags=validate_tags_strict(tags),
     )
 
 
 class _ObservableSourceAsset:
     def __init__(
         self,
         key: Optional[CoercibleToAssetKey] = None,
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.7.5/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/definitions_class.py` & `dagster-1.7.5/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/dependency.py` & `dagster-1.7.5/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/events.py` & `dagster-1.7.5/dagster/_core/definitions/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,21 @@
 from dagster._annotations import PublicAttr, deprecated, experimental_param, public
 from dagster._core.definitions.asset_key import (
     AssetKey as AssetKey,
     CoercibleToAssetKey as CoercibleToAssetKey,
     CoercibleToAssetKeyPrefix as CoercibleToAssetKeyPrefix,
     parse_asset_key_string,
 )
-from dagster._core.definitions.data_version import DATA_VERSION_TAG, DataVersion
-from dagster._core.storage.tags import MULTIDIMENSIONAL_PARTITION_PREFIX, SYSTEM_TAG_PREFIX
+from dagster._core.definitions.data_version import (
+    _OLD_DATA_VERSION_TAG,
+    _OLD_INPUT_DATA_VERSION_TAG_PREFIX,
+    DATA_VERSION_TAG,
+    DataVersion,
+)
+from dagster._core.storage.tags import MULTIDIMENSIONAL_PARTITION_PREFIX, REPORTING_USER_TAG
 from dagster._serdes import whitelist_for_serdes
 from dagster._serdes.serdes import NamedTupleSerializer
 
 from .metadata import (
     MetadataFieldSerializer,
     MetadataMapping,
     MetadataValue,
@@ -84,34 +89,43 @@
             "result")
         metadata (Optional[Dict[str, Union[str, float, int, MetadataValue]]]):
             Arbitrary metadata about the output.  Keys are displayed string labels, and values are
             one of the following: string, float, int, JSON-serializable dict, JSON-serializable
             list, and one of the data classes returned by a MetadataValue static method.
         data_version (Optional[DataVersion]): (Experimental) A data version to manually set
             for the asset.
+        tags (Optional[Mapping[str, str]]): (Experimental) Tags that will be attached to the asset
+            materialization event corresponding to this output, if there is one.
     """
 
     def __init__(
         self,
         value: T,
         output_name: Optional[str] = DEFAULT_OUTPUT,
         metadata: Optional[Mapping[str, RawMetadataValue]] = None,
         data_version: Optional[DataVersion] = None,
+        *,
+        tags: Optional[Mapping[str, str]] = None,
     ):
         self._value = value
         self._output_name = check.str_param(output_name, "output_name")
         self._data_version = check.opt_inst_param(data_version, "data_version", DataVersion)
         self._metadata = normalize_metadata(
             check.opt_mapping_param(metadata, "metadata", key_type=str),
         )
+        self._tags = validate_asset_event_tags(tags)
 
     @property
     def metadata(self) -> MetadataMapping:
         return self._metadata
 
+    @property
+    def tags(self) -> Optional[Mapping[str, str]]:
+        return self._tags
+
     @public
     @property
     def value(self) -> Any:
         """Any: The value returned by the compute function."""
         return self._value
 
     @public
@@ -128,14 +142,15 @@
 
     def __eq__(self, other: object) -> bool:
         return (
             isinstance(other, Output)
             and self.value == other.value
             and self.output_name == other.output_name
             and self.metadata == other.metadata
+            and self.tags == other.tags
         )
 
 
 class DynamicOutput(Generic[T]):
     """Variant of :py:class:`Output <dagster.Output>` used to support
     dynamic mapping & collect. Each ``DynamicOutput`` produced by an op represents
     one item in a set that can be processed individually with ``map`` or gathered
@@ -223,16 +238,15 @@
 ):
     """Event that captures metadata about an asset at a point in time.
 
     Args:
         asset_key (Union[str, List[str], AssetKey]): A key to identify the asset.
         partition (Optional[str]): The name of a partition of the asset that the metadata
             corresponds to.
-        tags (Optional[Mapping[str, str]]): A mapping containing system-populated tags for the
-            observation. Users should not pass values into this argument.
+        tags (Optional[Mapping[str, str]]): A mapping containing tags for the observation.
         metadata (Optional[Dict[str, Union[str, float, int, MetadataValue]]]):
             Arbitrary metadata about the asset.  Keys are displayed string labels, and values are
             one of the following: string, float, int, JSON-serializable dict, JSON-serializable
             list, and one of the data classes returned by a MetadataValue static method.
     """
 
     def __new__(
@@ -247,31 +261,26 @@
             check.inst_param(asset_key, "asset_key", AssetKey)
         elif isinstance(asset_key, str):
             asset_key = AssetKey(parse_asset_key_string(asset_key))
         else:
             check.sequence_param(asset_key, "asset_key", of_type=str)
             asset_key = AssetKey(asset_key)
 
-        tags = check.opt_mapping_param(tags, "tags", key_type=str, value_type=str)
-        if any([not tag.startswith(SYSTEM_TAG_PREFIX) for tag in tags or {}]):
-            check.failed(
-                "Users should not pass values into the tags argument for AssetMaterializations. "
-                "The tags argument is reserved for system-populated tags."
-            )
+        validate_asset_event_tags(tags)
 
         normed_metadata = normalize_metadata(
             check.opt_mapping_param(metadata, "metadata", key_type=str),
         )
 
         return super(AssetObservation, cls).__new__(
             cls,
             asset_key=asset_key,
             description=check.opt_str_param(description, "description"),
             metadata=normed_metadata,
-            tags=tags,
+            tags=tags or {},
             partition=check.opt_str_param(partition, "partition"),
         )
 
     @property
     def label(self) -> str:
         return " ".join(self.asset_key.path)
 
@@ -325,16 +334,15 @@
 
     Args:
         asset_key (Union[str, List[str], AssetKey]): A key to identify the materialized asset across
             job runs
         description (Optional[str]): A longer human-readable description of the materialized value.
         partition (Optional[str]): The name of the partition
             that was materialized.
-        tags (Optional[Mapping[str, str]]): A mapping containing system-populated tags for the
-            materialization. Users should not pass values into this argument.
+        tags (Optional[Mapping[str, str]]): A mapping containing tags for the materialization.
         metadata (Optional[Dict[str, RawMetadataValue]]):
             Arbitrary metadata about the asset.  Keys are displayed string labels, and values are
             one of the following: string, float, int, JSON-serializable dict, JSON-serializable
             list, and one of the data classes returned by a MetadataValue static method.
     """
 
     def __new__(
@@ -351,21 +359,15 @@
             check.inst_param(asset_key, "asset_key", AssetKey)
         elif isinstance(asset_key, str):
             asset_key = AssetKey(parse_asset_key_string(asset_key))
         else:
             check.sequence_param(asset_key, "asset_key", of_type=str)
             asset_key = AssetKey(asset_key)
 
-        check.opt_mapping_param(tags, "tags", key_type=str, value_type=str)
-        invalid_tags = [tag for tag in tags or {} if not tag.startswith(SYSTEM_TAG_PREFIX)]
-        if len(invalid_tags) > 0:
-            check.failed(
-                f"Invalid tags: {tags} Users should not pass values into the tags argument for"
-                " AssetMaterializations. The tags argument is reserved for system-populated tags."
-            )
+        validate_asset_event_tags(tags)
 
         normed_metadata = normalize_metadata(
             check.opt_mapping_param(metadata, "metadata", key_type=str),
         )
 
         partition = check.opt_str_param(partition, "partition")
 
@@ -686,7 +688,40 @@
             cls,
             hook_name=check.str_param(hook_name, "hook_name"),
             is_skipped=cast(bool, check.opt_bool_param(is_skipped, "is_skipped", default=False)),
         )
 
 
 UserEvent = Union[AssetMaterialization, AssetObservation, ExpectationResult]
+
+
+def validate_asset_event_tags(tags: Optional[Mapping[str, str]]) -> Optional[Mapping[str, str]]:
+    from dagster._core.definitions.utils import validate_tag_strict
+
+    if tags is None:
+        return None
+
+    for key, value in tags.items():
+        # The format of these particular tags does not fit strict validation. E.g.
+        # - Some of the keys have two slashes
+        # - The value for the data/code version tags can be an arbitrary string
+        if not is_system_asset_event_tag(key):
+            validate_tag_strict(key, value)
+
+    return tags
+
+
+def is_system_asset_event_tag(key: str) -> bool:
+    from .data_version import (
+        CODE_VERSION_TAG,
+        DATA_VERSION_TAG,
+        INPUT_DATA_VERSION_TAG_PREFIX,
+        INPUT_EVENT_POINTER_TAG_PREFIX,
+    )
+
+    return (
+        key in [CODE_VERSION_TAG, DATA_VERSION_TAG, _OLD_DATA_VERSION_TAG, REPORTING_USER_TAG]
+        or key.startswith(INPUT_DATA_VERSION_TAG_PREFIX)
+        or key.startswith(INPUT_EVENT_POINTER_TAG_PREFIX)
+        or key.startswith(_OLD_INPUT_DATA_VERSION_TAG_PREFIX)
+        or key.startswith(MULTIDIMENSIONAL_PARTITION_PREFIX)
+    )
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/executor_definition.py` & `dagster-1.7.5/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/external_asset.py` & `dagster-1.7.5/dagster/_core/definitions/external_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/freshness_based_auto_materialize.py` & `dagster-1.7.5/dagster/_core/definitions/freshness_based_auto_materialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,26 +7,28 @@
     i.e. it`s late enough to pull in the required data time, and early enough to not go over the
     maximum lag minutes.
 """
 
 import datetime
 from typing import TYPE_CHECKING, AbstractSet, Optional, Sequence, Tuple
 
-from dagster._core.definitions.asset_subset import AssetSubset
+from dagster._core.definitions.asset_subset import AssetSubset, ValidAssetSubset
 from dagster._core.definitions.events import AssetKeyPartitionKey
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
 from dagster._seven.compat.pendulum import (
     PendulumInterval,
 )
 from dagster._utils.schedules import cron_string_iterator
 
 if TYPE_CHECKING:
-    from .asset_condition.asset_condition import AssetSubsetWithMetadata
-    from .asset_condition.asset_condition_evaluation_context import AssetConditionEvaluationContext
     from .auto_materialize_rule_evaluation import TextRuleEvaluationData
+    from .declarative_scheduling.legacy.legacy_context import (
+        LegacyRuleEvaluationContext,
+    )
+    from .declarative_scheduling.serialized_objects import AssetSubsetWithMetadata
 
 
 def get_execution_period_for_policy(
     freshness_policy: FreshnessPolicy,
     effective_data_time: Optional[datetime.datetime],
     current_time: datetime.datetime,
 ) -> PendulumInterval:
@@ -109,15 +111,15 @@
             "Required by this asset's policy and downstream asset's policy"
         )
 
     return merged_period, evaluation_data
 
 
 def get_expected_data_time_for_asset_key(
-    context: "AssetConditionEvaluationContext", will_materialize: bool
+    context: "LegacyRuleEvaluationContext", will_materialize: bool
 ) -> Optional[datetime.datetime]:
     """Returns the data time that you would expect this asset to have if you were to execute it
     on this tick.
     """
     from dagster._core.definitions.remote_asset_graph import RemoteAssetGraph
 
     asset_key = context.asset_key
@@ -152,22 +154,22 @@
         return expected_data_time
     # for root assets, this would just be the current time
     else:
         return current_time
 
 
 def freshness_evaluation_results_for_asset_key(
-    context: "AssetConditionEvaluationContext",
-) -> Tuple[AssetSubset, Sequence["AssetSubsetWithMetadata"]]:
+    context: "LegacyRuleEvaluationContext",
+) -> Tuple[ValidAssetSubset, Sequence["AssetSubsetWithMetadata"]]:
     """Returns a set of AssetKeyPartitionKeys to materialize in order to abide by the given
     FreshnessPolicies.
 
     Attempts to minimize the total number of asset executions.
     """
-    from .asset_condition.asset_condition import AssetSubsetWithMetadata
+    from .declarative_scheduling.serialized_objects import AssetSubsetWithMetadata
 
     asset_key = context.asset_key
     current_time = context.evaluation_time
 
     if (
         not context.asset_graph.get_downstream_freshness_policies(asset_key=asset_key)
         or context.asset_graph.get(asset_key).is_partitioned
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/freshness_checks/sensor.py` & `dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Iterator, Optional, Sequence, cast
 
 import pendulum
 
 from dagster import _check as check
 from dagster._annotations import experimental
 
-from ..asset_check_spec import AssetCheckKey
-from ..asset_checks import AssetChecksDefinition
-from ..asset_selection import AssetSelection
-from ..decorators import sensor
-from ..run_request import RunRequest
-from ..sensor_definition import DefaultSensorStatus, SensorDefinition, SensorEvaluationContext
-from .utils import (
+from ...asset_check_spec import AssetCheckKey
+from ...asset_checks import AssetChecksDefinition
+from ...asset_selection import AssetSelection
+from ...decorators import sensor
+from ...run_request import RunRequest
+from ...sensor_definition import DefaultSensorStatus, SensorDefinition, SensorEvaluationContext
+from ..utils import (
     FRESH_UNTIL_METADATA_KEY,
     ensure_no_duplicate_asset_checks,
     seconds_in_words,
 )
 
 DEFAULT_FRESHNESS_SENSOR_NAME = "freshness_checks_sensor"
 MAXIMUM_RUNTIME_SECONDS = 35  # Due to GRPC communications, only allow this sensor to run for 40 seconds before pausing iteration and resuming in the next run. Leave a bit of time for run requests to be processed.
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/freshness_checks/shared_builder.py` & `dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,221 +1,224 @@
-import datetime
-from typing import Any, Callable, Dict, Iterable, Optional, Sequence, Union, cast
+from typing import Any, Dict, Iterable, Sequence, Union
 
 import pendulum
 
 from dagster import _check as check
+from dagster._annotations import experimental
 from dagster._core.definitions.asset_check_result import AssetCheckResult
-from dagster._core.definitions.asset_check_spec import AssetCheckSeverity, AssetCheckSpec
+from dagster._core.definitions.asset_check_spec import AssetCheckSeverity
 from dagster._core.definitions.asset_checks import AssetChecksDefinition
-from dagster._core.definitions.decorators.asset_check_decorator import (
-    multi_asset_check,
-)
+from dagster._core.definitions.assets import AssetsDefinition, SourceAsset
+from dagster._core.definitions.events import AssetKey, CoercibleToAssetKey
 from dagster._core.definitions.metadata import (
-    FloatMetadataValue,
     JsonMetadataValue,
     MetadataValue,
     TimestampMetadataValue,
 )
-from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
+from dagster._core.definitions.time_window_partitions import (
+    TimeWindowPartitionsDefinition,
+)
 from dagster._core.execution.context.compute import (
     AssetCheckExecutionContext,
 )
 from dagster._utils.schedules import (
     get_latest_completed_cron_tick,
     get_next_cron_tick,
     is_valid_cron_string,
 )
 
-from ..assets import AssetsDefinition, SourceAsset
-from ..events import AssetKey, CoercibleToAssetKey
-from .utils import (
+from ..utils import (
     DEADLINE_CRON_PARAM_KEY,
-    EXPECTED_BY_TIMESTAMP_METADATA_KEY,
+    DEFAULT_FRESHNESS_SEVERITY,
+    DEFAULT_FRESHNESS_TIMEZONE,
     FRESH_UNTIL_METADATA_KEY,
     FRESHNESS_PARAMS_METADATA_KEY,
     LAST_UPDATED_TIMESTAMP_METADATA_KEY,
-    LOWER_BOUND_DELTA_PARAM_KEY,
-    OVERDUE_SECONDS_METADATA_KEY,
+    LATEST_CRON_TICK_METADATA_KEY,
     TIMEZONE_PARAM_KEY,
-    asset_to_keys_iterable,
+    assets_to_keys,
     ensure_no_duplicate_assets,
-    get_description_for_freshness_check_result,
+    freshness_multi_asset_check,
     get_last_updated_timestamp,
     retrieve_latest_record,
-    unique_id_from_asset_keys,
 )
 
 
-def build_freshness_multi_check(
+@experimental
+def build_time_partition_freshness_checks(
+    *,
+    assets: Sequence[Union[SourceAsset, CoercibleToAssetKey, AssetsDefinition]],
+    deadline_cron: str,
+    timezone: str = DEFAULT_FRESHNESS_TIMEZONE,
+    severity: AssetCheckSeverity = DEFAULT_FRESHNESS_SEVERITY,
+) -> Sequence[AssetChecksDefinition]:
+    r"""Construct an `AssetChecksDefinition` that checks the freshness of the provided assets.
+
+    This check passes if the asset is considered "fresh" by the time that execution begins. We
+    consider an asset to be "fresh" if there exists a record for the most recent partition, once
+    the deadline has passed.
+
+    `deadline_cron` is a cron schedule that defines the deadline for when we should expect the most
+    recent partition to arrive by. Once a tick of the cron schedule has passed, this check will fail
+    if the most recent partition has not been observed/materialized.
+
+    Let's say I have a daily-partitioned asset which runs every day at 8:00 AM UTC, and takes around
+    45 minutes to complete. To account for operational delays, I would expect the asset to be done
+    materializing every day by 9:00 AM UTC. I would set the `deadline_cron` to "0 9 \* \* \*". This
+    means that starting at 9:00 AM, this check will expect a record to exist for the previous day's
+    partition. Note that if the check runs at 8:59 AM, the deadline has not yet passed, and we'll
+    instead be checking for the most recently passed deadline, which is yesterday (meaning the
+    partition representing the day before yesterday).
+
+    The timestamp of an observation record is the timestamp indicated by the
+    "dagster/last_updated_timestamp" metadata key. The timestamp of a materialization record is the
+    timestamp at which that record was created.
+
+    The check will fail at runtime if a non-time-window partitioned asset is passed in.
+
+    The check result will contain the following metadata:
+    "dagster/freshness_params": A dictionary containing the parameters used to construct the
+    check.
+    "dagster/last_updated_time": (Only present if the asset has been observed/materialized before)
+    The time of the most recent update to the asset.
+    "dagster/overdue_seconds": (Only present if asset is overdue) The number of seconds that the
+    asset is overdue by.
+    "dagster/overdue_deadline_timestamp": The timestamp that we are expecting the asset to have
+    arrived by. This is the timestamp of the most recent tick of the cron schedule.
+
+    Examples:
+        .. code-block:: python
+
+            from dagster import build_time_partition_freshness_checks, AssetKey
+            # A daily partitioned asset that is expected to be updated every day within 45 minutes
+            # of 9:00 AM UTC
+            from .somewhere import my_daily_scheduled_assets_def
+
+            checks_def = build_time_partition_freshness_checks(
+                [my_daily_scheduled_assets_def],
+                deadline_cron="0 9 * * *",
+            )
+
+
+    Args:
+        assets (Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]): The assets to
+            construct checks for. For each passed in asset, there will be a corresponding
+            constructed `AssetChecksDefinition`.
+        deadline_cron (str): The check will pass if the partition time window most recently
+            completed by the time of the last cron tick has been observed/materialized.
+        timezone (Optional[str]): The timezone to use when calculating freshness and deadline. If
+            not provided, defaults to "UTC".
+
+    Returns:
+        Sequence[AssetChecksDefinition]: `AssetChecksDefinition` objects which execute freshness
+            checks for the provided assets.
+    """
+    check.str_param(timezone, "timezone")
+    check.opt_str_param(deadline_cron, "deadline_cron")
+    check.invariant(
+        deadline_cron is None or is_valid_cron_string(deadline_cron), "Invalid cron string."
+    )
+    check.inst_param(severity, "severity", AssetCheckSeverity)
+    check.sequence_param(assets, "assets")
+    ensure_no_duplicate_assets(assets)
+    return [
+        _build_freshness_multi_check(
+            asset_keys=assets_to_keys(assets),
+            deadline_cron=deadline_cron,
+            timezone=timezone,
+            severity=severity,
+        )
+    ]
+
+
+def _build_freshness_multi_check(
     asset_keys: Sequence[AssetKey],
-    deadline_cron: Optional[str],
+    deadline_cron: str,
     timezone: str,
     severity: AssetCheckSeverity,
-    lower_bound_delta: Optional[datetime.timedelta],
-    asset_property_enforcement_lambda: Optional[Callable[[AssetsDefinition], bool]],
 ) -> AssetChecksDefinition:
-    params_metadata: dict[str, Any] = {TIMEZONE_PARAM_KEY: timezone}
-    if deadline_cron:
-        params_metadata[DEADLINE_CRON_PARAM_KEY] = deadline_cron
-    if lower_bound_delta:
-        params_metadata[LOWER_BOUND_DELTA_PARAM_KEY] = lower_bound_delta.total_seconds()
-
-    @multi_asset_check(
-        specs=[
-            AssetCheckSpec(
-                "freshness_check",
-                asset=asset_key,
-                metadata={FRESHNESS_PARAMS_METADATA_KEY: params_metadata},
-                description="Evaluates freshness for targeted asset.",
-            )
-            for asset_key in asset_keys
-        ],
-        can_subset=True,
-        name=f"freshness_check_{unique_id_from_asset_keys(asset_keys)}",
+    params_metadata: dict[str, Any] = {
+        TIMEZONE_PARAM_KEY: timezone,
+        DEADLINE_CRON_PARAM_KEY: deadline_cron,
+    }
+
+    @freshness_multi_asset_check(
+        params_metadata=JsonMetadataValue(params_metadata), asset_keys=asset_keys
     )
     def the_check(context: AssetCheckExecutionContext) -> Iterable[AssetCheckResult]:
         for check_key in context.selected_asset_check_keys:
             asset_key = check_key.asset_key
-            if asset_property_enforcement_lambda:
-                asset_property_enforcement_lambda(
-                    context.job_def.asset_layer.asset_graph.get(check_key.asset_key).assets_def
-                )
             current_timestamp = pendulum.now("UTC").timestamp()
 
-            # Explicit call to partitions def here will be replaced with AssetSlice reference once it's available.
-            partitions_def = cast(
-                Optional[TimeWindowPartitionsDefinition],
+            partitions_def = check.inst(
                 context.job_def.asset_layer.asset_graph.get(asset_key).partitions_def,
-            )
-
-            check.invariant(
-                partitions_def is None
-                or isinstance(partitions_def, TimeWindowPartitionsDefinition),
-                "Expected partitions_def to be time-windowed.",
+                TimeWindowPartitionsDefinition,
             )
             current_time_in_freshness_tz = pendulum.from_timestamp(current_timestamp, tz=timezone)
-            latest_completed_cron_tick = (
-                get_latest_completed_cron_tick(
-                    deadline_cron, current_time_in_freshness_tz, timezone
-                )
-                if deadline_cron
-                else None
+            deadline = get_latest_completed_cron_tick(
+                deadline_cron, current_time_in_freshness_tz, timezone
             )
-            deadline = check.inst_param(
-                latest_completed_cron_tick or current_time_in_freshness_tz,
-                "deadline",
-                datetime.datetime,
-            )
-            if not partitions_def:
-                last_completed_time_window = None
-                expected_partition_key = None
-            else:
-                deadline_in_partitions_def_tz = pendulum.from_timestamp(
-                    deadline.timestamp(), tz=partitions_def.timezone
-                )
-                last_completed_time_window = check.not_none(
-                    partitions_def.get_prev_partition_window(deadline_in_partitions_def_tz)
-                )
-                expected_partition_key = partitions_def.get_partition_key_range_for_time_window(
-                    last_completed_time_window
-                ).start
-
-            if lower_bound_delta:
-                last_update_time_lower_bound = cast(datetime.datetime, deadline - lower_bound_delta)
-            else:
-                last_update_time_lower_bound = check.not_none(
-                    last_completed_time_window,
-                    "Expected a valid partitioned asset with a completed time window in order to determine valid freshness window.",
-                ).end
-
+            deadline_in_partitions_def_tz = pendulum.from_timestamp(
+                deadline.timestamp(), tz=partitions_def.timezone
+            )
+            last_completed_time_window = check.not_none(
+                partitions_def.get_prev_partition_window(deadline_in_partitions_def_tz)
+            )
+            expected_partition_key = partitions_def.get_partition_key_range_for_time_window(
+                last_completed_time_window
+            ).start
             latest_record = retrieve_latest_record(
                 instance=context.instance, asset_key=asset_key, partition_key=expected_partition_key
             )
-            update_timestamp = get_last_updated_timestamp(latest_record, context)
-            passed = (
-                update_timestamp is not None
-                and update_timestamp >= last_update_time_lower_bound.timestamp()
-            )
+            passed = latest_record is not None
 
             metadata: Dict[str, MetadataValue] = {
                 FRESHNESS_PARAMS_METADATA_KEY: JsonMetadataValue(params_metadata),
+                LATEST_CRON_TICK_METADATA_KEY: TimestampMetadataValue(deadline.timestamp()),
             }
-            if not passed:
-                metadata[OVERDUE_SECONDS_METADATA_KEY] = FloatMetadataValue(
-                    current_timestamp - deadline.timestamp()
-                )
-                expected_by = (
-                    deadline.timestamp()
-                    if deadline_cron
-                    else update_timestamp + check.not_none(lower_bound_delta).total_seconds()
-                    if update_timestamp
-                    else None
+
+            # Allows us to distinguish between the case where the asset has never been
+            # observed/materialized, and the case where this partition in particular is missing
+            latest_record_any_partition = retrieve_latest_record(
+                instance=context.instance, asset_key=asset_key, partition_key=None
+            )
+
+            if not passed and latest_record_any_partition is not None:
+                # If this asset has been updated at all before, provide the time at which that
+                # happened as additional metadata.
+                metadata[LAST_UPDATED_TIMESTAMP_METADATA_KEY] = TimestampMetadataValue(
+                    check.not_none(get_last_updated_timestamp(latest_record_any_partition, context))
                 )
-                if expected_by:
-                    metadata[EXPECTED_BY_TIMESTAMP_METADATA_KEY] = TimestampMetadataValue(
-                        expected_by
-                    )
-            else:
-                # If the asset is fresh, we can potentially determine when it has the possibility of becoming stale again.
-                # In the case of a deadline cron, this is the next cron tick after the current time.
-                # In the case of just a lower_bound_delta, this is the last update time plus the
-                # lower_bound_delta.
-                fresh_until = (
-                    check.not_none(
-                        get_next_cron_tick(deadline_cron, current_time_in_freshness_tz, timezone)
+            elif passed:
+                metadata[FRESH_UNTIL_METADATA_KEY] = TimestampMetadataValue(
+                    get_next_cron_tick(
+                        deadline_cron, current_time_in_freshness_tz, timezone
                     ).timestamp()
-                    if deadline_cron
-                    else check.not_none(update_timestamp)
-                    + check.not_none(lower_bound_delta).total_seconds()
-                )
-                metadata[FRESH_UNTIL_METADATA_KEY] = TimestampMetadataValue(fresh_until)
-            if update_timestamp:
-                metadata[LAST_UPDATED_TIMESTAMP_METADATA_KEY] = TimestampMetadataValue(
-                    update_timestamp
                 )
 
             yield AssetCheckResult(
                 passed=passed,
-                description=get_description_for_freshness_check_result(
-                    passed,
-                    update_timestamp,
-                    last_update_time_lower_bound,
-                    current_timestamp,
-                    expected_partition_key,
-                    record_arrival_timestamp=latest_record.timestamp if latest_record else None,
-                    event_type=latest_record.event_type if latest_record else None,
+                description=_construct_description(
+                    partition_key=expected_partition_key,
+                    passed=passed,
+                    any_records_exist_for_asset=latest_record_any_partition is not None,
                 ),
                 severity=severity,
                 asset_key=asset_key,
                 metadata=metadata,
             )
 
     return the_check
 
 
-def build_freshness_checks_for_assets(
-    assets: Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]],
-    deadline_cron: Optional[str],
-    timezone: str,
-    severity: AssetCheckSeverity,
-    asset_property_enforcement_lambda: Optional[Callable[[AssetsDefinition], bool]] = None,
-    lower_bound_delta: Optional[datetime.timedelta] = None,
-) -> AssetChecksDefinition:
-    ensure_no_duplicate_assets(assets)
-    deadline_cron = check.opt_str_param(deadline_cron, "deadline_cron")
-    check.invariant(
-        is_valid_cron_string(deadline_cron) if deadline_cron else True,
-        "deadline_cron must be a valid cron string.",
-    )
-    severity = check.inst_param(severity, "severity", AssetCheckSeverity)
-    timezone = check.str_param(timezone, "timezone")
-    check.opt_inst_param(lower_bound_delta, "lower_bound_delta", datetime.timedelta)
-
-    return build_freshness_multi_check(
-        asset_keys=[asset_key for asset in assets for asset_key in asset_to_keys_iterable(asset)],
-        deadline_cron=deadline_cron,
-        timezone=timezone,
-        severity=severity,
-        lower_bound_delta=lower_bound_delta,
-        asset_property_enforcement_lambda=asset_property_enforcement_lambda,
+def _construct_description(
+    partition_key: str,
+    passed: bool,
+    any_records_exist_for_asset: bool,
+) -> str:
+    if passed:
+        return f"Asset is currently fresh, since partition {partition_key} has been observed/materialized."
+    elif not any_records_exist_for_asset:
+        return f"The asset has never been observed/materialized. We currently expect partition {partition_key} to have arrived."
+    return (
+        f"Asset is overdue. We expected partition {partition_key} to have arrived, and it has not."
     )
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/freshness_checks/utils.py` & `dagster-1.7.5/dagster/_core/definitions/asset_check_factories/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import datetime
 from typing import Iterator, Optional, Sequence, Union, cast
 
 from dagster import _check as check
-from dagster._core.definitions.asset_check_spec import AssetCheckSeverity
+from dagster._core.definitions.asset_check_spec import AssetCheckSeverity, AssetCheckSpec
 from dagster._core.definitions.asset_checks import AssetChecksDefinition
+from dagster._core.definitions.decorators.asset_check_decorator import (
+    MultiAssetCheckFunction,
+    multi_asset_check,
+)
+from dagster._core.definitions.metadata import JsonMetadataValue
 from dagster._core.event_api import AssetRecordsFilter, EventLogRecord
 from dagster._core.events import DagsterEventType
 from dagster._core.execution.context.compute import AssetCheckExecutionContext
 from dagster._core.instance import DagsterInstance
 from dagster._utils.security import non_secure_md5_hash_str
 
 from ..assets import AssetsDefinition, SourceAsset
@@ -16,22 +21,23 @@
 # Constants
 DEFAULT_FRESHNESS_SEVERITY = AssetCheckSeverity.WARN
 DEFAULT_FRESHNESS_TIMEZONE = "UTC"
 
 # Top-level metadata keys
 LAST_UPDATED_TIMESTAMP_METADATA_KEY = "dagster/last_updated_timestamp"
 FRESHNESS_PARAMS_METADATA_KEY = "dagster/freshness_params"
-# When an asset is overdue, this represents the timestamp by which the asset was expected to arrive.
-EXPECTED_BY_TIMESTAMP_METADATA_KEY = "dagster/expected_by_timestamp"
+# The latest asset record should be no earlier than this timestamp.
+LOWER_BOUND_TIMESTAMP_METADATA_KEY = "dagster/freshness_lower_bound_timestamp"
 # When an asset is fresh, this represents the timestamp when the asset can become stale again.
 FRESH_UNTIL_METADATA_KEY = "dagster/fresh_until_timestamp"
-OVERDUE_SECONDS_METADATA_KEY = "dagster/overdue_seconds"
+# If this is cron-based freshness, this is the latest tick of the cron.
+LATEST_CRON_TICK_METADATA_KEY = "dagster/latest_cron_tick_timestamp"
 
 # dagster/freshness_params inner keys
-LOWER_BOUND_DELTA_PARAM_KEY = "lower_bound_delta"
+LOWER_BOUND_DELTA_PARAM_KEY = "lower_bound_delta_seconds"
 DEADLINE_CRON_PARAM_KEY = "deadline_cron"
 TIMEZONE_PARAM_KEY = "timezone"
 
 
 def ensure_no_duplicate_assets(
     assets: Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]],
 ) -> None:
@@ -39,43 +45,40 @@
 
     Args:
         assets (Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]]): The assets to check for duplicates.
 
     Returns:
         Sequence[AssetKey]: A list of the duplicate assets.
     """
-    asset_keys = [
-        asset_key for asset in assets for asset_key in list(asset_to_keys_iterable(asset))
-    ]
+    asset_keys = assets_to_keys(assets)
     duplicate_assets = [asset_key for asset_key in asset_keys if asset_keys.count(asset_key) > 1]
     check.invariant(
         len(duplicate_assets) == 0,
         f"Found duplicate assets in the provided list of assets: {duplicate_assets}. Please ensure that each asset is unique.",
     )
 
 
-def asset_to_keys_iterable(
+def _asset_to_keys_iterable(
     asset: Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset],
 ) -> Iterator[AssetKey]:
-    """Converts the provided asset construct to a sequence of AssetKeys.
-
-    Args:
-        asset (Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]): The asset to convert to a sequence of AssetKeys.
-
-    Returns:
-        Sequence[AssetKey]: A sequence of AssetKeys.
-    """
     if isinstance(asset, AssetsDefinition):
         yield from asset.keys
     elif isinstance(asset, SourceAsset):
         yield asset.key
     else:
         yield AssetKey.from_coercible_or_definition(asset)
 
 
+def assets_to_keys(
+    assets: Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]],
+) -> Sequence[AssetKey]:
+    """Converts the provided assets to a sequence of their contained AssetKeys."""
+    return [asset_key for asset in assets for asset_key in _asset_to_keys_iterable(asset)]
+
+
 def ensure_no_duplicate_asset_checks(
     asset_checks: Sequence[AssetChecksDefinition],
 ) -> None:
     asset_check_keys = [
         asset_check_key
         for asset_check in asset_checks
         for asset_check_key in asset_check.check_keys
@@ -236,7 +239,26 @@
     This is necessary to disambiguate between different ops underlying freshness checks without
     forcing the user to provide a name for the underlying op.
     """
     sorted_asset_keys = sorted(asset_keys, key=lambda asset_key: asset_key.to_string())
     return non_secure_md5_hash_str(
         ",".join([str(asset_key) for asset_key in sorted_asset_keys]).encode()
     )[:8]
+
+
+def freshness_multi_asset_check(params_metadata: JsonMetadataValue, asset_keys: Sequence[AssetKey]):
+    def inner(fn: MultiAssetCheckFunction) -> AssetChecksDefinition:
+        return multi_asset_check(
+            specs=[
+                AssetCheckSpec(
+                    "freshness_check",
+                    asset=asset_key,
+                    metadata={FRESHNESS_PARAMS_METADATA_KEY: params_metadata},
+                    description="Evaluates freshness for targeted asset.",
+                )
+                for asset_key in asset_keys
+            ],
+            can_subset=True,
+            name=f"freshness_check_{unique_id_from_asset_keys(asset_keys)}",
+        )(fn)
+
+    return inner
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/freshness_policy.py` & `dagster-1.7.5/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.7.5/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/graph_definition.py` & `dagster-1.7.5/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/hook_definition.py` & `dagster-1.7.5/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/hook_invocation.py` & `dagster-1.7.5/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/inference.py` & `dagster-1.7.5/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/input.py` & `dagster-1.7.5/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/instigation_logger.py` & `dagster-1.7.5/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/job_base.py` & `dagster-1.7.5/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/job_definition.py` & `dagster-1.7.5/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/load_asset_checks_from_modules.py` & `dagster-1.7.5/dagster/_core/definitions/load_asset_checks_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.7.5/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/logger_definition.py` & `dagster-1.7.5/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/logger_invocation.py` & `dagster-1.7.5/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/materialize.py` & `dagster-1.7.5/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.7.5/dagster/_core/definitions/metadata/metadata_value.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,153 +1,52 @@
 import os
 from abc import ABC, abstractmethod
 from datetime import datetime
 from typing import (
-    AbstractSet,
     Any,
     Callable,
-    Dict,
     Generic,
-    List,
     Mapping,
-    NamedTuple,
     Optional,
     Sequence,
-    Type,
     Union,
-    cast,
 )
 
-from typing_extensions import Self, TypeAlias, TypeVar
+from pydantic import Field
+from typing_extensions import Self, TypeVar
 
 import dagster._check as check
 import dagster._seven as seven
-from dagster._annotations import PublicAttr, deprecated, deprecated_param, experimental, public
+from dagster._annotations import PublicAttr, experimental, public
 from dagster._core.definitions.asset_key import AssetKey
 from dagster._core.errors import DagsterInvalidMetadata
 from dagster._model import DagsterModel
-from dagster._model.pydantic_compat_layer import model_fields
-from dagster._serdes import whitelist_for_serdes
+from dagster._serdes import pack_value, whitelist_for_serdes
 from dagster._serdes.serdes import (
     FieldSerializer,
+    JsonSerializableValue,
     PackableValue,
     UnpackContext,
     WhitelistMap,
-    pack_value,
-)
-from dagster._utils.warnings import (
-    deprecation_warning,
-    normalize_renamed_param,
 )
 
 from .table import (  # re-exported
     TableColumn as TableColumn,
     TableColumnConstraints as TableColumnConstraints,
     TableColumnDep as TableColumnDep,
     TableColumnLineage as TableColumnLineage,
     TableConstraints as TableConstraints,
     TableRecord as TableRecord,
     TableSchema as TableSchema,
 )
 
-ArbitraryMetadataMapping: TypeAlias = Mapping[str, Any]
-
-RawMetadataValue = Union[
-    "MetadataValue",
-    TableSchema,
-    AssetKey,
-    os.PathLike,
-    Dict[Any, Any],
-    float,
-    int,
-    List[Any],
-    str,
-    datetime,
-    None,
-]
-
-MetadataMapping: TypeAlias = Mapping[str, "MetadataValue"]
-RawMetadataMapping: TypeAlias = Mapping[str, RawMetadataValue]
-
 T_Packable = TypeVar("T_Packable", bound=PackableValue, default=PackableValue, covariant=True)
 
 
 # ########################
-# ##### NORMALIZATION
-# ########################
-
-
-def normalize_metadata(
-    metadata: Mapping[str, RawMetadataValue],
-    allow_invalid: bool = False,
-) -> Mapping[str, "MetadataValue"]:
-    # This is a stopgap measure to deal with unsupported metadata values, which occur when we try
-    # to convert arbitrary metadata (on e.g. OutputDefinition) to a MetadataValue, which is required
-    # for serialization. This will cause unsupported values to be silently replaced with a
-    # string placeholder.
-    normalized_metadata: Dict[str, MetadataValue] = {}
-    for k, v in metadata.items():
-        try:
-            normalized_value = normalize_metadata_value(v)
-        except DagsterInvalidMetadata as e:
-            if allow_invalid:
-                deprecation_warning(
-                    "Support for arbitrary metadata values",
-                    "2.0.0",
-                    additional_warn_text=(
-                        "In the future, all user-supplied metadata values must be one of"
-                        f" {RawMetadataValue}"
-                    ),
-                    stacklevel=4,  # to get the caller of `normalize_metadata`
-                )
-                normalized_value = TextMetadataValue(f"[{v.__class__.__name__}] (unserializable)")
-            else:
-                raise DagsterInvalidMetadata(
-                    f'Could not resolve the metadata value for "{k}" to a known type. {e}'
-                ) from None
-        normalized_metadata[k] = normalized_value
-
-    return normalized_metadata
-
-
-def has_corresponding_metadata_value_class(obj: Any) -> bool:
-    return isinstance(obj, (str, float, bool, int, list, dict, os.PathLike, AssetKey, TableSchema))
-
-
-def normalize_metadata_value(raw_value: RawMetadataValue) -> "MetadataValue[Any]":
-    if isinstance(raw_value, MetadataValue):
-        return raw_value
-    elif isinstance(raw_value, str):
-        return MetadataValue.text(raw_value)
-    elif isinstance(raw_value, float):
-        return MetadataValue.float(raw_value)
-    elif isinstance(raw_value, bool):
-        return MetadataValue.bool(raw_value)
-    elif isinstance(raw_value, int):
-        return MetadataValue.int(raw_value)
-    elif isinstance(raw_value, (list, dict)):
-        return MetadataValue.json(raw_value)
-    elif isinstance(raw_value, os.PathLike):
-        return MetadataValue.path(raw_value)
-    elif isinstance(raw_value, AssetKey):
-        return MetadataValue.asset(raw_value)
-    elif isinstance(raw_value, TableSchema):
-        return MetadataValue.table_schema(raw_value)
-    elif isinstance(raw_value, TableColumnLineage):
-        return MetadataValue.column_lineage(raw_value)
-    elif raw_value is None:
-        return MetadataValue.null()
-
-    raise DagsterInvalidMetadata(
-        f"Its type was {type(raw_value)}. Consider wrapping the value with the appropriate "
-        "MetadataValue type."
-    )
-
-
-# ########################
 # ##### METADATA VALUE
 # ########################
 
 
 class MetadataValue(ABC, Generic[T_Packable]):
     """Utility class to wrap metadata values passed into Dagster events so that they can be
     displayed in the Dagster UI and other tooling.
@@ -610,381 +509,360 @@
 # for us because these static methods should never be called on instances.
 
 # NOTE: `XMetadataValue` classes are serialized with a storage name of `XMetadataEntryData` to
 # maintain backward compatibility. See docstring of `whitelist_for_serdes` for more info.
 
 
 @whitelist_for_serdes(storage_name="TextMetadataEntryData")
-class TextMetadataValue(
-    NamedTuple(
-        "_TextMetadataValue",
-        [
-            ("text", PublicAttr[Optional[str]]),
-        ],
-    ),
-    MetadataValue[str],
-):
+class TextMetadataValue(DagsterModel, MetadataValue[str]):
     """Container class for text metadata entry data.
 
     Args:
         text (Optional[str]): The text data.
     """
 
-    def __new__(cls, text: Optional[str]):
-        return super(TextMetadataValue, cls).__new__(
-            cls, check.opt_str_param(text, "text", default="")
-        )
+    text_inner: Optional[str] = Field(..., alias="text")
+
+    def __init__(self, text: Optional[str]):
+        super().__init__(text=text or "")
+
+    @public
+    @property
+    def text(self) -> Optional[str]:
+        return self.text_inner
 
     @public
     @property
     def value(self) -> Optional[str]:
         """Optional[str]: The wrapped text data."""
-        return self.text
+        return self.text_inner
 
 
 @whitelist_for_serdes(storage_name="UrlMetadataEntryData")
-class UrlMetadataValue(
-    NamedTuple(
-        "_UrlMetadataValue",
-        [
-            ("url", PublicAttr[Optional[str]]),
-        ],
-    ),
-    MetadataValue[str],
-):
+class UrlMetadataValue(DagsterModel, MetadataValue[str]):
     """Container class for URL metadata entry data.
 
     Args:
         url (Optional[str]): The URL as a string.
     """
 
-    def __new__(cls, url: Optional[str]):
-        return super(UrlMetadataValue, cls).__new__(
-            cls, check.opt_str_param(url, "url", default="")
-        )
+    url_inner: Optional[str] = Field(..., alias="url")
+
+    def __init__(self, url: Optional[str]):
+        super().__init__(url=url or "")
 
     @public
     @property
     def value(self) -> Optional[str]:
         """Optional[str]: The wrapped URL."""
-        return self.url
+        return self.url_inner
+
+    @public
+    @property
+    def url(self) -> Optional[str]:
+        """Optional[str]: The wrapped URL."""
+        return self.url_inner
 
 
 @whitelist_for_serdes(storage_name="PathMetadataEntryData")
-class PathMetadataValue(
-    NamedTuple("_PathMetadataValue", [("path", PublicAttr[Optional[str]])]), MetadataValue[str]
-):
+class PathMetadataValue(DagsterModel, MetadataValue[str]):
     """Container class for path metadata entry data.
 
     Args:
         path (Optional[str]): The path as a string or conforming to os.PathLike.
     """
 
-    def __new__(cls, path: Optional[Union[str, os.PathLike]]):
-        return super(PathMetadataValue, cls).__new__(
-            cls, check.opt_path_param(path, "path", default="")
-        )
+    path_inner: Optional[str] = Field(..., alias="path")
+
+    def __init__(self, path: Optional[Union[str, os.PathLike]]):
+        super().__init__(path=check.opt_path_param(path, "path", default=""))
+
+    @public
+    @property
+    def path(self) -> Optional[str]:
+        return self.path_inner
 
     @public
     @property
     def value(self) -> Optional[str]:
         """Optional[str]: The wrapped path."""
-        return self.path
+        return self.path_inner
 
 
 @whitelist_for_serdes(storage_name="NotebookMetadataEntryData")
-class NotebookMetadataValue(
-    NamedTuple("_NotebookMetadataValue", [("path", PublicAttr[Optional[str]])]), MetadataValue[str]
-):
+class NotebookMetadataValue(DagsterModel, MetadataValue[str]):
     """Container class for notebook metadata entry data.
 
     Args:
         path (Optional[str]): The path to the notebook as a string or conforming to os.PathLike.
     """
 
-    def __new__(cls, path: Optional[Union[str, os.PathLike]]):
-        return super(NotebookMetadataValue, cls).__new__(
-            cls, check.opt_path_param(path, "path", default="")
-        )
+    path_inner: Optional[str] = Field(..., alias="path")
+
+    def __init__(self, path: Optional[Union[str, os.PathLike]]):
+        super().__init__(path=check.opt_path_param(path, "path", default=""))
+
+    @public
+    @property
+    def path(self) -> Optional[str]:
+        return self.path_inner
 
     @public
     @property
     def value(self) -> Optional[str]:
         """Optional[str]: The wrapped path to the notebook as a string."""
-        return self.path
+        return self.path_inner
+
+
+class JsonDataFieldSerializer(FieldSerializer):
+    def pack(
+        self,
+        mapping: JsonSerializableValue,
+        whitelist_map: WhitelistMap,
+        descent_path: str,
+    ) -> JsonSerializableValue:
+        # return the json serializable data field as is
+        return mapping
+
+    def unpack(
+        self,
+        unpacked_value: JsonSerializableValue,
+        whitelist_map: WhitelistMap,
+        context: UnpackContext,
+    ) -> PackableValue:
+        # erase any serdes objects that were stored here in earlier versions and
+        # return plain json serializable data
+        return pack_value(unpacked_value, whitelist_map=whitelist_map)
 
 
-@whitelist_for_serdes(storage_name="JsonMetadataEntryData")
-class JsonMetadataValue(
-    NamedTuple(
-        "_JsonMetadataValue",
-        [
-            ("data", PublicAttr[Optional[Union[Sequence[Any], Mapping[str, Any]]]]),
-        ],
-    ),
-    MetadataValue[Union[Sequence[Any], Mapping[str, Any]]],
-):
+@whitelist_for_serdes(
+    storage_name="JsonMetadataEntryData",
+    field_serializers={"data": JsonDataFieldSerializer},
+)
+class JsonMetadataValue(DagsterModel, MetadataValue[Union[Sequence[Any], Mapping[str, Any]]]):
     """Container class for JSON metadata entry data.
 
     Args:
         data (Union[Sequence[Any], Dict[str, Any]]): The JSON data.
     """
 
-    def __new__(cls, data: Optional[Union[Sequence[Any], Mapping[str, Any]]]):
+    data: PublicAttr[Optional[Union[Sequence[Any], Mapping[str, Any]]]]
+
+    def __init__(self, data: Optional[Union[Sequence[Any], Mapping[str, Any]]]):
         data = check.opt_inst_param(data, "data", (Sequence, Mapping))
         try:
             # check that the value is JSON serializable
             seven.dumps(data)
         except TypeError:
             raise DagsterInvalidMetadata("Value is not JSON serializable.")
-        return super(JsonMetadataValue, cls).__new__(cls, data)
+        super().__init__(data=data)
 
     @public
     @property
     def value(self) -> Optional[Union[Sequence[Any], Mapping[str, Any]]]:
         """Optional[Union[Sequence[Any], Dict[str, Any]]]: The wrapped JSON data."""
         return self.data
 
 
 @whitelist_for_serdes(storage_name="MarkdownMetadataEntryData")
-class MarkdownMetadataValue(
-    NamedTuple(
-        "_MarkdownMetadataValue",
-        [
-            ("md_str", PublicAttr[Optional[str]]),
-        ],
-    ),
-    MetadataValue[str],
-):
+class MarkdownMetadataValue(DagsterModel, MetadataValue[str]):
     """Container class for markdown metadata entry data.
 
     Args:
         md_str (Optional[str]): The markdown as a string.
     """
 
-    def __new__(cls, md_str: Optional[str]):
-        return super(MarkdownMetadataValue, cls).__new__(
-            cls, check.opt_str_param(md_str, "md_str", default="")
-        )
+    md_str: PublicAttr[Optional[str]]
+
+    def __init__(self, md_str: Optional[str]):
+        super().__init__(md_str=md_str or "")
 
     @public
     @property
     def value(self) -> Optional[str]:
         """Optional[str]: The wrapped markdown as a string."""
         return self.md_str
 
 
 # This should be deprecated or fixed so that `value` does not return itself.
 @whitelist_for_serdes(storage_name="PythonArtifactMetadataEntryData")
-class PythonArtifactMetadataValue(
-    NamedTuple(
-        "_PythonArtifactMetadataValue",
-        [
-            ("module", PublicAttr[str]),
-            ("name", PublicAttr[str]),
-        ],
-    ),
-    MetadataValue["PythonArtifactMetadataValue"],
-):
+class PythonArtifactMetadataValue(DagsterModel, MetadataValue["PythonArtifactMetadataValue"]):
     """Container class for python artifact metadata entry data.
 
     Args:
         module (str): The module where the python artifact can be found
         name (str): The name of the python artifact
     """
 
-    def __new__(cls, module: str, name: str):
-        return super(PythonArtifactMetadataValue, cls).__new__(
-            cls, check.str_param(module, "module"), check.str_param(name, "name")
-        )
+    module: PublicAttr[str]
+    name: PublicAttr[str]
+
+    def __init__(self, module: str, name: str):
+        super().__init__(module=module, name=name)
 
     @public
     @property
     def value(self) -> Self:
         """PythonArtifactMetadataValue: Identity function."""
         return self
 
 
 @whitelist_for_serdes(storage_name="FloatMetadataEntryData")
-class FloatMetadataValue(
-    NamedTuple(
-        "_FloatMetadataValue",
-        [
-            ("value", PublicAttr[Optional[float]]),
-        ],
-    ),
-    MetadataValue[float],
-):
+class FloatMetadataValue(DagsterModel, MetadataValue[float]):
     """Container class for float metadata entry data.
 
     Args:
         value (Optional[float]): The float value.
     """
 
-    def __new__(cls, value: Optional[float]):
-        return super(FloatMetadataValue, cls).__new__(cls, check.opt_float_param(value, "value"))
+    value_inner: Optional[float] = Field(..., alias="value")
+
+    def __init__(self, value: Optional[float]):
+        super().__init__(value=value)
+
+    @public
+    @property
+    def value(self) -> Optional[float]:
+        return self.value_inner
 
 
 @whitelist_for_serdes(storage_name="IntMetadataEntryData")
-class IntMetadataValue(
-    NamedTuple(
-        "_IntMetadataValue",
-        [
-            ("value", PublicAttr[Optional[int]]),
-        ],
-    ),
-    MetadataValue[int],
-):
+class IntMetadataValue(DagsterModel, MetadataValue[int]):
     """Container class for int metadata entry data.
 
     Args:
         value (Optional[int]): The int value.
     """
 
-    def __new__(cls, value: Optional[int]):
-        return super(IntMetadataValue, cls).__new__(cls, check.opt_int_param(value, "value"))
+    value_inner: Optional[int] = Field(..., alias="value")
+
+    def __init__(self, value: Optional[int]):
+        super().__init__(value=value)
+
+    @public
+    @property
+    def value(self) -> Optional[int]:
+        return self.value_inner
 
 
 @whitelist_for_serdes(storage_name="BoolMetadataEntryData")
-class BoolMetadataValue(
-    NamedTuple("_BoolMetadataValue", [("value", PublicAttr[Optional[bool]])]),
-    MetadataValue[bool],
-):
+class BoolMetadataValue(DagsterModel, MetadataValue[bool]):
     """Container class for bool metadata entry data.
 
     Args:
         value (Optional[bool]): The bool value.
     """
 
-    def __new__(cls, value: Optional[bool]):
-        return super(BoolMetadataValue, cls).__new__(cls, check.opt_bool_param(value, "value"))
+    value_inner: Optional[bool] = Field(..., alias="value")
+
+    def __init__(self, value: Optional[bool]):
+        super().__init__(value=value)
+
+    @public
+    @property
+    def value(self) -> Optional[bool]:
+        return self.value_inner
 
 
 @whitelist_for_serdes
-class TimestampMetadataValue(
-    NamedTuple(
-        "_DateTimeMetadataValue",
-        [("value", PublicAttr[float])],
-    ),
-    MetadataValue[float],
-):
+class TimestampMetadataValue(DagsterModel, MetadataValue[float]):
     """Container class for metadata value that's a unix timestamp.
 
     Args:
         value (float): Seconds since the unix epoch.
     """
 
-    def __new__(cls, value: float):
-        return super(TimestampMetadataValue, cls).__new__(cls, check.float_param(value, "value"))
+    value_inner: Optional[float] = Field(..., alias="value")
+
+    def __init__(self, value: float):
+        super().__init__(value=value)
+
+    @public
+    @property
+    def value(self) -> Optional[float]:
+        return self.value_inner
 
 
 @whitelist_for_serdes(storage_name="DagsterPipelineRunMetadataEntryData")
-class DagsterRunMetadataValue(
-    NamedTuple(
-        "_DagsterRunMetadataValue",
-        [
-            ("run_id", PublicAttr[str]),
-        ],
-    ),
-    MetadataValue[str],
-):
+class DagsterRunMetadataValue(DagsterModel, MetadataValue[str]):
     """Representation of a dagster run.
 
     Args:
         run_id (str): The run id
     """
 
-    def __new__(cls, run_id: str):
-        return super(DagsterRunMetadataValue, cls).__new__(cls, check.str_param(run_id, "run_id"))
+    run_id: PublicAttr[str]
+
+    def __init__(self, run_id: str):
+        super().__init__(run_id=run_id)
 
     @public
     @property
     def value(self) -> str:
         """str: The wrapped run id."""
         return self.run_id
 
 
 @whitelist_for_serdes
-class DagsterJobMetadataValue(
-    NamedTuple(
-        "_DagsterJobMetadataValue",
-        [
-            ("job_name", PublicAttr[str]),
-            ("location_name", PublicAttr[str]),
-            ("repository_name", PublicAttr[Optional[str]]),
-        ],
-    ),
-    MetadataValue["DagsterJobMetadataValue"],
-):
+class DagsterJobMetadataValue(DagsterModel, MetadataValue["DagsterJobMetadataValue"]):
     """Representation of a dagster run.
 
     Args:
         job_name (str): The job's name
         location_name (str): The job's code location name
         repository_name (Optional[str]): The job's repository name. If not provided, the job is
             assumed to be in the same repository as this object.
     """
 
-    def __new__(
-        cls,
+    job_name: PublicAttr[str]
+    location_name: PublicAttr[str]
+    repository_name: PublicAttr[Optional[str]]
+
+    def __init__(
+        self,
         job_name: str,
         location_name: str,
         repository_name: Optional[str] = None,
     ):
-        return super(DagsterJobMetadataValue, cls).__new__(
-            cls,
-            check.str_param(job_name, "job_name"),
-            check.str_param(location_name, "location_name"),
-            check.opt_str_param(repository_name, "repository_name"),
+        super().__init__(
+            job_name=job_name,
+            location_name=location_name,
+            repository_name=repository_name,
         )
 
     @public
     @property
     def value(self) -> Self:
         return self
 
 
 @whitelist_for_serdes(storage_name="DagsterAssetMetadataEntryData")
-class DagsterAssetMetadataValue(
-    NamedTuple("_DagsterAssetMetadataValue", [("asset_key", PublicAttr["AssetKey"])]),
-    MetadataValue["AssetKey"],
-):
+class DagsterAssetMetadataValue(DagsterModel, MetadataValue[AssetKey]):
     """Representation of a dagster asset.
 
     Args:
         asset_key (AssetKey): The dagster asset key
     """
 
-    def __new__(cls, asset_key: "AssetKey"):
-        from dagster._core.definitions.events import AssetKey
+    asset_key: PublicAttr[AssetKey]
 
-        return super(DagsterAssetMetadataValue, cls).__new__(
-            cls, check.inst_param(asset_key, "asset_key", AssetKey)
-        )
+    def __init__(self, asset_key: AssetKey):
+        super().__init__(asset_key=asset_key)
 
     @public
     @property
     def value(self) -> "AssetKey":
         """AssetKey: The wrapped :py:class:`AssetKey`."""
         return self.asset_key
 
 
 # This should be deprecated or fixed so that `value` does not return itself.
 @experimental
 @whitelist_for_serdes(storage_name="TableMetadataEntryData")
-class TableMetadataValue(
-    NamedTuple(
-        "_TableMetadataValue",
-        [
-            ("records", PublicAttr[Sequence[TableRecord]]),
-            ("schema", PublicAttr[TableSchema]),
-        ],
-    ),
-    MetadataValue["TableMetadataValue"],
-):
+class TableMetadataValue(DagsterModel, MetadataValue["TableMetadataValue"]):
     """Container class for table metadata entry data.
 
     Args:
         records (TableRecord): The data as a list of records (i.e. rows).
         schema (Optional[TableSchema]): A schema for the table.
 
     Example:
@@ -997,28 +875,31 @@
                 records=[
                     TableRecord({"column1": 5, "column2": "x"}),
                     TableRecord({"column1": 7, "column2": "y"}),
                 ]
             )
     """
 
+    records: PublicAttr[Sequence[TableRecord]]
+    schema_inner: TableSchema = Field(..., alias="schema")
+
     @public
     @staticmethod
     def infer_column_type(value: object) -> str:
         """str: Infer the :py:class:`TableSchema` column type that will be used for a value."""
         if isinstance(value, bool):
             return "bool"
         elif isinstance(value, int):
             return "int"
         elif isinstance(value, float):
             return "float"
         else:
             return "string"
 
-    def __new__(cls, records: Sequence[TableRecord], schema: Optional[TableSchema]):
+    def __init__(self, records: Sequence[TableRecord], schema: Optional[TableSchema] = None):
         check.sequence_param(records, "records", of_type=TableRecord)
         check.opt_inst_param(schema, "schema", TableSchema)
 
         if len(records) == 0:
             schema = check.not_none(schema, "schema must be provided if records is empty")
         else:
             columns = set(records[0].data.keys())
@@ -1029,285 +910,81 @@
             schema = schema or TableSchema(
                 columns=[
                     TableColumn(name=k, type=TableMetadataValue.infer_column_type(v))
                     for k, v in records[0].data.items()
                 ]
             )
 
-        return super(TableMetadataValue, cls).__new__(
-            cls,
-            records,
-            schema,
-        )
+        super().__init__(records=records, schema=schema)
+
+    @public
+    @property
+    def schema(self) -> TableSchema:
+        return self.schema_inner
 
     @public
     @property
     def value(self) -> Self:
         """TableMetadataValue: Identity function."""
         return self
 
 
 @whitelist_for_serdes(storage_name="TableSchemaMetadataEntryData")
-class TableSchemaMetadataValue(
-    NamedTuple("_TableSchemaMetadataValue", [("schema", PublicAttr[TableSchema])]),
-    MetadataValue[TableSchema],
-):
+class TableSchemaMetadataValue(DagsterModel, MetadataValue[TableSchema]):
     """Representation of a schema for arbitrary tabular data.
 
     Args:
         schema (TableSchema): The dictionary containing the schema representation.
     """
 
-    def __new__(cls, schema: TableSchema):
-        return super(TableSchemaMetadataValue, cls).__new__(
-            cls, check.inst_param(schema, "schema", TableSchema)
-        )
+    schema_inner: TableSchema = Field(..., alias="schema")
+
+    def __init__(self, schema: TableSchema):
+        super().__init__(schema=schema)
 
     @public
     @property
     def value(self) -> TableSchema:
         """TableSchema: The wrapped :py:class:`TableSchema`."""
-        return self.schema
+        return self.schema_inner
+
+    @public
+    @property
+    def schema(self) -> TableSchema:
+        return self.schema_inner
 
 
 @whitelist_for_serdes
-class TableColumnLineageMetadataValue(
-    NamedTuple(
-        "_TableColumnLineageMetadataValue", [("column_lineage", PublicAttr[TableColumnLineage])]
-    ),
-    MetadataValue[TableColumnLineage],
-):
+class TableColumnLineageMetadataValue(DagsterModel, MetadataValue[TableColumnLineage]):
     """Representation of the lineage of column inputs to column outputs of arbitrary tabular data.
 
     Args:
         column_lineage (TableColumnLineage): The lineage of column inputs to column outputs
             for the table.
     """
 
-    def __new__(cls, column_lineage: TableColumnLineage):
-        return super(TableColumnLineageMetadataValue, cls).__new__(
-            cls, check.inst_param(column_lineage, "column_lineage", TableColumnLineage)
-        )
+    column_lineage_inner: TableColumnLineage = Field(..., alias="column_lineage")
+
+    def __init__(self, column_lineage: TableColumnLineage):
+        super().__init__(column_lineage=column_lineage)
+
+    @public
+    @property
+    def column_lineage(self) -> TableColumnLineage:
+        return self.column_lineage_inner
 
     @public
     @property
     def value(self) -> TableColumnLineage:
         """TableSpec: The wrapped :py:class:`TableSpec`."""
-        return self.column_lineage
+        return self.column_lineage_inner
 
 
 @whitelist_for_serdes(storage_name="NullMetadataEntryData")
-class NullMetadataValue(NamedTuple("_NullMetadataValue", []), MetadataValue[None]):
+class NullMetadataValue(DagsterModel, MetadataValue[None]):
     """Representation of null."""
 
     @public
     @property
     def value(self) -> None:
         """None: The wrapped null value."""
         return None
-
-
-# ########################
-# ##### METADATA BACKCOMPAT
-# ########################
-
-# Metadata used to be represented as a `List[MetadataEntry]`, but that class has been deleted. But
-# we still serialize metadata dicts to the serialized representation of `List[MetadataEntry]` for
-# backcompat purposes.
-
-
-class MetadataFieldSerializer(FieldSerializer):
-    """Converts between metadata dict (new) and metadata entries list (old)."""
-
-    storage_name = "metadata_entries"
-    loaded_name = "metadata"
-
-    def pack(
-        self,
-        metadata_dict: Mapping[str, MetadataValue],
-        whitelist_map: WhitelistMap,
-        descent_path: str,
-    ) -> Sequence[Mapping[str, Any]]:
-        return [
-            {
-                "__class__": "EventMetadataEntry",
-                "label": k,
-                # MetadataValue itself can't inherit from NamedTuple and so isn't a PackableValue,
-                # but one of its subclasses will always be returned here.
-                "entry_data": pack_value(v, whitelist_map, descent_path),  # type: ignore
-                "description": None,
-            }
-            for k, v in metadata_dict.items()
-        ]
-
-    def unpack(
-        self,
-        metadata_entries: List["MetadataEntry"],
-        whitelist_map: WhitelistMap,
-        context: UnpackContext,
-    ) -> Mapping[str, MetadataValue]:
-        return {e.label: e.entry_data for e in metadata_entries}
-
-
-T_MetadataValue = TypeVar("T_MetadataValue", bound=MetadataValue, covariant=True)
-
-
-# NOTE: MetadataEntry is no longer accessible via the public API-- all metadata APIs use metadata
-# dicts. This clas shas only been preserved to adhere strictly to our backcompat guarantees. It is
-# still instantiated in the above `MetadataFieldSerializer` but that can easily be changed.
-@deprecated(
-    breaking_version="2.0",
-    additional_warn_text="Please use a dict with `MetadataValue` values instead.",
-)
-@deprecated_param(
-    param="entry_data", breaking_version="2.0", additional_warn_text="Use `value` instead."
-)
-@whitelist_for_serdes(storage_name="EventMetadataEntry")
-class MetadataEntry(
-    NamedTuple(
-        "_MetadataEntry",
-        [
-            ("label", PublicAttr[str]),
-            ("description", PublicAttr[Optional[str]]),
-            ("entry_data", PublicAttr[MetadataValue]),
-        ],
-    ),
-    Generic[T_MetadataValue],
-):
-    """A structure for describing metadata for Dagster events.
-
-    .. note:: This class is no longer usable in any Dagster API, and will be completely removed in 2.0.
-
-    Lists of objects of this type can be passed as arguments to Dagster events and will be displayed
-    in the Dagster UI and other tooling.
-
-    Should be yielded from within an IO manager to append metadata for a given input/output event.
-    For other event types, passing a dict with `MetadataValue` values to the `metadata` argument
-    is preferred.
-
-    Args:
-        label (str): Short display label for this metadata entry.
-        description (Optional[str]): A human-readable description of this metadata entry.
-        value (MetadataValue): Typed metadata entry data. The different types allow
-            for customized display in tools like the Dagster UI.
-    """
-
-    def __new__(
-        cls,
-        label: str,
-        description: Optional[str] = None,
-        entry_data: Optional["RawMetadataValue"] = None,
-        value: Optional["RawMetadataValue"] = None,
-    ):
-        value = cast(
-            RawMetadataValue,
-            normalize_renamed_param(
-                new_val=value,
-                new_arg="value",
-                old_val=entry_data,
-                old_arg="entry_data",
-            ),
-        )
-        value = normalize_metadata_value(value)
-
-        return super(MetadataEntry, cls).__new__(
-            cls,
-            check.str_param(label, "label"),
-            check.opt_str_param(description, "description"),
-            check.inst_param(value, "value", MetadataValue),
-        )
-
-    @property
-    def value(self):
-        """Alias of `entry_data`."""
-        return self.entry_data
-
-
-T_NamespacedMetadataSet = TypeVar("T_NamespacedMetadataSet", bound="NamespacedMetadataSet")
-
-
-class NamespacedMetadataSet(ABC, DagsterModel):
-    """Extend this class to define a set of metadata fields in the same namespace.
-
-    Supports splatting to a dictionary that can be placed inside a metadata argument along with
-    other dictionary-structured metadata.
-
-    .. code-block:: python
-
-        my_metadata: NamespacedMetadataSet = ...
-        return MaterializeResult(metadata={**my_metadata, ...})
-    """
-
-    @classmethod
-    @abstractmethod
-    def namespace(cls) -> str:
-        raise NotImplementedError()
-
-    @classmethod
-    def _namespaced_key(cls, key: str) -> str:
-        return f"{cls.namespace()}/{key}"
-
-    @staticmethod
-    def _strip_namespace_from_key(key: str) -> str:
-        return key.split("/", 1)[1]
-
-    def keys(self) -> AbstractSet[str]:
-        return {
-            self._namespaced_key(key)
-            for key in model_fields(self).keys()
-            # getattr returns the pydantic property on the subclass
-            if getattr(self, key) is not None
-        }
-
-    def __getitem__(self, key: str) -> Any:
-        # getattr returns the pydantic property on the subclass
-        return getattr(self, self._strip_namespace_from_key(key))
-
-    @classmethod
-    def extract(
-        cls: Type[T_NamespacedMetadataSet], metadata: Mapping[str, Any]
-    ) -> T_NamespacedMetadataSet:
-        """Extracts entries from the provided metadata dictionary into an instance of this class.
-
-        Ignores any entries in the metadata dictionary whose keys don't correspond to fields on this
-        class.
-
-        In general, the following should always pass:
-
-        .. code-block:: python
-
-            class MyMetadataSet(NamedspacedMetadataSet):
-                ...
-
-            metadata: MyMetadataSet  = ...
-            assert MyMetadataSet.extract(dict(metadata)) == metadata
-
-        Args:
-            metadata (Mapping[str, Any]): A dictionary of metadata entries.
-        """
-        kwargs = {}
-        for namespaced_key, value in metadata.items():
-            splits = namespaced_key.split("/")
-            if len(splits) == 2:
-                namespace, key = splits
-                if namespace == cls.namespace() and key in model_fields(cls):
-                    kwargs[key] = value.value if isinstance(value, MetadataValue) else value
-
-        return cls(**kwargs)
-
-
-class TableMetadataSet(NamespacedMetadataSet):
-    """Metadata entries that apply to definitions, observations, or materializations of assets that
-    are tables.
-
-    Args:
-        column_schema (Optional[TableSchema]): The schema of the columns in the table.
-        column_lineage (Optional[TableColumnLineage]): The lineage of column inputs to column
-            outputs for the table.
-    """
-
-    column_schema: Optional[TableSchema] = None
-    column_lineage: Optional[TableColumnLineage] = None
-
-    @classmethod
-    def namespace(cls) -> str:
-        return "dagster"
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/metadata/table.py` & `dagster-1.7.5/dagster/_core/definitions/metadata/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,14 +263,15 @@
 
 
 # ###########################
 # ##### TABLE COLUMN LINEAGE
 # ###########################
 
 
+@experimental(emit_runtime_warning=False)
 @whitelist_for_serdes
 class TableColumnDep(
     NamedTuple(
         "_TableColumnDep",
         [
             ("asset_key", PublicAttr[AssetKey]),
             ("column_name", PublicAttr[str]),
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.7.5/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.7.5/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/node_container.py` & `dagster-1.7.5/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/node_definition.py` & `dagster-1.7.5/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/observe.py` & `dagster-1.7.5/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/op_definition.py` & `dagster-1.7.5/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/op_invocation.py` & `dagster-1.7.5/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/op_selection.py` & `dagster-1.7.5/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/output.py` & `dagster-1.7.5/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/partition.py` & `dagster-1.7.5/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/partition_key_range.py` & `dagster-1.7.5/dagster/_core/definitions/partition_key_range.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/partition_mapping.py` & `dagster-1.7.5/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.7.5/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/policy.py` & `dagster-1.7.5/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/reconstruct.py` & `dagster-1.7.5/dagster/_core/definitions/reconstruct.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,21 +181,21 @@
         solids_to_execute = unpacked_dict.get("solids_to_execute")
         if solid_selection_str:
             unpacked_dict["op_selection"] = json.loads(solid_selection_str)
         elif solids_to_execute:
             unpacked_dict["op_selection"] = solids_to_execute
         return unpacked_dict
 
-    def after_pack(self, **packed_dict: Any) -> Dict[str, Any]:
-        if packed_dict["op_selection"]:
-            packed_dict["solid_selection_str"] = json.dumps(packed_dict["op_selection"]["__set__"])
-        else:
-            packed_dict["solid_selection_str"] = None
-        del packed_dict["op_selection"]
-        return packed_dict
+    def pack_items(self, *args, **kwargs):
+        for k, v in super().pack_items(*args, **kwargs):
+            if k == "op_selection":
+                new_v = json.dumps(v["__set__"]) if v else None
+                yield "solid_selection_str", new_v
+            else:
+                yield k, v
 
 
 @whitelist_for_serdes(
     serializer=ReconstructableJobSerializer,
     storage_name="ReconstructablePipeline",
     storage_field_names={
         "job_name": "pipeline_name",
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/remote_asset_graph.py` & `dagster-1.7.5/dagster/_core/definitions/remote_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.7.5/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.7.5/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.7.5/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.7.5/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.7.5/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.7.5/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.7.5/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/resource_annotation.py` & `dagster-1.7.5/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/resource_definition.py` & `dagster-1.7.5/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/resource_invocation.py` & `dagster-1.7.5/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/resource_requirement.py` & `dagster-1.7.5/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/result.py` & `dagster-1.7.5/dagster/_core/definitions/result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import NamedTuple, Optional, Sequence
+from typing import Mapping, NamedTuple, Optional, Sequence
 
 import dagster._check as check
 from dagster._annotations import PublicAttr, experimental
 from dagster._core.definitions.asset_check_result import AssetCheckResult
 from dagster._core.definitions.data_version import DataVersion
 
 from .events import (
@@ -16,41 +16,46 @@
     NamedTuple(
         "_AssetResult",
         [
             ("asset_key", PublicAttr[Optional[AssetKey]]),
             ("metadata", PublicAttr[Optional[RawMetadataMapping]]),
             ("check_results", PublicAttr[Sequence[AssetCheckResult]]),
             ("data_version", PublicAttr[Optional[DataVersion]]),
+            ("tags", PublicAttr[Optional[Mapping[str, str]]]),
         ],
     )
 ):
     """Base class for MaterializeResult and ObserveResult."""
 
     def __new__(
         cls,
         *,  # enforce kwargs
         asset_key: Optional[CoercibleToAssetKey] = None,
         metadata: Optional[RawMetadataMapping] = None,
         check_results: Optional[Sequence[AssetCheckResult]] = None,
         data_version: Optional[DataVersion] = None,
+        tags: Optional[Mapping[str, str]] = None,
     ):
+        from dagster._core.definitions.events import validate_asset_event_tags
+
         asset_key = AssetKey.from_coercible(asset_key) if asset_key else None
 
         return super().__new__(
             cls,
             asset_key=asset_key,
             metadata=check.opt_nullable_mapping_param(
                 metadata,
                 "metadata",
                 key_type=str,
             ),
             check_results=check.opt_sequence_param(
                 check_results, "check_results", of_type=AssetCheckResult
             ),
             data_version=check.opt_inst_param(data_version, "data_version", DataVersion),
+            tags=validate_asset_event_tags(tags),
         )
 
     def check_result_named(self, check_name: str) -> AssetCheckResult:
         for check_result in self.check_results:
             if check_result.check_name == check_name:
                 return check_result
 
@@ -64,14 +69,16 @@
 
     Attributes:
         asset_key (Optional[AssetKey]): Optional in @asset, required in @multi_asset to discern which asset this refers to.
         metadata (Optional[RawMetadataMapping]): Metadata to record with the corresponding AssetMaterialization event.
         check_results (Optional[Sequence[AssetCheckResult]]): Check results to record with the
             corresponding AssetMaterialization event.
         data_version (Optional[DataVersion]): The data version of the asset that was observed.
+        tags (Optional[Mapping[str, str]]): Tags to record with the corresponding
+            AssetMaterialization event.
     """
 
 
 @experimental
 class ObserveResult(AssetResult):
     """An object representing a successful observation of an asset. These can be returned from an
     @observable_source_asset decorated function to pass metadata.
@@ -79,8 +86,10 @@
     Attributes:
         asset_key (Optional[AssetKey]): The asset key. Optional to include.
         metadata (Optional[RawMetadataMapping]): Metadata to record with the corresponding
             AssetObservation event.
         check_results (Optional[Sequence[AssetCheckResult]]): Check results to record with the
             corresponding AssetObservation event.
         data_version (Optional[DataVersion]): The data version of the asset that was observed.
+        tags (Optional[Mapping[str, str]]): Tags to record with the corresponding AssetObservation
+            event.
     """
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/run_config.py` & `dagster-1.7.5/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/run_config_schema.py` & `dagster-1.7.5/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/run_request.py` & `dagster-1.7.5/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.7.5/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import functools
 import logging
+import os
 from contextlib import ExitStack
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Iterator,
@@ -89,14 +90,28 @@
 ]
 RunFailureSensorEvaluationFn: TypeAlias = Union[
     Callable[..., RawSensorEvaluationFunctionReturn],
     Callable[..., RawSensorEvaluationFunctionReturn],
 ]
 
 
+def _get_run_status_sensor_fetch_limit(monitor_all_code_locations: bool) -> int:
+    if monitor_all_code_locations:
+        # No need to overfetch if we are going to process everything
+        return _get_run_status_sensor_process_limit()
+
+    # Otherwise, fetch more than we are planning to process, under the assumption
+    # that some will be filtered out
+    return int(os.getenv("DAGSTER_RUN_STATUS_SENSOR_FETCH_LIMIT", "25"))
+
+
+def _get_run_status_sensor_process_limit() -> int:
+    return int(os.getenv("DAGSTER_RUN_STATUS_SENSOR_PROCESS_LIMIT", "5"))
+
+
 @whitelist_for_serdes(old_storage_names={"PipelineSensorCursor"})
 class RunStatusSensorCursor(
     NamedTuple(
         "_RunStatusSensorCursor",
         [
             ("record_id", int),
             # deprecated arg, used as a record cursor for the run-sharded sqlite implementation to
@@ -705,71 +720,88 @@
                 )
                 context.update_cursor(new_cursor.to_json())
                 yield SkipReason(f"Initiating {name}. Set cursor to {new_cursor}")
                 return
 
             sensor_cursor = RunStatusSensorCursor.from_json(context.cursor)
 
+            process_limit = _get_run_status_sensor_process_limit()
+
+            fetch_limit = _get_run_status_sensor_fetch_limit(
+                monitor_all_code_locations=cast(bool, monitor_all_code_locations)
+            )
+
             # Fetch events after the cursor id
             # * we move the cursor forward to the latest visited event's id to avoid revisits
             # * when the daemon is down, bc we persist the cursor info, we can go back to where we
-            #   left and backfill alerts for the qualified events (up to 5 at a time) during the downtime
+            #   left and backfill alerts for the qualified events during the downtime
             if sensor_cursor.update_timestamp and context.instance.event_log_storage.is_run_sharded:
                 # The run status sensor cursor has the timestamp set... and the event log storage
                 # is run sharded.  We need to query the index shard by timestamp instead of by
                 # record id (which is reindexed relative to some run sharded query).  When we update
                 # the cursor, we should omit the timestamp, since this API only queries the global
                 # index shard instead of the run shard.
                 event_records = context.instance.fetch_run_status_changes(
                     records_filter=RunStatusChangeRecordsFilter(
                         event_type=cast(RunStatusChangeEventType, event_type),
                         after_timestamp=cast(
                             datetime, pendulum.parse(sensor_cursor.update_timestamp)
                         ).timestamp(),
                     ),
                     ascending=True,
-                    limit=5,
+                    limit=fetch_limit,
                 ).records
             else:
                 # the cursor storage id is globally unique, either because the event log storage is
                 # not run sharded or because the cursor was set from an event returned from the
                 # index shard. When we update the cursor, we should omit the timestamp, since this
                 # API only queries the global index shard instead of the run shard.
                 event_records = context.instance.fetch_run_status_changes(
                     records_filter=RunStatusChangeRecordsFilter(
                         event_type=cast(RunStatusChangeEventType, event_type),
                         after_storage_id=sensor_cursor.record_id,
                     ),
                     ascending=True,
-                    limit=5,
+                    limit=fetch_limit,
                 ).records
 
+            run_ids_to_fetch = list(
+                set(event_record.event_log_entry.run_id for event_record in event_records)
+            )
+
+            run_records = (
+                {
+                    record.dagster_run.run_id: record
+                    for record in context.instance.get_run_records(
+                        filters=RunsFilter(run_ids=run_ids_to_fetch)
+                    )
+                }
+                if run_ids_to_fetch
+                else {}
+            )
+
+            num_processed_runs = 0
             for event_record in event_records:
                 event_log_entry = event_record.event_log_entry
                 storage_id = event_record.storage_id
                 record_timestamp = utc_datetime_from_timestamp(event_record.timestamp).isoformat()
 
-                # get run info
-                run_records = context.instance.get_run_records(
-                    filters=RunsFilter(run_ids=[event_log_entry.run_id])
-                )
-
                 # skip if we couldn't find the right run
-                if len(run_records) != 1:
+                if event_log_entry.run_id not in run_records:
                     context.update_cursor(
                         RunStatusSensorCursor(
                             record_id=storage_id, record_timestamp=record_timestamp
                         ).to_json()
                     )
                     continue
 
-                dagster_run = run_records[0].dagster_run
+                dagster_run = run_records[event_log_entry.run_id].dagster_run
                 job_match = False
 
-                # if monitor_all_repositories is provided, then we want to run the sensor for all jobs in all repositories
+                # if monitor_all_code_locations is provided, then we want to run the sensor for all jobs in all code locations
                 if monitor_all_code_locations:
                     job_match = True
 
                 code_location_name = (
                     context.code_location_origin.location_name
                     if context.code_location_origin
                     else None
@@ -823,14 +855,21 @@
                     context.update_cursor(
                         RunStatusSensorCursor(
                             record_id=storage_id, record_timestamp=record_timestamp
                         ).to_json()
                     )
                     continue
 
+                # Stop processing runs once you reach a matching job but have exceeded the limit
+                # (It's fine to keep advancing the cursor for runs that do not match)
+                if num_processed_runs >= process_limit:
+                    break
+
+                num_processed_runs = num_processed_runs + 1
+
                 serializable_error = None
 
                 resource_args_populated = validate_and_get_resource_dict(
                     context.resources, name, resource_arg_names
                 )
 
                 try:
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/schedule_definition.py` & `dagster-1.7.5/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/schema_change_checks.py` & `dagster-1.7.5/dagster/_core/definitions/asset_check_factories/schema_change_checks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import Dict, Mapping, Sequence, Union, cast
+from typing import Dict, Mapping, Sequence, Tuple, Union, cast
 
 from pydantic import BaseModel
 
 from dagster._annotations import experimental
+from dagster._core.instance import DagsterInstance
 
-from .asset_check_result import AssetCheckResult
-from .asset_check_spec import AssetCheckSeverity, AssetCheckSpec
-from .asset_checks import AssetChecksDefinition
-from .asset_key import AssetKey, CoercibleToAssetKey
-from .assets import AssetsDefinition, SourceAsset
-from .decorators.asset_check_decorator import multi_asset_check
-from .events import AssetMaterialization
-from .metadata import TableColumn, TableMetadataSet, TableSchema
+from ..asset_check_result import AssetCheckResult
+from ..asset_check_spec import AssetCheckKey, AssetCheckSeverity, AssetCheckSpec
+from ..asset_checks import AssetChecksDefinition
+from ..asset_key import AssetKey, CoercibleToAssetKey
+from ..assets import AssetsDefinition, SourceAsset
+from ..decorators.asset_check_decorator import multi_asset_check
+from ..events import AssetMaterialization
+from ..metadata import TableColumn, TableMetadataSet, TableSchema
+from .utils import unique_id_from_asset_keys
 
 
 @experimental
 def build_column_schema_change_checks(
     *,
     assets: Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]],
     severity: AssetCheckSeverity = AssetCheckSeverity.WARN,
@@ -36,80 +38,81 @@
         if isinstance(el, AssetsDefinition):
             asset_keys |= el.keys
         elif isinstance(el, SourceAsset):
             asset_keys.add(el.key)
         else:
             asset_keys.add(AssetKey.from_coercible(el))
 
+    def _result_for_check_key(
+        instance: DagsterInstance, asset_check_key: AssetCheckKey
+    ) -> Tuple[bool, str]:
+        materialization_records = instance.fetch_materializations(
+            limit=2, records_filter=asset_check_key.asset_key
+        ).records
+        if len(materialization_records) < 2:
+            return True, "The asset has been materialized fewer than 2 times"
+
+        record, prev_record = materialization_records
+        metadata = cast(AssetMaterialization, record.asset_materialization).metadata
+        prev_metadata = cast(AssetMaterialization, prev_record.asset_materialization).metadata
+
+        column_schema = TableMetadataSet.extract(metadata).column_schema
+        prev_column_schema = TableMetadataSet.extract(prev_metadata).column_schema
+        if column_schema is None:
+            return False, "Latest materialization has no column schema metadata"
+        if prev_column_schema is None:
+            return False, "Previous materialization has no column schema metadata"
+
+        diff = TableSchemaDiff.from_table_schemas(prev_column_schema, column_schema)
+        if diff.added_columns or diff.removed_columns or diff.column_type_changes:
+            description = "Column schema changed between previous and latest materialization."
+            if diff.added_columns:
+                description += (
+                    f"\n\nAdded columns: {', '.join(col.name for col in diff.added_columns)}"
+                )
+
+            if diff.removed_columns:
+                description += (
+                    f"\n\nRemoved columns: {', '.join(col.name for col in diff.removed_columns)}"
+                )
+
+            if diff.column_type_changes:
+                description += "\n\nColumn type changes:"
+                for col_name, type_change in diff.column_type_changes.items():
+                    description += (
+                        f"\n- {col_name}: {type_change.old_type} -> {type_change.new_type}"
+                    )
+
+            return False, description
+
+        return True, "No changes to column schema between previous and latest materialization"
+
     @multi_asset_check(
         specs=[
             AssetCheckSpec(
                 "column_schema_change",
                 asset=asset_key,
                 description="Checks whether there are changes to column schema between the asset's "
                 " two most recent materializations",
             )
             for asset_key in asset_keys
         ],
         can_subset=True,
+        name=unique_id_from_asset_keys(list(asset_keys)),
     )
     def _checks(context):
-        instance = context.instance
         for asset_check_key in context.selected_asset_check_keys:
-            materialization_records = instance.fetch_materializations(
-                limit=2, records_filter=asset_check_key.asset_key
-            ).records
-            if len(materialization_records) < 2:
-                yield AssetCheckResult(
-                    passed=True, description="The asset has been materialized fewer than 2 times"
-                )
-            else:
-                record, prev_record = materialization_records
-                metadata = cast(AssetMaterialization, record.asset_materialization).metadata
-                prev_metadata = cast(
-                    AssetMaterialization, prev_record.asset_materialization
-                ).metadata
-
-                column_schema = TableMetadataSet.extract(metadata).column_schema
-                prev_column_schema = TableMetadataSet.extract(prev_metadata).column_schema
-                if column_schema is None:
-                    yield AssetCheckResult(
-                        passed=False,
-                        description="Latest materialization has no column schema metadata",
-                    )
-                if prev_column_schema is None:
-                    yield AssetCheckResult(
-                        passed=False,
-                        description="Previous materialization has no column schema metadata",
-                    )
-
-                diff = TableSchemaDiff.from_table_schemas(prev_column_schema, column_schema)
-                if diff.added_columns or diff.removed_columns or diff.column_type_changes:
-                    description = (
-                        "Column schema changed between previous and latest materialization."
-                    )
-                    if diff.added_columns:
-                        description += f"\n\nAdded columns: {', '.join(col.name for col in diff.added_columns)}"
-
-                    if diff.removed_columns:
-                        description += f"\n\nRemoved columns: {', '.join(col.name for col in diff.removed_columns)}"
-
-                    if diff.column_type_changes:
-                        description += "\n\nColumn type changes:"
-                        for col_name, type_change in diff.column_type_changes.items():
-                            description += (
-                                f"\n- {col_name}: {type_change.old_type} -> {type_change.new_type}"
-                            )
-
-                    yield AssetCheckResult(passed=False, severity=severity, description=description)
-                else:
-                    yield AssetCheckResult(
-                        passed=True,
-                        description="No changes to column schema between previous and latest materialization",
-                    )
+            passed, description = _result_for_check_key(context.instance, asset_check_key)
+            yield AssetCheckResult(
+                passed=passed,
+                description=description,
+                severity=severity,
+                check_name=asset_check_key.name,
+                asset_key=asset_check_key.asset_key,
+            )
 
     return [_checks]
 
 
 class TypeChange(BaseModel):
     old_type: str
     new_type: str
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.7.5/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/selector.py` & `dagster-1.7.5/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/sensor_definition.py` & `dagster-1.7.5/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/source_asset.py` & `dagster-1.7.5/dagster/_core/definitions/source_asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 )
 from dagster._core.errors import (
     DagsterInvalidDefinitionError,
     DagsterInvalidInvocationError,
     DagsterInvalidObservationError,
 )
 
-from .utils import validate_definition_tags
+from .utils import validate_tags_strict
 
 if TYPE_CHECKING:
     from dagster._core.definitions.decorators.op_decorator import (
         DecoratedOpFunction,
     )
 from dagster._core.storage.io_manager import IOManagerDefinition
 from dagster._utils.merger import merge_dicts
@@ -229,15 +229,15 @@
             wrap_resources_for_execution,
         )
 
         self.key = AssetKey.from_coercible(key)
         metadata = check.opt_mapping_param(metadata, "metadata", key_type=str)
         self.raw_metadata = metadata
         self.metadata = normalize_metadata(metadata, allow_invalid=True)
-        self.tags = validate_definition_tags(tags) or {}
+        self.tags = validate_tags_strict(tags) or {}
 
         resource_defs_dict = dict(check.opt_mapping_param(resource_defs, "resource_defs"))
         if io_manager_def:
             if not io_manager_key:
                 io_manager_key = self.key.to_python_identifier("io_manager")
 
             if (
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/step_launcher.py` & `dagster-1.7.5/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/target.py` & `dagster-1.7.5/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.7.5/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.7.5/dagster/_core/definitions/time_window_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.7.5/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/definitions/utils.py` & `dagster-1.7.5/dagster/_core/definitions/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,38 +174,41 @@
     return bool(VALID_DEFINITION_TAG_KEY_REGEX.match(key))
 
 
 def is_valid_definition_tag_value(key: str) -> bool:
     return bool(VALID_DEFINITION_TAG_VALUE_REGEX.match(key))
 
 
-def validate_definition_tags(tags: Optional[Mapping[str, str]]) -> Optional[Mapping[str, str]]:
-    """More restrictive than validate_tags."""
+def validate_tags_strict(tags: Optional[Mapping[str, str]]) -> Optional[Mapping[str, str]]:
     if tags is None:
         return tags
 
     for key, value in tags.items():
-        if not isinstance(key, str):
-            raise DagsterInvalidDefinitionError("Tag keys must be strings")
+        validate_tag_strict(key, value)
 
-        if not isinstance(value, str):
-            raise DagsterInvalidDefinitionError("Tag values must be strings")
+    return tags
 
-        if not is_valid_definition_tag_key(key):
-            raise DagsterInvalidDefinitionError(
-                f"Invalid tag key: {key}. {VALID_DEFINITION_TAG_KEY_EXPLANATION}"
-            )
-
-        if not is_valid_definition_tag_value(value):
-            raise DagsterInvalidDefinitionError(
-                f"Invalid tag value: {value}. Allowed characters: alpha-numeric, '_', '-', '.'. "
-                "Must have <= 63 characters."
-            )
 
-    return tags
+def validate_tag_strict(key: str, value: str) -> None:
+    if not isinstance(key, str):
+        raise DagsterInvalidDefinitionError("Tag keys must be strings")
+
+    if not isinstance(value, str):
+        raise DagsterInvalidDefinitionError("Tag values must be strings")
+
+    if not is_valid_definition_tag_key(key):
+        raise DagsterInvalidDefinitionError(
+            f"Invalid tag key: {key}. {VALID_DEFINITION_TAG_KEY_EXPLANATION}"
+        )
+
+    if not is_valid_definition_tag_value(value):
+        raise DagsterInvalidDefinitionError(
+            f"Invalid tag value: {value}, for key: {key}. Allowed characters: alpha-numeric, '_', '-', '.'. "
+            "Must have <= 63 characters."
+        )
 
 
 def validate_group_name(group_name: Optional[str]) -> str:
     """Ensures a string name is valid and returns a default if no name provided."""
     if group_name:
         check_valid_chars(group_name)
         return group_name
```

### Comparing `dagster-1.7.4/dagster/_core/definitions/version_strategy.py` & `dagster-1.7.5/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/errors.py` & `dagster-1.7.5/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/event_api.py` & `dagster-1.7.5/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/events/__init__.py` & `dagster-1.7.5/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/events/log.py` & `dagster-1.7.5/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/events/utils.py` & `dagster-1.7.5/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/api.py` & `dagster-1.7.5/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/asset_backfill.py` & `dagster-1.7.5/dagster/_core/execution/asset_backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,17 @@
         )
 
     def with_latest_storage_id(self, latest_storage_id: Optional[int]) -> "AssetBackfillData":
         return self._replace(
             latest_storage_id=latest_storage_id,
         )
 
+    def with_requested_runs_for_target_roots(self, requested_runs_for_target_roots: bool):
+        return self._replace(requested_runs_for_target_roots=requested_runs_for_target_roots)
+
     def is_complete(self) -> bool:
         """The asset backfill is complete when all runs to be requested have finished (success,
         failure, or cancellation). Since the AssetBackfillData object stores materialization states
         per asset partition, the daemon continues to update the backfill data until all runs have
         finished in order to display the final partition statuses in the UI.
         """
         return (
@@ -723,18 +726,21 @@
             asset_backfill_iteration_result.backfill_data.replace_requested_subset(
                 submitted_partitions
             )
         )
         if retryable_error_raised:
             # Code server became unavailable mid-backfill. Rewind the cursor back to the cursor
             # from the previous iteration, to allow next iteration to reevaluate the same
-            # events.
+            # events. If the previous iteration had not requested the target roots, this will also
+            # ensure the next iteration requests the target roots
             backfill_data_with_submitted_runs = (
                 backfill_data_with_submitted_runs.with_latest_storage_id(
                     previous_asset_backfill_data.latest_storage_id
+                ).with_requested_runs_for_target_roots(
+                    previous_asset_backfill_data.requested_runs_for_target_roots
                 )
             )
 
         # Refetch, in case the backfill was requested for cancellation in the meantime
         backfill = cast(PartitionBackfill, instance.get_backfill(backfill_id))
         updated_backfill = backfill.with_asset_backfill_data(
             backfill_data_with_submitted_runs,
@@ -1186,17 +1192,21 @@
 
     This is a generator so that we can return control to the daemon and let it heartbeat during
     expensive operations.
     """
     initial_candidates: Set[AssetKeyPartitionKey] = set()
     request_roots = not asset_backfill_data.requested_runs_for_target_roots
     if request_roots:
-        initial_candidates.update(
-            asset_backfill_data.get_target_root_asset_partitions(instance_queryer)
-        )
+        target_roots = asset_backfill_data.get_target_root_asset_partitions(instance_queryer)
+        # Because the code server may have failed while requesting roots, some roots may have
+        # already been requested. Checking here will reduce the amount of BFS work later in the iteration.
+        not_yet_requested = [
+            root for root in target_roots if root not in asset_backfill_data.requested_subset
+        ]
+        initial_candidates.update(not_yet_requested)
 
         yield None
 
         updated_materialized_subset = AssetGraphSubset()
         failed_and_downstream_subset = AssetGraphSubset()
         next_latest_storage_id = _get_next_latest_storage_id(instance_queryer)
     else:
```

### Comparing `dagster-1.7.4/dagster/_core/execution/backfill.py` & `dagster-1.7.5/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/build_resources.py` & `dagster-1.7.5/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/compute_logs.py` & `dagster-1.7.5/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/context/compute.py` & `dagster-1.7.5/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/context/data_version_cache.py` & `dagster-1.7.5/dagster/_core/execution/context/data_version_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/context/hook.py` & `dagster-1.7.5/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/context/init.py` & `dagster-1.7.5/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/context/input.py` & `dagster-1.7.5/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/context/invocation.py` & `dagster-1.7.5/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/context/logger.py` & `dagster-1.7.5/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/context/output.py` & `dagster-1.7.5/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/context/system.py` & `dagster-1.7.5/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/context_creation_job.py` & `dagster-1.7.5/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/execute_in_process.py` & `dagster-1.7.5/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.7.5/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/execution_result.py` & `dagster-1.7.5/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/host_mode.py` & `dagster-1.7.5/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/job_backfill.py` & `dagster-1.7.5/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/job_execution_result.py` & `dagster-1.7.5/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/memoization.py` & `dagster-1.7.5/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/active.py` & `dagster-1.7.5/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/compute.py` & `dagster-1.7.5/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.7.5/dagster/_core/execution/plan/compute_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,14 +352,15 @@
 
                 with disable_dagster_warnings():
                     yield Output(
                         output_name=output_def.name,
                         value=element.value,
                         metadata=element.metadata,
                         data_version=element.data_version,
+                        tags=element.tags,
                     )
             else:
                 # If annotation indicates a generic output annotation, and an
                 # output object was not received, throw an error.
                 if is_generic_output_annotation(annotation):
                     raise DagsterInvariantViolationError(
                         f"Error with output for {context.describe_op()}: output "
```

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.7.5/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/execute_step.py` & `dagster-1.7.5/dagster/_core/execution/plan/execute_step.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     Union,
     cast,
 )
 
 from typing_extensions import TypedDict
 
 import dagster._check as check
-from dagster import AssetCheckSeverity
 from dagster._core.definitions import (
     AssetCheckEvaluation,
+    AssetCheckSeverity,
     AssetKey,
     AssetMaterialization,
     AssetObservation,
     ExpectationResult,
     Output,
     OutputDefinition,
     TypeCheck,
@@ -122,14 +122,15 @@
             )
 
         yield Output(
             value=None,
             output_name=output_name,
             metadata=user_event.metadata,
             data_version=user_event.data_version,
+            tags=user_event.tags,
         )
     elif isinstance(user_event, AssetCheckResult):
         asset_check_evaluation = user_event.to_asset_check_evaluation(step_context)
         spec = check.not_none(
             step_context.job_def.asset_layer.get_spec_for_asset_check(
                 step_context.node_handle.root, asset_check_evaluation.asset_check_key
             ),
@@ -272,14 +273,15 @@
                     value=output.value,
                     output_name=output.output_name,
                     metadata={
                         **output.metadata,
                         **normalize_metadata(metadata or {}),
                     },
                     data_version=output.data_version,
+                    tags=output.tags,
                 )
         else:
             if not output_def.is_dynamic:
                 raise DagsterInvariantViolationError(
                     f"Compute for {op_label} yielded a DynamicOutput, but did not use "
                     "DynamicOutputDefinition."
                 )
@@ -654,14 +656,16 @@
         assert isinstance(output, Output)
         tags = (
             _build_data_version_observation_tags(output.data_version) if output.data_version else {}
         )
     else:
         tags = {}
 
+    all_tags = {**tags, **((output.tags if not isinstance(output, DynamicOutput) else None) or {})}
+
     backfill_id = step_context.get_tag(BACKFILL_ID_TAG)
     if backfill_id:
         tags[BACKFILL_ID_TAG] = backfill_id
 
     if execution_type == AssetExecutionType.MATERIALIZATION:
         event_class = AssetMaterialization
         event_class = AssetMaterialization
@@ -669,29 +673,29 @@
         event_class = AssetObservation
     else:
         check.failed(f"Unexpected asset execution type {execution_type}")
 
     if asset_partitions:
         for partition in asset_partitions:
             with disable_dagster_warnings():
-                tags.update(
+                all_tags.update(
                     get_tags_from_multi_partition_key(partition)
                     if isinstance(partition, MultiPartitionKey)
                     else {}
                 )
 
                 yield event_class(
                     asset_key=asset_key,
                     partition=partition,
                     metadata=all_metadata,
-                    tags=tags,
+                    tags=all_tags,
                 )
     else:
         with disable_dagster_warnings():
-            yield event_class(asset_key=asset_key, metadata=all_metadata, tags=tags)
+            yield event_class(asset_key=asset_key, metadata=all_metadata, tags=all_tags)
 
 
 def _get_code_version(asset_key: AssetKey, step_context: StepExecutionContext) -> str:
     return (
         step_context.job_def.asset_layer.get(asset_key).code_version
         or step_context.dagster_run.run_id
     )
```

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/external_step.py` & `dagster-1.7.5/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/handle.py` & `dagster-1.7.5/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/inputs.py` & `dagster-1.7.5/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/instance_concurrency_context.py` & `dagster-1.7.5/dagster/_core/execution/plan/instance_concurrency_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.7.5/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/objects.py` & `dagster-1.7.5/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/outputs.py` & `dagster-1.7.5/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/plan.py` & `dagster-1.7.5/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/state.py` & `dagster-1.7.5/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/step.py` & `dagster-1.7.5/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/plan/utils.py` & `dagster-1.7.5/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.7.5/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/resolve_versions.py` & `dagster-1.7.5/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/resources_init.py` & `dagster-1.7.5/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/retries.py` & `dagster-1.7.5/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.7.5/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/stats.py` & `dagster-1.7.5/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/submit_asset_runs.py` & `dagster-1.7.5/dagster/_core/execution/submit_asset_runs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import logging
+import sys
 import time
-from typing import Dict, Iterator, List, NamedTuple, Optional, Sequence, Tuple, cast
+from typing import AbstractSet, Dict, Iterator, List, NamedTuple, Optional, Sequence, Tuple, cast
 
 import dagster._check as check
 from dagster._core.definitions.asset_job import is_base_asset_job_name
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.partition import PartitionsDefinition
 from dagster._core.definitions.remote_asset_graph import RemoteAssetGraph
 from dagster._core.definitions.run_request import RunRequest
 from dagster._core.definitions.selector import JobSubsetSelector
 from dagster._core.errors import (
     DagsterCodeLocationLoadError,
     DagsterInvalidSubsetError,
+    DagsterUserCodeProcessError,
     DagsterUserCodeUnreachableError,
 )
 from dagster._core.instance import DagsterInstance
 from dagster._core.remote_representation import ExternalExecutionPlan, ExternalJob
 from dagster._core.snap import ExecutionPlanSnapshot
 from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus
 from dagster._core.workspace.context import BaseWorkspaceRequestContext, IWorkspaceProcessContext
@@ -36,25 +38,25 @@
     job_names = set(asset_graph.get_materialization_job_names(asset_keys[0]))
     for asset_key in asset_keys[1:]:
         job_names &= set(asset_graph.get_materialization_job_names(asset_key))
 
     return next(job_name for job_name in job_names if is_base_asset_job_name(job_name))
 
 
-def _execution_plan_targets_asset_selection(
-    execution_plan_snapshot: ExecutionPlanSnapshot, asset_selection: Sequence[AssetKey]
-) -> bool:
+def _get_execution_plan_asset_keys(
+    execution_plan_snapshot: ExecutionPlanSnapshot,
+) -> AbstractSet[AssetKey]:
     output_asset_keys = set()
     for step in execution_plan_snapshot.steps:
         if step.key in execution_plan_snapshot.step_keys_to_execute:
             for output in step.outputs:
                 asset_key = check.not_none(output.properties).asset_key
                 if asset_key:
                     output_asset_keys.add(asset_key)
-    return all(key in output_asset_keys for key in asset_selection)
+    return output_asset_keys
 
 
 def _get_job_execution_data_from_run_request(
     asset_graph: RemoteAssetGraph,
     run_request: RunRequest,
     instance: DagsterInstance,
     workspace: BaseWorkspaceRequestContext,
@@ -126,78 +128,104 @@
     a valid ExecutionPlan by reloading the workspace.
     """
     from dagster._daemon.controller import RELOAD_WORKSPACE_INTERVAL
 
     if not run_request.asset_selection:
         check.failed("Expected RunRequest to have an asset selection")
 
-    for _ in range(EXECUTION_PLAN_CREATION_RETRIES + 1):
+    for i in range(EXECUTION_PLAN_CREATION_RETRIES + 1):
+        should_retry = False
+        execution_data = None
+
+        # retry until the execution plan targets the asset selection
         try:
             # create a new request context for each run in case the code location server
             # is swapped out in the middle of the submission process
             workspace = workspace_process_context.create_request_context()
             execution_data = _get_job_execution_data_from_run_request(
                 asset_graph,
                 run_request,
                 instance,
                 workspace=workspace,
                 run_request_execution_data_cache=run_request_execution_data_cache,
             )
-            check_for_debug_crash(debug_crash_flags, "EXECUTION_PLAN_CREATED")
-            check_for_debug_crash(debug_crash_flags, f"EXECUTION_PLAN_CREATED_{run_request_index}")
 
-            # retry until the execution plan targets the asset selection
-            if _execution_plan_targets_asset_selection(
-                execution_data.external_execution_plan.execution_plan_snapshot,
-                check.not_none(run_request.asset_selection),
+        except (DagsterInvalidSubsetError, DagsterUserCodeProcessError):
+            logger.warning(
+                "Error while generating the execution plan, possibly because the code server is "
+                "out of sync with the daemon. The daemon periodically refreshes its representation "
+                f"of the workspace every {RELOAD_WORKSPACE_INTERVAL} seconds - pausing long enough "
+                "to ensure that that refresh will happen to bring them back in sync.",
+                exc_info=sys.exc_info(),
+            )
+            should_retry = True
+
+        check_for_debug_crash(debug_crash_flags, "EXECUTION_PLAN_CREATED")
+        check_for_debug_crash(debug_crash_flags, f"EXECUTION_PLAN_CREATED_{run_request_index}")
+
+        if not should_retry:
+            execution_plan_asset_keys = _get_execution_plan_asset_keys(
+                check.not_none(execution_data).external_execution_plan.execution_plan_snapshot
+            )
+
+            if not all(
+                key in execution_plan_asset_keys
+                for key in check.not_none(run_request.asset_selection)
             ):
-                external_job = execution_data.external_job
-                external_execution_plan = execution_data.external_execution_plan
-                partitions_def = execution_data.partitions_def
-
-                run = instance.create_run(
-                    job_snapshot=external_job.job_snapshot,
-                    execution_plan_snapshot=external_execution_plan.execution_plan_snapshot,
-                    parent_job_snapshot=external_job.parent_job_snapshot,
-                    job_name=external_job.name,
-                    run_id=run_id,
-                    resolved_op_selection=None,
-                    op_selection=None,
-                    run_config={},
-                    step_keys_to_execute=None,
-                    tags=run_request.tags,
-                    root_run_id=None,
-                    parent_run_id=None,
-                    status=DagsterRunStatus.NOT_STARTED,
-                    external_job_origin=external_job.get_external_origin(),
-                    job_code_origin=external_job.get_python_origin(),
-                    asset_selection=frozenset(run_request.asset_selection),
-                    asset_check_selection=None,
-                    asset_job_partitions_def=partitions_def,
+                logger.warning(
+                    f"Execution plan targeted the following keys: {execution_plan_asset_keys}, "
+                    "which did not include all assets on the run request, "
+                    "possibly because the code server is out of sync with the daemon. The daemon "
+                    "periodically refreshes its representation of the workspace every "
+                    f"{RELOAD_WORKSPACE_INTERVAL} seconds - pausing long enough "
+                    "to ensure that that refresh will happen to bring them back in sync.",
                 )
 
-                return run
-        except DagsterInvalidSubsetError:
-            pass
-
-        logger.warning(
-            "Execution plan is out of sync with the workspace. Pausing run submission for "
-            f"{RELOAD_WORKSPACE_INTERVAL} to allow the execution plan to rebuild with the updated workspace."
-        )
-        # Sleep for RELOAD_WORKSPACE_INTERVAL seconds since the workspace can be refreshed
-        # at most once every interval
-        time.sleep(RELOAD_WORKSPACE_INTERVAL)
-        # Clear the execution plan cache as this data is no longer valid
-        run_request_execution_data_cache = {}
-
-        # If the execution plan does not targets the asset selection, the asset graph
-        # likely is outdated and targeting the wrong job, refetch the asset
-        # graph from the workspace
-        workspace = workspace_process_context.create_request_context()
-        asset_graph = workspace.asset_graph
+                should_retry = True
+
+        if not should_retry:
+            external_job = check.not_none(execution_data).external_job
+            external_execution_plan = check.not_none(execution_data).external_execution_plan
+            partitions_def = check.not_none(execution_data).partitions_def
+
+            run = instance.create_run(
+                job_snapshot=external_job.job_snapshot,
+                execution_plan_snapshot=external_execution_plan.execution_plan_snapshot,
+                parent_job_snapshot=external_job.parent_job_snapshot,
+                job_name=external_job.name,
+                run_id=run_id,
+                resolved_op_selection=None,
+                op_selection=None,
+                run_config={},
+                step_keys_to_execute=None,
+                tags=run_request.tags,
+                root_run_id=None,
+                parent_run_id=None,
+                status=DagsterRunStatus.NOT_STARTED,
+                external_job_origin=external_job.get_external_origin(),
+                job_code_origin=external_job.get_python_origin(),
+                asset_selection=frozenset(run_request.asset_selection),
+                asset_check_selection=None,
+                asset_job_partitions_def=partitions_def,
+            )
+
+            return run
+
+        if i < EXECUTION_PLAN_CREATION_RETRIES:
+            # Sleep for RELOAD_WORKSPACE_INTERVAL seconds since the workspace can be refreshed
+            # at most once every interval
+            time.sleep(RELOAD_WORKSPACE_INTERVAL)
+            # Clear the execution plan cache as this data is no longer valid
+            run_request_execution_data_cache = {}
+
+            # If the execution plan does not targets the asset selection, the asset graph
+            # likely is outdated and targeting the wrong job, refetch the asset
+            # graph from the workspace
+            workspace = workspace_process_context.create_request_context()
+            asset_graph = workspace.asset_graph
 
     check.failed(
         f"Failed to target asset selection {run_request.asset_selection} in run after retrying."
     )
 
 
 def submit_asset_run(
```

### Comparing `dagster-1.7.4/dagster/_core/execution/tags.py` & `dagster-1.7.5/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/validate_run_config.py` & `dagster-1.7.5/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/watch_orphans.py` & `dagster-1.7.5/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/execution/with_resources.py` & `dagster-1.7.5/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/executor/base.py` & `dagster-1.7.5/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/executor/child_process_executor.py` & `dagster-1.7.5/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/executor/in_process.py` & `dagster-1.7.5/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/executor/init.py` & `dagster-1.7.5/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/executor/multiprocess.py` & `dagster-1.7.5/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.7.5/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.7.5/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/instance/__init__.py` & `dagster-1.7.5/dagster/_core/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/instance/config.py` & `dagster-1.7.5/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/instance/ref.py` & `dagster-1.7.5/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/instance_for_test.py` & `dagster-1.7.5/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/launcher/base.py` & `dagster-1.7.5/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.7.5/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.7.5/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/log_manager.py` & `dagster-1.7.5/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/nux.py` & `dagster-1.7.5/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/op_concurrency_limits_counter.py` & `dagster-1.7.5/dagster/_core/op_concurrency_limits_counter.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/origin.py` & `dagster-1.7.5/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/pipes/client.py` & `dagster-1.7.5/dagster/_core/pipes/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/pipes/context.py` & `dagster-1.7.5/dagster/_core/pipes/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/pipes/subprocess.py` & `dagster-1.7.5/dagster/_core/pipes/subprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/pipes/utils.py` & `dagster-1.7.5/dagster/_core/pipes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/remote_representation/__init__.py` & `dagster-1.7.5/dagster/_core/remote_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/remote_representation/code_location.py` & `dagster-1.7.5/dagster/_core/remote_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/remote_representation/external.py` & `dagster-1.7.5/dagster/_core/remote_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/remote_representation/external_data.py` & `dagster-1.7.5/dagster/_core/remote_representation/external_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/remote_representation/feature_flags.py` & `dagster-1.7.5/dagster/_core/remote_representation/feature_flags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/remote_representation/grpc_server_registry.py` & `dagster-1.7.5/dagster/_core/remote_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/remote_representation/grpc_server_state_subscriber.py` & `dagster-1.7.5/dagster/_core/remote_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/remote_representation/handle.py` & `dagster-1.7.5/dagster/_core/remote_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/remote_representation/historical.py` & `dagster-1.7.5/dagster/_core/remote_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/remote_representation/job_index.py` & `dagster-1.7.5/dagster/_core/remote_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/remote_representation/origin.py` & `dagster-1.7.5/dagster/_core/remote_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/remote_representation/represented.py` & `dagster-1.7.5/dagster/_core/remote_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/run_coordinator/base.py` & `dagster-1.7.5/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.7.5/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.7.5/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/scheduler/__init__.py` & `dagster-1.7.5/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/scheduler/execution.py` & `dagster-1.7.5/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/scheduler/instigation.py` & `dagster-1.7.5/dagster/_core/scheduler/instigation.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from typing import AbstractSet, Any, List, Mapping, NamedTuple, Optional, Sequence, Union
 
 import pendulum
 from typing_extensions import TypeAlias
 
 import dagster._check as check
 from dagster._core.definitions import RunRequest
-from dagster._core.definitions.asset_condition.asset_condition import (
-    AssetConditionEvaluationWithRunIds,
-)
 from dagster._core.definitions.auto_materialize_rule_evaluation import (
     deserialize_auto_materialize_asset_evaluation_to_asset_condition_evaluation_with_run_ids,
 )
+from dagster._core.definitions.declarative_scheduling.serialized_objects import (
+    AssetConditionEvaluationWithRunIds,
+)
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.partition import PartitionsDefinition
 
 # re-export
 from dagster._core.definitions.run_request import (
     InstigatorType as InstigatorType,
     SkipReason as SkipReason,
```

### Comparing `dagster-1.7.4/dagster/_core/scheduler/scheduler.py` & `dagster-1.7.5/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/secrets/env_file.py` & `dagster-1.7.5/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/selector/subset_selector.py` & `dagster-1.7.5/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/snap/__init__.py` & `dagster-1.7.5/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/snap/dagster_types.py` & `dagster-1.7.5/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/snap/dep_snapshot.py` & `dagster-1.7.5/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.7.5/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/snap/job_snapshot.py` & `dagster-1.7.5/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/snap/mode.py` & `dagster-1.7.5/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/snap/node.py` & `dagster-1.7.5/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.7.5/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/DEVELOPING.md` & `dagster-1.7.5/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/README.md` & `dagster-1.7.5/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/env.py` & `dagster-1.7.5/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py` & `dagster-1.7.5/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/asset_check_execution_record.py` & `dagster-1.7.5/dagster/_core/storage/asset_check_execution_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import enum
 from typing import NamedTuple, Optional
 
 import dagster._check as check
-from dagster import EventLogEntry
-from dagster._core.events import DagsterEventType
+from dagster._core.events.log import DagsterEventType, EventLogEntry
 from dagster._serdes.serdes import deserialize_value
 from dagster._utils import datetime_as_float
 
 
 class AssetCheckInstanceSupport(enum.Enum):
     """Reasons why a dagster instance might not support checks."""
```

### Comparing `dagster-1.7.4/dagster/_core/storage/asset_value_loader.py` & `dagster-1.7.5/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/base_storage.py` & `dagster-1.7.5/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.7.5/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/captured_log_manager.py` & `dagster-1.7.5/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.7.5/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/compute_log_manager.py` & `dagster-1.7.5/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/config.py` & `dagster-1.7.5/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/dagster_run.py` & `dagster-1.7.5/dagster/_core/storage/dagster_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/db_io_manager.py` & `dagster-1.7.5/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/event_log/__init__.py` & `dagster-1.7.5/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/event_log/base.py` & `dagster-1.7.5/dagster/_core/storage/event_log/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 )
 from dagster._core.instance import MayHaveInstanceWeakref, T_DagsterInstance
 from dagster._core.storage.asset_check_execution_record import AssetCheckExecutionRecord
 from dagster._core.storage.dagster_run import DagsterRunStatsSnapshot
 from dagster._core.storage.sql import AlembicVersion
 from dagster._utils import PrintFn
 from dagster._utils.concurrency import ConcurrencyClaimStatus, ConcurrencyKeyInfo
+from dagster._utils.warnings import deprecation_warning
 
 if TYPE_CHECKING:
     from dagster._core.events.log import EventLogEntry
     from dagster._core.storage.partition_status_cache import AssetStatusCacheValue
 
 
 class EventLogConnection(NamedTuple):
@@ -56,25 +57,29 @@
             ("last_materialization_record", Optional[EventLogRecord]),
             ("last_run_id", Optional[str]),
             ("asset_details", Optional[AssetDetails]),
             ("cached_status", Optional["AssetStatusCacheValue"]),
             # This is an optional field which can be used for more performant last observation
             # queries if the underlying storage supports it
             ("last_observation_record", Optional[EventLogRecord]),
+            ("last_planned_materialization_storage_id", Optional[int]),
+            ("last_planned_materialization_run_id", Optional[str]),
         ],
     )
 ):
     def __new__(
         cls,
         asset_key: AssetKey,
         last_materialization_record: Optional[EventLogRecord] = None,
         last_run_id: Optional[str] = None,
         asset_details: Optional[AssetDetails] = None,
         cached_status: Optional["AssetStatusCacheValue"] = None,
         last_observation_record: Optional[EventLogRecord] = None,
+        last_planned_materialization_storage_id: Optional[int] = None,
+        last_planned_materialization_run_id: Optional[str] = None,
     ):
         from dagster._core.storage.partition_status_cache import AssetStatusCacheValue
 
         return super(AssetEntry, cls).__new__(
             cls,
             asset_key=check.inst_param(asset_key, "asset_key", AssetKey),
             last_materialization_record=check.opt_inst_param(
@@ -84,14 +89,22 @@
             asset_details=check.opt_inst_param(asset_details, "asset_details", AssetDetails),
             cached_status=check.opt_inst_param(
                 cached_status, "cached_status", AssetStatusCacheValue
             ),
             last_observation_record=check.opt_inst_param(
                 last_observation_record, "last_observation_record", EventLogRecord
             ),
+            last_planned_materialization_storage_id=check.opt_int_param(
+                last_planned_materialization_storage_id,
+                "last_planned_materialization_storage_id",
+            ),
+            last_planned_materialization_run_id=check.opt_str_param(
+                last_planned_materialization_run_id,
+                "last_planned_materialization_run_id",
+            ),
         )
 
     @property
     def last_materialization(self) -> Optional["EventLogEntry"]:
         if self.last_materialization_record is None:
             return None
         return self.last_materialization_record.event_log_entry
@@ -155,14 +168,19 @@
             run_id (str): The id of the run for which to fetch logs.
             cursor (Optional[Union[str, int]]): Cursor value to track paginated queries.  Legacy
                 support for integer offset cursors.
             of_type (Optional[DagsterEventType]): the dagster event type to filter the logs.
             limit (Optional[int]): Max number of records to return.
         """
         if isinstance(cursor, int):
+            deprecation_warning(
+                "Integer cursor values in `get_logs_for_run`",
+                "1.8.0",
+                "You can instead construct a storage_id-based string cursor e.g. `cursor = EventLogCursor.from_storage_id(storage_id).to_string()`",
+            )
             cursor = EventLogCursor.from_offset(cursor + 1).to_string()
         records = self.get_records_for_run(
             run_id, cursor, of_type, limit, ascending=ascending
         ).records
         return [record.event_log_entry for record in records]
 
     @abstractmethod
@@ -289,14 +307,18 @@
 
     @abstractmethod
     def get_asset_records(
         self, asset_keys: Optional[Sequence[AssetKey]] = None
     ) -> Sequence[AssetRecord]:
         pass
 
+    @property
+    def asset_records_have_last_planned_materialization_storage_id(self) -> bool:
+        return False
+
     @abstractmethod
     def has_asset_key(self, asset_key: AssetKey) -> bool:
         pass
 
     @abstractmethod
     def all_asset_keys(self) -> Sequence[AssetKey]:
         pass
```

### Comparing `dagster-1.7.4/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.7.5/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/event_log/migration.py` & `dagster-1.7.5/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.7.5/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/event_log/schema.py` & `dagster-1.7.5/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.7.5/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     ClaimedSlotInfo,
     ConcurrencyClaimStatus,
     ConcurrencyKeyInfo,
     ConcurrencySlotStatus,
     PendingStepInfo,
     get_max_concurrency_limit_value,
 )
+from dagster._utils.warnings import deprecation_warning
 
 from ..dagster_run import DagsterRunStatsSnapshot
 from .base import (
     AssetEntry,
     AssetRecord,
     AssetRecordsFilter,
     EventLogConnection,
@@ -1120,14 +1121,22 @@
         limit: Optional[int] = None,
     ) -> Mapping[int, EventLogEntry]:
         check.int_param(after_cursor, "after_cursor")
         check.invariant(
             after_cursor >= -1,
             f"Don't know what to do with negative cursor {after_cursor}",
         )
+
+        if isinstance(dagster_event_type, set) and len(dagster_event_type) > 1:
+            deprecation_warning(
+                "Support for multiple event types to get_logs_for_all_runs_by_log_id",
+                "1.8.0",
+                "You should break up your query into multiple calls, one for each event type.",
+            )
+
         dagster_event_types = (
             {dagster_event_type}
             if isinstance(dagster_event_type, DagsterEventType)
             else check.opt_set_param(
                 dagster_event_type, "dagster_event_type", of_type=DagsterEventType
             )
         )
@@ -1187,14 +1196,15 @@
                     last_run_id=row["last_run_id"],
                     asset_details=AssetDetails.from_db_string(row["asset_details"]),
                     cached_status=(
                         AssetStatusCacheValue.from_db_string(row["cached_status_data"])
                         if can_cache_asset_status_data
                         else None
                     ),
+                    last_planned_materialization_storage_id=None,
                 ),
             )
         else:
             check.failed("Row did not contain asset key.")
 
     def _get_latest_materialization_records(
         self, raw_asset_rows
@@ -1958,35 +1968,37 @@
         )
 
         materialization_events = db_select(
             [
                 latest_events_subquery.c.dagster_event_type,
                 latest_events_subquery.c.partition,
                 latest_events_subquery.c.run_id,
+                latest_events_subquery.c.id,
             ]
         ).where(
             latest_events_subquery.c.dagster_event_type
             == DagsterEventType.ASSET_MATERIALIZATION.value
         )
 
         with self.index_connection() as conn:
             materialization_planned_rows = db_fetch_mappings(conn, materialization_planned_events)
             materialization_rows = db_fetch_mappings(conn, materialization_events)
 
         materialization_planned_rows_by_partition = {
-            cast(str, row["partition"]): (cast(str, row["run_id"]), cast(int, row["id"]))
-            for row in materialization_planned_rows
+            row["partition"]: (row["run_id"], row["id"]) for row in materialization_planned_rows
         }
-        for row in materialization_rows:
-            if (
-                row["partition"] in materialization_planned_rows_by_partition
-                and materialization_planned_rows_by_partition[cast(str, row["partition"])][0]
-                == row["run_id"]
-            ):
-                materialization_planned_rows_by_partition.pop(cast(str, row["partition"]))
+        for mat_row in materialization_rows:
+            mat_partition = mat_row["partition"]
+            mat_event_id = mat_row["id"]
+            if mat_partition not in materialization_planned_rows_by_partition:
+                continue
+            _, planned_event_id = materialization_planned_rows_by_partition[mat_partition]
+            if planned_event_id < mat_event_id:
+                # this planned materialization event was followed by a materialization event
+                materialization_planned_rows_by_partition.pop(mat_partition)
 
         return materialization_planned_rows_by_partition
 
     def _check_partitions_table(self) -> None:
         # Guards against cases where the user is not running the latest migration for
         # partitions storage. Should be updated when the partitions storage schema changes.
         if not self.has_table("dynamic_partitions"):
```

### Comparing `dagster-1.7.4/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.7.5/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.7.5/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.7.5/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/file_manager.py` & `dagster-1.7.5/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/fs_io_manager.py` & `dagster-1.7.5/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/input_manager.py` & `dagster-1.7.5/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/io_manager.py` & `dagster-1.7.5/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/legacy_storage.py` & `dagster-1.7.5/dagster/_core/storage/legacy_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Union,
 )
 
 from dagster import (
     _check as check,
 )
 from dagster._config.config_schema import UserConfigSchema
-from dagster._core.definitions.asset_condition.asset_condition import (
+from dagster._core.definitions.declarative_scheduling.serialized_objects import (
     AssetConditionEvaluationWithRunIds,
 )
 from dagster._core.definitions.events import AssetKey
 from dagster._core.event_api import EventHandlerFn
 from dagster._core.storage.asset_check_execution_record import (
     AssetCheckExecutionRecord,
 )
```

### Comparing `dagster-1.7.4/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.7.5/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/mem_io_manager.py` & `dagster-1.7.5/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.7.5/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/migration/bigint_migration.py` & `dagster-1.7.5/dagster/_core/storage/migration/bigint_migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/migration/utils.py` & `dagster-1.7.5/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.7.5/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/output_manager.py` & `dagster-1.7.5/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/partition_status_cache.py` & `dagster-1.7.5/dagster/_core/storage/partition_status_cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     get_dimension_from_partition_tag,
 )
 from dagster._serdes import whitelist_for_serdes
 from dagster._serdes.errors import DeserializationError
 from dagster._serdes.serdes import deserialize_value
 
 if TYPE_CHECKING:
+    from dagster._core.storage.batch_asset_record_loader import BatchAssetRecordLoader
     from dagster._core.storage.event_log.base import AssetRecord
 
 
 CACHEABLE_PARTITION_TYPES = (
     TimeWindowPartitionsDefinition,
     MultiPartitionsDefinition,
     StaticPartitionsDefinition,
@@ -219,76 +220,103 @@
             pk
             for pk in partition_keys
             if partitions_def.has_partition_key(pk, current_time=current_time)
         }
     return validated_partitions
 
 
-def _get_last_planned_storage_id(instance: DagsterInstance, asset_key: AssetKey):
+def get_last_planned_storage_id(
+    instance: DagsterInstance, asset_key: AssetKey, asset_record: Optional["AssetRecord"]
+) -> int:
+    if instance.event_log_storage.asset_records_have_last_planned_materialization_storage_id:
+        return (
+            (asset_record.asset_entry.last_planned_materialization_storage_id or 0)
+            if asset_record
+            else 0
+        )
+
     info = instance.get_latest_planned_materialization_info(asset_key)
     if not info:
         return 0
 
     return info.storage_id
 
 
 def _build_status_cache(
     instance: DagsterInstance,
     asset_key: AssetKey,
     partitions_def: Optional[PartitionsDefinition],
     dynamic_partitions_store: DynamicPartitionsStore,
-    stored_cache_value: Optional[AssetStatusCacheValue] = None,
-    last_materialization_storage_id: Optional[int] = None,
+    stored_cache_value: Optional[AssetStatusCacheValue],
+    asset_record: Optional["AssetRecord"],
 ) -> Optional[AssetStatusCacheValue]:
     """This method refreshes the asset status cache for a given asset key. It recalculates
     the materialized partition subset for the asset key and updates the cache value.
     """
+    last_materialization_storage_id = (
+        asset_record.asset_entry.last_materialization_storage_id if asset_record else None
+    )
+
+    last_planned_materialization_storage_id = get_last_planned_storage_id(
+        instance, asset_key, asset_record
+    )
+
     latest_storage_id = max(
-        last_materialization_storage_id if last_materialization_storage_id else 0,
-        _get_last_planned_storage_id(instance, asset_key),
+        last_materialization_storage_id or 0,
+        last_planned_materialization_storage_id or 0,
     )
     if not latest_storage_id:
         return None
 
     if not partitions_def or not is_cacheable_partition_type(partitions_def):
         return AssetStatusCacheValue(latest_storage_id=latest_storage_id)
 
-    cached_failed_subset: PartitionsSubset = (
-        partitions_def.deserialize_subset(stored_cache_value.serialized_failed_partition_subset)
+    failed_partitions: Set[str] = (
+        set(
+            partitions_def.deserialize_subset(
+                stored_cache_value.serialized_failed_partition_subset
+            ).get_partition_keys()
+        )
         if stored_cache_value and stored_cache_value.serialized_failed_partition_subset
-        else partitions_def.empty_subset()
+        else set()
     )
     cached_in_progress_cursor = (
         (
             stored_cache_value.earliest_in_progress_materialization_event_id - 1
             if stored_cache_value.earliest_in_progress_materialization_event_id
             else stored_cache_value.latest_storage_id
         )
         if stored_cache_value
         else None
     )
 
     if stored_cache_value:
         # fetch the incremental new materialized partitions, and update the cached materialized
         # subset
+        new_partitions = set()
+        if (
+            last_materialization_storage_id
+            and last_materialization_storage_id > stored_cache_value.latest_storage_id
+        ):
+            new_partitions = instance.get_materialized_partitions(
+                asset_key, after_cursor=stored_cache_value.latest_storage_id
+            )
+
         materialized_subset: PartitionsSubset = (
             partitions_def.deserialize_subset(
                 stored_cache_value.serialized_materialized_partition_subset
             )
             if stored_cache_value.serialized_materialized_partition_subset
             else partitions_def.empty_subset()
         ).with_partition_keys(
-            get_validated_partition_keys(
-                dynamic_partitions_store,
-                partitions_def,
-                instance.get_materialized_partitions(
-                    asset_key, after_cursor=stored_cache_value.latest_storage_id
-                ),
-            )
+            get_validated_partition_keys(dynamic_partitions_store, partitions_def, new_partitions)
         )
+
+        failed_partitions.difference_update(new_partitions)
+
     else:
         materialized_subset = partitions_def.empty_subset().with_partition_keys(
             get_validated_partition_keys(
                 dynamic_partitions_store,
                 partitions_def,
                 instance.get_materialized_partitions(asset_key),
             )
@@ -299,15 +327,16 @@
         in_progress_subset,
         earliest_in_progress_materialization_event_id,
     ) = build_failed_and_in_progress_partition_subset(
         instance,
         asset_key,
         partitions_def,
         dynamic_partitions_store,
-        failed_partitions_subset=cached_failed_subset,
+        last_planned_materialization_storage_id=last_planned_materialization_storage_id,
+        failed_partitions=failed_partitions,
         after_storage_id=cached_in_progress_cursor,
     )
 
     return AssetStatusCacheValue(
         latest_storage_id=latest_storage_id,
         partitions_def_id=partitions_def.get_serializable_unique_identifier(
             dynamic_partitions_store=dynamic_partitions_store
@@ -320,32 +349,31 @@
 
 
 def build_failed_and_in_progress_partition_subset(
     instance: DagsterInstance,
     asset_key: AssetKey,
     partitions_def: PartitionsDefinition,
     dynamic_partitions_store: DynamicPartitionsStore,
-    failed_partitions_subset: Optional[PartitionsSubset] = None,
+    last_planned_materialization_storage_id: int,
+    failed_partitions: Optional[Set[str]] = None,
     after_storage_id: Optional[int] = None,
 ) -> Tuple[PartitionsSubset, PartitionsSubset, Optional[int]]:
-    failed_partitions: Set[str] = (
-        set(failed_partitions_subset.get_partition_keys()) if failed_partitions_subset else set()
-    )
+    failed_partitions = failed_partitions or set()
     in_progress_partitions: Set[str] = set()
-    if failed_partitions:
-        # These partitions were cached as having been failed.  If they have since been materialized,
-        # then we can remove them from the set of failed partitions.
-        materialized_partitions = instance.event_log_storage.get_materialized_partitions(
-            asset_key, after_cursor=after_storage_id
-        )
-        failed_partitions.difference_update(materialized_partitions)
 
-    incomplete_materializations = instance.event_log_storage.get_latest_asset_partition_materialization_attempts_without_materializations(
-        asset_key, after_storage_id=after_storage_id
-    )
+    incomplete_materializations = {}
+
+    # Fetch incomplete materializations if there have been any planned materializations since the
+    # cursor
+    if last_planned_materialization_storage_id and (
+        not after_storage_id or last_planned_materialization_storage_id > after_storage_id
+    ):
+        incomplete_materializations = instance.event_log_storage.get_latest_asset_partition_materialization_attempts_without_materializations(
+            asset_key, after_storage_id=after_storage_id
+        )
 
     cursor = None
     if incomplete_materializations:
         to_fetch = list(set([run_id for run_id, _event_id in incomplete_materializations.values()]))
         finished_runs = {}
         unfinished_runs = {}
 
@@ -393,26 +421,27 @@
         cursor,
     )
 
 
 def get_and_update_asset_status_cache_value(
     instance: DagsterInstance,
     asset_key: AssetKey,
-    partitions_def: Optional[PartitionsDefinition] = None,
+    partitions_def: Optional[PartitionsDefinition],
     dynamic_partitions_loader: Optional[DynamicPartitionsStore] = None,
-    asset_record: Optional["AssetRecord"] = None,
+    batch_asset_record_loader: Optional["BatchAssetRecordLoader"] = None,
 ) -> Optional[AssetStatusCacheValue]:
-    asset_record = asset_record or next(
-        iter(instance.get_asset_records(asset_keys=[asset_key])), None
-    )
+    if batch_asset_record_loader:
+        asset_record = batch_asset_record_loader.get_asset_record(asset_key)
+    else:
+        asset_record = next(iter(instance.get_asset_records(asset_keys=[asset_key])), None)
+
     if asset_record is None:
-        stored_cache_value, latest_materialization_storage_id = None, None
+        stored_cache_value = None
     else:
         stored_cache_value = asset_record.asset_entry.cached_status
-        latest_materialization_storage_id = asset_record.asset_entry.last_materialization_storage_id
 
     dynamic_partitions_store = dynamic_partitions_loader if dynamic_partitions_loader else instance
     use_cached_value = (
         stored_cache_value
         and partitions_def
         and stored_cache_value.partitions_def_id
         == partitions_def.get_serializable_unique_identifier(
@@ -421,13 +450,13 @@
     )
     updated_cache_value = _build_status_cache(
         instance=instance,
         asset_key=asset_key,
         partitions_def=partitions_def,
         dynamic_partitions_store=dynamic_partitions_store,
         stored_cache_value=stored_cache_value if use_cached_value else None,
-        last_materialization_storage_id=latest_materialization_storage_id,
+        asset_record=asset_record,
     )
     if updated_cache_value is not None and updated_cache_value != stored_cache_value:
         instance.update_asset_cached_status_data(asset_key, updated_cache_value)
 
     return updated_cache_value
```

### Comparing `dagster-1.7.4/dagster/_core/storage/root.py` & `dagster-1.7.5/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/runs/base.py` & `dagster-1.7.5/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/runs/in_memory.py` & `dagster-1.7.5/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/runs/migration.py` & `dagster-1.7.5/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/runs/schema.py` & `dagster-1.7.5/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.7.5/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.7.5/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.7.5/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/schedules/base.py` & `dagster-1.7.5/dagster/_core/storage/schedules/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 from typing import Mapping, Optional, Sequence, Set
 
 from dagster import AssetKey
-from dagster._core.definitions.asset_condition.asset_condition import (
+from dagster._core.definitions.declarative_scheduling.serialized_objects import (
     AssetConditionEvaluationWithRunIds,
 )
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.instance import MayHaveInstanceWeakref, T_DagsterInstance
 from dagster._core.scheduler.instigation import (
     AutoMaterializeAssetEvaluationRecord,
     InstigatorState,
```

### Comparing `dagster-1.7.4/dagster/_core/storage/schedules/migration.py` & `dagster-1.7.5/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/schedules/schema.py` & `dagster-1.7.5/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.7.5/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import pendulum
 import sqlalchemy as db
 import sqlalchemy.exc as db_exc
 from sqlalchemy.engine import Connection
 
 import dagster._check as check
-from dagster._core.definitions.asset_condition.asset_condition import (
+from dagster._core.definitions.declarative_scheduling.serialized_objects import (
     AssetConditionEvaluationWithRunIds,
 )
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.scheduler.instigation import (
     AutoMaterializeAssetEvaluationRecord,
```

### Comparing `dagster-1.7.4/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.7.5/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.7.5/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/sql.py` & `dagster-1.7.5/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/sqlalchemy_compat.py` & `dagster-1.7.5/dagster/_core/storage/sqlalchemy_compat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/sqlite.py` & `dagster-1.7.5/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/sqlite_storage.py` & `dagster-1.7.5/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/tags.py` & `dagster-1.7.5/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/temp_file_manager.py` & `dagster-1.7.5/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/storage/upath_io_manager.py` & `dagster-1.7.5/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/system_config/composite_descent.py` & `dagster-1.7.5/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/system_config/objects.py` & `dagster-1.7.5/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/telemetry.py` & `dagster-1.7.5/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/telemetry_upload.py` & `dagster-1.7.5/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/test_utils.py` & `dagster-1.7.5/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.7.5/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/types/config_schema.py` & `dagster-1.7.5/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/types/dagster_type.py` & `dagster-1.7.5/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/types/decorator.py` & `dagster-1.7.5/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/types/loadable_target_origin.py` & `dagster-1.7.5/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/types/primitive_mapping.py` & `dagster-1.7.5/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/types/python_dict.py` & `dagster-1.7.5/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/types/python_set.py` & `dagster-1.7.5/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/types/python_tuple.py` & `dagster-1.7.5/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/types/transform_typing.py` & `dagster-1.7.5/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/utility_ops.py` & `dagster-1.7.5/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/utils.py` & `dagster-1.7.5/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/workspace/autodiscovery.py` & `dagster-1.7.5/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/workspace/batch_asset_record_loader.py` & `dagster-1.7.5/dagster/_core/storage/batch_asset_record_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,53 @@
-from typing import Iterable, Mapping, Optional, Sequence, Set
+from typing import TYPE_CHECKING, Iterable, Mapping, Optional, Sequence, Set
 
-from dagster import (
-    DagsterInstance,
-    _check as check,
-)
+import dagster._check as check
 from dagster._core.definitions.events import AssetKey
 from dagster._core.events.log import EventLogEntry
-from dagster._core.storage.event_log.base import AssetRecord
+from dagster._core.instance import DagsterInstance
+
+if TYPE_CHECKING:
+    from dagster._core.storage.event_log.base import AssetRecord
 
 
 class BatchAssetRecordLoader:
     """A batch loader that fetches asset records.  This loader is expected to be
     instantiated with a set of asset keys.
     """
 
     def __init__(self, instance: DagsterInstance, asset_keys: Iterable[AssetKey]):
         self._instance = instance
         self._unfetched_asset_keys: Set[AssetKey] = set(asset_keys)
-        self._asset_records: Mapping[AssetKey, Optional[AssetRecord]] = {}
+        self._asset_records: Mapping[AssetKey, Optional["AssetRecord"]] = {}
 
     def add_asset_keys(self, asset_keys: Iterable[AssetKey]):
-        unfetched_asset_keys = set(asset_keys).difference(self._asset_records.keys())
+        unfetched_asset_keys = set(asset_keys).difference(self._asset_records)
         self._unfetched_asset_keys = self._unfetched_asset_keys.union(unfetched_asset_keys)
 
-    def get_asset_record(self, asset_key: AssetKey) -> Optional[AssetRecord]:
+    def get_asset_record(self, asset_key: AssetKey) -> Optional["AssetRecord"]:
         if asset_key not in self._asset_records and asset_key not in self._unfetched_asset_keys:
             check.failed(
                 f"Asset key {asset_key} not recognized for this loader. Expected one of:"
                 f" {self._unfetched_asset_keys.union(self._asset_records.keys())}"
             )
 
         if asset_key in self._unfetched_asset_keys:
-            self._fetch()
+            self.fetch()
 
         return self._asset_records.get(asset_key)
 
     def clear_cache(self):
         """For use in tests."""
         self._unfetched_asset_keys = self._unfetched_asset_keys.union(self._asset_records.keys())
         self._asset_records = {}
 
-    def get_asset_records(self, asset_keys: Sequence[AssetKey]) -> Sequence[AssetRecord]:
+    def has_cached_asset_record(self, asset_key: AssetKey):
+        return asset_key in self._asset_records
+
+    def get_asset_records(self, asset_keys: Sequence[AssetKey]) -> Sequence["AssetRecord"]:
         records = [self.get_asset_record(asset_key) for asset_key in asset_keys]
         return [record for record in records if record]
 
     def get_latest_materialization_for_asset_key(
         self, asset_key: AssetKey
     ) -> Optional[EventLogEntry]:
         asset_record = self.get_asset_record(asset_key)
@@ -61,15 +64,15 @@
 
         asset_record = self.get_asset_record(asset_key)
         if not asset_record:
             return None
 
         return asset_record.asset_entry.last_observation
 
-    def _fetch(self) -> None:
+    def fetch(self) -> None:
         if not self._unfetched_asset_keys:
             return
 
         new_records = {
             record.asset_entry.asset_key: record
             for record in self._instance.get_asset_records(list(self._unfetched_asset_keys))
         }
```

### Comparing `dagster-1.7.4/dagster/_core/workspace/config_schema.py` & `dagster-1.7.5/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/workspace/context.py` & `dagster-1.7.5/dagster/_core/workspace/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,17 +35,17 @@
     LocationStateChangeEventType,
     LocationStateSubscriber,
 )
 from dagster._core.remote_representation.origin import (
     GrpcServerCodeLocationOrigin,
     ManagedGrpcPythonEnvCodeLocationOrigin,
 )
+from dagster._core.storage.batch_asset_record_loader import BatchAssetRecordLoader
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 
-from .batch_asset_record_loader import BatchAssetRecordLoader
 from .load_target import WorkspaceLoadTarget
 from .permissions import (
     PermissionResult,
     get_location_scoped_user_permissions,
     get_user_permissions,
 )
 from .workspace import (
```

### Comparing `dagster-1.7.4/dagster/_core/workspace/load.py` & `dagster-1.7.5/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/workspace/load_target.py` & `dagster-1.7.5/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/workspace/permissions.py` & `dagster-1.7.5/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_core/workspace/workspace.py` & `dagster-1.7.5/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/__init__.py` & `dagster-1.7.5/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/asset_daemon.py` & `dagster-1.7.5/dagster/_daemon/asset_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.7.5/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.7.5/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/backfill.py` & `dagster-1.7.5/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/cli/__init__.py` & `dagster-1.7.5/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/controller.py` & `dagster-1.7.5/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/daemon.py` & `dagster-1.7.5/dagster/_daemon/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import random
 import sys
 import time
 import uuid
 from abc import ABC, abstractmethod
 from collections import deque
 from contextlib import AbstractContextManager, ExitStack
 from enum import Enum
@@ -225,34 +226,36 @@
         either NoneType or a SerializableErrorInfo.
 
         returns: generator (SerializableErrorInfo).
         """
 
 
 class IntervalDaemon(DagsterDaemon[TContext], ABC):
-    def __init__(self, interval_seconds):
+    def __init__(self, interval_seconds, jitter_seconds: float = 0):
         self.interval_seconds = check.numeric_param(interval_seconds, "interval_seconds")
+        self.jitter_seconds = jitter_seconds
         super().__init__()
 
     def core_loop(
         self,
         workspace_process_context: TContext,
         shutdown_event: Event,
     ) -> DaemonIterator:
         while True:
+            interval = self.interval_seconds + random.uniform(0, self.jitter_seconds)
             start_time = time.time()
             yield SpanMarker.START_SPAN
             try:
                 yield from self.run_iteration(workspace_process_context)
             except Exception:
                 error_info = serializable_error_info_from_exc_info(sys.exc_info())
                 self._logger.error("Caught error:\n%s", error_info)
                 yield error_info
             yield SpanMarker.END_SPAN
-            while time.time() - start_time < self.interval_seconds:
+            while time.time() - start_time < interval:
                 shutdown_event.wait(0.5)
                 yield None
             yield None
 
     @abstractmethod
     def run_iteration(self, workspace_process_context: TContext) -> DaemonIterator: ...
```

### Comparing `dagster-1.7.4/dagster/_daemon/monitoring/concurrency.py` & `dagster-1.7.5/dagster/_daemon/monitoring/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/monitoring/run_monitoring.py` & `dagster-1.7.5/dagster/_daemon/monitoring/run_monitoring.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.7.5/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/sensor.py` & `dagster-1.7.5/dagster/_daemon/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/types.py` & `dagster-1.7.5/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/utils.py` & `dagster-1.7.5/dagster/_daemon/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_daemon/workspace.py` & `dagster-1.7.5/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_generate/download.py` & `dagster-1.7.5/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_generate/generate.py` & `dagster-1.7.5/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.7.5/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.7.5/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/__generated__/api_pb2.pyi` & `dagster-1.7.5/dagster/_grpc/__generated__/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.7.5/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/__init__.py` & `dagster-1.7.5/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/client.py` & `dagster-1.7.5/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/compile.py` & `dagster-1.7.5/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/impl.py` & `dagster-1.7.5/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/protos/api.proto` & `dagster-1.7.5/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/proxy_server.py` & `dagster-1.7.5/dagster/_grpc/proxy_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/server.py` & `dagster-1.7.5/dagster/_grpc/server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/server_watcher.py` & `dagster-1.7.5/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/types.py` & `dagster-1.7.5/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_grpc/utils.py` & `dagster-1.7.5/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_loggers/__init__.py` & `dagster-1.7.5/dagster/_loggers/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,21 @@
 from typing import TYPE_CHECKING, Mapping, Optional, Sequence, Tuple
 
 import coloredlogs
 
 from dagster import _seven
 from dagster._config import Field
 from dagster._core.definitions.logger_definition import LoggerDefinition, logger
+from dagster._core.log_manager import (
+    LOG_RECORD_EVENT_ATTR,
+    LOG_RECORD_METADATA_ATTR,
+    DagsterLogRecordMetadata,
+)
 from dagster._core.utils import coerce_valid_log_level
+from dagster._serdes import pack_value
 from dagster._utils.log import create_console_logger
 
 if TYPE_CHECKING:
     from dagster._core.execution.context.logger import InitLoggerContext
     from dagster._core.instance import DagsterInstance
 
 
@@ -89,15 +95,30 @@
     klass = logging.getLoggerClass()
     logger_ = klass(name, level=level)
 
     handler = coloredlogs.StandardErrorHandler()
 
     class JsonFormatter(logging.Formatter):
         def format(self, record):
-            return _seven.json.dumps(record.__dict__)
+            dict_to_dump = {}
+            for k, v in record.__dict__.items():
+                if k == LOG_RECORD_EVENT_ATTR:
+                    # Redundant with the "dagster_event" field under "dagster_meta"
+                    continue
+                elif k == LOG_RECORD_METADATA_ATTR:
+                    # Events objects are not always JSON-serializable, so need to pack them first
+                    json_serializable_event = pack_value(v[LOG_RECORD_EVENT_ATTR])
+                    json_serializable_dagster_meta = DagsterLogRecordMetadata(
+                        **{**v, "dagster_event": json_serializable_event}
+                    )
+                    dict_to_dump[LOG_RECORD_METADATA_ATTR] = json_serializable_dagster_meta
+                else:
+                    dict_to_dump[k] = v
+
+            return _seven.json.dumps(dict_to_dump)
 
     handler.setFormatter(JsonFormatter())
     logger_.addHandler(handler)
 
     return logger_
```

### Comparing `dagster-1.7.4/dagster/_model/__init__.py` & `dagster-1.7.5/dagster/_model/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_model/pydantic_compat_layer.py` & `dagster-1.7.5/dagster/_model/pydantic_compat_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_module_alias_map.py` & `dagster-1.7.5/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_scheduler/scheduler.py` & `dagster-1.7.5/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_scheduler/stale.py` & `dagster-1.7.5/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_serdes/__init__.py` & `dagster-1.7.5/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_serdes/config_class.py` & `dagster-1.7.5/dagster/_serdes/config_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import importlib
 from abc import ABC, abstractmethod
 from typing import (
     TYPE_CHECKING,
     Any,
-    Dict,
     Mapping,
     NamedTuple,
     Optional,
     Type,
     TypeVar,
     Union,
     cast,
@@ -32,17 +31,20 @@
 # the ConfigurableClass interface on our storage classes. The concrete implementations of these
 # classes end up implementing the ConfigurableClass interface without inheriting from it, so we
 # don't actually bound this var.
 T_ConfigurableClass = TypeVar("T_ConfigurableClass")
 
 
 class ConfigurableClassDataSerializer(NamedTupleSerializer["ConfigurableClassData"]):
-    def after_pack(self, **packed: Any) -> Dict[str, Any]:
-        packed["module_name"] = convert_dagster_submodule_name(packed["module_name"], "public")
-        return packed
+    def pack_items(self, *args, **kwargs):
+        for k, v in super().pack_items(*args, **kwargs):
+            if k == "module_name":
+                yield k, convert_dagster_submodule_name(v, "public")
+            else:
+                yield k, v
 
 
 @whitelist_for_serdes(serializer=ConfigurableClassDataSerializer)
 class ConfigurableClassData(
     NamedTuple(
         "_ConfigurableClassData",
         [
```

### Comparing `dagster-1.7.4/dagster/_serdes/ipc.py` & `dagster-1.7.5/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_serdes/serdes.py` & `dagster-1.7.5/dagster/_serdes/serdes.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 
 import collections.abc
 import dataclasses
 from abc import ABC, abstractmethod
 from dataclasses import is_dataclass
 from enum import Enum
-from functools import partial
+from functools import cached_property, partial
 from inspect import Parameter, signature
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Callable,
     Dict,
@@ -38,22 +38,21 @@
     Tuple,
     Type,
     Union,
     cast,
     overload,
 )
 
-import pydantic
+from pydantic import BaseModel
 from typing_extensions import Final, Self, TypeAlias, TypeVar
 
 import dagster._check as check
 import dagster._seven as seven
-from dagster._model.pydantic_compat_layer import model_fields
+from dagster._model.pydantic_compat_layer import ModelFieldCompat, model_fields
 from dagster._utils import is_named_tuple_instance, is_named_tuple_subclass
-from dagster._utils.cached_method import cached_method
 from dagster._utils.warnings import disable_dagster_warnings
 
 from .errors import DeserializationError, SerdesUsageError, SerializationError
 
 if TYPE_CHECKING:
     # There is no actual class backing Dataclasses, _typeshed provides this
     # protocol.
@@ -79,15 +78,15 @@
     Mapping[str, "PackableValue"],
     str,
     int,
     float,
     bool,
     None,
     NamedTuple,
-    pydantic.BaseModel,
+    BaseModel,
     "DataclassInstance",
     Set["PackableValue"],
     FrozenSet["PackableValue"],
     Enum,
 ]
 
 UnpackedValue: TypeAlias = Union[
@@ -95,22 +94,28 @@
     Mapping[str, "UnpackedValue"],
     str,
     int,
     float,
     bool,
     None,
     NamedTuple,
-    pydantic.BaseModel,
+    BaseModel,
     "DataclassInstance",
     Set["PackableValue"],
     FrozenSet["PackableValue"],
     Enum,
     "UnknownSerdesValue",
 ]
 
+SerializableObject: TypeAlias = Union[
+    NamedTuple,
+    BaseModel,
+    "DataclassInstance",
+]
+
 _K = TypeVar("_K")
 _V = TypeVar("_V")
 
 
 class SerializableNonScalarKeyMapping(Mapping[_K, _V]):
     """Wrapper class for non-scalar key mappings, used to performantly type check when serializing
     without impacting the performance of serializing the more common scalar key dicts.
@@ -393,15 +398,15 @@
                 old_storage_names=old_storage_names,
                 storage_field_names=storage_field_names,
                 old_fields=old_fields,
                 skip_when_empty_fields=skip_when_empty_fields,
                 field_serializers=field_serializers,
             )
             return klass  # type: ignore
-        elif issubclass(klass, pydantic.BaseModel) and (
+        elif issubclass(klass, BaseModel) and (
             serializer is None or issubclass(serializer, PydanticModelSerializer)
         ):
             whitelist_map.register_object(
                 klass.__name__,
                 klass,
                 serializer or PydanticModelSerializer,
                 storage_name=storage_name,
@@ -421,15 +426,15 @@
 def is_whitelisted_for_serdes_object(
     val: Any, whitelist_map: WhitelistMap = _WHITELIST_MAP
 ) -> bool:
     """Check if object has been decorated with `@whitelist_for_serdes`."""
     if (
         (isinstance(val, tuple) and hasattr(val, "_fields"))  # NamedTuple
         or (is_dataclass(val) and not isinstance(val, type))  # dataclass instance
-        or isinstance(val, pydantic.BaseModel)
+        or isinstance(val, BaseModel)
     ):
         klass_name = val.__class__.__name__
         return whitelist_map.has_object_serializer(klass_name)
 
     return False
 
 
@@ -592,53 +597,53 @@
         self,
         exc: Exception,
         context: UnpackContext,
         storage_dict: Dict[str, Any],
     ) -> Any:
         raise exc
 
-    def pack(
+    def pack_items(
         self,
         value: T,
         whitelist_map: WhitelistMap,
+        object_handler: Callable[[SerializableObject, WhitelistMap, str], JsonSerializableValue],
         descent_path: str,
-    ) -> Dict[str, JsonSerializableValue]:
-        packed: Dict[str, JsonSerializableValue] = {}
-        packed["__class__"] = self.get_storage_name()
+    ) -> Iterator[Tuple[str, JsonSerializableValue]]:
+        yield "__class__", self.get_storage_name()
         for key, inner_value in self.object_as_mapping(self.before_pack(value)).items():
             if key in self.skip_when_empty_fields and inner_value in EMPTY_VALUES_TO_SKIP:
                 continue
             storage_key = self.storage_field_names.get(key, key)
             custom = self.field_serializers.get(key)
             if custom:
-                packed[storage_key] = custom.pack(
-                    inner_value,
-                    whitelist_map=whitelist_map,
-                    descent_path=f"{descent_path}.{key}",
+                yield (
+                    storage_key,
+                    custom.pack(
+                        inner_value,
+                        whitelist_map=whitelist_map,
+                        descent_path=f"{descent_path}.{key}",
+                    ),
                 )
             else:
-                packed[storage_key] = _pack_value(
-                    inner_value,
-                    whitelist_map=whitelist_map,
-                    descent_path=f"{descent_path}.{key}",
+                yield (
+                    storage_key,
+                    _transform_for_serialization(
+                        inner_value,
+                        whitelist_map=whitelist_map,
+                        object_handler=object_handler,
+                        descent_path=f"{descent_path}.{key}",
+                    ),
                 )
         for key, default in self.old_fields.items():
-            packed[key] = default
-        packed = self.after_pack(**packed)
-        return packed
+            yield key, default
 
     # Hook: Modify the contents of the object before packing
     def before_pack(self, value: T) -> T:
         return value
 
-    # Hook: Modify the contents of the packed, json-serializable dict before it is converted to a
-    # string.
-    def after_pack(self, **packed_dict: JsonSerializableValue) -> Dict[str, JsonSerializableValue]:
-        return packed_dict
-
     @property
     @abstractmethod
     def constructor_param_names(self) -> Sequence[str]: ...
 
     def get_storage_name(self) -> str:
         return self.storage_name or self.klass.__name__
 
@@ -646,56 +651,59 @@
 T_NamedTuple = TypeVar("T_NamedTuple", bound=NamedTuple, default=NamedTuple)
 
 
 class NamedTupleSerializer(ObjectSerializer[T_NamedTuple]):
     def object_as_mapping(self, value: T_NamedTuple) -> Mapping[str, Any]:
         return value._asdict()
 
-    @property
-    @cached_method
+    @cached_property
     def constructor_param_names(self) -> Sequence[str]:
         return list(signature(self.klass.__new__).parameters.keys())
 
 
 T_Dataclass = TypeVar("T_Dataclass", bound="DataclassInstance", default="DataclassInstance")
 
 
 class DataclassSerializer(ObjectSerializer[T_Dataclass]):
     def object_as_mapping(self, value: T_Dataclass) -> Mapping[str, Any]:
         return value.__dict__
 
-    @property
+    @cached_property
     def constructor_param_names(self) -> Sequence[str]:
         return list(f.name for f in dataclasses.fields(self.klass))
 
 
-T_PydanticModel = TypeVar("T_PydanticModel", bound=pydantic.BaseModel, default=pydantic.BaseModel)
+T_PydanticModel = TypeVar("T_PydanticModel", bound=BaseModel, default=BaseModel)
 
 
 class PydanticModelSerializer(ObjectSerializer[T_PydanticModel]):
     def object_as_mapping(self, value: T_PydanticModel) -> Mapping[str, Any]:
         value_dict = value.__dict__
 
         result = {}
-        for key, field in model_fields(self.klass).items():
+        for key, field in self._model_fields.items():
             if field.alias is None and (
                 field.serialization_alias is not None or field.validation_alias is not None
             ):
                 raise SerializationError(
                     "Can't serialize pydantic models with serialization or validation aliases. Use "
                     "the storage_field_names argument to whitelist_for_serdes instead."
                 )
             result_key = field.alias if field.alias else key
             result[result_key] = value_dict[key]
 
         return result
 
-    @property
+    @cached_property
     def constructor_param_names(self) -> Sequence[str]:
-        return [field.alias or key for key, field in model_fields(self.klass).items()]
+        return [field.alias or key for key, field in self._model_fields.items()]
+
+    @cached_property
+    def _model_fields(self) -> Mapping[str, ModelFieldCompat]:
+        return model_fields(self.klass)
 
 
 class FieldSerializer(Serializer):
     _instance = None
 
     # Because `FieldSerializer` is not currently parameterizable (all variation is contained in the
     # logic of pack/unpack), we store references to a singleton instance in the whitelist map to
@@ -749,16 +757,21 @@
     whitelist_map: WhitelistMap = _WHITELIST_MAP,
     **json_kwargs: Any,
 ) -> str:
     """Serialize an object to a JSON string.
 
     Objects are first converted to a JSON-serializable form with `pack_value`.
     """
-    packed_value = pack_value(val, whitelist_map=whitelist_map)
-    return seven.json.dumps(packed_value, **json_kwargs)
+    serializable_value = _transform_for_serialization(
+        val,
+        whitelist_map=whitelist_map,
+        object_handler=_wrap_object,
+        descent_path=_root(val),
+    )
+    return seven.json.dumps(serializable_value, **json_kwargs)
 
 
 @overload
 def pack_value(
     val: T_Scalar,
     whitelist_map: WhitelistMap = ...,
     descent_path: Optional[str] = ...,
@@ -769,15 +782,15 @@
 def pack_value(
     val: Union[
         Mapping[str, PackableValue],
         Set[PackableValue],
         FrozenSet[PackableValue],
         NamedTuple,
         "DataclassInstance",
-        pydantic.BaseModel,
+        BaseModel,
         Enum,
     ],
     whitelist_map: WhitelistMap = ...,
     descent_path: Optional[str] = ...,
 ) -> Mapping[str, JsonSerializableValue]: ...
 
 
@@ -799,42 +812,68 @@
     The following types are transformed in to dicts with special marker keys:
         * whitelisted objects (NamedTuple, dataclass, or pydantic models)
         * whitelisted enums
         * set
         * frozenset
     """
     descent_path = _root(val) if descent_path is None else descent_path
-    return _pack_value(val, whitelist_map=whitelist_map, descent_path=descent_path)
+    return _transform_for_serialization(
+        val,
+        whitelist_map=whitelist_map,
+        descent_path=descent_path,
+        object_handler=_pack_object,
+    )
 
 
-def _pack_value(
+def _transform_for_serialization(
     val: PackableValue,
     whitelist_map: WhitelistMap,
+    object_handler: Callable[[SerializableObject, WhitelistMap, str], JsonSerializableValue],
     descent_path: str,
 ) -> JsonSerializableValue:
     # this is a hot code path so we handle the common base cases without isinstance
     tval = type(val)
     if tval in (int, float, str, bool) or val is None:
         return cast(JsonSerializableValue, val)
     if tval is list:
         return [
-            _pack_value(item, whitelist_map, f"{descent_path}[{idx}]")
+            _transform_for_serialization(
+                item,
+                whitelist_map,
+                object_handler,
+                f"{descent_path}[{idx}]",
+            )
             for idx, item in enumerate(cast(list, val))
         ]
     if tval is dict:
         return {
-            key: _pack_value(value, whitelist_map, f"{descent_path}.{key}")
+            key: _transform_for_serialization(
+                value,
+                whitelist_map,
+                object_handler,
+                f"{descent_path}.{key}",
+            )
             for key, value in cast(dict, val).items()
         }
     if tval is SerializableNonScalarKeyMapping:
         return {
             "__mapping_items__": [
                 [
-                    _pack_value(k, whitelist_map, f"{descent_path}.{k}"),
-                    _pack_value(v, whitelist_map, f"{descent_path}.{k}"),
+                    _transform_for_serialization(
+                        k,
+                        whitelist_map,
+                        object_handler,
+                        f"{descent_path}.{k}",
+                    ),
+                    _transform_for_serialization(
+                        v,
+                        whitelist_map,
+                        object_handler,
+                        f"{descent_path}.{k}",
+                    ),
                 ]
                 for k, v in cast(dict, val).items()
             ]
         }
 
     if isinstance(val, Enum):
         klass_name = val.__class__.__name__
@@ -843,60 +882,137 @@
                 "Can only serialize whitelisted Enums, received"
                 f" {klass_name}.\nDescent path: {descent_path}",
             )
         enum_serializer = whitelist_map.get_enum_entry(klass_name)
         return {"__enum__": enum_serializer.pack(val, whitelist_map, descent_path)}
     if (
         (isinstance(val, tuple) and hasattr(val, "_fields"))
+        or isinstance(val, BaseModel)
         or (is_dataclass(val) and not isinstance(val, type))
-        or isinstance(val, pydantic.BaseModel)
     ):
         klass_name = val.__class__.__name__
         if not whitelist_map.has_object_serializer(klass_name):
             raise SerializationError(
                 "Can only serialize whitelisted namedtuples, received"
                 f" {val}.\nDescent path: {descent_path}",
             )
-        serializer = whitelist_map.get_object_serializer(klass_name)
-        return serializer.pack(val, whitelist_map, descent_path)
+        return object_handler(
+            cast(SerializableObject, val),
+            whitelist_map,
+            descent_path,
+        )
     if isinstance(val, set):
         set_path = descent_path + "{}"
         return {
             "__set__": [
-                _pack_value(item, whitelist_map, set_path) for item in sorted(list(val), key=str)
+                _transform_for_serialization(
+                    item,
+                    whitelist_map,
+                    object_handler,
+                    set_path,
+                )
+                for item in sorted(list(val), key=str)
             ]
         }
     if isinstance(val, frozenset):
         frz_set_path = descent_path + "{}"
         return {
             "__frozenset__": [
-                _pack_value(item, whitelist_map, frz_set_path)
+                _transform_for_serialization(
+                    item,
+                    whitelist_map,
+                    object_handler,
+                    frz_set_path,
+                )
                 for item in sorted(list(val), key=str)
             ]
         }
 
     # custom string subclasses
     if isinstance(val, str):
         return val
 
     # handle more expensive and uncommon abc instance checks last
     if isinstance(val, collections.abc.Mapping):
         return {
-            key: _pack_value(value, whitelist_map, f"{descent_path}.{key}")
+            key: _transform_for_serialization(
+                value,
+                whitelist_map,
+                object_handler,
+                f"{descent_path}.{key}",
+            )
             for key, value in val.items()
         }
     if isinstance(val, collections.abc.Sequence):
         return [
-            _pack_value(item, whitelist_map, f"{descent_path}[{idx}]")
+            _transform_for_serialization(
+                item,
+                whitelist_map,
+                object_handler,
+                f"{descent_path}[{idx}]",
+            )
             for idx, item in enumerate(val)
         ]
 
     raise SerializationError(f"Unhandled value type {tval}")
 
 
+def _pack_object(
+    obj: SerializableObject, whitelist_map: WhitelistMap, descent_path: str
+) -> Mapping[str, JsonSerializableValue]:
+    # the object_handler for _transform_for_serialization to produce dicts for objects
+
+    klass_name = obj.__class__.__name__
+    serializer = whitelist_map.get_object_serializer(klass_name)
+    return dict(serializer.pack_items(obj, whitelist_map, _pack_object, descent_path))
+
+
+class _LazySerializationWrapper(dict):
+    """An object used to allow us to drive serialization iteratively
+    over the tree of objects via json.dumps, instead of having to create
+    an entire tree of primitive objects to pass to json.dumps.
+    """
+
+    __slots__ = [
+        "_obj",
+        "_whitelist_map",
+        "_descent_path",
+    ]
+
+    def __init__(
+        self,
+        obj: SerializableObject,
+        whitelist_map: WhitelistMap,
+        descent_path: str,
+    ):
+        self._obj = obj
+        self._whitelist_map = whitelist_map
+        self._descent_path = descent_path
+
+        # populate backing native dict to work around c fast path check
+        # https://github.com/python/cpython/blob/0fb18b02c8ad56299d6a2910be0bab8ad601ef24/Modules/_json.c#L1542
+        super().__init__({"__serdes": "wrapper"})
+
+    def items(self) -> Iterator[Tuple[str, JsonSerializableValue]]:
+        klass_name = self._obj.__class__.__name__
+        serializer = self._whitelist_map.get_object_serializer(klass_name)
+        yield from serializer.pack_items(
+            self._obj, self._whitelist_map, _wrap_object, self._descent_path
+        )
+
+
+def _wrap_object(
+    obj: SerializableObject,
+    whitelist_map: WhitelistMap,
+    descent_path: str,
+) -> "_LazySerializationWrapper":
+    # the object_handler for _transform_for_serialization to use in conjunction with json.dumps for iterative serialization
+    return _LazySerializationWrapper(obj, whitelist_map, descent_path)
+
+
 ###################################################################################################
 # Deserialize / Unpack
 ###################################################################################################
 
 T_PackableValue = TypeVar("T_PackableValue", bound=PackableValue, default=PackableValue)
 U_PackableValue = TypeVar("U_PackableValue", bound=PackableValue, default=PackableValue)
```

### Comparing `dagster-1.7.4/dagster/_serdes/utils.py` & `dagster-1.7.5/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_seven/__init__.py` & `dagster-1.7.5/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_seven/abc.py` & `dagster-1.7.5/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_seven/compat/pendulum.py` & `dagster-1.7.5/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/__init__.py` & `dagster-1.7.5/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/alert.py` & `dagster-1.7.5/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/backoff.py` & `dagster-1.7.5/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/cached_method.py` & `dagster-1.7.5/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/caching_instance_queryer.py` & `dagster-1.7.5/dagster/_utils/caching_instance_queryer.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 from dagster._core.errors import (
     DagsterDefinitionChangedDeserializationError,
     DagsterInvalidDefinitionError,
 )
 from dagster._core.event_api import AssetRecordsFilter, EventRecordsFilter
 from dagster._core.events import DagsterEventType
 from dagster._core.instance import DagsterInstance, DynamicPartitionsStore
+from dagster._core.storage.batch_asset_record_loader import BatchAssetRecordLoader
 from dagster._core.storage.dagster_run import (
+    IN_PROGRESS_RUN_STATUSES,
     DagsterRun,
     RunRecord,
 )
 from dagster._core.storage.tags import PARTITION_NAME_TAG
 from dagster._utils.cached_method import cached_method
 
 if TYPE_CHECKING:
@@ -72,15 +74,16 @@
         evaluation_time: Optional[datetime] = None,
         logger: Optional[logging.Logger] = None,
     ):
         self._instance = instance
         self._asset_graph = asset_graph
         self._logger = logger or logging.getLogger("dagster")
 
-        self._asset_record_cache: Dict[AssetKey, Optional[AssetRecord]] = {}
+        self._batch_asset_record_loader = BatchAssetRecordLoader(self._instance, set())
+
         self._asset_partitions_cache: Dict[Optional[int], Dict[AssetKey, Set[str]]] = defaultdict(
             dict
         )
         self._asset_partition_versions_updated_after_cursor_cache: Dict[
             AssetKeyPartitionKey, int
         ] = {}
 
@@ -106,43 +109,35 @@
 
     ####################
     # QUERY BATCHING
     ####################
 
     def prefetch_asset_records(self, asset_keys: Iterable[AssetKey]):
         """For performance, batches together queries for selected assets."""
-        keys_to_fetch = set(asset_keys) - set(self._asset_record_cache.keys())
-        if len(keys_to_fetch) == 0:
-            return
-        # get all asset records for selected assets that aren't already cached
-        asset_records = self.instance.get_asset_records(list(keys_to_fetch))
-        for asset_record in asset_records:
-            self._asset_record_cache[asset_record.asset_entry.asset_key] = asset_record
-        for key in asset_keys:
-            if key not in self._asset_record_cache:
-                self._asset_record_cache[key] = None
+        self._batch_asset_record_loader.add_asset_keys(asset_keys)
+        self._batch_asset_record_loader.fetch()
 
     ####################
     # ASSET STATUS CACHE
     ####################
 
     @cached_method
     def _get_updated_cache_value(self, *, asset_key: AssetKey) -> Optional["AssetStatusCacheValue"]:
         from dagster._core.storage.partition_status_cache import (
             get_and_update_asset_status_cache_value,
         )
 
         partitions_def = check.not_none(self.asset_graph.get(asset_key).partitions_def)
-        asset_record = self.get_asset_record(asset_key)
+        self._batch_asset_record_loader.add_asset_keys([asset_key])
         return get_and_update_asset_status_cache_value(
             instance=self.instance,
             asset_key=asset_key,
             partitions_def=partitions_def,
             dynamic_partitions_loader=self,
-            asset_record=asset_record,
+            batch_asset_record_loader=self._batch_asset_record_loader,
         )
 
     @cached_method
     def get_failed_or_in_progress_subset(self, *, asset_key: AssetKey) -> PartitionsSubset:
         """Returns a PartitionsSubset representing the set of partitions that are either in progress
         or whose last materialization attempt failed.
         """
@@ -152,42 +147,66 @@
             return partitions_def.empty_subset()
 
         return cache_value.deserialize_failed_partition_subsets(
             partitions_def
         ) | cache_value.deserialize_in_progress_partition_subsets(partitions_def)
 
     @cached_method
-    def get_materialized_asset_subset(self, *, asset_key: AssetKey) -> AssetSubset:
+    def get_materialized_asset_subset(self, *, asset_key: AssetKey) -> ValidAssetSubset:
         """Returns an AssetSubset representing the subset of the asset that has been materialized."""
         partitions_def = self.asset_graph.get(asset_key).partitions_def
         if partitions_def:
             cache_value = self._get_updated_cache_value(asset_key=asset_key)
             if cache_value is None:
                 value = partitions_def.empty_subset()
             else:
                 value = cache_value.deserialize_materialized_partition_subsets(partitions_def)
         else:
             value = self.asset_partition_has_materialization_or_observation(
                 AssetKeyPartitionKey(asset_key)
             )
-        return AssetSubset(asset_key=asset_key, value=value)
+        return ValidAssetSubset(asset_key=asset_key, value=value)
+
+    @cached_method
+    def get_in_progress_asset_subset(self, *, asset_key: AssetKey) -> ValidAssetSubset:
+        """Returns an AssetSubset representing the subset of the asset that is currently in progress."""
+        partitions_def = self.asset_graph.get(asset_key).partitions_def
+        if partitions_def:
+            cache_value = self._get_updated_cache_value(asset_key=asset_key)
+            if cache_value is None:
+                value = partitions_def.empty_subset()
+            else:
+                value = cache_value.deserialize_in_progress_partition_subsets(partitions_def)
+        else:
+            # NOTE: this computation is not correct in all cases for unpartitioned assets. it is
+            # possible (though rare) for run A to be launched targeting an asset, then later run B
+            # be launched, and then run B completes before run A. In these cases, the computation
+            # below will consider the asset to not be in progress, as the latest planned event
+            # will be associated with a completed run.
+            planned_materialization_info = (
+                self.instance.event_log_storage.get_latest_planned_materialization_info(asset_key)
+            )
+            if not planned_materialization_info:
+                value = False
+            else:
+                dagster_run = self.instance.get_run_by_id(planned_materialization_info.run_id)
+                value = dagster_run is not None and dagster_run.status in IN_PROGRESS_RUN_STATUSES
+
+        return ValidAssetSubset(asset_key=asset_key, value=value)
 
     ####################
     # ASSET RECORDS / STORAGE IDS
     ####################
 
     def has_cached_asset_record(self, asset_key: AssetKey) -> bool:
-        return asset_key in self._asset_record_cache
+        return self._batch_asset_record_loader.has_cached_asset_record(asset_key)
 
     def get_asset_record(self, asset_key: AssetKey) -> Optional["AssetRecord"]:
-        if asset_key not in self._asset_record_cache:
-            self._asset_record_cache[asset_key] = next(
-                iter(self.instance.get_asset_records([asset_key])), None
-            )
-        return self._asset_record_cache[asset_key]
+        self._batch_asset_record_loader.add_asset_keys({asset_key})
+        return self._batch_asset_record_loader.get_asset_record(asset_key)
 
     def _event_type_for_key(self, asset_key: AssetKey) -> DagsterEventType:
         if self.asset_graph.get(asset_key).is_observable:
             return DagsterEventType.ASSET_OBSERVATION
         else:
             return DagsterEventType.ASSET_MATERIALIZATION
```

### Comparing `dagster-1.7.4/dagster/_utils/concurrency.py` & `dagster-1.7.5/dagster/_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/container.py` & `dagster-1.7.5/dagster/_utils/container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/dagster_type.py` & `dagster-1.7.5/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/env.py` & `dagster-1.7.5/dagster/_utils/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/error.py` & `dagster-1.7.5/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/external.py` & `dagster-1.7.5/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/forked_pdb.py` & `dagster-1.7.5/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/hosted_user_process.py` & `dagster-1.7.5/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/indenting_printer.py` & `dagster-1.7.5/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/internal_init.py` & `dagster-1.7.5/dagster/_utils/internal_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/interrupts.py` & `dagster-1.7.5/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/log.py` & `dagster-1.7.5/dagster/_utils/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/merger.py` & `dagster-1.7.5/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/net.py` & `dagster-1.7.5/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/schedules.py` & `dagster-1.7.5/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/tags.py` & `dagster-1.7.5/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/temp_file.py` & `dagster-1.7.5/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/test/__init__.py` & `dagster-1.7.5/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/test/data_versions.py` & `dagster-1.7.5/dagster/_utils/test/data_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/test/mysql_instance.py` & `dagster-1.7.5/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/test/postgres_instance.py` & `dagster-1.7.5/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/test/schedule_storage.py` & `dagster-1.7.5/dagster/_utils/test/schedule_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sys
 import time
 
 import pendulum
 import pytest
 
 from dagster import StaticPartitionsDefinition
-from dagster._core.definitions.asset_condition.asset_condition import (
+from dagster._core.definitions.asset_subset import AssetSubset
+from dagster._core.definitions.declarative_scheduling.serialized_objects import (
     AssetConditionEvaluation,
     AssetConditionSnapshot,
     AssetSubsetWithMetadata,
 )
-from dagster._core.definitions.asset_subset import AssetSubset
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.metadata import MetadataValue
 from dagster._core.remote_representation import (
     ManagedGrpcPythonEnvCodeLocationOrigin,
     RemoteRepositoryOrigin,
 )
 from dagster._core.scheduler.instigation import (
```

### Comparing `dagster-1.7.4/dagster/_utils/timing.py` & `dagster-1.7.5/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/typed_dict.py` & `dagster-1.7.5/dagster/_utils/typed_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/typing_api.py` & `dagster-1.7.5/dagster/_utils/typing_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -124,7 +124,25 @@
         or is_closed_python_tuple_type(ttype)
         or is_closed_python_list_type(ttype)
         or ttype is typing.Tuple
         or ttype is typing.Set
         or ttype is typing.Dict
         or ttype is typing.List
     )
+
+
+def flatten_unions(ttype: typing.Type) -> typing.AbstractSet[typing.Type]:
+    """Accepts a type that may be a Union of other types, and returns those other types.
+    In addition to explicit Union annotations, works for Optional, which is represented as
+    Union[T, None] under the covers.
+
+    E.g. Optional[Union[str, Union[int, float]]] would result in (str, int, float, type(None))
+    """
+    return set(_flatten_unions_inner(ttype))
+
+
+def _flatten_unions_inner(ttype: typing.Type) -> typing.Iterable[typing.Type]:
+    if get_origin(ttype) is typing.Union:
+        for arg in get_args(ttype):
+            yield from flatten_unions(arg)
+    else:
+        yield ttype
```

### Comparing `dagster-1.7.4/dagster/_utils/warnings.py` & `dagster-1.7.5/dagster/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster/_utils/yaml_utils.py` & `dagster-1.7.5/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.4/dagster.egg-info/PKG-INFO` & `dagster-1.7.5/dagster.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.4
+Version: 1.7.5
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
@@ -102,29 +102,14 @@
 
 <p align="center">
   <img width="100%" alt="An example asset graph as rendered in the Dagster UI" src="https://raw.githubusercontent.com/dagster-io/dagster/master/.github/example-lineage.png">
 </p>
 
 Dagster is built to be used at every stage of the data development lifecycle - local development, unit tests, integration tests, staging environments, all the way up to production.
 
-## Special Event: Introducing Dagster+
-
-<p align="center">
-  <img width="100%" alt="Join us on April 17 (12PM ET) for a special event introducing Dagster+" src="https://i.imgur.com/1r7hOep.png">
-</p>
-
-Join us on April 17 (12PM ET) for a special event introducing Dagster+. [Register for our Dagster+ launch event here](https://dagster.io/events/dagster-plus-launch-event)
-
-In addition to the core open-source project, we are excited to announce Dagster+, the next generation of Dagster's cloud offering.
-
-- Find out how to weave data reliability and quality checks into the execution of your data pipelines.
-- See how diff-based branch deployments will accelerate your development cycle and cut extraneous compute costs.
-- Get a deep understanding of what is driving the cost of your data pipelines, then optimize to get the best cost/performance outcomes.
-- Enjoy the benefits of built-in data cataloging, and asset-level rich metadata.
-
 ## Quick Start:
 
 If you're new to Dagster, we recommend reading about its [core concepts](https://docs.dagster.io/concepts) or learning with the hands-on [tutorial](https://docs.dagster.io/tutorial).
 
 Dagster is available on PyPI and officially supports Python 3.8 through Python 3.12.
 
 ```bash
```

### Comparing `dagster-1.7.4/dagster.egg-info/SOURCES.txt` & `dagster-1.7.5/dagster.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -171,48 +171,63 @@
 dagster/_core/definitions/resource_requirement.py
 dagster/_core/definitions/result.py
 dagster/_core/definitions/run_config.py
 dagster/_core/definitions/run_config_schema.py
 dagster/_core/definitions/run_request.py
 dagster/_core/definitions/run_status_sensor_definition.py
 dagster/_core/definitions/schedule_definition.py
-dagster/_core/definitions/schema_change_checks.py
 dagster/_core/definitions/scoped_resources_builder.py
 dagster/_core/definitions/selector.py
 dagster/_core/definitions/sensor_definition.py
 dagster/_core/definitions/source_asset.py
 dagster/_core/definitions/step_launcher.py
 dagster/_core/definitions/target.py
 dagster/_core/definitions/time_window_partition_mapping.py
 dagster/_core/definitions/time_window_partitions.py
 dagster/_core/definitions/unresolved_asset_job_definition.py
 dagster/_core/definitions/utils.py
 dagster/_core/definitions/version_strategy.py
-dagster/_core/definitions/asset_condition/__init__.py
-dagster/_core/definitions/asset_condition/asset_condition.py
-dagster/_core/definitions/asset_condition/asset_condition_evaluation_context.py
+dagster/_core/definitions/asset_check_factories/__init__.py
+dagster/_core/definitions/asset_check_factories/schema_change_checks.py
+dagster/_core/definitions/asset_check_factories/utils.py
+dagster/_core/definitions/asset_check_factories/freshness_checks/__init__.py
+dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py
+dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py
+dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py
+dagster/_core/definitions/declarative_scheduling/README.md
+dagster/_core/definitions/declarative_scheduling/__init__.py
+dagster/_core/definitions/declarative_scheduling/scheduling_condition.py
+dagster/_core/definitions/declarative_scheduling/scheduling_context.py
+dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py
+dagster/_core/definitions/declarative_scheduling/serialized_objects.py
+dagster/_core/definitions/declarative_scheduling/legacy/__init__.py
+dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py
+dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py
+dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py
+dagster/_core/definitions/declarative_scheduling/operands/__init__.py
+dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py
+dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py
+dagster/_core/definitions/declarative_scheduling/operators/__init__.py
+dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py
+dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py
 dagster/_core/definitions/decorators/__init__.py
 dagster/_core/definitions/decorators/asset_check_decorator.py
 dagster/_core/definitions/decorators/asset_decorator.py
 dagster/_core/definitions/decorators/config_mapping_decorator.py
 dagster/_core/definitions/decorators/graph_decorator.py
 dagster/_core/definitions/decorators/hook_decorator.py
 dagster/_core/definitions/decorators/job_decorator.py
 dagster/_core/definitions/decorators/op_decorator.py
 dagster/_core/definitions/decorators/repository_decorator.py
 dagster/_core/definitions/decorators/schedule_decorator.py
 dagster/_core/definitions/decorators/sensor_decorator.py
 dagster/_core/definitions/decorators/source_asset_decorator.py
-dagster/_core/definitions/freshness_checks/__init__.py
-dagster/_core/definitions/freshness_checks/last_update.py
-dagster/_core/definitions/freshness_checks/sensor.py
-dagster/_core/definitions/freshness_checks/shared_builder.py
-dagster/_core/definitions/freshness_checks/time_partition.py
-dagster/_core/definitions/freshness_checks/utils.py
 dagster/_core/definitions/metadata/__init__.py
+dagster/_core/definitions/metadata/metadata_set.py
+dagster/_core/definitions/metadata/metadata_value.py
 dagster/_core/definitions/metadata/table.py
 dagster/_core/definitions/repository_definition/__init__.py
 dagster/_core/definitions/repository_definition/caching_index.py
 dagster/_core/definitions/repository_definition/repository_data.py
 dagster/_core/definitions/repository_definition/repository_data_builder.py
 dagster/_core/definitions/repository_definition/repository_definition.py
 dagster/_core/definitions/repository_definition/valid_definitions.py
@@ -330,14 +345,15 @@
 dagster/_core/snap/node.py
 dagster/_core/snap/snap_to_yaml.py
 dagster/_core/storage/DEVELOPING.md
 dagster/_core/storage/__init__.py
 dagster/_core/storage/asset_check_execution_record.py
 dagster/_core/storage/asset_value_loader.py
 dagster/_core/storage/base_storage.py
+dagster/_core/storage/batch_asset_record_loader.py
 dagster/_core/storage/captured_log_manager.py
 dagster/_core/storage/cloud_storage_compute_log_manager.py
 dagster/_core/storage/compute_log_manager.py
 dagster/_core/storage/config.py
 dagster/_core/storage/daemon_cursor.py
 dagster/_core/storage/dagster_run.py
 dagster/_core/storage/db_io_manager.py
@@ -489,15 +505,14 @@
 dagster/_core/types/primitive_mapping.py
 dagster/_core/types/python_dict.py
 dagster/_core/types/python_set.py
 dagster/_core/types/python_tuple.py
 dagster/_core/types/transform_typing.py
 dagster/_core/workspace/__init__.py
 dagster/_core/workspace/autodiscovery.py
-dagster/_core/workspace/batch_asset_record_loader.py
 dagster/_core/workspace/config_schema.py
 dagster/_core/workspace/context.py
 dagster/_core/workspace/load.py
 dagster/_core/workspace/load_target.py
 dagster/_core/workspace/permissions.py
 dagster/_core/workspace/workspace.py
 dagster/_daemon/__init__.py
```

### Comparing `dagster-1.7.4/dagster.egg-info/requires.txt` & `dagster-1.7.5/dagster.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 sqlalchemy<3,>=1.0
 toposort>=1.0
 watchdog>=0.8.3
 docstring-parser
 pydantic!=1.10.7,<3,>1.10.0
 rich
 filelock
-dagster-pipes==1.7.4
+dagster-pipes==1.7.5
 
 [:platform_system == "Windows"]
 psutil>=1.0
 pywin32!=226
 
 [:python_version < "3.11"]
 protobuf<5,>=3.20.0
```

### Comparing `dagster-1.7.4/setup.py` & `dagster-1.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         "docstring-parser",
         "universal_pathlib; python_version<'3.12'",
         "universal_pathlib>=0.2.0; python_version>='3.12'",
         # https://github.com/pydantic/pydantic/issues/5821
         "pydantic>1.10.0,!= 1.10.7,<3",
         "rich",
         "filelock",
-        "dagster-pipes==1.7.4",
+        "dagster-pipes==1.7.5",
     ],
     extras_require={
         "docker": ["docker"],
         "test": [
             "buildkite-test-collector",
             "docker",
             f"grpcio-tools>={GRPC_VERSION_FLOOR}",
```

