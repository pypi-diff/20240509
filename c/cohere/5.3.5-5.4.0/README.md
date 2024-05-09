# Comparing `tmp/cohere-5.3.5.tar.gz` & `tmp/cohere-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-5.3.5.tar", max compression
+gzip compressed data, was "cohere-5.4.0.tar", max compression
```

## Comparing `cohere-5.3.5.tar` & `cohere-5.4.0.tar`

### file list

```diff
@@ -1,180 +1,181 @@
--rw-r--r--   0        0        0     1062 2024-05-08 11:43:14.680259 cohere-5.3.5/LICENSE
--rw-r--r--   0        0        0     2359 2024-05-08 11:43:14.680259 cohere-5.3.5/README.md
--rw-r--r--   0        0        0      698 2024-05-08 11:43:14.684259 cohere-5.3.5/pyproject.toml
--rw-r--r--   0        0        0     8246 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/__init__.py
--rw-r--r--   0        0        0   228964 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/base_client.py
--rw-r--r--   0        0        0    19723 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/client.py
--rw-r--r--   0        0        0       22 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/config.py
--rw-r--r--   0        0        0       65 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/connectors/__init__.py
--rw-r--r--   0        0        0    50609 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/connectors/client.py
--rw-r--r--   0        0        0     1006 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/api_error.py
--rw-r--r--   0        0        0     2226 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/request_options.py
--rw-r--r--   0        0        0     7123 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/core/unchecked_base_model.py
--rw-r--r--   0        0        0      419 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/__init__.py
--rw-r--r--   0        0        0    35730 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/client.py
--rw-r--r--   0        0        0      578 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/types/__init__.py
--rw-r--r--   0        0        0     1002 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/types/datasets_create_response.py
--rw-r--r--   0        0        0     1402 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py
--rw-r--r--   0        0        0      959 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/types/datasets_get_response.py
--rw-r--r--   0        0        0     1057 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/types/datasets_get_usage_response.py
--rw-r--r--   0        0        0      998 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/datasets/types/datasets_list_response.py
--rw-r--r--   0        0        0      159 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/embed_jobs/__init__.py
--rw-r--r--   0        0        0    31897 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/embed_jobs/client.py
--rw-r--r--   0        0        0      187 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/embed_jobs/types/__init__.py
--rw-r--r--   0        0        0      169 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
--rw-r--r--   0        0        0      159 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/environment.py
--rw-r--r--   0        0        0      617 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/not_found_error.py
--rw-r--r--   0        0        0      290 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/service_unavailable_error.py
--rw-r--r--   0        0        0      326 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      284 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/errors/unauthorized_error.py
--rw-r--r--   0        0        0      953 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/__init__.py
--rw-r--r--   0        0        0    62115 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/client.py
--rw-r--r--   0        0        0      905 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/__init__.py
--rw-r--r--   0        0        0     1343 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/__init__.py
--rw-r--r--   0        0        0     1475 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/base_model.py
--rw-r--r--   0        0        0      273 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/base_type.py
--rw-r--r--   0        0        0     1175 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
--rw-r--r--   0        0        0      140 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
--rw-r--r--   0        0        0     1083 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/error.py
--rw-r--r--   0        0        0     1400 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/event.py
--rw-r--r--   0        0        0     2357 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/finetuned_model.py
--rw-r--r--   0        0        0     1171 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
--rw-r--r--   0        0        0     1823 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/hyperparameters.py
--rw-r--r--   0        0        0     1489 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/list_events_response.py
--rw-r--r--   0        0        0     1532 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
--rw-r--r--   0        0        0     1463 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
--rw-r--r--   0        0        0     1577 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/settings.py
--rw-r--r--   0        0        0      402 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/status.py
--rw-r--r--   0        0        0      193 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/strategy.py
--rw-r--r--   0        0        0     1390 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/training_step_metrics.py
--rw-r--r--   0        0        0     1177 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
--rw-r--r--   0        0        0      811 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/manually_maintained/cache.py
--rw-r--r--   0        0        0     3015 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/manually_maintained/tokenizers.py
--rw-r--r--   0        0        0       65 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/models/__init__.py
--rw-r--r--   0        0        0    13859 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/models/client.py
--rw-r--r--   0        0        0      730 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/overrides.py
--rw-r--r--   0        0        0        0 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/py.typed
--rw-r--r--   0        0        0    10562 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/__init__.py
--rw-r--r--   0        0        0     1260 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/api_meta.py
--rw-r--r--   0        0        0     1011 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/api_meta_api_version.py
--rw-r--r--   0        0        0     1434 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/api_meta_billed_units.py
--rw-r--r--   0        0        0     1177 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/api_meta_tokens.py
--rw-r--r--   0        0        0      168 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/auth_token_type.py
--rw-r--r--   0        0        0     1929 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_citation.py
--rw-r--r--   0        0        0     1127 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_citation_generation_event.py
--rw-r--r--   0        0        0     1861 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_connector.py
--rw-r--r--   0        0        0     1297 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_data_metrics.py
--rw-r--r--   0        0        0      117 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_document.py
--rw-r--r--   0        0        0     1644 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_message.py
--rw-r--r--   0        0        0      168 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_message_role.py
--rw-r--r--   0        0        0      170 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_request_citation_quality.py
--rw-r--r--   0        0        0     1708 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_request_connectors_search_options.py
--rw-r--r--   0        0        0      189 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_request_prompt_truncation.py
--rw-r--r--   0        0        0     1011 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_request_tool_results_item.py
--rw-r--r--   0        0        0     1180 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_search_queries_generation_event.py
--rw-r--r--   0        0        0     1247 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_search_query.py
--rw-r--r--   0        0        0     1653 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_search_result.py
--rw-r--r--   0        0        0     1055 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_search_result_connector.py
--rw-r--r--   0        0        0     1417 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_search_results_event.py
--rw-r--r--   0        0        0     1861 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_end_event.py
--rw-r--r--   0        0        0      225 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_end_event_finish_reason.py
--rw-r--r--   0        0        0      893 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_event.py
--rw-r--r--   0        0        0      176 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_request_citation_quality.py
--rw-r--r--   0        0        0     1714 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_request_connectors_search_options.py
--rw-r--r--   0        0        0      195 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_request_prompt_truncation.py
--rw-r--r--   0        0        0     1017 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_request_tool_results_item.py
--rw-r--r--   0        0        0     1102 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_stream_start_event.py
--rw-r--r--   0        0        0     1068 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_text_generation_event.py
--rw-r--r--   0        0        0     1040 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/chat_tool_calls_generation_event.py
--rw-r--r--   0        0        0     1005 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/check_api_key_response.py
--rw-r--r--   0        0        0     1004 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_data_metrics.py
--rw-r--r--   0        0        0      971 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_example.py
--rw-r--r--   0        0        0      171 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_request_truncate.py
--rw-r--r--   0        0        0     1137 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_response.py
--rw-r--r--   0        0        0     2560 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_response_classifications_item.py
--rw-r--r--   0        0        0      214 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_response_classifications_item_classification_type.py
--rw-r--r--   0        0        0      971 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/classify_response_classifications_item_labels_value.py
--rw-r--r--   0        0        0      220 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/compatible_endpoint.py
--rw-r--r--   0        0        0     3383 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/connector.py
--rw-r--r--   0        0        0      163 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/connector_auth_status.py
--rw-r--r--   0        0        0     1660 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/connector_o_auth.py
--rw-r--r--   0        0        0     1725 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/create_connector_o_auth.py
--rw-r--r--   0        0        0      960 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/create_connector_response.py
--rw-r--r--   0        0        0     1195 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/create_connector_service_auth.py
--rw-r--r--   0        0        0     1047 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/create_embed_job_response.py
--rw-r--r--   0        0        0     2209 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/dataset.py
--rw-r--r--   0        0        0     1788 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/dataset_part.py
--rw-r--r--   0        0        0      427 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/dataset_type.py
--rw-r--r--   0        0        0      222 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/dataset_validation_status.py
--rw-r--r--   0        0        0      135 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/delete_connector_response.py
--rw-r--r--   0        0        0     1068 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/detokenize_response.py
--rw-r--r--   0        0        0     1416 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/embed_by_type_response.py
--rw-r--r--   0        0        0     2271 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/embed_by_type_response_embeddings.py
--rw-r--r--   0        0        0     1364 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/embed_floats_response.py
--rw-r--r--   0        0        0      211 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/embed_input_type.py
--rw-r--r--   0        0        0     1864 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/embed_job.py
--rw-r--r--   0        0        0      201 2024-05-08 11:43:14.688259 cohere-5.3.5/src/cohere/types/embed_job_status.py
--rw-r--r--   0        0        0      156 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/embed_job_truncate.py
--rw-r--r--   0        0        0      168 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/embed_request_truncate.py
--rw-r--r--   0        0        0     1057 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/embed_response.py
--rw-r--r--   0        0        0      184 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/embedding_type.py
--rw-r--r--   0        0        0     1735 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/finetune_dataset_metrics.py
--rw-r--r--   0        0        0      222 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/finish_reason.py
--rw-r--r--   0        0        0      185 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_request_return_likelihoods.py
--rw-r--r--   0        0        0      171 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_request_truncate.py
--rw-r--r--   0        0        0     1197 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_end.py
--rw-r--r--   0        0        0     1101 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_end_response.py
--rw-r--r--   0        0        0     1311 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_error.py
--rw-r--r--   0        0        0      897 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_event.py
--rw-r--r--   0        0        0      191 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_request_return_likelihoods.py
--rw-r--r--   0        0        0      177 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_request_truncate.py
--rw-r--r--   0        0        0     1312 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_stream_text.py
--rw-r--r--   0        0        0     1456 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generate_streamed_response.py
--rw-r--r--   0        0        0     1254 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/generation.py
--rw-r--r--   0        0        0      957 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/get_connector_response.py
--rw-r--r--   0        0        0     2150 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/get_model_response.py
--rw-r--r--   0        0        0     1256 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/label_metric.py
--rw-r--r--   0        0        0     1095 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/list_connectors_response.py
--rw-r--r--   0        0        0      993 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/list_embed_job_response.py
--rw-r--r--   0        0        0     1187 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/list_models_response.py
--rw-r--r--   0        0        0     1130 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/metrics.py
--rw-r--r--   0        0        0     1115 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/metrics_embed_data.py
--rw-r--r--   0        0        0     1154 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/metrics_embed_data_fields_item.py
--rw-r--r--   0        0        0     2953 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/non_streamed_chat_response.py
--rw-r--r--   0        0        0     1080 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/o_auth_authorize_response.py
--rw-r--r--   0        0        0      974 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/parse_info.py
--rw-r--r--   0        0        0      239 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/rerank_request_documents_item.py
--rw-r--r--   0        0        0     1001 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/rerank_request_documents_item_text.py
--rw-r--r--   0        0        0     1200 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/rerank_response.py
--rw-r--r--   0        0        0     1909 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/rerank_response_results_item.py
--rw-r--r--   0        0        0     1136 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/rerank_response_results_item_document.py
--rw-r--r--   0        0        0     1818 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/reranker_data_metrics.py
--rw-r--r--   0        0        0     1819 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/single_generation.py
--rw-r--r--   0        0        0     1248 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/single_generation_in_stream.py
--rw-r--r--   0        0        0      952 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/single_generation_token_likelihoods_item.py
--rw-r--r--   0        0        0     3157 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/streamed_chat_response.py
--rw-r--r--   0        0        0      179 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/summarize_request_extractiveness.py
--rw-r--r--   0        0        0      170 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/summarize_request_format.py
--rw-r--r--   0        0        0      173 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/summarize_request_length.py
--rw-r--r--   0        0        0     1201 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/summarize_response.py
--rw-r--r--   0        0        0     1127 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/tokenize_response.py
--rw-r--r--   0        0        0      941 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/too_many_requests_error_body.py
--rw-r--r--   0        0        0     1928 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/tool.py
--rw-r--r--   0        0        0     1221 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/tool_call.py
--rw-r--r--   0        0        0     1331 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/tool_parameter_definitions_value.py
--rw-r--r--   0        0        0      960 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/types/update_connector_response.py
--rw-r--r--   0        0        0    10036 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/utils.py
--rw-r--r--   0        0        0       74 2024-05-08 11:43:14.692259 cohere-5.3.5/src/cohere/version.py
--rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 cohere-5.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-09 11:58:18.552228 cohere-5.4.0/LICENSE
+-rw-r--r--   0        0        0     2359 2024-05-09 11:58:18.552228 cohere-5.4.0/README.md
+-rw-r--r--   0        0        0      716 2024-05-09 11:58:18.556228 cohere-5.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8309 2024-05-09 11:58:18.556228 cohere-5.4.0/src/cohere/__init__.py
+-rw-r--r--   0        0        0   228964 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/base_client.py
+-rw-r--r--   0        0        0     9142 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/bedrock_client.py
+-rw-r--r--   0        0        0    19723 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/client.py
+-rw-r--r--   0        0        0       22 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/config.py
+-rw-r--r--   0        0        0       65 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/connectors/__init__.py
+-rw-r--r--   0        0        0    50609 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/connectors/client.py
+-rw-r--r--   0        0        0     1006 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/core/api_error.py
+-rw-r--r--   0        0        0     2226 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/core/request_options.py
+-rw-r--r--   0        0        0     7123 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      419 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/datasets/__init__.py
+-rw-r--r--   0        0        0    35730 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/datasets/client.py
+-rw-r--r--   0        0        0      578 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/datasets/types/__init__.py
+-rw-r--r--   0        0        0     1002 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/datasets/types/datasets_create_response.py
+-rw-r--r--   0        0        0     1402 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py
+-rw-r--r--   0        0        0      959 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/datasets/types/datasets_get_response.py
+-rw-r--r--   0        0        0     1057 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/datasets/types/datasets_get_usage_response.py
+-rw-r--r--   0        0        0      998 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/datasets/types/datasets_list_response.py
+-rw-r--r--   0        0        0      159 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/embed_jobs/__init__.py
+-rw-r--r--   0        0        0    31897 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/embed_jobs/client.py
+-rw-r--r--   0        0        0      187 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/embed_jobs/types/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
+-rw-r--r--   0        0        0      159 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/environment.py
+-rw-r--r--   0        0        0      617 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/errors/not_found_error.py
+-rw-r--r--   0        0        0      290 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/errors/service_unavailable_error.py
+-rw-r--r--   0        0        0      326 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      284 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      953 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/__init__.py
+-rw-r--r--   0        0        0    62127 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/client.py
+-rw-r--r--   0        0        0      905 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/__init__.py
+-rw-r--r--   0        0        0     1475 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/base_model.py
+-rw-r--r--   0        0        0      305 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/base_type.py
+-rw-r--r--   0        0        0     1175 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
+-rw-r--r--   0        0        0      140 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
+-rw-r--r--   0        0        0     1083 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/error.py
+-rw-r--r--   0        0        0     1400 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/event.py
+-rw-r--r--   0        0        0     2357 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/finetuned_model.py
+-rw-r--r--   0        0        0     1171 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
+-rw-r--r--   0        0        0     1823 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/hyperparameters.py
+-rw-r--r--   0        0        0     1489 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/list_events_response.py
+-rw-r--r--   0        0        0     1532 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
+-rw-r--r--   0        0        0     1463 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
+-rw-r--r--   0        0        0     1577 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/settings.py
+-rw-r--r--   0        0        0      402 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/status.py
+-rw-r--r--   0        0        0      193 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/strategy.py
+-rw-r--r--   0        0        0     1390 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/training_step_metrics.py
+-rw-r--r--   0        0        0     1177 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
+-rw-r--r--   0        0        0      811 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/manually_maintained/cache.py
+-rw-r--r--   0        0        0     3015 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/manually_maintained/tokenizers.py
+-rw-r--r--   0        0        0       65 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/models/__init__.py
+-rw-r--r--   0        0        0    13859 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/models/client.py
+-rw-r--r--   0        0        0      730 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/overrides.py
+-rw-r--r--   0        0        0        0 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/py.typed
+-rw-r--r--   0        0        0    10562 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/__init__.py
+-rw-r--r--   0        0        0     1260 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/api_meta.py
+-rw-r--r--   0        0        0     1011 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/api_meta_api_version.py
+-rw-r--r--   0        0        0     1434 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/api_meta_billed_units.py
+-rw-r--r--   0        0        0     1177 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/api_meta_tokens.py
+-rw-r--r--   0        0        0      168 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/auth_token_type.py
+-rw-r--r--   0        0        0     1929 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_citation.py
+-rw-r--r--   0        0        0     1127 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_citation_generation_event.py
+-rw-r--r--   0        0        0     1861 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_connector.py
+-rw-r--r--   0        0        0     1297 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_data_metrics.py
+-rw-r--r--   0        0        0      117 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_document.py
+-rw-r--r--   0        0        0     1644 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_message.py
+-rw-r--r--   0        0        0      168 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_message_role.py
+-rw-r--r--   0        0        0      170 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_request_citation_quality.py
+-rw-r--r--   0        0        0     1708 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_request_connectors_search_options.py
+-rw-r--r--   0        0        0      189 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1011 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_request_tool_results_item.py
+-rw-r--r--   0        0        0     1180 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_search_queries_generation_event.py
+-rw-r--r--   0        0        0     1247 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_search_query.py
+-rw-r--r--   0        0        0     1653 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_search_result.py
+-rw-r--r--   0        0        0     1055 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_search_result_connector.py
+-rw-r--r--   0        0        0     1417 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_search_results_event.py
+-rw-r--r--   0        0        0     1861 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_stream_end_event.py
+-rw-r--r--   0        0        0      225 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_stream_end_event_finish_reason.py
+-rw-r--r--   0        0        0      893 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_stream_event.py
+-rw-r--r--   0        0        0      176 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_stream_request_citation_quality.py
+-rw-r--r--   0        0        0     1714 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_stream_request_connectors_search_options.py
+-rw-r--r--   0        0        0      195 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_stream_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1017 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_stream_request_tool_results_item.py
+-rw-r--r--   0        0        0     1102 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_stream_start_event.py
+-rw-r--r--   0        0        0     1068 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_text_generation_event.py
+-rw-r--r--   0        0        0     1040 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/chat_tool_calls_generation_event.py
+-rw-r--r--   0        0        0     1005 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/check_api_key_response.py
+-rw-r--r--   0        0        0     1004 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/classify_data_metrics.py
+-rw-r--r--   0        0        0      971 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/classify_example.py
+-rw-r--r--   0        0        0      171 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/classify_request_truncate.py
+-rw-r--r--   0        0        0     1137 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/classify_response.py
+-rw-r--r--   0        0        0     2560 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/classify_response_classifications_item.py
+-rw-r--r--   0        0        0      214 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/classify_response_classifications_item_classification_type.py
+-rw-r--r--   0        0        0      971 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/classify_response_classifications_item_labels_value.py
+-rw-r--r--   0        0        0      220 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/compatible_endpoint.py
+-rw-r--r--   0        0        0     3383 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/connector.py
+-rw-r--r--   0        0        0      163 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/connector_auth_status.py
+-rw-r--r--   0        0        0     1660 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/connector_o_auth.py
+-rw-r--r--   0        0        0     1725 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/create_connector_o_auth.py
+-rw-r--r--   0        0        0      960 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/create_connector_response.py
+-rw-r--r--   0        0        0     1195 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/create_connector_service_auth.py
+-rw-r--r--   0        0        0     1047 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/create_embed_job_response.py
+-rw-r--r--   0        0        0     2209 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/dataset.py
+-rw-r--r--   0        0        0     1788 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/dataset_part.py
+-rw-r--r--   0        0        0      427 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/dataset_type.py
+-rw-r--r--   0        0        0      222 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/dataset_validation_status.py
+-rw-r--r--   0        0        0      135 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/delete_connector_response.py
+-rw-r--r--   0        0        0     1068 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/detokenize_response.py
+-rw-r--r--   0        0        0     1416 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/embed_by_type_response.py
+-rw-r--r--   0        0        0     2271 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/embed_by_type_response_embeddings.py
+-rw-r--r--   0        0        0     1364 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/embed_floats_response.py
+-rw-r--r--   0        0        0      211 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/embed_input_type.py
+-rw-r--r--   0        0        0     1864 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/embed_job.py
+-rw-r--r--   0        0        0      201 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/embed_job_status.py
+-rw-r--r--   0        0        0      156 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/embed_job_truncate.py
+-rw-r--r--   0        0        0      168 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/embed_request_truncate.py
+-rw-r--r--   0        0        0     1057 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/embed_response.py
+-rw-r--r--   0        0        0      184 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/embedding_type.py
+-rw-r--r--   0        0        0     1735 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/finetune_dataset_metrics.py
+-rw-r--r--   0        0        0      222 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/finish_reason.py
+-rw-r--r--   0        0        0      185 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/generate_request_return_likelihoods.py
+-rw-r--r--   0        0        0      171 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/generate_request_truncate.py
+-rw-r--r--   0        0        0     1197 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/generate_stream_end.py
+-rw-r--r--   0        0        0     1101 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/generate_stream_end_response.py
+-rw-r--r--   0        0        0     1311 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/generate_stream_error.py
+-rw-r--r--   0        0        0      897 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/generate_stream_event.py
+-rw-r--r--   0        0        0      191 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/generate_stream_request_return_likelihoods.py
+-rw-r--r--   0        0        0      177 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/generate_stream_request_truncate.py
+-rw-r--r--   0        0        0     1312 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/generate_stream_text.py
+-rw-r--r--   0        0        0     1456 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/generate_streamed_response.py
+-rw-r--r--   0        0        0     1254 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/generation.py
+-rw-r--r--   0        0        0      957 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/get_connector_response.py
+-rw-r--r--   0        0        0     2150 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/get_model_response.py
+-rw-r--r--   0        0        0     1256 2024-05-09 11:58:18.560228 cohere-5.4.0/src/cohere/types/label_metric.py
+-rw-r--r--   0        0        0     1095 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/list_connectors_response.py
+-rw-r--r--   0        0        0      993 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/list_embed_job_response.py
+-rw-r--r--   0        0        0     1187 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/list_models_response.py
+-rw-r--r--   0        0        0     1130 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/metrics.py
+-rw-r--r--   0        0        0     1115 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/metrics_embed_data.py
+-rw-r--r--   0        0        0     1154 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/metrics_embed_data_fields_item.py
+-rw-r--r--   0        0        0     2953 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/non_streamed_chat_response.py
+-rw-r--r--   0        0        0     1080 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/o_auth_authorize_response.py
+-rw-r--r--   0        0        0      974 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/parse_info.py
+-rw-r--r--   0        0        0      239 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/rerank_request_documents_item.py
+-rw-r--r--   0        0        0     1001 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/rerank_request_documents_item_text.py
+-rw-r--r--   0        0        0     1200 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/rerank_response.py
+-rw-r--r--   0        0        0     1909 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/rerank_response_results_item.py
+-rw-r--r--   0        0        0     1136 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/rerank_response_results_item_document.py
+-rw-r--r--   0        0        0     1818 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/reranker_data_metrics.py
+-rw-r--r--   0        0        0     1819 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/single_generation.py
+-rw-r--r--   0        0        0     1248 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/single_generation_in_stream.py
+-rw-r--r--   0        0        0      952 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/single_generation_token_likelihoods_item.py
+-rw-r--r--   0        0        0     3157 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/streamed_chat_response.py
+-rw-r--r--   0        0        0      179 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/summarize_request_extractiveness.py
+-rw-r--r--   0        0        0      170 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/summarize_request_format.py
+-rw-r--r--   0        0        0      173 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/summarize_request_length.py
+-rw-r--r--   0        0        0     1201 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/summarize_response.py
+-rw-r--r--   0        0        0     1127 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/tokenize_response.py
+-rw-r--r--   0        0        0      941 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/too_many_requests_error_body.py
+-rw-r--r--   0        0        0     1928 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/tool.py
+-rw-r--r--   0        0        0     1221 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/tool_call.py
+-rw-r--r--   0        0        0     1331 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/tool_parameter_definitions_value.py
+-rw-r--r--   0        0        0      960 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/types/update_connector_response.py
+-rw-r--r--   0        0        0    10055 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/utils.py
+-rw-r--r--   0        0        0       74 2024-05-09 11:58:18.564228 cohere-5.4.0/src/cohere/version.py
+-rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 cohere-5.4.0/PKG-INFO
```

### Comparing `cohere-5.3.5/LICENSE` & `cohere-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/README.md` & `cohere-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/pyproject.toml` & `cohere-5.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "cohere"
-version = "5.3.5"
+version = "5.4.0"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "cohere", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
+boto3 = "^1.34.0"
 fastavro = "^1.9.4"
 httpx = ">=0.21.2"
 httpx-sse = "^0.4.0"
 pydantic = ">= 1.9.2"
 requests = "^2.0.0"
 tokenizers = "^0.19"
 types-requests = "^2.0.0"
```

### Comparing `cohere-5.3.5/src/cohere/__init__.py` & `cohere-5.4.0/src/cohere/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
     InternalServerError,
     NotFoundError,
     ServiceUnavailableError,
     TooManyRequestsError,
     UnauthorizedError,
 )
 from . import connectors, datasets, embed_jobs, finetuning, models
+from .bedrock_client import BedrockClient
 from .client import AsyncClient, Client
 from .datasets import (
     DatasetsCreateResponse,
     DatasetsCreateResponseDatasetPartsItem,
     DatasetsGetResponse,
     DatasetsGetUsageResponse,
     DatasetsListResponse,
@@ -148,14 +149,15 @@
     "ApiMeta",
     "ApiMetaApiVersion",
     "ApiMetaBilledUnits",
     "ApiMetaTokens",
     "AsyncClient",
     "AuthTokenType",
     "BadRequestError",
+    "BedrockClient",
     "ChatCitation",
     "ChatCitationGenerationEvent",
     "ChatConnector",
     "ChatDataMetrics",
     "ChatDocument",
     "ChatMessage",
     "ChatMessageRole",
```

### Comparing `cohere-5.3.5/src/cohere/base_client.py` & `cohere-5.4.0/src/cohere/base_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/client.py` & `cohere-5.4.0/src/cohere/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/connectors/client.py` & `cohere-5.4.0/src/cohere/connectors/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/core/__init__.py` & `cohere-5.4.0/src/cohere/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/core/client_wrapper.py` & `cohere-5.4.0/src/cohere/core/client_wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "cohere",
-            "X-Fern-SDK-Version": "5.3.4",
+            "X-Fern-SDK-Version": "5.4.0",
         }
         if self._client_name is not None:
             headers["X-Client-Name"] = self._client_name
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
```

### Comparing `cohere-5.3.5/src/cohere/core/datetime_utils.py` & `cohere-5.4.0/src/cohere/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/core/file.py` & `cohere-5.4.0/src/cohere/core/file.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/core/http_client.py` & `cohere-5.4.0/src/cohere/core/http_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/core/jsonable_encoder.py` & `cohere-5.4.0/src/cohere/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/core/request_options.py` & `cohere-5.4.0/src/cohere/core/request_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/core/unchecked_base_model.py` & `cohere-5.4.0/src/cohere/core/unchecked_base_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/datasets/client.py` & `cohere-5.4.0/src/cohere/datasets/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/datasets/types/__init__.py` & `cohere-5.4.0/src/cohere/datasets/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/datasets/types/datasets_create_response.py` & `cohere-5.4.0/src/cohere/datasets/types/datasets_create_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py` & `cohere-5.4.0/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/datasets/types/datasets_get_response.py` & `cohere-5.4.0/src/cohere/datasets/types/datasets_get_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/datasets/types/datasets_get_usage_response.py` & `cohere-5.4.0/src/cohere/datasets/types/datasets_get_usage_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
 from ...core.unchecked_base_model import UncheckedBaseModel
 
 
 class DatasetsGetUsageResponse(UncheckedBaseModel):
-    organization_usage: typing.Optional[str] = pydantic_v1.Field(default=None)
+    organization_usage: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The total number of bytes used by the organization.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `cohere-5.3.5/src/cohere/datasets/types/datasets_list_response.py` & `cohere-5.4.0/src/cohere/datasets/types/datasets_list_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/embed_jobs/client.py` & `cohere-5.4.0/src/cohere/embed_jobs/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/errors/__init__.py` & `cohere-5.4.0/src/cohere/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/__init__.py` & `cohere-5.4.0/src/cohere/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/client.py` & `cohere-5.4.0/src/cohere/finetuning/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             token="YOUR_TOKEN",
         )
         client.finetuning.create_finetuned_model(
             request=FinetunedModel(
                 name="api-test",
                 settings=Settings(
                     base_model=BaseModel(
-                        base_type="BASE_TYPE_CHAT",
+                        base_type="BASE_TYPE_GENERATIVE",
                     ),
                     dataset_id="my-dataset-id",
                 ),
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
@@ -806,15 +806,15 @@
             token="YOUR_TOKEN",
         )
         await client.finetuning.create_finetuned_model(
             request=FinetunedModel(
                 name="api-test",
                 settings=Settings(
                     base_model=BaseModel(
-                        base_type="BASE_TYPE_CHAT",
+                        base_type="BASE_TYPE_GENERATIVE",
                     ),
                     dataset_id="my-dataset-id",
                 ),
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
```

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/__init__.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/__init__.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/base_model.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/base_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/error.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/event.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/finetuned_model.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/finetuned_model.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/hyperparameters.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/list_events_response.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/list_events_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/settings.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/settings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/training_step_metrics.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/training_step_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py` & `cohere-5.4.0/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/manually_maintained/cache.py` & `cohere-5.4.0/src/cohere/manually_maintained/cache.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/manually_maintained/tokenizers.py` & `cohere-5.4.0/src/cohere/manually_maintained/tokenizers.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/models/client.py` & `cohere-5.4.0/src/cohere/models/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/overrides.py` & `cohere-5.4.0/src/cohere/overrides.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/__init__.py` & `cohere-5.4.0/src/cohere/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/api_meta.py` & `cohere-5.4.0/src/cohere/types/api_meta.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/api_meta_api_version.py` & `cohere-5.4.0/src/cohere/types/api_meta_api_version.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/api_meta_billed_units.py` & `cohere-5.4.0/src/cohere/types/api_meta_billed_units.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/api_meta_tokens.py` & `cohere-5.4.0/src/cohere/types/api_meta_tokens.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_citation.py` & `cohere-5.4.0/src/cohere/types/chat_citation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_citation_generation_event.py` & `cohere-5.4.0/src/cohere/types/chat_citation_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_connector.py` & `cohere-5.4.0/src/cohere/types/chat_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_data_metrics.py` & `cohere-5.4.0/src/cohere/types/chat_data_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class ChatDataMetrics(UncheckedBaseModel):
-    num_train_turns: typing.Optional[str] = pydantic_v1.Field(default=None)
+    num_train_turns: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The sum of all turns of valid train examples.
     """
 
-    num_eval_turns: typing.Optional[str] = pydantic_v1.Field(default=None)
+    num_eval_turns: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The sum of all turns of valid eval examples.
     """
 
     preamble: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The preamble of this dataset.
```

### Comparing `cohere-5.3.5/src/cohere/types/chat_message.py` & `cohere-5.4.0/src/cohere/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_request_connectors_search_options.py` & `cohere-5.4.0/src/cohere/types/chat_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_request_tool_results_item.py` & `cohere-5.4.0/src/cohere/types/chat_request_tool_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_search_queries_generation_event.py` & `cohere-5.4.0/src/cohere/types/chat_search_queries_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_search_query.py` & `cohere-5.4.0/src/cohere/types/chat_search_query.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_search_result.py` & `cohere-5.4.0/src/cohere/types/chat_search_result.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_search_result_connector.py` & `cohere-5.4.0/src/cohere/types/chat_search_result_connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_search_results_event.py` & `cohere-5.4.0/src/cohere/types/chat_search_results_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_stream_end_event.py` & `cohere-5.4.0/src/cohere/types/chat_stream_end_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_stream_event.py` & `cohere-5.4.0/src/cohere/types/chat_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_stream_request_connectors_search_options.py` & `cohere-5.4.0/src/cohere/types/chat_stream_request_connectors_search_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_stream_request_tool_results_item.py` & `cohere-5.4.0/src/cohere/types/chat_stream_request_tool_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_stream_start_event.py` & `cohere-5.4.0/src/cohere/types/chat_stream_start_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_text_generation_event.py` & `cohere-5.4.0/src/cohere/types/chat_text_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/chat_tool_calls_generation_event.py` & `cohere-5.4.0/src/cohere/types/chat_tool_calls_generation_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/check_api_key_response.py` & `cohere-5.4.0/src/cohere/types/check_api_key_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/classify_data_metrics.py` & `cohere-5.4.0/src/cohere/types/classify_data_metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/classify_example.py` & `cohere-5.4.0/src/cohere/types/classify_example.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/classify_response.py` & `cohere-5.4.0/src/cohere/types/classify_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/classify_response_classifications_item.py` & `cohere-5.4.0/src/cohere/types/classify_response_classifications_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/classify_response_classifications_item_labels_value.py` & `cohere-5.4.0/src/cohere/types/classify_response_classifications_item_labels_value.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/connector.py` & `cohere-5.4.0/src/cohere/types/connector.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/connector_o_auth.py` & `cohere-5.4.0/src/cohere/types/connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/create_connector_o_auth.py` & `cohere-5.4.0/src/cohere/types/create_connector_o_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/create_connector_response.py` & `cohere-5.4.0/src/cohere/types/create_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/create_connector_service_auth.py` & `cohere-5.4.0/src/cohere/types/create_connector_service_auth.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/create_embed_job_response.py` & `cohere-5.4.0/src/cohere/types/create_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/dataset.py` & `cohere-5.4.0/src/cohere/types/dataset.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/dataset_part.py` & `cohere-5.4.0/src/cohere/types/dataset_part.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/detokenize_response.py` & `cohere-5.4.0/src/cohere/types/detokenize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/embed_by_type_response.py` & `cohere-5.4.0/src/cohere/types/embed_by_type_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/embed_by_type_response_embeddings.py` & `cohere-5.4.0/src/cohere/types/embed_by_type_response_embeddings.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/embed_floats_response.py` & `cohere-5.4.0/src/cohere/types/embed_floats_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/embed_job.py` & `cohere-5.4.0/src/cohere/types/embed_job.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/embed_response.py` & `cohere-5.4.0/src/cohere/types/embed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/finetune_dataset_metrics.py` & `cohere-5.4.0/src/cohere/types/finetune_dataset_metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,40 +5,40 @@
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class FinetuneDatasetMetrics(UncheckedBaseModel):
-    trainable_token_count: typing.Optional[str] = pydantic_v1.Field(default=None)
+    trainable_token_count: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The number of tokens of valid examples that can be used for training.
     """
 
-    total_examples: typing.Optional[str] = pydantic_v1.Field(default=None)
+    total_examples: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The overall number of examples.
     """
 
-    train_examples: typing.Optional[str] = pydantic_v1.Field(default=None)
+    train_examples: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The number of training examples.
     """
 
-    train_size_bytes: typing.Optional[str] = pydantic_v1.Field(default=None)
+    train_size_bytes: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The size in bytes of all training examples.
     """
 
-    eval_examples: typing.Optional[str] = pydantic_v1.Field(default=None)
+    eval_examples: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     Number of evaluation examples.
     """
 
-    eval_size_bytes: typing.Optional[str] = pydantic_v1.Field(default=None)
+    eval_size_bytes: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The size in bytes of all eval examples.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `cohere-5.3.5/src/cohere/types/generate_stream_end.py` & `cohere-5.4.0/src/cohere/types/generate_stream_end.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/generate_stream_end_response.py` & `cohere-5.4.0/src/cohere/types/generate_stream_end_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/generate_stream_error.py` & `cohere-5.4.0/src/cohere/types/generate_stream_error.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/generate_stream_event.py` & `cohere-5.4.0/src/cohere/types/generate_stream_event.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/generate_stream_text.py` & `cohere-5.4.0/src/cohere/types/generate_stream_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/generate_streamed_response.py` & `cohere-5.4.0/src/cohere/types/generate_streamed_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/generation.py` & `cohere-5.4.0/src/cohere/types/generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/get_connector_response.py` & `cohere-5.4.0/src/cohere/types/get_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/get_model_response.py` & `cohere-5.4.0/src/cohere/types/get_model_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/label_metric.py` & `cohere-5.4.0/src/cohere/types/label_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class LabelMetric(UncheckedBaseModel):
-    total_examples: typing.Optional[str] = pydantic_v1.Field(default=None)
+    total_examples: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     Total number of examples for this label
     """
 
     label: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     value of the label
```

### Comparing `cohere-5.3.5/src/cohere/types/list_connectors_response.py` & `cohere-5.4.0/src/cohere/types/list_connectors_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/list_embed_job_response.py` & `cohere-5.4.0/src/cohere/types/list_embed_job_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/list_models_response.py` & `cohere-5.4.0/src/cohere/types/list_models_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/metrics.py` & `cohere-5.4.0/src/cohere/types/metrics.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/metrics_embed_data.py` & `cohere-5.4.0/src/cohere/types/metrics_embed_data.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/metrics_embed_data_fields_item.py` & `cohere-5.4.0/src/cohere/types/metrics_embed_data_fields_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/non_streamed_chat_response.py` & `cohere-5.4.0/src/cohere/types/non_streamed_chat_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/o_auth_authorize_response.py` & `cohere-5.4.0/src/cohere/types/o_auth_authorize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/parse_info.py` & `cohere-5.4.0/src/cohere/types/parse_info.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/rerank_request_documents_item_text.py` & `cohere-5.4.0/src/cohere/types/rerank_request_documents_item_text.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/rerank_response.py` & `cohere-5.4.0/src/cohere/types/rerank_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/rerank_response_results_item.py` & `cohere-5.4.0/src/cohere/types/rerank_response_results_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/rerank_response_results_item_document.py` & `cohere-5.4.0/src/cohere/types/rerank_response_results_item_document.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/reranker_data_metrics.py` & `cohere-5.4.0/src/cohere/types/reranker_data_metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,40 +5,40 @@
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class RerankerDataMetrics(UncheckedBaseModel):
-    num_train_queries: typing.Optional[str] = pydantic_v1.Field(default=None)
+    num_train_queries: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The number of training queries.
     """
 
-    num_train_relevant_passages: typing.Optional[str] = pydantic_v1.Field(default=None)
+    num_train_relevant_passages: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The sum of all relevant passages of valid training examples.
     """
 
-    num_train_hard_negatives: typing.Optional[str] = pydantic_v1.Field(default=None)
+    num_train_hard_negatives: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The sum of all hard negatives of valid training examples.
     """
 
-    num_eval_queries: typing.Optional[str] = pydantic_v1.Field(default=None)
+    num_eval_queries: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The number of evaluation queries.
     """
 
-    num_eval_relevant_passages: typing.Optional[str] = pydantic_v1.Field(default=None)
+    num_eval_relevant_passages: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The sum of all relevant passages of valid eval examples.
     """
 
-    num_eval_hard_negatives: typing.Optional[str] = pydantic_v1.Field(default=None)
+    num_eval_hard_negatives: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The sum of all hard negatives of valid eval examples.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `cohere-5.3.5/src/cohere/types/single_generation.py` & `cohere-5.4.0/src/cohere/types/single_generation.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/single_generation_in_stream.py` & `cohere-5.4.0/src/cohere/types/single_generation_in_stream.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/single_generation_token_likelihoods_item.py` & `cohere-5.4.0/src/cohere/types/single_generation_token_likelihoods_item.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/streamed_chat_response.py` & `cohere-5.4.0/src/cohere/types/streamed_chat_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/summarize_response.py` & `cohere-5.4.0/src/cohere/types/summarize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/tokenize_response.py` & `cohere-5.4.0/src/cohere/types/tokenize_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/too_many_requests_error_body.py` & `cohere-5.4.0/src/cohere/types/too_many_requests_error_body.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/tool.py` & `cohere-5.4.0/src/cohere/types/tool.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/tool_call.py` & `cohere-5.4.0/src/cohere/types/tool_call.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/tool_parameter_definitions_value.py` & `cohere-5.4.0/src/cohere/types/tool_parameter_definitions_value.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/types/update_connector_response.py` & `cohere-5.4.0/src/cohere/types/update_connector_response.py`

 * *Files identical despite different names*

### Comparing `cohere-5.3.5/src/cohere/utils.py` & `cohere-5.4.0/src/cohere/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
 def sum_fields_if_not_none(obj: typing.Any, field: str) -> Optional[int]:
     non_none = [getattr(obj, field) for obj in obj if getattr(obj, field) is not None]
     return sum(non_none) if non_none else None
 
 
 def merge_meta_field(metas: typing.List[ApiMeta]) -> ApiMeta:
-    api_version = metas[0].api_version
+    api_version = metas[0].api_version if metas else None
     billed_units = [meta.billed_units for meta in metas]
     input_tokens = sum_fields_if_not_none(billed_units, "input_tokens")
     output_tokens = sum_fields_if_not_none(billed_units, "output_tokens")
     search_units = sum_fields_if_not_none(billed_units, "search_units")
     classifications = sum_fields_if_not_none(billed_units, "classifications")
     warnings = {warning for meta in metas if meta.warnings for warning in meta.warnings}
     return ApiMeta(
```

### Comparing `cohere-5.3.5/PKG-INFO` & `cohere-5.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 5.3.5
+Version: 5.4.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: boto3 (>=1.34.0,<2.0.0)
 Requires-Dist: fastavro (>=1.9.4,<2.0.0)
 Requires-Dist: httpx (>=0.21.2)
 Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
 Requires-Dist: pydantic (>=1.9.2)
 Requires-Dist: requests (>=2.0.0,<3.0.0)
 Requires-Dist: tokenizers (>=0.19,<0.20)
 Requires-Dist: types-requests (>=2.0.0,<3.0.0)
```

