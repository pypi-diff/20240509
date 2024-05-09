# Comparing `tmp/superwise_api-1.3.0.tar.gz` & `tmp/superwise_api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superwise_api-1.3.0.tar", max compression
+gzip compressed data, was "superwise_api-2.0.0.tar", max compression
```

## Comparing `superwise_api-1.3.0.tar` & `superwise_api-2.0.0.tar`

### file list

```diff
@@ -1,207 +1,207 @@
--rw-r--r--   0        0        0      487 2024-04-14 09:12:10.632515 superwise_api-1.3.0/README.md
--rw-r--r--   0        0        0      828 2024-04-14 09:12:30.199422 superwise_api-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      276 2024-04-14 09:12:10.671519 superwise_api-1.3.0/superwise_api/__init__.py
--rw-r--r--   0        0        0     9994 2024-04-14 09:12:10.671519 superwise_api-1.3.0/superwise_api/client/__init__.py
--rw-r--r--   0        0        0      654 2024-04-14 09:12:10.672519 superwise_api-1.3.0/superwise_api/client/api/__init__.py
--rw-r--r--   0        0        0    54734 2024-04-14 09:12:10.672519 superwise_api-1.3.0/superwise_api/client/api/applications_api.py
--rw-r--r--   0        0        0    33591 2024-04-14 09:12:10.673519 superwise_api-1.3.0/superwise_api/client/api/dashboard_items_api.py
--rw-r--r--   0        0        0    31775 2024-04-14 09:12:10.673519 superwise_api-1.3.0/superwise_api/client/api/dashboards_api.py
--rw-r--r--   0        0        0    43860 2024-04-14 09:12:10.674519 superwise_api-1.3.0/superwise_api/client/api/dataset_api.py
--rw-r--r--   0        0        0    38374 2024-04-14 09:12:10.674519 superwise_api-1.3.0/superwise_api/client/api/dataset_sources_api.py
--rw-r--r--   0        0        0    36742 2024-04-14 09:12:10.675519 superwise_api-1.3.0/superwise_api/client/api/destinations_api.py
--rw-r--r--   0        0        0    21619 2024-04-14 09:12:10.675519 superwise_api-1.3.0/superwise_api/client/api/integrations_api.py
--rw-r--r--   0        0        0    44731 2024-04-14 09:12:10.676519 superwise_api-1.3.0/superwise_api/client/api/policies_api.py
--rw-r--r--   0        0        0    38625 2024-04-14 09:12:10.676519 superwise_api-1.3.0/superwise_api/client/api/sources_api.py
--rw-r--r--   0        0        0    28011 2024-04-14 09:12:10.677519 superwise_api-1.3.0/superwise_api/client/api_client.py
--rw-r--r--   0        0        0      862 2024-04-14 09:12:10.677519 superwise_api-1.3.0/superwise_api/client/api_response.py
--rw-r--r--   0        0        0    14478 2024-04-14 09:12:10.677519 superwise_api-1.3.0/superwise_api/client/configuration.py
--rw-r--r--   0        0        0     5283 2024-04-14 09:12:10.677519 superwise_api-1.3.0/superwise_api/client/exceptions.py
--rw-r--r--   0        0        0     8787 2024-04-14 09:12:10.678519 superwise_api-1.3.0/superwise_api/client/models/__init__.py
--rw-r--r--   0        0        0      796 2024-04-14 09:12:10.678519 superwise_api-1.3.0/superwise_api/client/models/alert_on_status_direction.py
--rw-r--r--   0        0        0     4546 2024-04-14 09:12:10.678519 superwise_api-1.3.0/superwise_api/client/models/application.py
--rw-r--r--   0        0        0     3116 2024-04-14 09:12:10.678519 superwise_api-1.3.0/superwise_api/client/models/application_config.py
--rw-r--r--   0        0        0     3299 2024-04-14 09:12:10.678519 superwise_api-1.3.0/superwise_api/client/models/application_config_payload.py
--rw-r--r--   0        0        0     2634 2024-04-14 09:12:10.679519 superwise_api-1.3.0/superwise_api/client/models/application_create.py
--rw-r--r--   0        0        0     4781 2024-04-14 09:12:10.679519 superwise_api-1.3.0/superwise_api/client/models/application_model.py
--rw-r--r--   0        0        0     3046 2024-04-14 09:12:10.679519 superwise_api-1.3.0/superwise_api/client/models/application_response.py
--rw-r--r--   0        0        0     4816 2024-04-14 09:12:10.679519 superwise_api-1.3.0/superwise_api/client/models/application_type.py
--rw-r--r--   0        0        0     2816 2024-04-14 09:12:10.679519 superwise_api-1.3.0/superwise_api/client/models/application_update.py
--rw-r--r--   0        0        0     2160 2024-04-14 09:12:10.680519 superwise_api-1.3.0/superwise_api/client/models/ask_config.py
--rw-r--r--   0        0        0     3138 2024-04-14 09:12:10.680519 superwise_api-1.3.0/superwise_api/client/models/ask_request_payload.py
--rw-r--r--   0        0        0     1837 2024-04-14 09:12:10.680519 superwise_api-1.3.0/superwise_api/client/models/ask_response_payload.py
--rw-r--r--   0        0        0     2588 2024-04-14 09:12:10.680519 superwise_api-1.3.0/superwise_api/client/models/aws_credentials_request.py
--rw-r--r--   0        0        0     2577 2024-04-14 09:12:10.680519 superwise_api-1.3.0/superwise_api/client/models/aws_credentials_response.py
--rw-r--r--   0        0        0     2650 2024-04-14 09:12:10.681520 superwise_api-1.3.0/superwise_api/client/models/azure_credentials_request.py
--rw-r--r--   0        0        0     2643 2024-04-14 09:12:10.681520 superwise_api-1.3.0/superwise_api/client/models/azure_credentials_response.py
--rw-r--r--   0        0        0     1966 2024-04-14 09:12:10.681520 superwise_api-1.3.0/superwise_api/client/models/chat_history_entry.py
--rw-r--r--   0        0        0     8587 2024-04-14 09:12:10.681520 superwise_api-1.3.0/superwise_api/client/models/config.py
--rw-r--r--   0        0        0     5642 2024-04-14 09:12:10.681520 superwise_api-1.3.0/superwise_api/client/models/config1.py
--rw-r--r--   0        0        0     4820 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/created_at.py
--rw-r--r--   0        0        0     4756 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/created_by.py
--rw-r--r--   0        0        0     2304 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/dashboard.py
--rw-r--r--   0        0        0     1780 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/dashboard_create.py
--rw-r--r--   0        0        0     3285 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/dashboard_item.py
--rw-r--r--   0        0        0     3049 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/dashboard_item_create.py
--rw-r--r--   0        0        0     3994 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/dashboard_item_query.py
--rw-r--r--   0        0        0     4956 2024-04-14 09:12:10.682520 superwise_api-1.3.0/superwise_api/client/models/dashboard_item_query_order.py
--rw-r--r--   0        0        0     2929 2024-04-14 09:12:10.683520 superwise_api-1.3.0/superwise_api/client/models/dashboard_item_update.py
--rw-r--r--   0        0        0     1910 2024-04-14 09:12:10.683520 superwise_api-1.3.0/superwise_api/client/models/dashboard_update.py
--rw-r--r--   0        0        0     4297 2024-04-14 09:12:10.683520 superwise_api-1.3.0/superwise_api/client/models/dataset_create.py
--rw-r--r--   0        0        0     4756 2024-04-14 09:12:10.683520 superwise_api-1.3.0/superwise_api/client/models/dataset_id.py
--rw-r--r--   0        0        0     3971 2024-04-14 09:12:10.683520 superwise_api-1.3.0/superwise_api/client/models/dataset_response.py
--rw-r--r--   0        0        0     4317 2024-04-14 09:12:10.683520 superwise_api-1.3.0/superwise_api/client/models/dataset_source_create.py
--rw-r--r--   0        0        0     2904 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/dataset_source_response.py
--rw-r--r--   0        0        0     3355 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/dataset_source_response_with_source.py
--rw-r--r--   0        0        0     2514 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/dataset_source_update.py
--rw-r--r--   0        0        0     1769 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/dataset_tag.py
--rw-r--r--   0        0        0     2632 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/dataset_update.py
--rw-r--r--   0        0        0      678 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/datasource.py
--rw-r--r--   0        0        0     6335 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/default_value.py
--rw-r--r--   0        0        0     6127 2024-04-14 09:12:10.684520 superwise_api-1.3.0/superwise_api/client/models/default_value1.py
--rw-r--r--   0        0        0     4776 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/description.py
--rw-r--r--   0        0        0     2113 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/destination_create_base.py
--rw-r--r--   0        0        0     2614 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/destination_response.py
--rw-r--r--   0        0        0     1963 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/destination_update_base.py
--rw-r--r--   0        0        0     5042 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/embedding_model.py
--rw-r--r--   0        0        0     2226 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/filter.py
--rw-r--r--   0        0        0     2384 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/gcp_credentials_request.py
--rw-r--r--   0        0        0     2369 2024-04-14 09:12:10.685520 superwise_api-1.3.0/superwise_api/client/models/gcp_credentials_response.py
--rw-r--r--   0        0        0      771 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/google_model_version.py
--rw-r--r--   0        0        0      770 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/granularity.py
--rw-r--r--   0        0        0     2375 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/http_validation_error.py
--rw-r--r--   0        0        0      674 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/ingest_type.py
--rw-r--r--   0        0        0     2478 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/integration_response.py
--rw-r--r--   0        0        0      670 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/integration_type.py
--rw-r--r--   0        0        0     2418 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/model_create.py
--rw-r--r--   0        0        0     4736 2024-04-14 09:12:10.686520 superwise_api-1.3.0/superwise_api/client/models/model_id.py
--rw-r--r--   0        0        0     2156 2024-04-14 09:12:10.687520 superwise_api-1.3.0/superwise_api/client/models/model_llm.py
--rw-r--r--   0        0        0      736 2024-04-14 09:12:10.687520 superwise_api-1.3.0/superwise_api/client/models/model_provider.py
--rw-r--r--   0        0        0     2788 2024-04-14 09:12:10.687520 superwise_api-1.3.0/superwise_api/client/models/model_response.py
--rw-r--r--   0        0        0     1802 2024-04-14 09:12:10.687520 superwise_api-1.3.0/superwise_api/client/models/model_schema.py
--rw-r--r--   0        0        0     5637 2024-04-14 09:12:10.687520 superwise_api-1.3.0/superwise_api/client/models/model_version.py
--rw-r--r--   0        0        0     5717 2024-04-14 09:12:10.687520 superwise_api-1.3.0/superwise_api/client/models/model_version_response.py
--rw-r--r--   0        0        0     4706 2024-04-14 09:12:10.688520 superwise_api-1.3.0/superwise_api/client/models/name.py
--rw-r--r--   0        0        0     1009 2024-04-14 09:12:10.688520 superwise_api-1.3.0/superwise_api/client/models/open_ai_model_version.py
--rw-r--r--   0        0        0     4697 2024-04-14 09:12:10.688520 superwise_api-1.3.0/superwise_api/client/models/order.py
--rw-r--r--   0        0        0     4786 2024-04-14 09:12:10.688520 superwise_api-1.3.0/superwise_api/client/models/order1.py
--rw-r--r--   0        0        0     4750 2024-04-14 09:12:10.688520 superwise_api-1.3.0/superwise_api/client/models/page.py
--rw-r--r--   0        0        0     3719 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_application.py
--rw-r--r--   0        0        0     3816 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_application_response.py
--rw-r--r--   0        0        0     3093 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_dashboard.py
--rw-r--r--   0        0        0     3142 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_dashboard_item.py
--rw-r--r--   0        0        0     3166 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_dataset_response.py
--rw-r--r--   0        0        0     3361 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_dataset_source_response_with_source.py
--rw-r--r--   0        0        0     3214 2024-04-14 09:12:10.689520 superwise_api-1.3.0/superwise_api/client/models/page_destination_response.py
--rw-r--r--   0        0        0     3214 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/page_integration_response.py
--rw-r--r--   0        0        0     3744 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/page_model_response.py
--rw-r--r--   0        0        0     3154 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/page_policy_response.py
--rw-r--r--   0        0        0     3154 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/page_source_response.py
--rw-r--r--   0        0        0     3732 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/page_tool_response.py
--rw-r--r--   0        0        0     4760 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/pages.py
--rw-r--r--   0        0        0     8597 2024-04-14 09:12:10.690520 superwise_api-1.3.0/superwise_api/client/models/payload.py
--rw-r--r--   0        0        0     4615 2024-04-14 09:12:10.691521 superwise_api-1.3.0/superwise_api/client/models/policy_create.py
--rw-r--r--   0        0        0     3876 2024-04-14 09:12:10.691521 superwise_api-1.3.0/superwise_api/client/models/policy_query.py
--rw-r--r--   0        0        0     2314 2024-04-14 09:12:10.691521 superwise_api-1.3.0/superwise_api/client/models/policy_query_filter.py
--rw-r--r--   0        0        0     1842 2024-04-14 09:12:10.691521 superwise_api-1.3.0/superwise_api/client/models/policy_query_order.py
--rw-r--r--   0        0        0     5592 2024-04-14 09:12:10.691521 superwise_api-1.3.0/superwise_api/client/models/policy_response.py
--rw-r--r--   0        0        0      740 2024-04-14 09:12:10.692521 superwise_api-1.3.0/superwise_api/client/models/policy_status.py
--rw-r--r--   0        0        0     4020 2024-04-14 09:12:10.692521 superwise_api-1.3.0/superwise_api/client/models/policy_update.py
--rw-r--r--   0        0        0     4726 2024-04-14 09:12:10.692521 superwise_api-1.3.0/superwise_api/client/models/prompt.py
--rw-r--r--   0        0        0     4746 2024-04-14 09:12:10.692521 superwise_api-1.3.0/superwise_api/client/models/provider.py
--rw-r--r--   0        0        0     3815 2024-04-14 09:12:10.692521 superwise_api-1.3.0/superwise_api/client/models/query.py
--rw-r--r--   0        0        0      748 2024-04-14 09:12:10.692521 superwise_api-1.3.0/superwise_api/client/models/query_type.py
--rw-r--r--   0        0        0      629 2024-04-14 09:12:10.693521 superwise_api-1.3.0/superwise_api/client/models/role.py
--rw-r--r--   0        0        0     2100 2024-04-14 09:12:10.693521 superwise_api-1.3.0/superwise_api/client/models/schema_item.py
--rw-r--r--   0        0        0     1810 2024-04-14 09:12:10.693521 superwise_api-1.3.0/superwise_api/client/models/schema_update.py
--rw-r--r--   0        0        0     2908 2024-04-14 09:12:10.693521 superwise_api-1.3.0/superwise_api/client/models/schema_update_item.py
--rw-r--r--   0        0        0     4750 2024-04-14 09:12:10.693521 superwise_api-1.3.0/superwise_api/client/models/size.py
--rw-r--r--   0        0        0     6051 2024-04-14 09:12:10.693521 superwise_api-1.3.0/superwise_api/client/models/source.py
--rw-r--r--   0        0        0     3409 2024-04-14 09:12:10.694521 superwise_api-1.3.0/superwise_api/client/models/source_azure_params.py
--rw-r--r--   0        0        0     5617 2024-04-14 09:12:10.694521 superwise_api-1.3.0/superwise_api/client/models/source_create.py
--rw-r--r--   0        0        0     4059 2024-04-14 09:12:10.694521 superwise_api-1.3.0/superwise_api/client/models/source_create_azure.py
--rw-r--r--   0        0        0     4001 2024-04-14 09:12:10.694521 superwise_api-1.3.0/superwise_api/client/models/source_create_gcs.py
--rw-r--r--   0        0        0     5687 2024-04-14 09:12:10.694521 superwise_api-1.3.0/superwise_api/client/models/source_create_payload.py
--rw-r--r--   0        0        0     3983 2024-04-14 09:12:10.695521 superwise_api-1.3.0/superwise_api/client/models/source_create_s3.py
--rw-r--r--   0        0        0     2781 2024-04-14 09:12:10.695521 superwise_api-1.3.0/superwise_api/client/models/source_gcs_params.py
--rw-r--r--   0        0        0     3533 2024-04-14 09:12:10.695521 superwise_api-1.3.0/superwise_api/client/models/source_get_azure.py
--rw-r--r--   0        0        0     3471 2024-04-14 09:12:10.695521 superwise_api-1.3.0/superwise_api/client/models/source_get_gcs.py
--rw-r--r--   0        0        0     3453 2024-04-14 09:12:10.695521 superwise_api-1.3.0/superwise_api/client/models/source_get_s3.py
--rw-r--r--   0        0        0     6147 2024-04-14 09:12:10.695521 superwise_api-1.3.0/superwise_api/client/models/source_response.py
--rw-r--r--   0        0        0     2815 2024-04-14 09:12:10.696521 superwise_api-1.3.0/superwise_api/client/models/source_s3_params.py
--rw-r--r--   0        0        0      706 2024-04-14 09:12:10.696521 superwise_api-1.3.0/superwise_api/client/models/source_type.py
--rw-r--r--   0        0        0     5595 2024-04-14 09:12:10.696521 superwise_api-1.3.0/superwise_api/client/models/source_update.py
--rw-r--r--   0        0        0     3143 2024-04-14 09:12:10.696521 superwise_api-1.3.0/superwise_api/client/models/source_update_gcs.py
--rw-r--r--   0        0        0     3127 2024-04-14 09:12:10.696521 superwise_api-1.3.0/superwise_api/client/models/source_update_s3.py
--rw-r--r--   0        0        0     1908 2024-04-14 09:12:10.696521 superwise_api-1.3.0/superwise_api/client/models/time_dimension.py
--rw-r--r--   0        0        0      736 2024-04-14 09:12:10.697521 superwise_api-1.3.0/superwise_api/client/models/time_range_unit.py
--rw-r--r--   0        0        0     9354 2024-04-14 09:12:10.697521 superwise_api-1.3.0/superwise_api/client/models/tool_config.py
--rw-r--r--   0        0        0     2339 2024-04-14 09:12:10.697521 superwise_api-1.3.0/superwise_api/client/models/tool_config_big_query.py
--rw-r--r--   0        0        0     2820 2024-04-14 09:12:10.697521 superwise_api-1.3.0/superwise_api/client/models/tool_config_pg_vector.py
--rw-r--r--   0        0        0     2181 2024-04-14 09:12:10.697521 superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database.py
--rw-r--r--   0        0        0     2563 2024-04-14 09:12:10.697521 superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_mssql.py
--rw-r--r--   0        0        0     2563 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_my_sql.py
--rw-r--r--   0        0        0     2573 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_oracle.py
--rw-r--r--   0        0        0     2597 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_postgres.py
--rw-r--r--   0        0        0     2648 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_create.py
--rw-r--r--   0        0        0     2439 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_def_input.py
--rw-r--r--   0        0        0     2636 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_def_output.py
--rw-r--r--   0        0        0     4813 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_name.py
--rw-r--r--   0        0        0     4873 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_name_update.py
--rw-r--r--   0        0        0     2911 2024-04-14 09:12:10.698521 superwise_api-1.3.0/superwise_api/client/models/tool_response.py
--rw-r--r--   0        0        0     4674 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/tool_type.py
--rw-r--r--   0        0        0     2863 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/tool_update.py
--rw-r--r--   0        0        0     4760 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/total.py
--rw-r--r--   0        0        0      720 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/type.py
--rw-r--r--   0        0        0     4820 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/updated_at.py
--rw-r--r--   0        0        0     2537 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/validation_error.py
--rw-r--r--   0        0        0     2013 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/validation_error_detail.py
--rw-r--r--   0        0        0     4912 2024-04-14 09:12:10.699521 superwise_api-1.3.0/superwise_api/client/models/validation_error_loc_inner.py
--rw-r--r--   0        0        0     2512 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/validation_result.py
--rw-r--r--   0        0        0     4726 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/values.py
--rw-r--r--   0        0        0     4736 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/version.py
--rw-r--r--   0        0        0     5597 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/version1.py
--rw-r--r--   0        0        0     2593 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/vertex_ai_model_garden_embedding_model.py
--rw-r--r--   0        0        0      794 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/visualization_type.py
--rw-r--r--   0        0        0     2355 2024-04-14 09:12:10.700521 superwise_api-1.3.0/superwise_api/client/models/widget_meta.py
--rw-r--r--   0        0        0    13894 2024-04-14 09:12:10.701521 superwise_api-1.3.0/superwise_api/client/rest.py
--rw-r--r--   0        0        0     1184 2024-04-14 09:12:10.701521 superwise_api-1.3.0/superwise_api/config.py
--rw-r--r--   0        0        0        0 2024-04-14 09:12:10.870538 superwise_api-1.3.0/superwise_api/entities/__init__.py
--rw-r--r--   0        0        0     3035 2024-04-14 09:12:10.701521 superwise_api-1.3.0/superwise_api/entities/application.py
--rw-r--r--   0        0        0     2991 2024-04-14 09:12:10.702522 superwise_api-1.3.0/superwise_api/entities/dashboard.py
--rw-r--r--   0        0        0     3222 2024-04-14 09:12:10.702522 superwise_api-1.3.0/superwise_api/entities/dashboard_item.py
--rw-r--r--   0        0        0     4004 2024-04-14 09:12:10.702522 superwise_api-1.3.0/superwise_api/entities/dataset.py
--rw-r--r--   0        0        0     3638 2024-04-14 09:12:10.702522 superwise_api-1.3.0/superwise_api/entities/dataset_source.py
--rw-r--r--   0        0        0     3035 2024-04-14 09:12:10.703522 superwise_api-1.3.0/superwise_api/entities/destination.py
--rw-r--r--   0        0        0     1549 2024-04-14 09:12:10.703522 superwise_api-1.3.0/superwise_api/entities/integration.py
--rw-r--r--   0        0        0     4797 2024-04-14 09:12:10.703522 superwise_api-1.3.0/superwise_api/entities/policy.py
--rw-r--r--   0        0        0     5410 2024-04-14 09:12:10.703522 superwise_api-1.3.0/superwise_api/entities/source.py
--rw-r--r--   0        0        0     1489 2024-04-14 09:12:10.703522 superwise_api-1.3.0/superwise_api/errors.py
--rw-r--r--   0        0        0     7125 2024-04-14 09:12:10.703522 superwise_api-1.3.0/superwise_api/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-14 09:12:10.871538 superwise_api-1.3.0/superwise_api/models/application/__init__.py
--rw-r--r--   0        0        0      686 2024-04-14 09:12:10.704522 superwise_api-1.3.0/superwise_api/models/application/enums.py
--rw-r--r--   0        0        0     3776 2024-04-14 09:12:10.704522 superwise_api-1.3.0/superwise_api/models/application/schemas.py
--rw-r--r--   0        0        0        0 2024-04-14 09:12:10.872538 superwise_api-1.3.0/superwise_api/models/dashboard/__init__.py
--rw-r--r--   0        0        0      838 2024-04-14 09:12:10.704522 superwise_api-1.3.0/superwise_api/models/dashboard/dashboard_response.py
--rw-r--r--   0        0        0     1261 2024-04-14 09:12:10.704522 superwise_api-1.3.0/superwise_api/models/dashboard/page_dashboard.py
--rw-r--r--   0        0        0        0 2024-04-14 09:12:10.873538 superwise_api-1.3.0/superwise_api/models/dashboard_item/__init__.py
--rw-r--r--   0        0        0     1333 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dashboard_item/dashboard_item.py
--rw-r--r--   0        0        0     1499 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dashboard_item/dashboard_item_create.py
--rw-r--r--   0        0        0     1280 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dashboard_item/dashboard_item_response.py
--rw-r--r--   0        0        0     1328 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dashboard_item/page_dashboard_item.py
--rw-r--r--   0        0        0     1308 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dashboard_item/query.py
--rw-r--r--   0        0        0      799 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dashboard_item/query_filter.py
--rw-r--r--   0        0        0     1131 2024-04-14 09:12:10.705522 superwise_api-1.3.0/superwise_api/models/dataset/__init__.py
--rw-r--r--   0        0        0     1439 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/dataset/dataset_response.py
--rw-r--r--   0        0        0      620 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/dataset/dataset_schema.py
--rw-r--r--   0        0        0      400 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/dataset/dataset_update.py
--rw-r--r--   0        0        0     1207 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/dataset/page_dataset_response.py
--rw-r--r--   0        0        0      688 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/policy/__init__.py
--rw-r--r--   0        0        0     1300 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/policy/page_policy_response.py
--rw-r--r--   0        0        0     1933 2024-04-14 09:12:10.706522 superwise_api-1.3.0/superwise_api/models/policy/policy_response.py
--rw-r--r--   0        0        0     3179 2024-04-14 09:12:10.707522 superwise_api-1.3.0/superwise_api/models/policy/query.py
--rw-r--r--   0        0        0      799 2024-04-14 09:12:10.707522 superwise_api-1.3.0/superwise_api/models/policy/query_filter.py
--rw-r--r--   0        0        0        0 2024-04-14 09:12:10.874538 superwise_api-1.3.0/superwise_api/models/tool/__init__.py
--rw-r--r--   0        0        0      749 2024-04-14 09:12:10.707522 superwise_api-1.3.0/superwise_api/models/tool/enums.py
--rw-r--r--   0        0        0     3208 2024-04-14 09:12:10.707522 superwise_api-1.3.0/superwise_api/models/tool/schemas.py
--rw-r--r--   0        0        0    10222 2024-04-14 09:12:10.707522 superwise_api-1.3.0/superwise_api/superwise_client.py
--rw-r--r--   0        0        0     1241 1970-01-01 00:00:00.000000 superwise_api-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      487 2024-05-09 12:24:47.589632 superwise_api-2.0.0/README.md
+-rw-r--r--   0        0        0      828 2024-05-09 12:25:00.541982 superwise_api-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      276 2024-05-09 12:24:47.616635 superwise_api-2.0.0/superwise_api/__init__.py
+-rw-r--r--   0        0        0     9994 2024-05-09 12:24:47.617635 superwise_api-2.0.0/superwise_api/client/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-09 12:24:47.617635 superwise_api-2.0.0/superwise_api/client/api/__init__.py
+-rw-r--r--   0        0        0    54744 2024-05-09 12:24:47.617635 superwise_api-2.0.0/superwise_api/client/api/applications_api.py
+-rw-r--r--   0        0        0    33591 2024-05-09 12:24:47.617635 superwise_api-2.0.0/superwise_api/client/api/dashboard_items_api.py
+-rw-r--r--   0        0        0    31775 2024-05-09 12:24:47.618636 superwise_api-2.0.0/superwise_api/client/api/dashboards_api.py
+-rw-r--r--   0        0        0    43860 2024-05-09 12:24:47.619636 superwise_api-2.0.0/superwise_api/client/api/dataset_api.py
+-rw-r--r--   0        0        0    38374 2024-05-09 12:24:47.619636 superwise_api-2.0.0/superwise_api/client/api/dataset_sources_api.py
+-rw-r--r--   0        0        0    36742 2024-05-09 12:24:47.619636 superwise_api-2.0.0/superwise_api/client/api/destinations_api.py
+-rw-r--r--   0        0        0    21619 2024-05-09 12:24:47.620636 superwise_api-2.0.0/superwise_api/client/api/integrations_api.py
+-rw-r--r--   0        0        0    44731 2024-05-09 12:24:47.620636 superwise_api-2.0.0/superwise_api/client/api/policies_api.py
+-rw-r--r--   0        0        0    38625 2024-05-09 12:24:47.620636 superwise_api-2.0.0/superwise_api/client/api/sources_api.py
+-rw-r--r--   0        0        0    28011 2024-05-09 12:24:47.621636 superwise_api-2.0.0/superwise_api/client/api_client.py
+-rw-r--r--   0        0        0      862 2024-05-09 12:24:47.621636 superwise_api-2.0.0/superwise_api/client/api_response.py
+-rw-r--r--   0        0        0    14478 2024-05-09 12:24:47.621636 superwise_api-2.0.0/superwise_api/client/configuration.py
+-rw-r--r--   0        0        0     5283 2024-05-09 12:24:47.621636 superwise_api-2.0.0/superwise_api/client/exceptions.py
+-rw-r--r--   0        0        0     8787 2024-05-09 12:24:47.622636 superwise_api-2.0.0/superwise_api/client/models/__init__.py
+-rw-r--r--   0        0        0      796 2024-05-09 12:24:47.622636 superwise_api-2.0.0/superwise_api/client/models/alert_on_status_direction.py
+-rw-r--r--   0        0        0     4546 2024-05-09 12:24:47.622636 superwise_api-2.0.0/superwise_api/client/models/application.py
+-rw-r--r--   0        0        0     3116 2024-05-09 12:24:47.622636 superwise_api-2.0.0/superwise_api/client/models/application_config.py
+-rw-r--r--   0        0        0     3299 2024-05-09 12:24:47.622636 superwise_api-2.0.0/superwise_api/client/models/application_config_payload.py
+-rw-r--r--   0        0        0     2634 2024-05-09 12:24:47.623636 superwise_api-2.0.0/superwise_api/client/models/application_create.py
+-rw-r--r--   0        0        0     4781 2024-05-09 12:24:47.623636 superwise_api-2.0.0/superwise_api/client/models/application_model.py
+-rw-r--r--   0        0        0     3046 2024-05-09 12:24:47.623636 superwise_api-2.0.0/superwise_api/client/models/application_response.py
+-rw-r--r--   0        0        0     4816 2024-05-09 12:24:47.623636 superwise_api-2.0.0/superwise_api/client/models/application_type.py
+-rw-r--r--   0        0        0     2816 2024-05-09 12:24:47.623636 superwise_api-2.0.0/superwise_api/client/models/application_update.py
+-rw-r--r--   0        0        0     2160 2024-05-09 12:24:47.623636 superwise_api-2.0.0/superwise_api/client/models/ask_config.py
+-rw-r--r--   0        0        0     3138 2024-05-09 12:24:47.624636 superwise_api-2.0.0/superwise_api/client/models/ask_request_payload.py
+-rw-r--r--   0        0        0     1837 2024-05-09 12:24:47.624636 superwise_api-2.0.0/superwise_api/client/models/ask_response_payload.py
+-rw-r--r--   0        0        0     2588 2024-05-09 12:24:47.624636 superwise_api-2.0.0/superwise_api/client/models/aws_credentials_request.py
+-rw-r--r--   0        0        0     2577 2024-05-09 12:24:47.624636 superwise_api-2.0.0/superwise_api/client/models/aws_credentials_response.py
+-rw-r--r--   0        0        0     2650 2024-05-09 12:24:47.624636 superwise_api-2.0.0/superwise_api/client/models/azure_credentials_request.py
+-rw-r--r--   0        0        0     2643 2024-05-09 12:24:47.624636 superwise_api-2.0.0/superwise_api/client/models/azure_credentials_response.py
+-rw-r--r--   0        0        0     1966 2024-05-09 12:24:47.625636 superwise_api-2.0.0/superwise_api/client/models/chat_history_entry.py
+-rw-r--r--   0        0        0     8587 2024-05-09 12:24:47.625636 superwise_api-2.0.0/superwise_api/client/models/config.py
+-rw-r--r--   0        0        0     5642 2024-05-09 12:24:47.625636 superwise_api-2.0.0/superwise_api/client/models/config1.py
+-rw-r--r--   0        0        0     4820 2024-05-09 12:24:47.625636 superwise_api-2.0.0/superwise_api/client/models/created_at.py
+-rw-r--r--   0        0        0     4756 2024-05-09 12:24:47.625636 superwise_api-2.0.0/superwise_api/client/models/created_by.py
+-rw-r--r--   0        0        0     2304 2024-05-09 12:24:47.625636 superwise_api-2.0.0/superwise_api/client/models/dashboard.py
+-rw-r--r--   0        0        0     1780 2024-05-09 12:24:47.625636 superwise_api-2.0.0/superwise_api/client/models/dashboard_create.py
+-rw-r--r--   0        0        0     3285 2024-05-09 12:24:47.625636 superwise_api-2.0.0/superwise_api/client/models/dashboard_item.py
+-rw-r--r--   0        0        0     3049 2024-05-09 12:24:47.626636 superwise_api-2.0.0/superwise_api/client/models/dashboard_item_create.py
+-rw-r--r--   0        0        0     3994 2024-05-09 12:24:47.626636 superwise_api-2.0.0/superwise_api/client/models/dashboard_item_query.py
+-rw-r--r--   0        0        0     4956 2024-05-09 12:24:47.626636 superwise_api-2.0.0/superwise_api/client/models/dashboard_item_query_order.py
+-rw-r--r--   0        0        0     2929 2024-05-09 12:24:47.626636 superwise_api-2.0.0/superwise_api/client/models/dashboard_item_update.py
+-rw-r--r--   0        0        0     1910 2024-05-09 12:24:47.626636 superwise_api-2.0.0/superwise_api/client/models/dashboard_update.py
+-rw-r--r--   0        0        0     4297 2024-05-09 12:24:47.626636 superwise_api-2.0.0/superwise_api/client/models/dataset_create.py
+-rw-r--r--   0        0        0     4756 2024-05-09 12:24:47.626636 superwise_api-2.0.0/superwise_api/client/models/dataset_id.py
+-rw-r--r--   0        0        0     3971 2024-05-09 12:24:47.626636 superwise_api-2.0.0/superwise_api/client/models/dataset_response.py
+-rw-r--r--   0        0        0     4317 2024-05-09 12:24:47.627637 superwise_api-2.0.0/superwise_api/client/models/dataset_source_create.py
+-rw-r--r--   0        0        0     2904 2024-05-09 12:24:47.627637 superwise_api-2.0.0/superwise_api/client/models/dataset_source_response.py
+-rw-r--r--   0        0        0     3355 2024-05-09 12:24:47.627637 superwise_api-2.0.0/superwise_api/client/models/dataset_source_response_with_source.py
+-rw-r--r--   0        0        0     2514 2024-05-09 12:24:47.627637 superwise_api-2.0.0/superwise_api/client/models/dataset_source_update.py
+-rw-r--r--   0        0        0     1769 2024-05-09 12:24:47.627637 superwise_api-2.0.0/superwise_api/client/models/dataset_tag.py
+-rw-r--r--   0        0        0     2632 2024-05-09 12:24:47.627637 superwise_api-2.0.0/superwise_api/client/models/dataset_update.py
+-rw-r--r--   0        0        0      678 2024-05-09 12:24:47.627637 superwise_api-2.0.0/superwise_api/client/models/datasource.py
+-rw-r--r--   0        0        0     6335 2024-05-09 12:24:47.627637 superwise_api-2.0.0/superwise_api/client/models/default_value.py
+-rw-r--r--   0        0        0     6127 2024-05-09 12:24:47.628636 superwise_api-2.0.0/superwise_api/client/models/default_value1.py
+-rw-r--r--   0        0        0     4776 2024-05-09 12:24:47.628636 superwise_api-2.0.0/superwise_api/client/models/description.py
+-rw-r--r--   0        0        0     2113 2024-05-09 12:24:47.628636 superwise_api-2.0.0/superwise_api/client/models/destination_create_base.py
+-rw-r--r--   0        0        0     2614 2024-05-09 12:24:47.628636 superwise_api-2.0.0/superwise_api/client/models/destination_response.py
+-rw-r--r--   0        0        0     1963 2024-05-09 12:24:47.628636 superwise_api-2.0.0/superwise_api/client/models/destination_update_base.py
+-rw-r--r--   0        0        0     5042 2024-05-09 12:24:47.628636 superwise_api-2.0.0/superwise_api/client/models/embedding_model.py
+-rw-r--r--   0        0        0     2226 2024-05-09 12:24:47.628636 superwise_api-2.0.0/superwise_api/client/models/filter.py
+-rw-r--r--   0        0        0     2384 2024-05-09 12:24:47.628636 superwise_api-2.0.0/superwise_api/client/models/gcp_credentials_request.py
+-rw-r--r--   0        0        0     2369 2024-05-09 12:24:47.629637 superwise_api-2.0.0/superwise_api/client/models/gcp_credentials_response.py
+-rw-r--r--   0        0        0      771 2024-05-09 12:24:47.629637 superwise_api-2.0.0/superwise_api/client/models/google_model_version.py
+-rw-r--r--   0        0        0      770 2024-05-09 12:24:47.629637 superwise_api-2.0.0/superwise_api/client/models/granularity.py
+-rw-r--r--   0        0        0     2375 2024-05-09 12:24:47.629637 superwise_api-2.0.0/superwise_api/client/models/http_validation_error.py
+-rw-r--r--   0        0        0      674 2024-05-09 12:24:47.629637 superwise_api-2.0.0/superwise_api/client/models/ingest_type.py
+-rw-r--r--   0        0        0     2478 2024-05-09 12:24:47.629637 superwise_api-2.0.0/superwise_api/client/models/integration_response.py
+-rw-r--r--   0        0        0      670 2024-05-09 12:24:47.630637 superwise_api-2.0.0/superwise_api/client/models/integration_type.py
+-rw-r--r--   0        0        0     2418 2024-05-09 12:24:47.630637 superwise_api-2.0.0/superwise_api/client/models/model_create.py
+-rw-r--r--   0        0        0     4736 2024-05-09 12:24:47.630637 superwise_api-2.0.0/superwise_api/client/models/model_id.py
+-rw-r--r--   0        0        0     2156 2024-05-09 12:24:47.630637 superwise_api-2.0.0/superwise_api/client/models/model_llm.py
+-rw-r--r--   0        0        0      736 2024-05-09 12:24:47.630637 superwise_api-2.0.0/superwise_api/client/models/model_provider.py
+-rw-r--r--   0        0        0     2788 2024-05-09 12:24:47.630637 superwise_api-2.0.0/superwise_api/client/models/model_response.py
+-rw-r--r--   0        0        0     1802 2024-05-09 12:24:47.630637 superwise_api-2.0.0/superwise_api/client/models/model_schema.py
+-rw-r--r--   0        0        0     5637 2024-05-09 12:24:47.631637 superwise_api-2.0.0/superwise_api/client/models/model_version.py
+-rw-r--r--   0        0        0     5717 2024-05-09 12:24:47.631637 superwise_api-2.0.0/superwise_api/client/models/model_version_response.py
+-rw-r--r--   0        0        0     4706 2024-05-09 12:24:47.631637 superwise_api-2.0.0/superwise_api/client/models/name.py
+-rw-r--r--   0        0        0     1009 2024-05-09 12:24:47.631637 superwise_api-2.0.0/superwise_api/client/models/open_ai_model_version.py
+-rw-r--r--   0        0        0     4697 2024-05-09 12:24:47.631637 superwise_api-2.0.0/superwise_api/client/models/order.py
+-rw-r--r--   0        0        0     4786 2024-05-09 12:24:47.631637 superwise_api-2.0.0/superwise_api/client/models/order1.py
+-rw-r--r--   0        0        0     4750 2024-05-09 12:24:47.632637 superwise_api-2.0.0/superwise_api/client/models/page.py
+-rw-r--r--   0        0        0     3719 2024-05-09 12:24:47.632637 superwise_api-2.0.0/superwise_api/client/models/page_application.py
+-rw-r--r--   0        0        0     3816 2024-05-09 12:24:47.632637 superwise_api-2.0.0/superwise_api/client/models/page_application_response.py
+-rw-r--r--   0        0        0     3093 2024-05-09 12:24:47.632637 superwise_api-2.0.0/superwise_api/client/models/page_dashboard.py
+-rw-r--r--   0        0        0     3142 2024-05-09 12:24:47.632637 superwise_api-2.0.0/superwise_api/client/models/page_dashboard_item.py
+-rw-r--r--   0        0        0     3166 2024-05-09 12:24:47.632637 superwise_api-2.0.0/superwise_api/client/models/page_dataset_response.py
+-rw-r--r--   0        0        0     3361 2024-05-09 12:24:47.633637 superwise_api-2.0.0/superwise_api/client/models/page_dataset_source_response_with_source.py
+-rw-r--r--   0        0        0     3214 2024-05-09 12:24:47.633637 superwise_api-2.0.0/superwise_api/client/models/page_destination_response.py
+-rw-r--r--   0        0        0     3214 2024-05-09 12:24:47.633637 superwise_api-2.0.0/superwise_api/client/models/page_integration_response.py
+-rw-r--r--   0        0        0     3744 2024-05-09 12:24:47.633637 superwise_api-2.0.0/superwise_api/client/models/page_model_response.py
+-rw-r--r--   0        0        0     3154 2024-05-09 12:24:47.633637 superwise_api-2.0.0/superwise_api/client/models/page_policy_response.py
+-rw-r--r--   0        0        0     3154 2024-05-09 12:24:47.633637 superwise_api-2.0.0/superwise_api/client/models/page_source_response.py
+-rw-r--r--   0        0        0     3732 2024-05-09 12:24:47.633637 superwise_api-2.0.0/superwise_api/client/models/page_tool_response.py
+-rw-r--r--   0        0        0     4760 2024-05-09 12:24:47.633637 superwise_api-2.0.0/superwise_api/client/models/pages.py
+-rw-r--r--   0        0        0     8597 2024-05-09 12:24:47.633637 superwise_api-2.0.0/superwise_api/client/models/payload.py
+-rw-r--r--   0        0        0     5796 2024-05-09 12:24:47.634637 superwise_api-2.0.0/superwise_api/client/models/policy_create.py
+-rw-r--r--   0        0        0     3876 2024-05-09 12:24:47.634637 superwise_api-2.0.0/superwise_api/client/models/policy_query.py
+-rw-r--r--   0        0        0     2314 2024-05-09 12:24:47.634637 superwise_api-2.0.0/superwise_api/client/models/policy_query_filter.py
+-rw-r--r--   0        0        0     1842 2024-05-09 12:24:47.634637 superwise_api-2.0.0/superwise_api/client/models/policy_query_order.py
+-rw-r--r--   0        0        0     5592 2024-05-09 12:24:47.634637 superwise_api-2.0.0/superwise_api/client/models/policy_response.py
+-rw-r--r--   0        0        0      740 2024-05-09 12:24:47.634637 superwise_api-2.0.0/superwise_api/client/models/policy_status.py
+-rw-r--r--   0        0        0     4020 2024-05-09 12:24:47.634637 superwise_api-2.0.0/superwise_api/client/models/policy_update.py
+-rw-r--r--   0        0        0     4726 2024-05-09 12:24:47.634637 superwise_api-2.0.0/superwise_api/client/models/prompt.py
+-rw-r--r--   0        0        0     4746 2024-05-09 12:24:47.635637 superwise_api-2.0.0/superwise_api/client/models/provider.py
+-rw-r--r--   0        0        0     3815 2024-05-09 12:24:47.635637 superwise_api-2.0.0/superwise_api/client/models/query.py
+-rw-r--r--   0        0        0      748 2024-05-09 12:24:47.635637 superwise_api-2.0.0/superwise_api/client/models/query_type.py
+-rw-r--r--   0        0        0      629 2024-05-09 12:24:47.635637 superwise_api-2.0.0/superwise_api/client/models/role.py
+-rw-r--r--   0        0        0     2100 2024-05-09 12:24:47.635637 superwise_api-2.0.0/superwise_api/client/models/schema_item.py
+-rw-r--r--   0        0        0     1810 2024-05-09 12:24:47.635637 superwise_api-2.0.0/superwise_api/client/models/schema_update.py
+-rw-r--r--   0        0        0     2908 2024-05-09 12:24:47.635637 superwise_api-2.0.0/superwise_api/client/models/schema_update_item.py
+-rw-r--r--   0        0        0     4750 2024-05-09 12:24:47.636637 superwise_api-2.0.0/superwise_api/client/models/size.py
+-rw-r--r--   0        0        0     6051 2024-05-09 12:24:47.636637 superwise_api-2.0.0/superwise_api/client/models/source.py
+-rw-r--r--   0        0        0     3409 2024-05-09 12:24:47.636637 superwise_api-2.0.0/superwise_api/client/models/source_azure_params.py
+-rw-r--r--   0        0        0     5617 2024-05-09 12:24:47.636637 superwise_api-2.0.0/superwise_api/client/models/source_create.py
+-rw-r--r--   0        0        0     4059 2024-05-09 12:24:47.636637 superwise_api-2.0.0/superwise_api/client/models/source_create_azure.py
+-rw-r--r--   0        0        0     4001 2024-05-09 12:24:47.636637 superwise_api-2.0.0/superwise_api/client/models/source_create_gcs.py
+-rw-r--r--   0        0        0     5687 2024-05-09 12:24:47.637637 superwise_api-2.0.0/superwise_api/client/models/source_create_payload.py
+-rw-r--r--   0        0        0     3983 2024-05-09 12:24:47.637637 superwise_api-2.0.0/superwise_api/client/models/source_create_s3.py
+-rw-r--r--   0        0        0     2781 2024-05-09 12:24:47.637637 superwise_api-2.0.0/superwise_api/client/models/source_gcs_params.py
+-rw-r--r--   0        0        0     3533 2024-05-09 12:24:47.637637 superwise_api-2.0.0/superwise_api/client/models/source_get_azure.py
+-rw-r--r--   0        0        0     3471 2024-05-09 12:24:47.637637 superwise_api-2.0.0/superwise_api/client/models/source_get_gcs.py
+-rw-r--r--   0        0        0     3453 2024-05-09 12:24:47.637637 superwise_api-2.0.0/superwise_api/client/models/source_get_s3.py
+-rw-r--r--   0        0        0     6147 2024-05-09 12:24:47.637637 superwise_api-2.0.0/superwise_api/client/models/source_response.py
+-rw-r--r--   0        0        0     2815 2024-05-09 12:24:47.637637 superwise_api-2.0.0/superwise_api/client/models/source_s3_params.py
+-rw-r--r--   0        0        0      706 2024-05-09 12:24:47.637637 superwise_api-2.0.0/superwise_api/client/models/source_type.py
+-rw-r--r--   0        0        0     5595 2024-05-09 12:24:47.638638 superwise_api-2.0.0/superwise_api/client/models/source_update.py
+-rw-r--r--   0        0        0     3143 2024-05-09 12:24:47.638638 superwise_api-2.0.0/superwise_api/client/models/source_update_gcs.py
+-rw-r--r--   0        0        0     3127 2024-05-09 12:24:47.638638 superwise_api-2.0.0/superwise_api/client/models/source_update_s3.py
+-rw-r--r--   0        0        0     1908 2024-05-09 12:24:47.638638 superwise_api-2.0.0/superwise_api/client/models/time_dimension.py
+-rw-r--r--   0        0        0      736 2024-05-09 12:24:47.638638 superwise_api-2.0.0/superwise_api/client/models/time_range_unit.py
+-rw-r--r--   0        0        0     9354 2024-05-09 12:24:47.638638 superwise_api-2.0.0/superwise_api/client/models/tool_config.py
+-rw-r--r--   0        0        0     2339 2024-05-09 12:24:47.639638 superwise_api-2.0.0/superwise_api/client/models/tool_config_big_query.py
+-rw-r--r--   0        0        0     2820 2024-05-09 12:24:47.639638 superwise_api-2.0.0/superwise_api/client/models/tool_config_pg_vector.py
+-rw-r--r--   0        0        0     2181 2024-05-09 12:24:47.639638 superwise_api-2.0.0/superwise_api/client/models/tool_config_sql_database.py
+-rw-r--r--   0        0        0     2563 2024-05-09 12:24:47.639638 superwise_api-2.0.0/superwise_api/client/models/tool_config_sql_database_mssql.py
+-rw-r--r--   0        0        0     2563 2024-05-09 12:24:47.639638 superwise_api-2.0.0/superwise_api/client/models/tool_config_sql_database_my_sql.py
+-rw-r--r--   0        0        0     2573 2024-05-09 12:24:47.639638 superwise_api-2.0.0/superwise_api/client/models/tool_config_sql_database_oracle.py
+-rw-r--r--   0        0        0     2597 2024-05-09 12:24:47.640638 superwise_api-2.0.0/superwise_api/client/models/tool_config_sql_database_postgres.py
+-rw-r--r--   0        0        0     2648 2024-05-09 12:24:47.640638 superwise_api-2.0.0/superwise_api/client/models/tool_create.py
+-rw-r--r--   0        0        0     2439 2024-05-09 12:24:47.640638 superwise_api-2.0.0/superwise_api/client/models/tool_def_input.py
+-rw-r--r--   0        0        0     2636 2024-05-09 12:24:47.640638 superwise_api-2.0.0/superwise_api/client/models/tool_def_output.py
+-rw-r--r--   0        0        0     4813 2024-05-09 12:24:47.640638 superwise_api-2.0.0/superwise_api/client/models/tool_name.py
+-rw-r--r--   0        0        0     4873 2024-05-09 12:24:47.640638 superwise_api-2.0.0/superwise_api/client/models/tool_name_update.py
+-rw-r--r--   0        0        0     2911 2024-05-09 12:24:47.640638 superwise_api-2.0.0/superwise_api/client/models/tool_response.py
+-rw-r--r--   0        0        0     4674 2024-05-09 12:24:47.641638 superwise_api-2.0.0/superwise_api/client/models/tool_type.py
+-rw-r--r--   0        0        0     2863 2024-05-09 12:24:47.641638 superwise_api-2.0.0/superwise_api/client/models/tool_update.py
+-rw-r--r--   0        0        0     4760 2024-05-09 12:24:47.641638 superwise_api-2.0.0/superwise_api/client/models/total.py
+-rw-r--r--   0        0        0      720 2024-05-09 12:24:47.641638 superwise_api-2.0.0/superwise_api/client/models/type.py
+-rw-r--r--   0        0        0     4820 2024-05-09 12:24:47.641638 superwise_api-2.0.0/superwise_api/client/models/updated_at.py
+-rw-r--r--   0        0        0     2537 2024-05-09 12:24:47.641638 superwise_api-2.0.0/superwise_api/client/models/validation_error.py
+-rw-r--r--   0        0        0     2013 2024-05-09 12:24:47.641638 superwise_api-2.0.0/superwise_api/client/models/validation_error_detail.py
+-rw-r--r--   0        0        0     4912 2024-05-09 12:24:47.641638 superwise_api-2.0.0/superwise_api/client/models/validation_error_loc_inner.py
+-rw-r--r--   0        0        0     2512 2024-05-09 12:24:47.642638 superwise_api-2.0.0/superwise_api/client/models/validation_result.py
+-rw-r--r--   0        0        0     4726 2024-05-09 12:24:47.642638 superwise_api-2.0.0/superwise_api/client/models/values.py
+-rw-r--r--   0        0        0     4736 2024-05-09 12:24:47.642638 superwise_api-2.0.0/superwise_api/client/models/version.py
+-rw-r--r--   0        0        0     5597 2024-05-09 12:24:47.642638 superwise_api-2.0.0/superwise_api/client/models/version1.py
+-rw-r--r--   0        0        0     2593 2024-05-09 12:24:47.642638 superwise_api-2.0.0/superwise_api/client/models/vertex_ai_model_garden_embedding_model.py
+-rw-r--r--   0        0        0      794 2024-05-09 12:24:47.642638 superwise_api-2.0.0/superwise_api/client/models/visualization_type.py
+-rw-r--r--   0        0        0     2355 2024-05-09 12:24:47.642638 superwise_api-2.0.0/superwise_api/client/models/widget_meta.py
+-rw-r--r--   0        0        0    13894 2024-05-09 12:24:47.643638 superwise_api-2.0.0/superwise_api/client/rest.py
+-rw-r--r--   0        0        0     1184 2024-05-09 12:24:47.643638 superwise_api-2.0.0/superwise_api/config.py
+-rw-r--r--   0        0        0        0 2024-05-09 12:24:47.751649 superwise_api-2.0.0/superwise_api/entities/__init__.py
+-rw-r--r--   0        0        0     3045 2024-05-09 12:24:47.643638 superwise_api-2.0.0/superwise_api/entities/application.py
+-rw-r--r--   0        0        0     2991 2024-05-09 12:24:47.643638 superwise_api-2.0.0/superwise_api/entities/dashboard.py
+-rw-r--r--   0        0        0     3222 2024-05-09 12:24:47.643638 superwise_api-2.0.0/superwise_api/entities/dashboard_item.py
+-rw-r--r--   0        0        0     4004 2024-05-09 12:24:47.643638 superwise_api-2.0.0/superwise_api/entities/dataset.py
+-rw-r--r--   0        0        0     3638 2024-05-09 12:24:47.643638 superwise_api-2.0.0/superwise_api/entities/dataset_source.py
+-rw-r--r--   0        0        0     3035 2024-05-09 12:24:47.643638 superwise_api-2.0.0/superwise_api/entities/destination.py
+-rw-r--r--   0        0        0     1549 2024-05-09 12:24:47.644638 superwise_api-2.0.0/superwise_api/entities/integration.py
+-rw-r--r--   0        0        0     4797 2024-05-09 12:24:47.644638 superwise_api-2.0.0/superwise_api/entities/policy.py
+-rw-r--r--   0        0        0     5410 2024-05-09 12:24:47.644638 superwise_api-2.0.0/superwise_api/entities/source.py
+-rw-r--r--   0        0        0     1489 2024-05-09 12:24:47.644638 superwise_api-2.0.0/superwise_api/errors.py
+-rw-r--r--   0        0        0     7125 2024-05-09 12:24:47.644638 superwise_api-2.0.0/superwise_api/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 12:24:47.752649 superwise_api-2.0.0/superwise_api/models/application/__init__.py
+-rw-r--r--   0        0        0      686 2024-05-09 12:24:47.644638 superwise_api-2.0.0/superwise_api/models/application/enums.py
+-rw-r--r--   0        0        0     3776 2024-05-09 12:24:47.644638 superwise_api-2.0.0/superwise_api/models/application/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-09 12:24:47.752649 superwise_api-2.0.0/superwise_api/models/dashboard/__init__.py
+-rw-r--r--   0        0        0      838 2024-05-09 12:24:47.645638 superwise_api-2.0.0/superwise_api/models/dashboard/dashboard_response.py
+-rw-r--r--   0        0        0     1261 2024-05-09 12:24:47.645638 superwise_api-2.0.0/superwise_api/models/dashboard/page_dashboard.py
+-rw-r--r--   0        0        0        0 2024-05-09 12:24:47.752649 superwise_api-2.0.0/superwise_api/models/dashboard_item/__init__.py
+-rw-r--r--   0        0        0     1333 2024-05-09 12:24:47.645638 superwise_api-2.0.0/superwise_api/models/dashboard_item/dashboard_item.py
+-rw-r--r--   0        0        0     1499 2024-05-09 12:24:47.645638 superwise_api-2.0.0/superwise_api/models/dashboard_item/dashboard_item_create.py
+-rw-r--r--   0        0        0     1280 2024-05-09 12:24:47.645638 superwise_api-2.0.0/superwise_api/models/dashboard_item/dashboard_item_response.py
+-rw-r--r--   0        0        0     1328 2024-05-09 12:24:47.645638 superwise_api-2.0.0/superwise_api/models/dashboard_item/page_dashboard_item.py
+-rw-r--r--   0        0        0     1308 2024-05-09 12:24:47.645638 superwise_api-2.0.0/superwise_api/models/dashboard_item/query.py
+-rw-r--r--   0        0        0      799 2024-05-09 12:24:47.646638 superwise_api-2.0.0/superwise_api/models/dashboard_item/query_filter.py
+-rw-r--r--   0        0        0     1131 2024-05-09 12:24:47.646638 superwise_api-2.0.0/superwise_api/models/dataset/__init__.py
+-rw-r--r--   0        0        0     1439 2024-05-09 12:24:47.646638 superwise_api-2.0.0/superwise_api/models/dataset/dataset_response.py
+-rw-r--r--   0        0        0      620 2024-05-09 12:24:47.646638 superwise_api-2.0.0/superwise_api/models/dataset/dataset_schema.py
+-rw-r--r--   0        0        0      400 2024-05-09 12:24:47.646638 superwise_api-2.0.0/superwise_api/models/dataset/dataset_update.py
+-rw-r--r--   0        0        0     1207 2024-05-09 12:24:47.646638 superwise_api-2.0.0/superwise_api/models/dataset/page_dataset_response.py
+-rw-r--r--   0        0        0      688 2024-05-09 12:24:47.646638 superwise_api-2.0.0/superwise_api/models/policy/__init__.py
+-rw-r--r--   0        0        0     1300 2024-05-09 12:24:47.646638 superwise_api-2.0.0/superwise_api/models/policy/page_policy_response.py
+-rw-r--r--   0        0        0     1933 2024-05-09 12:24:47.647638 superwise_api-2.0.0/superwise_api/models/policy/policy_response.py
+-rw-r--r--   0        0        0     3179 2024-05-09 12:24:47.647638 superwise_api-2.0.0/superwise_api/models/policy/query.py
+-rw-r--r--   0        0        0      799 2024-05-09 12:24:47.647638 superwise_api-2.0.0/superwise_api/models/policy/query_filter.py
+-rw-r--r--   0        0        0        0 2024-05-09 12:24:47.753650 superwise_api-2.0.0/superwise_api/models/tool/__init__.py
+-rw-r--r--   0        0        0      773 2024-05-09 12:24:47.647638 superwise_api-2.0.0/superwise_api/models/tool/enums.py
+-rw-r--r--   0        0        0     3591 2024-05-09 12:24:47.647638 superwise_api-2.0.0/superwise_api/models/tool/schemas.py
+-rw-r--r--   0        0        0    10232 2024-05-09 12:24:47.647638 superwise_api-2.0.0/superwise_api/superwise_client.py
+-rw-r--r--   0        0        0     1241 1970-01-01 00:00:00.000000 superwise_api-2.0.0/PKG-INFO
```

### Comparing `superwise_api-1.3.0/pyproject.toml` & `superwise_api-2.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "superwise-api"
 packages = [{include = "superwise_api", from = "."}]
-version = "1.3.0"
+version = "2.0.0"
 description = "Superwise SDK for Python"
 authors = ["Superwise"]
 license = "MIT"
 readme = "README.md"
 keywords = ["OpenAPI", "SuperwiseSDK"]
 include = ["superwise_api/client/py.typed"]
```

### Comparing `superwise_api-1.3.0/superwise_api/client/__init__.py` & `superwise_api-2.0.0/superwise_api/client/__init__.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/api/__init__.py` & `superwise_api-2.0.0/superwise_api/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/api/applications_api.py` & `superwise_api-2.0.0/superwise_api/client/api/applications_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         _response_types_map = {
             "200": "object",
             "422": None,
             "500": None,
         }
 
         return self.api_client.call_api(
-            "/v1/applications/ask",
+            "/v1/application-playground/ask",
             "POST",
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
```

### Comparing `superwise_api-1.3.0/superwise_api/client/api/dashboard_items_api.py` & `superwise_api-2.0.0/superwise_api/client/api/dashboard_items_api.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/api/dashboards_api.py` & `superwise_api-2.0.0/superwise_api/client/api/dashboards_api.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/api/dataset_api.py` & `superwise_api-2.0.0/superwise_api/client/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/api/dataset_sources_api.py` & `superwise_api-2.0.0/superwise_api/client/api/dataset_sources_api.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/api/destinations_api.py` & `superwise_api-2.0.0/superwise_api/client/api/destinations_api.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/api/integrations_api.py` & `superwise_api-2.0.0/superwise_api/client/api/integrations_api.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/api/policies_api.py` & `superwise_api-2.0.0/superwise_api/client/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/api/sources_api.py` & `superwise_api-2.0.0/superwise_api/client/api/sources_api.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/api_client.py` & `superwise_api-2.0.0/superwise_api/client/api_client.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/api_response.py` & `superwise_api-2.0.0/superwise_api/client/api_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/configuration.py` & `superwise_api-2.0.0/superwise_api/client/configuration.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/exceptions.py` & `superwise_api-2.0.0/superwise_api/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/__init__.py` & `superwise_api-2.0.0/superwise_api/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/alert_on_status_direction.py` & `superwise_api-2.0.0/superwise_api/client/models/alert_on_status_direction.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/application.py` & `superwise_api-2.0.0/superwise_api/client/models/application.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/application_config.py` & `superwise_api-2.0.0/superwise_api/client/models/application_config.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/application_config_payload.py` & `superwise_api-2.0.0/superwise_api/client/models/application_config_payload.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/application_create.py` & `superwise_api-2.0.0/superwise_api/client/models/application_create.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/application_model.py` & `superwise_api-2.0.0/superwise_api/client/models/application_model.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/application_response.py` & `superwise_api-2.0.0/superwise_api/client/models/application_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/application_type.py` & `superwise_api-2.0.0/superwise_api/client/models/application_type.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/application_update.py` & `superwise_api-2.0.0/superwise_api/client/models/application_update.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/ask_config.py` & `superwise_api-2.0.0/superwise_api/client/models/ask_config.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/ask_request_payload.py` & `superwise_api-2.0.0/superwise_api/client/models/ask_request_payload.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/ask_response_payload.py` & `superwise_api-2.0.0/superwise_api/client/models/ask_response_payload.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/aws_credentials_request.py` & `superwise_api-2.0.0/superwise_api/client/models/aws_credentials_request.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/aws_credentials_response.py` & `superwise_api-2.0.0/superwise_api/client/models/aws_credentials_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/azure_credentials_request.py` & `superwise_api-2.0.0/superwise_api/client/models/azure_credentials_request.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/azure_credentials_response.py` & `superwise_api-2.0.0/superwise_api/client/models/azure_credentials_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/chat_history_entry.py` & `superwise_api-2.0.0/superwise_api/client/models/chat_history_entry.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/config.py` & `superwise_api-2.0.0/superwise_api/client/models/config.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/config1.py` & `superwise_api-2.0.0/superwise_api/client/models/config1.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/created_at.py` & `superwise_api-2.0.0/superwise_api/client/models/created_at.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/created_by.py` & `superwise_api-2.0.0/superwise_api/client/models/created_by.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dashboard.py` & `superwise_api-2.0.0/superwise_api/client/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dashboard_create.py` & `superwise_api-2.0.0/superwise_api/client/models/dashboard_create.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dashboard_item.py` & `superwise_api-2.0.0/superwise_api/client/models/dashboard_item.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dashboard_item_create.py` & `superwise_api-2.0.0/superwise_api/client/models/dashboard_item_create.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dashboard_item_query.py` & `superwise_api-2.0.0/superwise_api/client/models/dashboard_item_query.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dashboard_item_query_order.py` & `superwise_api-2.0.0/superwise_api/client/models/dashboard_item_query_order.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dashboard_item_update.py` & `superwise_api-2.0.0/superwise_api/client/models/dashboard_item_update.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dashboard_update.py` & `superwise_api-2.0.0/superwise_api/client/models/dashboard_update.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dataset_create.py` & `superwise_api-2.0.0/superwise_api/client/models/dataset_create.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dataset_id.py` & `superwise_api-2.0.0/superwise_api/client/models/dataset_id.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dataset_response.py` & `superwise_api-2.0.0/superwise_api/client/models/dataset_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dataset_source_create.py` & `superwise_api-2.0.0/superwise_api/client/models/dataset_source_create.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dataset_source_response.py` & `superwise_api-2.0.0/superwise_api/client/models/dataset_source_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dataset_source_response_with_source.py` & `superwise_api-2.0.0/superwise_api/client/models/dataset_source_response_with_source.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dataset_source_update.py` & `superwise_api-2.0.0/superwise_api/client/models/dataset_source_update.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dataset_tag.py` & `superwise_api-2.0.0/superwise_api/client/models/dataset_tag.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/dataset_update.py` & `superwise_api-2.0.0/superwise_api/client/models/dataset_update.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/datasource.py` & `superwise_api-2.0.0/superwise_api/client/models/datasource.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/default_value.py` & `superwise_api-2.0.0/superwise_api/client/models/default_value.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/default_value1.py` & `superwise_api-2.0.0/superwise_api/client/models/default_value1.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/description.py` & `superwise_api-2.0.0/superwise_api/client/models/description.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/destination_create_base.py` & `superwise_api-2.0.0/superwise_api/client/models/destination_create_base.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/destination_response.py` & `superwise_api-2.0.0/superwise_api/client/models/destination_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/destination_update_base.py` & `superwise_api-2.0.0/superwise_api/client/models/destination_update_base.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/embedding_model.py` & `superwise_api-2.0.0/superwise_api/client/models/embedding_model.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/filter.py` & `superwise_api-2.0.0/superwise_api/client/models/filter.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/gcp_credentials_request.py` & `superwise_api-2.0.0/superwise_api/client/models/gcp_credentials_request.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/gcp_credentials_response.py` & `superwise_api-2.0.0/superwise_api/client/models/gcp_credentials_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/google_model_version.py` & `superwise_api-2.0.0/superwise_api/client/models/google_model_version.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/granularity.py` & `superwise_api-2.0.0/superwise_api/client/models/granularity.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/http_validation_error.py` & `superwise_api-2.0.0/superwise_api/client/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/ingest_type.py` & `superwise_api-2.0.0/superwise_api/client/models/ingest_type.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/integration_response.py` & `superwise_api-2.0.0/superwise_api/client/models/integration_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/integration_type.py` & `superwise_api-2.0.0/superwise_api/client/models/integration_type.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/model_create.py` & `superwise_api-2.0.0/superwise_api/client/models/model_create.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/model_id.py` & `superwise_api-2.0.0/superwise_api/client/models/model_id.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/model_llm.py` & `superwise_api-2.0.0/superwise_api/client/models/model_llm.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/model_provider.py` & `superwise_api-2.0.0/superwise_api/client/models/model_provider.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/model_response.py` & `superwise_api-2.0.0/superwise_api/client/models/model_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/model_schema.py` & `superwise_api-2.0.0/superwise_api/client/models/model_schema.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/model_version.py` & `superwise_api-2.0.0/superwise_api/client/models/model_version.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/model_version_response.py` & `superwise_api-2.0.0/superwise_api/client/models/model_version_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/name.py` & `superwise_api-2.0.0/superwise_api/client/models/name.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/open_ai_model_version.py` & `superwise_api-2.0.0/superwise_api/client/models/open_ai_model_version.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/order.py` & `superwise_api-2.0.0/superwise_api/client/models/order.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/order1.py` & `superwise_api-2.0.0/superwise_api/client/models/order1.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page.py` & `superwise_api-2.0.0/superwise_api/client/models/page.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page_application.py` & `superwise_api-2.0.0/superwise_api/client/models/page_application.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page_application_response.py` & `superwise_api-2.0.0/superwise_api/client/models/page_application_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page_dashboard.py` & `superwise_api-2.0.0/superwise_api/client/models/page_dashboard.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page_dashboard_item.py` & `superwise_api-2.0.0/superwise_api/client/models/page_dashboard_item.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page_dataset_response.py` & `superwise_api-2.0.0/superwise_api/client/models/page_dataset_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page_dataset_source_response_with_source.py` & `superwise_api-2.0.0/superwise_api/client/models/page_dataset_source_response_with_source.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page_destination_response.py` & `superwise_api-2.0.0/superwise_api/client/models/page_destination_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page_integration_response.py` & `superwise_api-2.0.0/superwise_api/client/models/page_integration_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page_model_response.py` & `superwise_api-2.0.0/superwise_api/client/models/page_model_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page_policy_response.py` & `superwise_api-2.0.0/superwise_api/client/models/page_policy_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page_source_response.py` & `superwise_api-2.0.0/superwise_api/client/models/page_source_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/page_tool_response.py` & `superwise_api-2.0.0/superwise_api/client/models/page_tool_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/pages.py` & `superwise_api-2.0.0/superwise_api/client/models/pages.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/payload.py` & `superwise_api-2.0.0/superwise_api/client/models/payload.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/policy_create.py` & `superwise_api-2.0.0/superwise_api/client/models/policy_create.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,41 +10,63 @@
     Do not edit the class manually.
 """  # noqa: E501
 from __future__ import annotations
 
 import json
 import pprint
 import re  # noqa: F401
-from typing import List
+from enum import Enum
+from typing import Literal
 from typing import Optional
 from typing import Union
 
 from pydantic import BaseModel
 from pydantic import conlist
 from pydantic import Field
+from pydantic import PositiveFloat
+from pydantic import PositiveInt
 from pydantic import StrictBool
-from pydantic import StrictFloat
 from pydantic import StrictInt
 from pydantic import StrictStr
 
 from superwise_api.client.models.alert_on_status_direction import AlertOnStatusDirection
 from superwise_api.client.models.policy_query import PolicyQuery
 from superwise_api.client.models.time_range_unit import TimeRangeUnit
 
 
+class ThresholdTypes(str, Enum):
+    STATIC: Literal["static"] = "static"
+    MOVING_AVERAGE: Literal["moving_average"] = "moving_average"
+
+
+class StaticThresholdSettings(BaseModel):
+    condition_above_value: Optional[float] = Field(description="Condition above value")
+    condition_below_value: Optional[float] = Field(description="Condition below value")
+    threshold_type: Literal["static"] = ThresholdTypes.STATIC.value
+
+
+class MovingAverageThresholdSettings(BaseModel):
+    is_violation_above: bool = True
+    is_violation_below: bool = True
+    violation_deviation: PositiveFloat
+    threshold_type: Literal["moving_average"] = ThresholdTypes.MOVING_AVERAGE.value
+    window_size: PositiveInt
+
+
 class PolicyCreate(BaseModel):
     """
     PolicyCreate
     """
 
     name: StrictStr = Field(..., description="A descriptive name for this policy")
     query: PolicyQuery = Field(..., description="Cube.js query")
     cron_expression: StrictStr = Field(..., description="Cron expression for policy evaluation")
-    condition_above_value: Optional[Union[StrictFloat, StrictInt]] = Field(None, description="Condition above value")
-    condition_below_value: Optional[Union[StrictFloat, StrictInt]] = Field(None, description="Condition below value")
+    threshold_settings: Union[StaticThresholdSettings, MovingAverageThresholdSettings] = Field(
+        discriminator="threshold_type"
+    )
     destination_ids: conlist(StrictStr) = Field(
         ..., description="List of communication channels to get notified through"
     )
     alert_on_status: AlertOnStatusDirection = Field(
         ..., description="Trigger policy action if the value is above/below"
     )
     alert_on_policy_level: StrictBool = Field(..., description="Trigger policy action on a single group/entire groups")
@@ -52,16 +74,15 @@
     time_range_field: StrictStr = Field(..., description="Time feature to scan")
     time_range_unit: TimeRangeUnit = Field(..., description="Time unit to scan")
     time_range_value: StrictInt = Field(..., description="Time value to scan")
     __properties = [
         "name",
         "query",
         "cron_expression",
-        "condition_above_value",
-        "condition_below_value",
+        "threshold_settings",
         "destination_ids",
         "alert_on_status",
         "alert_on_policy_level",
         "dataset_id",
         "time_range_field",
         "time_range_unit",
         "time_range_value",
@@ -99,21 +120,31 @@
         """Create an instance of PolicyCreate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return PolicyCreate.parse_obj(obj)
 
+        threshold_settings = obj.get("threshold_settings")
+        if threshold_settings is not None:
+            if threshold_settings.get("threshold_type") == ThresholdTypes.STATIC.value:
+                _threshold_settings = StaticThresholdSettings.parse_obj(threshold_settings)
+            elif threshold_settings.get("threshold_type") == ThresholdTypes.MOVING_AVERAGE.value:
+                _threshold_settings = MovingAverageThresholdSettings.parse_obj(threshold_settings)
+            else:
+                raise ValueError("Invalid value for threshold_settings.threshold_type")
+        else:
+            _threshold_settings = None
+
         _obj = PolicyCreate.parse_obj(
             {
                 "name": obj.get("name"),
                 "query": PolicyQuery.from_dict(obj.get("query")) if obj.get("query") is not None else None,
                 "cron_expression": obj.get("cron_expression"),
-                "condition_above_value": obj.get("condition_above_value"),
-                "condition_below_value": obj.get("condition_below_value"),
+                "threshold_settings": _threshold_settings,
                 "destination_ids": obj.get("destination_ids"),
                 "alert_on_status": obj.get("alert_on_status"),
                 "alert_on_policy_level": obj.get("alert_on_policy_level"),
                 "dataset_id": obj.get("dataset_id"),
                 "time_range_field": obj.get("time_range_field"),
                 "time_range_unit": obj.get("time_range_unit"),
                 "time_range_value": obj.get("time_range_value"),
```

### Comparing `superwise_api-1.3.0/superwise_api/client/models/policy_query.py` & `superwise_api-2.0.0/superwise_api/client/models/policy_query.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/policy_query_filter.py` & `superwise_api-2.0.0/superwise_api/client/models/policy_query_filter.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/policy_query_order.py` & `superwise_api-2.0.0/superwise_api/client/models/policy_query_order.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/policy_response.py` & `superwise_api-2.0.0/superwise_api/client/models/policy_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/policy_status.py` & `superwise_api-2.0.0/superwise_api/client/models/policy_status.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/policy_update.py` & `superwise_api-2.0.0/superwise_api/client/models/policy_update.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/prompt.py` & `superwise_api-2.0.0/superwise_api/client/models/prompt.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/provider.py` & `superwise_api-2.0.0/superwise_api/client/models/provider.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/query.py` & `superwise_api-2.0.0/superwise_api/client/models/query.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/query_type.py` & `superwise_api-2.0.0/superwise_api/client/models/query_type.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/role.py` & `superwise_api-2.0.0/superwise_api/client/models/role.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/schema_item.py` & `superwise_api-2.0.0/superwise_api/client/models/schema_item.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/schema_update.py` & `superwise_api-2.0.0/superwise_api/client/models/schema_update.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/schema_update_item.py` & `superwise_api-2.0.0/superwise_api/client/models/schema_update_item.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/size.py` & `superwise_api-2.0.0/superwise_api/client/models/size.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source.py` & `superwise_api-2.0.0/superwise_api/client/models/source.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_azure_params.py` & `superwise_api-2.0.0/superwise_api/client/models/source_azure_params.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_create.py` & `superwise_api-2.0.0/superwise_api/client/models/source_create.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_create_azure.py` & `superwise_api-2.0.0/superwise_api/client/models/source_create_azure.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_create_gcs.py` & `superwise_api-2.0.0/superwise_api/client/models/source_create_gcs.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_create_payload.py` & `superwise_api-2.0.0/superwise_api/client/models/source_create_payload.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_create_s3.py` & `superwise_api-2.0.0/superwise_api/client/models/source_create_s3.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_gcs_params.py` & `superwise_api-2.0.0/superwise_api/client/models/source_gcs_params.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_get_azure.py` & `superwise_api-2.0.0/superwise_api/client/models/source_get_azure.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_get_gcs.py` & `superwise_api-2.0.0/superwise_api/client/models/source_get_gcs.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_get_s3.py` & `superwise_api-2.0.0/superwise_api/client/models/source_get_s3.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_response.py` & `superwise_api-2.0.0/superwise_api/client/models/source_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_s3_params.py` & `superwise_api-2.0.0/superwise_api/client/models/source_s3_params.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_type.py` & `superwise_api-2.0.0/superwise_api/client/models/source_type.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_update.py` & `superwise_api-2.0.0/superwise_api/client/models/source_update.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_update_gcs.py` & `superwise_api-2.0.0/superwise_api/client/models/source_update_gcs.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/source_update_s3.py` & `superwise_api-2.0.0/superwise_api/client/models/source_update_s3.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/time_dimension.py` & `superwise_api-2.0.0/superwise_api/client/models/time_dimension.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/time_range_unit.py` & `superwise_api-2.0.0/superwise_api/client/models/time_range_unit.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_config.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_config.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_config_big_query.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_config_big_query.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_config_pg_vector.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_config_pg_vector.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_config_sql_database.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_mssql.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_config_sql_database_mssql.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_my_sql.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_config_sql_database_my_sql.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_oracle.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_config_sql_database_oracle.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_config_sql_database_postgres.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_config_sql_database_postgres.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_create.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_create.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_def_input.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_def_input.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_def_output.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_def_output.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_name.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_name.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_name_update.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_name_update.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_response.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_type.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_type.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/tool_update.py` & `superwise_api-2.0.0/superwise_api/client/models/tool_update.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/total.py` & `superwise_api-2.0.0/superwise_api/client/models/total.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/type.py` & `superwise_api-2.0.0/superwise_api/client/models/type.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/updated_at.py` & `superwise_api-2.0.0/superwise_api/client/models/updated_at.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/validation_error.py` & `superwise_api-2.0.0/superwise_api/client/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/validation_error_detail.py` & `superwise_api-2.0.0/superwise_api/client/models/validation_error_detail.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/validation_error_loc_inner.py` & `superwise_api-2.0.0/superwise_api/client/models/validation_error_loc_inner.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/validation_result.py` & `superwise_api-2.0.0/superwise_api/client/models/validation_result.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/values.py` & `superwise_api-2.0.0/superwise_api/client/models/values.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/version.py` & `superwise_api-2.0.0/superwise_api/client/models/version.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/version1.py` & `superwise_api-2.0.0/superwise_api/client/models/version1.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/vertex_ai_model_garden_embedding_model.py` & `superwise_api-2.0.0/superwise_api/client/models/vertex_ai_model_garden_embedding_model.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/visualization_type.py` & `superwise_api-2.0.0/superwise_api/client/models/visualization_type.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/models/widget_meta.py` & `superwise_api-2.0.0/superwise_api/client/models/widget_meta.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/client/rest.py` & `superwise_api-2.0.0/superwise_api/client/rest.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/config.py` & `superwise_api-2.0.0/superwise_api/config.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/entities/application.py` & `superwise_api-2.0.0/superwise_api/entities/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from superwise_api.models.application.schemas import ModelLLM
 
 
 class Application:
     """
     Method | HTTP request | Description
     ------------- | ------------- | -------------
-    **ask** | **POST** /v1/applications/ask | Ask
+    **ask** | **POST** /v1/application-playground/ask | Ask
     **create_application** | **POST** /v1/applications | Create Application
     """
 
     def __init__(self, client):
         self.api = ApplicationsApi(client)
 
     @raise_exception
```

### Comparing `superwise_api-1.3.0/superwise_api/entities/dashboard.py` & `superwise_api-2.0.0/superwise_api/entities/dashboard.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/entities/dashboard_item.py` & `superwise_api-2.0.0/superwise_api/entities/dashboard_item.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/entities/dataset.py` & `superwise_api-2.0.0/superwise_api/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/entities/dataset_source.py` & `superwise_api-2.0.0/superwise_api/entities/dataset_source.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/entities/destination.py` & `superwise_api-2.0.0/superwise_api/entities/destination.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/entities/integration.py` & `superwise_api-2.0.0/superwise_api/entities/integration.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/entities/policy.py` & `superwise_api-2.0.0/superwise_api/entities/policy.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/entities/source.py` & `superwise_api-2.0.0/superwise_api/entities/source.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/errors.py` & `superwise_api-2.0.0/superwise_api/errors.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/__init__.py` & `superwise_api-2.0.0/superwise_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/application/enums.py` & `superwise_api-2.0.0/superwise_api/models/application/enums.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/application/schemas.py` & `superwise_api-2.0.0/superwise_api/models/application/schemas.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/dashboard/dashboard_response.py` & `superwise_api-2.0.0/superwise_api/models/dashboard/dashboard_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/dashboard/page_dashboard.py` & `superwise_api-2.0.0/superwise_api/models/dashboard/page_dashboard.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/dashboard_item/dashboard_item.py` & `superwise_api-2.0.0/superwise_api/models/dashboard_item/dashboard_item.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/dashboard_item/dashboard_item_create.py` & `superwise_api-2.0.0/superwise_api/models/dashboard_item/dashboard_item_create.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/dashboard_item/dashboard_item_response.py` & `superwise_api-2.0.0/superwise_api/models/dashboard_item/dashboard_item_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/dashboard_item/page_dashboard_item.py` & `superwise_api-2.0.0/superwise_api/models/dashboard_item/page_dashboard_item.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/dashboard_item/query.py` & `superwise_api-2.0.0/superwise_api/models/dashboard_item/query.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/dashboard_item/query_filter.py` & `superwise_api-2.0.0/superwise_api/models/dashboard_item/query_filter.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/dataset/__init__.py` & `superwise_api-2.0.0/superwise_api/models/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/dataset/dataset_response.py` & `superwise_api-2.0.0/superwise_api/models/dataset/dataset_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/dataset/dataset_schema.py` & `superwise_api-2.0.0/superwise_api/models/dataset/dataset_schema.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/dataset/page_dataset_response.py` & `superwise_api-2.0.0/superwise_api/models/dataset/page_dataset_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/policy/__init__.py` & `superwise_api-2.0.0/superwise_api/models/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/policy/page_policy_response.py` & `superwise_api-2.0.0/superwise_api/models/policy/page_policy_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/policy/policy_response.py` & `superwise_api-2.0.0/superwise_api/models/policy/policy_response.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/policy/query.py` & `superwise_api-2.0.0/superwise_api/models/policy/query.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/policy/query_filter.py` & `superwise_api-2.0.0/superwise_api/models/policy/query_filter.py`

 * *Files identical despite different names*

### Comparing `superwise_api-1.3.0/superwise_api/models/tool/enums.py` & `superwise_api-2.0.0/superwise_api/models/tool/enums.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     PINECONE_VECTOR_DB = "PineconeVectorDB"
     PG_VECTOR = "PGVector"
     SQL_DATABASE_POSTGRES = "PostgreSQL"
     SQL_DATABASE_BIGQUERY = "BigQuery"
     SQL_DATABASE_MYSQL = "MySQL"
     SQL_DATABASE_MSSQL = "MSSQL"
     SQL_DATABASE_ORACLE = "Oracle"
+    OPENAPI = "OpenAPI"
 
 
 class EmbeddingModelProvider(str, Enum):
     VERTEX_AI_MODEL_GARDEN = "VertexAIModelGarden"
     OPEN_AI = "OpenAI"
     GOOGLE_AI = "GoogleAI"
```

### Comparing `superwise_api-1.3.0/superwise_api/models/tool/schemas.py` & `superwise_api-2.0.0/superwise_api/models/tool/schemas.py`

 * *Files 7% similar despite different names*

```diff
@@ -95,22 +95,38 @@
 class ToolConfigPineconeVectorDB(ToolConfigBase):
     type: Literal[ToolType.PINECONE_VECTOR_DB]
     api_key: str
     index_name: str
     embedding_model: EmbeddingModel = Field(..., discriminator="provider")
 
 
+class BearerAuthenticationConfig(BaseModel):
+    type: Literal["Bearer"]
+    token: str
+
+
+# can add more types of authentication here like OAuth2
+AuthenticationConfig = BearerAuthenticationConfig
+
+
+class ToolConfigOpenAPI(ToolConfigBase):
+    type: Literal[ToolType.OPENAPI]
+    openapi_schema: dict
+    authentication: Optional[AuthenticationConfig] = None
+
+
 ToolConfig = Union[
     ToolConfigPGVector,
     ToolConfigPineconeVectorDB,
     ToolConfigSQLDatabasePostgres,
     ToolConfigSQLDatabaseMySQL,
     ToolConfigSQLDatabaseMSSQL,
     ToolConfigSQLDatabaseOracle,
     ToolConfigBigQuery,
+    ToolConfigOpenAPI,
 ]
 
 
 class ToolDef(BaseModel):
     name: str
     description: Optional[str] = Field(default=None)
     config: ToolConfig
```

### Comparing `superwise_api-1.3.0/superwise_api/superwise_client.py` & `superwise_api-2.0.0/superwise_api/superwise_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         *DashboardItemsApi* | [**get_dashboards_items**](../docs/dashboard_item/schemas/DashboardItemsApi.md#get_dashboards_items) | **GET** /v1/dashboard-items | Get Dashboards Items
         """
         return DashboardItem(self)
 
     @property
     def application(self):
         """
-        *ApplicationsApi* | [**ask**](../docs/application/schemas/ApplicationsApi.md#ask) | **POST** /v1/applications/ask | Ask
+        *ApplicationsApi* | [**ask**](../docs/application/schemas/ApplicationsApi.md#ask) | **POST** /v1/application-playground/ask | Ask
 
         *ApplicationsApi* | [**create_application**](../docs/application/schemas/ApplicationsApi.md#create_application) | **POST** /v1/applications | Create Application
         """
         return Application(self)
 
     @staticmethod
     def _fetch_token(auth_url: str, client_id: str, client_secret: str) -> str:
```

### Comparing `superwise_api-1.3.0/PKG-INFO` & `superwise_api-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superwise-api
-Version: 1.3.0
+Version: 2.0.0
 Summary: Superwise SDK for Python
 License: MIT
 Keywords: OpenAPI,SuperwiseSDK
 Author: Superwise
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

