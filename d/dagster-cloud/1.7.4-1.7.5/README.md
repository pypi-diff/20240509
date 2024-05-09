# Comparing `tmp/dagster-cloud-1.7.4.tar.gz` & `tmp/dagster-cloud-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-1.7.4.tar", last modified: Thu May  2 20:44:01 2024, max compression
+gzip compressed data, was "dagster-cloud-1.7.5.tar", last modified: Thu May  9 17:58:27 2024, max compression
```

## Comparing `dagster-cloud-1.7.4.tar` & `dagster-cloud-1.7.5.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.758723 dagster-cloud-1.7.4/
--rw-r--r--   0 root         (0) root         (0)     4562 2024-05-02 20:44:01.758723 dagster-cloud-1.7.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.690724 dagster-cloud-1.7.4/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      316 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.694724 dagster-cloud-1.7.4/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)      796 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.694724 dagster-cloud-1.7.4/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45582 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1837 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.694724 dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9296 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/defs.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/mutation.py
--rw-r--r--   0 root         (0) root         (0)     1986 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.698724 dagster-cloud-1.7.4/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19251 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.698724 dagster-cloud-1.7.4/dagster_cloud/artifacts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/artifacts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.702724 dagster-cloud-1.7.4/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      248 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1242 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/auth/constants.py
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.706724 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/
--rw-r--r--   0 root         (0) root         (0)     1873 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.706724 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py
--rw-r--r--   0 root         (0) root         (0)     7964 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     3234 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/errors.py
--rw-r--r--   0 root         (0) root         (0)     2524 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/insights_utils.py
--rw-r--r--   0 root         (0) root         (0)     4194 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/metrics_utils.py
--rw-r--r--   0 root         (0) root         (0)     1403 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.710724 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5611 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py
--rw-r--r--   0 root         (0) root         (0)     5185 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     7254 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/definitions.py
--rw-r--r--   0 root         (0) root         (0)    10624 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py
--rw-r--r--   0 root         (0) root         (0)     3808 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.710724 dagster-cloud-1.7.4/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.714724 dagster-cloud-1.7.4/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3098 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.714724 dagster-cloud-1.7.4/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    17294 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.714724 dagster-cloud-1.7.4/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.718724 dagster-cloud-1.7.4/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    22345 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.718724 dagster-cloud-1.7.4/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.718724 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.722724 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3907 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9301 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5251 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3790 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.726724 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.726724 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     2115 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17844 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)    12797 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    15703 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     3322 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.730723 dagster-cloud-1.7.4/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1620 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.730723 dagster-cloud-1.7.4/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4247 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.730723 dagster-cloud-1.7.4/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.734723 dagster-cloud-1.7.4/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4753 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.738723 dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16377 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    46580 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.738723 dagster-cloud-1.7.4/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6446 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    18839 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.742723 dagster-cloud-1.7.4/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     7575 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.742723 dagster-cloud-1.7.4/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2778 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4693 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/util/container_resources.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.742723 dagster-cloud-1.7.4/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.746723 dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)    10918 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     6575 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     5319 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.746723 dagster-cloud-1.7.4/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12977 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      352 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.750723 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28818 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    28623 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      534 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4126 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     2746 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.754723 dagster-cloud-1.7.4/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26248 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)     9825 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/kubernetes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.758723 dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14248 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    83997 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1209 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 20:44:01.690724 dagster-cloud-1.7.4/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4562 2024-05-02 20:44:01.000000 dagster-cloud-1.7.4/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4240 2024-05-02 20:44:01.000000 dagster-cloud-1.7.4/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 20:44:01.000000 dagster-cloud-1.7.4/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      509 2024-05-02 20:44:01.000000 dagster-cloud-1.7.4/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-02 20:44:01.000000 dagster-cloud-1.7.4/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 20:44:01.758723 dagster-cloud-1.7.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3078 2024-05-02 20:32:04.000000 dagster-cloud-1.7.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.536201 dagster-cloud-1.7.5/
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-05-09 17:58:27.536201 dagster-cloud-1.7.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.464201 dagster-cloud-1.7.5/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      316 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.468201 dagster-cloud-1.7.5/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)      826 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.468201 dagster-cloud-1.7.5/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45896 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.468201 dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9443 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/defs.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/mutation.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.468201 dagster-cloud-1.7.5/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19251 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.476201 dagster-cloud-1.7.5/dagster_cloud/artifacts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/artifacts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.476201 dagster-cloud-1.7.5/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/auth/constants.py
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.476201 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/
+-rw-r--r--   0 root         (0) root         (0)     1873 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.480201 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7964 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/insights_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/metrics_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.484201 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py
+-rw-r--r--   0 root         (0) root         (0)     5185 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/definitions.py
+-rw-r--r--   0 root         (0) root         (0)    10624 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.484201 dagster-cloud-1.7.5/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.484201 dagster-cloud-1.7.5/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.484201 dagster-cloud-1.7.5/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    17294 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.488201 dagster-cloud-1.7.5/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.488201 dagster-cloud-1.7.5/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    22345 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.488201 dagster-cloud-1.7.5/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.492201 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.496201 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9301 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.496201 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.500201 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17844 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)    12797 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    15703 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.500201 dagster-cloud-1.7.5/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.504201 dagster-cloud-1.7.5/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.504201 dagster-cloud-1.7.5/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.504201 dagster-cloud-1.7.5/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4753 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.508201 dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16377 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    46580 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.512201 dagster-cloud-1.7.5/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6446 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    18839 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.512201 dagster-cloud-1.7.5/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7585 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.516201 dagster-cloud-1.7.5/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/util/container_resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.516201 dagster-cloud-1.7.5/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.520201 dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)    10918 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.524201 dagster-cloud-1.7.5/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12977 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      352 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.528201 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28818 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    28623 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.528201 dagster-cloud-1.7.5/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26248 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)     9825 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/kubernetes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.536201 dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14248 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    83997 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.464201 dagster-cloud-1.7.5/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-05-09 17:58:27.000000 dagster-cloud-1.7.5/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4240 2024-05-09 17:58:27.000000 dagster-cloud-1.7.5/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:58:27.000000 dagster-cloud-1.7.5/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      509 2024-05-09 17:58:27.000000 dagster-cloud-1.7.5/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-09 17:58:27.000000 dagster-cloud-1.7.5/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 17:58:27.536201 dagster-cloud-1.7.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/setup.py
```

### Comparing `dagster-cloud-1.7.4/PKG-INFO` & `dagster-cloud-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.7.4
+Version: 1.7.5
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-cloud-1.7.4/README.md` & `dagster-cloud-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/agent/__init__.py` & `dagster-cloud-1.7.5/dagster_cloud/agent/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import List, NamedTuple, Optional
 
 from dagster._serdes import (
     whitelist_for_serdes,
 )
-
-AgentQueue = Optional[str]
+from dagster_cloud_cli.core.agent_queue import AgentQueue
 
 
 @whitelist_for_serdes
 class AgentQueuesConfig(NamedTuple):
     include_default_queue: bool = True
     additional_queues: Optional[List[AgentQueue]] = None
```

### Comparing `dagster-cloud-1.7.4/dagster_cloud/agent/cli/__init__.py` & `dagster-cloud-1.7.5/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster-cloud-1.7.5/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,18 @@
     retrieve_containerized_utilization_metrics,
 )
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from dagster._utils.interrupts import raise_interrupts_as
 from dagster._utils.merger import merge_dicts
 from dagster._utils.typed_dict import init_optional_typeddict
 from dagster_cloud_cli.core.errors import raise_http_error
-from dagster_cloud_cli.core.workspace import CodeDeploymentMetadata
+from dagster_cloud_cli.core.workspace import (
+    CodeDeploymentMetadata,
+    get_instance_ref_for_user_code,
+)
 
 from dagster_cloud.api.dagster_cloud_api import (
     AgentHeartbeat,
     AgentUtilizationMetrics,
     DagsterCloudApi,
     DagsterCloudApiErrorResponse,
     DagsterCloudApiGrpcResponse,
@@ -625,14 +628,19 @@
         elif api_name == DagsterCloudApi.GET_EXTERNAL_NOTEBOOK_DATA:
             return request.request_args.code_location_origin
         elif api_name == DagsterCloudApi.PING_LOCATION:
             return RegisteredCodeLocationOrigin(request.request_args.location_name)
         else:
             return None
 
+    def _get_user_code_instance_ref(
+        self, instance: DagsterCloudAgentInstance, deployment_name: str
+    ):
+        return get_instance_ref_for_user_code(instance.ref_for_deployment(deployment_name))
+
     def _handle_api_request(
         self,
         request: DagsterCloudApiRequest,
         deployment_name: str,
         is_branch_deployment: bool,
         instance: DagsterCloudAgentInstance,
         user_code_launcher: DagsterCloudUserCodeLauncher,
@@ -654,15 +662,15 @@
             return DagsterCloudApiSuccess()
         elif api_name == DagsterCloudApi.GET_EXTERNAL_EXECUTION_PLAN:
             client = self._get_grpc_client(
                 user_code_launcher, deployment_name, cast(str, location_name)
             )
             serialized_snapshot_or_error = client.execution_plan_snapshot(
                 execution_plan_snapshot_args=request.request_args._replace(
-                    instance_ref=instance.ref_for_deployment(deployment_name)
+                    instance_ref=self._get_user_code_instance_ref(instance, deployment_name)
                 )
             )
             return DagsterCloudApiGrpcResponse(serialized_snapshot_or_error)
 
         elif api_name == DagsterCloudApi.GET_SUBSET_EXTERNAL_PIPELINE_RESULT:
             client = self._get_grpc_client(
                 user_code_launcher, deployment_name, cast(str, location_name)
@@ -709,30 +717,30 @@
             return DagsterCloudApiGrpcResponse(serialized_partition_execution_params_or_error)
         elif api_name == DagsterCloudApi.GET_EXTERNAL_SCHEDULE_EXECUTION_DATA:
             client = self._get_grpc_client(
                 user_code_launcher, deployment_name, cast(str, location_name)
             )
 
             args = request.request_args._replace(
-                instance_ref=instance.ref_for_deployment(deployment_name)
+                instance_ref=self._get_user_code_instance_ref(instance, deployment_name)
             )
 
             serialized_schedule_data_or_error = client.external_schedule_execution(
                 external_schedule_execution_args=args,
             )
 
             return DagsterCloudApiGrpcResponse(serialized_schedule_data_or_error)
 
         elif api_name == DagsterCloudApi.GET_EXTERNAL_SENSOR_EXECUTION_DATA:
             client = self._get_grpc_client(
                 user_code_launcher, deployment_name, cast(str, location_name)
             )
 
             args = request.request_args._replace(
-                instance_ref=instance.ref_for_deployment(deployment_name)
+                instance_ref=self._get_user_code_instance_ref(instance, deployment_name)
             )
 
             serialized_sensor_data_or_error = client.external_sensor_execution(
                 sensor_execution_args=args,
             )
 
             return DagsterCloudApiGrpcResponse(serialized_sensor_data_or_error)
@@ -742,15 +750,15 @@
             )
             response = client.external_notebook_data(request.request_args.notebook_path)
             return DagsterCloudApiGrpcResponse(response.decode())
         elif api_name == DagsterCloudApi.LAUNCH_RUN:
             run = request.request_args.dagster_run
 
             with DagsterInstance.from_ref(
-                instance.ref_for_deployment(deployment_name)
+                self._get_user_code_instance_ref(instance, deployment_name)
             ) as scoped_instance:
                 scoped_instance.report_engine_event(
                     f"{instance.agent_display_name} is launching run {run.run_id}",
                     run,
                     cls=self.__class__,
                 )
```

### Comparing `dagster-cloud-1.7.4/dagster_cloud/agent/queries.py` & `dagster-cloud-1.7.5/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/defs.py` & `dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,86 @@
 from typing import Iterable, Optional, Sequence, Union, cast
 
 from dagster import (
     AssetCheckExecutionContext,
     MetadataValue,
     _check as check,
 )
+from dagster._core.definitions.asset_check_factories.freshness_checks.last_update import (
+    construct_description,
+)
+from dagster._core.definitions.asset_check_factories.utils import (
+    FRESH_UNTIL_METADATA_KEY,
+    LAST_UPDATED_TIMESTAMP_METADATA_KEY,
+    LOWER_BOUND_TIMESTAMP_METADATA_KEY,
+    assets_to_keys,
+    unique_id_from_asset_keys,
+)
 from dagster._core.definitions.asset_check_result import AssetCheckResult
-from dagster._core.definitions.asset_check_spec import AssetCheckSeverity, AssetCheckSpec
+from dagster._core.definitions.asset_check_spec import (
+    AssetCheckKey,
+    AssetCheckSeverity,
+    AssetCheckSpec,
+)
 from dagster._core.definitions.asset_checks import AssetChecksDefinition
 from dagster._core.definitions.asset_key import AssetKey
 from dagster._core.definitions.assets import AssetsDefinition
 from dagster._core.definitions.decorators.asset_check_decorator import multi_asset_check
 from dagster._core.definitions.events import CoercibleToAssetKey
-from dagster._core.definitions.freshness_checks.utils import (
-    asset_to_keys_iterable,
-    seconds_in_words,
-    unique_id_from_asset_keys,
-)
 from dagster._core.definitions.source_asset import SourceAsset
 from dagster._core.errors import (
     DagsterError,
     DagsterInvariantViolationError,
 )
 from dagster._core.instance import DagsterInstance
-from dagster_cloud_cli.core.graphql_client import create_cloud_webserver_client
+from dagster_cloud_cli.core.graphql_client import (
+    DagsterCloudGraphQLClient,
+    create_cloud_webserver_client,
+)
 
 from dagster_cloud import DagsterCloudAgentInstance
 
 from .mutation import ANOMALY_DETECTION_INFERENCE_MUTATION
 from .types import (
     AnomalyDetectionModelParams,
     BetaFreshnessAnomalyDetectionParams,
+    FreshnessAnomalyDetectionResult,
 )
 
 DEFAULT_MODEL_PARAMS = BetaFreshnessAnomalyDetectionParams(sensitivity=0.1)
+MODEL_PARAMS_METADATA_KEY = "dagster/anomaly_detection_model_params"
+MODEL_VERSION_METADATA_KEY = "dagster/anomaly_detection_model_version"
+MODEL_TRAINING_RANGE_START_TIMESTAMP_METADATA_KEY = (
+    "dagster/anomaly_detection_model_training_range_start_timestamp"
+)
+MODEL_TRAINING_RANGE_END_TIMESTAMP_METADATA_KEY = (
+    "dagster/anomaly_detection_model_training_range_end_timestamp"
+)
+MAXIMUM_ACCEPTABLE_DELTA_METADATA_KEY = "dagster/anomaly_detection_maximum_acceptable_delta"
 
 
 class DagsterCloudAnomalyDetectionFailed(DagsterError):
     """Raised when an anomaly detection check fails host-side."""
 
 
 def _build_check_for_assets(
     asset_keys: Sequence[AssetKey],
     params: AnomalyDetectionModelParams,
+    severity: AssetCheckSeverity,
 ) -> AssetChecksDefinition:
     @multi_asset_check(
         specs=[
             AssetCheckSpec(
                 name="anomaly_detection_freshness_check",
                 description=f"Detects anomalies in the freshness of the asset using model {params.model_version.value.lower()}.",
                 asset=asset_key,
+                metadata={
+                    MODEL_PARAMS_METADATA_KEY: params.as_metadata,
+                    MODEL_VERSION_METADATA_KEY: params.model_version.value,
+                },
             )
             for asset_key in asset_keys
         ],
         can_subset=True,
         name=f"anomaly_detection_freshness_check_{unique_id_from_asset_keys(asset_keys)}",
     )
     def the_check(context: AssetCheckExecutionContext) -> Iterable[AssetCheckResult]:
@@ -67,143 +94,144 @@
         with create_cloud_webserver_client(
             instance.dagit_url[:-1]
             if instance.dagit_url.endswith("/")
             else instance.dagit_url,  # Remove trailing slash
             check.str_param(instance.dagster_cloud_agent_token, "dagster_cloud_agent_token"),
         ) as client:
             for check_key in context.selected_asset_check_keys:
-                asset_key = check_key.asset_key
-                if not context.job_def.asset_layer.has(asset_key):
-                    raise Exception(f"Could not find targeted asset {asset_key.to_string()}.")
-                result = client.execute(
-                    ANOMALY_DETECTION_INFERENCE_MUTATION,
-                    {
-                        "modelVersion": params.model_version.value,
-                        "params": {
-                            **dict(params),
-                            "asset_key_user_string": asset_key.to_user_string(),
-                        },
-                    },
-                )
-                data = result["data"]["anomalyDetectionInference"]
-                metadata = {
-                    "model_params": {**params.as_metadata},
-                    "model_version": params.model_version.value,
-                }
-                if data["__typename"] != "AnomalyDetectionSuccess":
-                    yield handle_anomaly_detection_inference_failure(
-                        data, metadata, params, asset_key
-                    )
-                    continue
-                response = result["data"]["anomalyDetectionInference"]["response"]
-                overdue_seconds = check.float_param(response["overdue_seconds"], "overdue_seconds")
-                overdue_deadline_timestamp = response["overdue_deadline_timestamp"]
-                metadata["overdue_deadline_timestamp"] = MetadataValue.timestamp(
-                    overdue_deadline_timestamp
-                )
-                metadata["model_training_range_start_timestamp"] = MetadataValue.timestamp(
-                    response["model_training_range_start_timestamp"]
-                )
-                metadata["model_training_range_end_timestamp"] = MetadataValue.timestamp(
-                    response["model_training_range_end_timestamp"]
-                )
-
-                last_updated_timestamp = response["last_updated_timestamp"]
-                if last_updated_timestamp is None:
-                    yield AssetCheckResult(
-                        passed=True,
-                        description="The asset has never been materialized or otherwise observed to have been updated",
-                    )
-                    continue
-
-                evaluation_timestamp = response["evaluation_timestamp"]
-                last_update_lag_str = seconds_in_words(
-                    evaluation_timestamp - last_updated_timestamp
-                )
-                expected_lag_str = seconds_in_words(
-                    overdue_deadline_timestamp - last_updated_timestamp
-                )
-                gt_or_lte_str = "greater than" if overdue_seconds > 0 else "less than or equal to"
-                lag_comparison_str = (
-                    f"At the time of this check's evaluation, {last_update_lag_str} had passed since its "
-                    f"last update. This is {gt_or_lte_str} the allowed {expected_lag_str} threshold, which "
-                    "is based on its prior history of updates."
-                )
-
-                if overdue_seconds > 0:
-                    metadata["overdue_minutes"] = round(overdue_seconds / 60, 2)
-
-                    yield AssetCheckResult(
-                        passed=False,
-                        severity=AssetCheckSeverity.WARN,
-                        metadata=metadata,
-                        description=f"The asset is overdue for an update. {lag_comparison_str}",
-                        asset_key=asset_key,
-                    )
-                else:
-                    yield AssetCheckResult(
-                        passed=True,
-                        metadata=metadata,
-                        description=f"The asset is fresh. {lag_comparison_str}",
-                        asset_key=asset_key,
-                    )
+                yield _anomaly_detection_inner(check_key, context, client, params, severity)
 
     return the_check
 
 
 def handle_anomaly_detection_inference_failure(
-    data: dict, metadata: dict, params: AnomalyDetectionModelParams, asset_key: AssetKey
+    data: dict,
+    metadata: dict,
+    params: AnomalyDetectionModelParams,
+    asset_key: AssetKey,
+    severity: AssetCheckSeverity,
 ) -> AssetCheckResult:
     if (
         data["__typename"] == "AnomalyDetectionFailure"
         and data["message"] == params.model_version.minimum_required_records_msg
     ):
         # Intercept failure in the case of not enough records, and return a pass to avoid
         # being too noisy with failures.
         return AssetCheckResult(
             passed=True,
-            severity=AssetCheckSeverity.WARN,
+            severity=severity,
             metadata=metadata,
             description=data["message"],
             asset_key=asset_key,
         )
     raise DagsterCloudAnomalyDetectionFailed(f"Anomaly detection failed: {data['message']}")
 
 
+def _anomaly_detection_inner(
+    check_key: AssetCheckKey,
+    context: AssetCheckExecutionContext,
+    client: DagsterCloudGraphQLClient,
+    params: AnomalyDetectionModelParams,
+    severity: AssetCheckSeverity,
+) -> AssetCheckResult:
+    asset_key = check_key.asset_key
+    if not context.job_def.asset_layer.has(asset_key):
+        raise Exception(f"Could not find targeted asset {asset_key.to_string()}.")
+    result = client.execute(
+        ANOMALY_DETECTION_INFERENCE_MUTATION,
+        {
+            "modelVersion": params.model_version.value,
+            "params": {
+                **dict(params),
+                "asset_key_user_string": asset_key.to_user_string(),
+            },
+        },
+    )
+    data = result["data"]["anomalyDetectionInference"]
+    metadata = {
+        MODEL_PARAMS_METADATA_KEY: {**params.as_metadata},
+        MODEL_VERSION_METADATA_KEY: params.model_version.value,
+    }
+    if data["__typename"] != "AnomalyDetectionSuccess":
+        return handle_anomaly_detection_inference_failure(
+            data, metadata, params, asset_key, severity
+        )
+    response = result["data"]["anomalyDetectionInference"]["response"]
+    result_obj = FreshnessAnomalyDetectionResult(**response)
+    metadata[MODEL_TRAINING_RANGE_START_TIMESTAMP_METADATA_KEY] = MetadataValue.timestamp(
+        result_obj.model_training_range_start_timestamp
+    )
+    metadata[MODEL_TRAINING_RANGE_END_TIMESTAMP_METADATA_KEY] = MetadataValue.timestamp(
+        result_obj.model_training_range_end_timestamp
+    )
+    metadata[LAST_UPDATED_TIMESTAMP_METADATA_KEY] = MetadataValue.timestamp(
+        result_obj.last_updated_timestamp
+    )
+    metadata[LOWER_BOUND_TIMESTAMP_METADATA_KEY] = MetadataValue.timestamp(
+        result_obj.last_update_time_lower_bound
+    )
+    passed = result_obj.last_update_time_lower_bound <= result_obj.last_updated_timestamp
+
+    if passed:
+        fresh_until = result_obj.last_updated_timestamp + result_obj.maximum_acceptable_delta
+        metadata[FRESH_UNTIL_METADATA_KEY] = MetadataValue.timestamp(fresh_until)
+
+    return AssetCheckResult(
+        passed=passed,
+        description=construct_description(
+            passed=passed,
+            last_update_time_lower_bound=result_obj.last_update_time_lower_bound,
+            current_timestamp=result_obj.evaluation_timestamp,
+            update_timestamp=result_obj.last_updated_timestamp,
+        ),
+        severity=AssetCheckSeverity.WARN,
+        metadata=metadata,
+        asset_key=asset_key,
+    )
+
+
 def build_anomaly_detection_freshness_checks(
     *,
     assets: Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]],
     params: Optional[AnomalyDetectionModelParams],
-) -> AssetChecksDefinition:
+    severity: AssetCheckSeverity = AssetCheckSeverity.WARN,
+) -> Sequence[AssetChecksDefinition]:
     """Builds a list of asset checks which utilize anomaly detection algorithms to
     determine the freshness of data.
 
     Args:
         assets (Sequence[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]]): The assets to construct checks for. For each passed in
             asset, there will be a corresponding constructed `AssetChecksDefinition`.
         params (AnomalyDetectionModelParams): The parameters to use for the model. The parameterization corresponds to the model used.
+        severity (AssetCheckSeverity): The severity of the check. Defaults to `AssetCheckSeverity.WARN`.
 
     Returns:
-        AssetChecksDefinition: A list of `AssetChecksDefinition` objects, each corresponding to an asset in the `assets` parameter.
+        Sequence[AssetChecksDefinition]: `AssetChecksDefinition` objects which execute freshness checks
+            for the provided assets.
 
     Examples:
         .. code-block:: python
 
             from dagster_cloud import build_anomaly_detection_freshness_checks, BetaFreshnessAnomalyDetectionParams
 
             checks_def = build_anomaly_detection_freshness_checks(
                 assets=[AssetKey("foo_asset"), AssetKey("foo_asset")],
                 params=BetaFreshnessAnomalyDetectionParams(sensitivity=0.1),
             )
     """
     params = check.opt_inst_param(
         params, "params", AnomalyDetectionModelParams, DEFAULT_MODEL_PARAMS
     )
-    return _build_check_for_assets(
-        [asset_key for asset in assets for asset_key in asset_to_keys_iterable(asset)], params
-    )
+    severity = check.inst_param(severity, "severity", AssetCheckSeverity)
+    return [
+        _build_check_for_assets(
+            [asset_key for asset in assets for asset_key in assets_to_keys([asset])],
+            params,
+            severity,
+        )
+    ]
 
 
 def _is_agent_instance(instance: DagsterInstance) -> bool:
     if hasattr(instance, "dagster_cloud_agent_token") and hasattr(instance, "dagit_url"):
         return True
     return False
```

### Comparing `dagster-cloud-1.7.4/dagster_cloud/anomaly_detection/types.py` & `dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 from abc import abstractproperty
 from enum import Enum
-from typing import Dict
+from typing import Any, Dict
 
-from dagster._core.definitions.metadata import FloatMetadataValue, MetadataValue
+from dagster import DagsterError
 from pydantic import BaseModel
 
 
+class AnomalyDetectionError(DagsterError):
+    pass
+
+
+class FreshnessAnomalyDetectionResult(BaseModel):
+    last_updated_timestamp: float
+    evaluation_timestamp: float
+    last_update_time_lower_bound: float
+    maximum_acceptable_delta: float
+    model_training_range_start_timestamp: float
+    model_training_range_end_timestamp: float
+
+
 class AnomalyDetectionModelVersion(Enum):
     FRESHNESS_BETA = "FRESHNESS_BETA"
 
     @property
     def minimum_required_records(self) -> int:
         if self == AnomalyDetectionModelVersion.FRESHNESS_BETA:
             return 15
@@ -43,23 +56,23 @@
 
 class AnomalyDetectionModelParams(BaseModel):
     @abstractproperty
     def model_version(self) -> AnomalyDetectionModelVersion:
         raise NotImplementedError("Subclasses must implement this method")
 
     @abstractproperty
-    def as_metadata(self) -> Dict[str, MetadataValue]:
+    def as_metadata(self) -> Dict[str, Any]:
         raise NotImplementedError("Subclasses must implement this method")
 
 
 class BetaFreshnessAnomalyDetectionParams(AnomalyDetectionModelParams):
     sensitivity: float
 
     @property
     def model_version(self) -> AnomalyDetectionModelVersion:
         return AnomalyDetectionModelVersion.FRESHNESS_BETA
 
     @property
-    def as_metadata(self) -> Dict[str, MetadataValue]:
+    def as_metadata(self) -> Dict[str, Any]:
         return {
-            "sensitivity": FloatMetadataValue(self.sensitivity),
+            "sensitivity": self.sensitivity,
         }
```

### Comparing `dagster-cloud-1.7.4/dagster_cloud/api/dagster_cloud_api.py` & `dagster-cloud-1.7.5/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/auth/constants.py` & `dagster-cloud-1.7.5/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/__init__.py` & `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py` & `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py` & `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py` & `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/insights_utils.py` & `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/insights_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/metrics_utils.py` & `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/query.py` & `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/query.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py` & `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py` & `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/definitions.py` & `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py` & `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py` & `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster-cloud-1.7.5/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 import dagster._check as check
 from dagster._core.launcher import RunLauncher
 from dagster._core.launcher.base import LaunchRunContext
 from dagster._core.utils import parse_env_var
 from dagster._grpc.types import ExecuteRunArgs
 from dagster._serdes.ipc import open_ipc_subprocess
+from dagster_cloud_cli.core.workspace import (
+    get_instance_ref_for_user_code,
+)
 
 from dagster_cloud.execution.utils import TaskStatus
 from dagster_cloud.execution.utils.process import check_on_process, kill_process
 
 PID_TAG = "process/pid"
 
 
@@ -22,15 +25,15 @@
     def launch_run(self, context: LaunchRunContext) -> None:
         run = context.dagster_run
         pipeline_code_origin = check.not_none(context.job_code_origin)
 
         run_args = ExecuteRunArgs(
             job_origin=pipeline_code_origin,
             run_id=run.run_id,
-            instance_ref=self._instance.get_ref(),
+            instance_ref=get_instance_ref_for_user_code(self._instance.get_ref()),
         )
         args = run_args.get_command_args()
 
         kwargs = {}
         if (
             run.job_code_origin
             and run.job_code_origin.repository_origin.container_context
```

### Comparing `dagster-cloud-1.7.4/dagster_cloud/execution/monitoring/__init__.py` & `dagster-cloud-1.7.5/dagster_cloud/execution/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/execution/utils/process.py` & `dagster-cloud-1.7.5/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/instance/__init__.py` & `dagster-cloud-1.7.5/dagster_cloud/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/client.py` & `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/compile.py` & `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/manager.py` & `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/registry.py` & `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/server/server.py` & `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/pex/grpc/types.py` & `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/secrets/loader.py` & `dagster-cloud-1.7.5/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/serverless/io_manager.py` & `dagster-cloud-1.7.5/dagster_cloud/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/storage/client.py` & `dagster-cloud-1.7.5/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster-cloud-1.7.5/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/queries.py` & `dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/storage.py` & `dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/storage/event_logs/utils.py` & `dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/storage/runs/queries.py` & `dagster-cloud-1.7.5/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/storage/runs/storage.py` & `dagster-cloud-1.7.5/dagster_cloud/storage/runs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/storage/schedules/queries.py` & `dagster-cloud-1.7.5/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/storage/schedules/storage.py` & `dagster-cloud-1.7.5/dagster_cloud/storage/schedules/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TYPE_CHECKING, Any, Iterable, Optional, Sequence, Set
 
 import dagster._check as check
 from dagster import AssetKey
-from dagster._core.definitions.asset_condition.asset_condition import (
+from dagster._core.definitions.declarative_scheduling.serialized_objects import (
     AssetConditionEvaluationWithRunIds,
 )
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.scheduler.instigation import (
     AutoMaterializeAssetEvaluationRecord,
     InstigatorState,
     InstigatorStatus,
```

### Comparing `dagster-cloud-1.7.4/dagster_cloud/util/__init__.py` & `dagster-cloud-1.7.5/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/util/container_resources.py` & `dagster-cloud-1.7.5/dagster_cloud/util/container_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/__init__.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/docker.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/ecs.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/docker/__init__.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/client.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/launcher.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/service.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/ecs/utils.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/kubernetes/utils.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/dagster_cloud.egg-info/PKG-INFO` & `dagster-cloud-1.7.5/dagster_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.7.4
+Version: 1.7.5
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-cloud-1.7.4/dagster_cloud.egg-info/SOURCES.txt` & `dagster-cloud-1.7.5/dagster_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.4/setup.py` & `dagster-cloud-1.7.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.7.4",
-        "dagster-cloud-cli==1.7.4",
+        "dagster==1.7.5",
+        "dagster-cloud-cli==1.7.5",
         "pex>=2.1.132,<3",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -62,21 +62,21 @@
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
             "dbt-core",
             "dbt-snowflake",
             "dbt-postgres",
             "dbt-duckdb",
-            "dagster-dbt==0.23.4",
-            "dagster_k8s==0.23.4",
+            "dagster-dbt==0.23.5",
+            "dagster_k8s==0.23.5",
         ],
         "insights": ["pyarrow"],
-        "docker": ["docker", "dagster_docker==0.23.4"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.23.4"],
-        "ecs": ["dagster_aws==0.23.4", "boto3"],
+        "docker": ["docker", "dagster_docker==0.23.5"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.23.5"],
+        "ecs": ["dagster_aws==0.23.5", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

