# Comparing `tmp/h2o-featurestore-1.1.2.tar.gz` & `tmp/h2o-featurestore-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h2o-featurestore-1.1.2.tar", last modified: Thu Nov 30 12:37:53 2023, max compression
+gzip compressed data, was "h2o-featurestore-1.2.0.tar", last modified: Wed Jan 24 09:13:04 2024, max compression
```

## Comparing `h2o-featurestore-1.1.2.tar` & `h2o-featurestore-1.2.0.tar`

### file list

```diff
@@ -1,130 +1,137 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-30 12:37:53.756812 h2o-featurestore-1.1.2/
--rw-r--r--   0 root         (0) root         (0)      151 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1210 2023-11-30 12:37:53.756812 h2o-featurestore-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      546 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-30 12:37:53.736812 h2o-featurestore-1.1.2/ai/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-30 12:37:53.736812 h2o-featurestore-1.1.2/ai/h2o/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-30 12:37:53.736812 h2o-featurestore-1.1.2/ai/h2o/featurestore/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-30 12:37:53.736812 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-30 12:37:53.740812 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/
--rw-r--r--   0 root         (0) root         (0)   217063 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/CoreService_pb2.py
--rw-r--r--   0 root         (0) root         (0)   337926 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/CoreService_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1419 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/DashboardApi_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/DashboardApi_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/FeatureSetProtoApi_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/FeatureSetProtoApi_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2228 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/FeatureSetSearch_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/FeatureSetSearch_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8760 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/OnlineApi_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/OnlineApi_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3447 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/RecommendationProtoApi_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/RecommendationProtoApi_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2258 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/TimeToLiveApi_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/TimeToLiveApi_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-30 12:37:53.740812 h2o-featurestore-1.1.2/featurestore/
--rw-r--r--   0 root         (0) root         (0)     2489 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16557 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-30 12:37:53.744812 h2o-featurestore-1.1.2/featurestore/core/
--rw-r--r--   0 root         (0) root         (0)       69 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1387 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/access_type.py
--rw-r--r--   0 root         (0) root         (0)     8668 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/acl.py
--rw-r--r--   0 root         (0) root         (0)     7392 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/auth.py
--rw-r--r--   0 root         (0) root         (0)     1121 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/browser.py
--rw-r--r--   0 root         (0) root         (0)      235 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-30 12:37:53.748812 h2o-featurestore-1.1.2/featurestore/core/collections/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4577 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/artifacts.py
--rw-r--r--   0 root         (0) root         (0)     7324 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/classifiers.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/feature_set_reviews.py
--rw-r--r--   0 root         (0) root         (0)     7890 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/feature_sets.py
--rw-r--r--   0 root         (0) root         (0)     2890 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/feature_views.py
--rw-r--r--   0 root         (0) root         (0)     2698 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/ingest_history.py
--rw-r--r--   0 root         (0) root         (0)     4134 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/jobs.py
--rw-r--r--   0 root         (0) root         (0)     4571 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/ml_datasets.py
--rw-r--r--   0 root         (0) root         (0)     4665 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/pats.py
--rw-r--r--   0 root         (0) root         (0)     4499 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/projects.py
--rw-r--r--   0 root         (0) root         (0)     3333 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/scheduled_tasks.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/collections/transformation_functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-30 12:37:53.748812 h2o-featurestore-1.1.2/featurestore/core/commons/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/commons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/commons/case_insensitive_dict.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/commons/spark_utils.py
--rw-r--r--   0 root         (0) root         (0)     1868 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/config.py
--rw-r--r--   0 root         (0) root         (0)    12173 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/credentials.py
--rw-r--r--   0 root         (0) root         (0)     2795 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/dashboard.py
--rw-r--r--   0 root         (0) root         (0)    15193 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/data_source_wrappers.py
--rw-r--r--   0 root         (0) root         (0)      807 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/data_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-30 12:37:53.756812 h2o-featurestore-1.1.2/featurestore/core/entities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/advanced_search_option.py
--rw-r--r--   0 root         (0) root         (0)     3974 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/artifact.py
--rw-r--r--   0 root         (0) root         (0)      653 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/backfill_job.py
--rw-r--r--   0 root         (0) root         (0)     1288 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/backfill_option.py
--rw-r--r--   0 root         (0) root         (0)     2616 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/base_job.py
--rw-r--r--   0 root         (0) root         (0)      789 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/component_versions.py
--rw-r--r--   0 root         (0) root         (0)      196 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/compute_recommendation_classifiers_job.py
--rw-r--r--   0 root         (0) root         (0)      166 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/compute_statistics_job.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/create_ml_dataset_job.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/extract_schema_job.py
--rw-r--r--   0 root         (0) root         (0)    15108 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/feature.py
--rw-r--r--   0 root         (0) root         (0)      523 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/feature_ref.py
--rw-r--r--   0 root         (0) root         (0)    66613 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/feature_set.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/feature_set_popularity.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/feature_set_ref.py
--rw-r--r--   0 root         (0) root         (0)     5595 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/feature_set_review.py
--rw-r--r--   0 root         (0) root         (0)     4141 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/feature_set_schema.py
--rw-r--r--   0 root         (0) root         (0)     7269 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/feature_view.py
--rw-r--r--   0 root         (0) root         (0)     3330 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/ingest.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/ingest_job.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/materialization_online_job.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/ml_data_feature.py
--rw-r--r--   0 root         (0) root         (0)     8658 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/ml_dataset.py
--rw-r--r--   0 root         (0) root         (0)      590 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/optimize_storage_job.py
--rw-r--r--   0 root         (0) root         (0)     1350 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/pat.py
--rw-r--r--   0 root         (0) root         (0)      936 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/permission.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/permission_base.py
--rw-r--r--   0 root         (0) root         (0)     1986 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/permission_request.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/pinned_feature_set.py
--rw-r--r--   0 root         (0) root         (0)    13778 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/project.py
--rw-r--r--   0 root         (0) root         (0)     1431 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/project_history.py
--rw-r--r--   0 root         (0) root         (0)    15219 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/query.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/recently_used_feature_set.py
--rw-r--r--   0 root         (0) root         (0)     1111 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/recently_used_project.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/recommendation.py
--rw-r--r--   0 root         (0) root         (0)      671 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/retrieve_job.py
--rw-r--r--   0 root         (0) root         (0)      156 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/revert_ingest_job.py
--rw-r--r--   0 root         (0) root         (0)     6721 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/scheduled_task.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/task_execution_history.py
--rw-r--r--   0 root         (0) root         (0)     1957 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/transformation_function.py
--rw-r--r--   0 root         (0) root         (0)      477 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/user.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/entities/user_with_permission.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/feature_set_flow.py
--rw-r--r--   0 root         (0) root         (0)      718 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/interactive_console.py
--rw-r--r--   0 root         (0) root         (0)     5122 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/interceptors.py
--rw-r--r--   0 root         (0) root         (0)     1858 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/job_info.py
--rw-r--r--   0 root         (0) root         (0)      509 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/job_types.py
--rw-r--r--   0 root         (0) root         (0)    12957 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/retrieve_holder.py
--rw-r--r--   0 root         (0) root         (0)      216 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/review_statuses.py
--rw-r--r--   0 root         (0) root         (0)    18945 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/schema.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/search_field.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/search_operator.py
--rw-r--r--   0 root         (0) root         (0)     1651 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/storage_optimization.py
--rw-r--r--   0 root         (0) root         (0)     6733 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/transformations.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/user_credentials.py
--rw-r--r--   0 root         (0) root         (0)     4052 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/core/utils.py
--rw-r--r--   0 root         (0) root         (0)      947 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/logger.py
--rw-r--r--   0 root         (0) root         (0)     1750 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/rest_stub.py
--rw-r--r--   0 root         (0) root         (0)        5 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/featurestore/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-30 12:37:53.756812 h2o-featurestore-1.1.2/h2o_featurestore.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1210 2023-11-30 12:37:53.000000 h2o-featurestore-1.1.2/h2o_featurestore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4775 2023-11-30 12:37:53.000000 h2o-featurestore-1.1.2/h2o_featurestore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-30 12:37:53.000000 h2o-featurestore-1.1.2/h2o_featurestore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-11-30 12:37:53.000000 h2o-featurestore-1.1.2/h2o_featurestore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-11-30 12:37:53.000000 h2o-featurestore-1.1.2/h2o_featurestore.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-11-30 12:37:53.756812 h2o-featurestore-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1611 2023-11-29 11:44:08.000000 h2o-featurestore-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:13:04.600894 h2o-featurestore-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      151 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1626 2024-01-24 09:13:04.600894 h2o-featurestore-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      546 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:13:04.576894 h2o-featurestore-1.2.0/ai/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:13:04.576894 h2o-featurestore-1.2.0/ai/h2o/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:13:04.576894 h2o-featurestore-1.2.0/ai/h2o/featurestore/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:13:04.576894 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:13:04.584894 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/
+-rw-r--r--   0 root         (0) root         (0)   218902 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/CoreService_pb2.py
+-rw-r--r--   0 root         (0) root         (0)   375584 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/CoreService_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)   341695 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/CoreService_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/DashboardApi_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/DashboardApi_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      159 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/DashboardApi_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/FeatureSetProtoApi_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2856 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/FeatureSetProtoApi_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      159 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/FeatureSetProtoApi_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/FeatureSetSearch_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3754 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/FeatureSetSearch_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      159 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/FeatureSetSearch_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8760 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/OnlineApi_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    21970 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/OnlineApi_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      159 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/OnlineApi_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3447 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/RecommendationProtoApi_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6398 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/RecommendationProtoApi_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      159 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/RecommendationProtoApi_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/TimeToLiveApi_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3887 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/TimeToLiveApi_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      159 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/TimeToLiveApi_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:13:04.584894 h2o-featurestore-1.2.0/featurestore/
+-rw-r--r--   0 root         (0) root         (0)     2489 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16417 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:13:04.588894 h2o-featurestore-1.2.0/featurestore/core/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/access_type.py
+-rw-r--r--   0 root         (0) root         (0)     8508 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/acl.py
+-rw-r--r--   0 root         (0) root         (0)     7352 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/auth.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/browser.py
+-rw-r--r--   0 root         (0) root         (0)      235 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:13:04.592894 h2o-featurestore-1.2.0/featurestore/core/collections/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4577 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     7264 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/classifiers.py
+-rw-r--r--   0 root         (0) root         (0)     2809 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/feature_set_reviews.py
+-rw-r--r--   0 root         (0) root         (0)     7810 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/feature_sets.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/feature_views.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/ingest_history.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/jobs.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/ml_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     4645 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/pats.py
+-rw-r--r--   0 root         (0) root         (0)     4522 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/projects.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/scheduled_tasks.py
+-rw-r--r--   0 root         (0) root         (0)      950 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/collections/transformation_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:13:04.592894 h2o-featurestore-1.2.0/featurestore/core/commons/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/commons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/commons/case_insensitive_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1350 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/commons/spark_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/config.py
+-rw-r--r--   0 root         (0) root         (0)    12570 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/credentials.py
+-rw-r--r--   0 root         (0) root         (0)     2795 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/dashboard.py
+-rw-r--r--   0 root         (0) root         (0)    15193 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/data_source_wrappers.py
+-rw-r--r--   0 root         (0) root         (0)      807 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/data_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:13:04.600894 h2o-featurestore-1.2.0/featurestore/core/entities/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/advanced_search_option.py
+-rw-r--r--   0 root         (0) root         (0)     3974 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/artifact.py
+-rw-r--r--   0 root         (0) root         (0)      653 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/backfill_job.py
+-rw-r--r--   0 root         (0) root         (0)     1288 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/backfill_option.py
+-rw-r--r--   0 root         (0) root         (0)     2616 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/base_job.py
+-rw-r--r--   0 root         (0) root         (0)      789 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/component_versions.py
+-rw-r--r--   0 root         (0) root         (0)      196 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/compute_recommendation_classifiers_job.py
+-rw-r--r--   0 root         (0) root         (0)      166 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/compute_statistics_job.py
+-rw-r--r--   0 root         (0) root         (0)      464 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/create_ml_dataset_job.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/extract_schema_job.py
+-rw-r--r--   0 root         (0) root         (0)    15108 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/feature.py
+-rw-r--r--   0 root         (0) root         (0)      523 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/feature_ref.py
+-rw-r--r--   0 root         (0) root         (0)    67862 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/feature_set.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/feature_set_popularity.py
+-rw-r--r--   0 root         (0) root         (0)      415 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/feature_set_ref.py
+-rw-r--r--   0 root         (0) root         (0)     5495 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/feature_set_review.py
+-rw-r--r--   0 root         (0) root         (0)     4101 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/feature_set_schema.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/feature_view.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/ingest.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/ingest_job.py
+-rw-r--r--   0 root         (0) root         (0)      722 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/materialization_online_job.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/ml_data_feature.py
+-rw-r--r--   0 root         (0) root         (0)     8598 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/ml_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      590 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/optimize_storage_job.py
+-rw-r--r--   0 root         (0) root         (0)     1350 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/pat.py
+-rw-r--r--   0 root         (0) root         (0)      916 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/permission.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/permission_base.py
+-rw-r--r--   0 root         (0) root         (0)     1926 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/permission_request.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/pinned_feature_set.py
+-rw-r--r--   0 root         (0) root         (0)    13558 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/project.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/project_history.py
+-rw-r--r--   0 root         (0) root         (0)    15218 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/query.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/recently_used_feature_set.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/recently_used_project.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/recommendation.py
+-rw-r--r--   0 root         (0) root         (0)      671 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/retrieve_job.py
+-rw-r--r--   0 root         (0) root         (0)      156 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/revert_ingest_job.py
+-rw-r--r--   0 root         (0) root         (0)     6721 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/scheduled_task.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/task_execution_history.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/transformation_function.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/user.py
+-rw-r--r--   0 root         (0) root         (0)      977 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/entities/user_with_permission.py
+-rw-r--r--   0 root         (0) root         (0)      803 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/feature_set_flow.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/interactive_console.py
+-rw-r--r--   0 root         (0) root         (0)     5120 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/interceptors.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/job_info.py
+-rw-r--r--   0 root         (0) root         (0)      509 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/job_types.py
+-rw-r--r--   0 root         (0) root         (0)    12857 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/retrieve_holder.py
+-rw-r--r--   0 root         (0) root         (0)      216 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/review_statuses.py
+-rw-r--r--   0 root         (0) root         (0)    19028 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)      645 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/search_field.py
+-rw-r--r--   0 root         (0) root         (0)      466 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/search_operator.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/storage_optimization.py
+-rw-r--r--   0 root         (0) root         (0)     6733 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/transformations.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/user_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)      947 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1750 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/rest_stub.py
+-rw-r--r--   0 root         (0) root         (0)        5 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/featurestore/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:13:04.600894 h2o-featurestore-1.2.0/h2o_featurestore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1626 2024-01-24 09:13:04.000000 h2o-featurestore-1.2.0/h2o_featurestore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5128 2024-01-24 09:13:04.000000 h2o-featurestore-1.2.0/h2o_featurestore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-24 09:13:04.000000 h2o-featurestore-1.2.0/h2o_featurestore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2024-01-24 09:13:04.000000 h2o-featurestore-1.2.0/h2o_featurestore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-01-24 09:13:04.000000 h2o-featurestore-1.2.0/h2o_featurestore.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-01-24 09:13:04.600894 h2o-featurestore-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1767 2024-01-23 14:59:38.000000 h2o-featurestore-1.2.0/setup.py
```

### Comparing `h2o-featurestore-1.1.2/README.md` & `h2o-featurestore-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/CoreService_pb2.py` & `h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/CoreService_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ai/h2o/featurestore/api/v1/CoreService.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -21,15 +21,15 @@
 from ai.h2o.featurestore.api.v1 import OnlineApi_pb2 as ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_OnlineApi__pb2
 from ai.h2o.featurestore.api.v1 import TimeToLiveApi_pb2 as ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_TimeToLiveApi__pb2
 from ai.h2o.featurestore.api.v1 import FeatureSetProtoApi_pb2 as ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_FeatureSetProtoApi__pb2
 from ai.h2o.featurestore.api.v1 import RecommendationProtoApi_pb2 as ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_RecommendationProtoApi__pb2
 from ai.h2o.featurestore.api.v1 import DashboardApi_pb2 as ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_DashboardApi__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,ai/h2o/featurestore/api/v1/CoreService.proto\x12\x1a\x61i.h2o.featurestore.api.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x31\x61i/h2o/featurestore/api/v1/FeatureSetSearch.proto\x1a*ai/h2o/featurestore/api/v1/OnlineApi.proto\x1a.ai/h2o/featurestore/api/v1/TimeToLiveApi.proto\x1a\x33\x61i/h2o/featurestore/api/v1/FeatureSetProtoApi.proto\x1a\x37\x61i/h2o/featurestore/api/v1/RecommendationProtoApi.proto\x1a-ai/h2o/featurestore/api/v1/DashboardApi.proto\"\x9c\x01\n\x1dValidatePersonalTokenResponse\x12\x37\n\x04user\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x13\n\x0b\x61uthorities\x18\x02 \x03(\t\x12-\n\texpire_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x9e\x01\n\x19GetUserPermissionsRequest\x12\x13\n\x0bresource_id\x18\x01 \x01(\t\x12\x45\n\x11permission_filter\x18\x02 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\x12\n\npage_token\x18\x04 \x01(\t\"\xb4\x01\n\x1fGetUserActivePermissionsRequest\x12\x13\n\x0bresource_id\x18\x01 \x01(\t\x12\x46\n\x12permission_filters\x18\x02 \x03(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12\r\n\x05query\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\x12\x12\n\npage_token\x18\x05 \x01(\t\"t\n\x1aGetUserPermissionsResponse\x12=\n\x05users\x18\x01 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.UserWithPermission\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x9a\x01\n\x12UserWithPermission\x12\x37\n\x04user\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12K\n\x13resource_permission\x18\x02 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.ResourcePermission\"\x95\x01\n\x12ResourcePermission\x12>\n\npermission\x18\x01 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12?\n\rresource_type\x18\x02 \x01(\x0e\x32(.ai.h2o.featurestore.api.v1.ResourceType\"^\n GetUsersWithoutPermissionRequest\x12\x13\n\x0bresource_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"v\n!GetUsersWithoutPermissionResponse\x12\x38\n\x05users\x18\x01 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"H\n\x1fListPersonalAccessTokensRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\"\x8c\x01\n ListPersonalAccessTokensResponse\x12O\n\x16personal_access_tokens\x18\x01 \x03(\x0b\x32/.ai.h2o.featurestore.api.v1.PersonalAccessToken\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"R\n\x17IdentityProviderDetails\x12\x14\n\x0cidp_meta_url\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t\x12\x0e\n\x06scopes\x18\x03 \x03(\t\"\x9e\x01\n\x14GetWebConfigResponse\x12H\n\x0bipd_details\x18\x01 \x01(\x0b\x32\x33.ai.h2o.featurestore.api.v1.IdentityProviderDetails\x12\x15\n\rapp_store_url\x18\x02 \x01(\t\x12\x0f\n\x07web_url\x18\x03 \x01(\t\x12\x14\n\x0creview_roles\x18\x04 \x03(\t\"d\n-GetFeatureSetsLastMinorForCurrentMajorRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"\x81\x01\n.GetLastMinorFeatureSetForMajorInProjectRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x03 \x01(\x05\"m\n\x17\x46\x65\x61tureSetExistsRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\x12\x17\n\x0f\x65xclude_deleted\x18\x05 \x01(\x08\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x06 \x01(\x05\"N\n\x17GetIngestHistoryRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x03 \x01(\t\"C\n\x14ProjectExistsRequest\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x17\n\x0f\x65xclude_deleted\x18\x03 \x01(\x08\"L\n\x18\x46\x65\x61tureViewExistsRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x04 \x01(\t\x12\x17\n\x0f\x65xclude_deleted\x18\x05 \x01(\x08\"H\n\x16MLDatasetExistsRequest\x12\x15\n\rml_dataset_id\x18\x04 \x01(\t\x12\x17\n\x0f\x65xclude_deleted\x18\x05 \x01(\x08\" \n\x0e\x45xistsResponse\x12\x0e\n\x06\x65xists\x18\x01 \x01(\x08\")\n\x17ProjectsDefaultResponse\x12\x0e\n\x06locked\x18\x01 \x01(\x08\"P\n\x1eHasPermissionToRetrieveRequest\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\"B\n\x1fHasPermissionToRetrieveResponse\x12\x1f\n\x17has_retrieve_permission\x18\x01 \x01(\x08\"e\n\x1bStartRevertIngestJobRequest\x12\x11\n\tingest_id\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x03 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x04 \x01(\t\"e\n\x12OnlineRetrieveMeta\x12\x17\n\x0f\x62\x61se_online_url\x18\x01 \x01(\t\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x12\n\nis_enabled\x18\x04 \x01(\x08\",\n\x13RefreshTokenRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\" \n\x0cTokenRequest\x12\x10\n\x08token_id\x18\x01 \x01(\t\"j\n\x14GenerateTokenRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12/\n\x0b\x65xpiry_date\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"O\n\rTokenResponse\x12>\n\x05token\x18\x01 \x01(\x0b\x32/.ai.h2o.featurestore.api.v1.PersonalAccessToken\"X\n\x10RawTokenResponse\x12\r\n\x05token\x18\x01 \x01(\t\x12\x35\n\x11token_expiry_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"Y\n\x14TokensConfigResponse\x12\x41\n\x1emaximum_allowed_token_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\"p\n\x0fListJobsRequest\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x12\x35\n\x08job_type\x18\x03 \x01(\x0e\x32#.ai.h2o.featurestore.api.v1.JobType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\"A\n\x10ListJobsResponse\x12-\n\x04jobs\x18\x01 \x03(\x0b\x32\x1f.ai.h2o.featurestore.api.v1.Job\"\xc5\x01\n$FeatureSetSchemaCompatibilityRequest\x12\x42\n\x0foriginal_schema\x18\x01 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12=\n\nnew_schema\x18\x02 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12\x1a\n\x12\x63ompare_data_types\x18\x03 \x01(\x08\">\n%FeatureSetSchemaCompatibilityResponse\x12\x15\n\ris_compatible\x18\x01 \x01(\x08\"\xbd\x01\n\x1c\x46\x65\x61tureSetSchemaPatchRequest\x12\x42\n\x0foriginal_schema\x18\x01 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12=\n\nnew_schema\x18\x02 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12\x1a\n\x12\x63ompare_data_types\x18\x03 \x01(\x08\"Z\n\x1d\x46\x65\x61tureSetSchemaPatchResponse\x12\x39\n\x06schema\x18\x01 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\"\x17\n\x05JobId\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"2\n\x18GetRecommendationRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\"\xaf\x02\n\x19GetRecommendationResponse\x12L\n\x07matches\x18\x01 \x03(\x0b\x32;.ai.h2o.featurestore.api.v1.GetRecommendationResponse.Match\x1a+\n\x04Join\x12\x12\n\nclassifier\x18\x01 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\x1a\x96\x01\n\x05Match\x12\x42\n\x12target_feature_set\x18\x01 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\x12I\n\x05joins\x18\x02 \x03(\x0b\x32:.ai.h2o.featurestore.api.v1.GetRecommendationResponse.Join\"\xc3\x02\n\x03Job\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x35\n\x08job_type\x18\x02 \x01(\x0e\x32#.ai.h2o.featurestore.api.v1.JobType\x12\x0c\n\x04\x64one\x18\x03 \x01(\x08\x12\x13\n\x0b\x63hildJobIds\x18\x04 \x03(\t\x12\x11\n\tcancelled\x18\x05 \x01(\x08\x12\x39\n\njob_status\x18\x06 \x01(\x0e\x32%.ai.h2o.featurestore.api.v1.JobStatus\x12=\n\ncreated_by\x18\x07 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12.\n\ncreated_on\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rerror_message\x18\t \x01(\t\"6\n\x10JobProgressInput\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x12\n\nnext_index\x18\x02 \x01(\x05\"\xc6\x01\n\x11JobProgressOutput\x12H\n\x08progress\x18\x01 \x03(\x0b\x32\x36.ai.h2o.featurestore.api.v1.JobProgressOutput.Progress\x1ag\n\x08Progress\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x1b\n\x13\x64uration_in_seconds\x18\x02 \x01(\r\x12-\n\ttimestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8a\x01\n\x1b\x46\x65\x61tureSetPermissionRequest\x12\x13\n\x0buser_emails\x18\x02 \x03(\t\x12>\n\npermission\x18\x03 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\"\x83\x01\n\x18ProjectPermissionRequest\x12\x13\n\x0buser_emails\x18\x02 \x03(\t\x12>\n\npermission\x18\x03 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12\x12\n\nproject_id\x18\x04 \x01(\t\"\xe8\x01\n\x1cStartExtractSchemaJobRequest\x12?\n\x08raw_data\x18\x01 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocationH\x00\x12\x46\n\x0c\x64\x65rived_from\x18\x03 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformationH\x00\x12\x35\n\x04\x63red\x18\x02 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.CredentialsB\x08\n\x06source\"\x98\x01\n\x15\x45xtractSchemaResponse\x12\x39\n\x06schema\x18\x01 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12\x44\n\x0c\x64\x65rived_from\x18\x02 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\"7\n\x1dListFeatureSetsVersionRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\"\x81\x01\n\x12\x46\x65\x61tureSetResponse\x12;\n\x0b\x66\x65\x61ture_set\x18\x01 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\x12.\n\x03job\x18\x02 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.JobId\"_\n\x18UpdateFeatureSetResponse\x12\x43\n\x13updated_feature_set\x18\x01 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\"U\n\x15UpdateProjectResponse\x12<\n\x0fupdated_project\x18\x02 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\"\x9a\x01\n\x15UpdateFeatureResponse\x12\x43\n\x13updated_feature_set\x18\x01 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\x12<\n\x0fupdated_feature\x18\x02 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\"G\n\x0fProjectResponse\x12\x34\n\x07project\x18\x01 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\"I\n\rLoginResponse\x12\x13\n\tlogin_url\x18\x01 \x01(\tH\x00\x12\x17\n\rrefresh_token\x18\x02 \x01(\tH\x00\x42\n\n\x08response\"d\n\x15GetActiveUserResponse\x12\x37\n\x04user\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x12\n\nuser_roles\x18\x02 \x03(\t\")\n\x11GetProjectRequest\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\"+\n\x15GetProjectByIdRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\"1\n\x17\x44\x65leteFeatureSetRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\"[\n\x1e\x44\x65leteFeatureSetVersionRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x02 \x01(\x05\"&\n\rLogoutRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\"P\n\rUserBasicInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x16\n\x0epreferred_name\x18\x04 \x01(\t\"Y\n\x04User\x12\x42\n\x0fuser_basic_info\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\r\n\x05\x61\x64min\x18\x02 \x01(\x08\"y\n\x13\x41\x63\x63\x65ssTokenResponse\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\x03\x12\r\n\x05scope\x18\x04 \x01(\t\x12\x12\n\ntoken_type\x18\x05 \x01(\t\"*\n\x14\x44\x65leteProjectRequest\x12\x12\n\nproject_id\x18\x02 \x01(\t\"\x8f\x01\n\x14\x43reateProjectRequest\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06secret\x18\x03 \x01(\x08\x12\x0e\n\x06locked\x18\x04 \x01(\x08\x12,\n\x0b\x63ustom_data\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"e\n\x15\x43reateProjectResponse\x12\x34\n\x07project\x18\x01 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\x12\x16\n\x0e\x61lready_exists\x18\x02 \x01(\x08\"M\n\x14ListProjectsResponse\x12\x35\n\x08projects\x18\x01 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\"Z\n\x1dListProjectHistoryPageRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"\xc2\x01\n\x0eProjectHistory\x12\x39\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32).ai.h2o.featurestore.api.v1.ProjectAction\x12?\n\x0cperformed_by\x18\x02 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x34\n\x07project\x18\x03 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\"v\n\x1eListProjectHistoryPageResponse\x12;\n\x07history\x18\x01 \x03(\x0b\x32*.ai.h2o.featurestore.api.v1.ProjectHistory\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"`\n\x18GetIngestHistoryResponse\x12\x44\n\x0eingest_history\x18\x01 \x03(\x0b\x32,.ai.h2o.featurestore.api.v1.FeatureSetIngest\"Z\n\x1aListFeatureSetsPageRequest\x12\x15\n\rproject_names\x18\x01 \x03(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"t\n\x1bListFeatureSetsPageResponse\x12<\n\x0c\x66\x65\x61ture_sets\x18\x01 \x03(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x87\x01\n\x0e\x41WSCredentials\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12\x14\n\x0csecret_token\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x05 \x01(\t\x12\x10\n\x08role_arn\x18\x06 \x01(\t\x12\x15\n\rsession_token\x18\x07 \x01(\t\"\xa6\x01\n\x10\x41zureCredentials\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63\x63ount_key\x18\x02 \x01(\t\x12\x11\n\tsas_token\x18\x03 \x01(\t\x12\x15\n\rsas_container\x18\x04 \x01(\t\x12\x14\n\x0csp_client_id\x18\x05 \x01(\t\x12\x14\n\x0csp_tenant_id\x18\x06 \x01(\t\x12\x11\n\tsp_secret\x18\x07 \x01(\t\"c\n\x14SnowflakeCredentials\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x17\n\x0fpem_private_key\x18\x03 \x01(\t\x12\x12\n\npassphrase\x18\x04 \x01(\t\"1\n\x0fJDBCCredentials\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"4\n\x12MongoDbCredentials\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"\xd4\x02\n\x0b\x43redentials\x12\x37\n\x03\x61ws\x18\x01 \x01(\x0b\x32*.ai.h2o.featurestore.api.v1.AWSCredentials\x12;\n\x05\x61zure\x18\x02 \x01(\x0b\x32,.ai.h2o.featurestore.api.v1.AzureCredentials\x12\x43\n\tsnowflake\x18\x03 \x01(\x0b\x32\x30.ai.h2o.featurestore.api.v1.SnowflakeCredentials\x12\x42\n\rjdbc_database\x18\x04 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.JDBCCredentials\x12@\n\x08mongo_db\x18\x06 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.MongoDbCredentialsJ\x04\x08\x05\x10\x06\"W\n\x17ListFeatureSetsResponse\x12<\n\x0c\x66\x65\x61ture_sets\x18\x01 \x03(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\"l\n\x1eListFeatureSetVersionsResponse\x12J\n\x08versions\x18\x01 \x03(\x0b\x32\x38.ai.h2o.featurestore.api.v1.FeatureSetVersionDescription\"~\n\x1c\x46\x65\x61tureSetVersionDescription\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x16\n\x0eversion_change\x18\x02 \x01(\t\x12\x35\n\x11\x63reated_date_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"U\n\x14GetFeatureSetRequest\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x12\n\nproject_id\x18\x04 \x01(\t\"\xd1\x01\n\x15StartIngestJobRequest\x12\x35\n\x04\x63red\x18\x02 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.Credentials\x12@\n\x0b\x64\x61ta_source\x18\x05 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocation\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x06 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x07 \x01(\tJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05\"\xe3\x02\n\x0eIngestResponse\x12\x43\n\x04meta\x18\x01 \x01(\x0b\x32\x35.ai.h2o.featurestore.api.v1.IngestResponse.IngestMeta\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x03 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x04 \x01(\t\x1a\xd6\x01\n\nIngestMeta\x12\x16\n\x0e\x63\x61\x63he_location\x18\x01 \x01(\t\x12\x1a\n\x12raw_cache_location\x18\x02 \x01(\t\x12\x37\n\x13ingestion_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x0cingest_scope\x18\x04 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x0f\n\x07message\x18\x05 \x01(\t\x12\x11\n\tingest_id\x18\x06 \x01(\t\"\x9d\x01\n\x0fRetrieveRequest\x12\x17\n\x0fstart_date_time\x18\x02 \x01(\t\x12\x15\n\rend_date_time\x18\x03 \x01(\t\x12\x11\n\tingest_id\x18\x04 \x01(\t\x12\x12\n\nsession_id\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x06 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x07 \x01(\t\"\x8b\x01\n\x17RetrieveAsLinksResponse\x12\x16\n\x0e\x64ownload_links\x18\x01 \x03(\t\x12\x39\n\x0eretrieve_scope\x18\x02 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x1d\n\x15retrieve_job_executed\x18\x03 \x01(\x08\"\xe8\x02\n\x17RetrieveAsSparkResponse\x12\x12\n\ncache_path\x18\x01 \x01(\t\x12Q\n\x07options\x18\x02 \x03(\x0b\x32@.ai.h2o.featurestore.api.v1.RetrieveAsSparkResponse.OptionsEntry\x12\x39\n\x0eretrieve_scope\x18\x03 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x12\n\nsession_id\x18\x04 \x01(\t\x12\x15\n\rdelta_version\x18\x05 \x01(\x03\x12P\n\x16offline_storage_format\x18\x06 \x01(\x0e\x32\x30.ai.h2o.featurestore.api.v1.OfflineStorageFormat\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"X\n!StartMaterializationOnlineRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x03 \x01(\t\"v\n\x1dMaterializationOnlineResponse\x12@\n\x15materialization_scope\x18\x01 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x13\n\x0bnum_records\x18\x02 \x01(\x04\"2\n\x1cIngestWriteCredentialRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"\xca\x01\n\x1dIngestWriteCredentialResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\x12W\n\x07options\x18\x02 \x03(\x0b\x32\x46.ai.h2o.featurestore.api.v1.IngestWriteCredentialResponse.OptionsEntry\x12\x12\n\nsession_id\x18\x03 \x01(\t\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9c\x01\n\x1eStartOptimizeStorageJobRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\x12\x45\n\x0coptimization\x18\x03 \x01(\x0b\x32/.ai.h2o.featurestore.api.v1.StorageOptimization\"\xb9\x01\n\x13StorageOptimization\x12M\n\nz_order_by\x18\x01 \x01(\x0b\x32\x37.ai.h2o.featurestore.api.v1.OptimizeStorageZOrderBySpecH\x00\x12I\n\x07\x63ompact\x18\x02 \x01(\x0b\x32\x36.ai.h2o.featurestore.api.v1.OptimizeStorageCompactSpecH\x00\x42\x08\n\x06method\".\n\x1bOptimizeStorageZOrderBySpec\x12\x0f\n\x07\x63olumns\x18\x01 \x03(\t\"\x1c\n\x1aOptimizeStorageCompactSpec\"7\n\x17OptimizeStorageResponse\x12\x1c\n\x14optimization_metrics\x18\x01 \x01(\t\"\xb4\x06\n\x0fRawDataLocation\x12\x36\n\x03\x63sv\x18\x01 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.CSVFileSpecH\x00\x12>\n\x07parquet\x18\x02 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.ParquetFileSpecH\x00\x12\x43\n\tsnowflake\x18\x03 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.SnowflakeTableSpecH\x00\x12\x39\n\x04jdbc\x18\x04 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.JDBCTableSpecH\x00\x12\x38\n\x04json\x18\x07 \x01(\x0b\x32(.ai.h2o.featurestore.api.v1.JSONFileSpecH\x00\x12\x41\n\x0b\x64\x65lta_table\x18\x08 \x01(\x0b\x32*.ai.h2o.featurestore.api.v1.DeltaTableSpecH\x00\x12?\n\ncsv_folder\x18\n \x01(\x0b\x32).ai.h2o.featurestore.api.v1.CSVFolderSpecH\x00\x12G\n\x0eparquet_folder\x18\x0b \x01(\x0b\x32-.ai.h2o.featurestore.api.v1.ParquetFolderSpecH\x00\x12\x41\n\x0bjson_folder\x18\x0c \x01(\x0b\x32*.ai.h2o.featurestore.api.v1.JSONFolderSpecH\x00\x12G\n\x0ctemp_parquet\x18\r \x01(\x0b\x32/.ai.h2o.featurestore.api.v1.TempParquetFileSpecH\x00\x12\x45\n\ronline_source\x18\x0e \x01(\x0b\x32,.ai.h2o.featurestore.api.v1.OnlineSourceSpecH\x00\x12\x45\n\x08mongo_db\x18\x0f \x01(\x0b\x32\x31.ai.h2o.featurestore.api.v1.MongoDbCollectionSpecH\x00\x42\x08\n\x06source\"5\n\x10OnlineSourceSpec\x12!\n\x19\x61\x62solute_json_folder_path\x18\x01 \x01(\t\".\n\x0b\x43SVFileSpec\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tdelimiter\x18\x02 \x01(\t\"/\n\x0cJSONFileSpec\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tmultiline\x18\x02 \x01(\x08\"\x1f\n\x0fParquetFileSpec\x12\x0c\n\x04path\x18\x01 \x01(\t\"#\n\x13TempParquetFileSpec\x12\x0c\n\x04path\x18\x01 \x01(\t\"C\n\x05Proxy\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x0c\n\x04user\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\"\xd7\x01\n\x12SnowflakeTableSpec\x12\r\n\x05table\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\x12\x11\n\twarehouse\x18\x05 \x01(\t\x12\x0e\n\x06schema\x18\x06 \x01(\t\x12\x10\n\x08insecure\x18\x07 \x01(\x08\x12\x30\n\x05proxy\x18\x08 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Proxy\x12\x0c\n\x04role\x18\t \x01(\t\x12\x0f\n\x07\x61\x63\x63ount\x18\n \x01(\t\"\xb5\x01\n\rJDBCTableSpec\x12\r\n\x05table\x18\x01 \x01(\t\x12\r\n\x05query\x18\x02 \x01(\t\x12\x16\n\x0e\x63onnection_url\x18\x03 \x01(\t\x12\x16\n\x0enum_partitions\x18\x04 \x01(\x05\x12\x18\n\x10partition_column\x18\x05 \x01(\t\x12\x13\n\x0blower_bound\x18\x06 \x01(\x04\x12\x13\n\x0bupper_bound\x18\x07 \x01(\x04\x12\x12\n\nfetch_size\x18\x08 \x01(\x05\"v\n\x0e\x44\x65ltaTableSpec\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\x11\n\ttimestamp\x18\x03 \x01(\t\x12\x32\n\x06\x66ilter\x18\x04 \x01(\x0b\x32\".ai.h2o.featurestore.api.v1.Filter\"O\n\rCSVFolderSpec\x12\x13\n\x0broot_folder\x18\x01 \x01(\t\x12\x16\n\x0e\x66ilter_pattern\x18\x02 \x01(\t\x12\x11\n\tdelimiter\x18\x03 \x01(\t\"@\n\x11ParquetFolderSpec\x12\x13\n\x0broot_folder\x18\x01 \x01(\t\x12\x16\n\x0e\x66ilter_pattern\x18\x02 \x01(\t\"P\n\x0eJSONFolderSpec\x12\x13\n\x0broot_folder\x18\x01 \x01(\t\x12\x16\n\x0e\x66ilter_pattern\x18\x02 \x01(\t\x12\x11\n\tmultiline\x18\x03 \x01(\x08\"U\n\x15MongoDbCollectionSpec\x12\x16\n\x0e\x63onnection_uri\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x12\n\ncollection\x18\x03 \x01(\t\"&\n\x12MojoTransformation\x12\x10\n\x08\x66ilename\x18\x03 \x01(\t\"/\n\x1bSparkPipelineTransformation\x12\x10\n\x08\x66ilename\x18\x03 \x01(\t\"r\n\x12JoinTransformation\x12\x10\n\x08left_key\x18\x01 \x01(\t\x12\x11\n\tright_key\x18\x02 \x01(\t\x12\x37\n\tjoin_type\x18\x03 \x01(\x0e\x32$.ai.h2o.featurestore.api.v1.JoinType\"0\n\x0bVersionedId\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rmajor_version\x18\x02 \x01(\r\"\xec\x01\n\x0eTransformation\x12>\n\x04mojo\x18\x02 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.MojoTransformationH\x00\x12Q\n\x0espark_pipeline\x18\x03 \x01(\x0b\x32\x37.ai.h2o.featurestore.api.v1.SparkPipelineTransformationH\x00\x12>\n\x04join\x18\x04 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.JoinTransformationH\x00\x42\x07\n\x05value\"\x9a\x01\n\x12\x44\x65rivedInformation\x12@\n\x0f\x66\x65\x61ture_set_ids\x18\x01 \x03(\x0b\x32\'.ai.h2o.featurestore.api.v1.VersionedId\x12\x42\n\x0etransformation\x18\x02 \x01(\x0b\x32*.ai.h2o.featurestore.api.v1.Transformation\"J\n\x0fSelectedFeature\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12\x0f\n\x07\x66\x65\x61ture\x18\x02 \x01(\t\x12\x16\n\x0etransformation\x18\x03 \x01(\t\"\xa1\x01\n\x14\x46ilterConditionUnion\x12;\n\x06\x66ilter\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureFilterH\x00\x12?\n\x05logic\x18\x02 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.FeatureFilterLogicH\x00\x42\x0b\n\tcondition\"\xa1\x01\n\rFeatureFilter\x12<\n\x07\x66\x65\x61ture\x18\x01 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.SelectedFeature\x12\x43\n\x08operator\x18\x02 \x01(\x0e\x32\x31.ai.h2o.featurestore.api.v1.FeatureFilterOperator\x12\r\n\x05value\x18\x03 \x01(\t\"\xe5\x01\n\x12\x46\x65\x61tureFilterLogic\x12>\n\x04left\x18\x01 \x01(\x0b\x32\x30.ai.h2o.featurestore.api.v1.FilterConditionUnion\x12?\n\x05right\x18\x02 \x01(\x0b\x32\x30.ai.h2o.featurestore.api.v1.FilterConditionUnion\x12N\n\x0elogic_operator\x18\x03 \x01(\x0e\x32\x36.ai.h2o.featurestore.api.v1.FeatureFilterLogicOperator\"\xc8\x05\n\x0c\x46\x65\x61tureQuery\x12\x46\n\x11selected_features\x18\x01 \x03(\x0b\x32+.ai.h2o.featurestore.api.v1.SelectedFeature\x12G\n\x10\x66rom_feature_set\x18\x02 \x01(\x0b\x32-.ai.h2o.featurestore.api.v1.FeatureQuery.From\x12;\n\x04join\x18\x03 \x03(\x0b\x32-.ai.h2o.featurestore.api.v1.FeatureQuery.Join\x12?\n\x05where\x18\x04 \x01(\x0b\x32\x30.ai.h2o.featurestore.api.v1.FilterConditionUnion\x1aS\n\x04\x46rom\x12<\n\x0b\x66\x65\x61ture_set\x18\x01 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.VersionedId\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x1a\xd3\x02\n\x04Join\x12<\n\x0b\x66\x65\x61ture_set\x18\x01 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.VersionedId\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x12<\n\x02on\x18\x03 \x03(\x0b\x32\x30.ai.h2o.featurestore.api.v1.FeatureQuery.Join.On\x12\x43\n\tjoin_type\x18\x04 \x01(\x0e\x32\x30.ai.h2o.featurestore.api.v1.FeatureQueryJoinType\x1a{\n\x02On\x12\x39\n\x04left\x18\x01 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.SelectedFeature\x12:\n\x05right\x18\x02 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.SelectedFeature\"\x9a\x01\n\x0b\x46\x65\x61tureView\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x12\n\nproject_id\x18\x05 \x01(\t\x12\x37\n\x05query\x18\x06 \x01(\x0b\x32(.ai.h2o.featurestore.api.v1.FeatureQuery\"\x8a\x01\n\x18\x43reateFeatureViewRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x12\n\nproject_id\x18\x03 \x01(\t\x12\x37\n\x05query\x18\x04 \x01(\x0b\x32(.ai.h2o.featurestore.api.v1.FeatureQuery\"f\n\x18UpdateFeatureViewRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\"\x94\x01\n\"CreateFeatureViewNewVersionRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\x12\x37\n\x05query\x18\x03 \x01(\x0b\x32(.ai.h2o.featurestore.api.v1.FeatureQuery\"J\n\x15GetFeatureViewRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\"T\n\x13\x46\x65\x61tureViewResponse\x12=\n\x0c\x66\x65\x61ture_view\x18\x01 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.FeatureView\"-\n\x17ListFeatureViewsRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\"Z\n\x18ListFeatureViewsResponse\x12>\n\rfeature_views\x18\x01 \x03(\x0b\x32\'.ai.h2o.featurestore.api.v1.FeatureView\"\xc8\x01\n!RetrieveFeatureViewAsSparkRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\x12,\n\x08start_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x65nd_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nsession_id\x18\x05 \x01(\t\"\xa6\x02\n\"RetrieveFeatureViewAsSparkResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\\\n\x07options\x18\x02 \x03(\x0b\x32K.ai.h2o.featurestore.api.v1.RetrieveFeatureViewAsSparkResponse.OptionsEntry\x12\x12\n\nsession_id\x18\x04 \x01(\t\x12P\n\x16offline_storage_format\x18\x05 \x01(\x0e\x32\x30.ai.h2o.featurestore.api.v1.OfflineStorageFormat\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb6\x01\n#RetrieveFeatureViewAsAsLinksRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\x12,\n\x08start_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x65nd_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\">\n$RetrieveFeatureViewAsAsLinksResponse\x12\x16\n\x0e\x64ownload_links\x18\x01 \x03(\t\"3\n\x18\x44\x65leteFeatureViewRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\"\x8f\x03\n\x10MLDatasetFeature\x12\x12\n\nfeature_id\x18\x01 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x03 \x01(\x05\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x04 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x05 \x01(\x05\x12\x11\n\tdata_type\x18\x06 \x01(\t\x12=\n\x0c\x66\x65\x61ture_type\x18\x07 \x01(\x0e\x32\'.ai.h2o.featurestore.api.v1.FeatureType\x12\x15\n\rml_dataset_id\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12\x15\n\roriginal_name\x18\n \x01(\t\x12\x12\n\nproject_id\x18\x0b \x01(\t\x12\x1a\n\x12original_data_type\x18\x0c \x01(\t\x12\x1f\n\x17transformation_function\x18\r \x01(\t\x12\x16\n\x0eis_primary_key\x18\x0e \x01(\x08\"\xf6\x03\n\tMLDataset\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x33\n\x0fstart_date_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_date_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x06 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x07 \x01(\x05\x12\x12\n\nproject_id\x18\x08 \x01(\t\x12>\n\x08\x66\x65\x61tures\x18\t \x03(\x0b\x32,.ai.h2o.featurestore.api.v1.MLDatasetFeature\x12\x43\n\x05state\x18\n \x01(\x0e\x32\x34.ai.h2o.featurestore.api.v1.MLDataset.MLDatasetState\x12\x14\n\x0cprimary_keys\x18\x0b \x03(\t\"l\n\x0eMLDatasetState\x12\x1c\n\x18ML_DATASET_STATE_UNKNOWN\x10\x00\x12\x1c\n\x18ML_DATASET_STATE_PENDING\x10\x01\x12\x1e\n\x1aML_DATASET_STATE_AVAILABLE\x10\x02\"\xda\x01\n\x16\x43reateMLDatasetRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x33\n\x0fstart_date_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_date_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x16UpdateMLDatasetRequest\x12\x15\n\rml_dataset_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"/\n\x16\x44\x65leteMLDatasetRequest\x12\x15\n\rml_dataset_id\x18\x01 \x01(\t\"\x84\x01\n\x17\x43reateMLDatasetResponse\x12\x39\n\nml_dataset\x18\x01 \x01(\x0b\x32%.ai.h2o.featurestore.api.v1.MLDataset\x12.\n\x03job\x18\x02 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.JobId\"e\n\x13GetMLDatasetRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\x12\x17\n\x0fml_dataset_name\x18\x03 \x01(\t\"N\n\x15ListMLDatasetsRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\"T\n\x16ListMLDatasetsResponse\x12:\n\x0bml_datasets\x18\x01 \x03(\x0b\x32%.ai.h2o.featurestore.api.v1.MLDataset\"L\n\x1fRetrieveMLDatasetAsSparkRequest\x12\x15\n\rml_dataset_id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\"\xa2\x02\n RetrieveMLDatasetAsSparkResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\x12Z\n\x07options\x18\x02 \x03(\x0b\x32I.ai.h2o.featurestore.api.v1.RetrieveMLDatasetAsSparkResponse.OptionsEntry\x12\x12\n\nsession_id\x18\x04 \x01(\t\x12P\n\x16offline_storage_format\x18\x05 \x01(\x0e\x32\x30.ai.h2o.featurestore.api.v1.OfflineStorageFormat\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\":\n!RetrieveMLDatasetAsAsLinksRequest\x12\x15\n\rml_dataset_id\x18\x01 \x01(\t\"<\n\"RetrieveMLDatasetAsAsLinksResponse\x12\x16\n\x0e\x64ownload_links\x18\x01 \x03(\t\"\xbd\x0f\n\nFeatureSet\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x16\n\x0eversion_change\x18\x05 \x01(\t\x12\x1a\n\x12time_travel_column\x18\x06 \x01(\t\x12!\n\x19time_travel_column_format\x18\x07 \x01(\t\x12\x44\n\x10\x66\x65\x61ture_set_type\x18\x08 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.FeatureSetType\x12\x13\n\x0b\x64\x65scription\x18\t \x01(\t\x12\x39\n\x06\x61uthor\x18\x0b \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x35\n\x11\x63reated_date_time\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15last_update_date_time\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x61pplication_name\x18\x0e \x01(\t\x12\x12\n\ndeprecated\x18\x0f \x01(\x08\x12\x33\n\x0f\x64\x65precated_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13\x64\x61ta_source_domains\x18\x11 \x03(\t\x12\x0c\n\x04tags\x18\x12 \x03(\t\x12\x18\n\x10process_interval\x18\x13 \x01(\r\x12N\n\x15process_interval_unit\x18\x14 \x01(\x0e\x32/.ai.h2o.featurestore.api.v1.ProcessIntervalUnit\x12\x0c\n\x04\x66low\x18\x15 \x01(\t\x12<\n\x0ctime_to_live\x18\x16 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.TimeToLive\x12\x35\n\x08\x66\x65\x61tures\x18\x17 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\x12\x45\n\nstatistics\x18\x18 \x01(\x0b\x32\x31.ai.h2o.featurestore.api.v1.FeatureSet.Statistics\x12H\n\x0cspecial_data\x18\x19 \x01(\x0b\x32\x32.ai.h2o.featurestore.api.v1.FeatureSet.SpecialData\x12\x13\n\x0bprimary_key\x18\x1a \x03(\t\x12\n\n\x02id\x18\x1c \x01(\t\x12<\n\x11time_travel_scope\x18\x1d \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x16\n\x0e\x61pplication_id\x18\x1e \x01(\t\x12\x19\n\x11\x66\x65\x61ture_set_state\x18\x1f \x01(\t\x12=\n\x06online\x18  \x01(\x0b\x32-.ai.h2o.featurestore.api.v1.FeatureSet.Online\x12\x0e\n\x06secret\x18! \x01(\x08\x12\x12\n\nproject_id\x18\" \x01(\t\x12\x14\n\x0cpartition_by\x18# \x03(\t\x12,\n\x0b\x63ustom_data\x18$ \x01(\x0b\x32\x17.google.protobuf.Struct\x12G\n\x1conline_materialization_scope\x18% \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x44\n\x0c\x64\x65rived_from\x18& \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\x12\x1b\n\x13\x66\x65\x61ture_classifiers\x18\' \x03(\t\x12\x42\n\x0flast_updated_by\x18( \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12M\n\x14storage_optimization\x18) \x01(\x0b\x32/.ai.h2o.featurestore.api.v1.StorageOptimization\x1a\x39\n\nStatistics\x12\x14\n\x0c\x64\x61ta_latency\x18\x01 \x01(\x05\x12\x15\n\rrecords_count\x18\x02 \x01(\x03\x1a\x82\x02\n\x0bSpecialData\x12\x0b\n\x03spi\x18\x01 \x01(\x08\x12\x0b\n\x03pci\x18\x02 \x01(\x08\x12\x0b\n\x03rpi\x18\x03 \x01(\x08\x12\x13\n\x0b\x64\x65mographic\x18\x04 \x01(\x08\x12\x11\n\tsensitive\x18\x05 \x01(\x08\x12G\n\x05legal\x18\x06 \x01(\x0b\x32\x38.ai.h2o.featurestore.api.v1.FeatureSet.SpecialData.Legal\x1a[\n\x05Legal\x12\x10\n\x08\x61pproved\x18\x01 \x01(\x08\x12\x31\n\rapproved_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05notes\x18\x03 \x01(\t\x1aJ\n\x06Online\x12\x18\n\x10online_namespace\x18\x01 \x01(\t\x12\x17\n\x0f\x63onnection_type\x18\x02 \x01(\t\x12\r\n\x05topic\x18\x03 \x01(\tJ\x04\x08\n\x10\x0b\"R\n\x1bGetFeatureSetPreviewRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"I\n\x1cGetFeatureSetPreviewResponse\x12\x13\n\x0bpreview_url\x18\x01 \x01(\t\x12\x14\n\x0cmax_cols_num\x18\x02 \x01(\r\"o\n\x05Scope\x12\x33\n\x0fstart_date_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_date_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xcf\x07\n\x19RegisterFeatureSetRequest\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x01 \x01(\t\x12\x34\n\x07project\x18\x02 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\x12\x1a\n\x12time_travel_column\x18\x03 \x01(\t\x12!\n\x19time_travel_column_format\x18\x04 \x01(\t\x12\x13\n\x0bprimary_key\x18\x05 \x03(\t\x12\x39\n\x06schema\x18\x07 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12\x0e\n\x06secret\x18\x08 \x01(\x08\x12\x13\n\x0b\x64\x65scription\x18\t \x01(\t\x12\x14\n\x0cpartition_by\x18\n \x03(\t\x12\'\n\x1ftime_travel_column_as_partition\x18\x0b \x01(\x08\x12\x44\n\x10\x66\x65\x61ture_set_type\x18\x0c \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.FeatureSetType\x12\x19\n\x11\x66\x65\x61ture_set_state\x18\r \x01(\t\x12\x18\n\x10\x61pplication_name\x18\x0e \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x0f \x01(\t\x12=\n\x06online\x18\x10 \x01(\x0b\x32-.ai.h2o.featurestore.api.v1.FeatureSet.Online\x12\x1b\n\x13\x64\x61ta_source_domains\x18\x11 \x03(\t\x12\x0c\n\x04tags\x18\x12 \x03(\t\x12\x18\n\x10process_interval\x18\x13 \x01(\r\x12N\n\x15process_interval_unit\x18\x14 \x01(\x0e\x32/.ai.h2o.featurestore.api.v1.ProcessIntervalUnit\x12\x0c\n\x04\x66low\x18\x15 \x01(\t\x12H\n\x0cspecial_data\x18\x16 \x01(\x0b\x32\x32.ai.h2o.featurestore.api.v1.FeatureSet.SpecialData\x12,\n\x0b\x63ustom_data\x18\x17 \x01(\x0b\x32\x17.google.protobuf.Struct\x12<\n\x0ctime_to_live\x18\x18 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.TimeToLive\x12\x44\n\x0c\x64\x65rived_from\x18\x19 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\"\xb4\x05\n!CreateNewFeatureSetVersionRequest\x12\x39\n\x06schema\x18\x02 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12\x19\n\x11\x61\x66\x66\x65\x63ted_features\x18\x03 \x03(\t\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x44\n\x0c\x64\x65rived_from\x18\x05 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\x12\x13\n\x0bprimary_key\x18\x06 \x03(\t\x12-\n%use_primary_key_from_previous_version\x18\x07 \x01(\x08\x12\x45\n\x10\x62\x61\x63kfill_options\x18\x08 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.BackfillOptions\x12\x14\n\x0cpartition_by\x18\t \x03(\t\x12.\n&use_partition_by_from_previous_version\x18\n \x01(\x08\x12+\n#use_time_travel_column_as_partition\x18\x0b \x01(\x08\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x0c \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\r \x01(\t\x12\x1a\n\x12time_travel_column\x18\x0e \x01(\t\x12!\n\x19time_travel_column_format\x18\x0f \x01(\t\x12\x34\n,use_time_travel_column_from_previous_version\x18\x10 \x01(\x08\x12;\n3use_time_travel_column_format_from_previous_version\x18\x11 \x01(\x08\"\xff\x01\n\x0e\x46\x65\x61tureProfile\x12=\n\x0c\x66\x65\x61ture_type\x18\x01 \x01(\x0e\x32\'.ai.h2o.featurestore.api.v1.FeatureType\x12M\n\x0b\x63\x61tegorical\x18\x02 \x01(\x0b\x32\x38.ai.h2o.featurestore.api.v1.CategoricalFeatureStatistics\x12\x41\n\nstatistics\x18\x03 \x01(\x0b\x32-.ai.h2o.featurestore.api.v1.FeatureStatistics\x12\x1c\n\x14statistics_available\x18\x04 \x01(\x08\"\xa0\x04\n\rFeatureSchema\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tdata_type\x18\x02 \x01(\t\x12\x39\n\x06nested\x18\x03 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12K\n\x0cspecial_data\x18\x04 \x01(\x0b\x32\x35.ai.h2o.featurestore.api.v1.FeatureSchema.SpecialData\x12=\n\x0c\x66\x65\x61ture_type\x18\x05 \x01(\x0e\x32\'.ai.h2o.featurestore.api.v1.FeatureType\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x13\n\x0b\x63lassifiers\x18\x07 \x03(\t\x12,\n\x0b\x63ustom_data\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12H\n\nmonitoring\x18\t \x01(\x0b\x32\x34.ai.h2o.featurestore.api.v1.FeatureSchema.Monitoring\x1a\\\n\x0bSpecialData\x12\x0b\n\x03spi\x18\x01 \x01(\x08\x12\x0b\n\x03pci\x18\x02 \x01(\x08\x12\x0b\n\x03rpi\x18\x03 \x01(\x08\x12\x13\n\x0b\x64\x65mographic\x18\x04 \x01(\x08\x12\x11\n\tsensitive\x18\x05 \x01(\x08\x1a\'\n\nMonitoring\x12\x19\n\x11\x61nomaly_detection\x18\x01 \x01(\x08\"\x91\x05\n\x07\x46\x65\x61ture\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x16\n\x0eversion_change\x18\x03 \x01(\t\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x11\n\tdata_type\x18\x05 \x01(\t\x12;\n\x07profile\x18\x06 \x01(\x0b\x32*.ai.h2o.featurestore.api.v1.FeatureProfile\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x12\n\nimportance\x18\x08 \x01(\x01\x12\x0f\n\x07special\x18\t \x01(\t\x12\x42\n\nmonitoring\x18\n \x01(\x0b\x32..ai.h2o.featurestore.api.v1.Feature.Monitoring\x12<\n\x0fnested_features\x18\x0b \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\x12\x45\n\x0cspecial_data\x18\r \x01(\x0b\x32/.ai.h2o.featurestore.api.v1.Feature.SpecialData\x12\x13\n\x0b\x63lassifiers\x18\x0e \x03(\t\x12,\n\x0b\x63ustom_data\x18\x0f \x01(\x0b\x32\x17.google.protobuf.Struct\x12\n\n\x02id\x18\x10 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x11 \x01(\t\x1a\'\n\nMonitoring\x12\x19\n\x11\x61nomaly_detection\x18\x01 \x01(\x08\x1a\\\n\x0bSpecialData\x12\x0b\n\x03spi\x18\x01 \x01(\x08\x12\x0b\n\x03pci\x18\x02 \x01(\x08\x12\x0b\n\x03rpi\x18\x03 \x01(\x08\x12\x13\n\x0b\x64\x65mographic\x18\x04 \x01(\x08\x12\x11\n\tsensitive\x18\x05 \x01(\x08\"\xac\x01\n\x11\x46\x65\x61tureStatistics\x12\x0b\n\x03max\x18\x01 \x01(\x01\x12\x0c\n\x04mean\x18\x02 \x01(\x01\x12\x0e\n\x06median\x18\x03 \x01(\x01\x12\x0b\n\x03min\x18\x04 \x01(\x01\x12\x0e\n\x06stddev\x18\x05 \x01(\x01\x12\x18\n\x10stddev_rec_count\x18\x06 \x01(\x03\x12\x12\n\nnull_count\x18\x07 \x01(\x03\x12\x11\n\tnan_count\x18\x08 \x01(\x03\x12\x0e\n\x06unique\x18\t \x01(\x03\"\xab\x01\n\x1c\x43\x61tegoricalFeatureStatistics\x12\x0e\n\x06unique\x18\x01 \x01(\x03\x12P\n\x03top\x18\x02 \x03(\x0b\x32\x43.ai.h2o.featurestore.api.v1.CategoricalFeatureStatistics.FeatureTop\x1a)\n\nFeatureTop\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\x03\"%\n\x12GetVersionResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"\\\n\x14GetApiConfigResponse\x12 \n\x18public_core_rest_api_url\x18\x01 \x01(\t\x12\"\n\x1apublic_online_rest_api_url\x18\x02 \x01(\t\"\x99\x03\n\x07Project\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x39\n\x06\x61uthor\x18\x04 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x35\n\x11\x63reated_date_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15last_update_date_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06secret\x18\x07 \x01(\x08\x12\x0e\n\x06locked\x18\x08 \x01(\x08\x12\n\n\x02id\x18\t \x01(\t\x12,\n\x0b\x63ustom_data\x18\n \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1a\n\x12\x66\x65\x61ture_sets_count\x18\x0b \x01(\x04\x12\x42\n\x0flast_updated_by\x18\x0c \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfoJ\x04\x08\x03\x10\x04\"\xa4\x02\n\x0fListableProject\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x39\n\x15last_update_date_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06locked\x18\x05 \x01(\x08\x12@\n\npermission\x18\x06 \x01(\x0e\x32,.ai.h2o.featurestore.api.v1.ActivePermission\x12\x39\n\x06\x61uthor\x18\x07 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x1a\n\x12\x66\x65\x61ture_sets_count\x18\x08 \x01(\x04\"\xf6\x02\n\x10\x46\x65\x61tureSetIngest\x12\x11\n\tingest_id\x18\x01 \x01(\t\x12\x34\n\x10ingest_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x06source\x18\x03 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocation\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x05 \x01(\t\x12\x30\n\x05scope\x18\x07 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x16\n\x0eparent_ingests\x18\x08 \x03(\t\x12\x1e\n\x16ingested_records_count\x18\t \x01(\t\x12=\n\nstarted_by\x18\n \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\"\xd7\x01\n\x13PersonalAccessToken\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12-\n\tlast_used\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rcreation_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x65xpiry_date\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x88\x01\n#GenerateTransformationUploadRequest\x12K\n\x13transformation_type\x18\x01 \x01(\x0e\x32..ai.h2o.featurestore.api.v1.TransformationType\x12\x14\n\x0cmd5_checksum\x18\x02 \x01(\t\"\xd5\x01\n$GenerateTransformationUploadResponse\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12^\n\x07headers\x18\x03 \x03(\x0b\x32M.ai.h2o.featurestore.api.v1.GenerateTransformationUploadResponse.HeadersEntry\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"@\n\x17ListProjectsPageRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\"j\n\x18ListProjectsPageResponse\x12\x35\n\x08projects\x18\x01 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xa0\x04\n\x14ProjectSearchRequest\x12\r\n\x05query\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12I\n\x13required_permission\x18\x04 \x01(\x0e\x32,.ai.h2o.featurestore.api.v1.ActivePermission\x12\x13\n\x0bproject_ids\x18\x05 \x03(\t\x12U\n\nsort_field\x18\x06 \x01(\x0e\x32\x41.ai.h2o.featurestore.api.v1.ProjectSearchRequest.ProjectSortField\x12\x41\n\x0esort_direction\x18\x07 \x01(\x0e\x32).ai.h2o.featurestore.api.v1.SortDirection\"\xd7\x01\n\x10ProjectSortField\x12 \n\x1cPROJECT_SORT_FIELD_UNDEFINED\x10\x00\x12\x1b\n\x17PROJECT_SORT_FIELD_NAME\x10\x01\x12\"\n\x1ePROJECT_SORT_FIELD_DESCRIPTION\x10\x02\x12\x1d\n\x19PROJECT_SORT_FIELD_LOCKED\x10\x03\x12\x1d\n\x19PROJECT_SORT_FIELD_AUTHOR\x10\x04\x12\"\n\x1ePROJECT_SORT_FIELD_LAST_UPDATE\x10\x05\"\xd6\x04\n\x17\x46\x65\x61tureSetSearchRequest\x12\r\n\x05query\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x12\n\nowned_only\x18\x04 \x01(\x08\x12\x13\n\x0bproject_ids\x18\x05 \x03(\t\x12[\n\nsort_field\x18\x06 \x01(\x0e\x32G.ai.h2o.featurestore.api.v1.FeatureSetSearchRequest.FeatureSetSortField\x12\x41\n\x0esort_direction\x18\x07 \x01(\x0e\x32).ai.h2o.featurestore.api.v1.SortDirection\x12\x41\n\x07options\x18\x08 \x03(\x0b\x32\x30.ai.h2o.featurestore.api.v1.AdvancedSearchOption\"\xf8\x01\n\x13\x46\x65\x61tureSetSortField\x12$\n FEATURE_SET_SORT_FIELD_UNDEFINED\x10\x00\x12\x1f\n\x1b\x46\x45\x41TURE_SET_SORT_FIELD_NAME\x10\x01\x12&\n\"FEATURE_SET_SORT_FIELD_DESCRIPTION\x10\x02\x12!\n\x1d\x46\x45\x41TURE_SET_SORT_FIELD_AUTHOR\x10\x03\x12&\n\"FEATURE_SET_SORT_FIELD_LAST_UPDATE\x10\x04\x12\'\n#FEATURE_SET_SORT_FIELD_PROJECT_NAME\x10\x05\"\x86\x03\n\x14\x46\x65\x61tureSearchRequest\x12\r\n\x05query\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x12\n\nowned_only\x18\x04 \x01(\x08\x12\x13\n\x0bproject_ids\x18\x05 \x03(\t\x12U\n\nsort_field\x18\x06 \x01(\x0e\x32\x41.ai.h2o.featurestore.api.v1.FeatureSearchRequest.FeatureSortField\x12\x41\n\x0esort_direction\x18\x07 \x01(\x0e\x32).ai.h2o.featurestore.api.v1.SortDirection\"u\n\x10\x46\x65\x61tureSortField\x12 \n\x1c\x46\x45\x41TURE_SORT_FIELD_UNDEFINED\x10\x00\x12\x1b\n\x17\x46\x45\x41TURE_SORT_FIELD_NAME\x10\x01\x12\"\n\x1e\x46\x45\x41TURE_SORT_FIELD_DESCRIPTION\x10\x02\"v\n\x14ProjectSearchResults\x12\x45\n\x10listable_project\x18\x01 \x03(\x0b\x32+.ai.h2o.featurestore.api.v1.ListableProject\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xfa\x0c\n\x12ListableFeatureSet\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0cproject_name\x18\x04 \x01(\t\x12\x39\n\x15last_update_date_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07version\x18\x06 \x01(\t\x12@\n\npermission\x18\x07 \x01(\x0e\x32,.ai.h2o.featurestore.api.v1.ActivePermission\x12\x12\n\nproject_id\x18\x08 \x01(\t\x12\x16\n\x0eversion_change\x18\t \x01(\t\x12\x1a\n\x12time_travel_column\x18\n \x01(\t\x12!\n\x19time_travel_column_format\x18\x0b \x01(\t\x12\x44\n\x10\x66\x65\x61ture_set_type\x18\x0c \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.FeatureSetType\x12\x39\n\x06\x61uthor\x18\r \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x35\n\x11\x63reated_date_time\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ndeprecated\x18\x0f \x01(\x08\x12\x33\n\x0f\x64\x65precated_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04tags\x18\x11 \x03(\t\x12<\n\x0ctime_to_live\x18\x12 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.TimeToLive\x12H\n\x0cspecial_data\x18\x13 \x01(\x0b\x32\x32.ai.h2o.featurestore.api.v1.FeatureSet.SpecialData\x12\x13\n\x0bprimary_key\x18\x14 \x03(\t\x12<\n\x11time_travel_scope\x18\x15 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x0e\n\x06secret\x18\x16 \x01(\x08\x12\x14\n\x0cpartition_by\x18\x17 \x03(\t\x12G\n\x1conline_materialization_scope\x18\x18 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x44\n\x0c\x64\x65rived_from\x18\x19 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\x12\x1b\n\x13\x66\x65\x61ture_classifiers\x18\x1a \x03(\t\x12\x15\n\rrecords_count\x18\x1b \x01(\x04\x12\x38\n\x04\x66low\x18\x1c \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.FeatureSetFlow\x12\x18\n\x10\x61pplication_name\x18\x1d \x01(\t\x12\x1b\n\x13\x64\x61ta_source_domains\x18\x1e \x03(\t\x12\x18\n\x10process_interval\x18\x1f \x01(\r\x12N\n\x15process_interval_unit\x18  \x01(\x0e\x32/.ai.h2o.featurestore.api.v1.ProcessIntervalUnit\x12\x45\n\nstatistics\x18! \x01(\x0b\x32\x31.ai.h2o.featurestore.api.v1.FeatureSet.Statistics\x12\x16\n\x0e\x61pplication_id\x18\" \x01(\t\x12\x19\n\x11\x66\x65\x61ture_set_state\x18# \x01(\t\x12=\n\x06online\x18$ \x01(\x0b\x32-.ai.h2o.featurestore.api.v1.FeatureSet.Online\x12,\n\x0b\x63ustom_data\x18% \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x42\n\x0flast_updated_by\x18& \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12M\n\x14storage_optimization\x18\' \x01(\x0b\x32/.ai.h2o.featurestore.api.v1.StorageOptimization\"\x80\x01\n\x17\x46\x65\x61tureSetSearchResults\x12L\n\x14listable_feature_set\x18\x01 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.ListableFeatureSet\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xde\x01\n\x0fListableFeature\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x19\n\x11\x61nomaly_detection\x18\x04 \x01(\x08\x12=\n\x0c\x66\x65\x61ture_type\x18\x05 \x01(\x0e\x32\'.ai.h2o.featurestore.api.v1.FeatureType\x12\x11\n\tdata_type\x18\x06 \x01(\t\x12\x0f\n\x07version\x18\x07 \x01(\t\x12\x12\n\nfeature_id\x18\x08 \x01(\t\"v\n\x14\x46\x65\x61tureSearchResults\x12\x45\n\x10listable_feature\x18\x01 \x03(\x0b\x32+.ai.h2o.featurestore.api.v1.ListableFeature\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"J\n\x13\x46\x65\x61tureSetRequestId\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"\\\n\x11GetFeatureRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\x12\x12\n\nfeature_id\x18\x03 \x01(\t\"j\n\x18ListFeaturesPageResponse\x12\x35\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"G\n\x0f\x46\x65\x61tureResponse\x12\x34\n\x07\x66\x65\x61ture\x18\x01 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\"\x80\x01\n\x13ListFeaturesRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x05 \x01(\t\"f\n\x14ListFeaturesResponse\x12\x35\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"P\n\x19ListableFeatureSetRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"j\n\x1aListableFeatureSetResponse\x12L\n\x14listable_feature_set\x18\x01 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.ListableFeatureSet\"Z\n\x1d\x46\x65\x61tureSetsDerivedFromRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x02 \x01(\t\"o\n\x1e\x46\x65\x61tureSetsDerivedFromResponse\x12M\n\x15listable_feature_sets\x18\x01 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.ListableFeatureSet\"\x85\x01\n\x1eSubmitPendingPermissionRequest\x12\x13\n\x0bresource_id\x18\x01 \x01(\t\x12>\n\npermission\x18\x02 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12\x0e\n\x06reason\x18\x03 \x01(\t\"8\n\x1fSubmitPendingPermissionResponse\x12\x15\n\rpermission_id\x18\x01 \x01(\t\"\x96\x01\n\x1aListPermissionsPageRequest\x12<\n\x07\x66ilters\x18\x01 \x03(\x0e\x32+.ai.h2o.featurestore.api.v1.PermissionState\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x13\n\x0bresource_id\x18\x04 \x01(\t\"\x88\x01\n#ListProjectsPermissionsPageResponse\x12H\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x37.ai.h2o.featurestore.api.v1.ListableProjectToPermission\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x8e\x01\n&ListFeatureSetsPermissionsPageResponse\x12K\n\x07\x65ntries\x18\x01 \x03(\x0b\x32:.ai.h2o.featurestore.api.v1.ListableFeatureSetToPermission\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x97\x01\n\x1bListableProjectToPermission\x12<\n\x07project\x18\x01 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.ListableProject\x12:\n\npermission\x18\x02 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.Permission\"\xa1\x01\n\x1eListableFeatureSetToPermission\x12\x43\n\x0b\x66\x65\x61ture_set\x18\x01 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.ListableFeatureSet\x12:\n\npermission\x18\x02 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.Permission\"\xec\x08\n\nPermission\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bresource_id\x18\x02 \x01(\t\x12?\n\rresource_type\x18\x03 \x01(\x0e\x32(.ai.h2o.featurestore.api.v1.ResourceType\x12>\n\npermission\x18\x04 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12\x37\n\x04user\x18\x05 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x17\n\x0f\x63reation_reason\x18\x06 \x01(\t\x12:\n\x05state\x18\x07 \x01(\x0e\x32+.ai.h2o.featurestore.api.v1.PermissionState\x12.\n\ncreated_on\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0elast_update_on\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\n \x01(\x08\x12[\n\x13granted_or_rejected\x18\x0b \x01(\x0b\x32>.ai.h2o.featurestore.api.v1.Permission.GrantedOrRejectedUpdate\x12\x45\n\x07revoked\x18\x0c \x01(\x0b\x32\x34.ai.h2o.featurestore.api.v1.Permission.RevokedUpdate\x12G\n\x08promoted\x18\r \x01(\x0b\x32\x35.ai.h2o.featurestore.api.v1.Permission.PromotedUpdate\x1a\xac\x01\n\x0ePromotedUpdate\x12\x37\n\x04user\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12.\n\nupdated_on\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06reason\x18\x03 \x01(\t\x12!\n\x19replaced_by_permission_id\x18\x04 \x01(\t\x1a\x88\x01\n\rRevokedUpdate\x12\x37\n\x04user\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12.\n\nupdated_on\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06reason\x18\x03 \x01(\t\x1a\x92\x01\n\x17GrantedOrRejectedUpdate\x12\x37\n\x04user\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12.\n\nupdated_on\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06reason\x18\x03 \x01(\t\"@\n\x17RevokePermissionRequest\x12\x15\n\rpermission_id\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"H\n\x1f\x41pprovePendingPermissionRequest\x12\x15\n\rpermission_id\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"G\n\x1eRejectPendingPermissionRequest\x12\x15\n\rpermission_id\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"9\n WithdrawPendingPermissionRequest\x12\x15\n\rpermission_id\x18\x01 \x01(\t\"1\n\x1aGetActivePermissionRequest\x12\x13\n\x0bresource_id\x18\x01 \x01(\t\"\xa0\x01\n\x1bGetActivePermissionResponse\x12@\n\npermission\x18\x01 \x01(\x0e\x32,.ai.h2o.featurestore.api.v1.ActivePermission\x12?\n\rresource_type\x18\x02 \x01(\x0e\x32(.ai.h2o.featurestore.api.v1.ResourceType\"\xcf\x04\n\rScheduledTask\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\x12\x12\n\nproject_id\x18\x05 \x01(\t\x12;\n\x06source\x18\x06 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocation\x12\x10\n\x08schedule\x18\x07 \x01(\t\x12\x31\n\rnext_run_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tlast_exec\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x05owner\x18\n \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x35\n\x11\x63reated_date_time\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15last_update_date_time\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\ttask_type\x18\r \x01(\x0e\x32$.ai.h2o.featurestore.api.v1.TaskType\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x0e \x01(\t\x12\x16\n\x0e\x63ron_time_zone\x18\x0f \x01(\t\x12\x18\n\x10\x61llowed_failures\x18\x10 \x01(\x05\"\xb9\x02\n\x13ScheduleTaskRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x12\n\nproject_id\x18\x04 \x01(\t\x12\x35\n\x04\x63red\x18\x05 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.Credentials\x12;\n\x06source\x18\x06 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocation\x12\x10\n\x08schedule\x18\x07 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x08 \x01(\t\x12\x16\n\x0e\x63ron_time_zone\x18\t \x01(\t\x12\x18\n\x10\x61llowed_failures\x18\n \x01(\x05\"Z\n\x19ListScheduledTasksRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"o\n\x1aListScheduledTasksResponse\x12\x38\n\x05tasks\x18\x01 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.ScheduledTask\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\",\n\x0fScheduledTaskId\x12\x19\n\x11scheduled_task_id\x18\x01 \x01(\t\"P\n\x15ScheduledTaskResponse\x12\x37\n\x04task\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.ScheduledTask\"v\n\x1aScheduledTaskUpdateRequest\x12\x19\n\x11scheduled_task_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x10\n\x08schedule\x18\x03 \x01(\t\x12\x16\n\x0eupdated_fields\x18\x04 \x03(\t\"6\n\x19PauseScheduledTaskRequest\x12\x19\n\x11scheduled_task_id\x18\x01 \x01(\t\"i\n\x1aResumeScheduledTaskRequest\x12\x19\n\x11scheduled_task_id\x18\x01 \x01(\t\x12\x16\n\x0esetup_failures\x18\x02 \x01(\x08\x12\x18\n\x10\x61llowed_failures\x18\x03 \x01(\x05\"H\n\x11LazyIngestRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"G\n\x12LazyIngestResponse\x12\x31\n\x06job_id\x18\x01 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.JobId\"O\n\x18GetLazyIngestTaskRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"f\n\"ListScheduledTaskExecutionsRequest\x12\x19\n\x11scheduled_task_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"\xe9\x01\n\x16ScheduledTaskExecution\x12\x31\n\x06job_id\x18\x01 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.JobId\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x66inished_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x0c\x66inal_status\x18\x04 \x01(\x0e\x32%.ai.h2o.featurestore.api.v1.JobStatus\"\x8d\x01\n#ListScheduledTaskExecutionsResponse\x12M\n\x11\x65xecution_history\x18\x01 \x03(\x0b\x32\x32.ai.h2o.featurestore.api.v1.ScheduledTaskExecution\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"c\n\x16TransformationFunction\x12\x15\n\rfunction_name\x18\x01 \x01(\t\x12\x1d\n\x15supported_input_types\x18\x02 \x03(\t\x12\x13\n\x0boutput_type\x18\x03 \x01(\t\"$\n\"ListTransformationFunctionsRequest\"{\n#ListTransformationFunctionsResponse\x12T\n\x18transformation_functions\x18\x01 \x03(\x0b\x32\x32.ai.h2o.featurestore.api.v1.TransformationFunction\"H\n GetTransformationFunctionRequest\x12$\n\x1ctransformation_function_name\x18\x01 \x01(\t\"x\n!GetTransformationFunctionResponse\x12S\n\x17transformation_function\x18\x01 \x01(\x0b\x32\x32.ai.h2o.featurestore.api.v1.TransformationFunction\"\xda\x01\n\x14UpdateProjectRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x0e\n\x06locked\x18\x02 \x01(\x08\x12\x0e\n\x06secret\x18\x03 \x01(\x08\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12,\n\x0b\x63ustom_data\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12K\n\x10\x66ields_to_update\x18\x06 \x03(\x0e\x32\x31.ai.h2o.featurestore.api.v1.UpdatableProjectField\"\xbc\x07\n\x17UpdateFeatureSetRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\x12\x0c\n\x04tags\x18\x03 \x03(\t\x12\x1b\n\x13\x64\x61ta_source_domains\x18\x04 \x03(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x38\n\x04type\x18\x06 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.FeatureSetType\x12\x12\n\ndeprecated\x18\x07 \x01(\x08\x12\x18\n\x10process_interval\x18\x08 \x01(\x05\x12N\n\x15process_interval_unit\x18\t \x01(\x0e\x32/.ai.h2o.featurestore.api.v1.ProcessIntervalUnit\x12\x0e\n\x06secret\x18\n \x01(\x08\x12%\n\x1dtime_to_live_offline_interval\x18\x0b \x01(\r\x12\x62\n\"time_to_live_offline_interval_unit\x18\x0c \x01(\x0e\x32\x36.ai.h2o.featurestore.api.v1.Offline.TimeToLiveInterval\x12$\n\x1ctime_to_live_online_interval\x18\r \x01(\r\x12`\n!time_to_live_online_interval_unit\x18\x0e \x01(\x0e\x32\x35.ai.h2o.featurestore.api.v1.Online.TimeToLiveInterval\x12\x16\n\x0elegal_approved\x18\x0f \x01(\x08\x12\x1c\n\x14legal_approved_notes\x18\x10 \x01(\t\x12\r\n\x05state\x18\x11 \x01(\t\x12\x0c\n\x04\x66low\x18\x12 \x01(\t\x12\x18\n\x10\x61pplication_name\x18\x13 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x14 \x01(\t\x12,\n\x0b\x63ustom_data\x18\x15 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x18\n\x10online_namespace\x18\x16 \x01(\t\x12\x14\n\x0conline_topic\x18\x17 \x01(\t\x12\x1e\n\x16online_connection_type\x18\x18 \x01(\t\x12N\n\x10\x66ields_to_update\x18\x19 \x03(\x0e\x32\x34.ai.h2o.featurestore.api.v1.UpdatableFeatureSetField\"\x8b\x03\n\x14UpdateFeatureRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\x12\x12\n\nfeature_id\x18\x03 \x01(\t\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x35\n\x04type\x18\x05 \x01(\x0e\x32\'.ai.h2o.featurestore.api.v1.FeatureType\x12\x12\n\nimportance\x18\x06 \x01(\x01\x12,\n\x0b\x63ustom_data\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12\x0f\n\x07special\x18\t \x01(\t\x12\x19\n\x11\x61nomaly_detection\x18\n \x01(\x08\x12\x13\n\x0b\x63lassifiers\x18\x0b \x03(\t\x12K\n\x10\x66ields_to_update\x18\x0c \x03(\x0e\x32\x31.ai.h2o.featurestore.api.v1.UpdatableFeatureField\"\xe5\x02\n\x0f\x42\x61\x63kfillOptions\x12-\n\tfrom_date\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07to_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x66rom_version\x18\x03 \x01(\t\x12O\n\x0espark_pipeline\x18\x04 \x01(\x0b\x32\x37.ai.h2o.featurestore.api.v1.SparkPipelineTransformation\x12X\n\x0f\x66\x65\x61ture_mapping\x18\x05 \x03(\x0b\x32?.ai.h2o.featurestore.api.v1.BackfillOptions.FeatureMappingEntry\x1a\x35\n\x13\x46\x65\x61tureMappingEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"W\n\x10\x42\x61\x63kfillResponse\x12\x43\n\x0fingest_response\x18\x01 \x01(\x0b\x32*.ai.h2o.featurestore.api.v1.IngestResponse\"\xac\x02\n\x16\x46\x65\x61tureSetDraftRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x35\n\x04\x63red\x18\x05 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.Credentials\x12@\n\x0b\x64\x61ta_source\x18\x06 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocation\x12\x0e\n\x06secret\x18\x07 \x01(\x08\x12\x44\n\x0c\x64\x65rived_from\x18\x08 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\"\x84\x02\n\"FeatureSetMajorVersionDraftRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x03 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x04 \x01(\t\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x35\n\x04\x63red\x18\x06 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.Credentials\x12@\n\x0b\x64\x61ta_source\x18\x07 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocation\"\x93\x03\n\x18\x44raftToFeatureSetRequest\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12>\n\x06schema\x18\x05 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.FeatureSchemaDraft\x12\x61\n\x12time_travel_column\x18\x06 \x01(\x0b\x32\x45.ai.h2o.featurestore.api.v1.DraftToFeatureSetRequest.TimeTravelColumn\x12\x0e\n\x06secret\x18\x07 \x01(\x08\x12\x0c\n\x04tags\x18\x08 \x03(\t\x1as\n\x10TimeTravelColumn\x12\x1f\n\x17time_travel_column_name\x18\x01 \x01(\t\x12!\n\x19time_travel_column_format\x18\x02 \x01(\t\x12\x1b\n\x13is_partition_column\x18\x03 \x01(\x08\"\xc6\x02\n+MajorVersionDraftToFeatureSetVersionRequest\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12>\n\x06schema\x18\x03 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.FeatureSchemaDraft\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x45\n\x10\x62\x61\x63kfill_options\x18\x05 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.BackfillOptions\x12+\n#use_time_travel_column_as_partition\x18\x06 \x01(\x08\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x07 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x08 \x01(\t\"3\n\x19\x44raftToFeatureSetResponse\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\"\x8d\x01\n,MajorVersionDraftToFeatureSetVersionResponse\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x0e\n\x06job_id\x18\x02 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x03 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x04 \x01(\t\"\xc9\x03\n\x12\x46\x65\x61tureSchemaDraft\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tdata_type\x18\x02 \x01(\t\x12>\n\x06nested\x18\x03 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.FeatureSchemaDraft\x12P\n\x0cspecial_data\x18\x04 \x01(\x0b\x32:.ai.h2o.featurestore.api.v1.FeatureSchemaDraft.SpecialData\x12=\n\x0c\x66\x65\x61ture_type\x18\x05 \x01(\x0e\x32\'.ai.h2o.featurestore.api.v1.FeatureType\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x19\n\x11\x61nomaly_detection\x18\x07 \x01(\x08\x12\x16\n\x0eis_primary_key\x18\x08 \x01(\x08\x12\x1b\n\x13is_partition_column\x18\t \x01(\x08\x1a\\\n\x0bSpecialData\x12\x0b\n\x03spi\x18\x01 \x01(\x08\x12\x0b\n\x03pci\x18\x02 \x01(\x08\x12\x0b\n\x03rpi\x18\x03 \x01(\x08\x12\x13\n\x0b\x64\x65mographic\x18\x04 \x01(\x08\x12\x11\n\tsensitive\x18\x05 \x01(\x08\"1\n\x11\x46\x65\x61tureSetDraftId\x12\x1c\n\x14\x66\x65\x61ture_set_draft_id\x18\x01 \x01(\x04\"D\n\x1bListFeatureSetDraftsRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\"\xe0\x04\n\x17ListableFeatureSetDraft\x12\x1c\n\x14\x66\x65\x61ture_set_draft_id\x18\x01 \x01(\x04\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0cproject_name\x18\x04 \x01(\t\x12\x38\n\x05owner\x18\x05 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12Y\n\x06status\x18\x06 \x01(\x0e\x32I.ai.h2o.featurestore.api.v1.ListableFeatureSetDraft.FeatureSetDraftStatus\x12\x15\n\rerror_message\x18\x07 \x01(\t\x12\x0e\n\x06job_id\x18\x08 \x01(\t\x12\x33\n\x0f\x65xpiration_date\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\ndraft_type\x18\n \x01(\x0e\x32/.ai.h2o.featurestore.api.v1.FeatureSetDraftType\"\xb7\x01\n\x15\x46\x65\x61tureSetDraftStatus\x12(\n$FEATURE_SET_DRAFT_STATUS_UNSPECIFIED\x10\x00\x12(\n$FEATURE_SET_DRAFT_STATUS_IN_PROGRESS\x10\x01\x12%\n!FEATURE_SET_DRAFT_STATUS_FINISHED\x10\x02\x12#\n\x1f\x46\x45\x41TURE_SET_DRAFT_STATUS_FAILED\x10\x03\"\x94\x03\n\x0f\x46\x65\x61tureSetDraft\x12\x1c\n\x14\x66\x65\x61ture_set_draft_id\x18\x01 \x01(\x04\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12>\n\x06schema\x18\x05 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.FeatureSchemaDraft\x12\x0e\n\x06secret\x18\x06 \x01(\x08\x12\x0c\n\x04tags\x18\x07 \x03(\t\x12\x43\n\ndraft_type\x18\x08 \x01(\x0e\x32/.ai.h2o.featurestore.api.v1.FeatureSetDraftType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\t \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\n \x01(\t\x12\x0e\n\x06reason\x18\x0b \x01(\t\x12\x44\n\x0c\x64\x65rived_from\x18\x0c \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\"|\n\x1cListFeatureSetDraftsResponse\x12\x43\n\x06\x64rafts\x18\x01 \x03(\x0b\x32\x33.ai.h2o.featurestore.api.v1.ListableFeatureSetDraft\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"a\n\x17\x46\x65\x61tureSetDraftResponse\x12\x46\n\x11\x66\x65\x61ture_set_draft\x18\x01 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.FeatureSetDraft\"\xec\x01\n\x08\x41rtifact\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x10\n\x08\x66ilename\x18\x04 \x01(\t\x12\x0b\n\x03url\x18\x05 \x01(\t\x12?\n\rartifact_type\x18\x06 \x01(\x0e\x32(.ai.h2o.featurestore.api.v1.ArtifactType\x12G\n\rupload_status\x18\x07 \x01(\x0e\x32\x30.ai.h2o.featurestore.api.v1.ArtifactUploadStatus\"\xae\x01\n\x18StoreFileArtifactRequest\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x10\n\x08\x66ilename\x18\x04 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x05 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x06 \x01(\r\x12\x14\n\x0cmd5_checksum\x18\x07 \x01(\t\"\xd4\x01\n\x19StoreFileArtifactResponse\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\x12\x10\n\x08\x66ilename\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12S\n\x07headers\x18\x04 \x03(\x0b\x32\x42.ai.h2o.featurestore.api.v1.StoreFileArtifactResponse.HeadersEntry\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\".\n\x17RetrieveArtifactRequest\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\"R\n\x18RetrieveArtifactResponse\x12\x36\n\x08\x61rtifact\x18\x01 \x01(\x0b\x32$.ai.h2o.featurestore.api.v1.Artifact\"y\n\x19UpdateUploadStatusRequest\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\x12G\n\rupload_status\x18\x02 \x01(\x0e\x32\x30.ai.h2o.featurestore.api.v1.ArtifactUploadStatus\",\n\x15\x44\x65leteArtifactRequest\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\"x\n\x14ListArtifactsRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x02 \x01(\r\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\x12\n\npage_token\x18\x04 \x01(\t\"i\n\x15ListArtifactsResponse\x12\x37\n\tartifacts\x18\x01 \x03(\x0b\x32$.ai.h2o.featurestore.api.v1.Artifact\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"~\n\x10StoreLinkRequest\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x05 \x01(\r\"(\n\x11StoreLinkResponse\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\"\xc9\x01\n\x14\x46\x65\x61tureSetPopularity\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1c\n\x14number_of_retrievals\x18\x02 \x01(\x04\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x03 \x01(\t\x12\x1f\n\x17\x66\x65\x61ture_set_description\x18\x04 \x01(\t\x12@\n\npermission\x18\x05 \x01(\x0e\x32,.ai.h2o.featurestore.api.v1.ActivePermission\"g\n\x1d\x46\x65\x61tureSetsPopularityResponse\x12\x46\n\x0c\x66\x65\x61ture_sets\x18\x01 \x03(\x0b\x32\x30.ai.h2o.featurestore.api.v1.FeatureSetPopularity\"\x96\x01\n\x1eListFeatureSetsToReviewRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\x12\x39\n\x07\x66ilters\x18\x03 \x03(\x0e\x32(.ai.h2o.featurestore.api.v1.ReviewStatus\x12\x12\n\nproject_id\x18\x04 \x01(\t\"{\n\x1fListFeatureSetsToReviewResponse\x12?\n\x07\x65ntries\x18\x01 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.FeatureSetToReview\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xb6\x02\n\x12\x46\x65\x61tureSetToReview\x12\x11\n\treview_id\x18\x01 \x01(\x04\x12\x14\n\x0cproject_name\x18\x02 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x03 \x01(\t\x12\x38\n\x05owner\x18\x04 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x06status\x18\x07 \x01(\x0e\x32(.ai.h2o.featurestore.api.v1.ReviewStatus\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x08 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\t \x01(\r\"9\n\x14\x41pproveReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\x12\x0e\n\x06reason\x18\x02 \x01(\t\"8\n\x13RejectReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x98\x01\n ListFeatureSetReviewsPageRequest\x12\x39\n\x07\x66ilters\x18\x01 \x03(\x0e\x32(.ai.h2o.featurestore.api.v1.ReviewStatus\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x12\n\nproject_id\x18\x04 \x01(\t\"\xf8\x02\n\x10\x46\x65\x61tureSetReview\x12\x11\n\treview_id\x18\x01 \x01(\x04\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x03 \x01(\r\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x04 \x01(\t\x12\x14\n\x0cproject_name\x18\x05 \x01(\t\x12\x38\n\x06status\x18\x06 \x01(\x0e\x32(.ai.h2o.featurestore.api.v1.ReviewStatus\x12\x0e\n\x06reason\x18\x07 \x01(\t\x12;\n\x08reviewer\x18\x08 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12/\n\x0breviewed_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ncreated_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"{\n!ListFeatureSetReviewsPageResponse\x12=\n\x07\x65ntries\x18\x01 \x03(\x0b\x32,.ai.h2o.featurestore.api.v1.FeatureSetReview\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"9\n$GetListableFeatureSetToReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"u\n%GetListableFeatureSetToReviewResponse\x12L\n\x14listable_feature_set\x18\x01 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.ListableFeatureSet\"9\n$GetListableFeatureSetInReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"u\n%GetListableFeatureSetInReviewResponse\x12L\n\x14listable_feature_set\x18\x01 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.ListableFeatureSet\"4\n\x1f\x44\x65leteRejectedFeatureSetRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"f\n\x1bListFeaturesToReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\"n\n\x1cListFeaturesToReviewResponse\x12\x35\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"f\n\x1bListFeaturesInReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\"n\n\x1cListFeaturesInReviewResponse\x12\x35\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"8\n#GetFeatureSetPreviewToReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"Q\n$GetFeatureSetPreviewToReviewResponse\x12\x13\n\x0bpreview_url\x18\x01 \x01(\t\x12\x14\n\x0cmax_cols_num\x18\x02 \x01(\r\"8\n#GetFeatureSetPreviewInReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"Q\n$GetFeatureSetPreviewInReviewResponse\x12\x13\n\x0bpreview_url\x18\x01 \x01(\t\x12\x14\n\x0cmax_cols_num\x18\x02 \x01(\r\"1\n\x1cGetFeatureSetToReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"\\\n\x1dGetFeatureSetToReviewResponse\x12;\n\x0b\x66\x65\x61ture_set\x18\x01 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\"1\n\x1cGetFeatureSetInReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"\\\n\x1dGetFeatureSetInReviewResponse\x12;\n\x0b\x66\x65\x61ture_set\x18\x01 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\"\xc0\x01\n\x13RecentlyUsedProject\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x14\n\x0cproject_name\x18\x02 \x01(\t\x12\x1b\n\x13project_description\x18\x03 \x01(\t\x12.\n\nupdated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0elast_access_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"a\n\x1cRecentlyUsedProjectsResponse\x12\x41\n\x08projects\x18\x01 \x03(\x0b\x32/.ai.h2o.featurestore.api.v1.RecentlyUsedProject\"\xcf\x01\n\x16RecentlyUsedFeatureSet\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x1f\n\x17\x66\x65\x61ture_set_description\x18\x03 \x01(\t\x12.\n\nupdated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0elast_access_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"k\n\x1fRecentlyUsedFeatureSetsResponse\x12H\n\x0c\x66\x65\x61ture_sets\x18\x01 \x03(\x0b\x32\x32.ai.h2o.featurestore.api.v1.RecentlyUsedFeatureSet\"_\n\x14TargetFeatureRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\x12\x12\n\nfeature_id\x18\x03 \x01(\t\"P\n\x19ListTargetFeaturesRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"B\n\x16TargetFeatureReference\x12\x12\n\nfeature_id\x18\x01 \x01(\t\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x02 \x01(\t\"b\n\x1aListTargetFeaturesResponse\x12\x44\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x32.ai.h2o.featurestore.api.v1.TargetFeatureReference\"\x80\x02\n#ListJobsPageByFeatureSetNameRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\x12\x41\n\rstatus_filter\x18\x03 \x01(\x0e\x32%.ai.h2o.featurestore.api.v1.JobStatusH\x00\x88\x01\x01\x12\x1e\n\x16\x66\x65\x61ture_set_name_query\x18\x04 \x01(\t\x12=\n\x10job_type_filters\x18\x05 \x03(\x0e\x32#.ai.h2o.featurestore.api.v1.JobTypeB\x10\n\x0e_status_filter\"\xf6\x01\n!ListJobsPageByFeatureSetIdRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\x12\x41\n\rstatus_filter\x18\x03 \x01(\x0e\x32%.ai.h2o.featurestore.api.v1.JobStatusH\x00\x88\x01\x01\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\x12=\n\x10job_type_filters\x18\x05 \x03(\x0e\x32#.ai.h2o.featurestore.api.v1.JobTypeB\x10\n\x0e_status_filter\"m\n\x18\x46\x65\x61tureSetJobRelatedInfo\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x1f\n\x17\x66\x65\x61ture_set_description\x18\x03 \x01(\t\"\xe0\x01\n\x0bListableJob\x12R\n\x14\x66\x65\x61ture_set_job_info\x18\x01 \x01(\x0b\x32\x34.ai.h2o.featurestore.api.v1.FeatureSetJobRelatedInfo\x12,\n\x03job\x18\x02 \x01(\x0b\x32\x1f.ai.h2o.featurestore.api.v1.Job\x12;\n\nchild_jobs\x18\x03 \x03(\x0b\x32\'.ai.h2o.featurestore.api.v1.ListableJob\x12\x12\n\nis_derived\x18\x04 \x01(\x08\"i\n\x14ListJobsPageResponse\x12\x38\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\'.ai.h2o.featurestore.api.v1.ListableJob\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"]\n\x1dGetJobsWithStatusCountRequest\x12<\n\rstatus_filter\x18\x01 \x01(\x0e\x32%.ai.h2o.featurestore.api.v1.JobStatus\"4\n\x1eGetJobsWithStatusCountResponse\x12\x12\n\njobs_count\x18\x01 \x01(\r\".\n\x14PinFeatureSetRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\"0\n\x16UnpinFeatureSetRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\"A\n\x18PinnedFeatureSetsRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\"\xd8\x01\n\x10PinnedFeatureSet\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x1f\n\x17\x66\x65\x61ture_set_description\x18\x03 \x01(\t\x12.\n\nupdated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tpinned_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nuser_order\x18\x06 \x01(\x03\"x\n\x19PinnedFeatureSetsResponse\x12\x42\n\x0c\x66\x65\x61ture_sets\x18\x01 \x03(\x0b\x32,.ai.h2o.featurestore.api.v1.PinnedFeatureSet\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"3\n\x19IsFeatureSetPinnedRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\",\n\x1aIsFeatureSetPinnedResponse\x12\x0e\n\x06pinned\x18\x01 \x01(\x08\"Q\n\x14\x43odeSnippedIdRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x02 \x01(\r\",\n\x15\x43odeSnippedIdResponse\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\"\xd0\x03\n\x14\x41\x64vancedSearchOption\x12X\n\x0fsearch_operator\x18\x01 \x01(\x0e\x32?.ai.h2o.featurestore.api.v1.AdvancedSearchOption.SearchOperator\x12R\n\x0csearch_field\x18\x02 \x01(\x0e\x32<.ai.h2o.featurestore.api.v1.AdvancedSearchOption.SearchField\x12\x14\n\x0csearch_value\x18\x03 \x01(\t\"c\n\x0eSearchOperator\x12\x1f\n\x1bSEARCH_OPERATOR_UNSPECIFIED\x10\x00\x12\x18\n\x14SEARCH_OPERATOR_LIKE\x10\x01\x12\x16\n\x12SEARCH_OPERATOR_EQ\x10\x02\"\x8e\x01\n\x0bSearchField\x12\x1c\n\x18SEARCH_FIELD_UNSPECIFIED\x10\x00\x12\x1d\n\x19SEARCH_FIELD_FEATURE_NAME\x10\x01\x12$\n SEARCH_FIELD_FEATURE_DESCRIPTION\x10\x02\x12\x1c\n\x18SEARCH_FIELD_FEATURE_TAG\x10\x03*\xbc\x02\n\x07JobType\x12\x0b\n\x07Unknown\x10\x00\x12\n\n\x06Ingest\x10\x01\x12\x0c\n\x08Retrieve\x10\x02\x12\x11\n\rExtractSchema\x10\x03\x12\x15\n\x11\x43omputeStatistics\x10\x05\x12\n\n\x06Revert\x10\x06\x12\x19\n\x15MaterializationOnline\x10\x07\x12$\n ComputeRecommendationClassifiers\x10\x08\x12\x13\n\x0f\x43reateMLDataset\x10\t\x12\x1e\n\x1a\x46\x65\x61tureViewRetrieveAsLinks\x10\n\x12\x1e\n\x1a\x46\x65\x61tureViewRetrieveAsSpark\x10\x0b\x12\x0c\n\x08\x42\x61\x63kfill\x10\x0c\x12\x15\n\x11RetrieveMLDataset\x10\r\x12\x13\n\x0fOptimizeStorage\x10\x0e\"\x04\x08\x04\x10\x04*X\n\x0ePermissionType\x12\t\n\x05Owner\x10\x00\x12\n\n\x06\x45\x64itor\x10\x01\x12\x0c\n\x08\x43onsumer\x10\x02\x12\x15\n\x11SensitiveConsumer\x10\x03\x12\n\n\x06Viewer\x10\x04*\xd1\x01\n\x10\x41\x63tivePermission\x12\x1a\n\x16\x41\x43TIVE_PERMISSION_NONE\x10\x00\x12\x1b\n\x17\x41\x43TIVE_PERMISSION_OWNER\x10\x01\x12\x1c\n\x18\x41\x43TIVE_PERMISSION_EDITOR\x10\x02\x12\x1e\n\x1a\x41\x43TIVE_PERMISSION_CONSUMER\x10\x03\x12(\n$ACTIVE_PERMISSION_SENSITIVE_CONSUMER\x10\x04\x12\x1c\n\x18\x41\x43TIVE_PERMISSION_VIEWER\x10\x05*9\n\rProjectAction\x12\x13\n\x0fPROJECT_CREATED\x10\x00\x12\x13\n\x0fPROJECT_UPDATED\x10\x01*^\n\x14OfflineStorageFormat\x12 \n\x1cOFFLINE_STORAGE_FORMAT_DELTA\x10\x00\x12$\n OFFLINE_STORAGE_FORMAT_SNOWFLAKE\x10\x01*q\n\x08JoinType\x12\x13\n\x0fJOIN_TYPE_INNER\x10\x00\x12\x12\n\x0eJOIN_TYPE_LEFT\x10\x01\x12\x13\n\x0fJOIN_TYPE_RIGHT\x10\x02\x12\x12\n\x0eJOIN_TYPE_FULL\x10\x03\x12\x13\n\x0fJOIN_TYPE_CROSS\x10\x04*\xfc\x01\n\x15\x46\x65\x61tureFilterOperator\x12#\n\x1f\x46\x45\x41TURE_FILTER_OPERATOR_UNKNOWN\x10\x00\x12\x1e\n\x1a\x46\x45\x41TURE_FILTER_OPERATOR_EQ\x10\x01\x12\x1e\n\x1a\x46\x45\x41TURE_FILTER_OPERATOR_LT\x10\x02\x12\x1e\n\x1a\x46\x45\x41TURE_FILTER_OPERATOR_LE\x10\x03\x12\x1e\n\x1a\x46\x45\x41TURE_FILTER_OPERATOR_GT\x10\x04\x12\x1e\n\x1a\x46\x45\x41TURE_FILTER_OPERATOR_GE\x10\x05\x12\x1e\n\x1a\x46\x45\x41TURE_FILTER_OPERATOR_NE\x10\x06*\x94\x01\n\x1a\x46\x65\x61tureFilterLogicOperator\x12)\n%FEATURE_FILTER_LOGIC_OPERATOR_UNKNOWN\x10\x00\x12%\n!FEATURE_FILTER_LOGIC_OPERATOR_AND\x10\x01\x12$\n FEATURE_FILTER_LOGIC_OPERATOR_OR\x10\x02*Q\n\x14\x46\x65\x61tureQueryJoinType\x12\x1c\n\x18\x46\x45\x41TURE_QUERY_JOIN_INNER\x10\x00\x12\x1b\n\x17\x46\x45\x41TURE_QUERY_JOIN_LEFT\x10\x01*\x96\x01\n\x0f\x46\x65\x61tureDataType\x12\x0b\n\x07TinyInt\x10\x00\x12\x0c\n\x08SmallInt\x10\x01\x12\n\n\x06\x42igInt\x10\x02\x12\x07\n\x03Int\x10\x03\x12\t\n\x05\x46loat\x10\x04\x12\n\n\x06\x44ouble\x10\x05\x12\n\n\x06String\x10\x06\x12\n\n\x06\x42inary\x10\x07\x12\x0b\n\x07\x42oolean\x10\x08\x12\x08\n\x04\x44\x61te\x10\t\x12\r\n\tTimestamp\x10\n*q\n\x13ProcessIntervalUnit\x12\r\n\tUNDEFINED\x10\x00\x12\t\n\x05HOURS\x10\x01\x12\n\n\x06MONTHS\x10\x02\x12\x08\n\x04\x44\x41YS\x10\x03\x12\x0b\n\x07MINUTES\x10\x04\x12\x0b\n\x07SECONDS\x10\x05\x12\x10\n\x0cMILLISECONDS\x10\x06*h\n\x12TransformationType\x12\x19\n\x15TransformationUnknown\x10\x00\x12\x16\n\x12TransformationMojo\x10\x01\x12\x1f\n\x1bTransformationSparkPipeline\x10\x02*,\n\rSortDirection\x12\x0c\n\x08SORT_ASC\x10\x00\x12\r\n\tSORT_DESC\x10\x01*,\n\x0cResourceType\x12\x0b\n\x07PROJECT\x10\x00\x12\x0f\n\x0b\x46\x45\x41TURE_SET\x10\x01*T\n\x0fPermissionState\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07GRANTED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02\x12\x0b\n\x07REVOKED\x10\x03\x12\x0c\n\x08PROMOTED\x10\x04*\'\n\x08TaskType\x12\n\n\x06INGEST\x10\x00\x12\x0f\n\x0bLAZY_INGEST\x10\x01*\xae\x01\n\tJobStatus\x12\x0b\n\x07\x43reated\x10\x00\x12\r\n\tSubmitted\x10\x01\x12\x0b\n\x07Running\x10\x02\x12\x14\n\x10SubmissionFailed\x10\x03\x12\n\n\x06\x46\x61iled\x10\x04\x12\x0b\n\x07Success\x10\x06\x12\x0b\n\x07Pending\x10\x07\x12\x10\n\x0cPendingRerun\x10\x08\x12\x0b\n\x07\x46\x61iling\x10\t\x12\x0e\n\nCancelling\x10\n\x12\r\n\tCancelled\x10\x0b*\x8a\x01\n\x15UpdatableProjectField\x12\x17\n\x13PROJECT_UNSPECIFIED\x10\x00\x12\x12\n\x0ePROJECT_LOCKED\x10\x01\x12\x12\n\x0ePROJECT_SECRET\x10\x02\x12\x17\n\x13PROJECT_DESCRIPTION\x10\x03\x12\x17\n\x13PROJECT_CUSTOM_DATA\x10\x04*\xf1\x05\n\x18UpdatableFeatureSetField\x12\x1b\n\x17\x46\x45\x41TURE_SET_UNSPECIFIED\x10\x00\x12\x14\n\x10\x46\x45\x41TURE_SET_TAGS\x10\x01\x12#\n\x1f\x46\x45\x41TURE_SET_DATA_SOURCE_DOMAINS\x10\x02\x12\x1b\n\x17\x46\x45\x41TURE_SET_DESCRIPTION\x10\x03\x12\x14\n\x10\x46\x45\x41TURE_SET_TYPE\x10\x04\x12 \n\x1c\x46\x45\x41TURE_SET_APPLICATION_NAME\x10\x05\x12\x1e\n\x1a\x46\x45\x41TURE_SET_APPLICATION_ID\x10\x06\x12\x1a\n\x16\x46\x45\x41TURE_SET_DEPRECATED\x10\x07\x12 \n\x1c\x46\x45\x41TURE_SET_PROCESS_INTERVAL\x10\x08\x12%\n!FEATURE_SET_PROCESS_INTERVAL_UNIT\x10\t\x12\x14\n\x10\x46\x45\x41TURE_SET_FLOW\x10\n\x12\x15\n\x11\x46\x45\x41TURE_SET_STATE\x10\x0b\x12\x16\n\x12\x46\x45\x41TURE_SET_SECRET\x10\x0c\x12\x1b\n\x17\x46\x45\x41TURE_SET_TTL_OFFLINE\x10\r\x12$\n FEATURE_SET_TTL_OFFLINE_INTERVAL\x10\x0e\x12\x1a\n\x16\x46\x45\x41TURE_SET_TTL_ONLINE\x10\x0f\x12#\n\x1f\x46\x45\x41TURE_SET_TTL_ONLINE_INTERVAL\x10\x10\x12\x1b\n\x17\x46\x45\x41TURE_SET_CUSTOM_DATA\x10\x11\x12+\n\'FEATURE_SET_SPECIAL_DATA_LEGAL_APPROVED\x10\x12\x12(\n$FEATURE_SET_SPECIAL_DATA_LEGAL_NOTES\x10\x13\x12 \n\x1c\x46\x45\x41TURE_SET_ONLINE_NAMESPACE\x10\x14\x12\x1c\n\x18\x46\x45\x41TURE_SET_ONLINE_TOPIC\x10\x15\x12&\n\"FEATURE_SET_ONLINE_CONNECTION_TYPE\x10\x16*\xed\x01\n\x15UpdatableFeatureField\x12\x17\n\x13\x46\x45\x41TURE_UNSPECIFIED\x10\x00\x12\x12\n\x0e\x46\x45\x41TURE_STATUS\x10\x01\x12\x10\n\x0c\x46\x45\x41TURE_TYPE\x10\x02\x12\x16\n\x12\x46\x45\x41TURE_IMPORTANCE\x10\x03\x12\x17\n\x13\x46\x45\x41TURE_CUSTOM_DATA\x10\x04\x12\x17\n\x13\x46\x45\x41TURE_DESCRIPTION\x10\x05\x12\x13\n\x0f\x46\x45\x41TURE_SPECIAL\x10\x06\x12\x1d\n\x19\x46\x45\x41TURE_ANOMALY_DETECTION\x10\x07\x12\x17\n\x13\x46\x45\x41TURE_CLASSIFIERS\x10\x08*\xc4\x01\n\x13\x46\x65\x61tureSetDraftType\x12&\n\"FEATURE_SET_DRAFT_TYPE_UNSPECIFIED\x10\x00\x12%\n!FEATURE_SET_DRAFT_TYPE_CREATE_NEW\x10\x01\x12/\n+FEATURE_SET_DRAFT_TYPE_CREATE_MAJOR_VERSION\x10\x02\x12-\n)FEATURE_SET_DRAFT_TYPE_CREATE_NEW_DERIVED\x10\x03*]\n\x0c\x41rtifactType\x12\x1d\n\x19\x41RTIFACT_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12\x41RTIFACT_TYPE_LINK\x10\x01\x12\x16\n\x12\x41RTIFACT_TYPE_FILE\x10\x02*\xad\x01\n\x14\x41rtifactUploadStatus\x12)\n%ARTIFACT_UPLOAD_STATUS_NOT_APPLICABLE\x10\x00\x12&\n\"ARTIFACT_UPLOAD_STATUS_IN_PROGRESS\x10\x01\x12\x1f\n\x1b\x41RTIFACT_UPLOAD_STATUS_DONE\x10\x02\x12!\n\x1d\x41RTIFACT_UPLOAD_STATUS_FAILED\x10\x03*\x9d\x01\n\x0cReviewStatus\x12\x1d\n\x19REVIEW_STATUS_UNSPECIFIED\x10\x00\x12\x1b\n\x17REVIEW_STATUS_TO_REVIEW\x10\x01\x12\x1a\n\x16REVIEW_STATUS_APPROVED\x10\x02\x12\x1a\n\x16REVIEW_STATUS_REJECTED\x10\x03\x12\x19\n\x15REVIEW_STATUS_CREATED\x10\x04\x32\xc1\xef\x01\n\x0b\x43oreService\x12{\n\x08ListJobs\x12+.ai.h2o.featurestore.api.v1.ListJobsRequest\x1a,.ai.h2o.featurestore.api.v1.ListJobsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/api/v1/jobs\x12k\n\x06GetJob\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x1f.ai.h2o.featurestore.api.v1.Job\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/api/v1/jobs/{job_id}\x12\xa2\x01\n\x0eGetJobProgress\x12,.ai.h2o.featurestore.api.v1.JobProgressInput\x1a-.ai.h2o.featurestore.api.v1.JobProgressOutput\"3\x82\xd3\xe4\x93\x02-\x12+/api/v1/jobs/{job_id}/progress/{next_index}\x12\x65\n\tCancelJob\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x16.google.protobuf.Empty\"\x1d\x82\xd3\xe4\x93\x02\x17*\x15/api/v1/jobs/{job_id}\x12\xb8\x01\n\x1cListJobsPageByFeatureSetName\x12?.ai.h2o.featurestore.api.v1.ListJobsPageByFeatureSetNameRequest\x1a\x30.ai.h2o.featurestore.api.v1.ListJobsPageResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/api/v1/jobs/feature-set/name\x12\xb2\x01\n\x1aListJobsPageByFeatureSetId\x12=.ai.h2o.featurestore.api.v1.ListJobsPageByFeatureSetIdRequest\x1a\x30.ai.h2o.featurestore.api.v1.ListJobsPageResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/api/v1/jobs/feature-set/id\x12\xb5\x01\n\x16GetJobsWithStatusCount\x12\x39.ai.h2o.featurestore.api.v1.GetJobsWithStatusCountRequest\x1a:.ai.h2o.featurestore.api.v1.GetJobsWithStatusCountResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/api/v1/jobs/count-by-status\x12\x9c\x01\n\x15StartExtractSchemaJob\x12\x38.ai.h2o.featurestore.api.v1.StartExtractSchemaJobRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"&\x82\xd3\xe4\x93\x02 \"\x1b/api/v1/jobs/extract-schema:\x01*\x12\xa6\x01\n\x19GetExtractSchemaJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x31.ai.h2o.featurestore.api.v1.ExtractSchemaResponse\"3\x82\xd3\xe4\x93\x02-\x12+/api/v1/jobs/{job_id}/output/extract-schema\x12\x87\x01\n\x0eStartIngestJob\x12\x31.ai.h2o.featurestore.api.v1.StartIngestJobRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x14/api/v1/ingest/start:\x01*\x12\x93\x01\n\x12GetIngestJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a*.ai.h2o.featurestore.api.v1.IngestResponse\".\x82\xd3\xe4\x93\x02(\x12&/api/v1/jobs/{job_id}/output/ingestion\x12\x93\x01\n\x17StartRetrieveAsLinksJob\x12+.ai.h2o.featurestore.api.v1.RetrieveRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"(\x82\xd3\xe4\x93\x02\"\"\x1d/api/v1/feature-sets/retrieve:\x01*\x12\xa5\x01\n\x1bGetRetrieveAsLinksJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x33.ai.h2o.featurestore.api.v1.RetrieveAsLinksResponse\".\x82\xd3\xe4\x93\x02(\x12&/api/v1/feature-sets/retrieve/{job_id}\x12\xa6\x01\n\x0fRetrieveAsSpark\x12+.ai.h2o.featurestore.api.v1.RetrieveRequest\x1a\x33.ai.h2o.featurestore.api.v1.RetrieveAsSparkResponse\"1\x82\xd3\xe4\x93\x02+\"&/api/v1/feature-sets/retrieve/as-spark:\x01*\x12\xc0\x01\n\x19GetIngestWriteCredentials\x12\x38.ai.h2o.featurestore.api.v1.IngestWriteCredentialRequest\x1a\x39.ai.h2o.featurestore.api.v1.IngestWriteCredentialResponse\".\x82\xd3\xe4\x93\x02(\x12&/api/v1/ingest/credential/{session_id}\x12\x94\x01\n\x14StartRevertIngestJob\x12\x37.ai.h2o.featurestore.api.v1.StartRevertIngestJobRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\" \x82\xd3\xe4\x93\x02\x1a\"\x15/api/v1/ingest/revert:\x01*\x12}\n\x18GetRevertIngestJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x16.google.protobuf.Empty\"&\x82\xd3\xe4\x93\x02 \x12\x1e/api/v1/ingest/revert/{job_id}\x12\xe6\x01\n\x17HasPermissionToRetrieve\x12:.ai.h2o.featurestore.api.v1.HasPermissionToRetrieveRequest\x1a;.ai.h2o.featurestore.api.v1.HasPermissionToRetrieveResponse\"R\x82\xd3\xe4\x93\x02L\x12J/api/v1/feature-sets/retrieve/permission/{project_name}/{feature_set_name}\x12\x9c\x01\n\x12RegisterFeatureSet\x12\x35.ai.h2o.featurestore.api.v1.RegisterFeatureSetRequest\x1a..ai.h2o.featurestore.api.v1.FeatureSetResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x14/api/v1/feature-sets:\x01*\x12\xc5\x01\n\x1a\x43reateNewFeatureSetVersion\x12=.ai.h2o.featurestore.api.v1.CreateNewFeatureSetVersionRequest\x1a..ai.h2o.featurestore.api.v1.FeatureSetResponse\"8\x82\xd3\xe4\x93\x02\x32\"-/api/v1/feature-sets/{feature_set_id}/version:\x01*\x12\x80\x01\n\x15GetOnlineRetrieveMeta\x12\x16.google.protobuf.Empty\x1a..ai.h2o.featurestore.api.v1.OnlineRetrieveMeta\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/api/v1/online-retrieve\x12m\n\nGetVersion\x12\x16.google.protobuf.Empty\x1a..ai.h2o.featurestore.api.v1.GetVersionResponse\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/api/v1/version\x12\xb8\x01\n\rGetFeatureSet\x12\x30.ai.h2o.featurestore.api.v1.GetFeatureSetRequest\x1a..ai.h2o.featurestore.api.v1.FeatureSetResponse\"E\x82\xd3\xe4\x93\x02?\x12=/api/v1/projects/{project_id}/feature-sets/{feature_set_name}\x12\xa3\x01\n\x11GetFeatureSetById\x12/.ai.h2o.featurestore.api.v1.FeatureSetRequestId\x1a..ai.h2o.featurestore.api.v1.FeatureSetResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/api/v1/feature-sets/{feature_set_id}\x12\xd7\x01\n&GetFeatureSetsLastMinorForCurrentMajor\x12I.ai.h2o.featurestore.api.v1.GetFeatureSetsLastMinorForCurrentMajorRequest\x1a..ai.h2o.featurestore.api.v1.FeatureSetResponse\"2\x82\xd3\xe4\x93\x02,\x12*/api/v1/feature-sets/{feature_set_id}/last\x12\x8d\x02\n\'GetLastMinorFeatureSetForMajorInProject\x12J.ai.h2o.featurestore.api.v1.GetLastMinorFeatureSetForMajorInProjectRequest\x1a..ai.h2o.featurestore.api.v1.FeatureSetResponse\"f\x82\xd3\xe4\x93\x02`\x12^/api/v1/projects/{project_id}/feature-sets/{feature_set_name}/{feature_set_major_version}/last\x12\xc7\x01\n\x16ListFeatureSetVersions\x12\x39.ai.h2o.featurestore.api.v1.ListFeatureSetsVersionRequest\x1a:.ai.h2o.featurestore.api.v1.ListFeatureSetVersionsResponse\"6\x82\xd3\xe4\x93\x02\x30\x12./api/v1/feature-sets/{feature_set_id}/versions\x12\x8e\x01\n\x10\x44\x65leteFeatureSet\x12\x33.ai.h2o.featurestore.api.v1.DeleteFeatureSetRequest\x1a\x16.google.protobuf.Empty\"-\x82\xd3\xe4\x93\x02\'*%/api/v1/feature-sets/{feature_set_id}\x12\xc1\x01\n\x17\x44\x65leteFeatureSetVersion\x12:.ai.h2o.featurestore.api.v1.DeleteFeatureSetVersionRequest\x1a\x16.google.protobuf.Empty\"R\x82\xd3\xe4\x93\x02L*J/api/v1/feature-sets/{feature_set_id}/versions/{feature_set_major_version}\x12\xa4\x01\n\x13ListFeatureSetsPage\x12\x36.ai.h2o.featurestore.api.v1.ListFeatureSetsPageRequest\x1a\x37.ai.h2o.featurestore.api.v1.ListFeatureSetsPageResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/api/v1/feature-sets\x12\xa9\x01\n\x10\x46\x65\x61tureSetExists\x12\x33.ai.h2o.featurestore.api.v1.FeatureSetExistsRequest\x1a*.ai.h2o.featurestore.api.v1.ExistsResponse\"4\x82\xd3\xe4\x93\x02.\x12,/api/v1/feature-sets/exists/{feature_set_id}\x12\xc4\x01\n\x10GetIngestHistory\x12\x33.ai.h2o.featurestore.api.v1.GetIngestHistoryRequest\x1a\x34.ai.h2o.featurestore.api.v1.GetIngestHistoryResponse\"E\x82\xd3\xe4\x93\x02?\x12=/api/v1/ingest/{feature_set_id}/{feature_set_version}/history\x12\xdf\x01\n\x1cIsFeatureSetSchemaCompatible\x12@.ai.h2o.featurestore.api.v1.FeatureSetSchemaCompatibilityRequest\x1a\x41.ai.h2o.featurestore.api.v1.FeatureSetSchemaCompatibilityResponse\":\x82\xd3\xe4\x93\x02\x34\"//api/v1/feature-sets/features/schema-compatible:\x01*\x12\xc3\x01\n\x15\x46\x65\x61tureSetSchemaPatch\x12\x38.ai.h2o.featurestore.api.v1.FeatureSetSchemaPatchRequest\x1a\x39.ai.h2o.featurestore.api.v1.FeatureSetSchemaPatchResponse\"5\x82\xd3\xe4\x93\x02/\"*/api/v1/feature-sets/features/schema-patch:\x01*\x12\xc0\x01\n\x14GetFeatureSetPreview\x12\x37.ai.h2o.featurestore.api.v1.GetFeatureSetPreviewRequest\x1a\x38.ai.h2o.featurestore.api.v1.GetFeatureSetPreviewResponse\"5\x82\xd3\xe4\x93\x02/\x12-/api/v1/feature-sets/{feature_set_id}/preview\x12\xaf\x01\n\x10UpdateFeatureSet\x12\x33.ai.h2o.featurestore.api.v1.UpdateFeatureSetRequest\x1a\x34.ai.h2o.featurestore.api.v1.UpdateFeatureSetResponse\"0\x82\xd3\xe4\x93\x02*\x1a%/api/v1/feature-sets/{feature_set_id}:\x01*\x12\xa8\x01\n\x17StartOptimizeStorageJob\x12:.ai.h2o.featurestore.api.v1.StartOptimizeStorageJobRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\".\x82\xd3\xe4\x93\x02(\"#/api/v1/jobs/optimize-storage/start:\x01*\x12\xac\x01\n\x1bGetOptimizeStorageJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x33.ai.h2o.featurestore.api.v1.OptimizeStorageResponse\"5\x82\xd3\xe4\x93\x02/\x12-/api/v1/jobs/{job_id}/output/optimize-storage\x12\x9c\x01\n\x11\x43reateFeatureView\x12\x34.ai.h2o.featurestore.api.v1.CreateFeatureViewRequest\x1a/.ai.h2o.featurestore.api.v1.FeatureViewResponse\" \x82\xd3\xe4\x93\x02\x1a\"\x15/api/v1/feature-views:\x01*\x12\xae\x01\n\x11UpdateFeatureView\x12\x34.ai.h2o.featurestore.api.v1.UpdateFeatureViewRequest\x1a/.ai.h2o.featurestore.api.v1.FeatureViewResponse\"2\x82\xd3\xe4\x93\x02,\x1a\'/api/v1/feature-views/{feature_view_id}:\x01*\x12\xb0\x01\n\x0eGetFeatureView\x12\x31.ai.h2o.featurestore.api.v1.GetFeatureViewRequest\x1a/.ai.h2o.featurestore.api.v1.FeatureViewResponse\":\x82\xd3\xe4\x93\x02\x34\x12\x32/api/v1/projects/{project_id}/feature-views/{name}\x12\xad\x01\n\x11\x46\x65\x61tureViewExists\x12\x34.ai.h2o.featurestore.api.v1.FeatureViewExistsRequest\x1a*.ai.h2o.featurestore.api.v1.ExistsResponse\"6\x82\xd3\xe4\x93\x02\x30\x12./api/v1/feature-views/{feature_view_id}/exists\x12\xb2\x01\n\x10ListFeatureViews\x12\x33.ai.h2o.featurestore.api.v1.ListFeatureViewsRequest\x1a\x34.ai.h2o.featurestore.api.v1.ListFeatureViewsResponse\"3\x82\xd3\xe4\x93\x02-\x12+/api/v1/projects/{project_id}/feature-views\x12\xb0\x01\n\x1b\x43reateFeatureViewNewVersion\x12>.ai.h2o.featurestore.api.v1.CreateFeatureViewNewVersionRequest\x1a/.ai.h2o.featurestore.api.v1.FeatureViewResponse\" \x82\xd3\xe4\x93\x02\x1a\"\x15/api/v1/feature-views:\x01*\x12\xe7\x01\n\"StartRetrieveFeatureViewAsSparkJob\x12=.ai.h2o.featurestore.api.v1.RetrieveFeatureViewAsSparkRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"_\x82\xd3\xe4\x93\x02Y\"T/api/v1/feature-views/{feature_view_id}/{feature_view_version}/retrieve-as-spark-job:\x01*\x12\xb9\x01\n&GetRetrieveFeatureViewAsSparkJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a>.ai.h2o.featurestore.api.v1.RetrieveFeatureViewAsSparkResponse\",\x82\xd3\xe4\x93\x02&\x12$/api/v1/feature-views/spark/{job_id}\x12\xe9\x01\n\"StartRetrieveFeatureViewAsLinksJob\x12?.ai.h2o.featurestore.api.v1.RetrieveFeatureViewAsAsLinksRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"_\x82\xd3\xe4\x93\x02Y\"T/api/v1/feature-views/{feature_view_id}/{feature_view_version}/retrieve-as-links-job:\x01*\x12\xbb\x01\n&GetRetrieveFeatureViewAsLinksJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a@.ai.h2o.featurestore.api.v1.RetrieveFeatureViewAsAsLinksResponse\",\x82\xd3\xe4\x93\x02&\x12$/api/v1/feature-views/links/{job_id}\x12\x92\x01\n\x11\x44\x65leteFeatureView\x12\x34.ai.h2o.featurestore.api.v1.DeleteFeatureViewRequest\x1a\x16.google.protobuf.Empty\"/\x82\xd3\xe4\x93\x02)*\'/api/v1/feature-views/{feature_view_id}\x12\x9a\x01\n\x0f\x43reateMLDataset\x12\x32.ai.h2o.featurestore.api.v1.CreateMLDatasetRequest\x1a\x33.ai.h2o.featurestore.api.v1.CreateMLDatasetResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\"\x13/api/v1/ml-datasets:\x01*\x12\xae\x01\n\x1dGetMLDatasetCreationJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a%.ai.h2o.featurestore.api.v1.MLDataset\"C\x82\xd3\xe4\x93\x02=\x12;/api/v1/ml-datasets//{ml_datasets_id}/creation-job/{job_id}\x12\x9c\x01\n\x0fUpdateMLDataset\x12\x32.ai.h2o.featurestore.api.v1.UpdateMLDatasetRequest\x1a%.ai.h2o.featurestore.api.v1.MLDataset\".\x82\xd3\xe4\x93\x02(\x1a#/api/v1/ml-datasets/{ml_dataset_id}:\x01*\x12\x8a\x01\n\x0f\x44\x65leteMLDataset\x12\x32.ai.h2o.featurestore.api.v1.DeleteMLDatasetRequest\x1a\x16.google.protobuf.Empty\"+\x82\xd3\xe4\x93\x02%*#/api/v1/ml-datasets/{ml_dataset_id}\x12\xc2\x01\n\x0cGetMLDataset\x12/.ai.h2o.featurestore.api.v1.GetMLDatasetRequest\x1a%.ai.h2o.featurestore.api.v1.MLDataset\"Z\x82\xd3\xe4\x93\x02T\x12R/api/v1/feature-views/{feature_view_id}/version/{feature_view_version}/ml-datasets\x12\xa5\x01\n\x0fMLDatasetExists\x12\x32.ai.h2o.featurestore.api.v1.MLDatasetExistsRequest\x1a*.ai.h2o.featurestore.api.v1.ExistsResponse\"2\x82\xd3\xe4\x93\x02,\x12*/api/v1/ml-datasets/{ml_dataset_id}/exists\x12\x94\x01\n\x0eListMLDatasets\x12\x31.ai.h2o.featurestore.api.v1.ListMLDatasetsRequest\x1a\x32.ai.h2o.featurestore.api.v1.ListMLDatasetsResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/api/v1/ml-datasets\x12\xcb\x01\n\x18RetrieveMLDatasetAsSpark\x12;.ai.h2o.featurestore.api.v1.RetrieveMLDatasetAsSparkRequest\x1a<.ai.h2o.featurestore.api.v1.RetrieveMLDatasetAsSparkResponse\"4\x82\xd3\xe4\x93\x02.\")/api/v1/ml-datasets/{ml_dataset_id}/spark:\x01*\x12\xad\x01\n StartRetrieveMLDatasetAsLinksJob\x12=.ai.h2o.featurestore.api.v1.RetrieveMLDatasetAsAsLinksRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"\'\x82\xd3\xe4\x93\x02!\"\x1c/api/v1/ml-datasets/retrieve:\x01*\x12\xb8\x01\n$GetRetrieveMLDatasetAsLinksJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a>.ai.h2o.featurestore.api.v1.RetrieveMLDatasetAsAsLinksResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/api/v1/ml-datasets/retrieve/{job_id}\x12\xe5\x01\n%GenerateMLDatasetOnlineRetrievalToken\x12?.ai.h2o.featurestore.api.v1.OnlineMLDataSetRetrieveTokenRequest\x1a\x37.ai.h2o.featurestore.api.v1.OnlineRetrieveTokenResponse\"B\x82\xd3\xe4\x93\x02<\x12:/api/v1/ml-datasets/{ml_dataset_id}/online/retrieval/token\x12\x97\x01\n\x10ListProjectsPage\x12\x33.ai.h2o.featurestore.api.v1.ListProjectsPageRequest\x1a\x34.ai.h2o.featurestore.api.v1.ListProjectsPageResponse\"\x18\x82\xd3\xe4\x93\x02\x12\x12\x10/api/v1/projects\x12\x91\x01\n\rCreateProject\x12\x30.ai.h2o.featurestore.api.v1.CreateProjectRequest\x1a\x31.ai.h2o.featurestore.api.v1.CreateProjectResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\"\x10/api/v1/projects:\x01*\x12\x91\x01\n\nGetProject\x12-.ai.h2o.featurestore.api.v1.GetProjectRequest\x1a+.ai.h2o.featurestore.api.v1.ProjectResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/api/v1/projects/{project_name}\x12\x97\x01\n\x0eGetProjectById\x12\x31.ai.h2o.featurestore.api.v1.GetProjectByIdRequest\x1a+.ai.h2o.featurestore.api.v1.ProjectResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/api/v1/projects/{project_id}\x12\x7f\n\rDeleteProject\x12\x30.ai.h2o.featurestore.api.v1.DeleteProjectRequest\x1a\x16.google.protobuf.Empty\"$\x82\xd3\xe4\x93\x02\x1e*\x1c/api/v1/projects/{projectId}\x12\x83\x01\n\x12GetProjectsDefault\x12\x16.google.protobuf.Empty\x1a\x33.ai.h2o.featurestore.api.v1.ProjectsDefaultResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/api/v1/projects/default\x12\x9b\x01\n\rProjectExists\x12\x30.ai.h2o.featurestore.api.v1.ProjectExistsRequest\x1a*.ai.h2o.featurestore.api.v1.ExistsResponse\",\x82\xd3\xe4\x93\x02&\x12$/api/v1/projects/{project_id}/exists\x12\x9e\x01\n\rUpdateProject\x12\x30.ai.h2o.featurestore.api.v1.UpdateProjectRequest\x1a\x31.ai.h2o.featurestore.api.v1.UpdateProjectResponse\"(\x82\xd3\xe4\x93\x02\"\x1a\x1d/api/v1/projects/{project_id}:\x01*\x12\xbe\x01\n\x16ListProjectHistoryPage\x12\x39.ai.h2o.featurestore.api.v1.ListProjectHistoryPageRequest\x1a:.ai.h2o.featurestore.api.v1.ListProjectHistoryPageResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/api/v1/projects/{project_id}/history\x12\x91\x01\n\x0eGetAccessToken\x12/.ai.h2o.featurestore.api.v1.RefreshTokenRequest\x1a/.ai.h2o.featurestore.api.v1.AccessTokenResponse\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/api/v1/auth/token:\x01*\x12k\n\x06Logout\x12).ai.h2o.featurestore.api.v1.LogoutRequest\x1a\x16.google.protobuf.Empty\"\x1e\x82\xd3\xe4\x93\x02\x18\"\x13/api/v1/auth/logout:\x01*\x12v\n\rGetActiveUser\x12\x16.google.protobuf.Empty\x1a\x31.ai.h2o.featurestore.api.v1.GetActiveUserResponse\"\x1a\x82\xd3\xe4\x93\x02\x14\x12\x12/api/v1/auth/users\x12k\n\x05Login\x12\x16.google.protobuf.Empty\x1a).ai.h2o.featurestore.api.v1.LoginResponse\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/api/v1/auth/login:\x01*0\x01\x12p\n\x0cGetWebConfig\x12\x16.google.protobuf.Empty\x1a\x30.ai.h2o.featurestore.api.v1.GetWebConfigResponse\"\x16\x82\xd3\xe4\x93\x02\x10\x12\x0e/api/v1/config\x12t\n\x0cGetApiConfig\x12\x16.google.protobuf.Empty\x1a\x30.ai.h2o.featurestore.api.v1.GetApiConfigResponse\"\x1a\x82\xd3\xe4\x93\x02\x14\x12\x12/api/v1/api-config\x12\xb7\x01\n\x17\x41\x64\x64\x46\x65\x61tureSetPermission\x12\x37.ai.h2o.featurestore.api.v1.FeatureSetPermissionRequest\x1a\x16.google.protobuf.Empty\"K\x82\xd3\xe4\x93\x02\x45\"@/api/v1/permissions/feature-sets/add/permission/{feature_set_id}:\x01*\x12\xa9\x01\n\x14\x41\x64\x64ProjectPermission\x12\x34.ai.h2o.featurestore.api.v1.ProjectPermissionRequest\x1a\x16.google.protobuf.Empty\"C\x82\xd3\xe4\x93\x02=\"8/api/v1/permissions/projects/add/permission/{project_id}:\x01*\x12\xbd\x01\n\x1aRemoveFeatureSetPermission\x12\x37.ai.h2o.featurestore.api.v1.FeatureSetPermissionRequest\x1a\x16.google.protobuf.Empty\"N\x82\xd3\xe4\x93\x02H*C/api/v1/permissions/feature-sets/remove/permission/{feature_set_id}:\x01*\x12\xaf\x01\n\x17RemoveProjectPermission\x12\x34.ai.h2o.featurestore.api.v1.ProjectPermissionRequest\x1a\x16.google.protobuf.Empty\"F\x82\xd3\xe4\x93\x02@*;/api/v1/permissions/projects/remove/permission/{project_id}:\x01*\x12\xd0\x01\n\x1eSubmitPendingProjectPermission\x12:.ai.h2o.featurestore.api.v1.SubmitPendingPermissionRequest\x1a;.ai.h2o.featurestore.api.v1.SubmitPendingPermissionResponse\"5\x82\xd3\xe4\x93\x02/\"*/api/v1/permissions/projects/{resource_id}:\x01*\x12\xd7\x01\n!SubmitPendingFeatureSetPermission\x12:.ai.h2o.featurestore.api.v1.SubmitPendingPermissionRequest\x1a;.ai.h2o.featurestore.api.v1.SubmitPendingPermissionResponse\"9\x82\xd3\xe4\x93\x02\x33\"./api/v1/permissions/feature-sets/{resource_id}:\x01*\x12\xbb\x01\n\x1aListProjectPermissionsPage\x12\x36.ai.h2o.featurestore.api.v1.ListPermissionsPageRequest\x1a?.ai.h2o.featurestore.api.v1.ListProjectsPermissionsPageResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/api/v1/permissions/projects\x12\xc6\x01\n\x1eListFeatureSetsPermissionsPage\x12\x36.ai.h2o.featurestore.api.v1.ListPermissionsPageRequest\x1a\x42.ai.h2o.featurestore.api.v1.ListFeatureSetsPermissionsPageResponse\"(\x82\xd3\xe4\x93\x02\"\x12 /api/v1/permissions/feature-sets\x12\xd0\x01\n$ListManageableProjectPermissionsPage\x12\x36.ai.h2o.featurestore.api.v1.ListPermissionsPageRequest\x1a?.ai.h2o.featurestore.api.v1.ListProjectsPermissionsPageResponse\"/\x82\xd3\xe4\x93\x02)\x12\'/api/v1/permissions/manageable-projects\x12\xdb\x01\n(ListManageableFeatureSetsPermissionsPage\x12\x36.ai.h2o.featurestore.api.v1.ListPermissionsPageRequest\x1a\x42.ai.h2o.featurestore.api.v1.ListFeatureSetsPermissionsPageResponse\"3\x82\xd3\xe4\x93\x02-\x12+/api/v1/permissions/manageable-feature-sets\x12\x98\x01\n\x18\x41pprovePendingPermission\x12;.ai.h2o.featurestore.api.v1.ApprovePendingPermissionRequest\x1a\x16.google.protobuf.Empty\"\'\x82\xd3\xe4\x93\x02!\"\x1c/api/v1/permissions/approval:\x01*\x12\x97\x01\n\x17RejectPendingPermission\x12:.ai.h2o.featurestore.api.v1.RejectPendingPermissionRequest\x1a\x16.google.protobuf.Empty\"(\x82\xd3\xe4\x93\x02\"\"\x1d/api/v1/permissions/rejection:\x01*\x12\x9a\x01\n\x19WithdrawPendingPermission\x12<.ai.h2o.featurestore.api.v1.WithdrawPendingPermissionRequest\x1a\x16.google.protobuf.Empty\"\'\x82\xd3\xe4\x93\x02!\"\x1c/api/v1/permissions/withdraw:\x01*\x12\x86\x01\n\x10RevokePermission\x12\x33.ai.h2o.featurestore.api.v1.RevokePermissionRequest\x1a\x16.google.protobuf.Empty\"%\x82\xd3\xe4\x93\x02\x1f\"\x1a/api/v1/permissions/revoke:\x01*\x12\xc8\x01\n\x1aGetActiveProjectPermission\x12\x36.ai.h2o.featurestore.api.v1.GetActivePermissionRequest\x1a\x37.ai.h2o.featurestore.api.v1.GetActivePermissionResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/api/v1/permissions/projects/{resource_id}/active\x12\xcf\x01\n\x1dGetActiveFeatureSetPermission\x12\x36.ai.h2o.featurestore.api.v1.GetActivePermissionRequest\x1a\x37.ai.h2o.featurestore.api.v1.GetActivePermissionResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/api/v1/permissions/feature-sets/{resource_id}/active\x12\xbe\x01\n\x19GetUserProjectPermissions\x12\x35.ai.h2o.featurestore.api.v1.GetUserPermissionsRequest\x1a\x36.ai.h2o.featurestore.api.v1.GetUserPermissionsResponse\"2\x82\xd3\xe4\x93\x02,\x12*/api/v1/permissions/projects/{resource_id}\x12\xc5\x01\n\x1cGetUserFeatureSetPermissions\x12\x35.ai.h2o.featurestore.api.v1.GetUserPermissionsRequest\x1a\x36.ai.h2o.featurestore.api.v1.GetUserPermissionsResponse\"6\x82\xd3\xe4\x93\x02\x30\x12./api/v1/permissions/feature-sets/{resource_id}\x12\xd1\x01\n\x1fGetUserActiveProjectPermissions\x12;.ai.h2o.featurestore.api.v1.GetUserActivePermissionsRequest\x1a\x36.ai.h2o.featurestore.api.v1.GetUserPermissionsResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/api/v1/permissions/projects/active/{resource_id}\x12\xd8\x01\n\"GetUserActiveFeatureSetPermissions\x12;.ai.h2o.featurestore.api.v1.GetUserActivePermissionsRequest\x1a\x36.ai.h2o.featurestore.api.v1.GetUserPermissionsResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/api/v1/permissions/feature-sets/active/{resource_id}\x12\xe8\x01\n!GetUsersWithoutProjectPermissions\x12<.ai.h2o.featurestore.api.v1.GetUsersWithoutPermissionRequest\x1a=.ai.h2o.featurestore.api.v1.GetUsersWithoutPermissionResponse\"F\x82\xd3\xe4\x93\x02@\x12>/api/v1/permissions/projects/{resourceId}/user/permission/none\x12\xef\x01\n$GetUsersWithoutFeatureSetPermissions\x12<.ai.h2o.featurestore.api.v1.GetUsersWithoutPermissionRequest\x1a=.ai.h2o.featurestore.api.v1.GetUsersWithoutPermissionResponse\"J\x82\xd3\xe4\x93\x02\x44\x12\x42/api/v1/permissions/feature-sets/{resourceId}/user/permission/none\x12w\n\x0bRevokeToken\x12(.ai.h2o.featurestore.api.v1.TokenRequest\x1a\x16.google.protobuf.Empty\"&\x82\xd3\xe4\x93\x02 *\x1e/api/v1/auth/tokens/{token_id}\x12\x8f\x01\n\rGenerateToken\x12\x30.ai.h2o.featurestore.api.v1.GenerateTokenRequest\x1a,.ai.h2o.featurestore.api.v1.RawTokenResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\"\x13/api/v1/auth/tokens:\x01*\x12\xb2\x01\n\x18ListPersonalAccessTokens\x12;.ai.h2o.featurestore.api.v1.ListPersonalAccessTokensRequest\x1a<.ai.h2o.featurestore.api.v1.ListPersonalAccessTokensResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/api/v1/auth/tokens\x12\x87\x01\n\x08GetToken\x12(.ai.h2o.featurestore.api.v1.TokenRequest\x1a).ai.h2o.featurestore.api.v1.TokenResponse\"&\x82\xd3\xe4\x93\x02 \x12\x1e/api/v1/auth/tokens/{token_id}\x12\x7f\n\x0fGetTokensConfig\x12\x16.google.protobuf.Empty\x1a\x30.ai.h2o.featurestore.api.v1.TokensConfigResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/auth/tokens/config\x12\xda\x01\n\x13GenerateIngestToken\x12\x37.ai.h2o.featurestore.api.v1.OnlineIngestionTokenRequest\x1a\x38.ai.h2o.featurestore.api.v1.OnlineIngestionTokenResponse\"P\x82\xd3\xe4\x93\x02J\x12H/api/v1/feature-sets/{feature_set_id}/{feature_set_version}/online/token\x12\xeb\x01\n\x1cGenerateOnlineRetrievalToken\x12\x36.ai.h2o.featurestore.api.v1.OnlineRetrieveTokenRequest\x1a\x37.ai.h2o.featurestore.api.v1.OnlineRetrieveTokenResponse\"Z\x82\xd3\xe4\x93\x02T\x12R/api/v1/feature-sets/{feature_set_id}/{feature_set_version}/online/retrieval/token\x12\xca\x01\n\x1dStartMaterializationOnlineJob\x12=.ai.h2o.featurestore.api.v1.StartMaterializationOnlineRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"G\x82\xd3\xe4\x93\x02\x41\"</api/v1/feature-sets/{feature_set_id}/online-materialization:\x01*\x12\xbe\x01\n!GetMaterializationOnlineJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x39.ai.h2o.featurestore.api.v1.MaterializationOnlineResponse\";\x82\xd3\xe4\x93\x02\x35\x12\x33/api/v1/jobs/{job_id}/output/online-materialization\x12\x87\x01\n\x1dGetComputeStatisticsJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x16.google.protobuf.Empty\"+\x82\xd3\xe4\x93\x02%\x12#/api/v1/compute-statistics/{job_id}\x12\xb6\x01\n,GetComputeRecommendationClassifiersJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x16.google.protobuf.Empty\"K\x82\xd3\xe4\x93\x02\x45\x12\x43/api/v1/jobs/{job_id}/output/recommendation-classifiers-computation\x12\xc5\x01\n\x1cGenerateTransformationUpload\x12?.ai.h2o.featurestore.api.v1.GenerateTransformationUploadRequest\x1a@.ai.h2o.featurestore.api.v1.GenerateTransformationUploadResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/api/v1/transformations:\x01*\x12\x96\x01\n\x1dListRecommendationClassifiers\x12\x16.google.protobuf.Empty\x1a@.ai.h2o.featurestore.api.v1.ListRecommendationClassifierResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/api/v1/classifiers\x12\x9b\x01\n\x1e\x43reateRecommendationClassifier\x12\x41.ai.h2o.featurestore.api.v1.CreateRecommendationClassifierRequest\x1a\x16.google.protobuf.Empty\"\x1e\x82\xd3\xe4\x93\x02\x18\"\x13/api/v1/classifiers:\x01*\x12\xa2\x01\n\x1eUpdateRecommendationClassifier\x12\x41.ai.h2o.featurestore.api.v1.UpdateRecommendationClassifierRequest\x1a\x16.google.protobuf.Empty\"%\x82\xd3\xe4\x93\x02\x1f\x1a\x1a/api/v1/classifiers/{name}:\x01*\x12\xaa\x01\n\x1e\x44\x65leteRecommendationClassifier\x12\x41.ai.h2o.featurestore.api.v1.DeleteRecommendationClassifierRequest\x1a\x16.google.protobuf.Empty\"-\x82\xd3\xe4\x93\x02\'*%/api/v1/classifiers/{classifier_name}\x12\xc0\x01\n\x12GetRecommendations\x12\x34.ai.h2o.featurestore.api.v1.GetRecommendationRequest\x1a\x35.ai.h2o.featurestore.api.v1.GetRecommendationResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/api/v1/feature-sets/{feature_set_id}/recommendations\x12p\n\x0cGetDashboard\x12\x16.google.protobuf.Empty\x1a-.ai.h2o.featurestore.api.v1.DashboardResponse\"\x19\x82\xd3\xe4\x93\x02\x13\x12\x11/api/v1/dashboard\x12\x9d\x01\n\x18GetFeatureSetsPopularity\x12\x16.google.protobuf.Empty\x1a\x39.ai.h2o.featurestore.api.v1.FeatureSetsPopularityResponse\".\x82\xd3\xe4\x93\x02(\x12&/api/v1/dashboard/popular-feature-sets\x12\x9d\x01\n\x17GetRecentlyUsedProjects\x12\x16.google.protobuf.Empty\x1a\x38.ai.h2o.featurestore.api.v1.RecentlyUsedProjectsResponse\"0\x82\xd3\xe4\x93\x02*\x12(/api/v1/dashboard/recently-used-projects\x12\xa7\x01\n\x1aGetRecentlyUsedFeatureSets\x12\x16.google.protobuf.Empty\x1a;.ai.h2o.featurestore.api.v1.RecentlyUsedFeatureSetsResponse\"4\x82\xd3\xe4\x93\x02.\x12,/api/v1/dashboard/recently-used-feature-sets\x12\x9c\x01\n\rPinFeatureSet\x12\x30.ai.h2o.featurestore.api.v1.PinFeatureSetRequest\x1a\x16.google.protobuf.Empty\"A\x82\xd3\xe4\x93\x02;\x1a\x36/api/v1/dashboard/pinned-feature-sets/{feature_set_id}:\x01*\x12\xa0\x01\n\x0fUnpinFeatureSet\x12\x32.ai.h2o.featurestore.api.v1.UnpinFeatureSetRequest\x1a\x16.google.protobuf.Empty\"A\x82\xd3\xe4\x93\x02;*6/api/v1/dashboard/pinned-feature-sets/{feature_set_id}:\x01*\x12\xcd\x01\n\x12IsFeatureSetPinned\x12\x35.ai.h2o.featurestore.api.v1.IsFeatureSetPinnedRequest\x1a\x36.ai.h2o.featurestore.api.v1.IsFeatureSetPinnedResponse\"H\x82\xd3\xe4\x93\x02\x42\x12=/api/v1/dashboard/pinned-feature-sets/exists/{feature_set_id}:\x01*\x12\xb3\x01\n\x15ListPinnedFeatureSets\x12\x34.ai.h2o.featurestore.api.v1.PinnedFeatureSetsRequest\x1a\x35.ai.h2o.featurestore.api.v1.PinnedFeatureSetsResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/api/v1/dashboard/pinned-feature-sets\x12\x95\x01\n\x0eSearchProjects\x12\x30.ai.h2o.featurestore.api.v1.ProjectSearchRequest\x1a\x30.ai.h2o.featurestore.api.v1.ProjectSearchResults\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/api/v1/search/projects\x12\xa2\x01\n\x11SearchFeatureSets\x12\x33.ai.h2o.featurestore.api.v1.FeatureSetSearchRequest\x1a\x33.ai.h2o.featurestore.api.v1.FeatureSetSearchResults\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/api/v1/search/feature-sets\x12\x95\x01\n\x0eSearchFeatures\x12\x30.ai.h2o.featurestore.api.v1.FeatureSearchRequest\x1a\x30.ai.h2o.featurestore.api.v1.FeatureSearchResults\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/api/v1/search/features\x12\xad\x01\n\nGetFeature\x12-.ai.h2o.featurestore.api.v1.GetFeatureRequest\x1a+.ai.h2o.featurestore.api.v1.FeatureResponse\"C\x82\xd3\xe4\x93\x02=\x12;/api/v1/feature-sets/{feature_set_id}/features/{feature_id}\x12\xa9\x01\n\x0cListFeatures\x12/.ai.h2o.featurestore.api.v1.ListFeaturesRequest\x1a\x30.ai.h2o.featurestore.api.v1.ListFeaturesResponse\"6\x82\xd3\xe4\x93\x02\x30\x12./api/v1/feature-sets/{feature_set_id}/features\x12\xbc\x01\n\rUpdateFeature\x12\x30.ai.h2o.featurestore.api.v1.UpdateFeatureRequest\x1a\x31.ai.h2o.featurestore.api.v1.UpdateFeatureResponse\"F\x82\xd3\xe4\x93\x02@\x1a;/api/v1/feature-sets/{feature_set_id}/features/{feature_id}:\x01*\x12\xac\x01\n\x13MarkFeatureAsTarget\x12\x30.ai.h2o.featurestore.api.v1.TargetFeatureRequest\x1a\x16.google.protobuf.Empty\"K\x82\xd3\xe4\x93\x02\x45\x1a\x43/api/v1/feature-sets/{feature_set_id}/target-variables/{feature_id}\x12\xaf\x01\n\x16\x44iscardFeatureAsTarget\x12\x30.ai.h2o.featurestore.api.v1.TargetFeatureRequest\x1a\x16.google.protobuf.Empty\"K\x82\xd3\xe4\x93\x02\x45*C/api/v1/feature-sets/{feature_set_id}/target-variables/{feature_id}\x12\xc3\x01\n\x12ListTargetFeatures\x12\x35.ai.h2o.featurestore.api.v1.ListTargetFeaturesRequest\x1a\x36.ai.h2o.featurestore.api.v1.ListTargetFeaturesResponse\">\x82\xd3\xe4\x93\x02\x38\x12\x36/api/v1/feature-sets/{feature_set_id}/target-variables\x12\xbe\x01\n\x15GetListableFeatureSet\x12\x35.ai.h2o.featurestore.api.v1.ListableFeatureSetRequest\x1a\x36.ai.h2o.featurestore.api.v1.ListableFeatureSetResponse\"6\x82\xd3\xe4\x93\x02\x30\x12./api/v1/feature-sets/{feature_set_id}/listable\x12\xce\x01\n\x19GetFeatureSetsDerivedFrom\x12\x39.ai.h2o.featurestore.api.v1.FeatureSetsDerivedFromRequest\x1a:.ai.h2o.featurestore.api.v1.FeatureSetsDerivedFromResponse\":\x82\xd3\xe4\x93\x02\x34\x12\x32/api/v1/feature-sets/{feature_set_id}/derived-from\x12\x9f\x01\n\x11ScheduleIngestJob\x12/.ai.h2o.featurestore.api.v1.ScheduleTaskRequest\x1a\x31.ai.h2o.featurestore.api.v1.ScheduledTaskResponse\"&\x82\xd3\xe4\x93\x02 \"\x1b/api/v1/schedules/ingestion:\x01*\x12\xbc\x01\n\x12ListScheduledTasks\x12\x35.ai.h2o.featurestore.api.v1.ListScheduledTasksRequest\x1a\x36.ai.h2o.featurestore.api.v1.ListScheduledTasksResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//api/v1/feature-sets/{feature_set_id}/schedules\x12\xa1\x01\n\x10GetScheduledTask\x12+.ai.h2o.featurestore.api.v1.ScheduledTaskId\x1a\x31.ai.h2o.featurestore.api.v1.ScheduledTaskResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/api/v1/schedules/{scheduled_task_id}\x12\x89\x01\n\x13\x44\x65leteScheduledTask\x12+.ai.h2o.featurestore.api.v1.ScheduledTaskId\x1a\x16.google.protobuf.Empty\"-\x82\xd3\xe4\x93\x02\'*%/api/v1/schedules/{scheduled_task_id}\x12\x97\x01\n\x13UpdateScheduledTask\x12\x36.ai.h2o.featurestore.api.v1.ScheduledTaskUpdateRequest\x1a\x16.google.protobuf.Empty\"0\x82\xd3\xe4\x93\x02*\x1a%/api/v1/schedules/{scheduled_task_id}:\x01*\x12\x9b\x01\n\x12PauseScheduledTask\x12\x35.ai.h2o.featurestore.api.v1.PauseScheduledTaskRequest\x1a\x16.google.protobuf.Empty\"6\x82\xd3\xe4\x93\x02\x30\x1a+/api/v1/schedules/{scheduled_task_id}/pause:\x01*\x12\x9e\x01\n\x13ResumeScheduledTask\x12\x36.ai.h2o.featurestore.api.v1.ResumeScheduledTaskRequest\x1a\x16.google.protobuf.Empty\"7\x82\xd3\xe4\x93\x02\x31\x1a,/api/v1/schedules/{scheduled_task_id}/resume:\x01*\x12\xa9\x01\n\x16ScheduleLazyIngestTask\x12/.ai.h2o.featurestore.api.v1.ScheduleTaskRequest\x1a\x31.ai.h2o.featurestore.api.v1.ScheduledTaskResponse\"+\x82\xd3\xe4\x93\x02%\" /api/v1/schedules/lazy/ingestion:\x01*\x12\xa4\x01\n\x13StartLazyIngestTask\x12-.ai.h2o.featurestore.api.v1.LazyIngestRequest\x1a..ai.h2o.featurestore.api.v1.LazyIngestResponse\".\x82\xd3\xe4\x93\x02(\x12&/api/v1/schedules/lazy/ingestion/start\x12\xcd\x01\n\x11GetLazyIngestTask\x12\x34.ai.h2o.featurestore.api.v1.GetLazyIngestTaskRequest\x1a\x31.ai.h2o.featurestore.api.v1.ScheduledTaskResponse\"O\x82\xd3\xe4\x93\x02I\x12G/api/v1/schedules/lazy/ingestion/{feature_set_id}/{feature_set_version}\x12\xe8\x01\n!ListScheduledTaskExecutionHistory\x12>.ai.h2o.featurestore.api.v1.ListScheduledTaskExecutionsRequest\x1a?.ai.h2o.featurestore.api.v1.ListScheduledTaskExecutionsResponse\"B\x82\xd3\xe4\x93\x02<\x12\x37/api/v1/schedules/{scheduled_task_id}/execution-history:\x01*\x12\xc8\x01\n\x1bListTransformationFunctions\x12>.ai.h2o.featurestore.api.v1.ListTransformationFunctionsRequest\x1a?.ai.h2o.featurestore.api.v1.ListTransformationFunctionsResponse\"(\x82\xd3\xe4\x93\x02\"\x12 /api/v1/transformation_functions\x12\xe1\x01\n\x19GetTransformationFunction\x12<.ai.h2o.featurestore.api.v1.GetTransformationFunctionRequest\x1a=.ai.h2o.featurestore.api.v1.GetTransformationFunctionResponse\"G\x82\xd3\xe4\x93\x02\x41\x12?/api/v1/transformation_functions/{transformation_function_name}\x12\x96\x01\n\x14GetBackfillJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a,.ai.h2o.featurestore.api.v1.BackfillResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/api/v1/jobs/{job_id}/output/backfill\x12\x8a\x01\n\x15\x43reateDraftFeatureSet\x12\x32.ai.h2o.featurestore.api.v1.FeatureSetDraftRequest\x1a\x16.google.protobuf.Empty\"%\x82\xd3\xe4\x93\x02\x1f\"\x1a/api/v1/feature-sets/draft:\x01*\x12\xb0\x01\n!CreateMajorVersionDraftFeatureSet\x12>.ai.h2o.featurestore.api.v1.FeatureSetMajorVersionDraftRequest\x1a\x16.google.protobuf.Empty\"3\x82\xd3\xe4\x93\x02-\"(/api/v1/feature-sets/draft-major-version:\x01*\x12\xb7\x01\n\x19\x43reateFeatureSetFromDraft\x12\x34.ai.h2o.featurestore.api.v1.DraftToFeatureSetRequest\x1a\x35.ai.h2o.featurestore.api.v1.DraftToFeatureSetResponse\"-\x82\xd3\xe4\x93\x02\'\"\"/api/v1/feature-sets/draft/publish:\x01*\x12\xfe\x01\n,CreateFeatureSetVersionFromMajorVersionDraft\x12G.ai.h2o.featurestore.api.v1.MajorVersionDraftToFeatureSetVersionRequest\x1aH.ai.h2o.featurestore.api.v1.MajorVersionDraftToFeatureSetVersionResponse\";\x82\xd3\xe4\x93\x02\x35\"0/api/v1/feature-sets/draft-major-version/publish:\x01*\x12\x99\x01\n\x15\x44\x65leteFeatureSetDraft\x12-.ai.h2o.featurestore.api.v1.FeatureSetDraftId\x1a\x16.google.protobuf.Empty\"9\x82\xd3\xe4\x93\x02\x33*1/api/v1/feature-sets/draft/{feature_set_draft_id}\x12\xad\x01\n\x14ListFeatureSetDrafts\x12\x37.ai.h2o.featurestore.api.v1.ListFeatureSetDraftsRequest\x1a\x38.ai.h2o.featurestore.api.v1.ListFeatureSetDraftsResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/feature-sets/draft\x12\xb3\x01\n\x12GetFeatureSetDraft\x12-.ai.h2o.featurestore.api.v1.FeatureSetDraftId\x1a\x33.ai.h2o.featurestore.api.v1.FeatureSetDraftResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/api/v1/feature-sets/draft/{feature_set_draft_id}\x12\xa4\x01\n\x11StoreFileArtifact\x12\x34.ai.h2o.featurestore.api.v1.StoreFileArtifactRequest\x1a\x35.ai.h2o.featurestore.api.v1.StoreFileArtifactResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/api/v1/artifacts/files:\x01*\x12\xa6\x01\n\x10RetrieveArtifact\x12\x33.ai.h2o.featurestore.api.v1.RetrieveArtifactRequest\x1a\x34.ai.h2o.featurestore.api.v1.RetrieveArtifactResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/api/v1/artifacts/{artifact_id}\x12\x96\x01\n\x12UpdateUploadStatus\x12\x35.ai.h2o.featurestore.api.v1.UpdateUploadStatusRequest\x1a\x16.google.protobuf.Empty\"1\x82\xd3\xe4\x93\x02+\x1a&/api/v1/artifacts/{artifact_id}/status:\x01*\x12\x84\x01\n\x0e\x44\x65leteArtifact\x12\x31.ai.h2o.featurestore.api.v1.DeleteArtifactRequest\x1a\x16.google.protobuf.Empty\"\'\x82\xd3\xe4\x93\x02!*\x1f/api/v1/artifacts/{artifact_id}\x12\xbc\x01\n\rListArtifacts\x12\x30.ai.h2o.featurestore.api.v1.ListArtifactsRequest\x1a\x31.ai.h2o.featurestore.api.v1.ListArtifactsResponse\"F\x82\xd3\xe4\x93\x02@\x12>/api/v1/artifacts/{feature_set_id}/{feature_set_major_version}\x12\x8c\x01\n\tStoreLink\x12,.ai.h2o.featurestore.api.v1.StoreLinkRequest\x1a-.ai.h2o.featurestore.api.v1.StoreLinkResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/api/v1/artifacts/links:\x01*\x12\xcf\x01\n\x10GetCodeSnippedId\x12\x30.ai.h2o.featurestore.api.v1.CodeSnippedIdRequest\x1a\x31.ai.h2o.featurestore.api.v1.CodeSnippedIdResponse\"V\x82\xd3\xe4\x93\x02P\x12N/api/v1/artifacts/{feature_set_id}/{feature_set_major_version}/code-snipped-id\x12\xab\x01\n\x17ListFeatureSetsToReview\x12:.ai.h2o.featurestore.api.v1.ListFeatureSetsToReviewRequest\x1a;.ai.h2o.featurestore.api.v1.ListFeatureSetsToReviewResponse\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/api/v1/reviews\x12\x8a\x01\n\rApproveReview\x12\x30.ai.h2o.featurestore.api.v1.ApproveReviewRequest\x1a\x16.google.protobuf.Empty\"/\x82\xd3\xe4\x93\x02)\"$/api/v1/reviews/{review_id}/approval:\x01*\x12\x89\x01\n\x0cRejectReview\x12/.ai.h2o.featurestore.api.v1.RejectReviewRequest\x1a\x16.google.protobuf.Empty\"0\x82\xd3\xe4\x93\x02*\"%/api/v1/reviews/{review_id}/rejection:\x01*\x12\xbd\x01\n\x1aListFeatureSetsReviewsPage\x12<.ai.h2o.featurestore.api.v1.ListFeatureSetReviewsPageRequest\x1a=.ai.h2o.featurestore.api.v1.ListFeatureSetReviewsPageResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/reviews/my-reviews\x12\xde\x01\n\x1dGetListableFeatureSetToReview\x12@.ai.h2o.featurestore.api.v1.GetListableFeatureSetToReviewRequest\x1a\x41.ai.h2o.featurestore.api.v1.GetListableFeatureSetToReviewResponse\"8\x82\xd3\xe4\x93\x02\x32\x12\x30/api/v1/reviews/{review_id}/listable/feature-set\x12\xe9\x01\n\x1dGetListableFeatureSetInReview\x12@.ai.h2o.featurestore.api.v1.GetListableFeatureSetInReviewRequest\x1a\x41.ai.h2o.featurestore.api.v1.GetListableFeatureSetInReviewResponse\"C\x82\xd3\xe4\x93\x02=\x12;/api/v1/reviews/my-reviews/{review_id}/listable/feature-set\x12\xb2\x01\n\x1f\x44\x65leteFeatureSetVersionInReview\x12;.ai.h2o.featurestore.api.v1.DeleteRejectedFeatureSetRequest\x1a\x16.google.protobuf.Empty\":\x82\xd3\xe4\x93\x02\x34*2/api/v1/reviews/my-reviews/{review_id}/feature-set\x12\xcc\x01\n\x14ListFeaturesToReview\x12\x37.ai.h2o.featurestore.api.v1.ListFeaturesToReviewRequest\x1a\x38.ai.h2o.featurestore.api.v1.ListFeaturesToReviewResponse\"A\x82\xd3\xe4\x93\x02;\x12\x39/api/v1/reviews/{review_id}/listable/feature-set/features\x12\xd7\x01\n\x14ListFeaturesInReview\x12\x37.ai.h2o.featurestore.api.v1.ListFeaturesInReviewRequest\x1a\x38.ai.h2o.featurestore.api.v1.ListFeaturesInReviewResponse\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/api/v1/reviews/my-reviews/{review_id}/listable/feature-set/features\x12\xda\x01\n\x1cGetFeatureSetPreviewToReview\x12?.ai.h2o.featurestore.api.v1.GetFeatureSetPreviewToReviewRequest\x1a@.ai.h2o.featurestore.api.v1.GetFeatureSetPreviewToReviewResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//api/v1/reviews/{review_id}/feature-set/preview\x12\xe5\x01\n\x1cGetFeatureSetPreviewInReview\x12?.ai.h2o.featurestore.api.v1.GetFeatureSetPreviewInReviewRequest\x1a@.ai.h2o.featurestore.api.v1.GetFeatureSetPreviewInReviewResponse\"B\x82\xd3\xe4\x93\x02<\x12:/api/v1/reviews/my-reviews/{review_id}/feature-set/preview\x12\xbd\x01\n\x15GetFeatureSetToReview\x12\x38.ai.h2o.featurestore.api.v1.GetFeatureSetToReviewRequest\x1a\x39.ai.h2o.featurestore.api.v1.GetFeatureSetToReviewResponse\"/\x82\xd3\xe4\x93\x02)\x12\'/api/v1/reviews/{review_id}/feature-set\x12\xc8\x01\n\x15GetFeatureSetInReview\x12\x38.ai.h2o.featurestore.api.v1.GetFeatureSetInReviewRequest\x1a\x39.ai.h2o.featurestore.api.v1.GetFeatureSetInReviewResponse\":\x82\xd3\xe4\x93\x02\x34\x12\x32/api/v1/reviews/my-reviews/{review_id}/feature-setB\x14\x42\x10\x43oreServiceProtoP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,ai/h2o/featurestore/api/v1/CoreService.proto\x12\x1a\x61i.h2o.featurestore.api.v1\x1a\x1egoogle/protobuf/duration.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x31\x61i/h2o/featurestore/api/v1/FeatureSetSearch.proto\x1a*ai/h2o/featurestore/api/v1/OnlineApi.proto\x1a.ai/h2o/featurestore/api/v1/TimeToLiveApi.proto\x1a\x33\x61i/h2o/featurestore/api/v1/FeatureSetProtoApi.proto\x1a\x37\x61i/h2o/featurestore/api/v1/RecommendationProtoApi.proto\x1a-ai/h2o/featurestore/api/v1/DashboardApi.proto\"\x9c\x01\n\x1dValidatePersonalTokenResponse\x12\x37\n\x04user\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x13\n\x0b\x61uthorities\x18\x02 \x03(\t\x12-\n\texpire_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x9e\x01\n\x19GetUserPermissionsRequest\x12\x13\n\x0bresource_id\x18\x01 \x01(\t\x12\x45\n\x11permission_filter\x18\x02 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\x12\n\npage_token\x18\x04 \x01(\t\"\xb4\x01\n\x1fGetUserActivePermissionsRequest\x12\x13\n\x0bresource_id\x18\x01 \x01(\t\x12\x46\n\x12permission_filters\x18\x02 \x03(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12\r\n\x05query\x18\x03 \x01(\t\x12\x11\n\tpage_size\x18\x04 \x01(\x05\x12\x12\n\npage_token\x18\x05 \x01(\t\"t\n\x1aGetUserPermissionsResponse\x12=\n\x05users\x18\x01 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.UserWithPermission\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x9a\x01\n\x12UserWithPermission\x12\x37\n\x04user\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12K\n\x13resource_permission\x18\x02 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.ResourcePermission\"\x95\x01\n\x12ResourcePermission\x12>\n\npermission\x18\x01 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12?\n\rresource_type\x18\x02 \x01(\x0e\x32(.ai.h2o.featurestore.api.v1.ResourceType\"^\n GetUsersWithoutPermissionRequest\x12\x13\n\x0bresource_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"v\n!GetUsersWithoutPermissionResponse\x12\x38\n\x05users\x18\x01 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"H\n\x1fListPersonalAccessTokensRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\"\x8c\x01\n ListPersonalAccessTokensResponse\x12O\n\x16personal_access_tokens\x18\x01 \x03(\x0b\x32/.ai.h2o.featurestore.api.v1.PersonalAccessToken\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"R\n\x17IdentityProviderDetails\x12\x14\n\x0cidp_meta_url\x18\x01 \x01(\t\x12\x11\n\tclient_id\x18\x02 \x01(\t\x12\x0e\n\x06scopes\x18\x03 \x03(\t\"\xb4\x01\n\x14GetWebConfigResponse\x12H\n\x0bipd_details\x18\x01 \x01(\x0b\x32\x33.ai.h2o.featurestore.api.v1.IdentityProviderDetails\x12\x15\n\rapp_store_url\x18\x02 \x01(\t\x12\x0f\n\x07web_url\x18\x03 \x01(\t\x12\x14\n\x0creview_roles\x18\x04 \x03(\t\x12\x14\n\x0ch2o_gpte_url\x18\x05 \x01(\t\"d\n-GetFeatureSetsLastMinorForCurrentMajorRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"\x81\x01\n.GetLastMinorFeatureSetForMajorInProjectRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x03 \x01(\x05\"m\n\x17\x46\x65\x61tureSetExistsRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\x12\x17\n\x0f\x65xclude_deleted\x18\x05 \x01(\x08\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x06 \x01(\x05\"N\n\x17GetIngestHistoryRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x03 \x01(\t\"C\n\x14ProjectExistsRequest\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x17\n\x0f\x65xclude_deleted\x18\x03 \x01(\x08\"L\n\x18\x46\x65\x61tureViewExistsRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x04 \x01(\t\x12\x17\n\x0f\x65xclude_deleted\x18\x05 \x01(\x08\"H\n\x16MLDatasetExistsRequest\x12\x15\n\rml_dataset_id\x18\x04 \x01(\t\x12\x17\n\x0f\x65xclude_deleted\x18\x05 \x01(\x08\" \n\x0e\x45xistsResponse\x12\x0e\n\x06\x65xists\x18\x01 \x01(\x08\")\n\x17ProjectsDefaultResponse\x12\x0e\n\x06locked\x18\x01 \x01(\x08\"P\n\x1eHasPermissionToRetrieveRequest\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\"B\n\x1fHasPermissionToRetrieveResponse\x12\x1f\n\x17has_retrieve_permission\x18\x01 \x01(\x08\"e\n\x1bStartRevertIngestJobRequest\x12\x11\n\tingest_id\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x03 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x04 \x01(\t\"e\n\x12OnlineRetrieveMeta\x12\x17\n\x0f\x62\x61se_online_url\x18\x01 \x01(\t\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x12\n\nis_enabled\x18\x04 \x01(\x08\",\n\x13RefreshTokenRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\" \n\x0cTokenRequest\x12\x10\n\x08token_id\x18\x01 \x01(\t\"j\n\x14GenerateTokenRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12/\n\x0b\x65xpiry_date\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"O\n\rTokenResponse\x12>\n\x05token\x18\x01 \x01(\x0b\x32/.ai.h2o.featurestore.api.v1.PersonalAccessToken\"X\n\x10RawTokenResponse\x12\r\n\x05token\x18\x01 \x01(\t\x12\x35\n\x11token_expiry_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"Y\n\x14TokensConfigResponse\x12\x41\n\x1emaximum_allowed_token_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\"p\n\x0fListJobsRequest\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x12\x35\n\x08job_type\x18\x03 \x01(\x0e\x32#.ai.h2o.featurestore.api.v1.JobType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\"A\n\x10ListJobsResponse\x12-\n\x04jobs\x18\x01 \x03(\x0b\x32\x1f.ai.h2o.featurestore.api.v1.Job\"\xc5\x01\n$FeatureSetSchemaCompatibilityRequest\x12\x42\n\x0foriginal_schema\x18\x01 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12=\n\nnew_schema\x18\x02 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12\x1a\n\x12\x63ompare_data_types\x18\x03 \x01(\x08\">\n%FeatureSetSchemaCompatibilityResponse\x12\x15\n\ris_compatible\x18\x01 \x01(\x08\"\xbd\x01\n\x1c\x46\x65\x61tureSetSchemaPatchRequest\x12\x42\n\x0foriginal_schema\x18\x01 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12=\n\nnew_schema\x18\x02 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12\x1a\n\x12\x63ompare_data_types\x18\x03 \x01(\x08\"Z\n\x1d\x46\x65\x61tureSetSchemaPatchResponse\x12\x39\n\x06schema\x18\x01 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\"\x17\n\x05JobId\x12\x0e\n\x06job_id\x18\x01 \x01(\t\"2\n\x18GetRecommendationRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\"\xaf\x02\n\x19GetRecommendationResponse\x12L\n\x07matches\x18\x01 \x03(\x0b\x32;.ai.h2o.featurestore.api.v1.GetRecommendationResponse.Match\x1a+\n\x04Join\x12\x12\n\nclassifier\x18\x01 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x02 \x03(\t\x1a\x96\x01\n\x05Match\x12\x42\n\x12target_feature_set\x18\x01 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\x12I\n\x05joins\x18\x02 \x03(\x0b\x32:.ai.h2o.featurestore.api.v1.GetRecommendationResponse.Join\"\xc3\x02\n\x03Job\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x35\n\x08job_type\x18\x02 \x01(\x0e\x32#.ai.h2o.featurestore.api.v1.JobType\x12\x0c\n\x04\x64one\x18\x03 \x01(\x08\x12\x13\n\x0b\x63hildJobIds\x18\x04 \x03(\t\x12\x11\n\tcancelled\x18\x05 \x01(\x08\x12\x39\n\njob_status\x18\x06 \x01(\x0e\x32%.ai.h2o.featurestore.api.v1.JobStatus\x12=\n\ncreated_by\x18\x07 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12.\n\ncreated_on\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x15\n\rerror_message\x18\t \x01(\t\"6\n\x10JobProgressInput\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x12\n\nnext_index\x18\x02 \x01(\x05\"\xc6\x01\n\x11JobProgressOutput\x12H\n\x08progress\x18\x01 \x03(\x0b\x32\x36.ai.h2o.featurestore.api.v1.JobProgressOutput.Progress\x1ag\n\x08Progress\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x1b\n\x13\x64uration_in_seconds\x18\x02 \x01(\r\x12-\n\ttimestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8a\x01\n\x1b\x46\x65\x61tureSetPermissionRequest\x12\x13\n\x0buser_emails\x18\x02 \x03(\t\x12>\n\npermission\x18\x03 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\"\x83\x01\n\x18ProjectPermissionRequest\x12\x13\n\x0buser_emails\x18\x02 \x03(\t\x12>\n\npermission\x18\x03 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12\x12\n\nproject_id\x18\x04 \x01(\t\"\xe8\x01\n\x1cStartExtractSchemaJobRequest\x12?\n\x08raw_data\x18\x01 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocationH\x00\x12\x46\n\x0c\x64\x65rived_from\x18\x03 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformationH\x00\x12\x35\n\x04\x63red\x18\x02 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.CredentialsB\x08\n\x06source\"\x98\x01\n\x15\x45xtractSchemaResponse\x12\x39\n\x06schema\x18\x01 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12\x44\n\x0c\x64\x65rived_from\x18\x02 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\"7\n\x1dListFeatureSetsVersionRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\"\x81\x01\n\x12\x46\x65\x61tureSetResponse\x12;\n\x0b\x66\x65\x61ture_set\x18\x01 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\x12.\n\x03job\x18\x02 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.JobId\"_\n\x18UpdateFeatureSetResponse\x12\x43\n\x13updated_feature_set\x18\x01 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\"U\n\x15UpdateProjectResponse\x12<\n\x0fupdated_project\x18\x02 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\"\x9a\x01\n\x15UpdateFeatureResponse\x12\x43\n\x13updated_feature_set\x18\x01 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\x12<\n\x0fupdated_feature\x18\x02 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\"G\n\x0fProjectResponse\x12\x34\n\x07project\x18\x01 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\"I\n\rLoginResponse\x12\x13\n\tlogin_url\x18\x01 \x01(\tH\x00\x12\x17\n\rrefresh_token\x18\x02 \x01(\tH\x00\x42\n\n\x08response\"d\n\x15GetActiveUserResponse\x12\x37\n\x04user\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x12\n\nuser_roles\x18\x02 \x03(\t\")\n\x11GetProjectRequest\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\"+\n\x15GetProjectByIdRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\"1\n\x17\x44\x65leteFeatureSetRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\"[\n\x1e\x44\x65leteFeatureSetVersionRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x02 \x01(\x05\"&\n\rLogoutRequest\x12\x15\n\rrefresh_token\x18\x01 \x01(\t\"P\n\rUserBasicInfo\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x16\n\x0epreferred_name\x18\x04 \x01(\t\"Y\n\x04User\x12\x42\n\x0fuser_basic_info\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\r\n\x05\x61\x64min\x18\x02 \x01(\x08\"y\n\x13\x41\x63\x63\x65ssTokenResponse\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12\x15\n\rrefresh_token\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\x03\x12\r\n\x05scope\x18\x04 \x01(\t\x12\x12\n\ntoken_type\x18\x05 \x01(\t\"*\n\x14\x44\x65leteProjectRequest\x12\x12\n\nproject_id\x18\x02 \x01(\t\"\x8f\x01\n\x14\x43reateProjectRequest\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06secret\x18\x03 \x01(\x08\x12\x0e\n\x06locked\x18\x04 \x01(\x08\x12,\n\x0b\x63ustom_data\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\"e\n\x15\x43reateProjectResponse\x12\x34\n\x07project\x18\x01 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\x12\x16\n\x0e\x61lready_exists\x18\x02 \x01(\x08\"M\n\x14ListProjectsResponse\x12\x35\n\x08projects\x18\x01 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\"Z\n\x1dListProjectHistoryPageRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"\xc2\x01\n\x0eProjectHistory\x12\x39\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32).ai.h2o.featurestore.api.v1.ProjectAction\x12?\n\x0cperformed_by\x18\x02 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x34\n\x07project\x18\x03 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\"v\n\x1eListProjectHistoryPageResponse\x12;\n\x07history\x18\x01 \x03(\x0b\x32*.ai.h2o.featurestore.api.v1.ProjectHistory\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"`\n\x18GetIngestHistoryResponse\x12\x44\n\x0eingest_history\x18\x01 \x03(\x0b\x32,.ai.h2o.featurestore.api.v1.FeatureSetIngest\"Z\n\x1aListFeatureSetsPageRequest\x12\x15\n\rproject_names\x18\x01 \x03(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"t\n\x1bListFeatureSetsPageResponse\x12<\n\x0c\x66\x65\x61ture_sets\x18\x01 \x03(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x87\x01\n\x0e\x41WSCredentials\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12\x14\n\x0csecret_token\x18\x02 \x01(\t\x12\x0e\n\x06region\x18\x03 \x01(\t\x12\x10\n\x08\x65ndpoint\x18\x05 \x01(\t\x12\x10\n\x08role_arn\x18\x06 \x01(\t\x12\x15\n\rsession_token\x18\x07 \x01(\t\"\xa6\x01\n\x10\x41zureCredentials\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x63\x63ount_key\x18\x02 \x01(\t\x12\x11\n\tsas_token\x18\x03 \x01(\t\x12\x15\n\rsas_container\x18\x04 \x01(\t\x12\x14\n\x0csp_client_id\x18\x05 \x01(\t\x12\x14\n\x0csp_tenant_id\x18\x06 \x01(\t\x12\x11\n\tsp_secret\x18\x07 \x01(\t\"c\n\x14SnowflakeCredentials\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x17\n\x0fpem_private_key\x18\x03 \x01(\t\x12\x12\n\npassphrase\x18\x04 \x01(\t\"1\n\x0fJDBCCredentials\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"4\n\x12MongoDbCredentials\x12\x0c\n\x04user\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"\x12\n\x10\x44riveCredentials\"\x91\x03\n\x0b\x43redentials\x12\x37\n\x03\x61ws\x18\x01 \x01(\x0b\x32*.ai.h2o.featurestore.api.v1.AWSCredentials\x12;\n\x05\x61zure\x18\x02 \x01(\x0b\x32,.ai.h2o.featurestore.api.v1.AzureCredentials\x12\x43\n\tsnowflake\x18\x03 \x01(\x0b\x32\x30.ai.h2o.featurestore.api.v1.SnowflakeCredentials\x12\x42\n\rjdbc_database\x18\x04 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.JDBCCredentials\x12@\n\x08mongo_db\x18\x06 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.MongoDbCredentials\x12;\n\x05\x64rive\x18\x07 \x01(\x0b\x32,.ai.h2o.featurestore.api.v1.DriveCredentialsJ\x04\x08\x05\x10\x06\"W\n\x17ListFeatureSetsResponse\x12<\n\x0c\x66\x65\x61ture_sets\x18\x01 \x03(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\"l\n\x1eListFeatureSetVersionsResponse\x12J\n\x08versions\x18\x01 \x03(\x0b\x32\x38.ai.h2o.featurestore.api.v1.FeatureSetVersionDescription\"~\n\x1c\x46\x65\x61tureSetVersionDescription\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x16\n\x0eversion_change\x18\x02 \x01(\t\x12\x35\n\x11\x63reated_date_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"U\n\x14GetFeatureSetRequest\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x12\n\nproject_id\x18\x04 \x01(\t\"\xd1\x01\n\x15StartIngestJobRequest\x12\x35\n\x04\x63red\x18\x02 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.Credentials\x12@\n\x0b\x64\x61ta_source\x18\x05 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocation\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x06 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x07 \x01(\tJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05\"\xe3\x02\n\x0eIngestResponse\x12\x43\n\x04meta\x18\x01 \x01(\x0b\x32\x35.ai.h2o.featurestore.api.v1.IngestResponse.IngestMeta\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x03 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x04 \x01(\t\x1a\xd6\x01\n\nIngestMeta\x12\x16\n\x0e\x63\x61\x63he_location\x18\x01 \x01(\t\x12\x1a\n\x12raw_cache_location\x18\x02 \x01(\t\x12\x37\n\x13ingestion_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\x0cingest_scope\x18\x04 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x0f\n\x07message\x18\x05 \x01(\t\x12\x11\n\tingest_id\x18\x06 \x01(\t\"\x9d\x01\n\x0fRetrieveRequest\x12\x17\n\x0fstart_date_time\x18\x02 \x01(\t\x12\x15\n\rend_date_time\x18\x03 \x01(\t\x12\x11\n\tingest_id\x18\x04 \x01(\t\x12\x12\n\nsession_id\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x06 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x07 \x01(\t\"\x8b\x01\n\x17RetrieveAsLinksResponse\x12\x16\n\x0e\x64ownload_links\x18\x01 \x03(\t\x12\x39\n\x0eretrieve_scope\x18\x02 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x1d\n\x15retrieve_job_executed\x18\x03 \x01(\x08\"\xe8\x02\n\x17RetrieveAsSparkResponse\x12\x12\n\ncache_path\x18\x01 \x01(\t\x12Q\n\x07options\x18\x02 \x03(\x0b\x32@.ai.h2o.featurestore.api.v1.RetrieveAsSparkResponse.OptionsEntry\x12\x39\n\x0eretrieve_scope\x18\x03 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x12\n\nsession_id\x18\x04 \x01(\t\x12\x15\n\rdelta_version\x18\x05 \x01(\x03\x12P\n\x16offline_storage_format\x18\x06 \x01(\x0e\x32\x30.ai.h2o.featurestore.api.v1.OfflineStorageFormat\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"X\n!StartMaterializationOnlineRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x03 \x01(\t\"v\n\x1dMaterializationOnlineResponse\x12@\n\x15materialization_scope\x18\x01 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x13\n\x0bnum_records\x18\x02 \x01(\x04\"Y\n\"StartOnlineOfflineIngestionRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"2\n\x1cIngestWriteCredentialRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"\xca\x01\n\x1dIngestWriteCredentialResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\x12W\n\x07options\x18\x02 \x03(\x0b\x32\x46.ai.h2o.featurestore.api.v1.IngestWriteCredentialResponse.OptionsEntry\x12\x12\n\nsession_id\x18\x03 \x01(\t\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x9c\x01\n\x1eStartOptimizeStorageJobRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\x12\x45\n\x0coptimization\x18\x03 \x01(\x0b\x32/.ai.h2o.featurestore.api.v1.StorageOptimization\"\xb9\x01\n\x13StorageOptimization\x12M\n\nz_order_by\x18\x01 \x01(\x0b\x32\x37.ai.h2o.featurestore.api.v1.OptimizeStorageZOrderBySpecH\x00\x12I\n\x07\x63ompact\x18\x02 \x01(\x0b\x32\x36.ai.h2o.featurestore.api.v1.OptimizeStorageCompactSpecH\x00\x42\x08\n\x06method\".\n\x1bOptimizeStorageZOrderBySpec\x12\x0f\n\x07\x63olumns\x18\x01 \x03(\t\"\x1c\n\x1aOptimizeStorageCompactSpec\"7\n\x17OptimizeStorageResponse\x12\x1c\n\x14optimization_metrics\x18\x01 \x01(\t\"\xb4\x06\n\x0fRawDataLocation\x12\x36\n\x03\x63sv\x18\x01 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.CSVFileSpecH\x00\x12>\n\x07parquet\x18\x02 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.ParquetFileSpecH\x00\x12\x43\n\tsnowflake\x18\x03 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.SnowflakeTableSpecH\x00\x12\x39\n\x04jdbc\x18\x04 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.JDBCTableSpecH\x00\x12\x38\n\x04json\x18\x07 \x01(\x0b\x32(.ai.h2o.featurestore.api.v1.JSONFileSpecH\x00\x12\x41\n\x0b\x64\x65lta_table\x18\x08 \x01(\x0b\x32*.ai.h2o.featurestore.api.v1.DeltaTableSpecH\x00\x12?\n\ncsv_folder\x18\n \x01(\x0b\x32).ai.h2o.featurestore.api.v1.CSVFolderSpecH\x00\x12G\n\x0eparquet_folder\x18\x0b \x01(\x0b\x32-.ai.h2o.featurestore.api.v1.ParquetFolderSpecH\x00\x12\x41\n\x0bjson_folder\x18\x0c \x01(\x0b\x32*.ai.h2o.featurestore.api.v1.JSONFolderSpecH\x00\x12G\n\x0ctemp_parquet\x18\r \x01(\x0b\x32/.ai.h2o.featurestore.api.v1.TempParquetFileSpecH\x00\x12\x45\n\ronline_source\x18\x0e \x01(\x0b\x32,.ai.h2o.featurestore.api.v1.OnlineSourceSpecH\x00\x12\x45\n\x08mongo_db\x18\x0f \x01(\x0b\x32\x31.ai.h2o.featurestore.api.v1.MongoDbCollectionSpecH\x00\x42\x08\n\x06source\"5\n\x10OnlineSourceSpec\x12!\n\x19\x61\x62solute_json_folder_path\x18\x01 \x01(\t\".\n\x0b\x43SVFileSpec\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tdelimiter\x18\x02 \x01(\t\"/\n\x0cJSONFileSpec\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\tmultiline\x18\x02 \x01(\x08\"\x1f\n\x0fParquetFileSpec\x12\x0c\n\x04path\x18\x01 \x01(\t\"#\n\x13TempParquetFileSpec\x12\x0c\n\x04path\x18\x01 \x01(\t\"C\n\x05Proxy\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x0c\n\x04user\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\"\xd7\x01\n\x12SnowflakeTableSpec\x12\r\n\x05table\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\x12\x11\n\twarehouse\x18\x05 \x01(\t\x12\x0e\n\x06schema\x18\x06 \x01(\t\x12\x10\n\x08insecure\x18\x07 \x01(\x08\x12\x30\n\x05proxy\x18\x08 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Proxy\x12\x0c\n\x04role\x18\t \x01(\t\x12\x0f\n\x07\x61\x63\x63ount\x18\n \x01(\t\"\xb5\x01\n\rJDBCTableSpec\x12\r\n\x05table\x18\x01 \x01(\t\x12\r\n\x05query\x18\x02 \x01(\t\x12\x16\n\x0e\x63onnection_url\x18\x03 \x01(\t\x12\x16\n\x0enum_partitions\x18\x04 \x01(\x05\x12\x18\n\x10partition_column\x18\x05 \x01(\t\x12\x13\n\x0blower_bound\x18\x06 \x01(\x04\x12\x13\n\x0bupper_bound\x18\x07 \x01(\x04\x12\x12\n\nfetch_size\x18\x08 \x01(\x05\"v\n\x0e\x44\x65ltaTableSpec\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\x11\n\ttimestamp\x18\x03 \x01(\t\x12\x32\n\x06\x66ilter\x18\x04 \x01(\x0b\x32\".ai.h2o.featurestore.api.v1.Filter\"O\n\rCSVFolderSpec\x12\x13\n\x0broot_folder\x18\x01 \x01(\t\x12\x16\n\x0e\x66ilter_pattern\x18\x02 \x01(\t\x12\x11\n\tdelimiter\x18\x03 \x01(\t\"@\n\x11ParquetFolderSpec\x12\x13\n\x0broot_folder\x18\x01 \x01(\t\x12\x16\n\x0e\x66ilter_pattern\x18\x02 \x01(\t\"P\n\x0eJSONFolderSpec\x12\x13\n\x0broot_folder\x18\x01 \x01(\t\x12\x16\n\x0e\x66ilter_pattern\x18\x02 \x01(\t\x12\x11\n\tmultiline\x18\x03 \x01(\x08\"U\n\x15MongoDbCollectionSpec\x12\x16\n\x0e\x63onnection_uri\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x12\n\ncollection\x18\x03 \x01(\t\"&\n\x12MojoTransformation\x12\x10\n\x08\x66ilename\x18\x03 \x01(\t\"/\n\x1bSparkPipelineTransformation\x12\x10\n\x08\x66ilename\x18\x03 \x01(\t\"r\n\x12JoinTransformation\x12\x10\n\x08left_key\x18\x01 \x01(\t\x12\x11\n\tright_key\x18\x02 \x01(\t\x12\x37\n\tjoin_type\x18\x03 \x01(\x0e\x32$.ai.h2o.featurestore.api.v1.JoinType\"0\n\x0bVersionedId\x12\n\n\x02id\x18\x01 \x01(\t\x12\x15\n\rmajor_version\x18\x02 \x01(\r\"\xec\x01\n\x0eTransformation\x12>\n\x04mojo\x18\x02 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.MojoTransformationH\x00\x12Q\n\x0espark_pipeline\x18\x03 \x01(\x0b\x32\x37.ai.h2o.featurestore.api.v1.SparkPipelineTransformationH\x00\x12>\n\x04join\x18\x04 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.JoinTransformationH\x00\x42\x07\n\x05value\"\x9a\x01\n\x12\x44\x65rivedInformation\x12@\n\x0f\x66\x65\x61ture_set_ids\x18\x01 \x03(\x0b\x32\'.ai.h2o.featurestore.api.v1.VersionedId\x12\x42\n\x0etransformation\x18\x02 \x01(\x0b\x32*.ai.h2o.featurestore.api.v1.Transformation\"J\n\x0fSelectedFeature\x12\x0e\n\x06prefix\x18\x01 \x01(\t\x12\x0f\n\x07\x66\x65\x61ture\x18\x02 \x01(\t\x12\x16\n\x0etransformation\x18\x03 \x01(\t\"\xa1\x01\n\x14\x46ilterConditionUnion\x12;\n\x06\x66ilter\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureFilterH\x00\x12?\n\x05logic\x18\x02 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.FeatureFilterLogicH\x00\x42\x0b\n\tcondition\"\xa1\x01\n\rFeatureFilter\x12<\n\x07\x66\x65\x61ture\x18\x01 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.SelectedFeature\x12\x43\n\x08operator\x18\x02 \x01(\x0e\x32\x31.ai.h2o.featurestore.api.v1.FeatureFilterOperator\x12\r\n\x05value\x18\x03 \x01(\t\"\xe5\x01\n\x12\x46\x65\x61tureFilterLogic\x12>\n\x04left\x18\x01 \x01(\x0b\x32\x30.ai.h2o.featurestore.api.v1.FilterConditionUnion\x12?\n\x05right\x18\x02 \x01(\x0b\x32\x30.ai.h2o.featurestore.api.v1.FilterConditionUnion\x12N\n\x0elogic_operator\x18\x03 \x01(\x0e\x32\x36.ai.h2o.featurestore.api.v1.FeatureFilterLogicOperator\"\xc8\x05\n\x0c\x46\x65\x61tureQuery\x12\x46\n\x11selected_features\x18\x01 \x03(\x0b\x32+.ai.h2o.featurestore.api.v1.SelectedFeature\x12G\n\x10\x66rom_feature_set\x18\x02 \x01(\x0b\x32-.ai.h2o.featurestore.api.v1.FeatureQuery.From\x12;\n\x04join\x18\x03 \x03(\x0b\x32-.ai.h2o.featurestore.api.v1.FeatureQuery.Join\x12?\n\x05where\x18\x04 \x01(\x0b\x32\x30.ai.h2o.featurestore.api.v1.FilterConditionUnion\x1aS\n\x04\x46rom\x12<\n\x0b\x66\x65\x61ture_set\x18\x01 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.VersionedId\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x1a\xd3\x02\n\x04Join\x12<\n\x0b\x66\x65\x61ture_set\x18\x01 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.VersionedId\x12\r\n\x05\x61lias\x18\x02 \x01(\t\x12<\n\x02on\x18\x03 \x03(\x0b\x32\x30.ai.h2o.featurestore.api.v1.FeatureQuery.Join.On\x12\x43\n\tjoin_type\x18\x04 \x01(\x0e\x32\x30.ai.h2o.featurestore.api.v1.FeatureQueryJoinType\x1a{\n\x02On\x12\x39\n\x04left\x18\x01 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.SelectedFeature\x12:\n\x05right\x18\x02 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.SelectedFeature\"\x9a\x01\n\x0b\x46\x65\x61tureView\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\x05\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x12\n\nproject_id\x18\x05 \x01(\t\x12\x37\n\x05query\x18\x06 \x01(\x0b\x32(.ai.h2o.featurestore.api.v1.FeatureQuery\"\x8a\x01\n\x18\x43reateFeatureViewRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x12\n\nproject_id\x18\x03 \x01(\t\x12\x37\n\x05query\x18\x04 \x01(\x0b\x32(.ai.h2o.featurestore.api.v1.FeatureQuery\"f\n\x18UpdateFeatureViewRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\"\x94\x01\n\"CreateFeatureViewNewVersionRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\x12\x37\n\x05query\x18\x03 \x01(\x0b\x32(.ai.h2o.featurestore.api.v1.FeatureQuery\"J\n\x15GetFeatureViewRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\x05\"T\n\x13\x46\x65\x61tureViewResponse\x12=\n\x0c\x66\x65\x61ture_view\x18\x01 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.FeatureView\"-\n\x17ListFeatureViewsRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\"Z\n\x18ListFeatureViewsResponse\x12>\n\rfeature_views\x18\x01 \x03(\x0b\x32\'.ai.h2o.featurestore.api.v1.FeatureView\"\xc8\x01\n!RetrieveFeatureViewAsSparkRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\x12,\n\x08start_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x65nd_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nsession_id\x18\x05 \x01(\t\"\xa6\x02\n\"RetrieveFeatureViewAsSparkResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\\\n\x07options\x18\x02 \x03(\x0b\x32K.ai.h2o.featurestore.api.v1.RetrieveFeatureViewAsSparkResponse.OptionsEntry\x12\x12\n\nsession_id\x18\x04 \x01(\t\x12P\n\x16offline_storage_format\x18\x05 \x01(\x0e\x32\x30.ai.h2o.featurestore.api.v1.OfflineStorageFormat\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb6\x01\n#RetrieveFeatureViewAsAsLinksRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\x12,\n\x08start_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x06\x65nd_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\">\n$RetrieveFeatureViewAsAsLinksResponse\x12\x16\n\x0e\x64ownload_links\x18\x01 \x03(\t\"3\n\x18\x44\x65leteFeatureViewRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\"\x8f\x03\n\x10MLDatasetFeature\x12\x12\n\nfeature_id\x18\x01 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x03 \x01(\x05\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x04 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x05 \x01(\x05\x12\x11\n\tdata_type\x18\x06 \x01(\t\x12=\n\x0c\x66\x65\x61ture_type\x18\x07 \x01(\x0e\x32\'.ai.h2o.featurestore.api.v1.FeatureType\x12\x15\n\rml_dataset_id\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12\x15\n\roriginal_name\x18\n \x01(\t\x12\x12\n\nproject_id\x18\x0b \x01(\t\x12\x1a\n\x12original_data_type\x18\x0c \x01(\t\x12\x1f\n\x17transformation_function\x18\r \x01(\t\x12\x16\n\x0eis_primary_key\x18\x0e \x01(\x08\"\xf6\x03\n\tMLDataset\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x33\n\x0fstart_date_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_date_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x06 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x07 \x01(\x05\x12\x12\n\nproject_id\x18\x08 \x01(\t\x12>\n\x08\x66\x65\x61tures\x18\t \x03(\x0b\x32,.ai.h2o.featurestore.api.v1.MLDatasetFeature\x12\x43\n\x05state\x18\n \x01(\x0e\x32\x34.ai.h2o.featurestore.api.v1.MLDataset.MLDatasetState\x12\x14\n\x0cprimary_keys\x18\x0b \x03(\t\"l\n\x0eMLDatasetState\x12\x1c\n\x18ML_DATASET_STATE_UNKNOWN\x10\x00\x12\x1c\n\x18ML_DATASET_STATE_PENDING\x10\x01\x12\x1e\n\x1aML_DATASET_STATE_AVAILABLE\x10\x02\"\xda\x01\n\x16\x43reateMLDatasetRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x33\n\x0fstart_date_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_date_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"D\n\x16UpdateMLDatasetRequest\x12\x15\n\rml_dataset_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\"/\n\x16\x44\x65leteMLDatasetRequest\x12\x15\n\rml_dataset_id\x18\x01 \x01(\t\"\x84\x01\n\x17\x43reateMLDatasetResponse\x12\x39\n\nml_dataset\x18\x01 \x01(\x0b\x32%.ai.h2o.featurestore.api.v1.MLDataset\x12.\n\x03job\x18\x02 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.JobId\"e\n\x13GetMLDatasetRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\x12\x17\n\x0fml_dataset_name\x18\x03 \x01(\t\"N\n\x15ListMLDatasetsRequest\x12\x17\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\t\x12\x1c\n\x14\x66\x65\x61ture_view_version\x18\x02 \x01(\x05\"T\n\x16ListMLDatasetsResponse\x12:\n\x0bml_datasets\x18\x01 \x03(\x0b\x32%.ai.h2o.featurestore.api.v1.MLDataset\"L\n\x1fRetrieveMLDatasetAsSparkRequest\x12\x15\n\rml_dataset_id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\"\xa2\x02\n RetrieveMLDatasetAsSparkResponse\x12\x0c\n\x04path\x18\x01 \x01(\t\x12Z\n\x07options\x18\x02 \x03(\x0b\x32I.ai.h2o.featurestore.api.v1.RetrieveMLDatasetAsSparkResponse.OptionsEntry\x12\x12\n\nsession_id\x18\x04 \x01(\t\x12P\n\x16offline_storage_format\x18\x05 \x01(\x0e\x32\x30.ai.h2o.featurestore.api.v1.OfflineStorageFormat\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\":\n!RetrieveMLDatasetAsAsLinksRequest\x12\x15\n\rml_dataset_id\x18\x01 \x01(\t\"<\n\"RetrieveMLDatasetAsAsLinksResponse\x12\x16\n\x0e\x64ownload_links\x18\x01 \x03(\t\"\xbd\x0f\n\nFeatureSet\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\x12\x16\n\x0eversion_change\x18\x05 \x01(\t\x12\x1a\n\x12time_travel_column\x18\x06 \x01(\t\x12!\n\x19time_travel_column_format\x18\x07 \x01(\t\x12\x44\n\x10\x66\x65\x61ture_set_type\x18\x08 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.FeatureSetType\x12\x13\n\x0b\x64\x65scription\x18\t \x01(\t\x12\x39\n\x06\x61uthor\x18\x0b \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x35\n\x11\x63reated_date_time\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15last_update_date_time\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x61pplication_name\x18\x0e \x01(\t\x12\x12\n\ndeprecated\x18\x0f \x01(\x08\x12\x33\n\x0f\x64\x65precated_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13\x64\x61ta_source_domains\x18\x11 \x03(\t\x12\x0c\n\x04tags\x18\x12 \x03(\t\x12\x18\n\x10process_interval\x18\x13 \x01(\r\x12N\n\x15process_interval_unit\x18\x14 \x01(\x0e\x32/.ai.h2o.featurestore.api.v1.ProcessIntervalUnit\x12\x0c\n\x04\x66low\x18\x15 \x01(\t\x12<\n\x0ctime_to_live\x18\x16 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.TimeToLive\x12\x35\n\x08\x66\x65\x61tures\x18\x17 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\x12\x45\n\nstatistics\x18\x18 \x01(\x0b\x32\x31.ai.h2o.featurestore.api.v1.FeatureSet.Statistics\x12H\n\x0cspecial_data\x18\x19 \x01(\x0b\x32\x32.ai.h2o.featurestore.api.v1.FeatureSet.SpecialData\x12\x13\n\x0bprimary_key\x18\x1a \x03(\t\x12\n\n\x02id\x18\x1c \x01(\t\x12<\n\x11time_travel_scope\x18\x1d \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x16\n\x0e\x61pplication_id\x18\x1e \x01(\t\x12\x19\n\x11\x66\x65\x61ture_set_state\x18\x1f \x01(\t\x12=\n\x06online\x18  \x01(\x0b\x32-.ai.h2o.featurestore.api.v1.FeatureSet.Online\x12\x0e\n\x06secret\x18! \x01(\x08\x12\x12\n\nproject_id\x18\" \x01(\t\x12\x14\n\x0cpartition_by\x18# \x03(\t\x12,\n\x0b\x63ustom_data\x18$ \x01(\x0b\x32\x17.google.protobuf.Struct\x12G\n\x1conline_materialization_scope\x18% \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x44\n\x0c\x64\x65rived_from\x18& \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\x12\x1b\n\x13\x66\x65\x61ture_classifiers\x18\' \x03(\t\x12\x42\n\x0flast_updated_by\x18( \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12M\n\x14storage_optimization\x18) \x01(\x0b\x32/.ai.h2o.featurestore.api.v1.StorageOptimization\x1a\x39\n\nStatistics\x12\x14\n\x0c\x64\x61ta_latency\x18\x01 \x01(\x05\x12\x15\n\rrecords_count\x18\x02 \x01(\x03\x1a\x82\x02\n\x0bSpecialData\x12\x0b\n\x03spi\x18\x01 \x01(\x08\x12\x0b\n\x03pci\x18\x02 \x01(\x08\x12\x0b\n\x03rpi\x18\x03 \x01(\x08\x12\x13\n\x0b\x64\x65mographic\x18\x04 \x01(\x08\x12\x11\n\tsensitive\x18\x05 \x01(\x08\x12G\n\x05legal\x18\x06 \x01(\x0b\x32\x38.ai.h2o.featurestore.api.v1.FeatureSet.SpecialData.Legal\x1a[\n\x05Legal\x12\x10\n\x08\x61pproved\x18\x01 \x01(\x08\x12\x31\n\rapproved_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05notes\x18\x03 \x01(\t\x1aJ\n\x06Online\x12\x18\n\x10online_namespace\x18\x01 \x01(\t\x12\x17\n\x0f\x63onnection_type\x18\x02 \x01(\t\x12\r\n\x05topic\x18\x03 \x01(\tJ\x04\x08\n\x10\x0b\"R\n\x1bGetFeatureSetPreviewRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"I\n\x1cGetFeatureSetPreviewResponse\x12\x13\n\x0bpreview_url\x18\x01 \x01(\t\x12\x14\n\x0cmax_cols_num\x18\x02 \x01(\r\"o\n\x05Scope\x12\x33\n\x0fstart_date_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_date_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xcf\x07\n\x19RegisterFeatureSetRequest\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x01 \x01(\t\x12\x34\n\x07project\x18\x02 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\x12\x1a\n\x12time_travel_column\x18\x03 \x01(\t\x12!\n\x19time_travel_column_format\x18\x04 \x01(\t\x12\x13\n\x0bprimary_key\x18\x05 \x03(\t\x12\x39\n\x06schema\x18\x07 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12\x0e\n\x06secret\x18\x08 \x01(\x08\x12\x13\n\x0b\x64\x65scription\x18\t \x01(\t\x12\x14\n\x0cpartition_by\x18\n \x03(\t\x12\'\n\x1ftime_travel_column_as_partition\x18\x0b \x01(\x08\x12\x44\n\x10\x66\x65\x61ture_set_type\x18\x0c \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.FeatureSetType\x12\x19\n\x11\x66\x65\x61ture_set_state\x18\r \x01(\t\x12\x18\n\x10\x61pplication_name\x18\x0e \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x0f \x01(\t\x12=\n\x06online\x18\x10 \x01(\x0b\x32-.ai.h2o.featurestore.api.v1.FeatureSet.Online\x12\x1b\n\x13\x64\x61ta_source_domains\x18\x11 \x03(\t\x12\x0c\n\x04tags\x18\x12 \x03(\t\x12\x18\n\x10process_interval\x18\x13 \x01(\r\x12N\n\x15process_interval_unit\x18\x14 \x01(\x0e\x32/.ai.h2o.featurestore.api.v1.ProcessIntervalUnit\x12\x0c\n\x04\x66low\x18\x15 \x01(\t\x12H\n\x0cspecial_data\x18\x16 \x01(\x0b\x32\x32.ai.h2o.featurestore.api.v1.FeatureSet.SpecialData\x12,\n\x0b\x63ustom_data\x18\x17 \x01(\x0b\x32\x17.google.protobuf.Struct\x12<\n\x0ctime_to_live\x18\x18 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.TimeToLive\x12\x44\n\x0c\x64\x65rived_from\x18\x19 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\"\xb4\x05\n!CreateNewFeatureSetVersionRequest\x12\x39\n\x06schema\x18\x02 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12\x19\n\x11\x61\x66\x66\x65\x63ted_features\x18\x03 \x03(\t\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x44\n\x0c\x64\x65rived_from\x18\x05 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\x12\x13\n\x0bprimary_key\x18\x06 \x03(\t\x12-\n%use_primary_key_from_previous_version\x18\x07 \x01(\x08\x12\x45\n\x10\x62\x61\x63kfill_options\x18\x08 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.BackfillOptions\x12\x14\n\x0cpartition_by\x18\t \x03(\t\x12.\n&use_partition_by_from_previous_version\x18\n \x01(\x08\x12+\n#use_time_travel_column_as_partition\x18\x0b \x01(\x08\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x0c \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\r \x01(\t\x12\x1a\n\x12time_travel_column\x18\x0e \x01(\t\x12!\n\x19time_travel_column_format\x18\x0f \x01(\t\x12\x34\n,use_time_travel_column_from_previous_version\x18\x10 \x01(\x08\x12;\n3use_time_travel_column_format_from_previous_version\x18\x11 \x01(\x08\"\xff\x01\n\x0e\x46\x65\x61tureProfile\x12=\n\x0c\x66\x65\x61ture_type\x18\x01 \x01(\x0e\x32\'.ai.h2o.featurestore.api.v1.FeatureType\x12M\n\x0b\x63\x61tegorical\x18\x02 \x01(\x0b\x32\x38.ai.h2o.featurestore.api.v1.CategoricalFeatureStatistics\x12\x41\n\nstatistics\x18\x03 \x01(\x0b\x32-.ai.h2o.featurestore.api.v1.FeatureStatistics\x12\x1c\n\x14statistics_available\x18\x04 \x01(\x08\"\xa0\x04\n\rFeatureSchema\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tdata_type\x18\x02 \x01(\t\x12\x39\n\x06nested\x18\x03 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.FeatureSchema\x12K\n\x0cspecial_data\x18\x04 \x01(\x0b\x32\x35.ai.h2o.featurestore.api.v1.FeatureSchema.SpecialData\x12=\n\x0c\x66\x65\x61ture_type\x18\x05 \x01(\x0e\x32\'.ai.h2o.featurestore.api.v1.FeatureType\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x13\n\x0b\x63lassifiers\x18\x07 \x03(\t\x12,\n\x0b\x63ustom_data\x18\x08 \x01(\x0b\x32\x17.google.protobuf.Struct\x12H\n\nmonitoring\x18\t \x01(\x0b\x32\x34.ai.h2o.featurestore.api.v1.FeatureSchema.Monitoring\x1a\\\n\x0bSpecialData\x12\x0b\n\x03spi\x18\x01 \x01(\x08\x12\x0b\n\x03pci\x18\x02 \x01(\x08\x12\x0b\n\x03rpi\x18\x03 \x01(\x08\x12\x13\n\x0b\x64\x65mographic\x18\x04 \x01(\x08\x12\x11\n\tsensitive\x18\x05 \x01(\x08\x1a\'\n\nMonitoring\x12\x19\n\x11\x61nomaly_detection\x18\x01 \x01(\x08\"\x91\x05\n\x07\x46\x65\x61ture\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x16\n\x0eversion_change\x18\x03 \x01(\t\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x11\n\tdata_type\x18\x05 \x01(\t\x12;\n\x07profile\x18\x06 \x01(\x0b\x32*.ai.h2o.featurestore.api.v1.FeatureProfile\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x12\n\nimportance\x18\x08 \x01(\x01\x12\x0f\n\x07special\x18\t \x01(\t\x12\x42\n\nmonitoring\x18\n \x01(\x0b\x32..ai.h2o.featurestore.api.v1.Feature.Monitoring\x12<\n\x0fnested_features\x18\x0b \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\x12\x45\n\x0cspecial_data\x18\r \x01(\x0b\x32/.ai.h2o.featurestore.api.v1.Feature.SpecialData\x12\x13\n\x0b\x63lassifiers\x18\x0e \x03(\t\x12,\n\x0b\x63ustom_data\x18\x0f \x01(\x0b\x32\x17.google.protobuf.Struct\x12\n\n\x02id\x18\x10 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x11 \x01(\t\x1a\'\n\nMonitoring\x12\x19\n\x11\x61nomaly_detection\x18\x01 \x01(\x08\x1a\\\n\x0bSpecialData\x12\x0b\n\x03spi\x18\x01 \x01(\x08\x12\x0b\n\x03pci\x18\x02 \x01(\x08\x12\x0b\n\x03rpi\x18\x03 \x01(\x08\x12\x13\n\x0b\x64\x65mographic\x18\x04 \x01(\x08\x12\x11\n\tsensitive\x18\x05 \x01(\x08\"\xac\x01\n\x11\x46\x65\x61tureStatistics\x12\x0b\n\x03max\x18\x01 \x01(\x01\x12\x0c\n\x04mean\x18\x02 \x01(\x01\x12\x0e\n\x06median\x18\x03 \x01(\x01\x12\x0b\n\x03min\x18\x04 \x01(\x01\x12\x0e\n\x06stddev\x18\x05 \x01(\x01\x12\x18\n\x10stddev_rec_count\x18\x06 \x01(\x03\x12\x12\n\nnull_count\x18\x07 \x01(\x03\x12\x11\n\tnan_count\x18\x08 \x01(\x03\x12\x0e\n\x06unique\x18\t \x01(\x03\"\xab\x01\n\x1c\x43\x61tegoricalFeatureStatistics\x12\x0e\n\x06unique\x18\x01 \x01(\x03\x12P\n\x03top\x18\x02 \x03(\x0b\x32\x43.ai.h2o.featurestore.api.v1.CategoricalFeatureStatistics.FeatureTop\x1a)\n\nFeatureTop\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x63ount\x18\x02 \x01(\x03\"%\n\x12GetVersionResponse\x12\x0f\n\x07version\x18\x01 \x01(\t\"\\\n\x14GetApiConfigResponse\x12 \n\x18public_core_rest_api_url\x18\x01 \x01(\t\x12\"\n\x1apublic_online_rest_api_url\x18\x02 \x01(\t\"(\n\x15GetGpteConfigResponse\x12\x0f\n\x07\x61pi_key\x18\x01 \x01(\t\"\x99\x03\n\x07Project\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x39\n\x06\x61uthor\x18\x04 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x35\n\x11\x63reated_date_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15last_update_date_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06secret\x18\x07 \x01(\x08\x12\x0e\n\x06locked\x18\x08 \x01(\x08\x12\n\n\x02id\x18\t \x01(\t\x12,\n\x0b\x63ustom_data\x18\n \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x1a\n\x12\x66\x65\x61ture_sets_count\x18\x0b \x01(\x04\x12\x42\n\x0flast_updated_by\x18\x0c \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfoJ\x04\x08\x03\x10\x04\"\xa4\x02\n\x0fListableProject\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x39\n\x15last_update_date_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06locked\x18\x05 \x01(\x08\x12@\n\npermission\x18\x06 \x01(\x0e\x32,.ai.h2o.featurestore.api.v1.ActivePermission\x12\x39\n\x06\x61uthor\x18\x07 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x1a\n\x12\x66\x65\x61ture_sets_count\x18\x08 \x01(\x04\"\xf6\x02\n\x10\x46\x65\x61tureSetIngest\x12\x11\n\tingest_id\x18\x01 \x01(\t\x12\x34\n\x10ingest_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x06source\x18\x03 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocation\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x05 \x01(\t\x12\x30\n\x05scope\x18\x07 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x16\n\x0eparent_ingests\x18\x08 \x03(\t\x12\x1e\n\x16ingested_records_count\x18\t \x01(\t\x12=\n\nstarted_by\x18\n \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\"\xd7\x01\n\x13PersonalAccessToken\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12-\n\tlast_used\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rcreation_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x65xpiry_date\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x88\x01\n#GenerateTransformationUploadRequest\x12K\n\x13transformation_type\x18\x01 \x01(\x0e\x32..ai.h2o.featurestore.api.v1.TransformationType\x12\x14\n\x0cmd5_checksum\x18\x02 \x01(\t\"\xd5\x01\n$GenerateTransformationUploadResponse\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x0b\n\x03url\x18\x02 \x01(\t\x12^\n\x07headers\x18\x03 \x03(\x0b\x32M.ai.h2o.featurestore.api.v1.GenerateTransformationUploadResponse.HeadersEntry\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"@\n\x17ListProjectsPageRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\"j\n\x18ListProjectsPageResponse\x12\x35\n\x08projects\x18\x01 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Project\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xa0\x04\n\x14ProjectSearchRequest\x12\r\n\x05query\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12I\n\x13required_permission\x18\x04 \x01(\x0e\x32,.ai.h2o.featurestore.api.v1.ActivePermission\x12\x13\n\x0bproject_ids\x18\x05 \x03(\t\x12U\n\nsort_field\x18\x06 \x01(\x0e\x32\x41.ai.h2o.featurestore.api.v1.ProjectSearchRequest.ProjectSortField\x12\x41\n\x0esort_direction\x18\x07 \x01(\x0e\x32).ai.h2o.featurestore.api.v1.SortDirection\"\xd7\x01\n\x10ProjectSortField\x12 \n\x1cPROJECT_SORT_FIELD_UNDEFINED\x10\x00\x12\x1b\n\x17PROJECT_SORT_FIELD_NAME\x10\x01\x12\"\n\x1ePROJECT_SORT_FIELD_DESCRIPTION\x10\x02\x12\x1d\n\x19PROJECT_SORT_FIELD_LOCKED\x10\x03\x12\x1d\n\x19PROJECT_SORT_FIELD_AUTHOR\x10\x04\x12\"\n\x1ePROJECT_SORT_FIELD_LAST_UPDATE\x10\x05\"\xd6\x04\n\x17\x46\x65\x61tureSetSearchRequest\x12\r\n\x05query\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x12\n\nowned_only\x18\x04 \x01(\x08\x12\x13\n\x0bproject_ids\x18\x05 \x03(\t\x12[\n\nsort_field\x18\x06 \x01(\x0e\x32G.ai.h2o.featurestore.api.v1.FeatureSetSearchRequest.FeatureSetSortField\x12\x41\n\x0esort_direction\x18\x07 \x01(\x0e\x32).ai.h2o.featurestore.api.v1.SortDirection\x12\x41\n\x07options\x18\x08 \x03(\x0b\x32\x30.ai.h2o.featurestore.api.v1.AdvancedSearchOption\"\xf8\x01\n\x13\x46\x65\x61tureSetSortField\x12$\n FEATURE_SET_SORT_FIELD_UNDEFINED\x10\x00\x12\x1f\n\x1b\x46\x45\x41TURE_SET_SORT_FIELD_NAME\x10\x01\x12&\n\"FEATURE_SET_SORT_FIELD_DESCRIPTION\x10\x02\x12!\n\x1d\x46\x45\x41TURE_SET_SORT_FIELD_AUTHOR\x10\x03\x12&\n\"FEATURE_SET_SORT_FIELD_LAST_UPDATE\x10\x04\x12\'\n#FEATURE_SET_SORT_FIELD_PROJECT_NAME\x10\x05\"\x86\x03\n\x14\x46\x65\x61tureSearchRequest\x12\r\n\x05query\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x12\n\nowned_only\x18\x04 \x01(\x08\x12\x13\n\x0bproject_ids\x18\x05 \x03(\t\x12U\n\nsort_field\x18\x06 \x01(\x0e\x32\x41.ai.h2o.featurestore.api.v1.FeatureSearchRequest.FeatureSortField\x12\x41\n\x0esort_direction\x18\x07 \x01(\x0e\x32).ai.h2o.featurestore.api.v1.SortDirection\"u\n\x10\x46\x65\x61tureSortField\x12 \n\x1c\x46\x45\x41TURE_SORT_FIELD_UNDEFINED\x10\x00\x12\x1b\n\x17\x46\x45\x41TURE_SORT_FIELD_NAME\x10\x01\x12\"\n\x1e\x46\x45\x41TURE_SORT_FIELD_DESCRIPTION\x10\x02\"v\n\x14ProjectSearchResults\x12\x45\n\x10listable_project\x18\x01 \x03(\x0b\x32+.ai.h2o.featurestore.api.v1.ListableProject\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xfa\x0c\n\x12ListableFeatureSet\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0cproject_name\x18\x04 \x01(\t\x12\x39\n\x15last_update_date_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07version\x18\x06 \x01(\t\x12@\n\npermission\x18\x07 \x01(\x0e\x32,.ai.h2o.featurestore.api.v1.ActivePermission\x12\x12\n\nproject_id\x18\x08 \x01(\t\x12\x16\n\x0eversion_change\x18\t \x01(\t\x12\x1a\n\x12time_travel_column\x18\n \x01(\t\x12!\n\x19time_travel_column_format\x18\x0b \x01(\t\x12\x44\n\x10\x66\x65\x61ture_set_type\x18\x0c \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.FeatureSetType\x12\x39\n\x06\x61uthor\x18\r \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x35\n\x11\x63reated_date_time\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ndeprecated\x18\x0f \x01(\x08\x12\x33\n\x0f\x64\x65precated_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04tags\x18\x11 \x03(\t\x12<\n\x0ctime_to_live\x18\x12 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.TimeToLive\x12H\n\x0cspecial_data\x18\x13 \x01(\x0b\x32\x32.ai.h2o.featurestore.api.v1.FeatureSet.SpecialData\x12\x13\n\x0bprimary_key\x18\x14 \x03(\t\x12<\n\x11time_travel_scope\x18\x15 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x0e\n\x06secret\x18\x16 \x01(\x08\x12\x14\n\x0cpartition_by\x18\x17 \x03(\t\x12G\n\x1conline_materialization_scope\x18\x18 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.Scope\x12\x44\n\x0c\x64\x65rived_from\x18\x19 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\x12\x1b\n\x13\x66\x65\x61ture_classifiers\x18\x1a \x03(\t\x12\x15\n\rrecords_count\x18\x1b \x01(\x04\x12\x38\n\x04\x66low\x18\x1c \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.FeatureSetFlow\x12\x18\n\x10\x61pplication_name\x18\x1d \x01(\t\x12\x1b\n\x13\x64\x61ta_source_domains\x18\x1e \x03(\t\x12\x18\n\x10process_interval\x18\x1f \x01(\r\x12N\n\x15process_interval_unit\x18  \x01(\x0e\x32/.ai.h2o.featurestore.api.v1.ProcessIntervalUnit\x12\x45\n\nstatistics\x18! \x01(\x0b\x32\x31.ai.h2o.featurestore.api.v1.FeatureSet.Statistics\x12\x16\n\x0e\x61pplication_id\x18\" \x01(\t\x12\x19\n\x11\x66\x65\x61ture_set_state\x18# \x01(\t\x12=\n\x06online\x18$ \x01(\x0b\x32-.ai.h2o.featurestore.api.v1.FeatureSet.Online\x12,\n\x0b\x63ustom_data\x18% \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x42\n\x0flast_updated_by\x18& \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12M\n\x14storage_optimization\x18\' \x01(\x0b\x32/.ai.h2o.featurestore.api.v1.StorageOptimization\"\x80\x01\n\x17\x46\x65\x61tureSetSearchResults\x12L\n\x14listable_feature_set\x18\x01 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.ListableFeatureSet\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xde\x01\n\x0fListableFeature\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x19\n\x11\x61nomaly_detection\x18\x04 \x01(\x08\x12=\n\x0c\x66\x65\x61ture_type\x18\x05 \x01(\x0e\x32\'.ai.h2o.featurestore.api.v1.FeatureType\x12\x11\n\tdata_type\x18\x06 \x01(\t\x12\x0f\n\x07version\x18\x07 \x01(\t\x12\x12\n\nfeature_id\x18\x08 \x01(\t\"v\n\x14\x46\x65\x61tureSearchResults\x12\x45\n\x10listable_feature\x18\x01 \x03(\x0b\x32+.ai.h2o.featurestore.api.v1.ListableFeature\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"J\n\x13\x46\x65\x61tureSetRequestId\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"\\\n\x11GetFeatureRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\x12\x12\n\nfeature_id\x18\x03 \x01(\t\"j\n\x18ListFeaturesPageResponse\x12\x35\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"G\n\x0f\x46\x65\x61tureResponse\x12\x34\n\x07\x66\x65\x61ture\x18\x01 \x01(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\"\x80\x01\n\x13ListFeaturesRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x05 \x01(\t\"f\n\x14ListFeaturesResponse\x12\x35\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"P\n\x19ListableFeatureSetRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"j\n\x1aListableFeatureSetResponse\x12L\n\x14listable_feature_set\x18\x01 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.ListableFeatureSet\"Z\n\x1d\x46\x65\x61tureSetsDerivedFromRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x02 \x01(\t\"o\n\x1e\x46\x65\x61tureSetsDerivedFromResponse\x12M\n\x15listable_feature_sets\x18\x01 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.ListableFeatureSet\"\x85\x01\n\x1eSubmitPendingPermissionRequest\x12\x13\n\x0bresource_id\x18\x01 \x01(\t\x12>\n\npermission\x18\x02 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12\x0e\n\x06reason\x18\x03 \x01(\t\"8\n\x1fSubmitPendingPermissionResponse\x12\x15\n\rpermission_id\x18\x01 \x01(\t\"\x96\x01\n\x1aListPermissionsPageRequest\x12<\n\x07\x66ilters\x18\x01 \x03(\x0e\x32+.ai.h2o.featurestore.api.v1.PermissionState\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x13\n\x0bresource_id\x18\x04 \x01(\t\"\x88\x01\n#ListProjectsPermissionsPageResponse\x12H\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\x37.ai.h2o.featurestore.api.v1.ListableProjectToPermission\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x8e\x01\n&ListFeatureSetsPermissionsPageResponse\x12K\n\x07\x65ntries\x18\x01 \x03(\x0b\x32:.ai.h2o.featurestore.api.v1.ListableFeatureSetToPermission\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x97\x01\n\x1bListableProjectToPermission\x12<\n\x07project\x18\x01 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.ListableProject\x12:\n\npermission\x18\x02 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.Permission\"\xa1\x01\n\x1eListableFeatureSetToPermission\x12\x43\n\x0b\x66\x65\x61ture_set\x18\x01 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.ListableFeatureSet\x12:\n\npermission\x18\x02 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.Permission\"\xec\x08\n\nPermission\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bresource_id\x18\x02 \x01(\t\x12?\n\rresource_type\x18\x03 \x01(\x0e\x32(.ai.h2o.featurestore.api.v1.ResourceType\x12>\n\npermission\x18\x04 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.PermissionType\x12\x37\n\x04user\x18\x05 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x17\n\x0f\x63reation_reason\x18\x06 \x01(\t\x12:\n\x05state\x18\x07 \x01(\x0e\x32+.ai.h2o.featurestore.api.v1.PermissionState\x12.\n\ncreated_on\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0elast_update_on\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\n \x01(\x08\x12[\n\x13granted_or_rejected\x18\x0b \x01(\x0b\x32>.ai.h2o.featurestore.api.v1.Permission.GrantedOrRejectedUpdate\x12\x45\n\x07revoked\x18\x0c \x01(\x0b\x32\x34.ai.h2o.featurestore.api.v1.Permission.RevokedUpdate\x12G\n\x08promoted\x18\r \x01(\x0b\x32\x35.ai.h2o.featurestore.api.v1.Permission.PromotedUpdate\x1a\xac\x01\n\x0ePromotedUpdate\x12\x37\n\x04user\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12.\n\nupdated_on\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06reason\x18\x03 \x01(\t\x12!\n\x19replaced_by_permission_id\x18\x04 \x01(\t\x1a\x88\x01\n\rRevokedUpdate\x12\x37\n\x04user\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12.\n\nupdated_on\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06reason\x18\x03 \x01(\t\x1a\x92\x01\n\x17GrantedOrRejectedUpdate\x12\x37\n\x04user\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12.\n\nupdated_on\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06reason\x18\x03 \x01(\t\"@\n\x17RevokePermissionRequest\x12\x15\n\rpermission_id\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"H\n\x1f\x41pprovePendingPermissionRequest\x12\x15\n\rpermission_id\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"G\n\x1eRejectPendingPermissionRequest\x12\x15\n\rpermission_id\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\"9\n WithdrawPendingPermissionRequest\x12\x15\n\rpermission_id\x18\x01 \x01(\t\"1\n\x1aGetActivePermissionRequest\x12\x13\n\x0bresource_id\x18\x01 \x01(\t\"\xa0\x01\n\x1bGetActivePermissionResponse\x12@\n\npermission\x18\x01 \x01(\x0e\x32,.ai.h2o.featurestore.api.v1.ActivePermission\x12?\n\rresource_type\x18\x02 \x01(\x0e\x32(.ai.h2o.featurestore.api.v1.ResourceType\"\xcf\x04\n\rScheduledTask\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\x12\x12\n\nproject_id\x18\x05 \x01(\t\x12;\n\x06source\x18\x06 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocation\x12\x10\n\x08schedule\x18\x07 \x01(\t\x12\x31\n\rnext_run_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tlast_exec\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x05owner\x18\n \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12\x35\n\x11\x63reated_date_time\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x15last_update_date_time\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x37\n\ttask_type\x18\r \x01(\x0e\x32$.ai.h2o.featurestore.api.v1.TaskType\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x0e \x01(\t\x12\x16\n\x0e\x63ron_time_zone\x18\x0f \x01(\t\x12\x18\n\x10\x61llowed_failures\x18\x10 \x01(\x05\"\xb9\x02\n\x13ScheduleTaskRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x12\n\nproject_id\x18\x04 \x01(\t\x12\x35\n\x04\x63red\x18\x05 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.Credentials\x12;\n\x06source\x18\x06 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocation\x12\x10\n\x08schedule\x18\x07 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x08 \x01(\t\x12\x16\n\x0e\x63ron_time_zone\x18\t \x01(\t\x12\x18\n\x10\x61llowed_failures\x18\n \x01(\x05\"Z\n\x19ListScheduledTasksRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"o\n\x1aListScheduledTasksResponse\x12\x38\n\x05tasks\x18\x01 \x03(\x0b\x32).ai.h2o.featurestore.api.v1.ScheduledTask\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\",\n\x0fScheduledTaskId\x12\x19\n\x11scheduled_task_id\x18\x01 \x01(\t\"P\n\x15ScheduledTaskResponse\x12\x37\n\x04task\x18\x01 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.ScheduledTask\"v\n\x1aScheduledTaskUpdateRequest\x12\x19\n\x11scheduled_task_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x10\n\x08schedule\x18\x03 \x01(\t\x12\x16\n\x0eupdated_fields\x18\x04 \x03(\t\"6\n\x19PauseScheduledTaskRequest\x12\x19\n\x11scheduled_task_id\x18\x01 \x01(\t\"i\n\x1aResumeScheduledTaskRequest\x12\x19\n\x11scheduled_task_id\x18\x01 \x01(\t\x12\x16\n\x0esetup_failures\x18\x02 \x01(\x08\x12\x18\n\x10\x61llowed_failures\x18\x03 \x01(\x05\"H\n\x11LazyIngestRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"G\n\x12LazyIngestResponse\x12\x31\n\x06job_id\x18\x01 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.JobId\"O\n\x18GetLazyIngestTaskRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"f\n\"ListScheduledTaskExecutionsRequest\x12\x19\n\x11scheduled_task_id\x18\x01 \x01(\t\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\"\xe9\x01\n\x16ScheduledTaskExecution\x12\x31\n\x06job_id\x18\x01 \x01(\x0b\x32!.ai.h2o.featurestore.api.v1.JobId\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x66inished_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x0c\x66inal_status\x18\x04 \x01(\x0e\x32%.ai.h2o.featurestore.api.v1.JobStatus\"\x8d\x01\n#ListScheduledTaskExecutionsResponse\x12M\n\x11\x65xecution_history\x18\x01 \x03(\x0b\x32\x32.ai.h2o.featurestore.api.v1.ScheduledTaskExecution\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"c\n\x16TransformationFunction\x12\x15\n\rfunction_name\x18\x01 \x01(\t\x12\x1d\n\x15supported_input_types\x18\x02 \x03(\t\x12\x13\n\x0boutput_type\x18\x03 \x01(\t\"$\n\"ListTransformationFunctionsRequest\"{\n#ListTransformationFunctionsResponse\x12T\n\x18transformation_functions\x18\x01 \x03(\x0b\x32\x32.ai.h2o.featurestore.api.v1.TransformationFunction\"H\n GetTransformationFunctionRequest\x12$\n\x1ctransformation_function_name\x18\x01 \x01(\t\"x\n!GetTransformationFunctionResponse\x12S\n\x17transformation_function\x18\x01 \x01(\x0b\x32\x32.ai.h2o.featurestore.api.v1.TransformationFunction\"\xda\x01\n\x14UpdateProjectRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x0e\n\x06locked\x18\x02 \x01(\x08\x12\x0e\n\x06secret\x18\x03 \x01(\x08\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12,\n\x0b\x63ustom_data\x18\x05 \x01(\x0b\x32\x17.google.protobuf.Struct\x12K\n\x10\x66ields_to_update\x18\x06 \x03(\x0e\x32\x31.ai.h2o.featurestore.api.v1.UpdatableProjectField\"\xbc\x07\n\x17UpdateFeatureSetRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\x12\x0c\n\x04tags\x18\x03 \x03(\t\x12\x1b\n\x13\x64\x61ta_source_domains\x18\x04 \x03(\t\x12\x13\n\x0b\x64\x65scription\x18\x05 \x01(\t\x12\x38\n\x04type\x18\x06 \x01(\x0e\x32*.ai.h2o.featurestore.api.v1.FeatureSetType\x12\x12\n\ndeprecated\x18\x07 \x01(\x08\x12\x18\n\x10process_interval\x18\x08 \x01(\x05\x12N\n\x15process_interval_unit\x18\t \x01(\x0e\x32/.ai.h2o.featurestore.api.v1.ProcessIntervalUnit\x12\x0e\n\x06secret\x18\n \x01(\x08\x12%\n\x1dtime_to_live_offline_interval\x18\x0b \x01(\r\x12\x62\n\"time_to_live_offline_interval_unit\x18\x0c \x01(\x0e\x32\x36.ai.h2o.featurestore.api.v1.Offline.TimeToLiveInterval\x12$\n\x1ctime_to_live_online_interval\x18\r \x01(\r\x12`\n!time_to_live_online_interval_unit\x18\x0e \x01(\x0e\x32\x35.ai.h2o.featurestore.api.v1.Online.TimeToLiveInterval\x12\x16\n\x0elegal_approved\x18\x0f \x01(\x08\x12\x1c\n\x14legal_approved_notes\x18\x10 \x01(\t\x12\r\n\x05state\x18\x11 \x01(\t\x12\x0c\n\x04\x66low\x18\x12 \x01(\t\x12\x18\n\x10\x61pplication_name\x18\x13 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x14 \x01(\t\x12,\n\x0b\x63ustom_data\x18\x15 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x18\n\x10online_namespace\x18\x16 \x01(\t\x12\x14\n\x0conline_topic\x18\x17 \x01(\t\x12\x1e\n\x16online_connection_type\x18\x18 \x01(\t\x12N\n\x10\x66ields_to_update\x18\x19 \x03(\x0e\x32\x34.ai.h2o.featurestore.api.v1.UpdatableFeatureSetField\"\x8b\x03\n\x14UpdateFeatureRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\x12\x12\n\nfeature_id\x18\x03 \x01(\t\x12\x0e\n\x06status\x18\x04 \x01(\t\x12\x35\n\x04type\x18\x05 \x01(\x0e\x32\'.ai.h2o.featurestore.api.v1.FeatureType\x12\x12\n\nimportance\x18\x06 \x01(\x01\x12,\n\x0b\x63ustom_data\x18\x07 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12\x0f\n\x07special\x18\t \x01(\t\x12\x19\n\x11\x61nomaly_detection\x18\n \x01(\x08\x12\x13\n\x0b\x63lassifiers\x18\x0b \x03(\t\x12K\n\x10\x66ields_to_update\x18\x0c \x03(\x0e\x32\x31.ai.h2o.featurestore.api.v1.UpdatableFeatureField\"\xe5\x02\n\x0f\x42\x61\x63kfillOptions\x12-\n\tfrom_date\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07to_date\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x66rom_version\x18\x03 \x01(\t\x12O\n\x0espark_pipeline\x18\x04 \x01(\x0b\x32\x37.ai.h2o.featurestore.api.v1.SparkPipelineTransformation\x12X\n\x0f\x66\x65\x61ture_mapping\x18\x05 \x03(\x0b\x32?.ai.h2o.featurestore.api.v1.BackfillOptions.FeatureMappingEntry\x1a\x35\n\x13\x46\x65\x61tureMappingEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"W\n\x10\x42\x61\x63kfillResponse\x12\x43\n\x0fingest_response\x18\x01 \x01(\x0b\x32*.ai.h2o.featurestore.api.v1.IngestResponse\"\xac\x02\n\x16\x46\x65\x61tureSetDraftRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04tags\x18\x04 \x03(\t\x12\x35\n\x04\x63red\x18\x05 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.Credentials\x12@\n\x0b\x64\x61ta_source\x18\x06 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocation\x12\x0e\n\x06secret\x18\x07 \x01(\x08\x12\x44\n\x0c\x64\x65rived_from\x18\x08 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\"\x84\x02\n\"FeatureSetMajorVersionDraftRequest\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x03 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x04 \x01(\t\x12\x0e\n\x06reason\x18\x05 \x01(\t\x12\x35\n\x04\x63red\x18\x06 \x01(\x0b\x32\'.ai.h2o.featurestore.api.v1.Credentials\x12@\n\x0b\x64\x61ta_source\x18\x07 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.RawDataLocation\"\x93\x03\n\x18\x44raftToFeatureSetRequest\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12>\n\x06schema\x18\x05 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.FeatureSchemaDraft\x12\x61\n\x12time_travel_column\x18\x06 \x01(\x0b\x32\x45.ai.h2o.featurestore.api.v1.DraftToFeatureSetRequest.TimeTravelColumn\x12\x0e\n\x06secret\x18\x07 \x01(\x08\x12\x0c\n\x04tags\x18\x08 \x03(\t\x1as\n\x10TimeTravelColumn\x12\x1f\n\x17time_travel_column_name\x18\x01 \x01(\t\x12!\n\x19time_travel_column_format\x18\x02 \x01(\t\x12\x1b\n\x13is_partition_column\x18\x03 \x01(\x08\"\x8d\x03\n+MajorVersionDraftToFeatureSetVersionRequest\x12\n\n\x02id\x18\x01 \x01(\x04\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12>\n\x06schema\x18\x03 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.FeatureSchemaDraft\x12\x0e\n\x06reason\x18\x04 \x01(\t\x12\x45\n\x10\x62\x61\x63kfill_options\x18\x05 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.BackfillOptions\x12+\n#use_time_travel_column_as_partition\x18\x06 \x01(\x08\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x07 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x08 \x01(\t\x12\x1e\n\x16new_time_travel_column\x18\t \x01(\t\x12%\n\x1dnew_time_travel_column_format\x18\n \x01(\t\"3\n\x19\x44raftToFeatureSetResponse\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\"\x8d\x01\n,MajorVersionDraftToFeatureSetVersionResponse\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x0e\n\x06job_id\x18\x02 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x03 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x04 \x01(\t\"\xc9\x03\n\x12\x46\x65\x61tureSchemaDraft\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tdata_type\x18\x02 \x01(\t\x12>\n\x06nested\x18\x03 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.FeatureSchemaDraft\x12P\n\x0cspecial_data\x18\x04 \x01(\x0b\x32:.ai.h2o.featurestore.api.v1.FeatureSchemaDraft.SpecialData\x12=\n\x0c\x66\x65\x61ture_type\x18\x05 \x01(\x0e\x32\'.ai.h2o.featurestore.api.v1.FeatureType\x12\x13\n\x0b\x64\x65scription\x18\x06 \x01(\t\x12\x19\n\x11\x61nomaly_detection\x18\x07 \x01(\x08\x12\x16\n\x0eis_primary_key\x18\x08 \x01(\x08\x12\x1b\n\x13is_partition_column\x18\t \x01(\x08\x1a\\\n\x0bSpecialData\x12\x0b\n\x03spi\x18\x01 \x01(\x08\x12\x0b\n\x03pci\x18\x02 \x01(\x08\x12\x0b\n\x03rpi\x18\x03 \x01(\x08\x12\x13\n\x0b\x64\x65mographic\x18\x04 \x01(\x08\x12\x11\n\tsensitive\x18\x05 \x01(\x08\"1\n\x11\x46\x65\x61tureSetDraftId\x12\x1c\n\x14\x66\x65\x61ture_set_draft_id\x18\x01 \x01(\x04\"D\n\x1bListFeatureSetDraftsRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\"\xe0\x04\n\x17ListableFeatureSetDraft\x12\x1c\n\x14\x66\x65\x61ture_set_draft_id\x18\x01 \x01(\x04\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0cproject_name\x18\x04 \x01(\t\x12\x38\n\x05owner\x18\x05 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12Y\n\x06status\x18\x06 \x01(\x0e\x32I.ai.h2o.featurestore.api.v1.ListableFeatureSetDraft.FeatureSetDraftStatus\x12\x15\n\rerror_message\x18\x07 \x01(\t\x12\x0e\n\x06job_id\x18\x08 \x01(\t\x12\x33\n\x0f\x65xpiration_date\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x43\n\ndraft_type\x18\n \x01(\x0e\x32/.ai.h2o.featurestore.api.v1.FeatureSetDraftType\"\xb7\x01\n\x15\x46\x65\x61tureSetDraftStatus\x12(\n$FEATURE_SET_DRAFT_STATUS_UNSPECIFIED\x10\x00\x12(\n$FEATURE_SET_DRAFT_STATUS_IN_PROGRESS\x10\x01\x12%\n!FEATURE_SET_DRAFT_STATUS_FINISHED\x10\x02\x12#\n\x1f\x46\x45\x41TURE_SET_DRAFT_STATUS_FAILED\x10\x03\"\x94\x03\n\x0f\x46\x65\x61tureSetDraft\x12\x1c\n\x14\x66\x65\x61ture_set_draft_id\x18\x01 \x01(\x04\x12\x12\n\nproject_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12>\n\x06schema\x18\x05 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.FeatureSchemaDraft\x12\x0e\n\x06secret\x18\x06 \x01(\x08\x12\x0c\n\x04tags\x18\x07 \x03(\t\x12\x43\n\ndraft_type\x18\x08 \x01(\x0e\x32/.ai.h2o.featurestore.api.v1.FeatureSetDraftType\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\t \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\n \x01(\t\x12\x0e\n\x06reason\x18\x0b \x01(\t\x12\x44\n\x0c\x64\x65rived_from\x18\x0c \x01(\x0b\x32..ai.h2o.featurestore.api.v1.DerivedInformation\"|\n\x1cListFeatureSetDraftsResponse\x12\x43\n\x06\x64rafts\x18\x01 \x03(\x0b\x32\x33.ai.h2o.featurestore.api.v1.ListableFeatureSetDraft\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"a\n\x17\x46\x65\x61tureSetDraftResponse\x12\x46\n\x11\x66\x65\x61ture_set_draft\x18\x01 \x01(\x0b\x32+.ai.h2o.featurestore.api.v1.FeatureSetDraft\"\xec\x01\n\x08\x41rtifact\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\x12\r\n\x05title\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x10\n\x08\x66ilename\x18\x04 \x01(\t\x12\x0b\n\x03url\x18\x05 \x01(\t\x12?\n\rartifact_type\x18\x06 \x01(\x0e\x32(.ai.h2o.featurestore.api.v1.ArtifactType\x12G\n\rupload_status\x18\x07 \x01(\x0e\x32\x30.ai.h2o.featurestore.api.v1.ArtifactUploadStatus\"\xae\x01\n\x18StoreFileArtifactRequest\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x10\n\x08\x66ilename\x18\x04 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x05 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x06 \x01(\r\x12\x14\n\x0cmd5_checksum\x18\x07 \x01(\t\"\xd4\x01\n\x19StoreFileArtifactResponse\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\x12\x10\n\x08\x66ilename\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12S\n\x07headers\x18\x04 \x03(\x0b\x32\x42.ai.h2o.featurestore.api.v1.StoreFileArtifactResponse.HeadersEntry\x1a.\n\x0cHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\".\n\x17RetrieveArtifactRequest\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\"R\n\x18RetrieveArtifactResponse\x12\x36\n\x08\x61rtifact\x18\x01 \x01(\x0b\x32$.ai.h2o.featurestore.api.v1.Artifact\"y\n\x19UpdateUploadStatusRequest\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\x12G\n\rupload_status\x18\x02 \x01(\x0e\x32\x30.ai.h2o.featurestore.api.v1.ArtifactUploadStatus\",\n\x15\x44\x65leteArtifactRequest\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\"x\n\x14ListArtifactsRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x02 \x01(\r\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\x12\n\npage_token\x18\x04 \x01(\t\"i\n\x15ListArtifactsResponse\x12\x37\n\tartifacts\x18\x01 \x03(\x0b\x32$.ai.h2o.featurestore.api.v1.Artifact\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"~\n\x10StoreLinkRequest\x12\r\n\x05title\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x05 \x01(\r\"(\n\x11StoreLinkResponse\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\"\xc9\x01\n\x14\x46\x65\x61tureSetPopularity\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1c\n\x14number_of_retrievals\x18\x02 \x01(\x04\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x03 \x01(\t\x12\x1f\n\x17\x66\x65\x61ture_set_description\x18\x04 \x01(\t\x12@\n\npermission\x18\x05 \x01(\x0e\x32,.ai.h2o.featurestore.api.v1.ActivePermission\"g\n\x1d\x46\x65\x61tureSetsPopularityResponse\x12\x46\n\x0c\x66\x65\x61ture_sets\x18\x01 \x03(\x0b\x32\x30.ai.h2o.featurestore.api.v1.FeatureSetPopularity\"\x96\x01\n\x1eListFeatureSetsToReviewRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\x12\x39\n\x07\x66ilters\x18\x03 \x03(\x0e\x32(.ai.h2o.featurestore.api.v1.ReviewStatus\x12\x12\n\nproject_id\x18\x04 \x01(\t\"{\n\x1fListFeatureSetsToReviewResponse\x12?\n\x07\x65ntries\x18\x01 \x03(\x0b\x32..ai.h2o.featurestore.api.v1.FeatureSetToReview\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xb6\x02\n\x12\x46\x65\x61tureSetToReview\x12\x11\n\treview_id\x18\x01 \x01(\x04\x12\x14\n\x0cproject_name\x18\x02 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x03 \x01(\t\x12\x38\n\x05owner\x18\x04 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x06status\x18\x07 \x01(\x0e\x32(.ai.h2o.featurestore.api.v1.ReviewStatus\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x08 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\t \x01(\r\"9\n\x14\x41pproveReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\x12\x0e\n\x06reason\x18\x02 \x01(\t\"8\n\x13RejectReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\x12\x0e\n\x06reason\x18\x02 \x01(\t\"\x98\x01\n ListFeatureSetReviewsPageRequest\x12\x39\n\x07\x66ilters\x18\x01 \x03(\x0e\x32(.ai.h2o.featurestore.api.v1.ReviewStatus\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\x12\n\nproject_id\x18\x04 \x01(\t\"\xf8\x02\n\x10\x46\x65\x61tureSetReview\x12\x11\n\treview_id\x18\x01 \x01(\x04\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x02 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x03 \x01(\r\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x04 \x01(\t\x12\x14\n\x0cproject_name\x18\x05 \x01(\t\x12\x38\n\x06status\x18\x06 \x01(\x0e\x32(.ai.h2o.featurestore.api.v1.ReviewStatus\x12\x0e\n\x06reason\x18\x07 \x01(\t\x12;\n\x08reviewer\x18\x08 \x01(\x0b\x32).ai.h2o.featurestore.api.v1.UserBasicInfo\x12/\n\x0breviewed_at\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\ncreated_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"{\n!ListFeatureSetReviewsPageResponse\x12=\n\x07\x65ntries\x18\x01 \x03(\x0b\x32,.ai.h2o.featurestore.api.v1.FeatureSetReview\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"9\n$GetListableFeatureSetToReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"u\n%GetListableFeatureSetToReviewResponse\x12L\n\x14listable_feature_set\x18\x01 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.ListableFeatureSet\"9\n$GetListableFeatureSetInReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"u\n%GetListableFeatureSetInReviewResponse\x12L\n\x14listable_feature_set\x18\x01 \x01(\x0b\x32..ai.h2o.featurestore.api.v1.ListableFeatureSet\"4\n\x1f\x44\x65leteRejectedFeatureSetRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"f\n\x1bListFeaturesToReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\"n\n\x1cListFeaturesToReviewResponse\x12\x35\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"f\n\x1bListFeaturesInReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x12\n\npage_token\x18\x03 \x01(\t\x12\r\n\x05query\x18\x04 \x01(\t\"n\n\x1cListFeaturesInReviewResponse\x12\x35\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32#.ai.h2o.featurestore.api.v1.Feature\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"8\n#GetFeatureSetPreviewToReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"Q\n$GetFeatureSetPreviewToReviewResponse\x12\x13\n\x0bpreview_url\x18\x01 \x01(\t\x12\x14\n\x0cmax_cols_num\x18\x02 \x01(\r\"8\n#GetFeatureSetPreviewInReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"Q\n$GetFeatureSetPreviewInReviewResponse\x12\x13\n\x0bpreview_url\x18\x01 \x01(\t\x12\x14\n\x0cmax_cols_num\x18\x02 \x01(\r\"1\n\x1cGetFeatureSetToReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"\\\n\x1dGetFeatureSetToReviewResponse\x12;\n\x0b\x66\x65\x61ture_set\x18\x01 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\"1\n\x1cGetFeatureSetInReviewRequest\x12\x11\n\treview_id\x18\x01 \x01(\x04\"\\\n\x1dGetFeatureSetInReviewResponse\x12;\n\x0b\x66\x65\x61ture_set\x18\x01 \x01(\x0b\x32&.ai.h2o.featurestore.api.v1.FeatureSet\"\xc0\x01\n\x13RecentlyUsedProject\x12\x12\n\nproject_id\x18\x01 \x01(\t\x12\x14\n\x0cproject_name\x18\x02 \x01(\t\x12\x1b\n\x13project_description\x18\x03 \x01(\t\x12.\n\nupdated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0elast_access_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"a\n\x1cRecentlyUsedProjectsResponse\x12\x41\n\x08projects\x18\x01 \x03(\x0b\x32/.ai.h2o.featurestore.api.v1.RecentlyUsedProject\"\xcf\x01\n\x16RecentlyUsedFeatureSet\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x1f\n\x17\x66\x65\x61ture_set_description\x18\x03 \x01(\t\x12.\n\nupdated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0elast_access_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"k\n\x1fRecentlyUsedFeatureSetsResponse\x12H\n\x0c\x66\x65\x61ture_sets\x18\x01 \x03(\x0b\x32\x32.ai.h2o.featurestore.api.v1.RecentlyUsedFeatureSet\"_\n\x14TargetFeatureRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\x12\x12\n\nfeature_id\x18\x03 \x01(\t\"P\n\x19ListTargetFeaturesRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x1b\n\x13\x66\x65\x61ture_set_version\x18\x02 \x01(\t\"B\n\x16TargetFeatureReference\x12\x12\n\nfeature_id\x18\x01 \x01(\t\x12\x14\n\x0c\x66\x65\x61ture_name\x18\x02 \x01(\t\"b\n\x1aListTargetFeaturesResponse\x12\x44\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x32.ai.h2o.featurestore.api.v1.TargetFeatureReference\"\x80\x02\n#ListJobsPageByFeatureSetNameRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\x12\x41\n\rstatus_filter\x18\x03 \x01(\x0e\x32%.ai.h2o.featurestore.api.v1.JobStatusH\x00\x88\x01\x01\x12\x1e\n\x16\x66\x65\x61ture_set_name_query\x18\x04 \x01(\t\x12=\n\x10job_type_filters\x18\x05 \x03(\x0e\x32#.ai.h2o.featurestore.api.v1.JobTypeB\x10\n\x0e_status_filter\"\xf6\x01\n!ListJobsPageByFeatureSetIdRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\x12\x41\n\rstatus_filter\x18\x03 \x01(\x0e\x32%.ai.h2o.featurestore.api.v1.JobStatusH\x00\x88\x01\x01\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x04 \x01(\t\x12=\n\x10job_type_filters\x18\x05 \x03(\x0e\x32#.ai.h2o.featurestore.api.v1.JobTypeB\x10\n\x0e_status_filter\"m\n\x18\x46\x65\x61tureSetJobRelatedInfo\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x1f\n\x17\x66\x65\x61ture_set_description\x18\x03 \x01(\t\"\xe0\x01\n\x0bListableJob\x12R\n\x14\x66\x65\x61ture_set_job_info\x18\x01 \x01(\x0b\x32\x34.ai.h2o.featurestore.api.v1.FeatureSetJobRelatedInfo\x12,\n\x03job\x18\x02 \x01(\x0b\x32\x1f.ai.h2o.featurestore.api.v1.Job\x12;\n\nchild_jobs\x18\x03 \x03(\x0b\x32\'.ai.h2o.featurestore.api.v1.ListableJob\x12\x12\n\nis_derived\x18\x04 \x01(\x08\"i\n\x14ListJobsPageResponse\x12\x38\n\x07\x65ntries\x18\x01 \x03(\x0b\x32\'.ai.h2o.featurestore.api.v1.ListableJob\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"]\n\x1dGetJobsWithStatusCountRequest\x12<\n\rstatus_filter\x18\x01 \x01(\x0e\x32%.ai.h2o.featurestore.api.v1.JobStatus\"4\n\x1eGetJobsWithStatusCountResponse\x12\x12\n\njobs_count\x18\x01 \x01(\r\".\n\x14PinFeatureSetRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\"0\n\x16UnpinFeatureSetRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\"A\n\x18PinnedFeatureSetsRequest\x12\x11\n\tpage_size\x18\x01 \x01(\x05\x12\x12\n\npage_token\x18\x02 \x01(\t\"\xd8\x01\n\x10PinnedFeatureSet\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12\x18\n\x10\x66\x65\x61ture_set_name\x18\x02 \x01(\t\x12\x1f\n\x17\x66\x65\x61ture_set_description\x18\x03 \x01(\t\x12.\n\nupdated_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\tpinned_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nuser_order\x18\x06 \x01(\x03\"x\n\x19PinnedFeatureSetsResponse\x12\x42\n\x0c\x66\x65\x61ture_sets\x18\x01 \x03(\x0b\x32,.ai.h2o.featurestore.api.v1.PinnedFeatureSet\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"3\n\x19IsFeatureSetPinnedRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\",\n\x1aIsFeatureSetPinnedResponse\x12\x0e\n\x06pinned\x18\x01 \x01(\x08\"Q\n\x14\x43odeSnippedIdRequest\x12\x16\n\x0e\x66\x65\x61ture_set_id\x18\x01 \x01(\t\x12!\n\x19\x66\x65\x61ture_set_major_version\x18\x02 \x01(\r\",\n\x15\x43odeSnippedIdResponse\x12\x13\n\x0b\x61rtifact_id\x18\x01 \x01(\x04\"\xd0\x03\n\x14\x41\x64vancedSearchOption\x12X\n\x0fsearch_operator\x18\x01 \x01(\x0e\x32?.ai.h2o.featurestore.api.v1.AdvancedSearchOption.SearchOperator\x12R\n\x0csearch_field\x18\x02 \x01(\x0e\x32<.ai.h2o.featurestore.api.v1.AdvancedSearchOption.SearchField\x12\x14\n\x0csearch_value\x18\x03 \x01(\t\"c\n\x0eSearchOperator\x12\x1f\n\x1bSEARCH_OPERATOR_UNSPECIFIED\x10\x00\x12\x18\n\x14SEARCH_OPERATOR_LIKE\x10\x01\x12\x16\n\x12SEARCH_OPERATOR_EQ\x10\x02\"\x8e\x01\n\x0bSearchField\x12\x1c\n\x18SEARCH_FIELD_UNSPECIFIED\x10\x00\x12\x1d\n\x19SEARCH_FIELD_FEATURE_NAME\x10\x01\x12$\n SEARCH_FIELD_FEATURE_DESCRIPTION\x10\x02\x12\x1c\n\x18SEARCH_FIELD_FEATURE_TAG\x10\x03*\xbc\x02\n\x07JobType\x12\x0b\n\x07Unknown\x10\x00\x12\n\n\x06Ingest\x10\x01\x12\x0c\n\x08Retrieve\x10\x02\x12\x11\n\rExtractSchema\x10\x03\x12\x15\n\x11\x43omputeStatistics\x10\x05\x12\n\n\x06Revert\x10\x06\x12\x19\n\x15MaterializationOnline\x10\x07\x12$\n ComputeRecommendationClassifiers\x10\x08\x12\x13\n\x0f\x43reateMLDataset\x10\t\x12\x1e\n\x1a\x46\x65\x61tureViewRetrieveAsLinks\x10\n\x12\x1e\n\x1a\x46\x65\x61tureViewRetrieveAsSpark\x10\x0b\x12\x0c\n\x08\x42\x61\x63kfill\x10\x0c\x12\x15\n\x11RetrieveMLDataset\x10\r\x12\x13\n\x0fOptimizeStorage\x10\x0e\"\x04\x08\x04\x10\x04*X\n\x0ePermissionType\x12\t\n\x05Owner\x10\x00\x12\n\n\x06\x45\x64itor\x10\x01\x12\x0c\n\x08\x43onsumer\x10\x02\x12\x15\n\x11SensitiveConsumer\x10\x03\x12\n\n\x06Viewer\x10\x04*\xd1\x01\n\x10\x41\x63tivePermission\x12\x1a\n\x16\x41\x43TIVE_PERMISSION_NONE\x10\x00\x12\x1b\n\x17\x41\x43TIVE_PERMISSION_OWNER\x10\x01\x12\x1c\n\x18\x41\x43TIVE_PERMISSION_EDITOR\x10\x02\x12\x1e\n\x1a\x41\x43TIVE_PERMISSION_CONSUMER\x10\x03\x12(\n$ACTIVE_PERMISSION_SENSITIVE_CONSUMER\x10\x04\x12\x1c\n\x18\x41\x43TIVE_PERMISSION_VIEWER\x10\x05*9\n\rProjectAction\x12\x13\n\x0fPROJECT_CREATED\x10\x00\x12\x13\n\x0fPROJECT_UPDATED\x10\x01*^\n\x14OfflineStorageFormat\x12 \n\x1cOFFLINE_STORAGE_FORMAT_DELTA\x10\x00\x12$\n OFFLINE_STORAGE_FORMAT_SNOWFLAKE\x10\x01*q\n\x08JoinType\x12\x13\n\x0fJOIN_TYPE_INNER\x10\x00\x12\x12\n\x0eJOIN_TYPE_LEFT\x10\x01\x12\x13\n\x0fJOIN_TYPE_RIGHT\x10\x02\x12\x12\n\x0eJOIN_TYPE_FULL\x10\x03\x12\x13\n\x0fJOIN_TYPE_CROSS\x10\x04*\xfc\x01\n\x15\x46\x65\x61tureFilterOperator\x12#\n\x1f\x46\x45\x41TURE_FILTER_OPERATOR_UNKNOWN\x10\x00\x12\x1e\n\x1a\x46\x45\x41TURE_FILTER_OPERATOR_EQ\x10\x01\x12\x1e\n\x1a\x46\x45\x41TURE_FILTER_OPERATOR_LT\x10\x02\x12\x1e\n\x1a\x46\x45\x41TURE_FILTER_OPERATOR_LE\x10\x03\x12\x1e\n\x1a\x46\x45\x41TURE_FILTER_OPERATOR_GT\x10\x04\x12\x1e\n\x1a\x46\x45\x41TURE_FILTER_OPERATOR_GE\x10\x05\x12\x1e\n\x1a\x46\x45\x41TURE_FILTER_OPERATOR_NE\x10\x06*\x94\x01\n\x1a\x46\x65\x61tureFilterLogicOperator\x12)\n%FEATURE_FILTER_LOGIC_OPERATOR_UNKNOWN\x10\x00\x12%\n!FEATURE_FILTER_LOGIC_OPERATOR_AND\x10\x01\x12$\n FEATURE_FILTER_LOGIC_OPERATOR_OR\x10\x02*Q\n\x14\x46\x65\x61tureQueryJoinType\x12\x1c\n\x18\x46\x45\x41TURE_QUERY_JOIN_INNER\x10\x00\x12\x1b\n\x17\x46\x45\x41TURE_QUERY_JOIN_LEFT\x10\x01*\x96\x01\n\x0f\x46\x65\x61tureDataType\x12\x0b\n\x07TinyInt\x10\x00\x12\x0c\n\x08SmallInt\x10\x01\x12\n\n\x06\x42igInt\x10\x02\x12\x07\n\x03Int\x10\x03\x12\t\n\x05\x46loat\x10\x04\x12\n\n\x06\x44ouble\x10\x05\x12\n\n\x06String\x10\x06\x12\n\n\x06\x42inary\x10\x07\x12\x0b\n\x07\x42oolean\x10\x08\x12\x08\n\x04\x44\x61te\x10\t\x12\r\n\tTimestamp\x10\n*q\n\x13ProcessIntervalUnit\x12\r\n\tUNDEFINED\x10\x00\x12\t\n\x05HOURS\x10\x01\x12\n\n\x06MONTHS\x10\x02\x12\x08\n\x04\x44\x41YS\x10\x03\x12\x0b\n\x07MINUTES\x10\x04\x12\x0b\n\x07SECONDS\x10\x05\x12\x10\n\x0cMILLISECONDS\x10\x06*h\n\x12TransformationType\x12\x19\n\x15TransformationUnknown\x10\x00\x12\x16\n\x12TransformationMojo\x10\x01\x12\x1f\n\x1bTransformationSparkPipeline\x10\x02*,\n\rSortDirection\x12\x0c\n\x08SORT_ASC\x10\x00\x12\r\n\tSORT_DESC\x10\x01*,\n\x0cResourceType\x12\x0b\n\x07PROJECT\x10\x00\x12\x0f\n\x0b\x46\x45\x41TURE_SET\x10\x01*T\n\x0fPermissionState\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07GRANTED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02\x12\x0b\n\x07REVOKED\x10\x03\x12\x0c\n\x08PROMOTED\x10\x04*\'\n\x08TaskType\x12\n\n\x06INGEST\x10\x00\x12\x0f\n\x0bLAZY_INGEST\x10\x01*\xae\x01\n\tJobStatus\x12\x0b\n\x07\x43reated\x10\x00\x12\r\n\tSubmitted\x10\x01\x12\x0b\n\x07Running\x10\x02\x12\x14\n\x10SubmissionFailed\x10\x03\x12\n\n\x06\x46\x61iled\x10\x04\x12\x0b\n\x07Success\x10\x06\x12\x0b\n\x07Pending\x10\x07\x12\x10\n\x0cPendingRerun\x10\x08\x12\x0b\n\x07\x46\x61iling\x10\t\x12\x0e\n\nCancelling\x10\n\x12\r\n\tCancelled\x10\x0b*\x8a\x01\n\x15UpdatableProjectField\x12\x17\n\x13PROJECT_UNSPECIFIED\x10\x00\x12\x12\n\x0ePROJECT_LOCKED\x10\x01\x12\x12\n\x0ePROJECT_SECRET\x10\x02\x12\x17\n\x13PROJECT_DESCRIPTION\x10\x03\x12\x17\n\x13PROJECT_CUSTOM_DATA\x10\x04*\xf1\x05\n\x18UpdatableFeatureSetField\x12\x1b\n\x17\x46\x45\x41TURE_SET_UNSPECIFIED\x10\x00\x12\x14\n\x10\x46\x45\x41TURE_SET_TAGS\x10\x01\x12#\n\x1f\x46\x45\x41TURE_SET_DATA_SOURCE_DOMAINS\x10\x02\x12\x1b\n\x17\x46\x45\x41TURE_SET_DESCRIPTION\x10\x03\x12\x14\n\x10\x46\x45\x41TURE_SET_TYPE\x10\x04\x12 \n\x1c\x46\x45\x41TURE_SET_APPLICATION_NAME\x10\x05\x12\x1e\n\x1a\x46\x45\x41TURE_SET_APPLICATION_ID\x10\x06\x12\x1a\n\x16\x46\x45\x41TURE_SET_DEPRECATED\x10\x07\x12 \n\x1c\x46\x45\x41TURE_SET_PROCESS_INTERVAL\x10\x08\x12%\n!FEATURE_SET_PROCESS_INTERVAL_UNIT\x10\t\x12\x14\n\x10\x46\x45\x41TURE_SET_FLOW\x10\n\x12\x15\n\x11\x46\x45\x41TURE_SET_STATE\x10\x0b\x12\x16\n\x12\x46\x45\x41TURE_SET_SECRET\x10\x0c\x12\x1b\n\x17\x46\x45\x41TURE_SET_TTL_OFFLINE\x10\r\x12$\n FEATURE_SET_TTL_OFFLINE_INTERVAL\x10\x0e\x12\x1a\n\x16\x46\x45\x41TURE_SET_TTL_ONLINE\x10\x0f\x12#\n\x1f\x46\x45\x41TURE_SET_TTL_ONLINE_INTERVAL\x10\x10\x12\x1b\n\x17\x46\x45\x41TURE_SET_CUSTOM_DATA\x10\x11\x12+\n\'FEATURE_SET_SPECIAL_DATA_LEGAL_APPROVED\x10\x12\x12(\n$FEATURE_SET_SPECIAL_DATA_LEGAL_NOTES\x10\x13\x12 \n\x1c\x46\x45\x41TURE_SET_ONLINE_NAMESPACE\x10\x14\x12\x1c\n\x18\x46\x45\x41TURE_SET_ONLINE_TOPIC\x10\x15\x12&\n\"FEATURE_SET_ONLINE_CONNECTION_TYPE\x10\x16*\xed\x01\n\x15UpdatableFeatureField\x12\x17\n\x13\x46\x45\x41TURE_UNSPECIFIED\x10\x00\x12\x12\n\x0e\x46\x45\x41TURE_STATUS\x10\x01\x12\x10\n\x0c\x46\x45\x41TURE_TYPE\x10\x02\x12\x16\n\x12\x46\x45\x41TURE_IMPORTANCE\x10\x03\x12\x17\n\x13\x46\x45\x41TURE_CUSTOM_DATA\x10\x04\x12\x17\n\x13\x46\x45\x41TURE_DESCRIPTION\x10\x05\x12\x13\n\x0f\x46\x45\x41TURE_SPECIAL\x10\x06\x12\x1d\n\x19\x46\x45\x41TURE_ANOMALY_DETECTION\x10\x07\x12\x17\n\x13\x46\x45\x41TURE_CLASSIFIERS\x10\x08*\xc4\x01\n\x13\x46\x65\x61tureSetDraftType\x12&\n\"FEATURE_SET_DRAFT_TYPE_UNSPECIFIED\x10\x00\x12%\n!FEATURE_SET_DRAFT_TYPE_CREATE_NEW\x10\x01\x12/\n+FEATURE_SET_DRAFT_TYPE_CREATE_MAJOR_VERSION\x10\x02\x12-\n)FEATURE_SET_DRAFT_TYPE_CREATE_NEW_DERIVED\x10\x03*]\n\x0c\x41rtifactType\x12\x1d\n\x19\x41RTIFACT_TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12\x41RTIFACT_TYPE_LINK\x10\x01\x12\x16\n\x12\x41RTIFACT_TYPE_FILE\x10\x02*\xad\x01\n\x14\x41rtifactUploadStatus\x12)\n%ARTIFACT_UPLOAD_STATUS_NOT_APPLICABLE\x10\x00\x12&\n\"ARTIFACT_UPLOAD_STATUS_IN_PROGRESS\x10\x01\x12\x1f\n\x1b\x41RTIFACT_UPLOAD_STATUS_DONE\x10\x02\x12!\n\x1d\x41RTIFACT_UPLOAD_STATUS_FAILED\x10\x03*\x9d\x01\n\x0cReviewStatus\x12\x1d\n\x19REVIEW_STATUS_UNSPECIFIED\x10\x00\x12\x1b\n\x17REVIEW_STATUS_TO_REVIEW\x10\x01\x12\x1a\n\x16REVIEW_STATUS_APPROVED\x10\x02\x12\x1a\n\x16REVIEW_STATUS_REJECTED\x10\x03\x12\x19\n\x15REVIEW_STATUS_CREATED\x10\x04\x32\xa8\xf2\x01\n\x0b\x43oreService\x12{\n\x08ListJobs\x12+.ai.h2o.featurestore.api.v1.ListJobsRequest\x1a,.ai.h2o.featurestore.api.v1.ListJobsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/api/v1/jobs\x12k\n\x06GetJob\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x1f.ai.h2o.featurestore.api.v1.Job\"\x1d\x82\xd3\xe4\x93\x02\x17\x12\x15/api/v1/jobs/{job_id}\x12\xa2\x01\n\x0eGetJobProgress\x12,.ai.h2o.featurestore.api.v1.JobProgressInput\x1a-.ai.h2o.featurestore.api.v1.JobProgressOutput\"3\x82\xd3\xe4\x93\x02-\x12+/api/v1/jobs/{job_id}/progress/{next_index}\x12\x65\n\tCancelJob\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x16.google.protobuf.Empty\"\x1d\x82\xd3\xe4\x93\x02\x17*\x15/api/v1/jobs/{job_id}\x12\xb8\x01\n\x1cListJobsPageByFeatureSetName\x12?.ai.h2o.featurestore.api.v1.ListJobsPageByFeatureSetNameRequest\x1a\x30.ai.h2o.featurestore.api.v1.ListJobsPageResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/api/v1/jobs/feature-set/name\x12\xb2\x01\n\x1aListJobsPageByFeatureSetId\x12=.ai.h2o.featurestore.api.v1.ListJobsPageByFeatureSetIdRequest\x1a\x30.ai.h2o.featurestore.api.v1.ListJobsPageResponse\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/api/v1/jobs/feature-set/id\x12\xb5\x01\n\x16GetJobsWithStatusCount\x12\x39.ai.h2o.featurestore.api.v1.GetJobsWithStatusCountRequest\x1a:.ai.h2o.featurestore.api.v1.GetJobsWithStatusCountResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/api/v1/jobs/count-by-status\x12\x9c\x01\n\x15StartExtractSchemaJob\x12\x38.ai.h2o.featurestore.api.v1.StartExtractSchemaJobRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"&\x82\xd3\xe4\x93\x02 \"\x1b/api/v1/jobs/extract-schema:\x01*\x12\xa6\x01\n\x19GetExtractSchemaJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x31.ai.h2o.featurestore.api.v1.ExtractSchemaResponse\"3\x82\xd3\xe4\x93\x02-\x12+/api/v1/jobs/{job_id}/output/extract-schema\x12\x87\x01\n\x0eStartIngestJob\x12\x31.ai.h2o.featurestore.api.v1.StartIngestJobRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x14/api/v1/ingest/start:\x01*\x12\x93\x01\n\x12GetIngestJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a*.ai.h2o.featurestore.api.v1.IngestResponse\".\x82\xd3\xe4\x93\x02(\x12&/api/v1/jobs/{job_id}/output/ingestion\x12\x93\x01\n\x17StartRetrieveAsLinksJob\x12+.ai.h2o.featurestore.api.v1.RetrieveRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"(\x82\xd3\xe4\x93\x02\"\"\x1d/api/v1/feature-sets/retrieve:\x01*\x12\xa5\x01\n\x1bGetRetrieveAsLinksJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x33.ai.h2o.featurestore.api.v1.RetrieveAsLinksResponse\".\x82\xd3\xe4\x93\x02(\x12&/api/v1/feature-sets/retrieve/{job_id}\x12\xa6\x01\n\x0fRetrieveAsSpark\x12+.ai.h2o.featurestore.api.v1.RetrieveRequest\x1a\x33.ai.h2o.featurestore.api.v1.RetrieveAsSparkResponse\"1\x82\xd3\xe4\x93\x02+\"&/api/v1/feature-sets/retrieve/as-spark:\x01*\x12\xc0\x01\n\x19GetIngestWriteCredentials\x12\x38.ai.h2o.featurestore.api.v1.IngestWriteCredentialRequest\x1a\x39.ai.h2o.featurestore.api.v1.IngestWriteCredentialResponse\".\x82\xd3\xe4\x93\x02(\x12&/api/v1/ingest/credential/{session_id}\x12\x94\x01\n\x14StartRevertIngestJob\x12\x37.ai.h2o.featurestore.api.v1.StartRevertIngestJobRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\" \x82\xd3\xe4\x93\x02\x1a\"\x15/api/v1/ingest/revert:\x01*\x12}\n\x18GetRevertIngestJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x16.google.protobuf.Empty\"&\x82\xd3\xe4\x93\x02 \x12\x1e/api/v1/ingest/revert/{job_id}\x12\xe6\x01\n\x17HasPermissionToRetrieve\x12:.ai.h2o.featurestore.api.v1.HasPermissionToRetrieveRequest\x1a;.ai.h2o.featurestore.api.v1.HasPermissionToRetrieveResponse\"R\x82\xd3\xe4\x93\x02L\x12J/api/v1/feature-sets/retrieve/permission/{project_name}/{feature_set_name}\x12\x9c\x01\n\x12RegisterFeatureSet\x12\x35.ai.h2o.featurestore.api.v1.RegisterFeatureSetRequest\x1a..ai.h2o.featurestore.api.v1.FeatureSetResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x14/api/v1/feature-sets:\x01*\x12\xc5\x01\n\x1a\x43reateNewFeatureSetVersion\x12=.ai.h2o.featurestore.api.v1.CreateNewFeatureSetVersionRequest\x1a..ai.h2o.featurestore.api.v1.FeatureSetResponse\"8\x82\xd3\xe4\x93\x02\x32\"-/api/v1/feature-sets/{feature_set_id}/version:\x01*\x12\x80\x01\n\x15GetOnlineRetrieveMeta\x12\x16.google.protobuf.Empty\x1a..ai.h2o.featurestore.api.v1.OnlineRetrieveMeta\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/api/v1/online-retrieve\x12m\n\nGetVersion\x12\x16.google.protobuf.Empty\x1a..ai.h2o.featurestore.api.v1.GetVersionResponse\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/api/v1/version\x12\xb8\x01\n\rGetFeatureSet\x12\x30.ai.h2o.featurestore.api.v1.GetFeatureSetRequest\x1a..ai.h2o.featurestore.api.v1.FeatureSetResponse\"E\x82\xd3\xe4\x93\x02?\x12=/api/v1/projects/{project_id}/feature-sets/{feature_set_name}\x12\xa3\x01\n\x11GetFeatureSetById\x12/.ai.h2o.featurestore.api.v1.FeatureSetRequestId\x1a..ai.h2o.featurestore.api.v1.FeatureSetResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/api/v1/feature-sets/{feature_set_id}\x12\xd7\x01\n&GetFeatureSetsLastMinorForCurrentMajor\x12I.ai.h2o.featurestore.api.v1.GetFeatureSetsLastMinorForCurrentMajorRequest\x1a..ai.h2o.featurestore.api.v1.FeatureSetResponse\"2\x82\xd3\xe4\x93\x02,\x12*/api/v1/feature-sets/{feature_set_id}/last\x12\x8d\x02\n\'GetLastMinorFeatureSetForMajorInProject\x12J.ai.h2o.featurestore.api.v1.GetLastMinorFeatureSetForMajorInProjectRequest\x1a..ai.h2o.featurestore.api.v1.FeatureSetResponse\"f\x82\xd3\xe4\x93\x02`\x12^/api/v1/projects/{project_id}/feature-sets/{feature_set_name}/{feature_set_major_version}/last\x12\xc7\x01\n\x16ListFeatureSetVersions\x12\x39.ai.h2o.featurestore.api.v1.ListFeatureSetsVersionRequest\x1a:.ai.h2o.featurestore.api.v1.ListFeatureSetVersionsResponse\"6\x82\xd3\xe4\x93\x02\x30\x12./api/v1/feature-sets/{feature_set_id}/versions\x12\x8e\x01\n\x10\x44\x65leteFeatureSet\x12\x33.ai.h2o.featurestore.api.v1.DeleteFeatureSetRequest\x1a\x16.google.protobuf.Empty\"-\x82\xd3\xe4\x93\x02\'*%/api/v1/feature-sets/{feature_set_id}\x12\xc1\x01\n\x17\x44\x65leteFeatureSetVersion\x12:.ai.h2o.featurestore.api.v1.DeleteFeatureSetVersionRequest\x1a\x16.google.protobuf.Empty\"R\x82\xd3\xe4\x93\x02L*J/api/v1/feature-sets/{feature_set_id}/versions/{feature_set_major_version}\x12\xa4\x01\n\x13ListFeatureSetsPage\x12\x36.ai.h2o.featurestore.api.v1.ListFeatureSetsPageRequest\x1a\x37.ai.h2o.featurestore.api.v1.ListFeatureSetsPageResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/api/v1/feature-sets\x12\xa9\x01\n\x10\x46\x65\x61tureSetExists\x12\x33.ai.h2o.featurestore.api.v1.FeatureSetExistsRequest\x1a*.ai.h2o.featurestore.api.v1.ExistsResponse\"4\x82\xd3\xe4\x93\x02.\x12,/api/v1/feature-sets/exists/{feature_set_id}\x12\xc4\x01\n\x10GetIngestHistory\x12\x33.ai.h2o.featurestore.api.v1.GetIngestHistoryRequest\x1a\x34.ai.h2o.featurestore.api.v1.GetIngestHistoryResponse\"E\x82\xd3\xe4\x93\x02?\x12=/api/v1/ingest/{feature_set_id}/{feature_set_version}/history\x12\xdf\x01\n\x1cIsFeatureSetSchemaCompatible\x12@.ai.h2o.featurestore.api.v1.FeatureSetSchemaCompatibilityRequest\x1a\x41.ai.h2o.featurestore.api.v1.FeatureSetSchemaCompatibilityResponse\":\x82\xd3\xe4\x93\x02\x34\"//api/v1/feature-sets/features/schema-compatible:\x01*\x12\xc3\x01\n\x15\x46\x65\x61tureSetSchemaPatch\x12\x38.ai.h2o.featurestore.api.v1.FeatureSetSchemaPatchRequest\x1a\x39.ai.h2o.featurestore.api.v1.FeatureSetSchemaPatchResponse\"5\x82\xd3\xe4\x93\x02/\"*/api/v1/feature-sets/features/schema-patch:\x01*\x12\xc0\x01\n\x14GetFeatureSetPreview\x12\x37.ai.h2o.featurestore.api.v1.GetFeatureSetPreviewRequest\x1a\x38.ai.h2o.featurestore.api.v1.GetFeatureSetPreviewResponse\"5\x82\xd3\xe4\x93\x02/\x12-/api/v1/feature-sets/{feature_set_id}/preview\x12\xaf\x01\n\x10UpdateFeatureSet\x12\x33.ai.h2o.featurestore.api.v1.UpdateFeatureSetRequest\x1a\x34.ai.h2o.featurestore.api.v1.UpdateFeatureSetResponse\"0\x82\xd3\xe4\x93\x02*\x1a%/api/v1/feature-sets/{feature_set_id}:\x01*\x12\xa8\x01\n\x17StartOptimizeStorageJob\x12:.ai.h2o.featurestore.api.v1.StartOptimizeStorageJobRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\".\x82\xd3\xe4\x93\x02(\"#/api/v1/jobs/optimize-storage/start:\x01*\x12\xac\x01\n\x1bGetOptimizeStorageJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x33.ai.h2o.featurestore.api.v1.OptimizeStorageResponse\"5\x82\xd3\xe4\x93\x02/\x12-/api/v1/jobs/{job_id}/output/optimize-storage\x12\x9c\x01\n\x11\x43reateFeatureView\x12\x34.ai.h2o.featurestore.api.v1.CreateFeatureViewRequest\x1a/.ai.h2o.featurestore.api.v1.FeatureViewResponse\" \x82\xd3\xe4\x93\x02\x1a\"\x15/api/v1/feature-views:\x01*\x12\xae\x01\n\x11UpdateFeatureView\x12\x34.ai.h2o.featurestore.api.v1.UpdateFeatureViewRequest\x1a/.ai.h2o.featurestore.api.v1.FeatureViewResponse\"2\x82\xd3\xe4\x93\x02,\x1a\'/api/v1/feature-views/{feature_view_id}:\x01*\x12\xb0\x01\n\x0eGetFeatureView\x12\x31.ai.h2o.featurestore.api.v1.GetFeatureViewRequest\x1a/.ai.h2o.featurestore.api.v1.FeatureViewResponse\":\x82\xd3\xe4\x93\x02\x34\x12\x32/api/v1/projects/{project_id}/feature-views/{name}\x12\xad\x01\n\x11\x46\x65\x61tureViewExists\x12\x34.ai.h2o.featurestore.api.v1.FeatureViewExistsRequest\x1a*.ai.h2o.featurestore.api.v1.ExistsResponse\"6\x82\xd3\xe4\x93\x02\x30\x12./api/v1/feature-views/{feature_view_id}/exists\x12\xb2\x01\n\x10ListFeatureViews\x12\x33.ai.h2o.featurestore.api.v1.ListFeatureViewsRequest\x1a\x34.ai.h2o.featurestore.api.v1.ListFeatureViewsResponse\"3\x82\xd3\xe4\x93\x02-\x12+/api/v1/projects/{project_id}/feature-views\x12\xb0\x01\n\x1b\x43reateFeatureViewNewVersion\x12>.ai.h2o.featurestore.api.v1.CreateFeatureViewNewVersionRequest\x1a/.ai.h2o.featurestore.api.v1.FeatureViewResponse\" \x82\xd3\xe4\x93\x02\x1a\"\x15/api/v1/feature-views:\x01*\x12\xe7\x01\n\"StartRetrieveFeatureViewAsSparkJob\x12=.ai.h2o.featurestore.api.v1.RetrieveFeatureViewAsSparkRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"_\x82\xd3\xe4\x93\x02Y\"T/api/v1/feature-views/{feature_view_id}/{feature_view_version}/retrieve-as-spark-job:\x01*\x12\xb9\x01\n&GetRetrieveFeatureViewAsSparkJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a>.ai.h2o.featurestore.api.v1.RetrieveFeatureViewAsSparkResponse\",\x82\xd3\xe4\x93\x02&\x12$/api/v1/feature-views/spark/{job_id}\x12\xe9\x01\n\"StartRetrieveFeatureViewAsLinksJob\x12?.ai.h2o.featurestore.api.v1.RetrieveFeatureViewAsAsLinksRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"_\x82\xd3\xe4\x93\x02Y\"T/api/v1/feature-views/{feature_view_id}/{feature_view_version}/retrieve-as-links-job:\x01*\x12\xbb\x01\n&GetRetrieveFeatureViewAsLinksJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a@.ai.h2o.featurestore.api.v1.RetrieveFeatureViewAsAsLinksResponse\",\x82\xd3\xe4\x93\x02&\x12$/api/v1/feature-views/links/{job_id}\x12\x92\x01\n\x11\x44\x65leteFeatureView\x12\x34.ai.h2o.featurestore.api.v1.DeleteFeatureViewRequest\x1a\x16.google.protobuf.Empty\"/\x82\xd3\xe4\x93\x02)*\'/api/v1/feature-views/{feature_view_id}\x12\x9a\x01\n\x0f\x43reateMLDataset\x12\x32.ai.h2o.featurestore.api.v1.CreateMLDatasetRequest\x1a\x33.ai.h2o.featurestore.api.v1.CreateMLDatasetResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\"\x13/api/v1/ml-datasets:\x01*\x12\xae\x01\n\x1dGetMLDatasetCreationJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a%.ai.h2o.featurestore.api.v1.MLDataset\"C\x82\xd3\xe4\x93\x02=\x12;/api/v1/ml-datasets//{ml_datasets_id}/creation-job/{job_id}\x12\x9c\x01\n\x0fUpdateMLDataset\x12\x32.ai.h2o.featurestore.api.v1.UpdateMLDatasetRequest\x1a%.ai.h2o.featurestore.api.v1.MLDataset\".\x82\xd3\xe4\x93\x02(\x1a#/api/v1/ml-datasets/{ml_dataset_id}:\x01*\x12\x8a\x01\n\x0f\x44\x65leteMLDataset\x12\x32.ai.h2o.featurestore.api.v1.DeleteMLDatasetRequest\x1a\x16.google.protobuf.Empty\"+\x82\xd3\xe4\x93\x02%*#/api/v1/ml-datasets/{ml_dataset_id}\x12\xc2\x01\n\x0cGetMLDataset\x12/.ai.h2o.featurestore.api.v1.GetMLDatasetRequest\x1a%.ai.h2o.featurestore.api.v1.MLDataset\"Z\x82\xd3\xe4\x93\x02T\x12R/api/v1/feature-views/{feature_view_id}/version/{feature_view_version}/ml-datasets\x12\xa5\x01\n\x0fMLDatasetExists\x12\x32.ai.h2o.featurestore.api.v1.MLDatasetExistsRequest\x1a*.ai.h2o.featurestore.api.v1.ExistsResponse\"2\x82\xd3\xe4\x93\x02,\x12*/api/v1/ml-datasets/{ml_dataset_id}/exists\x12\x94\x01\n\x0eListMLDatasets\x12\x31.ai.h2o.featurestore.api.v1.ListMLDatasetsRequest\x1a\x32.ai.h2o.featurestore.api.v1.ListMLDatasetsResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/api/v1/ml-datasets\x12\xcb\x01\n\x18RetrieveMLDatasetAsSpark\x12;.ai.h2o.featurestore.api.v1.RetrieveMLDatasetAsSparkRequest\x1a<.ai.h2o.featurestore.api.v1.RetrieveMLDatasetAsSparkResponse\"4\x82\xd3\xe4\x93\x02.\")/api/v1/ml-datasets/{ml_dataset_id}/spark:\x01*\x12\xad\x01\n StartRetrieveMLDatasetAsLinksJob\x12=.ai.h2o.featurestore.api.v1.RetrieveMLDatasetAsAsLinksRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"\'\x82\xd3\xe4\x93\x02!\"\x1c/api/v1/ml-datasets/retrieve:\x01*\x12\xb8\x01\n$GetRetrieveMLDatasetAsLinksJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a>.ai.h2o.featurestore.api.v1.RetrieveMLDatasetAsAsLinksResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/api/v1/ml-datasets/retrieve/{job_id}\x12\xe5\x01\n%GenerateMLDatasetOnlineRetrievalToken\x12?.ai.h2o.featurestore.api.v1.OnlineMLDataSetRetrieveTokenRequest\x1a\x37.ai.h2o.featurestore.api.v1.OnlineRetrieveTokenResponse\"B\x82\xd3\xe4\x93\x02<\x12:/api/v1/ml-datasets/{ml_dataset_id}/online/retrieval/token\x12\x97\x01\n\x10ListProjectsPage\x12\x33.ai.h2o.featurestore.api.v1.ListProjectsPageRequest\x1a\x34.ai.h2o.featurestore.api.v1.ListProjectsPageResponse\"\x18\x82\xd3\xe4\x93\x02\x12\x12\x10/api/v1/projects\x12\x91\x01\n\rCreateProject\x12\x30.ai.h2o.featurestore.api.v1.CreateProjectRequest\x1a\x31.ai.h2o.featurestore.api.v1.CreateProjectResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\"\x10/api/v1/projects:\x01*\x12\x91\x01\n\nGetProject\x12-.ai.h2o.featurestore.api.v1.GetProjectRequest\x1a+.ai.h2o.featurestore.api.v1.ProjectResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/api/v1/projects/{project_name}\x12\x97\x01\n\x0eGetProjectById\x12\x31.ai.h2o.featurestore.api.v1.GetProjectByIdRequest\x1a+.ai.h2o.featurestore.api.v1.ProjectResponse\"%\x82\xd3\xe4\x93\x02\x1f\x12\x1d/api/v1/projects/{project_id}\x12\x7f\n\rDeleteProject\x12\x30.ai.h2o.featurestore.api.v1.DeleteProjectRequest\x1a\x16.google.protobuf.Empty\"$\x82\xd3\xe4\x93\x02\x1e*\x1c/api/v1/projects/{projectId}\x12\x83\x01\n\x12GetProjectsDefault\x12\x16.google.protobuf.Empty\x1a\x33.ai.h2o.featurestore.api.v1.ProjectsDefaultResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/api/v1/projects/default\x12\x9b\x01\n\rProjectExists\x12\x30.ai.h2o.featurestore.api.v1.ProjectExistsRequest\x1a*.ai.h2o.featurestore.api.v1.ExistsResponse\",\x82\xd3\xe4\x93\x02&\x12$/api/v1/projects/{project_id}/exists\x12\x9e\x01\n\rUpdateProject\x12\x30.ai.h2o.featurestore.api.v1.UpdateProjectRequest\x1a\x31.ai.h2o.featurestore.api.v1.UpdateProjectResponse\"(\x82\xd3\xe4\x93\x02\"\x1a\x1d/api/v1/projects/{project_id}:\x01*\x12\xbe\x01\n\x16ListProjectHistoryPage\x12\x39.ai.h2o.featurestore.api.v1.ListProjectHistoryPageRequest\x1a:.ai.h2o.featurestore.api.v1.ListProjectHistoryPageResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/api/v1/projects/{project_id}/history\x12\x91\x01\n\x0eGetAccessToken\x12/.ai.h2o.featurestore.api.v1.RefreshTokenRequest\x1a/.ai.h2o.featurestore.api.v1.AccessTokenResponse\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/api/v1/auth/token:\x01*\x12k\n\x06Logout\x12).ai.h2o.featurestore.api.v1.LogoutRequest\x1a\x16.google.protobuf.Empty\"\x1e\x82\xd3\xe4\x93\x02\x18\"\x13/api/v1/auth/logout:\x01*\x12v\n\rGetActiveUser\x12\x16.google.protobuf.Empty\x1a\x31.ai.h2o.featurestore.api.v1.GetActiveUserResponse\"\x1a\x82\xd3\xe4\x93\x02\x14\x12\x12/api/v1/auth/users\x12k\n\x05Login\x12\x16.google.protobuf.Empty\x1a).ai.h2o.featurestore.api.v1.LoginResponse\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/api/v1/auth/login:\x01*0\x01\x12p\n\x0cGetWebConfig\x12\x16.google.protobuf.Empty\x1a\x30.ai.h2o.featurestore.api.v1.GetWebConfigResponse\"\x16\x82\xd3\xe4\x93\x02\x10\x12\x0e/api/v1/config\x12t\n\x0cGetApiConfig\x12\x16.google.protobuf.Empty\x1a\x30.ai.h2o.featurestore.api.v1.GetApiConfigResponse\"\x1a\x82\xd3\xe4\x93\x02\x14\x12\x12/api/v1/api-config\x12~\n\x10GetH2OGpteConfig\x12\x16.google.protobuf.Empty\x1a\x31.ai.h2o.featurestore.api.v1.GetGpteConfigResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/api/v1/h2o-gpte-config\x12\xb7\x01\n\x17\x41\x64\x64\x46\x65\x61tureSetPermission\x12\x37.ai.h2o.featurestore.api.v1.FeatureSetPermissionRequest\x1a\x16.google.protobuf.Empty\"K\x82\xd3\xe4\x93\x02\x45\"@/api/v1/permissions/feature-sets/add/permission/{feature_set_id}:\x01*\x12\xa9\x01\n\x14\x41\x64\x64ProjectPermission\x12\x34.ai.h2o.featurestore.api.v1.ProjectPermissionRequest\x1a\x16.google.protobuf.Empty\"C\x82\xd3\xe4\x93\x02=\"8/api/v1/permissions/projects/add/permission/{project_id}:\x01*\x12\xbd\x01\n\x1aRemoveFeatureSetPermission\x12\x37.ai.h2o.featurestore.api.v1.FeatureSetPermissionRequest\x1a\x16.google.protobuf.Empty\"N\x82\xd3\xe4\x93\x02H*C/api/v1/permissions/feature-sets/remove/permission/{feature_set_id}:\x01*\x12\xaf\x01\n\x17RemoveProjectPermission\x12\x34.ai.h2o.featurestore.api.v1.ProjectPermissionRequest\x1a\x16.google.protobuf.Empty\"F\x82\xd3\xe4\x93\x02@*;/api/v1/permissions/projects/remove/permission/{project_id}:\x01*\x12\xd0\x01\n\x1eSubmitPendingProjectPermission\x12:.ai.h2o.featurestore.api.v1.SubmitPendingPermissionRequest\x1a;.ai.h2o.featurestore.api.v1.SubmitPendingPermissionResponse\"5\x82\xd3\xe4\x93\x02/\"*/api/v1/permissions/projects/{resource_id}:\x01*\x12\xd7\x01\n!SubmitPendingFeatureSetPermission\x12:.ai.h2o.featurestore.api.v1.SubmitPendingPermissionRequest\x1a;.ai.h2o.featurestore.api.v1.SubmitPendingPermissionResponse\"9\x82\xd3\xe4\x93\x02\x33\"./api/v1/permissions/feature-sets/{resource_id}:\x01*\x12\xbb\x01\n\x1aListProjectPermissionsPage\x12\x36.ai.h2o.featurestore.api.v1.ListPermissionsPageRequest\x1a?.ai.h2o.featurestore.api.v1.ListProjectsPermissionsPageResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/api/v1/permissions/projects\x12\xc6\x01\n\x1eListFeatureSetsPermissionsPage\x12\x36.ai.h2o.featurestore.api.v1.ListPermissionsPageRequest\x1a\x42.ai.h2o.featurestore.api.v1.ListFeatureSetsPermissionsPageResponse\"(\x82\xd3\xe4\x93\x02\"\x12 /api/v1/permissions/feature-sets\x12\xd0\x01\n$ListManageableProjectPermissionsPage\x12\x36.ai.h2o.featurestore.api.v1.ListPermissionsPageRequest\x1a?.ai.h2o.featurestore.api.v1.ListProjectsPermissionsPageResponse\"/\x82\xd3\xe4\x93\x02)\x12\'/api/v1/permissions/manageable-projects\x12\xdb\x01\n(ListManageableFeatureSetsPermissionsPage\x12\x36.ai.h2o.featurestore.api.v1.ListPermissionsPageRequest\x1a\x42.ai.h2o.featurestore.api.v1.ListFeatureSetsPermissionsPageResponse\"3\x82\xd3\xe4\x93\x02-\x12+/api/v1/permissions/manageable-feature-sets\x12\x98\x01\n\x18\x41pprovePendingPermission\x12;.ai.h2o.featurestore.api.v1.ApprovePendingPermissionRequest\x1a\x16.google.protobuf.Empty\"\'\x82\xd3\xe4\x93\x02!\"\x1c/api/v1/permissions/approval:\x01*\x12\x97\x01\n\x17RejectPendingPermission\x12:.ai.h2o.featurestore.api.v1.RejectPendingPermissionRequest\x1a\x16.google.protobuf.Empty\"(\x82\xd3\xe4\x93\x02\"\"\x1d/api/v1/permissions/rejection:\x01*\x12\x9a\x01\n\x19WithdrawPendingPermission\x12<.ai.h2o.featurestore.api.v1.WithdrawPendingPermissionRequest\x1a\x16.google.protobuf.Empty\"\'\x82\xd3\xe4\x93\x02!\"\x1c/api/v1/permissions/withdraw:\x01*\x12\x86\x01\n\x10RevokePermission\x12\x33.ai.h2o.featurestore.api.v1.RevokePermissionRequest\x1a\x16.google.protobuf.Empty\"%\x82\xd3\xe4\x93\x02\x1f\"\x1a/api/v1/permissions/revoke:\x01*\x12\xc8\x01\n\x1aGetActiveProjectPermission\x12\x36.ai.h2o.featurestore.api.v1.GetActivePermissionRequest\x1a\x37.ai.h2o.featurestore.api.v1.GetActivePermissionResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/api/v1/permissions/projects/{resource_id}/active\x12\xcf\x01\n\x1dGetActiveFeatureSetPermission\x12\x36.ai.h2o.featurestore.api.v1.GetActivePermissionRequest\x1a\x37.ai.h2o.featurestore.api.v1.GetActivePermissionResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/api/v1/permissions/feature-sets/{resource_id}/active\x12\xbe\x01\n\x19GetUserProjectPermissions\x12\x35.ai.h2o.featurestore.api.v1.GetUserPermissionsRequest\x1a\x36.ai.h2o.featurestore.api.v1.GetUserPermissionsResponse\"2\x82\xd3\xe4\x93\x02,\x12*/api/v1/permissions/projects/{resource_id}\x12\xc5\x01\n\x1cGetUserFeatureSetPermissions\x12\x35.ai.h2o.featurestore.api.v1.GetUserPermissionsRequest\x1a\x36.ai.h2o.featurestore.api.v1.GetUserPermissionsResponse\"6\x82\xd3\xe4\x93\x02\x30\x12./api/v1/permissions/feature-sets/{resource_id}\x12\xd1\x01\n\x1fGetUserActiveProjectPermissions\x12;.ai.h2o.featurestore.api.v1.GetUserActivePermissionsRequest\x1a\x36.ai.h2o.featurestore.api.v1.GetUserPermissionsResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/api/v1/permissions/projects/active/{resource_id}\x12\xd8\x01\n\"GetUserActiveFeatureSetPermissions\x12;.ai.h2o.featurestore.api.v1.GetUserActivePermissionsRequest\x1a\x36.ai.h2o.featurestore.api.v1.GetUserPermissionsResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/api/v1/permissions/feature-sets/active/{resource_id}\x12\xe8\x01\n!GetUsersWithoutProjectPermissions\x12<.ai.h2o.featurestore.api.v1.GetUsersWithoutPermissionRequest\x1a=.ai.h2o.featurestore.api.v1.GetUsersWithoutPermissionResponse\"F\x82\xd3\xe4\x93\x02@\x12>/api/v1/permissions/projects/{resourceId}/user/permission/none\x12\xef\x01\n$GetUsersWithoutFeatureSetPermissions\x12<.ai.h2o.featurestore.api.v1.GetUsersWithoutPermissionRequest\x1a=.ai.h2o.featurestore.api.v1.GetUsersWithoutPermissionResponse\"J\x82\xd3\xe4\x93\x02\x44\x12\x42/api/v1/permissions/feature-sets/{resourceId}/user/permission/none\x12w\n\x0bRevokeToken\x12(.ai.h2o.featurestore.api.v1.TokenRequest\x1a\x16.google.protobuf.Empty\"&\x82\xd3\xe4\x93\x02 *\x1e/api/v1/auth/tokens/{token_id}\x12\x8f\x01\n\rGenerateToken\x12\x30.ai.h2o.featurestore.api.v1.GenerateTokenRequest\x1a,.ai.h2o.featurestore.api.v1.RawTokenResponse\"\x1e\x82\xd3\xe4\x93\x02\x18\"\x13/api/v1/auth/tokens:\x01*\x12\xb2\x01\n\x18ListPersonalAccessTokens\x12;.ai.h2o.featurestore.api.v1.ListPersonalAccessTokensRequest\x1a<.ai.h2o.featurestore.api.v1.ListPersonalAccessTokensResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/api/v1/auth/tokens\x12\x87\x01\n\x08GetToken\x12(.ai.h2o.featurestore.api.v1.TokenRequest\x1a).ai.h2o.featurestore.api.v1.TokenResponse\"&\x82\xd3\xe4\x93\x02 \x12\x1e/api/v1/auth/tokens/{token_id}\x12\x7f\n\x0fGetTokensConfig\x12\x16.google.protobuf.Empty\x1a\x30.ai.h2o.featurestore.api.v1.TokensConfigResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/auth/tokens/config\x12\xda\x01\n\x13GenerateIngestToken\x12\x37.ai.h2o.featurestore.api.v1.OnlineIngestionTokenRequest\x1a\x38.ai.h2o.featurestore.api.v1.OnlineIngestionTokenResponse\"P\x82\xd3\xe4\x93\x02J\x12H/api/v1/feature-sets/{feature_set_id}/{feature_set_version}/online/token\x12\xeb\x01\n\x1cGenerateOnlineRetrievalToken\x12\x36.ai.h2o.featurestore.api.v1.OnlineRetrieveTokenRequest\x1a\x37.ai.h2o.featurestore.api.v1.OnlineRetrieveTokenResponse\"Z\x82\xd3\xe4\x93\x02T\x12R/api/v1/feature-sets/{feature_set_id}/{feature_set_version}/online/retrieval/token\x12\xca\x01\n\x1dStartMaterializationOnlineJob\x12=.ai.h2o.featurestore.api.v1.StartMaterializationOnlineRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"G\x82\xd3\xe4\x93\x02\x41\"</api/v1/feature-sets/{feature_set_id}/online-materialization:\x01*\x12\xbe\x01\n!GetMaterializationOnlineJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x39.ai.h2o.featurestore.api.v1.MaterializationOnlineResponse\";\x82\xd3\xe4\x93\x02\x35\x12\x33/api/v1/jobs/{job_id}/output/online-materialization\x12\xe4\x01\n\x1eStartOnlineOfflineIngestionJob\x12>.ai.h2o.featurestore.api.v1.StartOnlineOfflineIngestionRequest\x1a!.ai.h2o.featurestore.api.v1.JobId\"_\x82\xd3\xe4\x93\x02Y\"T/api/v1/feature-sets/{feature_set_id}/{feature_set_version}/online-offline-ingestion:\x01*\x12\x87\x01\n\x1dGetComputeStatisticsJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x16.google.protobuf.Empty\"+\x82\xd3\xe4\x93\x02%\x12#/api/v1/compute-statistics/{job_id}\x12\xb6\x01\n,GetComputeRecommendationClassifiersJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a\x16.google.protobuf.Empty\"K\x82\xd3\xe4\x93\x02\x45\x12\x43/api/v1/jobs/{job_id}/output/recommendation-classifiers-computation\x12\xc5\x01\n\x1cGenerateTransformationUpload\x12?.ai.h2o.featurestore.api.v1.GenerateTransformationUploadRequest\x1a@.ai.h2o.featurestore.api.v1.GenerateTransformationUploadResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/api/v1/transformations:\x01*\x12\x96\x01\n\x1dListRecommendationClassifiers\x12\x16.google.protobuf.Empty\x1a@.ai.h2o.featurestore.api.v1.ListRecommendationClassifierResponse\"\x1b\x82\xd3\xe4\x93\x02\x15\x12\x13/api/v1/classifiers\x12\x9b\x01\n\x1e\x43reateRecommendationClassifier\x12\x41.ai.h2o.featurestore.api.v1.CreateRecommendationClassifierRequest\x1a\x16.google.protobuf.Empty\"\x1e\x82\xd3\xe4\x93\x02\x18\"\x13/api/v1/classifiers:\x01*\x12\xa2\x01\n\x1eUpdateRecommendationClassifier\x12\x41.ai.h2o.featurestore.api.v1.UpdateRecommendationClassifierRequest\x1a\x16.google.protobuf.Empty\"%\x82\xd3\xe4\x93\x02\x1f\x1a\x1a/api/v1/classifiers/{name}:\x01*\x12\xaa\x01\n\x1e\x44\x65leteRecommendationClassifier\x12\x41.ai.h2o.featurestore.api.v1.DeleteRecommendationClassifierRequest\x1a\x16.google.protobuf.Empty\"-\x82\xd3\xe4\x93\x02\'*%/api/v1/classifiers/{classifier_name}\x12\xc0\x01\n\x12GetRecommendations\x12\x34.ai.h2o.featurestore.api.v1.GetRecommendationRequest\x1a\x35.ai.h2o.featurestore.api.v1.GetRecommendationResponse\"=\x82\xd3\xe4\x93\x02\x37\x12\x35/api/v1/feature-sets/{feature_set_id}/recommendations\x12p\n\x0cGetDashboard\x12\x16.google.protobuf.Empty\x1a-.ai.h2o.featurestore.api.v1.DashboardResponse\"\x19\x82\xd3\xe4\x93\x02\x13\x12\x11/api/v1/dashboard\x12\x9d\x01\n\x18GetFeatureSetsPopularity\x12\x16.google.protobuf.Empty\x1a\x39.ai.h2o.featurestore.api.v1.FeatureSetsPopularityResponse\".\x82\xd3\xe4\x93\x02(\x12&/api/v1/dashboard/popular-feature-sets\x12\x9d\x01\n\x17GetRecentlyUsedProjects\x12\x16.google.protobuf.Empty\x1a\x38.ai.h2o.featurestore.api.v1.RecentlyUsedProjectsResponse\"0\x82\xd3\xe4\x93\x02*\x12(/api/v1/dashboard/recently-used-projects\x12\xa7\x01\n\x1aGetRecentlyUsedFeatureSets\x12\x16.google.protobuf.Empty\x1a;.ai.h2o.featurestore.api.v1.RecentlyUsedFeatureSetsResponse\"4\x82\xd3\xe4\x93\x02.\x12,/api/v1/dashboard/recently-used-feature-sets\x12\x9c\x01\n\rPinFeatureSet\x12\x30.ai.h2o.featurestore.api.v1.PinFeatureSetRequest\x1a\x16.google.protobuf.Empty\"A\x82\xd3\xe4\x93\x02;\x1a\x36/api/v1/dashboard/pinned-feature-sets/{feature_set_id}:\x01*\x12\xa0\x01\n\x0fUnpinFeatureSet\x12\x32.ai.h2o.featurestore.api.v1.UnpinFeatureSetRequest\x1a\x16.google.protobuf.Empty\"A\x82\xd3\xe4\x93\x02;*6/api/v1/dashboard/pinned-feature-sets/{feature_set_id}:\x01*\x12\xcd\x01\n\x12IsFeatureSetPinned\x12\x35.ai.h2o.featurestore.api.v1.IsFeatureSetPinnedRequest\x1a\x36.ai.h2o.featurestore.api.v1.IsFeatureSetPinnedResponse\"H\x82\xd3\xe4\x93\x02\x42\x12=/api/v1/dashboard/pinned-feature-sets/exists/{feature_set_id}:\x01*\x12\xb3\x01\n\x15ListPinnedFeatureSets\x12\x34.ai.h2o.featurestore.api.v1.PinnedFeatureSetsRequest\x1a\x35.ai.h2o.featurestore.api.v1.PinnedFeatureSetsResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/api/v1/dashboard/pinned-feature-sets\x12\x95\x01\n\x0eSearchProjects\x12\x30.ai.h2o.featurestore.api.v1.ProjectSearchRequest\x1a\x30.ai.h2o.featurestore.api.v1.ProjectSearchResults\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/api/v1/search/projects\x12\xa2\x01\n\x11SearchFeatureSets\x12\x33.ai.h2o.featurestore.api.v1.FeatureSetSearchRequest\x1a\x33.ai.h2o.featurestore.api.v1.FeatureSetSearchResults\"#\x82\xd3\xe4\x93\x02\x1d\x12\x1b/api/v1/search/feature-sets\x12\x95\x01\n\x0eSearchFeatures\x12\x30.ai.h2o.featurestore.api.v1.FeatureSearchRequest\x1a\x30.ai.h2o.featurestore.api.v1.FeatureSearchResults\"\x1f\x82\xd3\xe4\x93\x02\x19\x12\x17/api/v1/search/features\x12\xad\x01\n\nGetFeature\x12-.ai.h2o.featurestore.api.v1.GetFeatureRequest\x1a+.ai.h2o.featurestore.api.v1.FeatureResponse\"C\x82\xd3\xe4\x93\x02=\x12;/api/v1/feature-sets/{feature_set_id}/features/{feature_id}\x12\xa9\x01\n\x0cListFeatures\x12/.ai.h2o.featurestore.api.v1.ListFeaturesRequest\x1a\x30.ai.h2o.featurestore.api.v1.ListFeaturesResponse\"6\x82\xd3\xe4\x93\x02\x30\x12./api/v1/feature-sets/{feature_set_id}/features\x12\xbc\x01\n\rUpdateFeature\x12\x30.ai.h2o.featurestore.api.v1.UpdateFeatureRequest\x1a\x31.ai.h2o.featurestore.api.v1.UpdateFeatureResponse\"F\x82\xd3\xe4\x93\x02@\x1a;/api/v1/feature-sets/{feature_set_id}/features/{feature_id}:\x01*\x12\xac\x01\n\x13MarkFeatureAsTarget\x12\x30.ai.h2o.featurestore.api.v1.TargetFeatureRequest\x1a\x16.google.protobuf.Empty\"K\x82\xd3\xe4\x93\x02\x45\x1a\x43/api/v1/feature-sets/{feature_set_id}/target-variables/{feature_id}\x12\xaf\x01\n\x16\x44iscardFeatureAsTarget\x12\x30.ai.h2o.featurestore.api.v1.TargetFeatureRequest\x1a\x16.google.protobuf.Empty\"K\x82\xd3\xe4\x93\x02\x45*C/api/v1/feature-sets/{feature_set_id}/target-variables/{feature_id}\x12\xc3\x01\n\x12ListTargetFeatures\x12\x35.ai.h2o.featurestore.api.v1.ListTargetFeaturesRequest\x1a\x36.ai.h2o.featurestore.api.v1.ListTargetFeaturesResponse\">\x82\xd3\xe4\x93\x02\x38\x12\x36/api/v1/feature-sets/{feature_set_id}/target-variables\x12\xbe\x01\n\x15GetListableFeatureSet\x12\x35.ai.h2o.featurestore.api.v1.ListableFeatureSetRequest\x1a\x36.ai.h2o.featurestore.api.v1.ListableFeatureSetResponse\"6\x82\xd3\xe4\x93\x02\x30\x12./api/v1/feature-sets/{feature_set_id}/listable\x12\xce\x01\n\x19GetFeatureSetsDerivedFrom\x12\x39.ai.h2o.featurestore.api.v1.FeatureSetsDerivedFromRequest\x1a:.ai.h2o.featurestore.api.v1.FeatureSetsDerivedFromResponse\":\x82\xd3\xe4\x93\x02\x34\x12\x32/api/v1/feature-sets/{feature_set_id}/derived-from\x12\x9f\x01\n\x11ScheduleIngestJob\x12/.ai.h2o.featurestore.api.v1.ScheduleTaskRequest\x1a\x31.ai.h2o.featurestore.api.v1.ScheduledTaskResponse\"&\x82\xd3\xe4\x93\x02 \"\x1b/api/v1/schedules/ingestion:\x01*\x12\xbc\x01\n\x12ListScheduledTasks\x12\x35.ai.h2o.featurestore.api.v1.ListScheduledTasksRequest\x1a\x36.ai.h2o.featurestore.api.v1.ListScheduledTasksResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//api/v1/feature-sets/{feature_set_id}/schedules\x12\xa1\x01\n\x10GetScheduledTask\x12+.ai.h2o.featurestore.api.v1.ScheduledTaskId\x1a\x31.ai.h2o.featurestore.api.v1.ScheduledTaskResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/api/v1/schedules/{scheduled_task_id}\x12\x89\x01\n\x13\x44\x65leteScheduledTask\x12+.ai.h2o.featurestore.api.v1.ScheduledTaskId\x1a\x16.google.protobuf.Empty\"-\x82\xd3\xe4\x93\x02\'*%/api/v1/schedules/{scheduled_task_id}\x12\x97\x01\n\x13UpdateScheduledTask\x12\x36.ai.h2o.featurestore.api.v1.ScheduledTaskUpdateRequest\x1a\x16.google.protobuf.Empty\"0\x82\xd3\xe4\x93\x02*\x1a%/api/v1/schedules/{scheduled_task_id}:\x01*\x12\x9b\x01\n\x12PauseScheduledTask\x12\x35.ai.h2o.featurestore.api.v1.PauseScheduledTaskRequest\x1a\x16.google.protobuf.Empty\"6\x82\xd3\xe4\x93\x02\x30\x1a+/api/v1/schedules/{scheduled_task_id}/pause:\x01*\x12\x9e\x01\n\x13ResumeScheduledTask\x12\x36.ai.h2o.featurestore.api.v1.ResumeScheduledTaskRequest\x1a\x16.google.protobuf.Empty\"7\x82\xd3\xe4\x93\x02\x31\x1a,/api/v1/schedules/{scheduled_task_id}/resume:\x01*\x12\xa9\x01\n\x16ScheduleLazyIngestTask\x12/.ai.h2o.featurestore.api.v1.ScheduleTaskRequest\x1a\x31.ai.h2o.featurestore.api.v1.ScheduledTaskResponse\"+\x82\xd3\xe4\x93\x02%\" /api/v1/schedules/lazy/ingestion:\x01*\x12\xa4\x01\n\x13StartLazyIngestTask\x12-.ai.h2o.featurestore.api.v1.LazyIngestRequest\x1a..ai.h2o.featurestore.api.v1.LazyIngestResponse\".\x82\xd3\xe4\x93\x02(\x12&/api/v1/schedules/lazy/ingestion/start\x12\xcd\x01\n\x11GetLazyIngestTask\x12\x34.ai.h2o.featurestore.api.v1.GetLazyIngestTaskRequest\x1a\x31.ai.h2o.featurestore.api.v1.ScheduledTaskResponse\"O\x82\xd3\xe4\x93\x02I\x12G/api/v1/schedules/lazy/ingestion/{feature_set_id}/{feature_set_version}\x12\xe8\x01\n!ListScheduledTaskExecutionHistory\x12>.ai.h2o.featurestore.api.v1.ListScheduledTaskExecutionsRequest\x1a?.ai.h2o.featurestore.api.v1.ListScheduledTaskExecutionsResponse\"B\x82\xd3\xe4\x93\x02<\x12\x37/api/v1/schedules/{scheduled_task_id}/execution-history:\x01*\x12\xc8\x01\n\x1bListTransformationFunctions\x12>.ai.h2o.featurestore.api.v1.ListTransformationFunctionsRequest\x1a?.ai.h2o.featurestore.api.v1.ListTransformationFunctionsResponse\"(\x82\xd3\xe4\x93\x02\"\x12 /api/v1/transformation_functions\x12\xe1\x01\n\x19GetTransformationFunction\x12<.ai.h2o.featurestore.api.v1.GetTransformationFunctionRequest\x1a=.ai.h2o.featurestore.api.v1.GetTransformationFunctionResponse\"G\x82\xd3\xe4\x93\x02\x41\x12?/api/v1/transformation_functions/{transformation_function_name}\x12\x96\x01\n\x14GetBackfillJobOutput\x12!.ai.h2o.featurestore.api.v1.JobId\x1a,.ai.h2o.featurestore.api.v1.BackfillResponse\"-\x82\xd3\xe4\x93\x02\'\x12%/api/v1/jobs/{job_id}/output/backfill\x12\x8a\x01\n\x15\x43reateDraftFeatureSet\x12\x32.ai.h2o.featurestore.api.v1.FeatureSetDraftRequest\x1a\x16.google.protobuf.Empty\"%\x82\xd3\xe4\x93\x02\x1f\"\x1a/api/v1/feature-sets/draft:\x01*\x12\xb0\x01\n!CreateMajorVersionDraftFeatureSet\x12>.ai.h2o.featurestore.api.v1.FeatureSetMajorVersionDraftRequest\x1a\x16.google.protobuf.Empty\"3\x82\xd3\xe4\x93\x02-\"(/api/v1/feature-sets/draft-major-version:\x01*\x12\xb7\x01\n\x19\x43reateFeatureSetFromDraft\x12\x34.ai.h2o.featurestore.api.v1.DraftToFeatureSetRequest\x1a\x35.ai.h2o.featurestore.api.v1.DraftToFeatureSetResponse\"-\x82\xd3\xe4\x93\x02\'\"\"/api/v1/feature-sets/draft/publish:\x01*\x12\xfe\x01\n,CreateFeatureSetVersionFromMajorVersionDraft\x12G.ai.h2o.featurestore.api.v1.MajorVersionDraftToFeatureSetVersionRequest\x1aH.ai.h2o.featurestore.api.v1.MajorVersionDraftToFeatureSetVersionResponse\";\x82\xd3\xe4\x93\x02\x35\"0/api/v1/feature-sets/draft-major-version/publish:\x01*\x12\x99\x01\n\x15\x44\x65leteFeatureSetDraft\x12-.ai.h2o.featurestore.api.v1.FeatureSetDraftId\x1a\x16.google.protobuf.Empty\"9\x82\xd3\xe4\x93\x02\x33*1/api/v1/feature-sets/draft/{feature_set_draft_id}\x12\xad\x01\n\x14ListFeatureSetDrafts\x12\x37.ai.h2o.featurestore.api.v1.ListFeatureSetDraftsRequest\x1a\x38.ai.h2o.featurestore.api.v1.ListFeatureSetDraftsResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/feature-sets/draft\x12\xb3\x01\n\x12GetFeatureSetDraft\x12-.ai.h2o.featurestore.api.v1.FeatureSetDraftId\x1a\x33.ai.h2o.featurestore.api.v1.FeatureSetDraftResponse\"9\x82\xd3\xe4\x93\x02\x33\x12\x31/api/v1/feature-sets/draft/{feature_set_draft_id}\x12\xa4\x01\n\x11StoreFileArtifact\x12\x34.ai.h2o.featurestore.api.v1.StoreFileArtifactRequest\x1a\x35.ai.h2o.featurestore.api.v1.StoreFileArtifactResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/api/v1/artifacts/files:\x01*\x12\xa6\x01\n\x10RetrieveArtifact\x12\x33.ai.h2o.featurestore.api.v1.RetrieveArtifactRequest\x1a\x34.ai.h2o.featurestore.api.v1.RetrieveArtifactResponse\"\'\x82\xd3\xe4\x93\x02!\x12\x1f/api/v1/artifacts/{artifact_id}\x12\x96\x01\n\x12UpdateUploadStatus\x12\x35.ai.h2o.featurestore.api.v1.UpdateUploadStatusRequest\x1a\x16.google.protobuf.Empty\"1\x82\xd3\xe4\x93\x02+\x1a&/api/v1/artifacts/{artifact_id}/status:\x01*\x12\x84\x01\n\x0e\x44\x65leteArtifact\x12\x31.ai.h2o.featurestore.api.v1.DeleteArtifactRequest\x1a\x16.google.protobuf.Empty\"\'\x82\xd3\xe4\x93\x02!*\x1f/api/v1/artifacts/{artifact_id}\x12\xbc\x01\n\rListArtifacts\x12\x30.ai.h2o.featurestore.api.v1.ListArtifactsRequest\x1a\x31.ai.h2o.featurestore.api.v1.ListArtifactsResponse\"F\x82\xd3\xe4\x93\x02@\x12>/api/v1/artifacts/{feature_set_id}/{feature_set_major_version}\x12\x8c\x01\n\tStoreLink\x12,.ai.h2o.featurestore.api.v1.StoreLinkRequest\x1a-.ai.h2o.featurestore.api.v1.StoreLinkResponse\"\"\x82\xd3\xe4\x93\x02\x1c\"\x17/api/v1/artifacts/links:\x01*\x12\xcf\x01\n\x10GetCodeSnippedId\x12\x30.ai.h2o.featurestore.api.v1.CodeSnippedIdRequest\x1a\x31.ai.h2o.featurestore.api.v1.CodeSnippedIdResponse\"V\x82\xd3\xe4\x93\x02P\x12N/api/v1/artifacts/{feature_set_id}/{feature_set_major_version}/code-snipped-id\x12\xab\x01\n\x17ListFeatureSetsToReview\x12:.ai.h2o.featurestore.api.v1.ListFeatureSetsToReviewRequest\x1a;.ai.h2o.featurestore.api.v1.ListFeatureSetsToReviewResponse\"\x17\x82\xd3\xe4\x93\x02\x11\x12\x0f/api/v1/reviews\x12\x8a\x01\n\rApproveReview\x12\x30.ai.h2o.featurestore.api.v1.ApproveReviewRequest\x1a\x16.google.protobuf.Empty\"/\x82\xd3\xe4\x93\x02)\"$/api/v1/reviews/{review_id}/approval:\x01*\x12\x89\x01\n\x0cRejectReview\x12/.ai.h2o.featurestore.api.v1.RejectReviewRequest\x1a\x16.google.protobuf.Empty\"0\x82\xd3\xe4\x93\x02*\"%/api/v1/reviews/{review_id}/rejection:\x01*\x12\xbd\x01\n\x1aListFeatureSetsReviewsPage\x12<.ai.h2o.featurestore.api.v1.ListFeatureSetReviewsPageRequest\x1a=.ai.h2o.featurestore.api.v1.ListFeatureSetReviewsPageResponse\"\"\x82\xd3\xe4\x93\x02\x1c\x12\x1a/api/v1/reviews/my-reviews\x12\xde\x01\n\x1dGetListableFeatureSetToReview\x12@.ai.h2o.featurestore.api.v1.GetListableFeatureSetToReviewRequest\x1a\x41.ai.h2o.featurestore.api.v1.GetListableFeatureSetToReviewResponse\"8\x82\xd3\xe4\x93\x02\x32\x12\x30/api/v1/reviews/{review_id}/listable/feature-set\x12\xe9\x01\n\x1dGetListableFeatureSetInReview\x12@.ai.h2o.featurestore.api.v1.GetListableFeatureSetInReviewRequest\x1a\x41.ai.h2o.featurestore.api.v1.GetListableFeatureSetInReviewResponse\"C\x82\xd3\xe4\x93\x02=\x12;/api/v1/reviews/my-reviews/{review_id}/listable/feature-set\x12\xb2\x01\n\x1f\x44\x65leteFeatureSetVersionInReview\x12;.ai.h2o.featurestore.api.v1.DeleteRejectedFeatureSetRequest\x1a\x16.google.protobuf.Empty\":\x82\xd3\xe4\x93\x02\x34*2/api/v1/reviews/my-reviews/{review_id}/feature-set\x12\xcc\x01\n\x14ListFeaturesToReview\x12\x37.ai.h2o.featurestore.api.v1.ListFeaturesToReviewRequest\x1a\x38.ai.h2o.featurestore.api.v1.ListFeaturesToReviewResponse\"A\x82\xd3\xe4\x93\x02;\x12\x39/api/v1/reviews/{review_id}/listable/feature-set/features\x12\xd7\x01\n\x14ListFeaturesInReview\x12\x37.ai.h2o.featurestore.api.v1.ListFeaturesInReviewRequest\x1a\x38.ai.h2o.featurestore.api.v1.ListFeaturesInReviewResponse\"L\x82\xd3\xe4\x93\x02\x46\x12\x44/api/v1/reviews/my-reviews/{review_id}/listable/feature-set/features\x12\xda\x01\n\x1cGetFeatureSetPreviewToReview\x12?.ai.h2o.featurestore.api.v1.GetFeatureSetPreviewToReviewRequest\x1a@.ai.h2o.featurestore.api.v1.GetFeatureSetPreviewToReviewResponse\"7\x82\xd3\xe4\x93\x02\x31\x12//api/v1/reviews/{review_id}/feature-set/preview\x12\xe5\x01\n\x1cGetFeatureSetPreviewInReview\x12?.ai.h2o.featurestore.api.v1.GetFeatureSetPreviewInReviewRequest\x1a@.ai.h2o.featurestore.api.v1.GetFeatureSetPreviewInReviewResponse\"B\x82\xd3\xe4\x93\x02<\x12:/api/v1/reviews/my-reviews/{review_id}/feature-set/preview\x12\xbd\x01\n\x15GetFeatureSetToReview\x12\x38.ai.h2o.featurestore.api.v1.GetFeatureSetToReviewRequest\x1a\x39.ai.h2o.featurestore.api.v1.GetFeatureSetToReviewResponse\"/\x82\xd3\xe4\x93\x02)\x12\'/api/v1/reviews/{review_id}/feature-set\x12\xc8\x01\n\x15GetFeatureSetInReview\x12\x38.ai.h2o.featurestore.api.v1.GetFeatureSetInReviewRequest\x1a\x39.ai.h2o.featurestore.api.v1.GetFeatureSetInReviewResponse\":\x82\xd3\xe4\x93\x02\x34\x12\x32/api/v1/reviews/my-reviews/{review_id}/feature-setB\x14\x42\x10\x43oreServiceProtoP\x01\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ai.h2o.featurestore.api.v1.CoreService_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'B\020CoreServiceProtoP\001'
@@ -193,14 +193,16 @@
   _globals['_CORESERVICE'].methods_by_name['GetActiveUser']._serialized_options = b'\202\323\344\223\002\024\022\022/api/v1/auth/users'
   _globals['_CORESERVICE'].methods_by_name['Login']._options = None
   _globals['_CORESERVICE'].methods_by_name['Login']._serialized_options = b'\202\323\344\223\002\027\"\022/api/v1/auth/login:\001*'
   _globals['_CORESERVICE'].methods_by_name['GetWebConfig']._options = None
   _globals['_CORESERVICE'].methods_by_name['GetWebConfig']._serialized_options = b'\202\323\344\223\002\020\022\016/api/v1/config'
   _globals['_CORESERVICE'].methods_by_name['GetApiConfig']._options = None
   _globals['_CORESERVICE'].methods_by_name['GetApiConfig']._serialized_options = b'\202\323\344\223\002\024\022\022/api/v1/api-config'
+  _globals['_CORESERVICE'].methods_by_name['GetH2OGpteConfig']._options = None
+  _globals['_CORESERVICE'].methods_by_name['GetH2OGpteConfig']._serialized_options = b'\202\323\344\223\002\031\022\027/api/v1/h2o-gpte-config'
   _globals['_CORESERVICE'].methods_by_name['AddFeatureSetPermission']._options = None
   _globals['_CORESERVICE'].methods_by_name['AddFeatureSetPermission']._serialized_options = b'\202\323\344\223\002E\"@/api/v1/permissions/feature-sets/add/permission/{feature_set_id}:\001*'
   _globals['_CORESERVICE'].methods_by_name['AddProjectPermission']._options = None
   _globals['_CORESERVICE'].methods_by_name['AddProjectPermission']._serialized_options = b'\202\323\344\223\002=\"8/api/v1/permissions/projects/add/permission/{project_id}:\001*'
   _globals['_CORESERVICE'].methods_by_name['RemoveFeatureSetPermission']._options = None
   _globals['_CORESERVICE'].methods_by_name['RemoveFeatureSetPermission']._serialized_options = b'\202\323\344\223\002H*C/api/v1/permissions/feature-sets/remove/permission/{feature_set_id}:\001*'
   _globals['_CORESERVICE'].methods_by_name['RemoveProjectPermission']._options = None
@@ -255,14 +257,16 @@
   _globals['_CORESERVICE'].methods_by_name['GenerateIngestToken']._serialized_options = b'\202\323\344\223\002J\022H/api/v1/feature-sets/{feature_set_id}/{feature_set_version}/online/token'
   _globals['_CORESERVICE'].methods_by_name['GenerateOnlineRetrievalToken']._options = None
   _globals['_CORESERVICE'].methods_by_name['GenerateOnlineRetrievalToken']._serialized_options = b'\202\323\344\223\002T\022R/api/v1/feature-sets/{feature_set_id}/{feature_set_version}/online/retrieval/token'
   _globals['_CORESERVICE'].methods_by_name['StartMaterializationOnlineJob']._options = None
   _globals['_CORESERVICE'].methods_by_name['StartMaterializationOnlineJob']._serialized_options = b'\202\323\344\223\002A\"</api/v1/feature-sets/{feature_set_id}/online-materialization:\001*'
   _globals['_CORESERVICE'].methods_by_name['GetMaterializationOnlineJobOutput']._options = None
   _globals['_CORESERVICE'].methods_by_name['GetMaterializationOnlineJobOutput']._serialized_options = b'\202\323\344\223\0025\0223/api/v1/jobs/{job_id}/output/online-materialization'
+  _globals['_CORESERVICE'].methods_by_name['StartOnlineOfflineIngestionJob']._options = None
+  _globals['_CORESERVICE'].methods_by_name['StartOnlineOfflineIngestionJob']._serialized_options = b'\202\323\344\223\002Y\"T/api/v1/feature-sets/{feature_set_id}/{feature_set_version}/online-offline-ingestion:\001*'
   _globals['_CORESERVICE'].methods_by_name['GetComputeStatisticsJobOutput']._options = None
   _globals['_CORESERVICE'].methods_by_name['GetComputeStatisticsJobOutput']._serialized_options = b'\202\323\344\223\002%\022#/api/v1/compute-statistics/{job_id}'
   _globals['_CORESERVICE'].methods_by_name['GetComputeRecommendationClassifiersJobOutput']._options = None
   _globals['_CORESERVICE'].methods_by_name['GetComputeRecommendationClassifiersJobOutput']._serialized_options = b'\202\323\344\223\002E\022C/api/v1/jobs/{job_id}/output/recommendation-classifiers-computation'
   _globals['_CORESERVICE'].methods_by_name['GenerateTransformationUpload']._options = None
   _globals['_CORESERVICE'].methods_by_name['GenerateTransformationUpload']._serialized_options = b'\202\323\344\223\002\034\"\027/api/v1/transformations:\001*'
   _globals['_CORESERVICE'].methods_by_name['ListRecommendationClassifiers']._options = None
@@ -391,62 +395,62 @@
   _globals['_CORESERVICE'].methods_by_name['GetFeatureSetPreviewToReview']._serialized_options = b'\202\323\344\223\0021\022//api/v1/reviews/{review_id}/feature-set/preview'
   _globals['_CORESERVICE'].methods_by_name['GetFeatureSetPreviewInReview']._options = None
   _globals['_CORESERVICE'].methods_by_name['GetFeatureSetPreviewInReview']._serialized_options = b'\202\323\344\223\002<\022:/api/v1/reviews/my-reviews/{review_id}/feature-set/preview'
   _globals['_CORESERVICE'].methods_by_name['GetFeatureSetToReview']._options = None
   _globals['_CORESERVICE'].methods_by_name['GetFeatureSetToReview']._serialized_options = b'\202\323\344\223\002)\022\'/api/v1/reviews/{review_id}/feature-set'
   _globals['_CORESERVICE'].methods_by_name['GetFeatureSetInReview']._options = None
   _globals['_CORESERVICE'].methods_by_name['GetFeatureSetInReview']._serialized_options = b'\202\323\344\223\0024\0222/api/v1/reviews/my-reviews/{review_id}/feature-set'
-  _globals['_JOBTYPE']._serialized_start=50460
-  _globals['_JOBTYPE']._serialized_end=50776
-  _globals['_PERMISSIONTYPE']._serialized_start=50778
-  _globals['_PERMISSIONTYPE']._serialized_end=50866
-  _globals['_ACTIVEPERMISSION']._serialized_start=50869
-  _globals['_ACTIVEPERMISSION']._serialized_end=51078
-  _globals['_PROJECTACTION']._serialized_start=51080
-  _globals['_PROJECTACTION']._serialized_end=51137
-  _globals['_OFFLINESTORAGEFORMAT']._serialized_start=51139
-  _globals['_OFFLINESTORAGEFORMAT']._serialized_end=51233
-  _globals['_JOINTYPE']._serialized_start=51235
-  _globals['_JOINTYPE']._serialized_end=51348
-  _globals['_FEATUREFILTEROPERATOR']._serialized_start=51351
-  _globals['_FEATUREFILTEROPERATOR']._serialized_end=51603
-  _globals['_FEATUREFILTERLOGICOPERATOR']._serialized_start=51606
-  _globals['_FEATUREFILTERLOGICOPERATOR']._serialized_end=51754
-  _globals['_FEATUREQUERYJOINTYPE']._serialized_start=51756
-  _globals['_FEATUREQUERYJOINTYPE']._serialized_end=51837
-  _globals['_FEATUREDATATYPE']._serialized_start=51840
-  _globals['_FEATUREDATATYPE']._serialized_end=51990
-  _globals['_PROCESSINTERVALUNIT']._serialized_start=51992
-  _globals['_PROCESSINTERVALUNIT']._serialized_end=52105
-  _globals['_TRANSFORMATIONTYPE']._serialized_start=52107
-  _globals['_TRANSFORMATIONTYPE']._serialized_end=52211
-  _globals['_SORTDIRECTION']._serialized_start=52213
-  _globals['_SORTDIRECTION']._serialized_end=52257
-  _globals['_RESOURCETYPE']._serialized_start=52259
-  _globals['_RESOURCETYPE']._serialized_end=52303
-  _globals['_PERMISSIONSTATE']._serialized_start=52305
-  _globals['_PERMISSIONSTATE']._serialized_end=52389
-  _globals['_TASKTYPE']._serialized_start=52391
-  _globals['_TASKTYPE']._serialized_end=52430
-  _globals['_JOBSTATUS']._serialized_start=52433
-  _globals['_JOBSTATUS']._serialized_end=52607
-  _globals['_UPDATABLEPROJECTFIELD']._serialized_start=52610
-  _globals['_UPDATABLEPROJECTFIELD']._serialized_end=52748
-  _globals['_UPDATABLEFEATURESETFIELD']._serialized_start=52751
-  _globals['_UPDATABLEFEATURESETFIELD']._serialized_end=53504
-  _globals['_UPDATABLEFEATUREFIELD']._serialized_start=53507
-  _globals['_UPDATABLEFEATUREFIELD']._serialized_end=53744
-  _globals['_FEATURESETDRAFTTYPE']._serialized_start=53747
-  _globals['_FEATURESETDRAFTTYPE']._serialized_end=53943
-  _globals['_ARTIFACTTYPE']._serialized_start=53945
-  _globals['_ARTIFACTTYPE']._serialized_end=54038
-  _globals['_ARTIFACTUPLOADSTATUS']._serialized_start=54041
-  _globals['_ARTIFACTUPLOADSTATUS']._serialized_end=54214
-  _globals['_REVIEWSTATUS']._serialized_start=54217
-  _globals['_REVIEWSTATUS']._serialized_end=54374
+  _globals['_JOBTYPE']._serialized_start=50767
+  _globals['_JOBTYPE']._serialized_end=51083
+  _globals['_PERMISSIONTYPE']._serialized_start=51085
+  _globals['_PERMISSIONTYPE']._serialized_end=51173
+  _globals['_ACTIVEPERMISSION']._serialized_start=51176
+  _globals['_ACTIVEPERMISSION']._serialized_end=51385
+  _globals['_PROJECTACTION']._serialized_start=51387
+  _globals['_PROJECTACTION']._serialized_end=51444
+  _globals['_OFFLINESTORAGEFORMAT']._serialized_start=51446
+  _globals['_OFFLINESTORAGEFORMAT']._serialized_end=51540
+  _globals['_JOINTYPE']._serialized_start=51542
+  _globals['_JOINTYPE']._serialized_end=51655
+  _globals['_FEATUREFILTEROPERATOR']._serialized_start=51658
+  _globals['_FEATUREFILTEROPERATOR']._serialized_end=51910
+  _globals['_FEATUREFILTERLOGICOPERATOR']._serialized_start=51913
+  _globals['_FEATUREFILTERLOGICOPERATOR']._serialized_end=52061
+  _globals['_FEATUREQUERYJOINTYPE']._serialized_start=52063
+  _globals['_FEATUREQUERYJOINTYPE']._serialized_end=52144
+  _globals['_FEATUREDATATYPE']._serialized_start=52147
+  _globals['_FEATUREDATATYPE']._serialized_end=52297
+  _globals['_PROCESSINTERVALUNIT']._serialized_start=52299
+  _globals['_PROCESSINTERVALUNIT']._serialized_end=52412
+  _globals['_TRANSFORMATIONTYPE']._serialized_start=52414
+  _globals['_TRANSFORMATIONTYPE']._serialized_end=52518
+  _globals['_SORTDIRECTION']._serialized_start=52520
+  _globals['_SORTDIRECTION']._serialized_end=52564
+  _globals['_RESOURCETYPE']._serialized_start=52566
+  _globals['_RESOURCETYPE']._serialized_end=52610
+  _globals['_PERMISSIONSTATE']._serialized_start=52612
+  _globals['_PERMISSIONSTATE']._serialized_end=52696
+  _globals['_TASKTYPE']._serialized_start=52698
+  _globals['_TASKTYPE']._serialized_end=52737
+  _globals['_JOBSTATUS']._serialized_start=52740
+  _globals['_JOBSTATUS']._serialized_end=52914
+  _globals['_UPDATABLEPROJECTFIELD']._serialized_start=52917
+  _globals['_UPDATABLEPROJECTFIELD']._serialized_end=53055
+  _globals['_UPDATABLEFEATURESETFIELD']._serialized_start=53058
+  _globals['_UPDATABLEFEATURESETFIELD']._serialized_end=53811
+  _globals['_UPDATABLEFEATUREFIELD']._serialized_start=53814
+  _globals['_UPDATABLEFEATUREFIELD']._serialized_end=54051
+  _globals['_FEATURESETDRAFTTYPE']._serialized_start=54054
+  _globals['_FEATURESETDRAFTTYPE']._serialized_end=54250
+  _globals['_ARTIFACTTYPE']._serialized_start=54252
+  _globals['_ARTIFACTTYPE']._serialized_end=54345
+  _globals['_ARTIFACTUPLOADSTATUS']._serialized_start=54348
+  _globals['_ARTIFACTUPLOADSTATUS']._serialized_end=54521
+  _globals['_REVIEWSTATUS']._serialized_start=54524
+  _globals['_REVIEWSTATUS']._serialized_end=54681
   _globals['_VALIDATEPERSONALTOKENRESPONSE']._serialized_start=531
   _globals['_VALIDATEPERSONALTOKENRESPONSE']._serialized_end=687
   _globals['_GETUSERPERMISSIONSREQUEST']._serialized_start=690
   _globals['_GETUSERPERMISSIONSREQUEST']._serialized_end=848
   _globals['_GETUSERACTIVEPERMISSIONSREQUEST']._serialized_start=851
   _globals['_GETUSERACTIVEPERMISSIONSREQUEST']._serialized_end=1031
   _globals['_GETUSERPERMISSIONSRESPONSE']._serialized_start=1033
@@ -462,661 +466,667 @@
   _globals['_LISTPERSONALACCESSTOKENSREQUEST']._serialized_start=1676
   _globals['_LISTPERSONALACCESSTOKENSREQUEST']._serialized_end=1748
   _globals['_LISTPERSONALACCESSTOKENSRESPONSE']._serialized_start=1751
   _globals['_LISTPERSONALACCESSTOKENSRESPONSE']._serialized_end=1891
   _globals['_IDENTITYPROVIDERDETAILS']._serialized_start=1893
   _globals['_IDENTITYPROVIDERDETAILS']._serialized_end=1975
   _globals['_GETWEBCONFIGRESPONSE']._serialized_start=1978
-  _globals['_GETWEBCONFIGRESPONSE']._serialized_end=2136
-  _globals['_GETFEATURESETSLASTMINORFORCURRENTMAJORREQUEST']._serialized_start=2138
-  _globals['_GETFEATURESETSLASTMINORFORCURRENTMAJORREQUEST']._serialized_end=2238
-  _globals['_GETLASTMINORFEATURESETFORMAJORINPROJECTREQUEST']._serialized_start=2241
-  _globals['_GETLASTMINORFEATURESETFORMAJORINPROJECTREQUEST']._serialized_end=2370
-  _globals['_FEATURESETEXISTSREQUEST']._serialized_start=2372
-  _globals['_FEATURESETEXISTSREQUEST']._serialized_end=2481
-  _globals['_GETINGESTHISTORYREQUEST']._serialized_start=2483
-  _globals['_GETINGESTHISTORYREQUEST']._serialized_end=2561
-  _globals['_PROJECTEXISTSREQUEST']._serialized_start=2563
-  _globals['_PROJECTEXISTSREQUEST']._serialized_end=2630
-  _globals['_FEATUREVIEWEXISTSREQUEST']._serialized_start=2632
-  _globals['_FEATUREVIEWEXISTSREQUEST']._serialized_end=2708
-  _globals['_MLDATASETEXISTSREQUEST']._serialized_start=2710
-  _globals['_MLDATASETEXISTSREQUEST']._serialized_end=2782
-  _globals['_EXISTSRESPONSE']._serialized_start=2784
-  _globals['_EXISTSRESPONSE']._serialized_end=2816
-  _globals['_PROJECTSDEFAULTRESPONSE']._serialized_start=2818
-  _globals['_PROJECTSDEFAULTRESPONSE']._serialized_end=2859
-  _globals['_HASPERMISSIONTORETRIEVEREQUEST']._serialized_start=2861
-  _globals['_HASPERMISSIONTORETRIEVEREQUEST']._serialized_end=2941
-  _globals['_HASPERMISSIONTORETRIEVERESPONSE']._serialized_start=2943
-  _globals['_HASPERMISSIONTORETRIEVERESPONSE']._serialized_end=3009
-  _globals['_STARTREVERTINGESTJOBREQUEST']._serialized_start=3011
-  _globals['_STARTREVERTINGESTJOBREQUEST']._serialized_end=3112
-  _globals['_ONLINERETRIEVEMETA']._serialized_start=3114
-  _globals['_ONLINERETRIEVEMETA']._serialized_end=3215
-  _globals['_REFRESHTOKENREQUEST']._serialized_start=3217
-  _globals['_REFRESHTOKENREQUEST']._serialized_end=3261
-  _globals['_TOKENREQUEST']._serialized_start=3263
-  _globals['_TOKENREQUEST']._serialized_end=3295
-  _globals['_GENERATETOKENREQUEST']._serialized_start=3297
-  _globals['_GENERATETOKENREQUEST']._serialized_end=3403
-  _globals['_TOKENRESPONSE']._serialized_start=3405
-  _globals['_TOKENRESPONSE']._serialized_end=3484
-  _globals['_RAWTOKENRESPONSE']._serialized_start=3486
-  _globals['_RAWTOKENRESPONSE']._serialized_end=3574
-  _globals['_TOKENSCONFIGRESPONSE']._serialized_start=3576
-  _globals['_TOKENSCONFIGRESPONSE']._serialized_end=3665
-  _globals['_LISTJOBSREQUEST']._serialized_start=3667
-  _globals['_LISTJOBSREQUEST']._serialized_end=3779
-  _globals['_LISTJOBSRESPONSE']._serialized_start=3781
-  _globals['_LISTJOBSRESPONSE']._serialized_end=3846
-  _globals['_FEATURESETSCHEMACOMPATIBILITYREQUEST']._serialized_start=3849
-  _globals['_FEATURESETSCHEMACOMPATIBILITYREQUEST']._serialized_end=4046
-  _globals['_FEATURESETSCHEMACOMPATIBILITYRESPONSE']._serialized_start=4048
-  _globals['_FEATURESETSCHEMACOMPATIBILITYRESPONSE']._serialized_end=4110
-  _globals['_FEATURESETSCHEMAPATCHREQUEST']._serialized_start=4113
-  _globals['_FEATURESETSCHEMAPATCHREQUEST']._serialized_end=4302
-  _globals['_FEATURESETSCHEMAPATCHRESPONSE']._serialized_start=4304
-  _globals['_FEATURESETSCHEMAPATCHRESPONSE']._serialized_end=4394
-  _globals['_JOBID']._serialized_start=4396
-  _globals['_JOBID']._serialized_end=4419
-  _globals['_GETRECOMMENDATIONREQUEST']._serialized_start=4421
-  _globals['_GETRECOMMENDATIONREQUEST']._serialized_end=4471
-  _globals['_GETRECOMMENDATIONRESPONSE']._serialized_start=4474
-  _globals['_GETRECOMMENDATIONRESPONSE']._serialized_end=4777
-  _globals['_GETRECOMMENDATIONRESPONSE_JOIN']._serialized_start=4581
-  _globals['_GETRECOMMENDATIONRESPONSE_JOIN']._serialized_end=4624
-  _globals['_GETRECOMMENDATIONRESPONSE_MATCH']._serialized_start=4627
-  _globals['_GETRECOMMENDATIONRESPONSE_MATCH']._serialized_end=4777
-  _globals['_JOB']._serialized_start=4780
-  _globals['_JOB']._serialized_end=5103
-  _globals['_JOBPROGRESSINPUT']._serialized_start=5105
-  _globals['_JOBPROGRESSINPUT']._serialized_end=5159
-  _globals['_JOBPROGRESSOUTPUT']._serialized_start=5162
-  _globals['_JOBPROGRESSOUTPUT']._serialized_end=5360
-  _globals['_JOBPROGRESSOUTPUT_PROGRESS']._serialized_start=5257
-  _globals['_JOBPROGRESSOUTPUT_PROGRESS']._serialized_end=5360
-  _globals['_FEATURESETPERMISSIONREQUEST']._serialized_start=5363
-  _globals['_FEATURESETPERMISSIONREQUEST']._serialized_end=5501
-  _globals['_PROJECTPERMISSIONREQUEST']._serialized_start=5504
-  _globals['_PROJECTPERMISSIONREQUEST']._serialized_end=5635
-  _globals['_STARTEXTRACTSCHEMAJOBREQUEST']._serialized_start=5638
-  _globals['_STARTEXTRACTSCHEMAJOBREQUEST']._serialized_end=5870
-  _globals['_EXTRACTSCHEMARESPONSE']._serialized_start=5873
-  _globals['_EXTRACTSCHEMARESPONSE']._serialized_end=6025
-  _globals['_LISTFEATURESETSVERSIONREQUEST']._serialized_start=6027
-  _globals['_LISTFEATURESETSVERSIONREQUEST']._serialized_end=6082
-  _globals['_FEATURESETRESPONSE']._serialized_start=6085
-  _globals['_FEATURESETRESPONSE']._serialized_end=6214
-  _globals['_UPDATEFEATURESETRESPONSE']._serialized_start=6216
-  _globals['_UPDATEFEATURESETRESPONSE']._serialized_end=6311
-  _globals['_UPDATEPROJECTRESPONSE']._serialized_start=6313
-  _globals['_UPDATEPROJECTRESPONSE']._serialized_end=6398
-  _globals['_UPDATEFEATURERESPONSE']._serialized_start=6401
-  _globals['_UPDATEFEATURERESPONSE']._serialized_end=6555
-  _globals['_PROJECTRESPONSE']._serialized_start=6557
-  _globals['_PROJECTRESPONSE']._serialized_end=6628
-  _globals['_LOGINRESPONSE']._serialized_start=6630
-  _globals['_LOGINRESPONSE']._serialized_end=6703
-  _globals['_GETACTIVEUSERRESPONSE']._serialized_start=6705
-  _globals['_GETACTIVEUSERRESPONSE']._serialized_end=6805
-  _globals['_GETPROJECTREQUEST']._serialized_start=6807
-  _globals['_GETPROJECTREQUEST']._serialized_end=6848
-  _globals['_GETPROJECTBYIDREQUEST']._serialized_start=6850
-  _globals['_GETPROJECTBYIDREQUEST']._serialized_end=6893
-  _globals['_DELETEFEATURESETREQUEST']._serialized_start=6895
-  _globals['_DELETEFEATURESETREQUEST']._serialized_end=6944
-  _globals['_DELETEFEATURESETVERSIONREQUEST']._serialized_start=6946
-  _globals['_DELETEFEATURESETVERSIONREQUEST']._serialized_end=7037
-  _globals['_LOGOUTREQUEST']._serialized_start=7039
-  _globals['_LOGOUTREQUEST']._serialized_end=7077
-  _globals['_USERBASICINFO']._serialized_start=7079
-  _globals['_USERBASICINFO']._serialized_end=7159
-  _globals['_USER']._serialized_start=7161
-  _globals['_USER']._serialized_end=7250
-  _globals['_ACCESSTOKENRESPONSE']._serialized_start=7252
-  _globals['_ACCESSTOKENRESPONSE']._serialized_end=7373
-  _globals['_DELETEPROJECTREQUEST']._serialized_start=7375
-  _globals['_DELETEPROJECTREQUEST']._serialized_end=7417
-  _globals['_CREATEPROJECTREQUEST']._serialized_start=7420
-  _globals['_CREATEPROJECTREQUEST']._serialized_end=7563
-  _globals['_CREATEPROJECTRESPONSE']._serialized_start=7565
-  _globals['_CREATEPROJECTRESPONSE']._serialized_end=7666
-  _globals['_LISTPROJECTSRESPONSE']._serialized_start=7668
-  _globals['_LISTPROJECTSRESPONSE']._serialized_end=7745
-  _globals['_LISTPROJECTHISTORYPAGEREQUEST']._serialized_start=7747
-  _globals['_LISTPROJECTHISTORYPAGEREQUEST']._serialized_end=7837
-  _globals['_PROJECTHISTORY']._serialized_start=7840
-  _globals['_PROJECTHISTORY']._serialized_end=8034
-  _globals['_LISTPROJECTHISTORYPAGERESPONSE']._serialized_start=8036
-  _globals['_LISTPROJECTHISTORYPAGERESPONSE']._serialized_end=8154
-  _globals['_GETINGESTHISTORYRESPONSE']._serialized_start=8156
-  _globals['_GETINGESTHISTORYRESPONSE']._serialized_end=8252
-  _globals['_LISTFEATURESETSPAGEREQUEST']._serialized_start=8254
-  _globals['_LISTFEATURESETSPAGEREQUEST']._serialized_end=8344
-  _globals['_LISTFEATURESETSPAGERESPONSE']._serialized_start=8346
-  _globals['_LISTFEATURESETSPAGERESPONSE']._serialized_end=8462
-  _globals['_AWSCREDENTIALS']._serialized_start=8465
-  _globals['_AWSCREDENTIALS']._serialized_end=8600
-  _globals['_AZURECREDENTIALS']._serialized_start=8603
-  _globals['_AZURECREDENTIALS']._serialized_end=8769
-  _globals['_SNOWFLAKECREDENTIALS']._serialized_start=8771
-  _globals['_SNOWFLAKECREDENTIALS']._serialized_end=8870
-  _globals['_JDBCCREDENTIALS']._serialized_start=8872
-  _globals['_JDBCCREDENTIALS']._serialized_end=8921
-  _globals['_MONGODBCREDENTIALS']._serialized_start=8923
-  _globals['_MONGODBCREDENTIALS']._serialized_end=8975
-  _globals['_CREDENTIALS']._serialized_start=8978
-  _globals['_CREDENTIALS']._serialized_end=9318
-  _globals['_LISTFEATURESETSRESPONSE']._serialized_start=9320
-  _globals['_LISTFEATURESETSRESPONSE']._serialized_end=9407
-  _globals['_LISTFEATURESETVERSIONSRESPONSE']._serialized_start=9409
-  _globals['_LISTFEATURESETVERSIONSRESPONSE']._serialized_end=9517
-  _globals['_FEATURESETVERSIONDESCRIPTION']._serialized_start=9519
-  _globals['_FEATURESETVERSIONDESCRIPTION']._serialized_end=9645
-  _globals['_GETFEATURESETREQUEST']._serialized_start=9647
-  _globals['_GETFEATURESETREQUEST']._serialized_end=9732
-  _globals['_STARTINGESTJOBREQUEST']._serialized_start=9735
-  _globals['_STARTINGESTJOBREQUEST']._serialized_end=9944
-  _globals['_INGESTRESPONSE']._serialized_start=9947
-  _globals['_INGESTRESPONSE']._serialized_end=10302
-  _globals['_INGESTRESPONSE_INGESTMETA']._serialized_start=10088
-  _globals['_INGESTRESPONSE_INGESTMETA']._serialized_end=10302
-  _globals['_RETRIEVEREQUEST']._serialized_start=10305
-  _globals['_RETRIEVEREQUEST']._serialized_end=10462
-  _globals['_RETRIEVEASLINKSRESPONSE']._serialized_start=10465
-  _globals['_RETRIEVEASLINKSRESPONSE']._serialized_end=10604
-  _globals['_RETRIEVEASSPARKRESPONSE']._serialized_start=10607
-  _globals['_RETRIEVEASSPARKRESPONSE']._serialized_end=10967
-  _globals['_RETRIEVEASSPARKRESPONSE_OPTIONSENTRY']._serialized_start=10921
-  _globals['_RETRIEVEASSPARKRESPONSE_OPTIONSENTRY']._serialized_end=10967
-  _globals['_STARTMATERIALIZATIONONLINEREQUEST']._serialized_start=10969
-  _globals['_STARTMATERIALIZATIONONLINEREQUEST']._serialized_end=11057
-  _globals['_MATERIALIZATIONONLINERESPONSE']._serialized_start=11059
-  _globals['_MATERIALIZATIONONLINERESPONSE']._serialized_end=11177
-  _globals['_INGESTWRITECREDENTIALREQUEST']._serialized_start=11179
-  _globals['_INGESTWRITECREDENTIALREQUEST']._serialized_end=11229
-  _globals['_INGESTWRITECREDENTIALRESPONSE']._serialized_start=11232
-  _globals['_INGESTWRITECREDENTIALRESPONSE']._serialized_end=11434
-  _globals['_INGESTWRITECREDENTIALRESPONSE_OPTIONSENTRY']._serialized_start=10921
-  _globals['_INGESTWRITECREDENTIALRESPONSE_OPTIONSENTRY']._serialized_end=10967
-  _globals['_STARTOPTIMIZESTORAGEJOBREQUEST']._serialized_start=11437
-  _globals['_STARTOPTIMIZESTORAGEJOBREQUEST']._serialized_end=11593
-  _globals['_STORAGEOPTIMIZATION']._serialized_start=11596
-  _globals['_STORAGEOPTIMIZATION']._serialized_end=11781
-  _globals['_OPTIMIZESTORAGEZORDERBYSPEC']._serialized_start=11783
-  _globals['_OPTIMIZESTORAGEZORDERBYSPEC']._serialized_end=11829
-  _globals['_OPTIMIZESTORAGECOMPACTSPEC']._serialized_start=11831
-  _globals['_OPTIMIZESTORAGECOMPACTSPEC']._serialized_end=11859
-  _globals['_OPTIMIZESTORAGERESPONSE']._serialized_start=11861
-  _globals['_OPTIMIZESTORAGERESPONSE']._serialized_end=11916
-  _globals['_RAWDATALOCATION']._serialized_start=11919
-  _globals['_RAWDATALOCATION']._serialized_end=12739
-  _globals['_ONLINESOURCESPEC']._serialized_start=12741
-  _globals['_ONLINESOURCESPEC']._serialized_end=12794
-  _globals['_CSVFILESPEC']._serialized_start=12796
-  _globals['_CSVFILESPEC']._serialized_end=12842
-  _globals['_JSONFILESPEC']._serialized_start=12844
-  _globals['_JSONFILESPEC']._serialized_end=12891
-  _globals['_PARQUETFILESPEC']._serialized_start=12893
-  _globals['_PARQUETFILESPEC']._serialized_end=12924
-  _globals['_TEMPPARQUETFILESPEC']._serialized_start=12926
-  _globals['_TEMPPARQUETFILESPEC']._serialized_end=12961
-  _globals['_PROXY']._serialized_start=12963
-  _globals['_PROXY']._serialized_end=13030
-  _globals['_SNOWFLAKETABLESPEC']._serialized_start=13033
-  _globals['_SNOWFLAKETABLESPEC']._serialized_end=13248
-  _globals['_JDBCTABLESPEC']._serialized_start=13251
-  _globals['_JDBCTABLESPEC']._serialized_end=13432
-  _globals['_DELTATABLESPEC']._serialized_start=13434
-  _globals['_DELTATABLESPEC']._serialized_end=13552
-  _globals['_CSVFOLDERSPEC']._serialized_start=13554
-  _globals['_CSVFOLDERSPEC']._serialized_end=13633
-  _globals['_PARQUETFOLDERSPEC']._serialized_start=13635
-  _globals['_PARQUETFOLDERSPEC']._serialized_end=13699
-  _globals['_JSONFOLDERSPEC']._serialized_start=13701
-  _globals['_JSONFOLDERSPEC']._serialized_end=13781
-  _globals['_MONGODBCOLLECTIONSPEC']._serialized_start=13783
-  _globals['_MONGODBCOLLECTIONSPEC']._serialized_end=13868
-  _globals['_MOJOTRANSFORMATION']._serialized_start=13870
-  _globals['_MOJOTRANSFORMATION']._serialized_end=13908
-  _globals['_SPARKPIPELINETRANSFORMATION']._serialized_start=13910
-  _globals['_SPARKPIPELINETRANSFORMATION']._serialized_end=13957
-  _globals['_JOINTRANSFORMATION']._serialized_start=13959
-  _globals['_JOINTRANSFORMATION']._serialized_end=14073
-  _globals['_VERSIONEDID']._serialized_start=14075
-  _globals['_VERSIONEDID']._serialized_end=14123
-  _globals['_TRANSFORMATION']._serialized_start=14126
-  _globals['_TRANSFORMATION']._serialized_end=14362
-  _globals['_DERIVEDINFORMATION']._serialized_start=14365
-  _globals['_DERIVEDINFORMATION']._serialized_end=14519
-  _globals['_SELECTEDFEATURE']._serialized_start=14521
-  _globals['_SELECTEDFEATURE']._serialized_end=14595
-  _globals['_FILTERCONDITIONUNION']._serialized_start=14598
-  _globals['_FILTERCONDITIONUNION']._serialized_end=14759
-  _globals['_FEATUREFILTER']._serialized_start=14762
-  _globals['_FEATUREFILTER']._serialized_end=14923
-  _globals['_FEATUREFILTERLOGIC']._serialized_start=14926
-  _globals['_FEATUREFILTERLOGIC']._serialized_end=15155
-  _globals['_FEATUREQUERY']._serialized_start=15158
-  _globals['_FEATUREQUERY']._serialized_end=15870
-  _globals['_FEATUREQUERY_FROM']._serialized_start=15445
-  _globals['_FEATUREQUERY_FROM']._serialized_end=15528
-  _globals['_FEATUREQUERY_JOIN']._serialized_start=15531
-  _globals['_FEATUREQUERY_JOIN']._serialized_end=15870
-  _globals['_FEATUREQUERY_JOIN_ON']._serialized_start=15747
-  _globals['_FEATUREQUERY_JOIN_ON']._serialized_end=15870
-  _globals['_FEATUREVIEW']._serialized_start=15873
-  _globals['_FEATUREVIEW']._serialized_end=16027
-  _globals['_CREATEFEATUREVIEWREQUEST']._serialized_start=16030
-  _globals['_CREATEFEATUREVIEWREQUEST']._serialized_end=16168
-  _globals['_UPDATEFEATUREVIEWREQUEST']._serialized_start=16170
-  _globals['_UPDATEFEATUREVIEWREQUEST']._serialized_end=16272
-  _globals['_CREATEFEATUREVIEWNEWVERSIONREQUEST']._serialized_start=16275
-  _globals['_CREATEFEATUREVIEWNEWVERSIONREQUEST']._serialized_end=16423
-  _globals['_GETFEATUREVIEWREQUEST']._serialized_start=16425
-  _globals['_GETFEATUREVIEWREQUEST']._serialized_end=16499
-  _globals['_FEATUREVIEWRESPONSE']._serialized_start=16501
-  _globals['_FEATUREVIEWRESPONSE']._serialized_end=16585
-  _globals['_LISTFEATUREVIEWSREQUEST']._serialized_start=16587
-  _globals['_LISTFEATUREVIEWSREQUEST']._serialized_end=16632
-  _globals['_LISTFEATUREVIEWSRESPONSE']._serialized_start=16634
-  _globals['_LISTFEATUREVIEWSRESPONSE']._serialized_end=16724
-  _globals['_RETRIEVEFEATUREVIEWASSPARKREQUEST']._serialized_start=16727
-  _globals['_RETRIEVEFEATUREVIEWASSPARKREQUEST']._serialized_end=16927
-  _globals['_RETRIEVEFEATUREVIEWASSPARKRESPONSE']._serialized_start=16930
-  _globals['_RETRIEVEFEATUREVIEWASSPARKRESPONSE']._serialized_end=17224
-  _globals['_RETRIEVEFEATUREVIEWASSPARKRESPONSE_OPTIONSENTRY']._serialized_start=10921
-  _globals['_RETRIEVEFEATUREVIEWASSPARKRESPONSE_OPTIONSENTRY']._serialized_end=10967
-  _globals['_RETRIEVEFEATUREVIEWASASLINKSREQUEST']._serialized_start=17227
-  _globals['_RETRIEVEFEATUREVIEWASASLINKSREQUEST']._serialized_end=17409
-  _globals['_RETRIEVEFEATUREVIEWASASLINKSRESPONSE']._serialized_start=17411
-  _globals['_RETRIEVEFEATUREVIEWASASLINKSRESPONSE']._serialized_end=17473
-  _globals['_DELETEFEATUREVIEWREQUEST']._serialized_start=17475
-  _globals['_DELETEFEATUREVIEWREQUEST']._serialized_end=17526
-  _globals['_MLDATASETFEATURE']._serialized_start=17529
-  _globals['_MLDATASETFEATURE']._serialized_end=17928
-  _globals['_MLDATASET']._serialized_start=17931
-  _globals['_MLDATASET']._serialized_end=18433
-  _globals['_MLDATASET_MLDATASETSTATE']._serialized_start=18325
-  _globals['_MLDATASET_MLDATASETSTATE']._serialized_end=18433
-  _globals['_CREATEMLDATASETREQUEST']._serialized_start=18436
-  _globals['_CREATEMLDATASETREQUEST']._serialized_end=18654
-  _globals['_UPDATEMLDATASETREQUEST']._serialized_start=18656
-  _globals['_UPDATEMLDATASETREQUEST']._serialized_end=18724
-  _globals['_DELETEMLDATASETREQUEST']._serialized_start=18726
-  _globals['_DELETEMLDATASETREQUEST']._serialized_end=18773
-  _globals['_CREATEMLDATASETRESPONSE']._serialized_start=18776
-  _globals['_CREATEMLDATASETRESPONSE']._serialized_end=18908
-  _globals['_GETMLDATASETREQUEST']._serialized_start=18910
-  _globals['_GETMLDATASETREQUEST']._serialized_end=19011
-  _globals['_LISTMLDATASETSREQUEST']._serialized_start=19013
-  _globals['_LISTMLDATASETSREQUEST']._serialized_end=19091
-  _globals['_LISTMLDATASETSRESPONSE']._serialized_start=19093
-  _globals['_LISTMLDATASETSRESPONSE']._serialized_end=19177
-  _globals['_RETRIEVEMLDATASETASSPARKREQUEST']._serialized_start=19179
-  _globals['_RETRIEVEMLDATASETASSPARKREQUEST']._serialized_end=19255
-  _globals['_RETRIEVEMLDATASETASSPARKRESPONSE']._serialized_start=19258
-  _globals['_RETRIEVEMLDATASETASSPARKRESPONSE']._serialized_end=19548
-  _globals['_RETRIEVEMLDATASETASSPARKRESPONSE_OPTIONSENTRY']._serialized_start=10921
-  _globals['_RETRIEVEMLDATASETASSPARKRESPONSE_OPTIONSENTRY']._serialized_end=10967
-  _globals['_RETRIEVEMLDATASETASASLINKSREQUEST']._serialized_start=19550
-  _globals['_RETRIEVEMLDATASETASASLINKSREQUEST']._serialized_end=19608
-  _globals['_RETRIEVEMLDATASETASASLINKSRESPONSE']._serialized_start=19610
-  _globals['_RETRIEVEMLDATASETASASLINKSRESPONSE']._serialized_end=19670
-  _globals['_FEATURESET']._serialized_start=19673
-  _globals['_FEATURESET']._serialized_end=21654
-  _globals['_FEATURESET_STATISTICS']._serialized_start=21254
-  _globals['_FEATURESET_STATISTICS']._serialized_end=21311
-  _globals['_FEATURESET_SPECIALDATA']._serialized_start=21314
-  _globals['_FEATURESET_SPECIALDATA']._serialized_end=21572
-  _globals['_FEATURESET_SPECIALDATA_LEGAL']._serialized_start=21481
-  _globals['_FEATURESET_SPECIALDATA_LEGAL']._serialized_end=21572
-  _globals['_FEATURESET_ONLINE']._serialized_start=21574
-  _globals['_FEATURESET_ONLINE']._serialized_end=21648
-  _globals['_GETFEATURESETPREVIEWREQUEST']._serialized_start=21656
-  _globals['_GETFEATURESETPREVIEWREQUEST']._serialized_end=21738
-  _globals['_GETFEATURESETPREVIEWRESPONSE']._serialized_start=21740
-  _globals['_GETFEATURESETPREVIEWRESPONSE']._serialized_end=21813
-  _globals['_SCOPE']._serialized_start=21815
-  _globals['_SCOPE']._serialized_end=21926
-  _globals['_REGISTERFEATURESETREQUEST']._serialized_start=21929
-  _globals['_REGISTERFEATURESETREQUEST']._serialized_end=22904
-  _globals['_CREATENEWFEATURESETVERSIONREQUEST']._serialized_start=22907
-  _globals['_CREATENEWFEATURESETVERSIONREQUEST']._serialized_end=23599
-  _globals['_FEATUREPROFILE']._serialized_start=23602
-  _globals['_FEATUREPROFILE']._serialized_end=23857
-  _globals['_FEATURESCHEMA']._serialized_start=23860
-  _globals['_FEATURESCHEMA']._serialized_end=24404
-  _globals['_FEATURESCHEMA_SPECIALDATA']._serialized_start=21314
-  _globals['_FEATURESCHEMA_SPECIALDATA']._serialized_end=21406
-  _globals['_FEATURESCHEMA_MONITORING']._serialized_start=24365
-  _globals['_FEATURESCHEMA_MONITORING']._serialized_end=24404
-  _globals['_FEATURE']._serialized_start=24407
-  _globals['_FEATURE']._serialized_end=25064
-  _globals['_FEATURE_MONITORING']._serialized_start=24365
-  _globals['_FEATURE_MONITORING']._serialized_end=24404
-  _globals['_FEATURE_SPECIALDATA']._serialized_start=21314
-  _globals['_FEATURE_SPECIALDATA']._serialized_end=21406
-  _globals['_FEATURESTATISTICS']._serialized_start=25067
-  _globals['_FEATURESTATISTICS']._serialized_end=25239
-  _globals['_CATEGORICALFEATURESTATISTICS']._serialized_start=25242
-  _globals['_CATEGORICALFEATURESTATISTICS']._serialized_end=25413
-  _globals['_CATEGORICALFEATURESTATISTICS_FEATURETOP']._serialized_start=25372
-  _globals['_CATEGORICALFEATURESTATISTICS_FEATURETOP']._serialized_end=25413
-  _globals['_GETVERSIONRESPONSE']._serialized_start=25415
-  _globals['_GETVERSIONRESPONSE']._serialized_end=25452
-  _globals['_GETAPICONFIGRESPONSE']._serialized_start=25454
-  _globals['_GETAPICONFIGRESPONSE']._serialized_end=25546
-  _globals['_PROJECT']._serialized_start=25549
-  _globals['_PROJECT']._serialized_end=25958
-  _globals['_LISTABLEPROJECT']._serialized_start=25961
-  _globals['_LISTABLEPROJECT']._serialized_end=26253
-  _globals['_FEATURESETINGEST']._serialized_start=26256
-  _globals['_FEATURESETINGEST']._serialized_end=26630
-  _globals['_PERSONALACCESSTOKEN']._serialized_start=26633
-  _globals['_PERSONALACCESSTOKEN']._serialized_end=26848
-  _globals['_GENERATETRANSFORMATIONUPLOADREQUEST']._serialized_start=26851
-  _globals['_GENERATETRANSFORMATIONUPLOADREQUEST']._serialized_end=26987
-  _globals['_GENERATETRANSFORMATIONUPLOADRESPONSE']._serialized_start=26990
-  _globals['_GENERATETRANSFORMATIONUPLOADRESPONSE']._serialized_end=27203
-  _globals['_GENERATETRANSFORMATIONUPLOADRESPONSE_HEADERSENTRY']._serialized_start=27157
-  _globals['_GENERATETRANSFORMATIONUPLOADRESPONSE_HEADERSENTRY']._serialized_end=27203
-  _globals['_LISTPROJECTSPAGEREQUEST']._serialized_start=27205
-  _globals['_LISTPROJECTSPAGEREQUEST']._serialized_end=27269
-  _globals['_LISTPROJECTSPAGERESPONSE']._serialized_start=27271
-  _globals['_LISTPROJECTSPAGERESPONSE']._serialized_end=27377
-  _globals['_PROJECTSEARCHREQUEST']._serialized_start=27380
-  _globals['_PROJECTSEARCHREQUEST']._serialized_end=27924
-  _globals['_PROJECTSEARCHREQUEST_PROJECTSORTFIELD']._serialized_start=27709
-  _globals['_PROJECTSEARCHREQUEST_PROJECTSORTFIELD']._serialized_end=27924
-  _globals['_FEATURESETSEARCHREQUEST']._serialized_start=27927
-  _globals['_FEATURESETSEARCHREQUEST']._serialized_end=28525
-  _globals['_FEATURESETSEARCHREQUEST_FEATURESETSORTFIELD']._serialized_start=28277
-  _globals['_FEATURESETSEARCHREQUEST_FEATURESETSORTFIELD']._serialized_end=28525
-  _globals['_FEATURESEARCHREQUEST']._serialized_start=28528
-  _globals['_FEATURESEARCHREQUEST']._serialized_end=28918
-  _globals['_FEATURESEARCHREQUEST_FEATURESORTFIELD']._serialized_start=28801
-  _globals['_FEATURESEARCHREQUEST_FEATURESORTFIELD']._serialized_end=28918
-  _globals['_PROJECTSEARCHRESULTS']._serialized_start=28920
-  _globals['_PROJECTSEARCHRESULTS']._serialized_end=29038
-  _globals['_LISTABLEFEATURESET']._serialized_start=29041
-  _globals['_LISTABLEFEATURESET']._serialized_end=30699
-  _globals['_FEATURESETSEARCHRESULTS']._serialized_start=30702
-  _globals['_FEATURESETSEARCHRESULTS']._serialized_end=30830
-  _globals['_LISTABLEFEATURE']._serialized_start=30833
-  _globals['_LISTABLEFEATURE']._serialized_end=31055
-  _globals['_FEATURESEARCHRESULTS']._serialized_start=31057
-  _globals['_FEATURESEARCHRESULTS']._serialized_end=31175
-  _globals['_FEATURESETREQUESTID']._serialized_start=31177
-  _globals['_FEATURESETREQUESTID']._serialized_end=31251
-  _globals['_GETFEATUREREQUEST']._serialized_start=31253
-  _globals['_GETFEATUREREQUEST']._serialized_end=31345
-  _globals['_LISTFEATURESPAGERESPONSE']._serialized_start=31347
-  _globals['_LISTFEATURESPAGERESPONSE']._serialized_end=31453
-  _globals['_FEATURERESPONSE']._serialized_start=31455
-  _globals['_FEATURERESPONSE']._serialized_end=31526
-  _globals['_LISTFEATURESREQUEST']._serialized_start=31529
-  _globals['_LISTFEATURESREQUEST']._serialized_end=31657
-  _globals['_LISTFEATURESRESPONSE']._serialized_start=31659
-  _globals['_LISTFEATURESRESPONSE']._serialized_end=31761
-  _globals['_LISTABLEFEATURESETREQUEST']._serialized_start=31763
-  _globals['_LISTABLEFEATURESETREQUEST']._serialized_end=31843
-  _globals['_LISTABLEFEATURESETRESPONSE']._serialized_start=31845
-  _globals['_LISTABLEFEATURESETRESPONSE']._serialized_end=31951
-  _globals['_FEATURESETSDERIVEDFROMREQUEST']._serialized_start=31953
-  _globals['_FEATURESETSDERIVEDFROMREQUEST']._serialized_end=32043
-  _globals['_FEATURESETSDERIVEDFROMRESPONSE']._serialized_start=32045
-  _globals['_FEATURESETSDERIVEDFROMRESPONSE']._serialized_end=32156
-  _globals['_SUBMITPENDINGPERMISSIONREQUEST']._serialized_start=32159
-  _globals['_SUBMITPENDINGPERMISSIONREQUEST']._serialized_end=32292
-  _globals['_SUBMITPENDINGPERMISSIONRESPONSE']._serialized_start=32294
-  _globals['_SUBMITPENDINGPERMISSIONRESPONSE']._serialized_end=32350
-  _globals['_LISTPERMISSIONSPAGEREQUEST']._serialized_start=32353
-  _globals['_LISTPERMISSIONSPAGEREQUEST']._serialized_end=32503
-  _globals['_LISTPROJECTSPERMISSIONSPAGERESPONSE']._serialized_start=32506
-  _globals['_LISTPROJECTSPERMISSIONSPAGERESPONSE']._serialized_end=32642
-  _globals['_LISTFEATURESETSPERMISSIONSPAGERESPONSE']._serialized_start=32645
-  _globals['_LISTFEATURESETSPERMISSIONSPAGERESPONSE']._serialized_end=32787
-  _globals['_LISTABLEPROJECTTOPERMISSION']._serialized_start=32790
-  _globals['_LISTABLEPROJECTTOPERMISSION']._serialized_end=32941
-  _globals['_LISTABLEFEATURESETTOPERMISSION']._serialized_start=32944
-  _globals['_LISTABLEFEATURESETTOPERMISSION']._serialized_end=33105
-  _globals['_PERMISSION']._serialized_start=33108
-  _globals['_PERMISSION']._serialized_end=34240
-  _globals['_PERMISSION_PROMOTEDUPDATE']._serialized_start=33780
-  _globals['_PERMISSION_PROMOTEDUPDATE']._serialized_end=33952
-  _globals['_PERMISSION_REVOKEDUPDATE']._serialized_start=33955
-  _globals['_PERMISSION_REVOKEDUPDATE']._serialized_end=34091
-  _globals['_PERMISSION_GRANTEDORREJECTEDUPDATE']._serialized_start=34094
-  _globals['_PERMISSION_GRANTEDORREJECTEDUPDATE']._serialized_end=34240
-  _globals['_REVOKEPERMISSIONREQUEST']._serialized_start=34242
-  _globals['_REVOKEPERMISSIONREQUEST']._serialized_end=34306
-  _globals['_APPROVEPENDINGPERMISSIONREQUEST']._serialized_start=34308
-  _globals['_APPROVEPENDINGPERMISSIONREQUEST']._serialized_end=34380
-  _globals['_REJECTPENDINGPERMISSIONREQUEST']._serialized_start=34382
-  _globals['_REJECTPENDINGPERMISSIONREQUEST']._serialized_end=34453
-  _globals['_WITHDRAWPENDINGPERMISSIONREQUEST']._serialized_start=34455
-  _globals['_WITHDRAWPENDINGPERMISSIONREQUEST']._serialized_end=34512
-  _globals['_GETACTIVEPERMISSIONREQUEST']._serialized_start=34514
-  _globals['_GETACTIVEPERMISSIONREQUEST']._serialized_end=34563
-  _globals['_GETACTIVEPERMISSIONRESPONSE']._serialized_start=34566
-  _globals['_GETACTIVEPERMISSIONRESPONSE']._serialized_end=34726
-  _globals['_SCHEDULEDTASK']._serialized_start=34729
-  _globals['_SCHEDULEDTASK']._serialized_end=35320
-  _globals['_SCHEDULETASKREQUEST']._serialized_start=35323
-  _globals['_SCHEDULETASKREQUEST']._serialized_end=35636
-  _globals['_LISTSCHEDULEDTASKSREQUEST']._serialized_start=35638
-  _globals['_LISTSCHEDULEDTASKSREQUEST']._serialized_end=35728
-  _globals['_LISTSCHEDULEDTASKSRESPONSE']._serialized_start=35730
-  _globals['_LISTSCHEDULEDTASKSRESPONSE']._serialized_end=35841
-  _globals['_SCHEDULEDTASKID']._serialized_start=35843
-  _globals['_SCHEDULEDTASKID']._serialized_end=35887
-  _globals['_SCHEDULEDTASKRESPONSE']._serialized_start=35889
-  _globals['_SCHEDULEDTASKRESPONSE']._serialized_end=35969
-  _globals['_SCHEDULEDTASKUPDATEREQUEST']._serialized_start=35971
-  _globals['_SCHEDULEDTASKUPDATEREQUEST']._serialized_end=36089
-  _globals['_PAUSESCHEDULEDTASKREQUEST']._serialized_start=36091
-  _globals['_PAUSESCHEDULEDTASKREQUEST']._serialized_end=36145
-  _globals['_RESUMESCHEDULEDTASKREQUEST']._serialized_start=36147
-  _globals['_RESUMESCHEDULEDTASKREQUEST']._serialized_end=36252
-  _globals['_LAZYINGESTREQUEST']._serialized_start=36254
-  _globals['_LAZYINGESTREQUEST']._serialized_end=36326
-  _globals['_LAZYINGESTRESPONSE']._serialized_start=36328
-  _globals['_LAZYINGESTRESPONSE']._serialized_end=36399
-  _globals['_GETLAZYINGESTTASKREQUEST']._serialized_start=36401
-  _globals['_GETLAZYINGESTTASKREQUEST']._serialized_end=36480
-  _globals['_LISTSCHEDULEDTASKEXECUTIONSREQUEST']._serialized_start=36482
-  _globals['_LISTSCHEDULEDTASKEXECUTIONSREQUEST']._serialized_end=36584
-  _globals['_SCHEDULEDTASKEXECUTION']._serialized_start=36587
-  _globals['_SCHEDULEDTASKEXECUTION']._serialized_end=36820
-  _globals['_LISTSCHEDULEDTASKEXECUTIONSRESPONSE']._serialized_start=36823
-  _globals['_LISTSCHEDULEDTASKEXECUTIONSRESPONSE']._serialized_end=36964
-  _globals['_TRANSFORMATIONFUNCTION']._serialized_start=36966
-  _globals['_TRANSFORMATIONFUNCTION']._serialized_end=37065
-  _globals['_LISTTRANSFORMATIONFUNCTIONSREQUEST']._serialized_start=37067
-  _globals['_LISTTRANSFORMATIONFUNCTIONSREQUEST']._serialized_end=37103
-  _globals['_LISTTRANSFORMATIONFUNCTIONSRESPONSE']._serialized_start=37105
-  _globals['_LISTTRANSFORMATIONFUNCTIONSRESPONSE']._serialized_end=37228
-  _globals['_GETTRANSFORMATIONFUNCTIONREQUEST']._serialized_start=37230
-  _globals['_GETTRANSFORMATIONFUNCTIONREQUEST']._serialized_end=37302
-  _globals['_GETTRANSFORMATIONFUNCTIONRESPONSE']._serialized_start=37304
-  _globals['_GETTRANSFORMATIONFUNCTIONRESPONSE']._serialized_end=37424
-  _globals['_UPDATEPROJECTREQUEST']._serialized_start=37427
-  _globals['_UPDATEPROJECTREQUEST']._serialized_end=37645
-  _globals['_UPDATEFEATURESETREQUEST']._serialized_start=37648
-  _globals['_UPDATEFEATURESETREQUEST']._serialized_end=38604
-  _globals['_UPDATEFEATUREREQUEST']._serialized_start=38607
-  _globals['_UPDATEFEATUREREQUEST']._serialized_end=39002
-  _globals['_BACKFILLOPTIONS']._serialized_start=39005
-  _globals['_BACKFILLOPTIONS']._serialized_end=39362
-  _globals['_BACKFILLOPTIONS_FEATUREMAPPINGENTRY']._serialized_start=39309
-  _globals['_BACKFILLOPTIONS_FEATUREMAPPINGENTRY']._serialized_end=39362
-  _globals['_BACKFILLRESPONSE']._serialized_start=39364
-  _globals['_BACKFILLRESPONSE']._serialized_end=39451
-  _globals['_FEATURESETDRAFTREQUEST']._serialized_start=39454
-  _globals['_FEATURESETDRAFTREQUEST']._serialized_end=39754
-  _globals['_FEATURESETMAJORVERSIONDRAFTREQUEST']._serialized_start=39757
-  _globals['_FEATURESETMAJORVERSIONDRAFTREQUEST']._serialized_end=40017
-  _globals['_DRAFTTOFEATURESETREQUEST']._serialized_start=40020
-  _globals['_DRAFTTOFEATURESETREQUEST']._serialized_end=40423
-  _globals['_DRAFTTOFEATURESETREQUEST_TIMETRAVELCOLUMN']._serialized_start=40308
-  _globals['_DRAFTTOFEATURESETREQUEST_TIMETRAVELCOLUMN']._serialized_end=40423
-  _globals['_MAJORVERSIONDRAFTTOFEATURESETVERSIONREQUEST']._serialized_start=40426
-  _globals['_MAJORVERSIONDRAFTTOFEATURESETVERSIONREQUEST']._serialized_end=40752
-  _globals['_DRAFTTOFEATURESETRESPONSE']._serialized_start=40754
-  _globals['_DRAFTTOFEATURESETRESPONSE']._serialized_end=40805
-  _globals['_MAJORVERSIONDRAFTTOFEATURESETVERSIONRESPONSE']._serialized_start=40808
-  _globals['_MAJORVERSIONDRAFTTOFEATURESETVERSIONRESPONSE']._serialized_end=40949
-  _globals['_FEATURESCHEMADRAFT']._serialized_start=40952
-  _globals['_FEATURESCHEMADRAFT']._serialized_end=41409
-  _globals['_FEATURESCHEMADRAFT_SPECIALDATA']._serialized_start=21314
-  _globals['_FEATURESCHEMADRAFT_SPECIALDATA']._serialized_end=21406
-  _globals['_FEATURESETDRAFTID']._serialized_start=41411
-  _globals['_FEATURESETDRAFTID']._serialized_end=41460
-  _globals['_LISTFEATURESETDRAFTSREQUEST']._serialized_start=41462
-  _globals['_LISTFEATURESETDRAFTSREQUEST']._serialized_end=41530
-  _globals['_LISTABLEFEATURESETDRAFT']._serialized_start=41533
-  _globals['_LISTABLEFEATURESETDRAFT']._serialized_end=42141
-  _globals['_LISTABLEFEATURESETDRAFT_FEATURESETDRAFTSTATUS']._serialized_start=41958
-  _globals['_LISTABLEFEATURESETDRAFT_FEATURESETDRAFTSTATUS']._serialized_end=42141
-  _globals['_FEATURESETDRAFT']._serialized_start=42144
-  _globals['_FEATURESETDRAFT']._serialized_end=42548
-  _globals['_LISTFEATURESETDRAFTSRESPONSE']._serialized_start=42550
-  _globals['_LISTFEATURESETDRAFTSRESPONSE']._serialized_end=42674
-  _globals['_FEATURESETDRAFTRESPONSE']._serialized_start=42676
-  _globals['_FEATURESETDRAFTRESPONSE']._serialized_end=42773
-  _globals['_ARTIFACT']._serialized_start=42776
-  _globals['_ARTIFACT']._serialized_end=43012
-  _globals['_STOREFILEARTIFACTREQUEST']._serialized_start=43015
-  _globals['_STOREFILEARTIFACTREQUEST']._serialized_end=43189
-  _globals['_STOREFILEARTIFACTRESPONSE']._serialized_start=43192
-  _globals['_STOREFILEARTIFACTRESPONSE']._serialized_end=43404
-  _globals['_STOREFILEARTIFACTRESPONSE_HEADERSENTRY']._serialized_start=27157
-  _globals['_STOREFILEARTIFACTRESPONSE_HEADERSENTRY']._serialized_end=27203
-  _globals['_RETRIEVEARTIFACTREQUEST']._serialized_start=43406
-  _globals['_RETRIEVEARTIFACTREQUEST']._serialized_end=43452
-  _globals['_RETRIEVEARTIFACTRESPONSE']._serialized_start=43454
-  _globals['_RETRIEVEARTIFACTRESPONSE']._serialized_end=43536
-  _globals['_UPDATEUPLOADSTATUSREQUEST']._serialized_start=43538
-  _globals['_UPDATEUPLOADSTATUSREQUEST']._serialized_end=43659
-  _globals['_DELETEARTIFACTREQUEST']._serialized_start=43661
-  _globals['_DELETEARTIFACTREQUEST']._serialized_end=43705
-  _globals['_LISTARTIFACTSREQUEST']._serialized_start=43707
-  _globals['_LISTARTIFACTSREQUEST']._serialized_end=43827
-  _globals['_LISTARTIFACTSRESPONSE']._serialized_start=43829
-  _globals['_LISTARTIFACTSRESPONSE']._serialized_end=43934
-  _globals['_STORELINKREQUEST']._serialized_start=43936
-  _globals['_STORELINKREQUEST']._serialized_end=44062
-  _globals['_STORELINKRESPONSE']._serialized_start=44064
-  _globals['_STORELINKRESPONSE']._serialized_end=44104
-  _globals['_FEATURESETPOPULARITY']._serialized_start=44107
-  _globals['_FEATURESETPOPULARITY']._serialized_end=44308
-  _globals['_FEATURESETSPOPULARITYRESPONSE']._serialized_start=44310
-  _globals['_FEATURESETSPOPULARITYRESPONSE']._serialized_end=44413
-  _globals['_LISTFEATURESETSTOREVIEWREQUEST']._serialized_start=44416
-  _globals['_LISTFEATURESETSTOREVIEWREQUEST']._serialized_end=44566
-  _globals['_LISTFEATURESETSTOREVIEWRESPONSE']._serialized_start=44568
-  _globals['_LISTFEATURESETSTOREVIEWRESPONSE']._serialized_end=44691
-  _globals['_FEATURESETTOREVIEW']._serialized_start=44694
-  _globals['_FEATURESETTOREVIEW']._serialized_end=45004
-  _globals['_APPROVEREVIEWREQUEST']._serialized_start=45006
-  _globals['_APPROVEREVIEWREQUEST']._serialized_end=45063
-  _globals['_REJECTREVIEWREQUEST']._serialized_start=45065
-  _globals['_REJECTREVIEWREQUEST']._serialized_end=45121
-  _globals['_LISTFEATURESETREVIEWSPAGEREQUEST']._serialized_start=45124
-  _globals['_LISTFEATURESETREVIEWSPAGEREQUEST']._serialized_end=45276
-  _globals['_FEATURESETREVIEW']._serialized_start=45279
-  _globals['_FEATURESETREVIEW']._serialized_end=45655
-  _globals['_LISTFEATURESETREVIEWSPAGERESPONSE']._serialized_start=45657
-  _globals['_LISTFEATURESETREVIEWSPAGERESPONSE']._serialized_end=45780
-  _globals['_GETLISTABLEFEATURESETTOREVIEWREQUEST']._serialized_start=45782
-  _globals['_GETLISTABLEFEATURESETTOREVIEWREQUEST']._serialized_end=45839
-  _globals['_GETLISTABLEFEATURESETTOREVIEWRESPONSE']._serialized_start=45841
-  _globals['_GETLISTABLEFEATURESETTOREVIEWRESPONSE']._serialized_end=45958
-  _globals['_GETLISTABLEFEATURESETINREVIEWREQUEST']._serialized_start=45960
-  _globals['_GETLISTABLEFEATURESETINREVIEWREQUEST']._serialized_end=46017
-  _globals['_GETLISTABLEFEATURESETINREVIEWRESPONSE']._serialized_start=46019
-  _globals['_GETLISTABLEFEATURESETINREVIEWRESPONSE']._serialized_end=46136
-  _globals['_DELETEREJECTEDFEATURESETREQUEST']._serialized_start=46138
-  _globals['_DELETEREJECTEDFEATURESETREQUEST']._serialized_end=46190
-  _globals['_LISTFEATURESTOREVIEWREQUEST']._serialized_start=46192
-  _globals['_LISTFEATURESTOREVIEWREQUEST']._serialized_end=46294
-  _globals['_LISTFEATURESTOREVIEWRESPONSE']._serialized_start=46296
-  _globals['_LISTFEATURESTOREVIEWRESPONSE']._serialized_end=46406
-  _globals['_LISTFEATURESINREVIEWREQUEST']._serialized_start=46408
-  _globals['_LISTFEATURESINREVIEWREQUEST']._serialized_end=46510
-  _globals['_LISTFEATURESINREVIEWRESPONSE']._serialized_start=46512
-  _globals['_LISTFEATURESINREVIEWRESPONSE']._serialized_end=46622
-  _globals['_GETFEATURESETPREVIEWTOREVIEWREQUEST']._serialized_start=46624
-  _globals['_GETFEATURESETPREVIEWTOREVIEWREQUEST']._serialized_end=46680
-  _globals['_GETFEATURESETPREVIEWTOREVIEWRESPONSE']._serialized_start=46682
-  _globals['_GETFEATURESETPREVIEWTOREVIEWRESPONSE']._serialized_end=46763
-  _globals['_GETFEATURESETPREVIEWINREVIEWREQUEST']._serialized_start=46765
-  _globals['_GETFEATURESETPREVIEWINREVIEWREQUEST']._serialized_end=46821
-  _globals['_GETFEATURESETPREVIEWINREVIEWRESPONSE']._serialized_start=46823
-  _globals['_GETFEATURESETPREVIEWINREVIEWRESPONSE']._serialized_end=46904
-  _globals['_GETFEATURESETTOREVIEWREQUEST']._serialized_start=46906
-  _globals['_GETFEATURESETTOREVIEWREQUEST']._serialized_end=46955
-  _globals['_GETFEATURESETTOREVIEWRESPONSE']._serialized_start=46957
-  _globals['_GETFEATURESETTOREVIEWRESPONSE']._serialized_end=47049
-  _globals['_GETFEATURESETINREVIEWREQUEST']._serialized_start=47051
-  _globals['_GETFEATURESETINREVIEWREQUEST']._serialized_end=47100
-  _globals['_GETFEATURESETINREVIEWRESPONSE']._serialized_start=47102
-  _globals['_GETFEATURESETINREVIEWRESPONSE']._serialized_end=47194
-  _globals['_RECENTLYUSEDPROJECT']._serialized_start=47197
-  _globals['_RECENTLYUSEDPROJECT']._serialized_end=47389
-  _globals['_RECENTLYUSEDPROJECTSRESPONSE']._serialized_start=47391
-  _globals['_RECENTLYUSEDPROJECTSRESPONSE']._serialized_end=47488
-  _globals['_RECENTLYUSEDFEATURESET']._serialized_start=47491
-  _globals['_RECENTLYUSEDFEATURESET']._serialized_end=47698
-  _globals['_RECENTLYUSEDFEATURESETSRESPONSE']._serialized_start=47700
-  _globals['_RECENTLYUSEDFEATURESETSRESPONSE']._serialized_end=47807
-  _globals['_TARGETFEATUREREQUEST']._serialized_start=47809
-  _globals['_TARGETFEATUREREQUEST']._serialized_end=47904
-  _globals['_LISTTARGETFEATURESREQUEST']._serialized_start=47906
-  _globals['_LISTTARGETFEATURESREQUEST']._serialized_end=47986
-  _globals['_TARGETFEATUREREFERENCE']._serialized_start=47988
-  _globals['_TARGETFEATUREREFERENCE']._serialized_end=48054
-  _globals['_LISTTARGETFEATURESRESPONSE']._serialized_start=48056
-  _globals['_LISTTARGETFEATURESRESPONSE']._serialized_end=48154
-  _globals['_LISTJOBSPAGEBYFEATURESETNAMEREQUEST']._serialized_start=48157
-  _globals['_LISTJOBSPAGEBYFEATURESETNAMEREQUEST']._serialized_end=48413
-  _globals['_LISTJOBSPAGEBYFEATURESETIDREQUEST']._serialized_start=48416
-  _globals['_LISTJOBSPAGEBYFEATURESETIDREQUEST']._serialized_end=48662
-  _globals['_FEATURESETJOBRELATEDINFO']._serialized_start=48664
-  _globals['_FEATURESETJOBRELATEDINFO']._serialized_end=48773
-  _globals['_LISTABLEJOB']._serialized_start=48776
-  _globals['_LISTABLEJOB']._serialized_end=49000
-  _globals['_LISTJOBSPAGERESPONSE']._serialized_start=49002
-  _globals['_LISTJOBSPAGERESPONSE']._serialized_end=49107
-  _globals['_GETJOBSWITHSTATUSCOUNTREQUEST']._serialized_start=49109
-  _globals['_GETJOBSWITHSTATUSCOUNTREQUEST']._serialized_end=49202
-  _globals['_GETJOBSWITHSTATUSCOUNTRESPONSE']._serialized_start=49204
-  _globals['_GETJOBSWITHSTATUSCOUNTRESPONSE']._serialized_end=49256
-  _globals['_PINFEATURESETREQUEST']._serialized_start=49258
-  _globals['_PINFEATURESETREQUEST']._serialized_end=49304
-  _globals['_UNPINFEATURESETREQUEST']._serialized_start=49306
-  _globals['_UNPINFEATURESETREQUEST']._serialized_end=49354
-  _globals['_PINNEDFEATURESETSREQUEST']._serialized_start=49356
-  _globals['_PINNEDFEATURESETSREQUEST']._serialized_end=49421
-  _globals['_PINNEDFEATURESET']._serialized_start=49424
-  _globals['_PINNEDFEATURESET']._serialized_end=49640
-  _globals['_PINNEDFEATURESETSRESPONSE']._serialized_start=49642
-  _globals['_PINNEDFEATURESETSRESPONSE']._serialized_end=49762
-  _globals['_ISFEATURESETPINNEDREQUEST']._serialized_start=49764
-  _globals['_ISFEATURESETPINNEDREQUEST']._serialized_end=49815
-  _globals['_ISFEATURESETPINNEDRESPONSE']._serialized_start=49817
-  _globals['_ISFEATURESETPINNEDRESPONSE']._serialized_end=49861
-  _globals['_CODESNIPPEDIDREQUEST']._serialized_start=49863
-  _globals['_CODESNIPPEDIDREQUEST']._serialized_end=49944
-  _globals['_CODESNIPPEDIDRESPONSE']._serialized_start=49946
-  _globals['_CODESNIPPEDIDRESPONSE']._serialized_end=49990
-  _globals['_ADVANCEDSEARCHOPTION']._serialized_start=49993
-  _globals['_ADVANCEDSEARCHOPTION']._serialized_end=50457
-  _globals['_ADVANCEDSEARCHOPTION_SEARCHOPERATOR']._serialized_start=50213
-  _globals['_ADVANCEDSEARCHOPTION_SEARCHOPERATOR']._serialized_end=50312
-  _globals['_ADVANCEDSEARCHOPTION_SEARCHFIELD']._serialized_start=50315
-  _globals['_ADVANCEDSEARCHOPTION_SEARCHFIELD']._serialized_end=50457
-  _globals['_CORESERVICE']._serialized_start=54378
-  _globals['_CORESERVICE']._serialized_end=85035
+  _globals['_GETWEBCONFIGRESPONSE']._serialized_end=2158
+  _globals['_GETFEATURESETSLASTMINORFORCURRENTMAJORREQUEST']._serialized_start=2160
+  _globals['_GETFEATURESETSLASTMINORFORCURRENTMAJORREQUEST']._serialized_end=2260
+  _globals['_GETLASTMINORFEATURESETFORMAJORINPROJECTREQUEST']._serialized_start=2263
+  _globals['_GETLASTMINORFEATURESETFORMAJORINPROJECTREQUEST']._serialized_end=2392
+  _globals['_FEATURESETEXISTSREQUEST']._serialized_start=2394
+  _globals['_FEATURESETEXISTSREQUEST']._serialized_end=2503
+  _globals['_GETINGESTHISTORYREQUEST']._serialized_start=2505
+  _globals['_GETINGESTHISTORYREQUEST']._serialized_end=2583
+  _globals['_PROJECTEXISTSREQUEST']._serialized_start=2585
+  _globals['_PROJECTEXISTSREQUEST']._serialized_end=2652
+  _globals['_FEATUREVIEWEXISTSREQUEST']._serialized_start=2654
+  _globals['_FEATUREVIEWEXISTSREQUEST']._serialized_end=2730
+  _globals['_MLDATASETEXISTSREQUEST']._serialized_start=2732
+  _globals['_MLDATASETEXISTSREQUEST']._serialized_end=2804
+  _globals['_EXISTSRESPONSE']._serialized_start=2806
+  _globals['_EXISTSRESPONSE']._serialized_end=2838
+  _globals['_PROJECTSDEFAULTRESPONSE']._serialized_start=2840
+  _globals['_PROJECTSDEFAULTRESPONSE']._serialized_end=2881
+  _globals['_HASPERMISSIONTORETRIEVEREQUEST']._serialized_start=2883
+  _globals['_HASPERMISSIONTORETRIEVEREQUEST']._serialized_end=2963
+  _globals['_HASPERMISSIONTORETRIEVERESPONSE']._serialized_start=2965
+  _globals['_HASPERMISSIONTORETRIEVERESPONSE']._serialized_end=3031
+  _globals['_STARTREVERTINGESTJOBREQUEST']._serialized_start=3033
+  _globals['_STARTREVERTINGESTJOBREQUEST']._serialized_end=3134
+  _globals['_ONLINERETRIEVEMETA']._serialized_start=3136
+  _globals['_ONLINERETRIEVEMETA']._serialized_end=3237
+  _globals['_REFRESHTOKENREQUEST']._serialized_start=3239
+  _globals['_REFRESHTOKENREQUEST']._serialized_end=3283
+  _globals['_TOKENREQUEST']._serialized_start=3285
+  _globals['_TOKENREQUEST']._serialized_end=3317
+  _globals['_GENERATETOKENREQUEST']._serialized_start=3319
+  _globals['_GENERATETOKENREQUEST']._serialized_end=3425
+  _globals['_TOKENRESPONSE']._serialized_start=3427
+  _globals['_TOKENRESPONSE']._serialized_end=3506
+  _globals['_RAWTOKENRESPONSE']._serialized_start=3508
+  _globals['_RAWTOKENRESPONSE']._serialized_end=3596
+  _globals['_TOKENSCONFIGRESPONSE']._serialized_start=3598
+  _globals['_TOKENSCONFIGRESPONSE']._serialized_end=3687
+  _globals['_LISTJOBSREQUEST']._serialized_start=3689
+  _globals['_LISTJOBSREQUEST']._serialized_end=3801
+  _globals['_LISTJOBSRESPONSE']._serialized_start=3803
+  _globals['_LISTJOBSRESPONSE']._serialized_end=3868
+  _globals['_FEATURESETSCHEMACOMPATIBILITYREQUEST']._serialized_start=3871
+  _globals['_FEATURESETSCHEMACOMPATIBILITYREQUEST']._serialized_end=4068
+  _globals['_FEATURESETSCHEMACOMPATIBILITYRESPONSE']._serialized_start=4070
+  _globals['_FEATURESETSCHEMACOMPATIBILITYRESPONSE']._serialized_end=4132
+  _globals['_FEATURESETSCHEMAPATCHREQUEST']._serialized_start=4135
+  _globals['_FEATURESETSCHEMAPATCHREQUEST']._serialized_end=4324
+  _globals['_FEATURESETSCHEMAPATCHRESPONSE']._serialized_start=4326
+  _globals['_FEATURESETSCHEMAPATCHRESPONSE']._serialized_end=4416
+  _globals['_JOBID']._serialized_start=4418
+  _globals['_JOBID']._serialized_end=4441
+  _globals['_GETRECOMMENDATIONREQUEST']._serialized_start=4443
+  _globals['_GETRECOMMENDATIONREQUEST']._serialized_end=4493
+  _globals['_GETRECOMMENDATIONRESPONSE']._serialized_start=4496
+  _globals['_GETRECOMMENDATIONRESPONSE']._serialized_end=4799
+  _globals['_GETRECOMMENDATIONRESPONSE_JOIN']._serialized_start=4603
+  _globals['_GETRECOMMENDATIONRESPONSE_JOIN']._serialized_end=4646
+  _globals['_GETRECOMMENDATIONRESPONSE_MATCH']._serialized_start=4649
+  _globals['_GETRECOMMENDATIONRESPONSE_MATCH']._serialized_end=4799
+  _globals['_JOB']._serialized_start=4802
+  _globals['_JOB']._serialized_end=5125
+  _globals['_JOBPROGRESSINPUT']._serialized_start=5127
+  _globals['_JOBPROGRESSINPUT']._serialized_end=5181
+  _globals['_JOBPROGRESSOUTPUT']._serialized_start=5184
+  _globals['_JOBPROGRESSOUTPUT']._serialized_end=5382
+  _globals['_JOBPROGRESSOUTPUT_PROGRESS']._serialized_start=5279
+  _globals['_JOBPROGRESSOUTPUT_PROGRESS']._serialized_end=5382
+  _globals['_FEATURESETPERMISSIONREQUEST']._serialized_start=5385
+  _globals['_FEATURESETPERMISSIONREQUEST']._serialized_end=5523
+  _globals['_PROJECTPERMISSIONREQUEST']._serialized_start=5526
+  _globals['_PROJECTPERMISSIONREQUEST']._serialized_end=5657
+  _globals['_STARTEXTRACTSCHEMAJOBREQUEST']._serialized_start=5660
+  _globals['_STARTEXTRACTSCHEMAJOBREQUEST']._serialized_end=5892
+  _globals['_EXTRACTSCHEMARESPONSE']._serialized_start=5895
+  _globals['_EXTRACTSCHEMARESPONSE']._serialized_end=6047
+  _globals['_LISTFEATURESETSVERSIONREQUEST']._serialized_start=6049
+  _globals['_LISTFEATURESETSVERSIONREQUEST']._serialized_end=6104
+  _globals['_FEATURESETRESPONSE']._serialized_start=6107
+  _globals['_FEATURESETRESPONSE']._serialized_end=6236
+  _globals['_UPDATEFEATURESETRESPONSE']._serialized_start=6238
+  _globals['_UPDATEFEATURESETRESPONSE']._serialized_end=6333
+  _globals['_UPDATEPROJECTRESPONSE']._serialized_start=6335
+  _globals['_UPDATEPROJECTRESPONSE']._serialized_end=6420
+  _globals['_UPDATEFEATURERESPONSE']._serialized_start=6423
+  _globals['_UPDATEFEATURERESPONSE']._serialized_end=6577
+  _globals['_PROJECTRESPONSE']._serialized_start=6579
+  _globals['_PROJECTRESPONSE']._serialized_end=6650
+  _globals['_LOGINRESPONSE']._serialized_start=6652
+  _globals['_LOGINRESPONSE']._serialized_end=6725
+  _globals['_GETACTIVEUSERRESPONSE']._serialized_start=6727
+  _globals['_GETACTIVEUSERRESPONSE']._serialized_end=6827
+  _globals['_GETPROJECTREQUEST']._serialized_start=6829
+  _globals['_GETPROJECTREQUEST']._serialized_end=6870
+  _globals['_GETPROJECTBYIDREQUEST']._serialized_start=6872
+  _globals['_GETPROJECTBYIDREQUEST']._serialized_end=6915
+  _globals['_DELETEFEATURESETREQUEST']._serialized_start=6917
+  _globals['_DELETEFEATURESETREQUEST']._serialized_end=6966
+  _globals['_DELETEFEATURESETVERSIONREQUEST']._serialized_start=6968
+  _globals['_DELETEFEATURESETVERSIONREQUEST']._serialized_end=7059
+  _globals['_LOGOUTREQUEST']._serialized_start=7061
+  _globals['_LOGOUTREQUEST']._serialized_end=7099
+  _globals['_USERBASICINFO']._serialized_start=7101
+  _globals['_USERBASICINFO']._serialized_end=7181
+  _globals['_USER']._serialized_start=7183
+  _globals['_USER']._serialized_end=7272
+  _globals['_ACCESSTOKENRESPONSE']._serialized_start=7274
+  _globals['_ACCESSTOKENRESPONSE']._serialized_end=7395
+  _globals['_DELETEPROJECTREQUEST']._serialized_start=7397
+  _globals['_DELETEPROJECTREQUEST']._serialized_end=7439
+  _globals['_CREATEPROJECTREQUEST']._serialized_start=7442
+  _globals['_CREATEPROJECTREQUEST']._serialized_end=7585
+  _globals['_CREATEPROJECTRESPONSE']._serialized_start=7587
+  _globals['_CREATEPROJECTRESPONSE']._serialized_end=7688
+  _globals['_LISTPROJECTSRESPONSE']._serialized_start=7690
+  _globals['_LISTPROJECTSRESPONSE']._serialized_end=7767
+  _globals['_LISTPROJECTHISTORYPAGEREQUEST']._serialized_start=7769
+  _globals['_LISTPROJECTHISTORYPAGEREQUEST']._serialized_end=7859
+  _globals['_PROJECTHISTORY']._serialized_start=7862
+  _globals['_PROJECTHISTORY']._serialized_end=8056
+  _globals['_LISTPROJECTHISTORYPAGERESPONSE']._serialized_start=8058
+  _globals['_LISTPROJECTHISTORYPAGERESPONSE']._serialized_end=8176
+  _globals['_GETINGESTHISTORYRESPONSE']._serialized_start=8178
+  _globals['_GETINGESTHISTORYRESPONSE']._serialized_end=8274
+  _globals['_LISTFEATURESETSPAGEREQUEST']._serialized_start=8276
+  _globals['_LISTFEATURESETSPAGEREQUEST']._serialized_end=8366
+  _globals['_LISTFEATURESETSPAGERESPONSE']._serialized_start=8368
+  _globals['_LISTFEATURESETSPAGERESPONSE']._serialized_end=8484
+  _globals['_AWSCREDENTIALS']._serialized_start=8487
+  _globals['_AWSCREDENTIALS']._serialized_end=8622
+  _globals['_AZURECREDENTIALS']._serialized_start=8625
+  _globals['_AZURECREDENTIALS']._serialized_end=8791
+  _globals['_SNOWFLAKECREDENTIALS']._serialized_start=8793
+  _globals['_SNOWFLAKECREDENTIALS']._serialized_end=8892
+  _globals['_JDBCCREDENTIALS']._serialized_start=8894
+  _globals['_JDBCCREDENTIALS']._serialized_end=8943
+  _globals['_MONGODBCREDENTIALS']._serialized_start=8945
+  _globals['_MONGODBCREDENTIALS']._serialized_end=8997
+  _globals['_DRIVECREDENTIALS']._serialized_start=8999
+  _globals['_DRIVECREDENTIALS']._serialized_end=9017
+  _globals['_CREDENTIALS']._serialized_start=9020
+  _globals['_CREDENTIALS']._serialized_end=9421
+  _globals['_LISTFEATURESETSRESPONSE']._serialized_start=9423
+  _globals['_LISTFEATURESETSRESPONSE']._serialized_end=9510
+  _globals['_LISTFEATURESETVERSIONSRESPONSE']._serialized_start=9512
+  _globals['_LISTFEATURESETVERSIONSRESPONSE']._serialized_end=9620
+  _globals['_FEATURESETVERSIONDESCRIPTION']._serialized_start=9622
+  _globals['_FEATURESETVERSIONDESCRIPTION']._serialized_end=9748
+  _globals['_GETFEATURESETREQUEST']._serialized_start=9750
+  _globals['_GETFEATURESETREQUEST']._serialized_end=9835
+  _globals['_STARTINGESTJOBREQUEST']._serialized_start=9838
+  _globals['_STARTINGESTJOBREQUEST']._serialized_end=10047
+  _globals['_INGESTRESPONSE']._serialized_start=10050
+  _globals['_INGESTRESPONSE']._serialized_end=10405
+  _globals['_INGESTRESPONSE_INGESTMETA']._serialized_start=10191
+  _globals['_INGESTRESPONSE_INGESTMETA']._serialized_end=10405
+  _globals['_RETRIEVEREQUEST']._serialized_start=10408
+  _globals['_RETRIEVEREQUEST']._serialized_end=10565
+  _globals['_RETRIEVEASLINKSRESPONSE']._serialized_start=10568
+  _globals['_RETRIEVEASLINKSRESPONSE']._serialized_end=10707
+  _globals['_RETRIEVEASSPARKRESPONSE']._serialized_start=10710
+  _globals['_RETRIEVEASSPARKRESPONSE']._serialized_end=11070
+  _globals['_RETRIEVEASSPARKRESPONSE_OPTIONSENTRY']._serialized_start=11024
+  _globals['_RETRIEVEASSPARKRESPONSE_OPTIONSENTRY']._serialized_end=11070
+  _globals['_STARTMATERIALIZATIONONLINEREQUEST']._serialized_start=11072
+  _globals['_STARTMATERIALIZATIONONLINEREQUEST']._serialized_end=11160
+  _globals['_MATERIALIZATIONONLINERESPONSE']._serialized_start=11162
+  _globals['_MATERIALIZATIONONLINERESPONSE']._serialized_end=11280
+  _globals['_STARTONLINEOFFLINEINGESTIONREQUEST']._serialized_start=11282
+  _globals['_STARTONLINEOFFLINEINGESTIONREQUEST']._serialized_end=11371
+  _globals['_INGESTWRITECREDENTIALREQUEST']._serialized_start=11373
+  _globals['_INGESTWRITECREDENTIALREQUEST']._serialized_end=11423
+  _globals['_INGESTWRITECREDENTIALRESPONSE']._serialized_start=11426
+  _globals['_INGESTWRITECREDENTIALRESPONSE']._serialized_end=11628
+  _globals['_INGESTWRITECREDENTIALRESPONSE_OPTIONSENTRY']._serialized_start=11024
+  _globals['_INGESTWRITECREDENTIALRESPONSE_OPTIONSENTRY']._serialized_end=11070
+  _globals['_STARTOPTIMIZESTORAGEJOBREQUEST']._serialized_start=11631
+  _globals['_STARTOPTIMIZESTORAGEJOBREQUEST']._serialized_end=11787
+  _globals['_STORAGEOPTIMIZATION']._serialized_start=11790
+  _globals['_STORAGEOPTIMIZATION']._serialized_end=11975
+  _globals['_OPTIMIZESTORAGEZORDERBYSPEC']._serialized_start=11977
+  _globals['_OPTIMIZESTORAGEZORDERBYSPEC']._serialized_end=12023
+  _globals['_OPTIMIZESTORAGECOMPACTSPEC']._serialized_start=12025
+  _globals['_OPTIMIZESTORAGECOMPACTSPEC']._serialized_end=12053
+  _globals['_OPTIMIZESTORAGERESPONSE']._serialized_start=12055
+  _globals['_OPTIMIZESTORAGERESPONSE']._serialized_end=12110
+  _globals['_RAWDATALOCATION']._serialized_start=12113
+  _globals['_RAWDATALOCATION']._serialized_end=12933
+  _globals['_ONLINESOURCESPEC']._serialized_start=12935
+  _globals['_ONLINESOURCESPEC']._serialized_end=12988
+  _globals['_CSVFILESPEC']._serialized_start=12990
+  _globals['_CSVFILESPEC']._serialized_end=13036
+  _globals['_JSONFILESPEC']._serialized_start=13038
+  _globals['_JSONFILESPEC']._serialized_end=13085
+  _globals['_PARQUETFILESPEC']._serialized_start=13087
+  _globals['_PARQUETFILESPEC']._serialized_end=13118
+  _globals['_TEMPPARQUETFILESPEC']._serialized_start=13120
+  _globals['_TEMPPARQUETFILESPEC']._serialized_end=13155
+  _globals['_PROXY']._serialized_start=13157
+  _globals['_PROXY']._serialized_end=13224
+  _globals['_SNOWFLAKETABLESPEC']._serialized_start=13227
+  _globals['_SNOWFLAKETABLESPEC']._serialized_end=13442
+  _globals['_JDBCTABLESPEC']._serialized_start=13445
+  _globals['_JDBCTABLESPEC']._serialized_end=13626
+  _globals['_DELTATABLESPEC']._serialized_start=13628
+  _globals['_DELTATABLESPEC']._serialized_end=13746
+  _globals['_CSVFOLDERSPEC']._serialized_start=13748
+  _globals['_CSVFOLDERSPEC']._serialized_end=13827
+  _globals['_PARQUETFOLDERSPEC']._serialized_start=13829
+  _globals['_PARQUETFOLDERSPEC']._serialized_end=13893
+  _globals['_JSONFOLDERSPEC']._serialized_start=13895
+  _globals['_JSONFOLDERSPEC']._serialized_end=13975
+  _globals['_MONGODBCOLLECTIONSPEC']._serialized_start=13977
+  _globals['_MONGODBCOLLECTIONSPEC']._serialized_end=14062
+  _globals['_MOJOTRANSFORMATION']._serialized_start=14064
+  _globals['_MOJOTRANSFORMATION']._serialized_end=14102
+  _globals['_SPARKPIPELINETRANSFORMATION']._serialized_start=14104
+  _globals['_SPARKPIPELINETRANSFORMATION']._serialized_end=14151
+  _globals['_JOINTRANSFORMATION']._serialized_start=14153
+  _globals['_JOINTRANSFORMATION']._serialized_end=14267
+  _globals['_VERSIONEDID']._serialized_start=14269
+  _globals['_VERSIONEDID']._serialized_end=14317
+  _globals['_TRANSFORMATION']._serialized_start=14320
+  _globals['_TRANSFORMATION']._serialized_end=14556
+  _globals['_DERIVEDINFORMATION']._serialized_start=14559
+  _globals['_DERIVEDINFORMATION']._serialized_end=14713
+  _globals['_SELECTEDFEATURE']._serialized_start=14715
+  _globals['_SELECTEDFEATURE']._serialized_end=14789
+  _globals['_FILTERCONDITIONUNION']._serialized_start=14792
+  _globals['_FILTERCONDITIONUNION']._serialized_end=14953
+  _globals['_FEATUREFILTER']._serialized_start=14956
+  _globals['_FEATUREFILTER']._serialized_end=15117
+  _globals['_FEATUREFILTERLOGIC']._serialized_start=15120
+  _globals['_FEATUREFILTERLOGIC']._serialized_end=15349
+  _globals['_FEATUREQUERY']._serialized_start=15352
+  _globals['_FEATUREQUERY']._serialized_end=16064
+  _globals['_FEATUREQUERY_FROM']._serialized_start=15639
+  _globals['_FEATUREQUERY_FROM']._serialized_end=15722
+  _globals['_FEATUREQUERY_JOIN']._serialized_start=15725
+  _globals['_FEATUREQUERY_JOIN']._serialized_end=16064
+  _globals['_FEATUREQUERY_JOIN_ON']._serialized_start=15941
+  _globals['_FEATUREQUERY_JOIN_ON']._serialized_end=16064
+  _globals['_FEATUREVIEW']._serialized_start=16067
+  _globals['_FEATUREVIEW']._serialized_end=16221
+  _globals['_CREATEFEATUREVIEWREQUEST']._serialized_start=16224
+  _globals['_CREATEFEATUREVIEWREQUEST']._serialized_end=16362
+  _globals['_UPDATEFEATUREVIEWREQUEST']._serialized_start=16364
+  _globals['_UPDATEFEATUREVIEWREQUEST']._serialized_end=16466
+  _globals['_CREATEFEATUREVIEWNEWVERSIONREQUEST']._serialized_start=16469
+  _globals['_CREATEFEATUREVIEWNEWVERSIONREQUEST']._serialized_end=16617
+  _globals['_GETFEATUREVIEWREQUEST']._serialized_start=16619
+  _globals['_GETFEATUREVIEWREQUEST']._serialized_end=16693
+  _globals['_FEATUREVIEWRESPONSE']._serialized_start=16695
+  _globals['_FEATUREVIEWRESPONSE']._serialized_end=16779
+  _globals['_LISTFEATUREVIEWSREQUEST']._serialized_start=16781
+  _globals['_LISTFEATUREVIEWSREQUEST']._serialized_end=16826
+  _globals['_LISTFEATUREVIEWSRESPONSE']._serialized_start=16828
+  _globals['_LISTFEATUREVIEWSRESPONSE']._serialized_end=16918
+  _globals['_RETRIEVEFEATUREVIEWASSPARKREQUEST']._serialized_start=16921
+  _globals['_RETRIEVEFEATUREVIEWASSPARKREQUEST']._serialized_end=17121
+  _globals['_RETRIEVEFEATUREVIEWASSPARKRESPONSE']._serialized_start=17124
+  _globals['_RETRIEVEFEATUREVIEWASSPARKRESPONSE']._serialized_end=17418
+  _globals['_RETRIEVEFEATUREVIEWASSPARKRESPONSE_OPTIONSENTRY']._serialized_start=11024
+  _globals['_RETRIEVEFEATUREVIEWASSPARKRESPONSE_OPTIONSENTRY']._serialized_end=11070
+  _globals['_RETRIEVEFEATUREVIEWASASLINKSREQUEST']._serialized_start=17421
+  _globals['_RETRIEVEFEATUREVIEWASASLINKSREQUEST']._serialized_end=17603
+  _globals['_RETRIEVEFEATUREVIEWASASLINKSRESPONSE']._serialized_start=17605
+  _globals['_RETRIEVEFEATUREVIEWASASLINKSRESPONSE']._serialized_end=17667
+  _globals['_DELETEFEATUREVIEWREQUEST']._serialized_start=17669
+  _globals['_DELETEFEATUREVIEWREQUEST']._serialized_end=17720
+  _globals['_MLDATASETFEATURE']._serialized_start=17723
+  _globals['_MLDATASETFEATURE']._serialized_end=18122
+  _globals['_MLDATASET']._serialized_start=18125
+  _globals['_MLDATASET']._serialized_end=18627
+  _globals['_MLDATASET_MLDATASETSTATE']._serialized_start=18519
+  _globals['_MLDATASET_MLDATASETSTATE']._serialized_end=18627
+  _globals['_CREATEMLDATASETREQUEST']._serialized_start=18630
+  _globals['_CREATEMLDATASETREQUEST']._serialized_end=18848
+  _globals['_UPDATEMLDATASETREQUEST']._serialized_start=18850
+  _globals['_UPDATEMLDATASETREQUEST']._serialized_end=18918
+  _globals['_DELETEMLDATASETREQUEST']._serialized_start=18920
+  _globals['_DELETEMLDATASETREQUEST']._serialized_end=18967
+  _globals['_CREATEMLDATASETRESPONSE']._serialized_start=18970
+  _globals['_CREATEMLDATASETRESPONSE']._serialized_end=19102
+  _globals['_GETMLDATASETREQUEST']._serialized_start=19104
+  _globals['_GETMLDATASETREQUEST']._serialized_end=19205
+  _globals['_LISTMLDATASETSREQUEST']._serialized_start=19207
+  _globals['_LISTMLDATASETSREQUEST']._serialized_end=19285
+  _globals['_LISTMLDATASETSRESPONSE']._serialized_start=19287
+  _globals['_LISTMLDATASETSRESPONSE']._serialized_end=19371
+  _globals['_RETRIEVEMLDATASETASSPARKREQUEST']._serialized_start=19373
+  _globals['_RETRIEVEMLDATASETASSPARKREQUEST']._serialized_end=19449
+  _globals['_RETRIEVEMLDATASETASSPARKRESPONSE']._serialized_start=19452
+  _globals['_RETRIEVEMLDATASETASSPARKRESPONSE']._serialized_end=19742
+  _globals['_RETRIEVEMLDATASETASSPARKRESPONSE_OPTIONSENTRY']._serialized_start=11024
+  _globals['_RETRIEVEMLDATASETASSPARKRESPONSE_OPTIONSENTRY']._serialized_end=11070
+  _globals['_RETRIEVEMLDATASETASASLINKSREQUEST']._serialized_start=19744
+  _globals['_RETRIEVEMLDATASETASASLINKSREQUEST']._serialized_end=19802
+  _globals['_RETRIEVEMLDATASETASASLINKSRESPONSE']._serialized_start=19804
+  _globals['_RETRIEVEMLDATASETASASLINKSRESPONSE']._serialized_end=19864
+  _globals['_FEATURESET']._serialized_start=19867
+  _globals['_FEATURESET']._serialized_end=21848
+  _globals['_FEATURESET_STATISTICS']._serialized_start=21448
+  _globals['_FEATURESET_STATISTICS']._serialized_end=21505
+  _globals['_FEATURESET_SPECIALDATA']._serialized_start=21508
+  _globals['_FEATURESET_SPECIALDATA']._serialized_end=21766
+  _globals['_FEATURESET_SPECIALDATA_LEGAL']._serialized_start=21675
+  _globals['_FEATURESET_SPECIALDATA_LEGAL']._serialized_end=21766
+  _globals['_FEATURESET_ONLINE']._serialized_start=21768
+  _globals['_FEATURESET_ONLINE']._serialized_end=21842
+  _globals['_GETFEATURESETPREVIEWREQUEST']._serialized_start=21850
+  _globals['_GETFEATURESETPREVIEWREQUEST']._serialized_end=21932
+  _globals['_GETFEATURESETPREVIEWRESPONSE']._serialized_start=21934
+  _globals['_GETFEATURESETPREVIEWRESPONSE']._serialized_end=22007
+  _globals['_SCOPE']._serialized_start=22009
+  _globals['_SCOPE']._serialized_end=22120
+  _globals['_REGISTERFEATURESETREQUEST']._serialized_start=22123
+  _globals['_REGISTERFEATURESETREQUEST']._serialized_end=23098
+  _globals['_CREATENEWFEATURESETVERSIONREQUEST']._serialized_start=23101
+  _globals['_CREATENEWFEATURESETVERSIONREQUEST']._serialized_end=23793
+  _globals['_FEATUREPROFILE']._serialized_start=23796
+  _globals['_FEATUREPROFILE']._serialized_end=24051
+  _globals['_FEATURESCHEMA']._serialized_start=24054
+  _globals['_FEATURESCHEMA']._serialized_end=24598
+  _globals['_FEATURESCHEMA_SPECIALDATA']._serialized_start=21508
+  _globals['_FEATURESCHEMA_SPECIALDATA']._serialized_end=21600
+  _globals['_FEATURESCHEMA_MONITORING']._serialized_start=24559
+  _globals['_FEATURESCHEMA_MONITORING']._serialized_end=24598
+  _globals['_FEATURE']._serialized_start=24601
+  _globals['_FEATURE']._serialized_end=25258
+  _globals['_FEATURE_MONITORING']._serialized_start=24559
+  _globals['_FEATURE_MONITORING']._serialized_end=24598
+  _globals['_FEATURE_SPECIALDATA']._serialized_start=21508
+  _globals['_FEATURE_SPECIALDATA']._serialized_end=21600
+  _globals['_FEATURESTATISTICS']._serialized_start=25261
+  _globals['_FEATURESTATISTICS']._serialized_end=25433
+  _globals['_CATEGORICALFEATURESTATISTICS']._serialized_start=25436
+  _globals['_CATEGORICALFEATURESTATISTICS']._serialized_end=25607
+  _globals['_CATEGORICALFEATURESTATISTICS_FEATURETOP']._serialized_start=25566
+  _globals['_CATEGORICALFEATURESTATISTICS_FEATURETOP']._serialized_end=25607
+  _globals['_GETVERSIONRESPONSE']._serialized_start=25609
+  _globals['_GETVERSIONRESPONSE']._serialized_end=25646
+  _globals['_GETAPICONFIGRESPONSE']._serialized_start=25648
+  _globals['_GETAPICONFIGRESPONSE']._serialized_end=25740
+  _globals['_GETGPTECONFIGRESPONSE']._serialized_start=25742
+  _globals['_GETGPTECONFIGRESPONSE']._serialized_end=25782
+  _globals['_PROJECT']._serialized_start=25785
+  _globals['_PROJECT']._serialized_end=26194
+  _globals['_LISTABLEPROJECT']._serialized_start=26197
+  _globals['_LISTABLEPROJECT']._serialized_end=26489
+  _globals['_FEATURESETINGEST']._serialized_start=26492
+  _globals['_FEATURESETINGEST']._serialized_end=26866
+  _globals['_PERSONALACCESSTOKEN']._serialized_start=26869
+  _globals['_PERSONALACCESSTOKEN']._serialized_end=27084
+  _globals['_GENERATETRANSFORMATIONUPLOADREQUEST']._serialized_start=27087
+  _globals['_GENERATETRANSFORMATIONUPLOADREQUEST']._serialized_end=27223
+  _globals['_GENERATETRANSFORMATIONUPLOADRESPONSE']._serialized_start=27226
+  _globals['_GENERATETRANSFORMATIONUPLOADRESPONSE']._serialized_end=27439
+  _globals['_GENERATETRANSFORMATIONUPLOADRESPONSE_HEADERSENTRY']._serialized_start=27393
+  _globals['_GENERATETRANSFORMATIONUPLOADRESPONSE_HEADERSENTRY']._serialized_end=27439
+  _globals['_LISTPROJECTSPAGEREQUEST']._serialized_start=27441
+  _globals['_LISTPROJECTSPAGEREQUEST']._serialized_end=27505
+  _globals['_LISTPROJECTSPAGERESPONSE']._serialized_start=27507
+  _globals['_LISTPROJECTSPAGERESPONSE']._serialized_end=27613
+  _globals['_PROJECTSEARCHREQUEST']._serialized_start=27616
+  _globals['_PROJECTSEARCHREQUEST']._serialized_end=28160
+  _globals['_PROJECTSEARCHREQUEST_PROJECTSORTFIELD']._serialized_start=27945
+  _globals['_PROJECTSEARCHREQUEST_PROJECTSORTFIELD']._serialized_end=28160
+  _globals['_FEATURESETSEARCHREQUEST']._serialized_start=28163
+  _globals['_FEATURESETSEARCHREQUEST']._serialized_end=28761
+  _globals['_FEATURESETSEARCHREQUEST_FEATURESETSORTFIELD']._serialized_start=28513
+  _globals['_FEATURESETSEARCHREQUEST_FEATURESETSORTFIELD']._serialized_end=28761
+  _globals['_FEATURESEARCHREQUEST']._serialized_start=28764
+  _globals['_FEATURESEARCHREQUEST']._serialized_end=29154
+  _globals['_FEATURESEARCHREQUEST_FEATURESORTFIELD']._serialized_start=29037
+  _globals['_FEATURESEARCHREQUEST_FEATURESORTFIELD']._serialized_end=29154
+  _globals['_PROJECTSEARCHRESULTS']._serialized_start=29156
+  _globals['_PROJECTSEARCHRESULTS']._serialized_end=29274
+  _globals['_LISTABLEFEATURESET']._serialized_start=29277
+  _globals['_LISTABLEFEATURESET']._serialized_end=30935
+  _globals['_FEATURESETSEARCHRESULTS']._serialized_start=30938
+  _globals['_FEATURESETSEARCHRESULTS']._serialized_end=31066
+  _globals['_LISTABLEFEATURE']._serialized_start=31069
+  _globals['_LISTABLEFEATURE']._serialized_end=31291
+  _globals['_FEATURESEARCHRESULTS']._serialized_start=31293
+  _globals['_FEATURESEARCHRESULTS']._serialized_end=31411
+  _globals['_FEATURESETREQUESTID']._serialized_start=31413
+  _globals['_FEATURESETREQUESTID']._serialized_end=31487
+  _globals['_GETFEATUREREQUEST']._serialized_start=31489
+  _globals['_GETFEATUREREQUEST']._serialized_end=31581
+  _globals['_LISTFEATURESPAGERESPONSE']._serialized_start=31583
+  _globals['_LISTFEATURESPAGERESPONSE']._serialized_end=31689
+  _globals['_FEATURERESPONSE']._serialized_start=31691
+  _globals['_FEATURERESPONSE']._serialized_end=31762
+  _globals['_LISTFEATURESREQUEST']._serialized_start=31765
+  _globals['_LISTFEATURESREQUEST']._serialized_end=31893
+  _globals['_LISTFEATURESRESPONSE']._serialized_start=31895
+  _globals['_LISTFEATURESRESPONSE']._serialized_end=31997
+  _globals['_LISTABLEFEATURESETREQUEST']._serialized_start=31999
+  _globals['_LISTABLEFEATURESETREQUEST']._serialized_end=32079
+  _globals['_LISTABLEFEATURESETRESPONSE']._serialized_start=32081
+  _globals['_LISTABLEFEATURESETRESPONSE']._serialized_end=32187
+  _globals['_FEATURESETSDERIVEDFROMREQUEST']._serialized_start=32189
+  _globals['_FEATURESETSDERIVEDFROMREQUEST']._serialized_end=32279
+  _globals['_FEATURESETSDERIVEDFROMRESPONSE']._serialized_start=32281
+  _globals['_FEATURESETSDERIVEDFROMRESPONSE']._serialized_end=32392
+  _globals['_SUBMITPENDINGPERMISSIONREQUEST']._serialized_start=32395
+  _globals['_SUBMITPENDINGPERMISSIONREQUEST']._serialized_end=32528
+  _globals['_SUBMITPENDINGPERMISSIONRESPONSE']._serialized_start=32530
+  _globals['_SUBMITPENDINGPERMISSIONRESPONSE']._serialized_end=32586
+  _globals['_LISTPERMISSIONSPAGEREQUEST']._serialized_start=32589
+  _globals['_LISTPERMISSIONSPAGEREQUEST']._serialized_end=32739
+  _globals['_LISTPROJECTSPERMISSIONSPAGERESPONSE']._serialized_start=32742
+  _globals['_LISTPROJECTSPERMISSIONSPAGERESPONSE']._serialized_end=32878
+  _globals['_LISTFEATURESETSPERMISSIONSPAGERESPONSE']._serialized_start=32881
+  _globals['_LISTFEATURESETSPERMISSIONSPAGERESPONSE']._serialized_end=33023
+  _globals['_LISTABLEPROJECTTOPERMISSION']._serialized_start=33026
+  _globals['_LISTABLEPROJECTTOPERMISSION']._serialized_end=33177
+  _globals['_LISTABLEFEATURESETTOPERMISSION']._serialized_start=33180
+  _globals['_LISTABLEFEATURESETTOPERMISSION']._serialized_end=33341
+  _globals['_PERMISSION']._serialized_start=33344
+  _globals['_PERMISSION']._serialized_end=34476
+  _globals['_PERMISSION_PROMOTEDUPDATE']._serialized_start=34016
+  _globals['_PERMISSION_PROMOTEDUPDATE']._serialized_end=34188
+  _globals['_PERMISSION_REVOKEDUPDATE']._serialized_start=34191
+  _globals['_PERMISSION_REVOKEDUPDATE']._serialized_end=34327
+  _globals['_PERMISSION_GRANTEDORREJECTEDUPDATE']._serialized_start=34330
+  _globals['_PERMISSION_GRANTEDORREJECTEDUPDATE']._serialized_end=34476
+  _globals['_REVOKEPERMISSIONREQUEST']._serialized_start=34478
+  _globals['_REVOKEPERMISSIONREQUEST']._serialized_end=34542
+  _globals['_APPROVEPENDINGPERMISSIONREQUEST']._serialized_start=34544
+  _globals['_APPROVEPENDINGPERMISSIONREQUEST']._serialized_end=34616
+  _globals['_REJECTPENDINGPERMISSIONREQUEST']._serialized_start=34618
+  _globals['_REJECTPENDINGPERMISSIONREQUEST']._serialized_end=34689
+  _globals['_WITHDRAWPENDINGPERMISSIONREQUEST']._serialized_start=34691
+  _globals['_WITHDRAWPENDINGPERMISSIONREQUEST']._serialized_end=34748
+  _globals['_GETACTIVEPERMISSIONREQUEST']._serialized_start=34750
+  _globals['_GETACTIVEPERMISSIONREQUEST']._serialized_end=34799
+  _globals['_GETACTIVEPERMISSIONRESPONSE']._serialized_start=34802
+  _globals['_GETACTIVEPERMISSIONRESPONSE']._serialized_end=34962
+  _globals['_SCHEDULEDTASK']._serialized_start=34965
+  _globals['_SCHEDULEDTASK']._serialized_end=35556
+  _globals['_SCHEDULETASKREQUEST']._serialized_start=35559
+  _globals['_SCHEDULETASKREQUEST']._serialized_end=35872
+  _globals['_LISTSCHEDULEDTASKSREQUEST']._serialized_start=35874
+  _globals['_LISTSCHEDULEDTASKSREQUEST']._serialized_end=35964
+  _globals['_LISTSCHEDULEDTASKSRESPONSE']._serialized_start=35966
+  _globals['_LISTSCHEDULEDTASKSRESPONSE']._serialized_end=36077
+  _globals['_SCHEDULEDTASKID']._serialized_start=36079
+  _globals['_SCHEDULEDTASKID']._serialized_end=36123
+  _globals['_SCHEDULEDTASKRESPONSE']._serialized_start=36125
+  _globals['_SCHEDULEDTASKRESPONSE']._serialized_end=36205
+  _globals['_SCHEDULEDTASKUPDATEREQUEST']._serialized_start=36207
+  _globals['_SCHEDULEDTASKUPDATEREQUEST']._serialized_end=36325
+  _globals['_PAUSESCHEDULEDTASKREQUEST']._serialized_start=36327
+  _globals['_PAUSESCHEDULEDTASKREQUEST']._serialized_end=36381
+  _globals['_RESUMESCHEDULEDTASKREQUEST']._serialized_start=36383
+  _globals['_RESUMESCHEDULEDTASKREQUEST']._serialized_end=36488
+  _globals['_LAZYINGESTREQUEST']._serialized_start=36490
+  _globals['_LAZYINGESTREQUEST']._serialized_end=36562
+  _globals['_LAZYINGESTRESPONSE']._serialized_start=36564
+  _globals['_LAZYINGESTRESPONSE']._serialized_end=36635
+  _globals['_GETLAZYINGESTTASKREQUEST']._serialized_start=36637
+  _globals['_GETLAZYINGESTTASKREQUEST']._serialized_end=36716
+  _globals['_LISTSCHEDULEDTASKEXECUTIONSREQUEST']._serialized_start=36718
+  _globals['_LISTSCHEDULEDTASKEXECUTIONSREQUEST']._serialized_end=36820
+  _globals['_SCHEDULEDTASKEXECUTION']._serialized_start=36823
+  _globals['_SCHEDULEDTASKEXECUTION']._serialized_end=37056
+  _globals['_LISTSCHEDULEDTASKEXECUTIONSRESPONSE']._serialized_start=37059
+  _globals['_LISTSCHEDULEDTASKEXECUTIONSRESPONSE']._serialized_end=37200
+  _globals['_TRANSFORMATIONFUNCTION']._serialized_start=37202
+  _globals['_TRANSFORMATIONFUNCTION']._serialized_end=37301
+  _globals['_LISTTRANSFORMATIONFUNCTIONSREQUEST']._serialized_start=37303
+  _globals['_LISTTRANSFORMATIONFUNCTIONSREQUEST']._serialized_end=37339
+  _globals['_LISTTRANSFORMATIONFUNCTIONSRESPONSE']._serialized_start=37341
+  _globals['_LISTTRANSFORMATIONFUNCTIONSRESPONSE']._serialized_end=37464
+  _globals['_GETTRANSFORMATIONFUNCTIONREQUEST']._serialized_start=37466
+  _globals['_GETTRANSFORMATIONFUNCTIONREQUEST']._serialized_end=37538
+  _globals['_GETTRANSFORMATIONFUNCTIONRESPONSE']._serialized_start=37540
+  _globals['_GETTRANSFORMATIONFUNCTIONRESPONSE']._serialized_end=37660
+  _globals['_UPDATEPROJECTREQUEST']._serialized_start=37663
+  _globals['_UPDATEPROJECTREQUEST']._serialized_end=37881
+  _globals['_UPDATEFEATURESETREQUEST']._serialized_start=37884
+  _globals['_UPDATEFEATURESETREQUEST']._serialized_end=38840
+  _globals['_UPDATEFEATUREREQUEST']._serialized_start=38843
+  _globals['_UPDATEFEATUREREQUEST']._serialized_end=39238
+  _globals['_BACKFILLOPTIONS']._serialized_start=39241
+  _globals['_BACKFILLOPTIONS']._serialized_end=39598
+  _globals['_BACKFILLOPTIONS_FEATUREMAPPINGENTRY']._serialized_start=39545
+  _globals['_BACKFILLOPTIONS_FEATUREMAPPINGENTRY']._serialized_end=39598
+  _globals['_BACKFILLRESPONSE']._serialized_start=39600
+  _globals['_BACKFILLRESPONSE']._serialized_end=39687
+  _globals['_FEATURESETDRAFTREQUEST']._serialized_start=39690
+  _globals['_FEATURESETDRAFTREQUEST']._serialized_end=39990
+  _globals['_FEATURESETMAJORVERSIONDRAFTREQUEST']._serialized_start=39993
+  _globals['_FEATURESETMAJORVERSIONDRAFTREQUEST']._serialized_end=40253
+  _globals['_DRAFTTOFEATURESETREQUEST']._serialized_start=40256
+  _globals['_DRAFTTOFEATURESETREQUEST']._serialized_end=40659
+  _globals['_DRAFTTOFEATURESETREQUEST_TIMETRAVELCOLUMN']._serialized_start=40544
+  _globals['_DRAFTTOFEATURESETREQUEST_TIMETRAVELCOLUMN']._serialized_end=40659
+  _globals['_MAJORVERSIONDRAFTTOFEATURESETVERSIONREQUEST']._serialized_start=40662
+  _globals['_MAJORVERSIONDRAFTTOFEATURESETVERSIONREQUEST']._serialized_end=41059
+  _globals['_DRAFTTOFEATURESETRESPONSE']._serialized_start=41061
+  _globals['_DRAFTTOFEATURESETRESPONSE']._serialized_end=41112
+  _globals['_MAJORVERSIONDRAFTTOFEATURESETVERSIONRESPONSE']._serialized_start=41115
+  _globals['_MAJORVERSIONDRAFTTOFEATURESETVERSIONRESPONSE']._serialized_end=41256
+  _globals['_FEATURESCHEMADRAFT']._serialized_start=41259
+  _globals['_FEATURESCHEMADRAFT']._serialized_end=41716
+  _globals['_FEATURESCHEMADRAFT_SPECIALDATA']._serialized_start=21508
+  _globals['_FEATURESCHEMADRAFT_SPECIALDATA']._serialized_end=21600
+  _globals['_FEATURESETDRAFTID']._serialized_start=41718
+  _globals['_FEATURESETDRAFTID']._serialized_end=41767
+  _globals['_LISTFEATURESETDRAFTSREQUEST']._serialized_start=41769
+  _globals['_LISTFEATURESETDRAFTSREQUEST']._serialized_end=41837
+  _globals['_LISTABLEFEATURESETDRAFT']._serialized_start=41840
+  _globals['_LISTABLEFEATURESETDRAFT']._serialized_end=42448
+  _globals['_LISTABLEFEATURESETDRAFT_FEATURESETDRAFTSTATUS']._serialized_start=42265
+  _globals['_LISTABLEFEATURESETDRAFT_FEATURESETDRAFTSTATUS']._serialized_end=42448
+  _globals['_FEATURESETDRAFT']._serialized_start=42451
+  _globals['_FEATURESETDRAFT']._serialized_end=42855
+  _globals['_LISTFEATURESETDRAFTSRESPONSE']._serialized_start=42857
+  _globals['_LISTFEATURESETDRAFTSRESPONSE']._serialized_end=42981
+  _globals['_FEATURESETDRAFTRESPONSE']._serialized_start=42983
+  _globals['_FEATURESETDRAFTRESPONSE']._serialized_end=43080
+  _globals['_ARTIFACT']._serialized_start=43083
+  _globals['_ARTIFACT']._serialized_end=43319
+  _globals['_STOREFILEARTIFACTREQUEST']._serialized_start=43322
+  _globals['_STOREFILEARTIFACTREQUEST']._serialized_end=43496
+  _globals['_STOREFILEARTIFACTRESPONSE']._serialized_start=43499
+  _globals['_STOREFILEARTIFACTRESPONSE']._serialized_end=43711
+  _globals['_STOREFILEARTIFACTRESPONSE_HEADERSENTRY']._serialized_start=27393
+  _globals['_STOREFILEARTIFACTRESPONSE_HEADERSENTRY']._serialized_end=27439
+  _globals['_RETRIEVEARTIFACTREQUEST']._serialized_start=43713
+  _globals['_RETRIEVEARTIFACTREQUEST']._serialized_end=43759
+  _globals['_RETRIEVEARTIFACTRESPONSE']._serialized_start=43761
+  _globals['_RETRIEVEARTIFACTRESPONSE']._serialized_end=43843
+  _globals['_UPDATEUPLOADSTATUSREQUEST']._serialized_start=43845
+  _globals['_UPDATEUPLOADSTATUSREQUEST']._serialized_end=43966
+  _globals['_DELETEARTIFACTREQUEST']._serialized_start=43968
+  _globals['_DELETEARTIFACTREQUEST']._serialized_end=44012
+  _globals['_LISTARTIFACTSREQUEST']._serialized_start=44014
+  _globals['_LISTARTIFACTSREQUEST']._serialized_end=44134
+  _globals['_LISTARTIFACTSRESPONSE']._serialized_start=44136
+  _globals['_LISTARTIFACTSRESPONSE']._serialized_end=44241
+  _globals['_STORELINKREQUEST']._serialized_start=44243
+  _globals['_STORELINKREQUEST']._serialized_end=44369
+  _globals['_STORELINKRESPONSE']._serialized_start=44371
+  _globals['_STORELINKRESPONSE']._serialized_end=44411
+  _globals['_FEATURESETPOPULARITY']._serialized_start=44414
+  _globals['_FEATURESETPOPULARITY']._serialized_end=44615
+  _globals['_FEATURESETSPOPULARITYRESPONSE']._serialized_start=44617
+  _globals['_FEATURESETSPOPULARITYRESPONSE']._serialized_end=44720
+  _globals['_LISTFEATURESETSTOREVIEWREQUEST']._serialized_start=44723
+  _globals['_LISTFEATURESETSTOREVIEWREQUEST']._serialized_end=44873
+  _globals['_LISTFEATURESETSTOREVIEWRESPONSE']._serialized_start=44875
+  _globals['_LISTFEATURESETSTOREVIEWRESPONSE']._serialized_end=44998
+  _globals['_FEATURESETTOREVIEW']._serialized_start=45001
+  _globals['_FEATURESETTOREVIEW']._serialized_end=45311
+  _globals['_APPROVEREVIEWREQUEST']._serialized_start=45313
+  _globals['_APPROVEREVIEWREQUEST']._serialized_end=45370
+  _globals['_REJECTREVIEWREQUEST']._serialized_start=45372
+  _globals['_REJECTREVIEWREQUEST']._serialized_end=45428
+  _globals['_LISTFEATURESETREVIEWSPAGEREQUEST']._serialized_start=45431
+  _globals['_LISTFEATURESETREVIEWSPAGEREQUEST']._serialized_end=45583
+  _globals['_FEATURESETREVIEW']._serialized_start=45586
+  _globals['_FEATURESETREVIEW']._serialized_end=45962
+  _globals['_LISTFEATURESETREVIEWSPAGERESPONSE']._serialized_start=45964
+  _globals['_LISTFEATURESETREVIEWSPAGERESPONSE']._serialized_end=46087
+  _globals['_GETLISTABLEFEATURESETTOREVIEWREQUEST']._serialized_start=46089
+  _globals['_GETLISTABLEFEATURESETTOREVIEWREQUEST']._serialized_end=46146
+  _globals['_GETLISTABLEFEATURESETTOREVIEWRESPONSE']._serialized_start=46148
+  _globals['_GETLISTABLEFEATURESETTOREVIEWRESPONSE']._serialized_end=46265
+  _globals['_GETLISTABLEFEATURESETINREVIEWREQUEST']._serialized_start=46267
+  _globals['_GETLISTABLEFEATURESETINREVIEWREQUEST']._serialized_end=46324
+  _globals['_GETLISTABLEFEATURESETINREVIEWRESPONSE']._serialized_start=46326
+  _globals['_GETLISTABLEFEATURESETINREVIEWRESPONSE']._serialized_end=46443
+  _globals['_DELETEREJECTEDFEATURESETREQUEST']._serialized_start=46445
+  _globals['_DELETEREJECTEDFEATURESETREQUEST']._serialized_end=46497
+  _globals['_LISTFEATURESTOREVIEWREQUEST']._serialized_start=46499
+  _globals['_LISTFEATURESTOREVIEWREQUEST']._serialized_end=46601
+  _globals['_LISTFEATURESTOREVIEWRESPONSE']._serialized_start=46603
+  _globals['_LISTFEATURESTOREVIEWRESPONSE']._serialized_end=46713
+  _globals['_LISTFEATURESINREVIEWREQUEST']._serialized_start=46715
+  _globals['_LISTFEATURESINREVIEWREQUEST']._serialized_end=46817
+  _globals['_LISTFEATURESINREVIEWRESPONSE']._serialized_start=46819
+  _globals['_LISTFEATURESINREVIEWRESPONSE']._serialized_end=46929
+  _globals['_GETFEATURESETPREVIEWTOREVIEWREQUEST']._serialized_start=46931
+  _globals['_GETFEATURESETPREVIEWTOREVIEWREQUEST']._serialized_end=46987
+  _globals['_GETFEATURESETPREVIEWTOREVIEWRESPONSE']._serialized_start=46989
+  _globals['_GETFEATURESETPREVIEWTOREVIEWRESPONSE']._serialized_end=47070
+  _globals['_GETFEATURESETPREVIEWINREVIEWREQUEST']._serialized_start=47072
+  _globals['_GETFEATURESETPREVIEWINREVIEWREQUEST']._serialized_end=47128
+  _globals['_GETFEATURESETPREVIEWINREVIEWRESPONSE']._serialized_start=47130
+  _globals['_GETFEATURESETPREVIEWINREVIEWRESPONSE']._serialized_end=47211
+  _globals['_GETFEATURESETTOREVIEWREQUEST']._serialized_start=47213
+  _globals['_GETFEATURESETTOREVIEWREQUEST']._serialized_end=47262
+  _globals['_GETFEATURESETTOREVIEWRESPONSE']._serialized_start=47264
+  _globals['_GETFEATURESETTOREVIEWRESPONSE']._serialized_end=47356
+  _globals['_GETFEATURESETINREVIEWREQUEST']._serialized_start=47358
+  _globals['_GETFEATURESETINREVIEWREQUEST']._serialized_end=47407
+  _globals['_GETFEATURESETINREVIEWRESPONSE']._serialized_start=47409
+  _globals['_GETFEATURESETINREVIEWRESPONSE']._serialized_end=47501
+  _globals['_RECENTLYUSEDPROJECT']._serialized_start=47504
+  _globals['_RECENTLYUSEDPROJECT']._serialized_end=47696
+  _globals['_RECENTLYUSEDPROJECTSRESPONSE']._serialized_start=47698
+  _globals['_RECENTLYUSEDPROJECTSRESPONSE']._serialized_end=47795
+  _globals['_RECENTLYUSEDFEATURESET']._serialized_start=47798
+  _globals['_RECENTLYUSEDFEATURESET']._serialized_end=48005
+  _globals['_RECENTLYUSEDFEATURESETSRESPONSE']._serialized_start=48007
+  _globals['_RECENTLYUSEDFEATURESETSRESPONSE']._serialized_end=48114
+  _globals['_TARGETFEATUREREQUEST']._serialized_start=48116
+  _globals['_TARGETFEATUREREQUEST']._serialized_end=48211
+  _globals['_LISTTARGETFEATURESREQUEST']._serialized_start=48213
+  _globals['_LISTTARGETFEATURESREQUEST']._serialized_end=48293
+  _globals['_TARGETFEATUREREFERENCE']._serialized_start=48295
+  _globals['_TARGETFEATUREREFERENCE']._serialized_end=48361
+  _globals['_LISTTARGETFEATURESRESPONSE']._serialized_start=48363
+  _globals['_LISTTARGETFEATURESRESPONSE']._serialized_end=48461
+  _globals['_LISTJOBSPAGEBYFEATURESETNAMEREQUEST']._serialized_start=48464
+  _globals['_LISTJOBSPAGEBYFEATURESETNAMEREQUEST']._serialized_end=48720
+  _globals['_LISTJOBSPAGEBYFEATURESETIDREQUEST']._serialized_start=48723
+  _globals['_LISTJOBSPAGEBYFEATURESETIDREQUEST']._serialized_end=48969
+  _globals['_FEATURESETJOBRELATEDINFO']._serialized_start=48971
+  _globals['_FEATURESETJOBRELATEDINFO']._serialized_end=49080
+  _globals['_LISTABLEJOB']._serialized_start=49083
+  _globals['_LISTABLEJOB']._serialized_end=49307
+  _globals['_LISTJOBSPAGERESPONSE']._serialized_start=49309
+  _globals['_LISTJOBSPAGERESPONSE']._serialized_end=49414
+  _globals['_GETJOBSWITHSTATUSCOUNTREQUEST']._serialized_start=49416
+  _globals['_GETJOBSWITHSTATUSCOUNTREQUEST']._serialized_end=49509
+  _globals['_GETJOBSWITHSTATUSCOUNTRESPONSE']._serialized_start=49511
+  _globals['_GETJOBSWITHSTATUSCOUNTRESPONSE']._serialized_end=49563
+  _globals['_PINFEATURESETREQUEST']._serialized_start=49565
+  _globals['_PINFEATURESETREQUEST']._serialized_end=49611
+  _globals['_UNPINFEATURESETREQUEST']._serialized_start=49613
+  _globals['_UNPINFEATURESETREQUEST']._serialized_end=49661
+  _globals['_PINNEDFEATURESETSREQUEST']._serialized_start=49663
+  _globals['_PINNEDFEATURESETSREQUEST']._serialized_end=49728
+  _globals['_PINNEDFEATURESET']._serialized_start=49731
+  _globals['_PINNEDFEATURESET']._serialized_end=49947
+  _globals['_PINNEDFEATURESETSRESPONSE']._serialized_start=49949
+  _globals['_PINNEDFEATURESETSRESPONSE']._serialized_end=50069
+  _globals['_ISFEATURESETPINNEDREQUEST']._serialized_start=50071
+  _globals['_ISFEATURESETPINNEDREQUEST']._serialized_end=50122
+  _globals['_ISFEATURESETPINNEDRESPONSE']._serialized_start=50124
+  _globals['_ISFEATURESETPINNEDRESPONSE']._serialized_end=50168
+  _globals['_CODESNIPPEDIDREQUEST']._serialized_start=50170
+  _globals['_CODESNIPPEDIDREQUEST']._serialized_end=50251
+  _globals['_CODESNIPPEDIDRESPONSE']._serialized_start=50253
+  _globals['_CODESNIPPEDIDRESPONSE']._serialized_end=50297
+  _globals['_ADVANCEDSEARCHOPTION']._serialized_start=50300
+  _globals['_ADVANCEDSEARCHOPTION']._serialized_end=50764
+  _globals['_ADVANCEDSEARCHOPTION_SEARCHOPERATOR']._serialized_start=50520
+  _globals['_ADVANCEDSEARCHOPTION_SEARCHOPERATOR']._serialized_end=50619
+  _globals['_ADVANCEDSEARCHOPTION_SEARCHFIELD']._serialized_start=50622
+  _globals['_ADVANCEDSEARCHOPTION_SEARCHFIELD']._serialized_end=50764
+  _globals['_CORESERVICE']._serialized_start=54685
+  _globals['_CORESERVICE']._serialized_end=85701
 # @@protoc_insertion_point(module_scope)
```

### Comparing `h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/CoreService_pb2_grpc.py` & `h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/CoreService_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,14 +389,19 @@
                 response_deserializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.GetWebConfigResponse.FromString,
                 )
         self.GetApiConfig = channel.unary_unary(
                 '/ai.h2o.featurestore.api.v1.CoreService/GetApiConfig',
                 request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                 response_deserializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.GetApiConfigResponse.FromString,
                 )
+        self.GetH2OGpteConfig = channel.unary_unary(
+                '/ai.h2o.featurestore.api.v1.CoreService/GetH2OGpteConfig',
+                request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+                response_deserializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.GetGpteConfigResponse.FromString,
+                )
         self.AddFeatureSetPermission = channel.unary_unary(
                 '/ai.h2o.featurestore.api.v1.CoreService/AddFeatureSetPermission',
                 request_serializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.FeatureSetPermissionRequest.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.AddProjectPermission = channel.unary_unary(
                 '/ai.h2o.featurestore.api.v1.CoreService/AddProjectPermission',
@@ -544,14 +549,19 @@
                 response_deserializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.JobId.FromString,
                 )
         self.GetMaterializationOnlineJobOutput = channel.unary_unary(
                 '/ai.h2o.featurestore.api.v1.CoreService/GetMaterializationOnlineJobOutput',
                 request_serializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.JobId.SerializeToString,
                 response_deserializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.MaterializationOnlineResponse.FromString,
                 )
+        self.StartOnlineOfflineIngestionJob = channel.unary_unary(
+                '/ai.h2o.featurestore.api.v1.CoreService/StartOnlineOfflineIngestionJob',
+                request_serializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.StartOnlineOfflineIngestionRequest.SerializeToString,
+                response_deserializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.JobId.FromString,
+                )
         self.GetComputeStatisticsJobOutput = channel.unary_unary(
                 '/ai.h2o.featurestore.api.v1.CoreService/GetComputeStatisticsJobOutput',
                 request_serializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.JobId.SerializeToString,
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
         self.GetComputeRecommendationClassifiersJobOutput = channel.unary_unary(
                 '/ai.h2o.featurestore.api.v1.CoreService/GetComputeRecommendationClassifiersJobOutput',
@@ -1335,25 +1345,32 @@
     def Login(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetWebConfig(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Config API
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetApiConfig(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetH2OGpteConfig(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def AddFeatureSetPermission(self, request, context):
         """Permissions API
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -1535,14 +1552,20 @@
 
     def GetMaterializationOnlineJobOutput(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def StartOnlineOfflineIngestionJob(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetComputeStatisticsJobOutput(self, request, context):
         """ComputeStatistics API
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -2334,14 +2357,19 @@
                     response_serializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.GetWebConfigResponse.SerializeToString,
             ),
             'GetApiConfig': grpc.unary_unary_rpc_method_handler(
                     servicer.GetApiConfig,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.GetApiConfigResponse.SerializeToString,
             ),
+            'GetH2OGpteConfig': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetH2OGpteConfig,
+                    request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
+                    response_serializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.GetGpteConfigResponse.SerializeToString,
+            ),
             'AddFeatureSetPermission': grpc.unary_unary_rpc_method_handler(
                     servicer.AddFeatureSetPermission,
                     request_deserializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.FeatureSetPermissionRequest.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'AddProjectPermission': grpc.unary_unary_rpc_method_handler(
                     servicer.AddProjectPermission,
@@ -2489,14 +2517,19 @@
                     response_serializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.JobId.SerializeToString,
             ),
             'GetMaterializationOnlineJobOutput': grpc.unary_unary_rpc_method_handler(
                     servicer.GetMaterializationOnlineJobOutput,
                     request_deserializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.JobId.FromString,
                     response_serializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.MaterializationOnlineResponse.SerializeToString,
             ),
+            'StartOnlineOfflineIngestionJob': grpc.unary_unary_rpc_method_handler(
+                    servicer.StartOnlineOfflineIngestionJob,
+                    request_deserializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.StartOnlineOfflineIngestionRequest.FromString,
+                    response_serializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.JobId.SerializeToString,
+            ),
             'GetComputeStatisticsJobOutput': grpc.unary_unary_rpc_method_handler(
                     servicer.GetComputeStatisticsJobOutput,
                     request_deserializer=ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.JobId.FromString,
                     response_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ),
             'GetComputeRecommendationClassifiersJobOutput': grpc.unary_unary_rpc_method_handler(
                     servicer.GetComputeRecommendationClassifiersJobOutput,
@@ -4115,14 +4148,31 @@
         return grpc.experimental.unary_unary(request, target, '/ai.h2o.featurestore.api.v1.CoreService/GetApiConfig',
             google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
             ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.GetApiConfigResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetH2OGpteConfig(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ai.h2o.featurestore.api.v1.CoreService/GetH2OGpteConfig',
+            google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
+            ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.GetGpteConfigResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def AddFeatureSetPermission(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -4642,14 +4692,31 @@
         return grpc.experimental.unary_unary(request, target, '/ai.h2o.featurestore.api.v1.CoreService/GetMaterializationOnlineJobOutput',
             ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.JobId.SerializeToString,
             ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.MaterializationOnlineResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def StartOnlineOfflineIngestionJob(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ai.h2o.featurestore.api.v1.CoreService/StartOnlineOfflineIngestionJob',
+            ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.StartOnlineOfflineIngestionRequest.SerializeToString,
+            ai_dot_h2o_dot_featurestore_dot_api_dot_v1_dot_CoreService__pb2.JobId.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetComputeStatisticsJobOutput(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/DashboardApi_pb2.py` & `h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/DashboardApi_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ai/h2o/featurestore/api/v1/DashboardApi.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/FeatureSetProtoApi_pb2.py` & `h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/FeatureSetProtoApi_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ai/h2o/featurestore/api/v1/FeatureSetProtoApi.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/FeatureSetSearch_pb2.py` & `h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/FeatureSetSearch_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ai/h2o/featurestore/api/v1/FeatureSetSearch.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/OnlineApi_pb2.py` & `h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/OnlineApi_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ai/h2o/featurestore/api/v1/OnlineApi.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/RecommendationProtoApi_pb2.py` & `h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/RecommendationProtoApi_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ai/h2o/featurestore/api/v1/RecommendationProtoApi.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `h2o-featurestore-1.1.2/ai/h2o/featurestore/api/v1/TimeToLiveApi_pb2.py` & `h2o-featurestore-1.2.0/ai/h2o/featurestore/api/v1/TimeToLiveApi_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ai/h2o/featurestore/api/v1/TimeToLiveApi.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.2
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `h2o-featurestore-1.1.2/featurestore/__init__.py` & `h2o-featurestore-1.2.0/featurestore/__init__.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/client.py` & `h2o-featurestore-1.2.0/featurestore/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     Typical usage example:
 
         config = ClientConfig(wait_for_backend=True, timeout=300)
         client = Client(url=<endpoint_url>, secure=False, root_certificates=None, config=config)
 
     For more details:
-        https://docs.h2o.ai/feature-store/latest-stable/docs/api/client_initialization.html
+        https://docs.h2o.ai/featurestore/api/client_initialization.html
     """
 
     def __init__(
         self, url: str, secure: bool = True, root_certificates: str = None, config: ClientConfig = ClientConfig()
     ):
         self.__init_internal(url.strip(), secure, root_certificates, config)
 
@@ -164,18 +164,18 @@
 
             A job is created with unique id and type ExtractSchema. For example:
 
             Job(id=<job_id>, type=ExtractSchema, done=False, childJobIds=[])
 
         For more details:
             Supported data sources:
-              https://docs.h2o.ai/feature-store/latest-stable/docs/supported_data_sources.html#supported-data-sources
+              https://docs.h2o.ai/featurestore/supported_data_sources.html#supported-data-sources
 
             Passing credentials as parameters: An example
-              https://docs.h2o.ai/feature-store/latest-stable/docs/api/client_credentials.html#passing-credentials-as-a-parameters
+              https://docs.h2o.ai/featurestore/api/client_credentials.html#passing-credentials-as-a-parameters
         """
         request = pb.StartExtractSchemaJobRequest()
         if isinstance(raw_data_location, SparkDataFrame):
             raw_data_location._write_to_storage(self._stub)
             data_source = raw_data_location._get_storage_location()
         else:
             data_source = get_raw_data_location(raw_data_location)
@@ -207,18 +207,18 @@
 
             credentials = S3Credentials(access_key, secret_key, region=None, endpoint=None, role_arn=None)
             source = CSVFile(path, delimiter=",")
             schema = Client(...).extract_schema_from_source(source, credentials)
 
         For more details:
             Supported data sources:
-              https://docs.h2o.ai/feature-store/latest-stable/docs/supported_data_sources.html#supported-data-sources
+              https://docs.h2o.ai/featurestore/supported_data_sources.html#supported-data-sources
 
             Passing credentials as parameters: An example
-              https://docs.h2o.ai/feature-store/latest-stable/docs/api/client_credentials.html#passing-credentials-as-a-parameters
+              https://docs.h2o.ai/featurestore/api/client_credentials.html#passing-credentials-as-a-parameters
         """
         job = self.extract_schema_from_source_async(raw_data_location, credentials)
         return job.wait_for_result()
 
     @interactive_console.record_stats
     def extract_derived_schema(self, feature_sets, transformation) -> Schema:
         """Create a schema from an existing feature set using a selected transformation.
@@ -237,15 +237,15 @@
         Typical usage example:
 
             import featurestore.transformations as t
             spark_pipeline_transformation = t.SparkPipeline("...")
             schema = Client(...).extract_derived_schema([parent_feature_set], spark_pipeline_transformation)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/schema_api.html#create-a-derived-schema-from-a-parent-feature-set-with-applied-transformation
+            https://docs.h2o.ai/featurestore/api/schema_api.html#create-a-derived-schema-from-a-parent-feature-set-with-applied-transformation
         """
         job = self.extract_derived_schema_async(feature_sets, transformation)
         return job.wait_for_result()
 
     def extract_derived_schema_async(self, feature_sets, transformation) -> ExtractSchemaJob:
         """Create a schema extract job.
 
@@ -262,15 +262,15 @@
 
             A job is created with unique id and type ExtractSchema. For example:
 
             Job(id=<job_id>, type=ExtractSchema, done=False, childJobIds=[])
 
         For more details:
             Supported derived transformation:
-              https://docs.h2o.ai/feature-store/latest-stable/docs/supported_derived_transformation.html#supported-derived-transformation
+              https://docs.h2o.ai/featurestore/supported_derived_transformation.html#supported-derived-transformation
         """
         transformation._initialize(self._stub)
         request = pb.StartExtractSchemaJobRequest(
             derived_from=pb.DerivedInformation(
                 feature_set_ids=[pb.VersionedId(id=f.id, major_version=f.major_version) for f in feature_sets],
                 transformation=transformation._to_proto(),
             )
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/access_type.py` & `h2o-featurestore-1.2.0/featurestore/core/access_type.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/acl.py` & `h2o-featurestore-1.2.0/featurestore/core/acl.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         Returns:
             Generator of project permission requests
 
         Typical example:
             my_requests = client.acl.requests.projects.list()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#managing-permission-requests-from-other-users
+            https://docs.h2o.ai/featurestore/api/permissions.html#managing-permission-requests-from-other-users
         """
         request = pb.ListPermissionsPageRequest(filters=[pb.PermissionState.PENDING])
         return (
             PermissionRequest(self._stub, self._rest_stub, entry.permission, entry.project.name)
             for entry in paged_response_to_request(request, self._stub.ListProjectPermissionsPage)
         )
 
@@ -51,15 +51,15 @@
         Returns:
             Generator of manageable project permission requests
 
         Typical example:
             manageable_requests = client.acl.requests.projects.list_manageable()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#managing-permission-requests-from-other-users
+            https://docs.h2o.ai/featurestore/api/permissions.html#managing-permission-requests-from-other-users
         """
         request = pb.ListPermissionsPageRequest(filters=[pb.PermissionState.PENDING])
         return (
             ManageablePermissionRequest(self._stub, self._rest_stub, entry.permission, entry.project.name)
             for entry in paged_response_to_request(request, self._stub.ListManageableProjectPermissionsPage)
         )
 
@@ -75,15 +75,15 @@
         Returns:
             Generator of feature set permission requests
 
         Typical example:
             my_requests = client.acl.requests.feature_sets.list()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#managing-permission-requests-from-other-users
+            https://docs.h2o.ai/featurestore/api/permissions.html#managing-permission-requests-from-other-users
         """
         request = pb.ListPermissionsPageRequest(filters=[pb.PermissionState.PENDING])
         return (
             PermissionRequest(self._stub, self._rest_stub, entry.permission, entry.feature_set.project_name)
             for entry in paged_response_to_request(request, self._stub.ListFeatureSetsPermissionsPage)
         )
 
@@ -93,15 +93,15 @@
         Returns:
             Generator of manageable feature set permission requests
 
         Typical example:
             manageable_requests = client.acl.requests.feature_sets.list_manageable()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#managing-permission-requests-from-other-users
+            https://docs.h2o.ai/featurestore/api/permissions.html#managing-permission-requests-from-other-users
         """
         request = pb.ListPermissionsPageRequest(filters=[pb.PermissionState.PENDING])
         return (
             ManageablePermissionRequest(self._stub, self._rest_stub, entry.permission, entry.feature_set.project_name)
             for entry in paged_response_to_request(request, self._stub.ListManageableFeatureSetsPermissionsPage)
         )
 
@@ -121,15 +121,15 @@
             Generator of project permissions
 
         Typical example:
             filters = [PermissionState.REJECTED]
             my_requests = client.acl.requests.projects.list(filters)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#requesting-permissions-to-a-project
+            https://docs.h2o.ai/featurestore/api/permissions.html#requesting-permissions-to-a-project
         """
         if filters is None:
             filters = [pb.PermissionState.GRANTED]
         request = pb.ListPermissionsPageRequest(filters=filters)
         return (
             Permission(self._stub, self._rest_stub, entry.permission, entry.project.name)
             for entry in paged_response_to_request(request, self._stub.ListProjectPermissionsPage)
@@ -145,15 +145,15 @@
             Generator of manageable project permissions
 
         Typical example:
             filters = [PermissionState.REJECTED]
             manageable_requests = client.acl.requests.projects.list_manageable(filters)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#managing-permission-requests-from-other-users
+            https://docs.h2o.ai/featurestore/api/permissions.html#managing-permission-requests-from-other-users
         """
         if filters is None:
             filters = [pb.PermissionState.GRANTED]
         request = pb.ListPermissionsPageRequest(filters=filters)
         return (
             ManageablePermission(self._stub, self._rest_stub, entry.permission, entry.project.name)
             for entry in paged_response_to_request(request, self._stub.ListManageableProjectPermissionsPage)
@@ -175,15 +175,15 @@
             Generator of feature set permissions
 
         Typical example:
             filters = [PermissionState.REJECTED]
             my_requests = client.acl.requests.feature_sets.list(filters)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#managing-feature-set-permissions
+            https://docs.h2o.ai/featurestore/api/permissions.html#managing-feature-set-permissions
         """
         if filters is None:
             filters = [pb.PermissionState.GRANTED]
         request = pb.ListPermissionsPageRequest(filters=filters)
         return (
             Permission(self._stub, self._rest_stub, entry.permission, entry.feature_set.project_name)
             for entry in paged_response_to_request(request, self._stub.ListFeatureSetsPermissionsPage)
@@ -199,15 +199,15 @@
             Generator of manageable feature set permissions
 
         Typical example:
             filters = [PermissionState.REJECTED]
             manageable_requests = client.acl.requests.feature_sets.list_manageable(filters)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#managing-feature-set-permissions
+            https://docs.h2o.ai/featurestore/api/permissions.html#managing-feature-set-permissions
         """
         if filters is None:
             filters = [pb.PermissionState.GRANTED]
         request = pb.ListPermissionsPageRequest(filters=filters)
         return (
             ManageablePermission(self._stub, self._rest_stub, entry.permission, entry.feature_set.project_name)
             for entry in paged_response_to_request(request, self._stub.ListManageableFeatureSetsPermissionsPage)
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/auth.py` & `h2o-featurestore-1.2.0/featurestore/core/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         This will obtain an access token from the external environment to use for authentication.
 
         Args:
             method: (Callable) A method that returns a token from the external environment.
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/authentication.html#authentication-via-access-token-from-external-environment
+            https://docs.h2o.ai/featurestore/api/authentication.html#authentication-via-access-token-from-external-environment
         """
         self._get_access_token_external = method
 
     def logout(self):
         """Logout the current user session."""
         is_success, token_or_error = self._obtain_token()
         if is_success:
@@ -80,15 +80,15 @@
             open_browser: (bool) If True, opens the URL in the browser. Defaults to True.
 
         Raises:
             AuthException: Incorrect response or if user doesn't log in via browser,
               logging session will be expired.
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/authentication.html#authentication-via-refresh-token-from-identity-provider
+            https://docs.h2o.ai/featurestore/api/authentication.html#authentication-via-refresh-token-from-identity-provider
         """
         try:
             sys.tracebacklimit = None
             for response in self._stub.Login(Empty()):
                 if response.HasField("login_url"):
                     if open_browser:
                         try:
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/browser.py` & `h2o-featurestore-1.2.0/featurestore/core/browser.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/collections/artifacts.py` & `h2o-featurestore-1.2.0/featurestore/core/collections/artifacts.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/collections/classifiers.py` & `h2o-featurestore-1.2.0/featurestore/core/collections/classifiers.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             client.classifiers.create("classifierName")
             client.classifiers.create(RegexClassifier("classifierName", "test", 10))
 
         Raises:
             ValueError: Parameter classifier should be string or object of Classifier class.
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/recommendation_api.html#creating-a-new-classifier
+            https://docs.h2o.ai/featurestore/api/recommendation_api.html#creating-a-new-classifier
         """
         if isinstance(classifier, str):
             classifier_to_send = EmptyClassifier(classifier)
         elif isinstance(classifier, Classifier):
             classifier_to_send = classifier
         else:
             raise ValueError("Parameter classifier should be string or object of Classifier class")
@@ -185,15 +185,15 @@
             classifier: (Classifier) Object represents Classifier.
               EmptyClassifier | RegexClassifier | SampleClassifier
 
         Typical example:
             client.classifiers.update(RegexClassifier("classifierName", "test", 10))
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/recommendation_api.html#updating-an-existing-classifier
+            https://docs.h2o.ai/featurestore/api/recommendation_api.html#updating-an-existing-classifier
         """
         request = pb.UpdateRecommendationClassifierRequest(classifier=classifier._to_proto())
         self._stub.UpdateRecommendationClassifier(request)
 
     def delete(self, name: str):
         """Delete an existing classifier.
 
@@ -202,14 +202,14 @@
         Args:
             name: (str) A name of an existing classifier.
 
         Typical example:
             client.classifiers.delete("classifierName")
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/recommendation_api.html#deleting-an-existing-classifier
+            https://docs.h2o.ai/featurestore/api/recommendation_api.html#deleting-an-existing-classifier
         """
         request = pb.DeleteRecommendationClassifierRequest(classifier_name=name)
         self._stub.DeleteRecommendationClassifier(request)
 
     def __repr__(self):
         return "Recommendation classifiers"
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/collections/feature_set_reviews.py` & `h2o-featurestore-1.2.0/featurestore/core/collections/feature_set_reviews.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             Generator of feature set review requests
 
         Typical example:
             filters = [ReviewStatuses.IN_PROGRESS]
             reviews = client.feature_set_reviews.manageable_requests()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_review_api#manage-review-requests-from-other-users
+            https://docs.h2o.ai/featurestore/api/feature_set_review_api#manage-review-requests-from-other-users
         """
         request = pb.ListFeatureSetsToReviewRequest(filters=filters, project_id=self._project_id)
         return (
             FeatureSetReviewRequest(self._stub, self._rest_stub, entry)
             for entry in self.__paged_response_to_request(request, self._stub.ListFeatureSetsToReview)
         )
 
@@ -46,15 +46,15 @@
             Generator of feature set user review requests
 
         Typical example:
             filters = [ReviewStatuses.IN_PROGRESS]
             reviews = client.feature_set_reviews.my_requests(filters)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_review_api#manage-own-feature-sets-in-review
+            https://docs.h2o.ai/featurestore/api/feature_set_review_api#manage-own-feature-sets-in-review
         """
         request = pb.ListFeatureSetReviewsPageRequest(filters=filters, project_id=self._project_id)
         return (
             FeatureSetUserReview(self._stub, self._rest_stub, entry)
             for entry in self.__paged_response_to_request(request, self._stub.ListFeatureSetsReviewsPage)
         )
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/collections/feature_sets.py` & `h2o-featurestore-1.2.0/featurestore/core/collections/feature_sets.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
               time_travel_column=None, time_travel_column_format="yyyy-MM-dd HH:mm:ss", secret=False,
               partition_by=None, time_travel_column_as_partition=False)
 
         Raises:
             ValueError: Parameter schema should be of type Schema.
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#registering-a-feature-set
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#registering-a-feature-set
         """
         if not isinstance(schema, Schema):
             raise ValueError("Parameter `schema` should be of type `featurestore.core.schema.Schema`")
         request = pb.RegisterFeatureSetRequest()
         request.schema.extend(schema._to_proto_schema())
         request.project.CopyFrom(self._project)
         if schema.derivation is not None:
@@ -100,15 +100,15 @@
         Typical example:
             fs = project.feature_sets.get("feature_set_name", version=None)
 
         Raises:
             Exception: Version parameter must be in a format "major.minor".
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#obtaining-a-feature-set
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#obtaining-a-feature-set
         """
         request = pb.GetFeatureSetRequest()
         request.project_id = self._project.id
         request.feature_set_name = feature_set_name
         if version is not None:
             if not re.search(r"^\d+\.\d+$", str(version)):
                 raise Exception('Version parameter must be in a format "major.minor".')
@@ -126,15 +126,15 @@
         Returns:
             FeatureSet: An existing feature set.
 
         Typical example:
             fs = project.feature_sets.get_major_version("feature_set_name", 2)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#obtaining-a-feature-set
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#obtaining-a-feature-set
         """
         request = pb.GetLastMinorFeatureSetForMajorInProjectRequest()
         request.project_id = self._project.id
         request.feature_set_name = feature_set_name
         request.feature_set_major_version = major_version
         response = self._stub.GetLastMinorFeatureSetForMajorInProject(request)
         return FeatureSet(self._stub, self._rest_stub, response.feature_set)
@@ -151,15 +151,15 @@
             Iterable[FeatureSet]: A generator iterator object consists of feature sets.
 
         Typical example:
             advanced_search_options = [AdvancedSearchOption]
             project.feature_sets.list(advanced_search_options)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#listing-feature-sets-within-a-project
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#listing-feature-sets-within-a-project
         """
         request = pb.FeatureSetSearchRequest()
         request.project_ids.extend([self._project.id])
         if query:
             request.query = query
         if advanced_search_options:
             request.options.extend([ad._to_proto() for ad in advanced_search_options])
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/collections/feature_views.py` & `h2o-featurestore-1.2.0/featurestore/core/collections/feature_views.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         Returns:
             FeatureView: A feature view with relevant metadata.
 
         Typical example:
             feature_view = project.feature_views.create(name = "test", description="", query)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_view_api.html#creating-a-feature-view
+            https://docs.h2o.ai/featurestore/api/feature_view_api.html#creating-a-feature-view
         """
         request = pb.CreateFeatureViewRequest(
             name=name,
             description=description,
             project_id=self._project.id,
             query=query._to_proto(),
         )
@@ -48,15 +48,15 @@
         Returns:
             FeatureView: A feature view with relevant metadata.
 
         Typical example:
             feature_view = project.feature_views.get("feature_view_name", version=None)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_view_api.html#obtaining-a-feature-view
+            https://docs.h2o.ai/featurestore/api/feature_view_api.html#obtaining-a-feature-view
         """
         request = pb.GetFeatureViewRequest(project_id=self._project.id, name=name, version=(version or 0))
         resource = self._stub.GetFeatureView(request)
         return FeatureView(self._stub, self._rest_stub, resource.feature_view)
 
     def list(self):
         """Return a collection of feature views within a project.
@@ -64,12 +64,12 @@
         Returns:
             list[FeatureView]: A list of existing feature views.
 
         Typical example:
             project.feature_views.list()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_view_api.html#listing-feature-views-within-a-project
+            https://docs.h2o.ai/featurestore/api/feature_view_api.html#listing-feature-views-within-a-project
         """
         request = pb.ListFeatureViewsRequest(project_id=self._project.id)
         response = self._stub.ListFeatureViews(request)
         return [FeatureView(self._stub, self._rest_stub, feature_view) for feature_view in response.feature_views]
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/collections/ingest_history.py` & `h2o-featurestore-1.2.0/featurestore/core/collections/ingest_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             list[Ingest]: A collection of ingestion.
 
         Typical example:
             history = my_feature_set.ingest_history()
             history.list()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/ingest_history_api.html#getting-the-ingestion-history
+            https://docs.h2o.ai/featurestore/api/ingest_history_api.html#getting-the-ingestion-history
         """
         return [Ingest(self._stub, self._feature_set, ingest) for ingest in self._ingest_history]
 
     def refresh(self):
         """Refresh ingest history object with the latest ingestion (if there are any).
 
         Typical example:
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/collections/jobs.py` & `h2o-featurestore-1.2.0/featurestore/core/collections/jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             Job(id=test456, type=CreateMLDataset, done=True, childJobIds=[])]
 
         Typical example:
             client.jobs.list()
             client.jobs.list(active=False, job_type=INGEST)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/jobs_api.html#listing-jobs
+            https://docs.h2o.ai/featurestore/api/jobs_api.html#listing-jobs
         """
         request = pb.ListJobsRequest(active=active, job_type=job_type)
         resp = self._stub.ListJobs(request)
         return [Jobs._create_job(self._stub, self._rest_stub, job_proto) for job_proto in resp.jobs]
 
     def get(self, job_id: str) -> BaseJob:
         """Obtain an existing job.
@@ -87,15 +87,15 @@
 
             Job(id=test123, type=ExtractSchema, done=True, childJobIds=[])
 
         Typical example:
             job = client.jobs.get("job_id")
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/jobs_api.html#getting-a-job
+            https://docs.h2o.ai/featurestore/api/jobs_api.html#getting-a-job
         """
         request = pb.JobId(job_id=job_id)
         job_proto = self._stub.GetJob(request)
         return Jobs._create_job(self._stub, self._rest_stub, job_proto)
 
     def __repr__(self):
         return "This class wraps together methods working with jobs"
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/collections/ml_datasets.py` & `h2o-featurestore-1.2.0/featurestore/core/collections/ml_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         Returns:
             MLDataset: Machine Learning Dataset
 
         Typical example:
             ml_dataset = my_feature_view.ml_datasets.create("name", start_date_time=None, end_date_time=None)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_view_api.html#creating-a-mldataset
+            https://docs.h2o.ai/featurestore/api/feature_view_api.html#creating-a-mldataset
         """
         job, ml_dataset = self.create_async(name, description, start_date_time, end_date_time)
         return job.wait_for_result()
 
     def create_async(
         self,
         name: str,
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/collections/pats.py` & `h2o-featurestore-1.2.0/featurestore/core/collections/pats.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
               expiry_date="<dd/MM/yyyy>", timezone=None)
 
         Raises:
             Exception: Invalid timezone.
             ValueError: Expiry date must be in the format: dd/MM/yyyy.
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/authentication.html#authentication-via-personal-access-tokens-pats
+            https://docs.h2o.ai/featurestore/api/authentication.html#authentication-via-personal-access-tokens-pats
         """
         request = pb.GenerateTokenRequest()
         request.name = name
         request.description = description
         if expiry_date:
             try:
                 if timezone:
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/collections/projects.py` & `h2o-featurestore-1.2.0/featurestore/core/collections/projects.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         Returns:
             Generator of all projects
 
         Typical example:
             client.projects.list()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/projects_api.html#listing-projects
+            https://docs.h2o.ai/featurestore/api/projects_api.html#listing-projects
         """
         request = pb.ListProjectsPageRequest()
         while request:
             response = self._stub.ListProjectsPage(request)
             if response.next_page_token:
                 request = pb.ListProjectsPageRequest()
                 request.page_token = response.next_page_token
@@ -47,15 +47,15 @@
         Returns:
             Iterator[FeatureSet]: An iterator which obtains the feature sets lazily.
 
         Typical example:
             client.projects.list_feature_sets(["project_name_A", "project_name_B"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/projects_api.html#listing-feature-sets-across-multiple-projects
+            https://docs.h2o.ai/featurestore/api/projects_api.html#listing-feature-sets-across-multiple-projects
         """
         request = pb.ListFeatureSetsPageRequest()
         request.project_names.extend(project_names)
         while request:
             response = self._stub.ListFeatureSetsPage(request)
             if response.next_page_token:
                 request.page_token = response.next_page_token
@@ -73,25 +73,26 @@
     ) -> Project:
         """Create a project.
 
         Args:
             project_name: (str) A project name.
             description: (str) A description about the project.
             secret: (bool) If True, project is visible only to its owner.
-            locked: (bool) If True, only users with consumer permission can list and get feature sets from this project.
+            locked: (bool) If True, only users with viewer permission can list feature sets within this project.
+                           If False, every user can list feature sets within this project.
 
         Returns:
             Project: A new project with specified attributes.
 
         Typical example:
             project = client.projects.create(project_name="project", description="description",
               secret=False, locked=None)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/projects_api.html#create-a-project
+            https://docs.h2o.ai/featurestore/api/projects_api.html#create-a-project
         """
         if locked is None and self._default_lock_value is None:
             self._default_lock_value = self._stub.GetProjectsDefault(Empty()).locked
         if locked is None:
             locked_value = self._default_lock_value
         else:
             locked_value = locked
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/collections/scheduled_tasks.py` & `h2o-featurestore-1.2.0/featurestore/core/collections/scheduled_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         Returns:
             Generator of scheduled tasks
 
         Typical example:
             fs.schedule.tasks()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_schedule.html#to-list-scheduled-tasks
+            https://docs.h2o.ai/featurestore/api/feature_set_schedule.html#to-list-scheduled-tasks
         """
         request = pb.ListScheduledTasksRequest()
         request.feature_set_id = self._feature_set.id
         while request:
             response = self._stub.ListScheduledTasks(request)
             if response.next_page_token:
                 request.page_token = response.next_page_token
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/collections/transformation_functions.py` & `h2o-featurestore-1.2.0/featurestore/core/collections/transformation_functions.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/commons/case_insensitive_dict.py` & `h2o-featurestore-1.2.0/featurestore/core/commons/case_insensitive_dict.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/commons/spark_utils.py` & `h2o-featurestore-1.2.0/featurestore/core/commons/spark_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 class SparkUtils:
     @staticmethod
     def configure_user_spark(spark):
+        spark.conf.set("fs.gs.impl", "com.google.cloud.hadoop.fs.gcs.GoogleHadoopFileSystem")
         spark.conf.set("fs.wasbs.impl.disable.cache", "true")
+        spark.conf.set("fs.gs.impl.disable.cache", "true")
         spark.conf.set("fs.wasb.impl.disable.cache", "true")
         spark.conf.set("fs.abfss.impl.disable.cache", "true")
         spark.conf.set("fs.abfs.impl.disable.cache", "true")
         spark.conf.set("fs.s3a.impl.disable.cache", "true")
         spark.conf.set("fs.s3n.impl.disable.cache", "true")
         spark.conf.set("fs.s3.impl.disable.cache", "true")
         spark.conf.set("spark.sql.parquet.datetimeRebaseModeInWrite", "CORRECTED")
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/config.py` & `h2o-featurestore-1.2.0/featurestore/core/config.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/credentials.py` & `h2o-featurestore-1.2.0/featurestore/core/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,16 @@
     def get_credentials_based_on_cloud(request, url_path, credentials):
         if url_path.lower().startswith("s3"):
             CredentialsHelper.set_s3_credentials(request, credentials)
         elif url_path.lower().startswith("wasb") or url_path.lower().startswith("abfs"):
             CredentialsHelper.set_azure_credentials(request, url_path, credentials)
         elif url_path.lower().startswith("http"):
             pass
+        elif url_path.lower().startswith("drive:"):
+            CredentialsHelper.set_drive_credentials(request, url_path, credentials)
         else:
             raise Exception("Unsupported external data spec!")
 
     @staticmethod
     def set_azure_credentials(request, url_path, credentials):
         sas_container = urlparse(url_path).netloc.split("@")[0]
         if credentials is None:
@@ -244,7 +246,14 @@
         request.cred.mongo_db.user = credentials.user
         request.cred.mongo_db.password = credentials.password
 
     @staticmethod
     def read_private_key_pem_file(pem_file):
         with open(pem_file, "rb") as key:
             return key.read()
+
+    @staticmethod
+    def set_drive_credentials(request, url_path, credentials):
+        if credentials is not None:
+            logging.warning("Credentials were ignored, they are not needed for accessing H2O Drive")
+
+        request.cred.drive.SetInParent()
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/dashboard.py` & `h2o-featurestore-1.2.0/featurestore/core/dashboard.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/data_source_wrappers.py` & `h2o-featurestore-1.2.0/featurestore/core/data_source_wrappers.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/data_types.py` & `h2o-featurestore-1.2.0/featurestore/core/data_types.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/advanced_search_option.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/advanced_search_option.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/artifact.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/artifact.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/backfill_job.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/backfill_job.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/backfill_option.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/backfill_option.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/base_job.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/base_job.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/component_versions.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/component_versions.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/extract_schema_job.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/extract_schema_job.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/feature.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/feature.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/feature_ref.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/feature_ref.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/feature_set.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/feature_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -291,15 +291,14 @@
 
     @property
     def flow(self) -> FeatureSetFlow:
         return FeatureSetFlow[self._feature_set.flow]
 
     @flow.setter
     def flow(self, value: FeatureSetFlow):
-
         update_request = pb.UpdateFeatureSetRequest(
             feature_set_id=self._feature_set.id,
             feature_set_version=self._feature_set.version,
             flow=value.name,
             fields_to_update=[pb.FEATURE_SET_FLOW],
         )
         self._feature_set = self._stub.UpdateFeatureSet(update_request).updated_feature_set
@@ -461,15 +460,15 @@
             new_fs = fs.create_new_version(affected_features=["xyz"], reason="Computation of feature XYZ changed")
             new_fs = fs.create_new_version(schema=schema, reason="some message", backfill_options=backfill)
 
         Raises:
             ValueError: At least one of schema, affected_features or primary_key must be defined.
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_new_version.html
+            https://docs.h2o.ai/featurestore/api/feature_set_new_version.html
         """
         request = pb.CreateNewFeatureSetVersionRequest()
         request.feature_set_id = self._feature_set.id
         request.feature_set_version = self._feature_set.version
         request.reason = reason
         if schema:
             request.schema.extend(schema._to_proto_schema())
@@ -542,15 +541,15 @@
         Returns:
             FeatureSet: An existing feature set with the latest information.
 
         Typical example:
             fs.add_owners(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#feature-set-permissions-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#feature-set-permissions-api
         """
         return self._add_permissions(user_emails, pb.PermissionType.Owner)
 
     def add_editors(self, user_emails):
         """Add additional editor/editors to a feature set.
 
         Args:
@@ -559,15 +558,15 @@
         Returns:
             FeatureSet: An existing feature set with the latest information.
 
         Typical example:
             fs.add_editors(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#feature-set-permissions-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#feature-set-permissions-api
         """
         return self._add_permissions(user_emails, pb.PermissionType.Editor)
 
     def add_consumers(self, user_emails):
         """Add additional consumer/consumers to a feature set.
 
         Args:
@@ -576,15 +575,15 @@
         Returns:
             FeatureSet: An existing feature set with the latest information.
 
         Typical example:
             fs.add_consumers(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#feature-set-permissions-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#feature-set-permissions-api
         """
         return self._add_permissions(user_emails, pb.PermissionType.Consumer)
 
     def add_sensitive_consumers(self, user_emails):
         """Add additional sensitive consumer/consumers to a feature set.
 
         Args:
@@ -593,15 +592,15 @@
         Returns:
             FeatureSet: An existing feature set with the latest information.
 
         Typical example:
             fs.add_sensitive_consumers(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#feature-set-permissions-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#feature-set-permissions-api
         """
         return self._add_permissions(user_emails, pb.PermissionType.SensitiveConsumer)
 
     def add_viewers(self, user_emails):
         """Add additional viewer/viewers to a feature set.
 
         Args:
@@ -610,15 +609,15 @@
         Returns:
             FeatureSet: An existing feature set with the latest information.
 
         Typical example:
             fs.add_viewers(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#feature-set-permissions-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#feature-set-permissions-api
         """
         return self._add_permissions(user_emails, pb.PermissionType.Viewer)
 
     def remove_owners(self, user_emails):
         """Removes owner/owners from a feature set.
 
         Args:
@@ -627,15 +626,15 @@
         Returns:
             FeatureSet: An existing feature set with the latest information.
 
         Typical example:
             fs.remove_owners(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#feature-set-permissions-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#feature-set-permissions-api
         """
         return self._remove_permissions(user_emails, pb.PermissionType.Owner)
 
     def remove_editors(self, user_emails):
         """Remove editor/editors from a feature set.
 
         Args:
@@ -644,15 +643,15 @@
         Returns:
             FeatureSet: An existing feature set with the latest information.
 
         Typical example:
             fs.remove_editors(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#feature-set-permissions-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#feature-set-permissions-api
         """
         return self._remove_permissions(user_emails, pb.PermissionType.Editor)
 
     def remove_consumers(self, user_emails):
         """Remove consumer/consumers from a feature set.
 
         Args:
@@ -661,15 +660,15 @@
         Returns:
             FeatureSet: An existing feature set with the latest information.
 
         Typical example:
             fs.remove_consumers(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#feature-set-permissions-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#feature-set-permissions-api
         """
         return self._remove_permissions(user_emails, pb.PermissionType.Consumer)
 
     def remove_sensitive_consumers(self, user_emails):
         """Remove sensitive consumer/consumers from a feature set.
 
         Args:
@@ -678,15 +677,15 @@
         Returns:
             FeatureSet: An existing feature set with the latest information.
 
         Typical example:
             fs.remove_sensitive_consumers(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#feature-set-permissions-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#feature-set-permissions-api
         """
         return self._remove_permissions(user_emails, pb.PermissionType.SensitiveConsumer)
 
     def remove_viewers(self, user_emails):
         """Remove viewer/viewers from a feature set.
 
         Args:
@@ -695,15 +694,15 @@
         Returns:
             FeatureSet: An existing feature set with the latest information.
 
         Typical example:
             fs.remove_viewers(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#feature-set-permissions-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#feature-set-permissions-api
         """
         return self._remove_permissions(user_emails, pb.PermissionType.Viewer)
 
     def get_active_jobs(self, job_type=pb.JobType.Unknown):
         """List running jobs belonging to a feature set.
 
         This returns a list of jobs that are currently processing for a specific feature set.
@@ -723,15 +722,15 @@
             Job(id=test456, type=Backfill, done=False, childJobIds=[])]
 
         Typical example:
             fs.get_active_jobs()
             fs.get_active_jobs(job_type=INGEST)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#feature-set-jobs-api
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#feature-set-jobs-api
         """
         return self._get_jobs(True, job_type)
 
     def _get_jobs(self, active, job_type=pb.JobType.Unknown):
         from ..collections.jobs import Jobs  # Lazy import to avoid circular reference
 
         request = pb.ListJobsRequest(active=active)
@@ -767,15 +766,15 @@
         Returns:
             str: A permission id.
 
         Typical example:
             my_request_id = fs.request_access(AccessType.CONSUMER, "Preparing the best model")
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#managing-feature-set-permissions
+            https://docs.h2o.ai/featurestore/api/permissions.html#managing-feature-set-permissions
         """
         request = pb.SubmitPendingPermissionRequest()
         request.resource_id = self._feature_set.id
         request.permission = AccessType.to_proto_permission(access_type)
         request.reason = reason
         response = self._stub.SubmitPendingFeatureSetPermission(request)
         return response.permission_id
@@ -848,15 +847,15 @@
               SnowflakeCredentials | TeradataCredentials | PostgresCredentials | MongoDbCredentials)
               To access the provided data source. Default is None.
 
         Typical example:
             fs.ingest(source, credentials=credentials)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#offline-ingestion
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#offline-ingestion
         """
         job = self.ingest_async(source, credentials)
         result = job.wait_for_result()
         self._feature_set = self._stub.GetFeatureSetById(
             pb.FeatureSetRequestId(
                 feature_set_id=result._get_feature_set_id(), feature_set_version=result._get_feature_set_version()
             )
@@ -889,15 +888,15 @@
 
         This pushes existing data from offline Feature store into online.
 
         Typical example:
             feature_set.materialize_online()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#offline-to-online-api
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#offline-to-online-api
         """
         job = self.materialize_online_async()
         return job.wait_for_result()
 
     def ingest_online(self, rows):
         """Ingest data into the online Feature Store.
 
@@ -907,15 +906,15 @@
         Typical example:
             feature_set.ingest_online('{"id": 1, "label": "Carl"}')
 
         Raises:
             Exception: Manual ingest online is not allowed on derived feature set.
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#online-ingestion
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#online-ingestion
         """
         if self.is_derived():
             raise Exception("Manual ingest online is not allowed on derived feature set")
 
         if isinstance(rows, list):
             row_list = rows
         else:
@@ -958,15 +957,15 @@
 
             {'id': '01', 'department': 'Engineering', 'name': 'Test'}
 
         Typical example:
             json = feature_set.retrieve_online(key)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#retrieving-from-online
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#retrieving-from-online
         """
         if self._online_retrieval_token is None or not self._online_retrieval_token.is_valid_for(
             self.id, self.major_version
         ):
             request = OnlineApi.OnlineRetrieveTokenRequest(feature_set_id=self.id, feature_set_version=self.version)
 
             response: OnlineApi.OnlineRetrieveTokenResponse = self._stub.GenerateOnlineRetrievalToken(request)
@@ -1003,18 +1002,60 @@
         Returns:
             RetrieveHolder: Returns a link as output for reference.
 
         Typical example:
             ref = fs.retrieve(start_date_time="2023-01-01 00:00:00", end_date_time="2023-01-02 00:00:00")
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#retrieving-api
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#retrieving-api
         """
         return RetrieveHolder(self._stub, self._feature_set, start_date_time, end_date_time, "")
 
+    def start_online_offline_ingestion_async(self):
+        """Create a job for feature set online to offline ingestion.
+
+        Returns:
+            IngestionJob: A job for online ingestion in case there is a new online data.
+            It returns an error if there is nothing new to ingest from online.
+
+            A job is created with a unique id and type Ingestion. For example:
+
+            Job(id=<job_id>, type=Ingestion, done=False, childJobIds=[])
+
+        Typical example:
+            job = feature_set.start_online_offline_ingestion_async()
+        """
+        if self.is_derived():
+            raise Exception("Online to offline ingest is not allowed on derived feature set")
+
+        request = pb.StartOnlineOfflineIngestionRequest()
+        request.feature_set_id = self._feature_set.id
+        request.feature_set_version = self._feature_set.version
+        job_id = self._stub.StartOnlineOfflineIngestionJob(request)
+        return IngestJob(self._stub, job_id)
+
+    @interactive_console.record_stats
+    def start_online_offline_ingestion(self):
+        """Perform a feature set ingestion from online to offline store.
+
+        This pushes new existing data from online Feature store into offline.
+
+        Returns:
+            A finished IngestionJob in case there was a new online data.
+            It returns None if there was nothing new to ingest from online.
+
+        Typical example:
+            feature_set.online_offline_ingestion()
+
+        For more details:
+            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#offline-to-online-api
+        """
+        job = self.start_online_offline_ingestion_async()
+        return job.wait_for_result()
+
     def list_versions(self):
         """List all versions of a feature set.
 
         This shows all versions of a feature set (the current and previous ones).
 
         Returns:
             list[VersionDescription]: A list of versions and its details.
@@ -1047,15 +1088,15 @@
         Typical example:
             fs_different_version = feature_set.get(version)
 
         Raises:
             Exception: Version parameter must be in a format "major.minor".
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#obtaining-a-feature-set
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#obtaining-a-feature-set
         """
         request = pb.GetFeatureSetRequest()
         request.project_id = self._feature_set.project_id
         request.feature_set_name = self._feature_set.feature_set_name
         if not re.search(r"^\d+\.\d+$", str(version)):
             raise Exception('Version parameter must be in a format "major.minor".')
         request.version = str(version)
@@ -1113,29 +1154,29 @@
         Returns:
             IngestHistory: An object of IngestHistory class.
 
         Typical example:
             history = my_feature_set.ingest_history()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/ingest_history_api.html#getting-the-ingestion-history
+            https://docs.h2o.ai/featurestore/api/ingest_history_api.html#getting-the-ingestion-history
         """
         return IngestHistory(self._stub, self._feature_set)
 
     def get_recommendations(self):
         """Get feature set recommendations.
 
         Returns:
             list[Recommendation]: A list of recommendations.
 
         Typical example:
             fs.get_recommendations()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#getting-recommendations
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#getting-recommendations
         """
         request = pb.GetRecommendationRequest()
         request.feature_set_id = self._feature_set.id
         response = self._stub.GetRecommendations(request)
         return [Recommendation(self._stub, self._rest_stub, self, item) for item in response.matches]
 
     def schedule_ingest(
@@ -1163,15 +1204,15 @@
         Typical example:
             fs.schedule_ingest("task_name", source, schedule = "0 2 * * *", description = "", credentials = None)
 
         Raises:
             Exception: Scheduling Ingest with SparkDataFrame is not supported.
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_schedule.html#schedule-a-new-task
+            https://docs.h2o.ai/featurestore/api/feature_set_schedule.html#schedule-a-new-task
         """
         from ..data_source_wrappers import get_raw_data_location
 
         if isinstance(source, SparkDataFrame):
             raise Exception("Scheduling Ingest with SparkDataFrame is not supported.")
         else:
             data_source = get_raw_data_location(source)
@@ -1347,15 +1388,15 @@
             StorageOptimizationResponse object containing metrics of the performed optimization.
 
         Typical example:
             fs.optimize_storage()
             fs.optimize_storage(ZOrderByOptimization(["name"]))
 
          For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html
         """
         job = self.optimize_storage_async(optimization)
         return job.wait_for_result()
 
     def optimize_storage_async(self, optimization=None):
         """Create a job for feature set data storage optimization.
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/feature_set_popularity.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/feature_set_popularity.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/feature_set_review.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/feature_set_review.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,30 +54,30 @@
         Args:
         reason: (str) A reason for review request approval.
 
         Typical example:
         review_request.approve("it will be fun")
 
         For more details:
-        https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_review_api#manage-review-requests-from-other-users
+        https://docs.h2o.ai/featurestore/api/feature_set_review_api#manage-review-requests-from-other-users
         """
         request = pb.ApproveReviewRequest(review_id=self._review.review_id, reason=reason)
         self._stub.ApproveReview(request)
 
     def reject(self, reason):
         """Reject a review request.
 
         Args:
         reason: (str) A reason for review request rejection.
 
         Typical example:
         review_request.reject("it's not ready yet")
 
         For more details:
-        https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_review_api#manage-review-requests-from-other-users
+        https://docs.h2o.ai/featurestore/api/feature_set_review_api#manage-review-requests-from-other-users
         """
         request = pb.RejectReviewRequest(review_id=self._review.review_id, reason=reason)
         self._stub.RejectReview(request)
 
     def get_feature_set(self) -> FeatureSet:
         """Get a feature set to review.
 
@@ -132,15 +132,15 @@
         Returns:
             A corresponding feature set.
 
         Typical example:
             review_request.get_feature_set()
 
         For more details:
-        https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_review_api#manage-own-feature-sets-in-review
+        https://docs.h2o.ai/featurestore/api/feature_set_review_api#manage-own-feature-sets-in-review
         """
         request = pb.GetFeatureSetInReviewRequest(review_id=self._review.review_id)
         response = self._stub.GetFeatureSetInReview(request)
         return FeatureSet(self._stub, self._rest_stub, response.feature_set)
 
     def get_preview(self):
         """Preview the data of feature set in review.
@@ -150,15 +150,15 @@
         Returns:
             list[dict]: A list of dictionary which contains JSON rows.
 
         Typical example:
             review_request.get_preview()
 
         For more details:
-        https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_review_api#manage-own-feature-sets-in-review
+        https://docs.h2o.ai/featurestore/api/feature_set_review_api#manage-own-feature-sets-in-review
         """
         request = pb.GetFeatureSetPreviewInReviewRequest(
             review_id=self._review.review_id,
         )
         response = self._stub.GetFeatureSetPreviewInReview(request)
         if response.preview_url:
             json_response = Utils.fetch_preview_as_json_array(response.preview_url)
@@ -171,11 +171,11 @@
 
         Review must be in status IN_PROGRESS or REJECTED.
 
         Typical example:
             review_request.delete()
 
         For more details:
-        https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_review_api#manage-own-feature-sets-in-review
+        https://docs.h2o.ai/featurestore/api/feature_set_review_api#manage-own-feature-sets-in-review
         """
         request = pb.DeleteRejectedFeatureSetRequest(review_id=self._review.review_id)
         self._stub.DeleteFeatureSetVersionInReview(request)
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/feature_set_schema.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/feature_set_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         Returns:
             bool: A boolean describes whether compatible or not.
 
         Typical example:
             fs.schema.is_compatible_with(new_schema, compare_data_types=True)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#checking-schema-compatibility
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#checking-schema-compatibility
         """
         request = pb.FeatureSetSchemaCompatibilityRequest()
         request.original_schema.extend(self.get()._to_proto_schema())
         request.new_schema.extend(new_schema._to_proto_schema())
         request.compare_data_types = compare_data_types
         response = self._stub.IsFeatureSetSchemaCompatible(request)
         return response.is_compatible
@@ -60,15 +60,15 @@
         Returns:
             Schema: A new schema after patches.
 
         Typical example:
             fs.schema.patch_from(new_schema, compare_data_types=True)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#patching-new-schema
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#patching-new-schema
         """
         request = pb.FeatureSetSchemaPatchRequest()
         request.original_schema.extend(self.get()._to_proto_schema())
         request.new_schema.extend(new_schema._to_proto_schema())
         request.compare_data_types = compare_data_types
         response = self._stub.FeatureSetSchemaPatch(request)
         return Schema(self._create_schema_from_proto(response.schema), True)
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/feature_view.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/feature_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         Returns:
             FeatureView: A feature view with a new version.
 
         Typical example:
             fv.create_new_version(query)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_new_version.html
+            https://docs.h2o.ai/featurestore/api/feature_set_new_version.html
         """
         request = pb.CreateFeatureViewNewVersionRequest(
             feature_view_id=self.id,
             feature_view_version=self.version,
             query=new_query._to_proto(),
         )
         response: pb.FeatureViewResponse = self._stub.CreateFeatureViewNewVersion(request)
@@ -100,15 +100,15 @@
         Returns:
             str: A directory path where the files are downloaded.
 
         Typical usage example:
             dir = my_feature_view.download(start_at=None, end_at=None)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_view_api.html#downloading-the-files-from-feature-store
+            https://docs.h2o.ai/featurestore/api/feature_view_api.html#downloading-the-files-from-feature-store
         """
         request = pb.RetrieveFeatureViewAsAsLinksRequest(
             feature_view_id=self.id,
             feature_view_version=self.version,
             start_at=Utils.date_time_to_proto_timestamp(start_at),
             end_at=Utils.date_time_to_proto_timestamp(end_at),
         )
@@ -141,15 +141,15 @@
         Returns:
             DataFrame: Represents a spark data frame.
 
         Typical usage example:
             data_frame = my_feature_view.as_spark_frame(spark_session, start_at=None, end_at=None)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_view_api.html#obtaining-data-as-a-spark-frame
+            https://docs.h2o.ai/featurestore/api/feature_view_api.html#obtaining-data-as-a-spark-frame
         """
         from ..commons.spark_utils import SparkUtils
 
         session_id = spark_session.conf.get("ai.h2o.featurestore.sessionId", "")
         request = pb.RetrieveFeatureViewAsSparkRequest(
             feature_view_id=self.id,
             feature_view_version=self.version,
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/ingest.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/ingest.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
         Reverting creates a new minor version with the data corresponding to the specific ingest removed.
 
         Typical example:
             ingest.revert()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/ingest_history_api.html#reverting-ingestion
+            https://docs.h2o.ai/featurestore/api/ingest_history_api.html#reverting-ingestion
         """
         job = self.revert_async()
         return job.wait_for_result()
 
     def revert_async(self) -> RevertIngestJob:
         """Create a revert ingestion job for feature set.
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/ingest_job.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/ingest_job.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/materialization_online_job.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/materialization_online_job.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/ml_data_feature.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/ml_data_feature.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/ml_dataset.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/ml_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         Returns:
             str: A directory path where the files are downloaded.
 
         Typical usage example:
             dir = ml_dataset.download()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_view_api.html#downloading-the-files-from-feature-store-from-the-ml-dataset
+            https://docs.h2o.ai/featurestore/api/feature_view_api.html#downloading-the-files-from-feature-store-from-the-ml-dataset
         """
         request = pb.RetrieveMLDatasetAsAsLinksRequest(ml_dataset_id=self.id)
         job_id = self._stub.StartRetrieveMLDatasetAsLinksJob(request)
 
         info = JobInfo(self._stub, job_id)
         while not self._stub.GetJob(job_id).done:
             info.show_progress()
@@ -132,15 +132,15 @@
             The frame is made up of columns as features and rows as records.
             Rows contain data within retrieve scope (filtered).
 
         Typical usage example:
             data_frame = ml_dataset.as_spark_frame(sparkSession)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_view_api.html#obtaining-data-as-a-spark-frame-from-the-ml-dataset
+            https://docs.h2o.ai/featurestore/api/feature_view_api.html#obtaining-data-as-a-spark-frame-from-the-ml-dataset
         """
         from ..commons.spark_utils import SparkUtils
 
         session_id = spark_session.conf.get("ai.h2o.featurestore.sessionId", "")
         request = pb.RetrieveMLDatasetAsSparkRequest(ml_dataset_id=self.id, session_id=session_id)
 
         response = self._stub.RetrieveMLDatasetAsSpark(request)
@@ -185,15 +185,15 @@
 
             {'id': '01', 'department': 'Engineering', 'name': 'Test'}
 
         Typical example:
             ml_dataset.retrieve_online(1)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_view_api.html#retrieving-data-from-online-feature-store
+            https://docs.h2o.ai/featurestore/api/feature_view_api.html#retrieving-data-from-online-feature-store
         """
         if self._online_retrieval_token is None or not self._online_retrieval_token.is_valid_for(self.id):
             request = OnlineApi.OnlineMLDataSetRetrieveTokenRequest(ml_dataset_id=self.id)
 
             response: OnlineApi.OnlineRetrieveTokenResponse = self._stub.GenerateMLDatasetOnlineRetrievalToken(request)
             self._online_retrieval_token = OnlineToken(
                 ml_dataset_id=self.id,
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/optimize_storage_job.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/optimize_storage_job.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/pat.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/pat.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/permission.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/permission.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,11 +23,11 @@
         Args:
             reason: (str) A reason for revoke.
 
         Typical example:
             manageable_permission.revoke("user left the project")
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#managing-permission-requests-from-other-users
+            https://docs.h2o.ai/featurestore/api/permissions.html#managing-permission-requests-from-other-users
         """
         request = pb.RevokePermissionRequest(permission_id=self._permission.id, reason=reason)
         self._stub.RevokePermission(request)
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/permission_base.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/permission_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         Returns:
             Project | FeatureSet: A corresponding project or feature set.
 
         Typical example:
             manageable_request.get_resource()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#managing-permission-requests-from-other-users
+            https://docs.h2o.ai/featurestore/api/permissions.html#managing-permission-requests-from-other-users
         """
         if self._permission.resource_type == pb.ResourceType.PROJECT:
             request = pb.GetProjectRequest(project_name=self._project_name)
             response = self._stub.GetProject(request)
             return Project(self._stub, self._rest_stub, response.project)
         elif self._permission.resource_type == pb.ResourceType.FEATURE_SET:
             request = pb.FeatureSetRequestId(feature_set_id=self._permission.resource_id)
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/pinned_feature_set.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/pinned_feature_set.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/project.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         Returns:
             Project: An existing project with the latest information.
 
         Typical example:
             project.add_owners(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#project-permission-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#project-permission-api
         """
         return self._add_permissions(user_emails, pb.PermissionType.Owner)
 
     def add_editors(self, user_emails):
         """Add additional editor/editors to project.
 
         Args:
@@ -116,15 +116,15 @@
         Returns:
             Project: An existing project with the latest information.
 
         Typical example:
             project.add_editors(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#project-permission-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#project-permission-api
         """
         return self._add_permissions(user_emails, pb.PermissionType.Editor)
 
     def add_consumers(self, user_emails):
         """Add additional consumer/consumers to project.
 
         Args:
@@ -133,15 +133,15 @@
         Returns:
             Project: An existing project with the latest information.
 
         Typical example:
             project.add_consumers(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#project-permission-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#project-permission-api
         """
         return self._add_permissions(user_emails, pb.PermissionType.Consumer)
 
     def add_sensitive_consumers(self, user_emails):
         """Add additional sensitive consumer/consumers to project.
 
         Args:
@@ -150,15 +150,15 @@
         Returns:
             Project: An existing project with the latest information.
 
         Typical example:
             project.add_sensitive_consumers(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#project-permission-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#project-permission-api
         """
         return self._add_permissions(user_emails, pb.PermissionType.SensitiveConsumer)
 
     def add_viewers(self, user_emails):
         """Add additional viewer/viewers to project.
 
         Args:
@@ -167,15 +167,15 @@
         Returns:
             Project: An existing project with the latest information.
 
         Typical example:
             project.add_viewers(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#project-permission-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#project-permission-api
         """
         return self._add_permissions(user_emails, pb.PermissionType.Viewer)
 
     def remove_owners(self, user_emails):
         """Remove owner/owners from project.
 
         Args:
@@ -184,15 +184,15 @@
         Returns:
             Project: An existing project with the latest information.
 
         Typical example:
             project.remove_owners(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#project-permission-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#project-permission-api
         """
         return self._remove_permissions(user_emails, pb.PermissionType.Owner)
 
     def remove_editors(self, user_emails):
         """Remove editor/editors from project.
 
         Args:
@@ -201,15 +201,15 @@
         Returns:
             Project: An existing project with the latest information.
 
         Typical example:
             project.remove_editors(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#project-permission-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#project-permission-api
         """
         return self._remove_permissions(user_emails, pb.PermissionType.Editor)
 
     def remove_consumers(self, user_emails):
         """Remove consumer/consumers from project.
 
         Args:
@@ -218,15 +218,15 @@
         Returns:
             Project: An existing project with the latest information.
 
         Typical example:
             project.remove_consumers(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#project-permission-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#project-permission-api
         """
         return self._remove_permissions(user_emails, pb.PermissionType.Consumer)
 
     def remove_sensitive_consumers(self, user_emails):
         """Remove sensitive consumer/consumers from project.
 
         Args:
@@ -235,15 +235,15 @@
         Returns:
             Project: An existing project with the latest information.
 
         Typical example:
             project.remove_sensitive_consumers(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#project-permission-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#project-permission-api
         """
         return self._remove_permissions(user_emails, pb.PermissionType.SensitiveConsumer)
 
     def remove_viewers(self, user_emails):
         """Remove viewer/viewers from project.
 
         Args:
@@ -252,15 +252,15 @@
         Returns:
             Project: An existing project with the latest information.
 
         Typical example:
             project.remove_viewers(["bob@h2o.ai", "alice@h2o.ai"])
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#project-permission-api
+            https://docs.h2o.ai/featurestore/api/permissions.html#project-permission-api
         """
         return self._remove_permissions(user_emails, pb.PermissionType.Viewer)
 
     def list_owners(self):
         return self._list_users(pb.PermissionType.Owner)
 
     def list_editors(self):
@@ -314,15 +314,15 @@
         Returns:
             str: A permission id.
 
         Typical example:
             my_request_id = project.request_access(AccessType.CONSUMER, "Preparing the best model")
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/permissions.html#requesting-permissions-to-a-project
+            https://docs.h2o.ai/featurestore/api/permissions.html#requesting-permissions-to-a-project
         """
         request = pb.SubmitPendingPermissionRequest()
         request.resource_id = self._project.id
         request.permission = AccessType.to_proto_permission(access_type)
         request.reason = reason
         response = self._stub.SubmitPendingProjectPermission(request)
         return response.permission_id
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/project_history.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/project_history.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/query.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,14 @@
     def join(self, feature_set: Union[FeatureSet, fsref.FeatureSetRef], alias) -> OpenedJoin:
         return self._join(feature_set, alias, JoinType.INNER)
 
     def left_join(self, feature_set: Union[FeatureSet, fsref.FeatureSetRef], alias) -> OpenedJoin:
         return self._join(feature_set, alias, JoinType.LEFT)
 
     def _to_proto(self) -> pb.FeatureQuery:
-
         fs_to_alias = dict(
             [(join._feature_set, join._alias) for join in self._joins if join._alias]
             + [(self._select.feature_set, self._select.alias)]
             if self._select.alias
             else []
         )
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/recently_used_feature_set.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/recently_used_feature_set.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/recently_used_project.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/recently_used_project.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/recommendation.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/recommendation.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/retrieve_job.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/retrieve_job.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/scheduled_task.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/scheduled_task.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/task_execution_history.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/task_execution_history.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/transformation_function.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/transformation_function.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/entities/user_with_permission.py` & `h2o-featurestore-1.2.0/featurestore/core/entities/user_with_permission.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/feature_set_flow.py` & `h2o-featurestore-1.2.0/featurestore/core/feature_set_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from enum import Enum
 
 import ai.h2o.featurestore.api.v1.FeatureSetProtoApi_pb2 as FeatureSetApi
 
 
 class FeatureSetFlow(Enum):
-
     ONLINE_ONLY = 1
     OFFLINE_ONLY = 2
     OFFLINE_ONLINE_MANUAL = 3
     OFFLINE_ONLINE_AUTOMATIC = 4
 
     @staticmethod
     def _from_proto(flow: FeatureSetApi.FeatureSetFlow):
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/interactive_console.py` & `h2o-featurestore-1.2.0/featurestore/core/interactive_console.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/interceptors.py` & `h2o-featurestore-1.2.0/featurestore/core/interceptors.py`

 * *Files identical despite different names*

```diff
@@ -113,20 +113,18 @@
         status_for_retry: Optional[List[grpc.StatusCode]] = None,
     ):
         self.max_attempts = max_attempts
         self.sleeping_policy = sleeping_policy
         self.status_for_retry = status_for_retry
 
     def _intercept_call(self, continuation, client_call_details, request_or_iterator):
-
         for try_i in range(self.max_attempts):
             response = continuation(client_call_details, request_or_iterator)
 
             if isinstance(response, grpc.RpcError):
-
                 # Return if it was last attempt
                 if try_i == (self.max_attempts - 1):
                     return response
 
                 # If status code is not in retryable status codes
                 if self.status_for_retry and response.code() not in self.status_for_retry:
                     return response
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/job_info.py` & `h2o-featurestore-1.2.0/featurestore/core/job_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             'Finished reading data from source location to extract schema.': '7s',
             'Schema generation completed.': '0s'}
 
         Typical example:
             job.get_metrics()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/jobs_api.html?highlight=get_metrics#checking-job-metrics
+            https://docs.h2o.ai/featurestore/api/jobs_api.html?highlight=get_metrics#checking-job-metrics
         """
         if self._stub.GetJob(self._job_id).done:
             request = pb.JobProgressInput(job_id=self._job_id.job_id, next_index=0)
             response = self._stub.GetJobProgress(request)
             if response.progress:
                 return {progress.message: f"{progress.duration_in_seconds}s" for progress in response.progress}
         else:
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/retrieve_holder.py` & `h2o-featurestore-1.2.0/featurestore/core/retrieve_holder.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         Typical usage example:
 
             retrieve_job = client.jobs.get(<job id>)
             dir = retrieve_job.download()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/jobs_api.html#how-to-download-using-retrievejob
+            https://docs.h2o.ai/featurestore/api/jobs_api.html#how-to-download-using-retrievejob
         """
         self._process_lazy_ingest_task()
         if not self._job_id:
             self._job_id = self._start_retrieve_links_job()
 
         info = JobInfo(self._stub, self._job_id)
         while not self._get_job(self._job_id).done:
@@ -62,15 +62,15 @@
 
         Typical usage example:
 
             retrieve_job = client.jobs.get(<job id>)
             future = retrieve_job.download_async()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/jobs_api.html#how-to-download-using-retrievejob
+            https://docs.h2o.ai/featurestore/api/jobs_api.html#how-to-download-using-retrievejob
         """
         future = self._thread_pool.submit(self.download, output_dir)
         return DownloadFuture(future)
 
     def _start_retrieve_links_job(self):
         request = self._create_retrieve_request()
         return self._stub.StartRetrieveAsLinksJob(request)
@@ -131,15 +131,15 @@
 
         Typical usage example:
 
             ref = feature_set.retrieve()
             dir = ref.download()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#downloading-the-files-from-feature-store
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#downloading-the-files-from-feature-store
         """
         return super(RetrieveHolder, self).download(output_dir)
 
     def download_async(self, output_dir=None):
         """Downloads files asynchronously to the specified directory location.
 
         Args:
@@ -155,15 +155,15 @@
 
         Typical usage example:
 
             ref = feature_set.retrieve()
             future = ref.download_async()
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#downloading-the-files-from-feature-store
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#downloading-the-files-from-feature-store
         """
         return super(RetrieveHolder, self).download_async(output_dir)
 
     def as_spark_frame(self, spark_session):
         """Returns a spark data frame.
 
         Generates a data frame of the retrieved data using spark session.
@@ -179,15 +179,15 @@
 
         Typical usage example:
 
             ref = feature_set.retrieve()
             data_frame = ref.as_spark_frame(spark_session)
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/feature_set_api.html#obtaining-data-as-a-spark-frame
+            https://docs.h2o.ai/featurestore/api/feature_set_api.html#obtaining-data-as-a-spark-frame
         """
         from pyspark.sql.functions import col, from_utc_timestamp, lit, to_timestamp, unix_timestamp
         from pyspark.sql.types import TimestampType
 
         self._process_lazy_ingest_task()
         if self._retrieve_as_spark_response is None:
             request = self._create_retrieve_request(spark_session)
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/schema.py` & `h2o-featurestore-1.2.0/featurestore/core/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             FeatureSchemaMonitoring(feature.monitoring.anomaly_detection),
         )
 
     @staticmethod
     def get_and_validate_feature_type(feature_type):
         valid_values = FeatureSetApi.FeatureType.keys()
         if feature_type.upper() in valid_values:
-            FeatureSetApi.FeatureType.Value(feature_type.upper())
+            return FeatureSetApi.FeatureType.Value(feature_type.upper())
         else:
             raise Exception("Invalid feature type. Supported values are: " + ", ".join(map(str, valid_values)))
 
     def __repr__(self):
         return self.to_string()
 
 
@@ -224,15 +224,15 @@
         Typical example:
             schema = Schema.create_from("col1 string, col2 string, col3 integer")
 
         Raises:
             Exception: Schema can be created either from string or existing feature set.
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/schema_api.html#create-a-schema-from-a-string
+            https://docs.h2o.ai/featurestore/api/schema_api.html#create-a-schema-from-a-string
         """
         from .entities.feature_set import FeatureSet
 
         if isinstance(obj, FeatureSet):
             features = [FeatureSchema.create_from(feature) for name, feature in obj.features.items()]
             if obj.is_derived():
                 derived_from = obj._feature_set.derived_from
@@ -288,15 +288,15 @@
 
         Typical example:
             schema_str = "id INT, text STRING, label DOUBLE, state STRING, date STRING"
             schema = Schema.create_from(schema_str)
             schema.select("id text label")
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/schema_api.html#create-a-new-schema-by-column-selection
+            https://docs.h2o.ai/featurestore/api/schema_api.html#create-a-new-schema-by-column-selection
         """
         self._feature_schemas = list(filter(lambda schema: schema.name in feature_names, self._feature_schemas))
         return self
 
     def exclude(self, feature_names):
         """Create a new schema by column selection.
 
@@ -312,15 +312,15 @@
 
         Typical example:
             schema_str = "id INT, text STRING, label DOUBLE, state STRING, date STRING"
             schema = Schema.create_from(schema_str)
             schema.exclude("id text label")
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/schema_api.html#create-a-new-schema-by-column-selection
+            https://docs.h2o.ai/featurestore/api/schema_api.html#create-a-new-schema-by-column-selection
         """
         self._feature_schemas = list(filter(lambda schema: schema.name not in feature_names, self._feature_schemas))
         return self
 
     def append(self, feature_schema, after=None):
         """Create a new schema.
 
@@ -342,15 +342,15 @@
             schema.append(new_feature_schema)  # Append to the end
             schema.append(new_feature_schema, schema["old"])  # Append after old
 
         Raises:
             Exception: Feature name does not exist in the schema.
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/schema_api.html#create-a-new-schema-by-adding-a-new-feature-schema
+            https://docs.h2o.ai/featurestore/api/schema_api.html#create-a-new-schema-by-adding-a-new-feature-schema
         """
         if not after:
             self._feature_schemas.append(feature_schema)
         else:
             index = self._feature_schemas.index(after) + 1
             self._feature_schemas.insert(index, feature_schema)
         return self
@@ -376,15 +376,15 @@
             schema.prepend(new_feature_schema)  # Prepend to the beginning
             schema.prepend(new_feature_schema, schema["old"])  # Prepend before old
 
         Raises:
             Exception: Feature name does not exist in the schema.
 
         For more details:
-            https://docs.h2o.ai/feature-store/latest-stable/docs/api/schema_api.html#create-a-new-schema-by-adding-a-new-feature-schema
+            https://docs.h2o.ai/featurestore/api/schema_api.html#create-a-new-schema-by-adding-a-new-feature-schema
         """
         if not before:
             self._feature_schemas.insert(0, feature_schema)
         else:
             index = self._feature_schemas.index(before)
             self._feature_schemas.insert(index, feature_schema)
         return self
@@ -398,14 +398,19 @@
 
     def to_string(self):
         return self._to_string("")
 
     def _to_string(self, prefix):
         return "\n".join(["{}".format(nested._to_string(prefix)) for nested in self._feature_schemas])
 
+    def to_sql_string(self):
+        return ", ".join(
+            [f"{feature_schema.name} {feature_schema.data_type}" for feature_schema in self._feature_schemas]
+        )
+
     def _to_proto_schema(self):
         return [
             pb.FeatureSchema(
                 name=feature_schema.name,
                 data_type=feature_schema.data_type,
                 nested=feature_schema.schema._to_proto_schema(),
                 special_data=pb.FeatureSchema.SpecialData(
```

### Comparing `h2o-featurestore-1.1.2/featurestore/core/search_field.py` & `h2o-featurestore-1.2.0/featurestore/core/search_field.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/storage_optimization.py` & `h2o-featurestore-1.2.0/featurestore/core/storage_optimization.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/transformations.py` & `h2o-featurestore-1.2.0/featurestore/core/transformations.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/user_credentials.py` & `h2o-featurestore-1.2.0/featurestore/core/user_credentials.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/core/utils.py` & `h2o-featurestore-1.2.0/featurestore/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,19 @@
                     f.write(chunk)
         return dest
 
     @staticmethod
     def fetch_preview_as_json_array(preview_url: str):
         with requests.get(preview_url) as r:
             r.raise_for_status()
-            preview_array = r.text.strip().split("\n")
-            return [json.loads(item) for item in preview_array]
+            if r.text:
+                preview_array = r.text.strip().split("\n")
+                return [json.loads(item) for item in preview_array]
+            else:
+                return []
 
     @staticmethod
     def generate_md5_checksum(file):
         hash_md5 = hashlib.md5()
         with open(file, "rb") as f:
             for chunk in iter(lambda: f.read(4096), b""):
                 hash_md5.update(chunk)
```

### Comparing `h2o-featurestore-1.1.2/featurestore/logger.py` & `h2o-featurestore-1.2.0/featurestore/logger.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/featurestore/rest_stub.py` & `h2o-featurestore-1.2.0/featurestore/rest_stub.py`

 * *Files identical despite different names*

### Comparing `h2o-featurestore-1.1.2/h2o_featurestore.egg-info/SOURCES.txt` & `h2o-featurestore-1.2.0/h2o_featurestore.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,26 +3,33 @@
 setup.cfg
 setup.py
 ai/__init__.py
 ai/h2o/__init__.py
 ai/h2o/featurestore/__init__.py
 ai/h2o/featurestore/api/__init__.py
 ai/h2o/featurestore/api/v1/CoreService_pb2.py
+ai/h2o/featurestore/api/v1/CoreService_pb2.pyi
 ai/h2o/featurestore/api/v1/CoreService_pb2_grpc.py
 ai/h2o/featurestore/api/v1/DashboardApi_pb2.py
+ai/h2o/featurestore/api/v1/DashboardApi_pb2.pyi
 ai/h2o/featurestore/api/v1/DashboardApi_pb2_grpc.py
 ai/h2o/featurestore/api/v1/FeatureSetProtoApi_pb2.py
+ai/h2o/featurestore/api/v1/FeatureSetProtoApi_pb2.pyi
 ai/h2o/featurestore/api/v1/FeatureSetProtoApi_pb2_grpc.py
 ai/h2o/featurestore/api/v1/FeatureSetSearch_pb2.py
+ai/h2o/featurestore/api/v1/FeatureSetSearch_pb2.pyi
 ai/h2o/featurestore/api/v1/FeatureSetSearch_pb2_grpc.py
 ai/h2o/featurestore/api/v1/OnlineApi_pb2.py
+ai/h2o/featurestore/api/v1/OnlineApi_pb2.pyi
 ai/h2o/featurestore/api/v1/OnlineApi_pb2_grpc.py
 ai/h2o/featurestore/api/v1/RecommendationProtoApi_pb2.py
+ai/h2o/featurestore/api/v1/RecommendationProtoApi_pb2.pyi
 ai/h2o/featurestore/api/v1/RecommendationProtoApi_pb2_grpc.py
 ai/h2o/featurestore/api/v1/TimeToLiveApi_pb2.py
+ai/h2o/featurestore/api/v1/TimeToLiveApi_pb2.pyi
 ai/h2o/featurestore/api/v1/TimeToLiveApi_pb2_grpc.py
 ai/h2o/featurestore/api/v1/__init__.py
 featurestore/__init__.py
 featurestore/client.py
 featurestore/logger.py
 featurestore/rest_stub.py
 featurestore/version.txt
```

### Comparing `h2o-featurestore-1.1.2/setup.py` & `h2o-featurestore-1.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,28 +7,32 @@
 
 setup(
     name='h2o-featurestore',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="1.1.2",
+    version="1.2.0",
     description='Feature Store Client for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://docs.h2o.ai/feature-store/latest-stable/docs/index.html',
-    download_url='https://docs.h2o.ai/feature-store/latest-stable/docs/download.html',
+    url='https://docs.h2o.ai/featurestore/',
+    download_url='https://docs.h2o.ai/featurestore/get-started/download',
     author='H2O.ai',
     author_email='support@h2o.ai',
     license='Apache v2',
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8"
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12"
     ],
     keywords='machine learning, data mining, statistical analysis, modeling, big data, distributed, parallel',
 
     # find python packages starting in the current directory
     packages=find_packages(),
 
     # run-time dependencies
```

