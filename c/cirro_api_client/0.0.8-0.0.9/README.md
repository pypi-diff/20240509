# Comparing `tmp/cirro_api_client-0.0.8.tar.gz` & `tmp/cirro_api_client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirro_api_client-0.0.8.tar", max compression
+gzip compressed data, was "cirro_api_client-0.0.9.tar", max compression
```

## Comparing `cirro_api_client-0.0.8.tar` & `cirro_api_client-0.0.9.tar`

### file list

```diff
@@ -1,182 +1,182 @@
--rw-r--r--   0        0        0     3892 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/README.md
--rw-r--r--   0        0        0      164 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/__init__.py
--rw-r--r--   0        0        0      716 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/cirro_auth.py
--rw-r--r--   0        0        0     2148 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/cirro_client.py
--rw-r--r--   0        0        0      100 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/__init__.py
--rw-r--r--   0        0        0       47 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/__init__.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/billing/__init__.py
--rw-r--r--   0        0        0     4179 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/billing/create_billing_account.py
--rw-r--r--   0        0        0     2513 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/billing/delete_billing_account.py
--rw-r--r--   0        0        0     2101 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/billing/generate_billing_report.py
--rw-r--r--   0        0        0     4848 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/billing/get_billing_accounts.py
--rw-r--r--   0        0        0     2971 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/billing/update_billing_account.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/dashboards/__init__.py
--rw-r--r--   0        0        0     4438 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/dashboards/create_dashboard.py
--rw-r--r--   0        0        0     4174 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/dashboards/delete_dashboard.py
--rw-r--r--   0        0        0     4159 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/dashboards/get_dashboard.py
--rw-r--r--   0        0        0     4170 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/dashboards/get_dashboards.py
--rw-r--r--   0        0        0     4752 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/dashboards/update_dashboard.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/__init__.py
--rw-r--r--   0        0        0     2735 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/delete_dataset.py
--rw-r--r--   0        0        0     4246 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/get_dataset.py
--rw-r--r--   0        0        0     4529 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/get_dataset_manifest.py
--rw-r--r--   0        0        0     5396 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/get_datasets.py
--rw-r--r--   0        0        0     4551 2024-01-31 21:38:18.428845 cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/import_public_dataset.py
--rw-r--r--   0        0        0     2649 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/ingest_samples.py
--rw-r--r--   0        0        0     2686 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/regenerate_manifest.py
--rw-r--r--   0        0        0     2658 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/rerun_transform.py
--rw-r--r--   0        0        0     4824 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/update_dataset.py
--rw-r--r--   0        0        0     4847 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/upload_dataset.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/__init__.py
--rw-r--r--   0        0        0     5206 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/get_execution_logs.py
--rw-r--r--   0        0        0     5058 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/get_project_summary.py
--rw-r--r--   0        0        0     5504 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/get_task_logs.py
--rw-r--r--   0        0        0     5265 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/get_tasks_for_execution.py
--rw-r--r--   0        0        0     4411 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/run_analysis.py
--rw-r--r--   0        0        0     4421 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/stop_analysis.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/file/__init__.py
--rw-r--r--   0        0        0     4623 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/file/generate_project_file_access_token.py
--rw-r--r--   0        0        0     4762 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/file/generate_project_sftp_token.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/metadata/__init__.py
--rw-r--r--   0        0        0     5477 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/metadata/get_project_samples.py
--rw-r--r--   0        0        0     3727 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/metadata/get_project_schema.py
--rw-r--r--   0        0        0     2773 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/metadata/update_project_schema.py
--rw-r--r--   0        0        0     4647 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/metadata/update_sample.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/metrics/__init__.py
--rw-r--r--   0        0        0     3582 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/metrics/get_all_metrics.py
--rw-r--r--   0        0        0     3912 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/metrics/get_project_metrics.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/__init__.py
--rw-r--r--   0        0        0     4731 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/create_notebook_instance.py
--rw-r--r--   0        0        0     2791 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/delete_notebook_instance.py
--rw-r--r--   0        0        0     4866 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/generate_notebook_instance_url.py
--rw-r--r--   0        0        0     4714 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/get_notebook_instance_status.py
--rw-r--r--   0        0        0     4362 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/get_notebook_instances.py
--rw-r--r--   0        0        0     2778 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/stop_notebook_instance.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/__init__.py
--rw-r--r--   0        0        0     2493 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/archive_custom_process.py
--rw-r--r--   0        0        0     5162 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/create_custom_process.py
--rw-r--r--   0        0        0     3896 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/get_process.py
--rw-r--r--   0        0        0     3916 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/get_process_parameters.py
--rw-r--r--   0        0        0     4638 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/get_processes.py
--rw-r--r--   0        0        0     4079 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/sync_custom_process.py
--rw-r--r--   0        0        0     2836 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/update_custom_process.py
--rw-r--r--   0        0        0     4959 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/validate_file_requirements.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/__init__.py
--rw-r--r--   0        0        0     4038 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/create_project.py
--rw-r--r--   0        0        0     3851 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/get_project.py
--rw-r--r--   0        0        0     4194 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/get_project_users.py
--rw-r--r--   0        0        0     3415 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/get_projects.py
--rw-r--r--   0        0        0     2463 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/redeploy_project.py
--rw-r--r--   0        0        0     2926 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/set_user_project_role.py
--rw-r--r--   0        0        0     4370 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/update_project.py
--rw-r--r--   0        0        0     2894 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/update_project_tags.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/references/__init__.py
--rw-r--r--   0        0        0     4466 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/references/create_project_reference.py
--rw-r--r--   0        0        0     2437 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/references/delete_project_reference.py
--rw-r--r--   0        0        0     3541 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/references/get_reference_types.py
--rw-r--r--   0        0        0     3567 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/references/get_references.py
--rw-r--r--   0        0        0     4178 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/references/get_references_for_project.py
--rw-r--r--   0        0        0     2474 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/references/refresh_project_references.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/system/__init__.py
--rw-r--r--   0        0        0     3629 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/system/get_service_connections.py
--rw-r--r--   0        0        0     3159 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/system/info.py
--rw-r--r--   0        0        0        0 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/users/__init__.py
--rw-r--r--   0        0        0     3634 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/users/get_user.py
--rw-r--r--   0        0        0     4215 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/users/get_users.py
--rw-r--r--   0        0        0     4149 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/users/invite_user.py
--rw-r--r--   0        0        0     4259 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/api/users/update_user.py
--rw-r--r--   0        0        0     6024 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/client.py
--rw-r--r--   0        0        0      470 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/errors.py
--rw-r--r--   0        0        0     6492 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/__init__.py
--rw-r--r--   0        0        0      283 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/access_type.py
--rw-r--r--   0        0        0     2196 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/allowed_data_type.py
--rw-r--r--   0        0        0     2274 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/aws_credentials.py
--rw-r--r--   0        0        0     3610 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/billing_account.py
--rw-r--r--   0        0        0     3089 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/billing_account_request.py
--rw-r--r--   0        0        0      214 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/billing_method.py
--rw-r--r--   0        0        0      195 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/budget_period.py
--rw-r--r--   0        0        0     1883 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/cloud_account.py
--rw-r--r--   0        0        0     1539 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/contact.py
--rw-r--r--   0        0        0     1982 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/create_notebook_instance_request.py
--rw-r--r--   0        0        0     1723 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/create_reference_request.py
--rw-r--r--   0        0        0     1201 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/create_response.py
--rw-r--r--   0        0        0     5140 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/custom_pipeline_settings.py
--rw-r--r--   0        0        0      199 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/customer_type.py
--rw-r--r--   0        0        0     3181 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/dashboard.py
--rw-r--r--   0        0        0      884 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/dashboard_dashboard_data.py
--rw-r--r--   0        0        0      836 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/dashboard_info.py
--rw-r--r--   0        0        0     2442 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/dashboard_request.py
--rw-r--r--   0        0        0      922 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/dashboard_request_dashboard_data.py
--rw-r--r--   0        0        0      874 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/dashboard_request_info.py
--rw-r--r--   0        0        0     3566 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/dataset.py
--rw-r--r--   0        0        0     2870 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/dataset_assets_manifest.py
--rw-r--r--   0        0        0     4681 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/dataset_detail.py
--rw-r--r--   0        0        0      859 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/dataset_detail_info.py
--rw-r--r--   0        0        0      869 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/dataset_detail_params.py
--rw-r--r--   0        0        0     1910 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/dataset_viz.py
--rw-r--r--   0        0        0     1068 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/error_message.py
--rw-r--r--   0        0        0      187 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/executor.py
--rw-r--r--   0        0        0     2839 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/file_access_request.py
--rw-r--r--   0        0        0     2289 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/file_entry.py
--rw-r--r--   0        0        0      931 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/file_entry_metadata.py
--rw-r--r--   0        0        0     1347 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/file_name_pattern.py
--rw-r--r--   0        0        0     2215 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/file_requirements.py
--rw-r--r--   0        0        0     2265 2024-01-31 21:38:18.432845 cirro_api_client-0.0.8/cirro_api_client/v1/models/form_schema.py
--rw-r--r--   0        0        0      886 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/form_schema_form.py
--rw-r--r--   0        0        0      884 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/form_schema_ui.py
--rw-r--r--   0        0        0     1371 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/generate_sftp_credentials_request.py
--rw-r--r--   0        0        0     1571 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/get_execution_logs_response.py
--rw-r--r--   0        0        0     1784 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/get_project_summary_response_200.py
--rw-r--r--   0        0        0     1691 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/import_data_request.py
--rw-r--r--   0        0        0     1442 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/invite_user_request.py
--rw-r--r--   0        0        0     1101 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/invite_user_response.py
--rw-r--r--   0        0        0     1442 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/log_entry.py
--rw-r--r--   0        0        0     2565 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/metric_record.py
--rw-r--r--   0        0        0      980 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/metric_record_services.py
--rw-r--r--   0        0        0     2932 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/notebook_instance.py
--rw-r--r--   0        0        0     1395 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/notebook_instance_status_response.py
--rw-r--r--   0        0        0     1287 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/open_notebook_instance_response.py
--rw-r--r--   0        0        0     1757 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/paginated_response_dataset_list_dto.py
--rw-r--r--   0        0        0     1722 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/paginated_response_sample_dto.py
--rw-r--r--   0        0        0     2152 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/pipeline_code.py
--rw-r--r--   0        0        0     2204 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/portal_error_response.py
--rw-r--r--   0        0        0     4962 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/process.py
--rw-r--r--   0        0        0     8887 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/process_detail.py
--rw-r--r--   0        0        0     2373 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/project.py
--rw-r--r--   0        0        0     4378 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/project_detail.py
--rw-r--r--   0        0        0     3712 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/project_metrics.py
--rw-r--r--   0        0        0     5262 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/project_request.py
--rw-r--r--   0        0        0      220 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/project_role.py
--rw-r--r--   0        0        0     8472 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/project_settings.py
--rw-r--r--   0        0        0     2020 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/project_user.py
--rw-r--r--   0        0        0     2599 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/reference.py
--rw-r--r--   0        0        0     2284 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/reference_type.py
--rw-r--r--   0        0        0      912 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/reference_type_validation_item.py
--rw-r--r--   0        0        0      227 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/repository_type.py
--rw-r--r--   0        0        0     1753 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/resources_info.py
--rw-r--r--   0        0        0     4386 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/run_analysis_request.py
--rw-r--r--   0        0        0      938 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/run_analysis_request_params.py
--rw-r--r--   0        0        0     2324 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/sample.py
--rw-r--r--   0        0        0      841 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/sample_metadata.py
--rw-r--r--   0        0        0     1489 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/sample_request.py
--rw-r--r--   0        0        0      879 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/sample_request_metadata.py
--rw-r--r--   0        0        0     1276 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/service_connection.py
--rw-r--r--   0        0        0     1834 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/set_user_project_role_request.py
--rw-r--r--   0        0        0     1781 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/sftp_credentials.py
--rw-r--r--   0        0        0      335 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/status.py
--rw-r--r--   0        0        0     1824 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/stop_execution_response.py
--rw-r--r--   0        0        0      167 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/sync_status.py
--rw-r--r--   0        0        0     2853 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/system_info_response.py
--rw-r--r--   0        0        0     1318 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/tag.py
--rw-r--r--   0        0        0     3332 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/task.py
--rw-r--r--   0        0        0     2024 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/update_dataset_request.py
--rw-r--r--   0        0        0     2051 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/update_user_request.py
--rw-r--r--   0        0        0      902 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/update_user_request_settings.py
--rw-r--r--   0        0        0     1483 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/upload_dataset_create_response.py
--rw-r--r--   0        0        0     1996 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/upload_dataset_request.py
--rw-r--r--   0        0        0     1604 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/user.py
--rw-r--r--   0        0        0     1453 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/models/validate_file_requirements_request.py
--rw-r--r--   0        0        0       25 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/py.typed
--rw-r--r--   0        0        0      986 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/cirro_api_client/v1/types.py
--rw-r--r--   0        0        0      680 2024-01-31 21:38:18.436845 cirro_api_client-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 cirro_api_client-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3892 2024-02-06 18:22:42.222895 cirro_api_client-0.0.9/README.md
+-rw-r--r--   0        0        0      164 2024-02-06 18:22:42.222895 cirro_api_client-0.0.9/cirro_api_client/__init__.py
+-rw-r--r--   0        0        0      716 2024-02-06 18:22:42.222895 cirro_api_client-0.0.9/cirro_api_client/cirro_auth.py
+-rw-r--r--   0        0        0     2148 2024-02-06 18:22:42.222895 cirro_api_client-0.0.9/cirro_api_client/cirro_client.py
+-rw-r--r--   0        0        0      100 2024-02-06 18:22:42.222895 cirro_api_client-0.0.9/cirro_api_client/v1/__init__.py
+-rw-r--r--   0        0        0       47 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/billing/__init__.py
+-rw-r--r--   0        0        0     4179 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/billing/create_billing_account.py
+-rw-r--r--   0        0        0     2513 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/billing/delete_billing_account.py
+-rw-r--r--   0        0        0     2101 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/billing/generate_billing_report.py
+-rw-r--r--   0        0        0     4848 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/billing/get_billing_accounts.py
+-rw-r--r--   0        0        0     2971 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/billing/update_billing_account.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/dashboards/__init__.py
+-rw-r--r--   0        0        0     4438 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/dashboards/create_dashboard.py
+-rw-r--r--   0        0        0     4174 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/dashboards/delete_dashboard.py
+-rw-r--r--   0        0        0     4159 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/dashboards/get_dashboard.py
+-rw-r--r--   0        0        0     4170 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/dashboards/get_dashboards.py
+-rw-r--r--   0        0        0     4752 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/dashboards/update_dashboard.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/__init__.py
+-rw-r--r--   0        0        0     2735 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/delete_dataset.py
+-rw-r--r--   0        0        0     4246 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/get_dataset.py
+-rw-r--r--   0        0        0     4529 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/get_dataset_manifest.py
+-rw-r--r--   0        0        0     5387 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/get_datasets.py
+-rw-r--r--   0        0        0     4551 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/import_public_dataset.py
+-rw-r--r--   0        0        0     2649 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/ingest_samples.py
+-rw-r--r--   0        0        0     2686 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/regenerate_manifest.py
+-rw-r--r--   0        0        0     2658 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/rerun_transform.py
+-rw-r--r--   0        0        0     4824 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/update_dataset.py
+-rw-r--r--   0        0        0     4847 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/upload_dataset.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/__init__.py
+-rw-r--r--   0        0        0     5206 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/get_execution_logs.py
+-rw-r--r--   0        0        0     5058 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/get_project_summary.py
+-rw-r--r--   0        0        0     5504 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/get_task_logs.py
+-rw-r--r--   0        0        0     5265 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/get_tasks_for_execution.py
+-rw-r--r--   0        0        0     4411 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/run_analysis.py
+-rw-r--r--   0        0        0     4421 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/stop_analysis.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/file/__init__.py
+-rw-r--r--   0        0        0     4623 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/file/generate_project_file_access_token.py
+-rw-r--r--   0        0        0     4762 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/file/generate_project_sftp_token.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/metadata/__init__.py
+-rw-r--r--   0        0        0     5468 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/metadata/get_project_samples.py
+-rw-r--r--   0        0        0     3727 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/metadata/get_project_schema.py
+-rw-r--r--   0        0        0     2773 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/metadata/update_project_schema.py
+-rw-r--r--   0        0        0     4647 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/metadata/update_sample.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/metrics/__init__.py
+-rw-r--r--   0        0        0     3582 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/metrics/get_all_metrics.py
+-rw-r--r--   0        0        0     3912 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/metrics/get_project_metrics.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/__init__.py
+-rw-r--r--   0        0        0     4731 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/create_notebook_instance.py
+-rw-r--r--   0        0        0     2791 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/delete_notebook_instance.py
+-rw-r--r--   0        0        0     4866 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/generate_notebook_instance_url.py
+-rw-r--r--   0        0        0     4714 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/get_notebook_instance_status.py
+-rw-r--r--   0        0        0     4362 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/get_notebook_instances.py
+-rw-r--r--   0        0        0     2778 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/stop_notebook_instance.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/__init__.py
+-rw-r--r--   0        0        0     2493 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/archive_custom_process.py
+-rw-r--r--   0        0        0     5162 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/create_custom_process.py
+-rw-r--r--   0        0        0     3896 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/get_process.py
+-rw-r--r--   0        0        0     3916 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/get_process_parameters.py
+-rw-r--r--   0        0        0     4638 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/get_processes.py
+-rw-r--r--   0        0        0     4079 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/sync_custom_process.py
+-rw-r--r--   0        0        0     2836 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/update_custom_process.py
+-rw-r--r--   0        0        0     4959 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/validate_file_requirements.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/__init__.py
+-rw-r--r--   0        0        0     4038 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/create_project.py
+-rw-r--r--   0        0        0     3851 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/get_project.py
+-rw-r--r--   0        0        0     4194 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/get_project_users.py
+-rw-r--r--   0        0        0     3415 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/get_projects.py
+-rw-r--r--   0        0        0     2463 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/redeploy_project.py
+-rw-r--r--   0        0        0     2926 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/set_user_project_role.py
+-rw-r--r--   0        0        0     4370 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/update_project.py
+-rw-r--r--   0        0        0     2894 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/update_project_tags.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/references/__init__.py
+-rw-r--r--   0        0        0     4466 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/references/create_project_reference.py
+-rw-r--r--   0        0        0     2437 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/references/delete_project_reference.py
+-rw-r--r--   0        0        0     3541 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/references/get_reference_types.py
+-rw-r--r--   0        0        0     3567 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/references/get_references.py
+-rw-r--r--   0        0        0     4178 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/references/get_references_for_project.py
+-rw-r--r--   0        0        0     2474 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/references/refresh_project_references.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/system/__init__.py
+-rw-r--r--   0        0        0     3629 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/system/get_service_connections.py
+-rw-r--r--   0        0        0     3159 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/system/info.py
+-rw-r--r--   0        0        0        0 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/users/__init__.py
+-rw-r--r--   0        0        0     3634 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/users/get_user.py
+-rw-r--r--   0        0        0     4215 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/users/get_users.py
+-rw-r--r--   0        0        0     4149 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/users/invite_user.py
+-rw-r--r--   0        0        0     4259 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/api/users/update_user.py
+-rw-r--r--   0        0        0     6024 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/client.py
+-rw-r--r--   0        0        0      470 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/errors.py
+-rw-r--r--   0        0        0     6492 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/models/__init__.py
+-rw-r--r--   0        0        0      283 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/models/access_type.py
+-rw-r--r--   0        0        0     2196 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/models/allowed_data_type.py
+-rw-r--r--   0        0        0     2274 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/models/aws_credentials.py
+-rw-r--r--   0        0        0     3610 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/models/billing_account.py
+-rw-r--r--   0        0        0     3089 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/models/billing_account_request.py
+-rw-r--r--   0        0        0      214 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/models/billing_method.py
+-rw-r--r--   0        0        0      195 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/models/budget_period.py
+-rw-r--r--   0        0        0     1944 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/models/cloud_account.py
+-rw-r--r--   0        0        0     1539 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/models/contact.py
+-rw-r--r--   0        0        0     1982 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/models/create_notebook_instance_request.py
+-rw-r--r--   0        0        0     1723 2024-02-06 18:22:42.226895 cirro_api_client-0.0.9/cirro_api_client/v1/models/create_reference_request.py
+-rw-r--r--   0        0        0     1201 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/create_response.py
+-rw-r--r--   0        0        0     5140 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/custom_pipeline_settings.py
+-rw-r--r--   0        0        0      199 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/customer_type.py
+-rw-r--r--   0        0        0     3181 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/dashboard.py
+-rw-r--r--   0        0        0      884 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/dashboard_dashboard_data.py
+-rw-r--r--   0        0        0      836 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/dashboard_info.py
+-rw-r--r--   0        0        0     2442 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/dashboard_request.py
+-rw-r--r--   0        0        0      922 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/dashboard_request_dashboard_data.py
+-rw-r--r--   0        0        0      874 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/dashboard_request_info.py
+-rw-r--r--   0        0        0     3566 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/dataset.py
+-rw-r--r--   0        0        0     2870 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/dataset_assets_manifest.py
+-rw-r--r--   0        0        0     4681 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/dataset_detail.py
+-rw-r--r--   0        0        0      859 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/dataset_detail_info.py
+-rw-r--r--   0        0        0      869 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/dataset_detail_params.py
+-rw-r--r--   0        0        0     1910 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/dataset_viz.py
+-rw-r--r--   0        0        0     1068 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/error_message.py
+-rw-r--r--   0        0        0      187 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/executor.py
+-rw-r--r--   0        0        0     2839 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/file_access_request.py
+-rw-r--r--   0        0        0     2289 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/file_entry.py
+-rw-r--r--   0        0        0      931 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/file_entry_metadata.py
+-rw-r--r--   0        0        0     1347 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/file_name_pattern.py
+-rw-r--r--   0        0        0     2215 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/file_requirements.py
+-rw-r--r--   0        0        0     2265 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/form_schema.py
+-rw-r--r--   0        0        0      886 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/form_schema_form.py
+-rw-r--r--   0        0        0      884 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/form_schema_ui.py
+-rw-r--r--   0        0        0     1371 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/generate_sftp_credentials_request.py
+-rw-r--r--   0        0        0     1571 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/get_execution_logs_response.py
+-rw-r--r--   0        0        0     1784 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/get_project_summary_response_200.py
+-rw-r--r--   0        0        0     1691 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/import_data_request.py
+-rw-r--r--   0        0        0     1442 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/invite_user_request.py
+-rw-r--r--   0        0        0     1101 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/invite_user_response.py
+-rw-r--r--   0        0        0     1442 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/log_entry.py
+-rw-r--r--   0        0        0     2565 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/metric_record.py
+-rw-r--r--   0        0        0      980 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/metric_record_services.py
+-rw-r--r--   0        0        0     2932 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/notebook_instance.py
+-rw-r--r--   0        0        0     1395 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/notebook_instance_status_response.py
+-rw-r--r--   0        0        0     1287 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/open_notebook_instance_response.py
+-rw-r--r--   0        0        0     1757 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/paginated_response_dataset_list_dto.py
+-rw-r--r--   0        0        0     1722 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/paginated_response_sample_dto.py
+-rw-r--r--   0        0        0     2152 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/pipeline_code.py
+-rw-r--r--   0        0        0     2204 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/portal_error_response.py
+-rw-r--r--   0        0        0     6096 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/process.py
+-rw-r--r--   0        0        0     9677 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/process_detail.py
+-rw-r--r--   0        0        0     2373 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/project.py
+-rw-r--r--   0        0        0     4378 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/project_detail.py
+-rw-r--r--   0        0        0     3712 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/project_metrics.py
+-rw-r--r--   0        0        0     5262 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/project_request.py
+-rw-r--r--   0        0        0      220 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/project_role.py
+-rw-r--r--   0        0        0     8472 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/project_settings.py
+-rw-r--r--   0        0        0     2020 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/project_user.py
+-rw-r--r--   0        0        0     2599 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/reference.py
+-rw-r--r--   0        0        0     2284 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/reference_type.py
+-rw-r--r--   0        0        0      912 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/reference_type_validation_item.py
+-rw-r--r--   0        0        0      227 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/repository_type.py
+-rw-r--r--   0        0        0     1753 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/resources_info.py
+-rw-r--r--   0        0        0     4386 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/run_analysis_request.py
+-rw-r--r--   0        0        0      938 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/run_analysis_request_params.py
+-rw-r--r--   0        0        0     2324 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/sample.py
+-rw-r--r--   0        0        0      841 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/sample_metadata.py
+-rw-r--r--   0        0        0     1489 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/sample_request.py
+-rw-r--r--   0        0        0      879 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/sample_request_metadata.py
+-rw-r--r--   0        0        0     1276 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/service_connection.py
+-rw-r--r--   0        0        0     1834 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/set_user_project_role_request.py
+-rw-r--r--   0        0        0     1781 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/sftp_credentials.py
+-rw-r--r--   0        0        0      335 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/status.py
+-rw-r--r--   0        0        0     1824 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/stop_execution_response.py
+-rw-r--r--   0        0        0      167 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/sync_status.py
+-rw-r--r--   0        0        0     2853 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/system_info_response.py
+-rw-r--r--   0        0        0     1318 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/tag.py
+-rw-r--r--   0        0        0     3332 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/task.py
+-rw-r--r--   0        0        0     2024 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/update_dataset_request.py
+-rw-r--r--   0        0        0     2051 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/update_user_request.py
+-rw-r--r--   0        0        0      902 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/update_user_request_settings.py
+-rw-r--r--   0        0        0     1483 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/upload_dataset_create_response.py
+-rw-r--r--   0        0        0     1996 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/upload_dataset_request.py
+-rw-r--r--   0        0        0     1604 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/user.py
+-rw-r--r--   0        0        0     1453 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/models/validate_file_requirements_request.py
+-rw-r--r--   0        0        0       25 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/py.typed
+-rw-r--r--   0        0        0      986 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/cirro_api_client/v1/types.py
+-rw-r--r--   0        0        0      680 2024-02-06 18:22:42.230895 cirro_api_client-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4747 1970-01-01 00:00:00.000000 cirro_api_client-0.0.9/PKG-INFO
```

### Comparing `cirro_api_client-0.0.8/README.md` & `cirro_api_client-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/cirro_auth.py` & `cirro_api_client-0.0.9/cirro_api_client/cirro_auth.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/cirro_client.py` & `cirro_api_client-0.0.9/cirro_api_client/cirro_client.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/billing/create_billing_account.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/billing/create_billing_account.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/billing/delete_billing_account.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/billing/delete_billing_account.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/billing/generate_billing_report.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/billing/generate_billing_report.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/billing/get_billing_accounts.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/billing/get_billing_accounts.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/billing/update_billing_account.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/billing/update_billing_account.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/dashboards/create_dashboard.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/dashboards/create_dashboard.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/dashboards/delete_dashboard.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/dashboards/delete_dashboard.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/dashboards/get_dashboard.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/dashboards/get_dashboard.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/dashboards/get_dashboards.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/dashboards/get_dashboards.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/dashboards/update_dashboard.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/dashboards/update_dashboard.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/delete_dataset.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/delete_dataset.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/get_dataset.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/get_dataset.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/get_dataset_manifest.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/get_dataset_manifest.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/get_datasets.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/get_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ...models.paginated_response_dataset_list_dto import PaginatedResponseDatasetListDto
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     project_id: str,
     *,
-    limit: Union[Unset, int] = 10000,
+    limit: Union[Unset, int] = 5000,
     next_token: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
     params: Dict[str, Any] = {}
 
     params["limit"] = limit
 
     params["nextToken"] = next_token
@@ -52,24 +52,24 @@
     )
 
 
 def sync_detailed(
     project_id: str,
     *,
     client: Client,
-    limit: Union[Unset, int] = 10000,
+    limit: Union[Unset, int] = 5000,
     next_token: Union[Unset, str] = UNSET,
 ) -> Response[PaginatedResponseDatasetListDto]:
     """List datasets
 
      Retrieves a list of datasets for a given project
 
     Args:
         project_id (str):
-        limit (Union[Unset, int]):  Default: 10000.
+        limit (Union[Unset, int]):  Default: 5000.
         next_token (Union[Unset, str]):
         client (Client): instance of the API client
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -91,24 +91,24 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_id: str,
     *,
     client: Client,
-    limit: Union[Unset, int] = 10000,
+    limit: Union[Unset, int] = 5000,
     next_token: Union[Unset, str] = UNSET,
 ) -> Optional[PaginatedResponseDatasetListDto]:
     """List datasets
 
      Retrieves a list of datasets for a given project
 
     Args:
         project_id (str):
-        limit (Union[Unset, int]):  Default: 10000.
+        limit (Union[Unset, int]):  Default: 5000.
         next_token (Union[Unset, str]):
         client (Client): instance of the API client
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -124,24 +124,24 @@
     ).parsed
 
 
 async def asyncio_detailed(
     project_id: str,
     *,
     client: Client,
-    limit: Union[Unset, int] = 10000,
+    limit: Union[Unset, int] = 5000,
     next_token: Union[Unset, str] = UNSET,
 ) -> Response[PaginatedResponseDatasetListDto]:
     """List datasets
 
      Retrieves a list of datasets for a given project
 
     Args:
         project_id (str):
-        limit (Union[Unset, int]):  Default: 10000.
+        limit (Union[Unset, int]):  Default: 5000.
         next_token (Union[Unset, str]):
         client (Client): instance of the API client
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -160,24 +160,24 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: str,
     *,
     client: Client,
-    limit: Union[Unset, int] = 10000,
+    limit: Union[Unset, int] = 5000,
     next_token: Union[Unset, str] = UNSET,
 ) -> Optional[PaginatedResponseDatasetListDto]:
     """List datasets
 
      Retrieves a list of datasets for a given project
 
     Args:
         project_id (str):
-        limit (Union[Unset, int]):  Default: 10000.
+        limit (Union[Unset, int]):  Default: 5000.
         next_token (Union[Unset, str]):
         client (Client): instance of the API client
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/import_public_dataset.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/import_public_dataset.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/ingest_samples.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/ingest_samples.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/regenerate_manifest.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/regenerate_manifest.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/rerun_transform.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/rerun_transform.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/update_dataset.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/update_dataset.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/datasets/upload_dataset.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/datasets/upload_dataset.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/get_execution_logs.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/get_execution_logs.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/get_project_summary.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/get_project_summary.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/get_task_logs.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/get_task_logs.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/get_tasks_for_execution.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/get_tasks_for_execution.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/run_analysis.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/run_analysis.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/execution/stop_analysis.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/execution/stop_analysis.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/file/generate_project_file_access_token.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/file/generate_project_file_access_token.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/file/generate_project_sftp_token.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/file/generate_project_sftp_token.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/metadata/get_project_samples.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/metadata/get_project_samples.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ...models.paginated_response_sample_dto import PaginatedResponseSampleDto
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     project_id: str,
     *,
-    limit: Union[Unset, int] = 10000,
+    limit: Union[Unset, int] = 5000,
     next_token: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
     params: Dict[str, Any] = {}
 
     params["limit"] = limit
 
     params["nextToken"] = next_token
@@ -52,24 +52,24 @@
     )
 
 
 def sync_detailed(
     project_id: str,
     *,
     client: Client,
-    limit: Union[Unset, int] = 10000,
+    limit: Union[Unset, int] = 5000,
     next_token: Union[Unset, str] = UNSET,
 ) -> Response[PaginatedResponseSampleDto]:
     """Get project samples
 
      Retrieves a list of samples associated with a project along with their metadata
 
     Args:
         project_id (str):
-        limit (Union[Unset, int]):  Default: 10000.
+        limit (Union[Unset, int]):  Default: 5000.
         next_token (Union[Unset, str]):
         client (Client): instance of the API client
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -91,24 +91,24 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_id: str,
     *,
     client: Client,
-    limit: Union[Unset, int] = 10000,
+    limit: Union[Unset, int] = 5000,
     next_token: Union[Unset, str] = UNSET,
 ) -> Optional[PaginatedResponseSampleDto]:
     """Get project samples
 
      Retrieves a list of samples associated with a project along with their metadata
 
     Args:
         project_id (str):
-        limit (Union[Unset, int]):  Default: 10000.
+        limit (Union[Unset, int]):  Default: 5000.
         next_token (Union[Unset, str]):
         client (Client): instance of the API client
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -124,24 +124,24 @@
     ).parsed
 
 
 async def asyncio_detailed(
     project_id: str,
     *,
     client: Client,
-    limit: Union[Unset, int] = 10000,
+    limit: Union[Unset, int] = 5000,
     next_token: Union[Unset, str] = UNSET,
 ) -> Response[PaginatedResponseSampleDto]:
     """Get project samples
 
      Retrieves a list of samples associated with a project along with their metadata
 
     Args:
         project_id (str):
-        limit (Union[Unset, int]):  Default: 10000.
+        limit (Union[Unset, int]):  Default: 5000.
         next_token (Union[Unset, str]):
         client (Client): instance of the API client
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -160,24 +160,24 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: str,
     *,
     client: Client,
-    limit: Union[Unset, int] = 10000,
+    limit: Union[Unset, int] = 5000,
     next_token: Union[Unset, str] = UNSET,
 ) -> Optional[PaginatedResponseSampleDto]:
     """Get project samples
 
      Retrieves a list of samples associated with a project along with their metadata
 
     Args:
         project_id (str):
-        limit (Union[Unset, int]):  Default: 10000.
+        limit (Union[Unset, int]):  Default: 5000.
         next_token (Union[Unset, str]):
         client (Client): instance of the API client
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/metadata/get_project_schema.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/metadata/get_project_schema.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/metadata/update_project_schema.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/metadata/update_project_schema.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/metadata/update_sample.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/metadata/update_sample.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/metrics/get_all_metrics.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/metrics/get_all_metrics.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/metrics/get_project_metrics.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/metrics/get_project_metrics.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/create_notebook_instance.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/create_notebook_instance.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/delete_notebook_instance.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/delete_notebook_instance.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/generate_notebook_instance_url.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/generate_notebook_instance_url.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/get_notebook_instance_status.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/get_notebook_instance_status.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/get_notebook_instances.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/get_notebook_instances.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/notebooks/stop_notebook_instance.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/notebooks/stop_notebook_instance.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/archive_custom_process.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/archive_custom_process.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/create_custom_process.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/create_custom_process.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/get_process.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/get_process.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/get_process_parameters.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/get_process_parameters.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/get_processes.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/get_processes.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/sync_custom_process.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/sync_custom_process.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/update_custom_process.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/update_custom_process.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/processes/validate_file_requirements.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/processes/validate_file_requirements.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/create_project.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/create_project.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/get_project.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/get_project.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/get_project_users.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/get_project_users.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/get_projects.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/get_projects.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/redeploy_project.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/redeploy_project.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/set_user_project_role.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/set_user_project_role.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/update_project.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/update_project.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/projects/update_project_tags.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/projects/update_project_tags.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/references/create_project_reference.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/references/create_project_reference.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/references/delete_project_reference.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/references/delete_project_reference.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/references/get_reference_types.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/references/get_reference_types.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/references/get_references.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/references/get_references.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/references/get_references_for_project.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/references/get_references_for_project.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/references/refresh_project_references.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/references/refresh_project_references.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/system/get_service_connections.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/system/get_service_connections.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/system/info.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/system/info.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/users/get_user.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/users/get_users.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/users/get_users.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/users/invite_user.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/users/invite_user.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/api/users/update_user.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/api/users/update_user.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/client.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/client.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/__init__.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/allowed_data_type.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/allowed_data_type.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/aws_credentials.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/billing_account.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/billing_account.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/billing_account_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/billing_account_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/cloud_account.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/cloud_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 
 
 @_attrs_define
 class CloudAccount:
     """
     Attributes:
         account_id (Union[Unset, str]): AWS Account ID
-        account_name (Union[Unset, str]): Name used to describe the account
+        account_name (Union[Unset, str]): Name used to describe the account, useful when the account hosts multiple
+            projects
         region_name (Union[Unset, str]): AWS Region Code Example: us-west-2.
     """
 
     account_id: Union[Unset, str] = UNSET
     account_name: Union[Unset, str] = UNSET
     region_name: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
```

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/contact.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/contact.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/create_notebook_instance_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/create_notebook_instance_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/create_reference_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/create_reference_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/create_response.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/create_response.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/custom_pipeline_settings.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/custom_pipeline_settings.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/dashboard.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/dashboard_dashboard_data.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/dashboard_dashboard_data.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/dashboard_info.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/dashboard_info.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/dashboard_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/dashboard_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/dashboard_request_dashboard_data.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/dashboard_request_dashboard_data.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/dashboard_request_info.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/dashboard_request_info.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/dataset.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/dataset_assets_manifest.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/dataset_assets_manifest.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/dataset_detail.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/dataset_detail.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/dataset_detail_info.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/dataset_detail_info.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/dataset_detail_params.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/dataset_detail_params.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/dataset_viz.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/dataset_viz.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/error_message.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/error_message.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/file_access_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/file_access_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/file_entry.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/file_entry.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/file_entry_metadata.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/file_entry_metadata.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/file_name_pattern.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/file_name_pattern.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/file_requirements.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/file_requirements.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/form_schema.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/form_schema.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/form_schema_form.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/form_schema_form.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/form_schema_ui.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/form_schema_ui.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/generate_sftp_credentials_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/generate_sftp_credentials_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/get_execution_logs_response.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/get_execution_logs_response.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/get_project_summary_response_200.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/get_project_summary_response_200.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/import_data_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/import_data_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/invite_user_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/invite_user_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/invite_user_response.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/invite_user_response.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/log_entry.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/log_entry.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/metric_record.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/metric_record.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/metric_record_services.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/metric_record_services.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/notebook_instance.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/notebook_instance.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/notebook_instance_status_response.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/notebook_instance_status_response.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/open_notebook_instance_response.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/open_notebook_instance_response.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/paginated_response_dataset_list_dto.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/paginated_response_dataset_list_dto.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/paginated_response_sample_dto.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/paginated_response_sample_dto.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/pipeline_code.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/pipeline_code.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/portal_error_response.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/portal_error_response.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/process.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/process.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,44 +14,55 @@
     """
     Attributes:
         id (str): Unique ID of the Process Example: process-hutch-magic_flute-1_0.
         name (str): Friendly name for the process Example: MAGeCK Flute.
         executor (Executor):
         description (Union[Unset, str]):  Example: MAGeCK Flute enables accurate identification of essential genes with
             their related biological functions..
+        data_type (Union[None, Unset, str]): Name of the data type this pipeline produces (if it is not defined, use the
+            name)
         documentation_url (Union[Unset, str]): Link to pipeline documentation Example:
             https://docs.cirro.bio/pipelines/catalog_targeted_sequencing/#crispr-screen-analysis.
         file_requirements_message (Union[Unset, str]): Description of the files to be uploaded (optional)
         child_process_ids (Union[Unset, List[str]]): IDs of pipelines that can be run downstream
         parent_process_ids (Union[Unset, List[str]]): IDs of pipelines that can run this pipeline
         owner (Union[Unset, str]): Username of the pipeline creator (blank if Cirro curated)
         linked_project_ids (Union[Unset, List[str]]): Projects that can run this pipeline
+        is_archived (Union[Unset, bool]): Whether the pipeline is marked as archived
     """
 
     id: str
     name: str
     executor: Executor
     description: Union[Unset, str] = UNSET
+    data_type: Union[None, Unset, str] = UNSET
     documentation_url: Union[Unset, str] = UNSET
     file_requirements_message: Union[Unset, str] = UNSET
     child_process_ids: Union[Unset, List[str]] = UNSET
     parent_process_ids: Union[Unset, List[str]] = UNSET
     owner: Union[Unset, str] = UNSET
     linked_project_ids: Union[Unset, List[str]] = UNSET
+    is_archived: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
         name = self.name
 
         executor = self.executor.value
 
         description = self.description
 
+        data_type: Union[None, Unset, str]
+        if isinstance(self.data_type, Unset):
+            data_type = UNSET
+        else:
+            data_type = self.data_type
+
         documentation_url = self.documentation_url
 
         file_requirements_message = self.file_requirements_message
 
         child_process_ids: Union[Unset, List[str]] = UNSET
         if not isinstance(self.child_process_ids, Unset):
             child_process_ids = self.child_process_ids
@@ -62,74 +73,93 @@
 
         owner = self.owner
 
         linked_project_ids: Union[Unset, List[str]] = UNSET
         if not isinstance(self.linked_project_ids, Unset):
             linked_project_ids = self.linked_project_ids
 
+        is_archived = self.is_archived
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "id": id,
                 "name": name,
                 "executor": executor,
             }
         )
         if description is not UNSET:
             field_dict["description"] = description
+        if data_type is not UNSET:
+            field_dict["dataType"] = data_type
         if documentation_url is not UNSET:
             field_dict["documentationUrl"] = documentation_url
         if file_requirements_message is not UNSET:
             field_dict["fileRequirementsMessage"] = file_requirements_message
         if child_process_ids is not UNSET:
             field_dict["childProcessIds"] = child_process_ids
         if parent_process_ids is not UNSET:
             field_dict["parentProcessIds"] = parent_process_ids
         if owner is not UNSET:
             field_dict["owner"] = owner
         if linked_project_ids is not UNSET:
             field_dict["linkedProjectIds"] = linked_project_ids
+        if is_archived is not UNSET:
+            field_dict["isArchived"] = is_archived
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         name = d.pop("name")
 
         executor = Executor(d.pop("executor"))
 
         description = d.pop("description", UNSET)
 
+        def _parse_data_type(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        data_type = _parse_data_type(d.pop("dataType", UNSET))
+
         documentation_url = d.pop("documentationUrl", UNSET)
 
         file_requirements_message = d.pop("fileRequirementsMessage", UNSET)
 
         child_process_ids = cast(List[str], d.pop("childProcessIds", UNSET))
 
         parent_process_ids = cast(List[str], d.pop("parentProcessIds", UNSET))
 
         owner = d.pop("owner", UNSET)
 
         linked_project_ids = cast(List[str], d.pop("linkedProjectIds", UNSET))
 
+        is_archived = d.pop("isArchived", UNSET)
+
         process = cls(
             id=id,
             name=name,
             executor=executor,
             description=description,
+            data_type=data_type,
             documentation_url=documentation_url,
             file_requirements_message=file_requirements_message,
             child_process_ids=child_process_ids,
             parent_process_ids=parent_process_ids,
             owner=owner,
             linked_project_ids=linked_project_ids,
+            is_archived=is_archived,
         )
 
         process.additional_properties = d
         return process
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/process_detail.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/process_detail.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         name (str): Friendly name for the process Example: MAGeCK Flute.
         description (str):  Example: MAGeCK Flute enables accurate identification of essential genes with their related
             biological functions.
         executor (Executor):
         child_process_ids (List[str]): IDs of pipelines that can be run downstream
         parent_process_ids (List[str]): IDs of pipelines that can run this pipeline
         linked_project_ids (List[str]): Projects that can run this pipeline
+        data_type (Union[None, Unset, str]): Name of the data type this pipeline produces (if it is not defined, use the
+            name)
         documentation_url (Union[None, Unset, str]): Link to pipeline documentation Example:
             https://docs.cirro.bio/pipelines/catalog_targeted_sequencing/#crispr-screen-analysis.
         file_requirements_message (Union[None, Unset, str]): Description of the files to be uploaded (optional)
         pipeline_code (Union['PipelineCode', None, Unset]):
         owner (Union[None, Unset, str]): Username of the pipeline creator (blank if Cirro curated)
         custom_settings (Union['CustomPipelineSettings', None, Unset]):
         is_archived (Union[Unset, bool]): Whether the process is marked for removal
@@ -38,14 +40,15 @@
     id: str
     name: str
     description: str
     executor: Executor
     child_process_ids: List[str]
     parent_process_ids: List[str]
     linked_project_ids: List[str]
+    data_type: Union[None, Unset, str] = UNSET
     documentation_url: Union[None, Unset, str] = UNSET
     file_requirements_message: Union[None, Unset, str] = UNSET
     pipeline_code: Union["PipelineCode", None, Unset] = UNSET
     owner: Union[None, Unset, str] = UNSET
     custom_settings: Union["CustomPipelineSettings", None, Unset] = UNSET
     is_archived: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
@@ -64,14 +67,20 @@
 
         child_process_ids = self.child_process_ids
 
         parent_process_ids = self.parent_process_ids
 
         linked_project_ids = self.linked_project_ids
 
+        data_type: Union[None, Unset, str]
+        if isinstance(self.data_type, Unset):
+            data_type = UNSET
+        else:
+            data_type = self.data_type
+
         documentation_url: Union[None, Unset, str]
         if isinstance(self.documentation_url, Unset):
             documentation_url = UNSET
         else:
             documentation_url = self.documentation_url
 
         file_requirements_message: Union[None, Unset, str]
@@ -113,14 +122,16 @@
                 "description": description,
                 "executor": executor,
                 "childProcessIds": child_process_ids,
                 "parentProcessIds": parent_process_ids,
                 "linkedProjectIds": linked_project_ids,
             }
         )
+        if data_type is not UNSET:
+            field_dict["dataType"] = data_type
         if documentation_url is not UNSET:
             field_dict["documentationUrl"] = documentation_url
         if file_requirements_message is not UNSET:
             field_dict["fileRequirementsMessage"] = file_requirements_message
         if pipeline_code is not UNSET:
             field_dict["pipelineCode"] = pipeline_code
         if owner is not UNSET:
@@ -148,14 +159,23 @@
 
         child_process_ids = cast(List[str], d.pop("childProcessIds"))
 
         parent_process_ids = cast(List[str], d.pop("parentProcessIds"))
 
         linked_project_ids = cast(List[str], d.pop("linkedProjectIds"))
 
+        def _parse_data_type(data: object) -> Union[None, Unset, str]:
+            if data is None:
+                return data
+            if isinstance(data, Unset):
+                return data
+            return cast(Union[None, Unset, str], data)
+
+        data_type = _parse_data_type(d.pop("dataType", UNSET))
+
         def _parse_documentation_url(data: object) -> Union[None, Unset, str]:
             if data is None:
                 return data
             if isinstance(data, Unset):
                 return data
             return cast(Union[None, Unset, str], data)
 
@@ -219,14 +239,15 @@
             id=id,
             name=name,
             description=description,
             executor=executor,
             child_process_ids=child_process_ids,
             parent_process_ids=parent_process_ids,
             linked_project_ids=linked_project_ids,
+            data_type=data_type,
             documentation_url=documentation_url,
             file_requirements_message=file_requirements_message,
             pipeline_code=pipeline_code,
             owner=owner,
             custom_settings=custom_settings,
             is_archived=is_archived,
         )
```

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/project.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/project.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/project_detail.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/project_detail.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/project_metrics.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/project_metrics.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/project_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/project_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/project_settings.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/project_settings.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/project_user.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/project_user.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/reference.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/reference.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/reference_type.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/reference_type.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/reference_type_validation_item.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/reference_type_validation_item.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/resources_info.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/resources_info.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/run_analysis_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/run_analysis_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/run_analysis_request_params.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/run_analysis_request_params.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/sample.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/sample.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/sample_metadata.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/sample_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/sample_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/sample_request_metadata.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/sample_request_metadata.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/service_connection.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/service_connection.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/set_user_project_role_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/set_user_project_role_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/sftp_credentials.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/sftp_credentials.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/stop_execution_response.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/stop_execution_response.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/system_info_response.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/system_info_response.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/tag.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/tag.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/task.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/task.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/update_dataset_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/update_dataset_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/update_user_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/update_user_request_settings.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/update_user_request_settings.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/upload_dataset_create_response.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/upload_dataset_create_response.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/upload_dataset_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/upload_dataset_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/user.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/user.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/models/validate_file_requirements_request.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/models/validate_file_requirements_request.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/cirro_api_client/v1/types.py` & `cirro_api_client-0.0.9/cirro_api_client/v1/types.py`

 * *Files identical despite different names*

### Comparing `cirro_api_client-0.0.8/pyproject.toml` & `cirro_api_client-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cirro_api_client"
-version = "0.0.8"
+version = "0.0.9"
 description = "A client library for accessing Cirro"
 authors = ["Cirro <support@cirro.bio>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/CirroBio/Cirro-client-python"
 keywords = ["Cirro"]
 include = ["cirro_api_client/py.typed"]
```

### Comparing `cirro_api_client-0.0.8/PKG-INFO` & `cirro_api_client-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirro_api_client
-Version: 0.0.8
+Version: 0.0.9
 Summary: A client library for accessing Cirro
 Home-page: https://github.com/CirroBio/Cirro-client-python
 License: MIT
 Keywords: Cirro
 Author: Cirro
 Author-email: support@cirro.bio
 Requires-Python: >=3.8,<4.0
```

