# Comparing `tmp/odm-api-0.0.1.tar.gz` & `tmp/odm_api-1.57.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odm-api-0.0.1.tar", last modified: Thu Feb 22 12:05:40 2024, max compression
+gzip compressed data, was "odm_api-1.57.0.tar", last modified: Thu May  9 11:01:53 2024, max compression
```

## Comparing `odm-api-0.0.1.tar` & `odm_api-1.57.0.tar`

### file list

```diff
@@ -1,329 +1,331 @@
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 12:05:40.218161 odm-api-0.0.1/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      446 2024-02-22 12:05:40.218077 odm-api-0.0.1/PKG-INFO
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    74530 2024-02-22 12:03:48.000000 odm-api-0.0.1/README.md
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 12:05:40.141178 odm-api-0.0.1/odm_api/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    12007 2024-02-22 12:03:48.000000 odm-api-0.0.1/odm_api/__init__.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 12:05:40.165851 odm-api-0.0.1/odm_api/api/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3205 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/__init__.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    91688 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/data_import_jobs_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   295659 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/expression_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   147568 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/expression_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   209866 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/expression_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   170731 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/expression_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   115223 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/flow_cytometry_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    64572 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/flow_cytometry_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   208078 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/flow_cytometry_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   170043 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/flow_cytometry_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    73689 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/groups_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    39106 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/job_operations_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   125878 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/library_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    80195 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/library_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   142736 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/library_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    95312 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/library_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    72980 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/linkage_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    48417 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/linkage_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    31858 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/manage_data_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    13741 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/metadata_versioning_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   613834 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/omics_queries_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   614149 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/omics_queries_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   126367 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/preparation_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    80352 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/preparation_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   143280 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/preparation_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    95652 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/preparation_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   139113 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/sample_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    93836 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/sample_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   113735 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/sample_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    75831 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/sample_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   138099 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/study_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   137976 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/study_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   112549 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/study_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    75890 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/study_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    22849 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/tasks_api_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    66750 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/users_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    11391 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/validation_summary_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   115101 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/variant_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    64377 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/variant_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   214328 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/variant_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)   176593 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/variant_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    63223 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api/xrefset_queries_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    25715 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api_client.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      652 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/api_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    15658 2024-02-22 12:03:48.000000 odm-api-0.0.1/odm_api/configuration.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     5938 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/exceptions.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 12:05:40.188401 odm-api-0.0.1/odm_api/models/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     8369 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/__init__.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3447 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/applied_filter.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3196 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/attribute_invalid_value.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3236 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/attribute_invalid_value_errors_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3488 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/attribute_validation_summary.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3324 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/attribute_validation_summary_attribute_invalid_values_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2748 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/base_error_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2522 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/base_error_response_error.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3109 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/batch_of_ids.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2818 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/commit_info.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4406 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/create_group201_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3961 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/create_group_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2736 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/create_group_request_members_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4619 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/create_user201_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3190 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/create_user201_response_all_of_meta.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4174 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/create_user_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3001 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/create_user_request_emails_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2578 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/data_item.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3186 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/data_presentation.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3098 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/data_presentation_relationships.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3041 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/detached_collection.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3471 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/detached_collection_data_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3419 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/detached_object.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2909 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/email.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2482 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/error_message.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2582 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/exception_type_and_message.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4214 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/expression_item.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3071 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/expression_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4909 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/expression_signal_source.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4058 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/filter_groups_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2754 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/filter_option.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3419 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/filter_option_group.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4049 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/filter_users_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3739 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/find_objects_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3519 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/find_objects_response_filter_option_groups_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2922 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/find_objects_response_filter_option_groups_inner_options_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3768 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/find_objects_response_objects_page.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4192 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/find_objects_response_objects_page_content_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2704 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/find_objects_response_objects_page_content_inner_summary_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3414 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/flow_cytometry_item.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3108 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/flow_cytometry_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3227 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/flow_cytometry_signal_source.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4278 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/get_expression_as_user200_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4971 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/get_expression_as_user200_response_feature.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4928 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/get_expression_as_user200_response_value.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3490 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/get_flow_cytometry_as_curator200_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3654 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/get_variant_as_curator200_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3909 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/group.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3473 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/group_patch.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4370 2024-02-14 07:52:33.000000 odm-api-0.0.1/odm_api/models/group_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3248 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/group_validation_summary.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3532 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/group_validation_summary_attributes_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3405 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/i_metadata.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4852 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/import_expression_signal_run_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3103 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/import_metadata_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3410 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/import_signal_run_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3617 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/info.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3044 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/job_runtime_error.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2590 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/job_runtime_error_stack_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2626 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/json_metadata.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3193 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/link.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2814 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/list_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2832 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/list_response_meta.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2766 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/list_response_meta_pagination.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2902 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/managed_object.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2640 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/member.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3112 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/meta.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2816 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/meta_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3533 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/metadata_presentation.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3481 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/metadata_presentation_metadata.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2675 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/metadata_with_id.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2572 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/metainfo_key_for_summary.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3692 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/objects_page.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2825 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/omics_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3424 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/omics_response_data_presentation.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3274 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/omics_response_data_presentation_data_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3456 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/omics_response_metadata_presentation.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3599 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/omics_response_metadata_presentation_data_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3317 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/omics_response_metadata_with_id.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3749 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/output.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3052 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/output_errors_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2746 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/page_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2718 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/pagination_info.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2977 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/patch_operation.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3034 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/relationships.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2835 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/runs_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2732 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/sample_source.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3942 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/scim_error_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3392 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/search_study_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3515 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/search_study_request_filters_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2790 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/search_study_request_page.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2903 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/source_type_pair.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3437 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/start_import_flow_cytometry_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2772 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/study_generic_source.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4084 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/study_search_info.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3029 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/study_validation_summary.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3296 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/study_validation_summary_samples_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4156 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/task_info.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4122 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/user.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3469 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/user_patch.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3017 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/user_patch_operations_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4583 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/user_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3168 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/validation_error.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3796 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/variant_item.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3059 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/variant_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3203 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/variant_signal_source.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3611 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/xref_set_create_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3828 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/xref_set_create_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3049 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/xref_set_metadata.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3112 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/xref_set_search_result.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2830 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/xref_set_search_result_entry.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2854 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/models/xref_set_search_result_result_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)        0 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/py.typed
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     9191 2024-02-14 07:52:34.000000 odm-api-0.0.1/odm_api/rest.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 12:05:40.217717 odm-api-0.0.1/odm_api.egg-info/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      446 2024-02-22 12:05:40.000000 odm-api-0.0.1/odm_api.egg-info/PKG-INFO
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    12605 2024-02-22 12:05:40.000000 odm-api-0.0.1/odm_api.egg-info/SOURCES.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)        1 2024-02-22 12:05:40.000000 odm-api-0.0.1/odm_api.egg-info/dependency_links.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)       76 2024-02-22 12:05:40.000000 odm-api-0.0.1/odm_api.egg-info/requires.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)        8 2024-02-22 12:05:40.000000 odm-api-0.0.1/odm_api.egg-info/top_level.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1915 2024-02-22 12:03:48.000000 odm-api-0.0.1/pyproject.toml
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)       69 2024-02-22 12:05:40.218411 odm-api-0.0.1/setup.cfg
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1229 2024-02-22 12:03:48.000000 odm-api-0.0.1/setup.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 12:05:40.217363 odm-api-0.0.1/test/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1435 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_applied_filter.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1577 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_attribute_invalid_value.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1612 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_attribute_invalid_value_errors_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1718 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_attribute_validation_summary.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1965 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_attribute_validation_summary_attribute_invalid_values_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1602 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_base_error_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1469 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_base_error_response_error.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1549 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_batch_of_ids.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1384 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_commit_info.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2175 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_create_group201_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1745 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_create_group_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1644 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_create_group_request_members_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2335 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_create_user201_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1761 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_create_user201_response_all_of_meta.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1905 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_create_user_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1573 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_create_user_request_emails_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1948 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_data_import_jobs_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1302 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_data_item.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1651 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_data_presentation.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1612 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_data_presentation_relationships.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1794 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_detached_collection.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1943 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_detached_collection_data_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1785 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_detached_object.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1293 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_email.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1347 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_error_message.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1478 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_exception_type_and_message.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     5548 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_expression_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2441 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_expression_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1643 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_expression_item.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1645 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_expression_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1718 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_expression_signal_source.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2881 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_expression_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2238 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_expression_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1693 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_filter_groups_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1399 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_filter_option.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1539 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_filter_option_group.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1681 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_filter_users_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2137 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_find_objects_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1843 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_find_objects_response_filter_option_groups_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1910 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_find_objects_response_filter_option_groups_inner_options_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1886 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_find_objects_response_objects_page.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2021 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_find_objects_response_objects_page_content_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1897 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_find_objects_response_objects_page_content_inner_summary_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2532 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_flow_cytometry_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1453 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_flow_cytometry_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1609 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_flow_cytometry_item.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1654 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_flow_cytometry_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1617 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_flow_cytometry_signal_source.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2989 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_flow_cytometry_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2330 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_flow_cytometry_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1838 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_get_expression_as_user200_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1592 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_get_expression_as_user200_response_feature.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1568 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_get_expression_as_user200_response_value.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1840 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_get_flow_cytometry_as_curator200_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1936 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_get_variant_as_curator200_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1587 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_group.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1709 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_group_patch.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2066 2024-02-14 07:52:33.000000 odm-api-0.0.1/test/test_group_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1851 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_group_validation_summary.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1852 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_group_validation_summary_attributes_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1250 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_groups_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1663 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_i_metadata.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2085 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_import_expression_signal_run_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1684 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_import_metadata_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1830 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_import_signal_run_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1849 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_info.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1144 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_job_operations_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1450 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_job_runtime_error.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1503 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_job_runtime_error_stack_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1374 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_json_metadata.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2529 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_library_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1579 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_library_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2325 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_library_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1583 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_library_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1320 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_link.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1838 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_linkage_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1442 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_linkage_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1435 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_list_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1404 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_list_response_meta.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1570 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_list_response_meta_pagination.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      903 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_manage_data_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1731 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_managed_object.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1352 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_member.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1444 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_meta.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1355 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_meta_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2243 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_metadata_presentation.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1920 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_metadata_presentation_metadata.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      926 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_metadata_versioning_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1375 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_metadata_with_id.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1496 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_metainfo_key_for_summary.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1655 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_objects_page.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2529 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_omics_queries_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2466 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_omics_queries_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1513 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_omics_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2209 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_omics_response_data_presentation.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1949 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_omics_response_data_presentation_data_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2874 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_omics_response_metadata_presentation.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2511 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_omics_response_metadata_presentation_data_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1708 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_omics_response_metadata_with_id.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1473 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_output.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1474 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_output_errors_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1332 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_page_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1424 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_pagination_info.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1424 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_patch_operation.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2631 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_preparation_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1635 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_preparation_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2446 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_preparation_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1654 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_preparation_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1418 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_relationships.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1507 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_runs_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2206 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_sample_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1307 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_sample_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1384 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_sample_source.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1886 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_sample_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1369 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_sample_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1594 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_scim_error_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1558 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_search_study_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1642 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_search_study_request_filters_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1466 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_search_study_request_page.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1379 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_source_type_pair.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1939 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_start_import_flow_cytometry_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1569 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_study_generic_source.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1770 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_study_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1725 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_study_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1693 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_study_search_info.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1934 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_study_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1355 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_study_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2188 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_study_validation_summary.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1997 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_study_validation_summary_samples_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1458 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_task_info.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      966 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_tasks_api_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1747 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_user.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1697 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_user_patch.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1546 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_user_patch_operations_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2226 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_user_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1230 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_users_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1405 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_validation_error.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      900 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_validation_summary_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2368 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_variant_integration_as_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1373 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_variant_integration_as_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1663 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_variant_item.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1651 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_variant_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1544 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_variant_signal_source.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2769 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_variant_spo_tas_curator_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2166 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_variant_spo_tas_user_api.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1744 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_xref_set_create_request.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2075 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_xref_set_create_response.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1544 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_xref_set_metadata.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1629 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_xref_set_search_result.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1604 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_xref_set_search_result_entry.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1677 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_xref_set_search_result_result_inner.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1546 2024-02-14 07:52:34.000000 odm-api-0.0.1/test/test_xrefset_queries_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:01:53.460622 odm_api-1.57.0/
+-rw-r--r--   0 root         (0) root         (0)     1252 2024-05-09 11:01:53.460622 odm_api-1.57.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    75383 2024-05-09 11:01:21.000000 odm_api-1.57.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:01:53.392619 odm_api-1.57.0/odm_api/
+-rw-r--r--   0 root         (0) root         (0)    12853 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:01:53.408619 odm_api-1.57.0/odm_api/api/
+-rw-r--r--   0 root         (0) root         (0)     3205 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92561 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/data_import_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)   296706 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/expression_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)   148447 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/expression_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)   210816 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/expression_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)   171650 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/expression_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)   116102 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/flow_cytometry_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)    65395 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/flow_cytometry_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)   209013 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/flow_cytometry_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)   170947 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/flow_cytometry_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)    74534 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/groups_api.py
+-rw-r--r--   0 root         (0) root         (0)    39937 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/job_operations_api.py
+-rw-r--r--   0 root         (0) root         (0)   126782 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/library_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)    81043 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/library_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)   143643 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/library_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)    96174 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/library_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)    73839 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/linkage_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)    49254 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/linkage_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)    32661 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/manage_data_api.py
+-rw-r--r--   0 root         (0) root         (0)    14530 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/metadata_versioning_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)   614732 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/api/omics_queries_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)   615047 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/omics_queries_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)   127271 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/preparation_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)    81200 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/preparation_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)   144187 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/preparation_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)    96514 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/preparation_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)   139986 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/sample_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)    94653 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/sample_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)   114614 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/sample_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)    76679 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/sample_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)   138955 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/study_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)   138832 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/study_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)   113428 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/study_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)    76738 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/study_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)    23652 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/tasks_api_api.py
+-rw-r--r--   0 root         (0) root         (0)    67595 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/users_api.py
+-rw-r--r--   0 root         (0) root         (0)    12180 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/validation_summary_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)   115980 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/variant_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)    65200 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/variant_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)   215263 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/variant_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)   177497 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/variant_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)    64068 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api/xrefset_queries_api.py
+-rw-r--r--   0 root         (0) root         (0)    27042 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api_client.py
+-rw-r--r--   0 root         (0) root         (0)      652 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/api_response.py
+-rw-r--r--   0 root         (0) root         (0)    16434 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6713 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:01:53.432621 odm_api-1.57.0/odm_api/models/
+-rw-r--r--   0 root         (0) root         (0)     9214 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/applied_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3984 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/attribute_invalid_value.py
+-rw-r--r--   0 root         (0) root         (0)     4024 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/attribute_invalid_value_errors_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4276 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/attribute_validation_summary.py
+-rw-r--r--   0 root         (0) root         (0)     4112 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/attribute_validation_summary_attribute_invalid_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3536 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/base_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     3310 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/base_error_response_error.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/batch_of_ids.py
+-rw-r--r--   0 root         (0) root         (0)     3606 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/commit_info.py
+-rw-r--r--   0 root         (0) root         (0)     5198 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/create_group201_response.py
+-rw-r--r--   0 root         (0) root         (0)     3981 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/create_group201_response_all_of_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4749 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/create_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/create_group_request_members_inner.py
+-rw-r--r--   0 root         (0) root         (0)     5411 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/create_user201_response.py
+-rw-r--r--   0 root         (0) root         (0)     4962 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/create_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     3789 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/create_user_request_emails_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/data_item.py
+-rw-r--r--   0 root         (0) root         (0)     3974 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/data_presentation.py
+-rw-r--r--   0 root         (0) root         (0)     3886 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/data_presentation_relationships.py
+-rw-r--r--   0 root         (0) root         (0)     3829 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/detached_collection.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/detached_collection_data_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/detached_object.py
+-rw-r--r--   0 root         (0) root         (0)     3697 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/email.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/error_message.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/exception_type_and_message.py
+-rw-r--r--   0 root         (0) root         (0)     4647 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/expression_item.py
+-rw-r--r--   0 root         (0) root         (0)     3871 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/expression_response.py
+-rw-r--r--   0 root         (0) root         (0)     5697 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/expression_signal_source.py
+-rw-r--r--   0 root         (0) root         (0)     4846 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/filter_groups_response.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/filter_option.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/filter_option_group.py
+-rw-r--r--   0 root         (0) root         (0)     4837 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/filter_users_response.py
+-rw-r--r--   0 root         (0) root         (0)     4527 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/find_objects_response.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/find_objects_response_filter_option_groups_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/find_objects_response_filter_option_groups_inner_options_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4556 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/find_objects_response_objects_page.py
+-rw-r--r--   0 root         (0) root         (0)     4980 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/find_objects_response_objects_page_content_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/find_objects_response_objects_page_content_inner_summary_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/flow_cytometry_item.py
+-rw-r--r--   0 root         (0) root         (0)     3896 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/flow_cytometry_response.py
+-rw-r--r--   0 root         (0) root         (0)     4015 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/flow_cytometry_signal_source.py
+-rw-r--r--   0 root         (0) root         (0)     4723 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/get_expression_as_curator200_response.py
+-rw-r--r--   0 root         (0) root         (0)     5760 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/get_expression_as_curator200_response_feature.py
+-rw-r--r--   0 root         (0) root         (0)     4278 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/get_flow_cytometry_as_curator200_response.py
+-rw-r--r--   0 root         (0) root         (0)     4442 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/get_variant_as_curator200_response.py
+-rw-r--r--   0 root         (0) root         (0)     4697 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/group.py
+-rw-r--r--   0 root         (0) root         (0)     4265 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/group_patch.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/group_patch_operations_inner.py
+-rw-r--r--   0 root         (0) root         (0)     5142 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/group_response.py
+-rw-r--r--   0 root         (0) root         (0)     3504 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/group_response_all_of_members.py
+-rw-r--r--   0 root         (0) root         (0)     4036 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/group_validation_summary.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/group_validation_summary_attributes_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4279 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/i_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     5640 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/import_expression_signal_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     3891 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/import_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     4198 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/import_signal_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     4405 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/info.py
+-rw-r--r--   0 root         (0) root         (0)     3832 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/job_runtime_error.py
+-rw-r--r--   0 root         (0) root         (0)     3378 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/job_runtime_error_stack_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3587 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/json_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     4903 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/json_metadata_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     3981 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/list_response.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/list_response_meta.py
+-rw-r--r--   0 root         (0) root         (0)     3554 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/list_response_meta_pagination.py
+-rw-r--r--   0 root         (0) root         (0)     3690 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/managed_object.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/member.py
+-rw-r--r--   0 root         (0) root         (0)     3900 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/meta.py
+-rw-r--r--   0 root         (0) root         (0)     3604 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/meta_response.py
+-rw-r--r--   0 root         (0) root         (0)     4321 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/metadata_presentation.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/metadata_presentation_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/metadata_with_id.py
+-rw-r--r--   0 root         (0) root         (0)     3360 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/metainfo_key_for_summary.py
+-rw-r--r--   0 root         (0) root         (0)     4480 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/objects_page.py
+-rw-r--r--   0 root         (0) root         (0)     3613 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/omics_response.py
+-rw-r--r--   0 root         (0) root         (0)     4212 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/omics_response_data_presentation.py
+-rw-r--r--   0 root         (0) root         (0)     4062 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/omics_response_data_presentation_data_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4244 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/omics_response_metadata_presentation.py
+-rw-r--r--   0 root         (0) root         (0)     4387 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/omics_response_metadata_presentation_data_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4105 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/omics_response_metadata_with_id.py
+-rw-r--r--   0 root         (0) root         (0)     4537 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/output.py
+-rw-r--r--   0 root         (0) root         (0)     3840 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/output_errors_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3534 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/page_request.py
+-rw-r--r--   0 root         (0) root         (0)     3506 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/pagination_info.py
+-rw-r--r--   0 root         (0) root         (0)     3765 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/patch_operation.py
+-rw-r--r--   0 root         (0) root         (0)     3822 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/relationships.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/runs_response.py
+-rw-r--r--   0 root         (0) root         (0)     3520 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/sample_source.py
+-rw-r--r--   0 root         (0) root         (0)     4730 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/scim_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/search_study_request.py
+-rw-r--r--   0 root         (0) root         (0)     4303 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/search_study_request_filters_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3578 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/search_study_request_page.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/source_type_pair.py
+-rw-r--r--   0 root         (0) root         (0)     4225 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/start_import_flow_cytometry_request.py
+-rw-r--r--   0 root         (0) root         (0)     3560 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/study_generic_source.py
+-rw-r--r--   0 root         (0) root         (0)     4872 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/study_search_info.py
+-rw-r--r--   0 root         (0) root         (0)     3817 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/study_validation_summary.py
+-rw-r--r--   0 root         (0) root         (0)     4084 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/study_validation_summary_samples_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/task_info.py
+-rw-r--r--   0 root         (0) root         (0)     4910 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/user.py
+-rw-r--r--   0 root         (0) root         (0)     4261 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/user_patch.py
+-rw-r--r--   0 root         (0) root         (0)     5375 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/user_response.py
+-rw-r--r--   0 root         (0) root         (0)     3956 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/validation_error.py
+-rw-r--r--   0 root         (0) root         (0)     4366 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/variant_item.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/variant_response.py
+-rw-r--r--   0 root         (0) root         (0)     3991 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/variant_signal_source.py
+-rw-r--r--   0 root         (0) root         (0)     4399 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/xref_set_create_request.py
+-rw-r--r--   0 root         (0) root         (0)     4616 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/xref_set_create_response.py
+-rw-r--r--   0 root         (0) root         (0)     3837 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/xref_set_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     3900 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/xref_set_search_result.py
+-rw-r--r--   0 root         (0) root         (0)     3618 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/xref_set_search_result_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3642 2024-05-09 11:01:20.000000 odm_api-1.57.0/odm_api/models/xref_set_search_result_result_inner.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/py.typed
+-rw-r--r--   0 root         (0) root         (0)    10142 2024-05-09 11:01:21.000000 odm_api-1.57.0/odm_api/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:01:53.460622 odm_api-1.57.0/odm_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1252 2024-05-09 11:01:53.000000 odm_api-1.57.0/odm_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12680 2024-05-09 11:01:53.000000 odm_api-1.57.0/odm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 11:01:53.000000 odm_api-1.57.0/odm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-09 11:01:53.000000 odm_api-1.57.0/odm_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 11:01:53.000000 odm_api-1.57.0/odm_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1908 2024-05-09 11:01:21.000000 odm_api-1.57.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-09 11:01:53.460622 odm_api-1.57.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2810 2024-05-09 11:01:21.000000 odm_api-1.57.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:01:53.460622 odm_api-1.57.0/test/
+-rw-r--r--   0 root         (0) root         (0)     2210 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_applied_filter.py
+-rw-r--r--   0 root         (0) root         (0)     2352 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_attribute_invalid_value.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_attribute_invalid_value_errors_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_attribute_validation_summary.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_attribute_validation_summary_attribute_invalid_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_base_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     2244 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_base_error_response_error.py
+-rw-r--r--   0 root         (0) root         (0)     2324 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_batch_of_ids.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_commit_info.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_create_group201_response.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_create_group201_response_all_of_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_create_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_create_group_request_members_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3112 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_create_user201_response.py
+-rw-r--r--   0 root         (0) root         (0)     2680 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_create_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_create_user_request_emails_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2723 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_data_import_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)     2077 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_data_item.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_data_presentation.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_data_presentation_relationships.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_detached_collection.py
+-rw-r--r--   0 root         (0) root         (0)     2718 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_detached_collection_data_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2560 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_detached_object.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_email.py
+-rw-r--r--   0 root         (0) root         (0)     2122 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_error_message.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_exception_type_and_message.py
+-rw-r--r--   0 root         (0) root         (0)     6323 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_expression_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     3216 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_expression_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_expression_item.py
+-rw-r--r--   0 root         (0) root         (0)     2420 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_expression_response.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_expression_signal_source.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_expression_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_expression_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_filter_groups_response.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_filter_option.py
+-rw-r--r--   0 root         (0) root         (0)     2314 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_filter_option_group.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_filter_users_response.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_find_objects_response.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_find_objects_response_filter_option_groups_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_find_objects_response_filter_option_groups_inner_options_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_find_objects_response_objects_page.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_find_objects_response_objects_page_content_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_find_objects_response_objects_page_content_inner_summary_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3307 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_flow_cytometry_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_flow_cytometry_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2384 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_flow_cytometry_item.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_flow_cytometry_response.py
+-rw-r--r--   0 root         (0) root         (0)     2392 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_flow_cytometry_signal_source.py
+-rw-r--r--   0 root         (0) root         (0)     3764 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_flow_cytometry_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     3105 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_flow_cytometry_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2649 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_get_expression_as_curator200_response.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_get_expression_as_curator200_response_feature.py
+-rw-r--r--   0 root         (0) root         (0)     2615 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_get_flow_cytometry_as_curator200_response.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_get_variant_as_curator200_response.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_group.py
+-rw-r--r--   0 root         (0) root         (0)     2484 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_group_patch.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_group_patch_operations_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_group_response.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_group_response_all_of_members.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_group_validation_summary.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_group_validation_summary_attributes_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2025 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_groups_api.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_i_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_import_expression_signal_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     2459 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_import_metadata_request.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_import_signal_run_request.py
+-rw-r--r--   0 root         (0) root         (0)     2624 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_job_operations_api.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_job_runtime_error.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_job_runtime_error_stack_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2097 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_json_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2184 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_json_metadata_attributes.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_library_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2354 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_library_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_library_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_library_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_linkage_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2217 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_linkage_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_list_response.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_list_response_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_list_response_meta_pagination.py
+-rw-r--r--   0 root         (0) root         (0)     1678 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_manage_data_api.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_managed_object.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_member.py
+-rw-r--r--   0 root         (0) root         (0)     2219 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_meta_response.py
+-rw-r--r--   0 root         (0) root         (0)     2954 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_metadata_presentation.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_metadata_presentation_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_metadata_versioning_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_metadata_with_id.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_metainfo_key_for_summary.py
+-rw-r--r--   0 root         (0) root         (0)     2430 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_objects_page.py
+-rw-r--r--   0 root         (0) root         (0)     3304 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_omics_queries_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     3241 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_omics_queries_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_omics_response.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_omics_response_data_presentation.py
+-rw-r--r--   0 root         (0) root         (0)     2724 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_omics_response_data_presentation_data_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3553 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_omics_response_metadata_presentation.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_omics_response_metadata_presentation_data_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_omics_response_metadata_with_id.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_output.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_output_errors_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_page_request.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_pagination_info.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_patch_operation.py
+-rw-r--r--   0 root         (0) root         (0)     3406 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_preparation_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_preparation_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_preparation_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_preparation_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2193 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_relationships.py
+-rw-r--r--   0 root         (0) root         (0)     2282 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_runs_response.py
+-rw-r--r--   0 root         (0) root         (0)     2981 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_sample_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_sample_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_sample_source.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_sample_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_sample_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_scim_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_search_study_request.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_search_study_request_filters_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_search_study_request_page.py
+-rw-r--r--   0 root         (0) root         (0)     2154 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_source_type_pair.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_start_import_flow_cytometry_request.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_study_generic_source.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_study_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_study_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_study_search_info.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_study_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_study_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2963 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_study_validation_summary.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_study_validation_summary_samples_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_task_info.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_tasks_api_api.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_user.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_user_patch.py
+-rw-r--r--   0 root         (0) root         (0)     3003 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_user_response.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_users_api.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_validation_error.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_validation_summary_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     3143 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_variant_integration_as_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_variant_integration_as_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2508 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_variant_item.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_variant_response.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_variant_signal_source.py
+-rw-r--r--   0 root         (0) root         (0)     3544 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_variant_spo_tas_curator_api.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_variant_spo_tas_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_xref_set_create_request.py
+-rw-r--r--   0 root         (0) root         (0)     2850 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_xref_set_create_response.py
+-rw-r--r--   0 root         (0) root         (0)     2319 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_xref_set_metadata.py
+-rw-r--r--   0 root         (0) root         (0)     2404 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_xref_set_search_result.py
+-rw-r--r--   0 root         (0) root         (0)     2379 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_xref_set_search_result_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-05-09 11:01:20.000000 odm_api-1.57.0/test/test_xref_set_search_result_result_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2024-05-09 11:01:21.000000 odm_api-1.57.0/test/test_xrefset_queries_api.py
```

### Comparing `odm-api-0.0.1/README.md` & `odm_api-1.57.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 # odm-api
-These API endpoints serve to work with asynchronous tasks.
+This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.
 
+Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).
+
+To try out calls in this swagger page:
+
+1.  Click the 'Authorize' button below to enter your API token
+2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button
+3.  Enter parameter values that you wish to try
+4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears
+
+
+ The server response will be in the section that follows.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: default-released
-- Package version: 0.0.1
+- Package version: 1.57.0
+- Generator version: 7.5.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install git+https://github.com/genestack/odm-openapi.git
+pip install git+https://github.com/genestack/openapi.git
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/genestack/odm-openapi.git`)
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/genestack/openapi.git`)
 
 Then import the package:
 ```python
 import odm_api
 ```
 
 ### Setuptools
@@ -367,18 +379,18 @@
  - [AttributeValidationSummary](docs/AttributeValidationSummary.md)
  - [AttributeValidationSummaryAttributeInvalidValuesInner](docs/AttributeValidationSummaryAttributeInvalidValuesInner.md)
  - [BaseErrorResponse](docs/BaseErrorResponse.md)
  - [BaseErrorResponseError](docs/BaseErrorResponseError.md)
  - [BatchOfIds](docs/BatchOfIds.md)
  - [CommitInfo](docs/CommitInfo.md)
  - [CreateGroup201Response](docs/CreateGroup201Response.md)
+ - [CreateGroup201ResponseAllOfMeta](docs/CreateGroup201ResponseAllOfMeta.md)
  - [CreateGroupRequest](docs/CreateGroupRequest.md)
  - [CreateGroupRequestMembersInner](docs/CreateGroupRequestMembersInner.md)
  - [CreateUser201Response](docs/CreateUser201Response.md)
- - [CreateUser201ResponseAllOfMeta](docs/CreateUser201ResponseAllOfMeta.md)
  - [CreateUserRequest](docs/CreateUserRequest.md)
  - [CreateUserRequestEmailsInner](docs/CreateUserRequestEmailsInner.md)
  - [DataItem](docs/DataItem.md)
  - [DataPresentation](docs/DataPresentation.md)
  - [DataPresentationRelationships](docs/DataPresentationRelationships.md)
  - [DetachedCollection](docs/DetachedCollection.md)
  - [DetachedCollectionDataInner](docs/DetachedCollectionDataInner.md)
@@ -398,32 +410,34 @@
  - [FindObjectsResponseFilterOptionGroupsInnerOptionsInner](docs/FindObjectsResponseFilterOptionGroupsInnerOptionsInner.md)
  - [FindObjectsResponseObjectsPage](docs/FindObjectsResponseObjectsPage.md)
  - [FindObjectsResponseObjectsPageContentInner](docs/FindObjectsResponseObjectsPageContentInner.md)
  - [FindObjectsResponseObjectsPageContentInnerSummaryInner](docs/FindObjectsResponseObjectsPageContentInnerSummaryInner.md)
  - [FlowCytometryItem](docs/FlowCytometryItem.md)
  - [FlowCytometryResponse](docs/FlowCytometryResponse.md)
  - [FlowCytometrySignalSource](docs/FlowCytometrySignalSource.md)
- - [GetExpressionAsUser200Response](docs/GetExpressionAsUser200Response.md)
- - [GetExpressionAsUser200ResponseFeature](docs/GetExpressionAsUser200ResponseFeature.md)
- - [GetExpressionAsUser200ResponseValue](docs/GetExpressionAsUser200ResponseValue.md)
+ - [GetExpressionAsCurator200Response](docs/GetExpressionAsCurator200Response.md)
+ - [GetExpressionAsCurator200ResponseFeature](docs/GetExpressionAsCurator200ResponseFeature.md)
  - [GetFlowCytometryAsCurator200Response](docs/GetFlowCytometryAsCurator200Response.md)
  - [GetVariantAsCurator200Response](docs/GetVariantAsCurator200Response.md)
  - [Group](docs/Group.md)
  - [GroupPatch](docs/GroupPatch.md)
+ - [GroupPatchOperationsInner](docs/GroupPatchOperationsInner.md)
  - [GroupResponse](docs/GroupResponse.md)
+ - [GroupResponseAllOfMembers](docs/GroupResponseAllOfMembers.md)
  - [GroupValidationSummary](docs/GroupValidationSummary.md)
  - [GroupValidationSummaryAttributesInner](docs/GroupValidationSummaryAttributesInner.md)
  - [IMetadata](docs/IMetadata.md)
  - [ImportExpressionSignalRunRequest](docs/ImportExpressionSignalRunRequest.md)
  - [ImportMetadataRequest](docs/ImportMetadataRequest.md)
  - [ImportSignalRunRequest](docs/ImportSignalRunRequest.md)
  - [Info](docs/Info.md)
  - [JobRuntimeError](docs/JobRuntimeError.md)
  - [JobRuntimeErrorStackInner](docs/JobRuntimeErrorStackInner.md)
  - [JsonMetadata](docs/JsonMetadata.md)
+ - [JsonMetadataAttributes](docs/JsonMetadataAttributes.md)
  - [Link](docs/Link.md)
  - [ListResponse](docs/ListResponse.md)
  - [ListResponseMeta](docs/ListResponseMeta.md)
  - [ListResponseMetaPagination](docs/ListResponseMetaPagination.md)
  - [ManagedObject](docs/ManagedObject.md)
  - [Member](docs/Member.md)
  - [Meta](docs/Meta.md)
@@ -456,15 +470,14 @@
  - [StudyGenericSource](docs/StudyGenericSource.md)
  - [StudySearchInfo](docs/StudySearchInfo.md)
  - [StudyValidationSummary](docs/StudyValidationSummary.md)
  - [StudyValidationSummarySamplesInner](docs/StudyValidationSummarySamplesInner.md)
  - [TaskInfo](docs/TaskInfo.md)
  - [User](docs/User.md)
  - [UserPatch](docs/UserPatch.md)
- - [UserPatchOperationsInner](docs/UserPatchOperationsInner.md)
  - [UserResponse](docs/UserResponse.md)
  - [ValidationError](docs/ValidationError.md)
  - [VariantItem](docs/VariantItem.md)
  - [VariantResponse](docs/VariantResponse.md)
  - [VariantSignalSource](docs/VariantSignalSource.md)
  - [XrefSetCreateRequest](docs/XrefSetCreateRequest.md)
  - [XrefSetCreateResponse](docs/XrefSetCreateResponse.md)
```

### Comparing `odm-api-0.0.1/odm_api/__init__.py` & `odm_api-1.57.0/odm_api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.0.1"
+__version__ = "1.57.0"
 
 # import apis into sdk package
 from odm_api.api.data_import_jobs_api import DataImportJobsApi
 from odm_api.api.expression_spo_tas_curator_api import ExpressionSPoTAsCuratorApi
 from odm_api.api.expression_spo_tas_user_api import ExpressionSPoTAsUserApi
 from odm_api.api.expression_integration_as_curator_api import ExpressionIntegrationAsCuratorApi
 from odm_api.api.expression_integration_as_user_api import ExpressionIntegrationAsUserApi
@@ -77,18 +77,18 @@
 from odm_api.models.attribute_validation_summary import AttributeValidationSummary
 from odm_api.models.attribute_validation_summary_attribute_invalid_values_inner import AttributeValidationSummaryAttributeInvalidValuesInner
 from odm_api.models.base_error_response import BaseErrorResponse
 from odm_api.models.base_error_response_error import BaseErrorResponseError
 from odm_api.models.batch_of_ids import BatchOfIds
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.create_group201_response import CreateGroup201Response
+from odm_api.models.create_group201_response_all_of_meta import CreateGroup201ResponseAllOfMeta
 from odm_api.models.create_group_request import CreateGroupRequest
 from odm_api.models.create_group_request_members_inner import CreateGroupRequestMembersInner
 from odm_api.models.create_user201_response import CreateUser201Response
-from odm_api.models.create_user201_response_all_of_meta import CreateUser201ResponseAllOfMeta
 from odm_api.models.create_user_request import CreateUserRequest
 from odm_api.models.create_user_request_emails_inner import CreateUserRequestEmailsInner
 from odm_api.models.data_item import DataItem
 from odm_api.models.data_presentation import DataPresentation
 from odm_api.models.data_presentation_relationships import DataPresentationRelationships
 from odm_api.models.detached_collection import DetachedCollection
 from odm_api.models.detached_collection_data_inner import DetachedCollectionDataInner
@@ -108,32 +108,34 @@
 from odm_api.models.find_objects_response_filter_option_groups_inner_options_inner import FindObjectsResponseFilterOptionGroupsInnerOptionsInner
 from odm_api.models.find_objects_response_objects_page import FindObjectsResponseObjectsPage
 from odm_api.models.find_objects_response_objects_page_content_inner import FindObjectsResponseObjectsPageContentInner
 from odm_api.models.find_objects_response_objects_page_content_inner_summary_inner import FindObjectsResponseObjectsPageContentInnerSummaryInner
 from odm_api.models.flow_cytometry_item import FlowCytometryItem
 from odm_api.models.flow_cytometry_response import FlowCytometryResponse
 from odm_api.models.flow_cytometry_signal_source import FlowCytometrySignalSource
-from odm_api.models.get_expression_as_user200_response import GetExpressionAsUser200Response
-from odm_api.models.get_expression_as_user200_response_feature import GetExpressionAsUser200ResponseFeature
-from odm_api.models.get_expression_as_user200_response_value import GetExpressionAsUser200ResponseValue
+from odm_api.models.get_expression_as_curator200_response import GetExpressionAsCurator200Response
+from odm_api.models.get_expression_as_curator200_response_feature import GetExpressionAsCurator200ResponseFeature
 from odm_api.models.get_flow_cytometry_as_curator200_response import GetFlowCytometryAsCurator200Response
 from odm_api.models.get_variant_as_curator200_response import GetVariantAsCurator200Response
 from odm_api.models.group import Group
 from odm_api.models.group_patch import GroupPatch
+from odm_api.models.group_patch_operations_inner import GroupPatchOperationsInner
 from odm_api.models.group_response import GroupResponse
+from odm_api.models.group_response_all_of_members import GroupResponseAllOfMembers
 from odm_api.models.group_validation_summary import GroupValidationSummary
 from odm_api.models.group_validation_summary_attributes_inner import GroupValidationSummaryAttributesInner
 from odm_api.models.i_metadata import IMetadata
 from odm_api.models.import_expression_signal_run_request import ImportExpressionSignalRunRequest
 from odm_api.models.import_metadata_request import ImportMetadataRequest
 from odm_api.models.import_signal_run_request import ImportSignalRunRequest
 from odm_api.models.info import Info
 from odm_api.models.job_runtime_error import JobRuntimeError
 from odm_api.models.job_runtime_error_stack_inner import JobRuntimeErrorStackInner
 from odm_api.models.json_metadata import JsonMetadata
+from odm_api.models.json_metadata_attributes import JsonMetadataAttributes
 from odm_api.models.link import Link
 from odm_api.models.list_response import ListResponse
 from odm_api.models.list_response_meta import ListResponseMeta
 from odm_api.models.list_response_meta_pagination import ListResponseMetaPagination
 from odm_api.models.managed_object import ManagedObject
 from odm_api.models.member import Member
 from odm_api.models.meta import Meta
@@ -166,15 +168,14 @@
 from odm_api.models.study_generic_source import StudyGenericSource
 from odm_api.models.study_search_info import StudySearchInfo
 from odm_api.models.study_validation_summary import StudyValidationSummary
 from odm_api.models.study_validation_summary_samples_inner import StudyValidationSummarySamplesInner
 from odm_api.models.task_info import TaskInfo
 from odm_api.models.user import User
 from odm_api.models.user_patch import UserPatch
-from odm_api.models.user_patch_operations_inner import UserPatchOperationsInner
 from odm_api.models.user_response import UserResponse
 from odm_api.models.validation_error import ValidationError
 from odm_api.models.variant_item import VariantItem
 from odm_api.models.variant_response import VariantResponse
 from odm_api.models.variant_signal_source import VariantSignalSource
 from odm_api.models.xref_set_create_request import XrefSetCreateRequest
 from odm_api.models.xref_set_create_response import XrefSetCreateResponse
```

### Comparing `odm-api-0.0.1/odm_api/api/__init__.py` & `odm_api-1.57.0/odm_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `odm-api-0.0.1/odm_api/api/data_import_jobs_api.py` & `odm_api-1.57.0/odm_api/api/data_import_jobs_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -266,15 +266,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if allow_dups is not None:
             
             _query_params.append(('allow_dups', allow_dups))
@@ -555,15 +555,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if allow_dups is not None:
             
             _query_params.append(('allow_dups', allow_dups))
@@ -844,15 +844,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if allow_dups is not None:
             
             _query_params.append(('allow_dups', allow_dups))
@@ -1133,15 +1133,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if allow_dups is not None:
             
             _query_params.append(('allow_dups', allow_dups))
@@ -1422,15 +1422,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if allow_dups is not None:
             
             _query_params.append(('allow_dups', allow_dups))
@@ -1711,15 +1711,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if allow_dups is not None:
             
             _query_params.append(('allow_dups', allow_dups))
@@ -2000,15 +2000,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if allow_dups is not None:
             
             _query_params.append(('allow_dups', allow_dups))
```

### Comparing `odm-api-0.0.1/odm_api/api/expression_integration_as_curator_api.py` & `odm_api-1.57.0/odm_api/api/expression_integration_as_curator_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import List, Optional
 from typing_extensions import Annotated
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -276,15 +276,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -556,15 +556,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -849,15 +849,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1130,15 +1130,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1407,15 +1407,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1684,15 +1684,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1961,15 +1961,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -2238,15 +2238,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -2515,15 +2515,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -2792,15 +2792,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -3069,15 +3069,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -3346,15 +3346,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -3675,15 +3675,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -4029,15 +4029,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -4383,15 +4383,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -4711,15 +4711,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -5020,15 +5020,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
@@ -5325,15 +5325,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
@@ -5630,15 +5630,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/expression_integration_as_user_api.py` & `odm_api-1.57.0/odm_api/api/expression_integration_as_user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import List, Optional
 from typing_extensions import Annotated
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -325,15 +325,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -679,15 +679,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1033,15 +1033,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1361,15 +1361,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1670,15 +1670,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
@@ -1975,15 +1975,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
@@ -2280,15 +2280,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/expression_spo_tas_curator_api.py` & `odm_api-1.57.0/odm_api/api/expression_spo_tas_curator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -18,15 +18,15 @@
 
 from pydantic import Field, StrictBool, StrictFloat, StrictInt, StrictStr, field_validator
 from typing import Any, Dict, List, Optional, Union
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.expression_response import ExpressionResponse
 from odm_api.models.expression_signal_source import ExpressionSignalSource
-from odm_api.models.get_expression_as_user200_response import GetExpressionAsUser200Response
+from odm_api.models.get_expression_as_curator200_response import GetExpressionAsCurator200Response
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 from odm_api.models.runs_response import RunsResponse
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -265,15 +265,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -546,15 +546,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -602,15 +602,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> GetExpressionAsUser200Response:
+    ) -> GetExpressionAsCurator200Response:
         """Retrieve a single expression object by ID (accession)
 
 
         :param id: Unique identifier (accession) of the object. (required)
         :type id: str
         :param response_format: Allows to get an extended or updated response body. Available values:  `term_id` - returns extended information including IDs for values and dictionaries;  `multi_values` - returns data with several feature attributes and several sample measurements in the response body in case the original data had them. If not specified, returns only the first feature identifier and the first measurement per sample from the original data.
         :type response_format: List[str]
@@ -645,15 +645,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GetExpressionAsUser200Response",
+            '200': "GetExpressionAsCurator200Response",
             '400': None,
             '401': None,
             '404': None,
             '500': None,
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -680,15 +680,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[GetExpressionAsUser200Response]:
+    ) -> ApiResponse[GetExpressionAsCurator200Response]:
         """Retrieve a single expression object by ID (accession)
 
 
         :param id: Unique identifier (accession) of the object. (required)
         :type id: str
         :param response_format: Allows to get an extended or updated response body. Available values:  `term_id` - returns extended information including IDs for values and dictionaries;  `multi_values` - returns data with several feature attributes and several sample measurements in the response body in case the original data had them. If not specified, returns only the first feature identifier and the first measurement per sample from the original data.
         :type response_format: List[str]
@@ -723,15 +723,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GetExpressionAsUser200Response",
+            '200': "GetExpressionAsCurator200Response",
             '400': None,
             '401': None,
             '404': None,
             '500': None,
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -801,15 +801,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GetExpressionAsUser200Response",
+            '200': "GetExpressionAsCurator200Response",
             '400': None,
             '401': None,
             '404': None,
             '500': None,
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -835,15 +835,15 @@
             'responseFormat': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1150,15 +1150,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -1563,15 +1563,15 @@
             'featureList': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1899,15 +1899,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -2201,15 +2201,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -2471,15 +2471,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -2833,15 +2833,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -3160,15 +3160,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_offset is not None:
@@ -3452,15 +3452,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
```

### Comparing `odm-api-0.0.1/odm_api/api/expression_spo_tas_user_api.py` & `odm_api-1.57.0/odm_api/api/expression_spo_tas_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictFloat, StrictInt, StrictStr, field_validator
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.expression_response import ExpressionResponse
-from odm_api.models.get_expression_as_user200_response import GetExpressionAsUser200Response
+from odm_api.models.get_expression_as_curator200_response import GetExpressionAsCurator200Response
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
 
@@ -57,15 +57,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> GetExpressionAsUser200Response:
+    ) -> GetExpressionAsCurator200Response:
         """Retrieve a single expression object by ID (accession)
 
 
         :param id: Unique identifier (accession) of the object. (required)
         :type id: str
         :param response_format: Allows to get an extended or updated response body. Available values:  `term_id` - returns extended information including IDs for values and dictionaries;  `multi_values` - returns data with several feature attributes and several sample measurements in the response body in case the original data had them. If not specified, returns only the first feature identifier and the first measurement per sample from the original data.
         :type response_format: List[str]
@@ -100,15 +100,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GetExpressionAsUser200Response",
+            '200': "GetExpressionAsCurator200Response",
             '400': None,
             '401': None,
             '404': None,
             '500': None,
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -135,15 +135,15 @@
                 Annotated[StrictFloat, Field(gt=0)]
             ]
         ] = None,
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
-    ) -> ApiResponse[GetExpressionAsUser200Response]:
+    ) -> ApiResponse[GetExpressionAsCurator200Response]:
         """Retrieve a single expression object by ID (accession)
 
 
         :param id: Unique identifier (accession) of the object. (required)
         :type id: str
         :param response_format: Allows to get an extended or updated response body. Available values:  `term_id` - returns extended information including IDs for values and dictionaries;  `multi_values` - returns data with several feature attributes and several sample measurements in the response body in case the original data had them. If not specified, returns only the first feature identifier and the first measurement per sample from the original data.
         :type response_format: List[str]
@@ -178,15 +178,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GetExpressionAsUser200Response",
+            '200': "GetExpressionAsCurator200Response",
             '400': None,
             '401': None,
             '404': None,
             '500': None,
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -256,15 +256,15 @@
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
-            '200': "GetExpressionAsUser200Response",
+            '200': "GetExpressionAsCurator200Response",
             '400': None,
             '401': None,
             '404': None,
             '500': None,
         }
         response_data = self.api_client.call_api(
             *_param,
@@ -290,15 +290,15 @@
             'responseFormat': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -605,15 +605,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -1018,15 +1018,15 @@
             'featureList': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1354,15 +1354,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1656,15 +1656,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1926,15 +1926,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -2288,15 +2288,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -2615,15 +2615,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_offset is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/flow_cytometry_integration_as_curator_api.py` & `odm_api-1.57.0/odm_api/api/flow_cytometry_integration_as_curator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import List, Optional
 from typing_extensions import Annotated
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -289,15 +289,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -570,15 +570,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -847,15 +847,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1124,15 +1124,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1453,15 +1453,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1781,15 +1781,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -2090,15 +2090,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/flow_cytometry_integration_as_user_api.py` & `odm_api-1.57.0/odm_api/api/flow_cytometry_integration_as_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import List, Optional
 from typing_extensions import Annotated
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -325,15 +325,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -653,15 +653,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -962,15 +962,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/flow_cytometry_spo_tas_curator_api.py` & `odm_api-1.57.0/odm_api/api/flow_cytometry_spo_tas_curator_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictFloat, StrictInt, StrictStr, field_validator
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.flow_cytometry_response import FlowCytometryResponse
 from odm_api.models.flow_cytometry_signal_source import FlowCytometrySignalSource
 from odm_api.models.get_flow_cytometry_as_curator200_response import GetFlowCytometryAsCurator200Response
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
@@ -265,15 +265,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -546,15 +546,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -834,15 +834,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1149,15 +1149,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -1586,15 +1586,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1930,15 +1930,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -2232,15 +2232,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -2502,15 +2502,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -2864,15 +2864,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -3191,15 +3191,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_offset is not None:
@@ -3483,15 +3483,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
```

### Comparing `odm-api-0.0.1/odm_api/api/flow_cytometry_spo_tas_user_api.py` & `odm_api-1.57.0/odm_api/api/flow_cytometry_spo_tas_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictFloat, StrictInt, StrictStr, field_validator
-from typing import Optional, Union
+from typing import Any, Dict, List, Optional, Union
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.flow_cytometry_response import FlowCytometryResponse
 from odm_api.models.get_flow_cytometry_as_curator200_response import GetFlowCytometryAsCurator200Response
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 
@@ -289,15 +289,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -604,15 +604,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -1041,15 +1041,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1385,15 +1385,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1687,15 +1687,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1957,15 +1957,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -2319,15 +2319,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -2646,15 +2646,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_offset is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/groups_api.py` & `odm_api-1.57.0/odm_api/api/groups_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -265,15 +265,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -552,15 +552,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -859,15 +859,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if filter is not None:
             
             _query_params.append(('filter', filter))
@@ -1157,15 +1157,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if excluded_attributes is not None:
@@ -1448,15 +1448,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
```

### Comparing `odm-api-0.0.1/odm_api/api/job_operations_api.py` & `odm_api-1.57.0/odm_api/api/job_operations_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -246,15 +246,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if job_exec_id is not None:
             _path_params['jobExecId'] = job_exec_id
         # process the query parameters
         # process the header parameters
@@ -502,15 +502,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if job_exec_id is not None:
             _path_params['jobExecId'] = job_exec_id
         # process the query parameters
         # process the header parameters
@@ -758,15 +758,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if job_exec_id is not None:
             _path_params['jobExecId'] = job_exec_id
         # process the query parameters
         # process the header parameters
@@ -1014,15 +1014,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if job_exec_id is not None:
             _path_params['jobExecId'] = job_exec_id
         # process the query parameters
         # process the header parameters
```

### Comparing `odm-api-0.0.1/odm_api/api/library_integration_as_curator_api.py` & `odm_api-1.57.0/odm_api/api/library_integration_as_curator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -273,15 +273,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -550,15 +550,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -827,15 +827,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1104,15 +1104,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1443,15 +1443,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1761,15 +1761,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -2048,15 +2048,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -2349,15 +2349,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/library_integration_as_user_api.py` & `odm_api-1.57.0/odm_api/api/library_integration_as_user_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -335,15 +335,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -653,15 +653,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -940,15 +940,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1241,15 +1241,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/library_spo_tas_curator_api.py` & `odm_api-1.57.0/odm_api/api/library_spo_tas_curator_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.list_response import ListResponse
 from odm_api.models.sample_source import SampleSource
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
@@ -261,15 +261,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -542,15 +542,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -804,15 +804,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -1118,15 +1118,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1428,15 +1428,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1743,15 +1743,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -2015,15 +2015,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -2371,15 +2371,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -2686,15 +2686,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
```

### Comparing `odm-api-0.0.1/odm_api/api/library_spo_tas_user_api.py` & `odm_api-1.57.0/odm_api/api/library_spo_tas_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.list_response import ListResponse
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -312,15 +312,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -622,15 +622,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -937,15 +937,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -1209,15 +1209,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -1565,15 +1565,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
```

### Comparing `odm-api-0.0.1/odm_api/api/linkage_as_curator_api.py` & `odm_api-1.57.0/odm_api/api/linkage_as_curator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -304,15 +304,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if first_id is not None:
             
             _query_params.append(('firstId', first_id))
@@ -567,15 +567,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -833,15 +833,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if type is not None:
             
             _query_params.append(('type', type))
@@ -1103,15 +1103,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -1449,15 +1449,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if first_id is not None:
             
             _query_params.append(('firstId', first_id))
@@ -1746,15 +1746,15 @@
             'links': '',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
```

### Comparing `odm-api-0.0.1/odm_api/api/linkage_as_user_api.py` & `odm_api-1.57.0/odm_api/api/linkage_as_user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr
-from typing import Optional
+from typing import List, Optional
 from typing_extensions import Annotated
 from odm_api.models.batch_of_ids import BatchOfIds
 from odm_api.models.list_response import ListResponse
 from odm_api.models.source_type_pair import SourceTypePair
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
@@ -248,15 +248,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -514,15 +514,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if type is not None:
             
             _query_params.append(('type', type))
@@ -784,15 +784,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -1130,15 +1130,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if first_id is not None:
             
             _query_params.append(('firstId', first_id))
```

### Comparing `odm-api-0.0.1/odm_api/api/manage_data_api.py` & `odm_api-1.57.0/odm_api/api/manage_data_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -270,15 +270,15 @@
             'accession': 'csv',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if accession is not None:
             
             _query_params.append(('accession', accession))
@@ -570,15 +570,15 @@
             'detachedObjectType': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if detached_object_type is not None:
             
             _query_params.append(('detachedObjectType', detached_object_type))
```

### Comparing `odm-api-0.0.1/odm_api/api/metadata_versioning_as_curator_api.py` & `odm_api-1.57.0/odm_api/api/metadata_versioning_as_curator_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -272,15 +272,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if version_message is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/omics_queries_as_curator_api.py` & `odm_api-1.57.0/odm_api/api/omics_queries_as_curator_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.omics_response import OmicsResponse
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
 
@@ -507,15 +507,15 @@
             'responseFormat': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1100,15 +1100,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1693,15 +1693,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -2286,15 +2286,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -2879,15 +2879,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -3356,15 +3356,15 @@
             'featureList': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if sample_filter is not None:
             
             _query_params.append(('sampleFilter', sample_filter))
@@ -3913,15 +3913,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -4506,15 +4506,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
```

### Comparing `odm-api-0.0.1/odm_api/api/omics_queries_as_user_api.py` & `odm_api-1.57.0/odm_api/api/omics_queries_as_user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.omics_response import OmicsResponse
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
 
@@ -507,15 +507,15 @@
             'responseFormat': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1100,15 +1100,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1693,15 +1693,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -2286,15 +2286,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -2879,15 +2879,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -3356,15 +3356,15 @@
             'featureList': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if sample_filter is not None:
             
             _query_params.append(('sampleFilter', sample_filter))
@@ -3913,15 +3913,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -4506,15 +4506,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
```

### Comparing `odm-api-0.0.1/odm_api/api/preparation_integration_as_curator_api.py` & `odm_api-1.57.0/odm_api/api/preparation_integration_as_curator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -273,15 +273,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -550,15 +550,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -827,15 +827,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1104,15 +1104,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1391,15 +1391,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1678,15 +1678,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1979,15 +1979,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
@@ -2330,15 +2330,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
```

### Comparing `odm-api-0.0.1/odm_api/api/preparation_integration_as_user_api.py` & `odm_api-1.57.0/odm_api/api/preparation_integration_as_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -283,15 +283,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -570,15 +570,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -871,15 +871,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
@@ -1222,15 +1222,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
```

### Comparing `odm-api-0.0.1/odm_api/api/preparation_spo_tas_curator_api.py` & `odm_api-1.57.0/odm_api/api/preparation_spo_tas_curator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.list_response import ListResponse
 from odm_api.models.sample_source import SampleSource
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
@@ -261,15 +261,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -542,15 +542,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -804,15 +804,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -1092,15 +1092,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1407,15 +1407,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -1679,15 +1679,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -1999,15 +1999,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -2371,15 +2371,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -2686,15 +2686,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
```

### Comparing `odm-api-0.0.1/odm_api/api/preparation_spo_tas_user_api.py` & `odm_api-1.57.0/odm_api/api/preparation_spo_tas_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.list_response import ListResponse
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -286,15 +286,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -601,15 +601,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -873,15 +873,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -1193,15 +1193,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1565,15 +1565,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
```

### Comparing `odm-api-0.0.1/odm_api/api/sample_integration_as_curator_api.py` & `odm_api-1.57.0/odm_api/api/sample_integration_as_curator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -272,15 +272,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -549,15 +549,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -826,15 +826,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1103,15 +1103,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1442,15 +1442,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1812,15 +1812,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -2159,15 +2159,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/sample_integration_as_user_api.py` & `odm_api-1.57.0/odm_api/api/sample_integration_as_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -334,15 +334,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -704,15 +704,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1051,15 +1051,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/sample_spo_tas_curator_api.py` & `odm_api-1.57.0/odm_api/api/sample_spo_tas_curator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.list_response import ListResponse
 from odm_api.models.sample_source import SampleSource
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
@@ -261,15 +261,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -542,15 +542,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -830,15 +830,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1145,15 +1145,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -1417,15 +1417,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -1773,15 +1773,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -2088,15 +2088,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
```

### Comparing `odm-api-0.0.1/odm_api/api/sample_spo_tas_user_api.py` & `odm_api-1.57.0/odm_api/api/sample_spo_tas_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.list_response import ListResponse
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -286,15 +286,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -601,15 +601,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -873,15 +873,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -1229,15 +1229,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
```

### Comparing `odm-api-0.0.1/odm_api/api/study_integration_as_curator_api.py` & `odm_api-1.57.0/odm_api/api/study_integration_as_curator_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import Any, Dict, Optional
 from typing_extensions import Annotated
 from odm_api.models.find_objects_response import FindObjectsResponse
 from odm_api.models.list_response import ListResponse
 from odm_api.models.search_study_request import SearchStudyRequest
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
@@ -336,15 +336,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -706,15 +706,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1076,15 +1076,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1394,15 +1394,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1670,15 +1670,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
```

### Comparing `odm-api-0.0.1/odm_api/api/study_integration_as_user_api.py` & `odm_api-1.57.0/odm_api/api/study_integration_as_user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import Any, Dict, Optional
 from typing_extensions import Annotated
 from odm_api.models.find_objects_response import FindObjectsResponse
 from odm_api.models.list_response import ListResponse
 from odm_api.models.search_study_request import SearchStudyRequest
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
@@ -336,15 +336,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -706,15 +706,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1076,15 +1076,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1394,15 +1394,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1670,15 +1670,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
```

### Comparing `odm-api-0.0.1/odm_api/api/study_spo_tas_curator_api.py` & `odm_api-1.57.0/odm_api/api/study_spo_tas_curator_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.list_response import ListResponse
 from odm_api.models.study_generic_source import StudyGenericSource
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
@@ -261,15 +261,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -542,15 +542,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -830,15 +830,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1145,15 +1145,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -1417,15 +1417,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -1773,15 +1773,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -2088,15 +2088,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
```

### Comparing `odm-api-0.0.1/odm_api/api/study_spo_tas_user_api.py` & `odm_api-1.57.0/odm_api/api/study_spo_tas_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.list_response import ListResponse
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -286,15 +286,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -601,15 +601,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -873,15 +873,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -1229,15 +1229,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
```

### Comparing `odm-api-0.0.1/odm_api/api/tasks_api_api.py` & `odm_api-1.57.0/odm_api/api/tasks_api_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -259,15 +259,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -527,15 +527,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if version_message is not None:
             
             _query_params.append(('versionMessage', version_message))
```

### Comparing `odm-api-0.0.1/odm_api/api/users_api.py` & `odm_api-1.57.0/odm_api/api/users_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -268,15 +268,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -552,15 +552,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -849,15 +849,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if filter is not None:
             
             _query_params.append(('filter', filter))
@@ -1133,15 +1133,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -1420,15 +1420,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
```

### Comparing `odm-api-0.0.1/odm_api/api/validation_summary_as_curator_api.py` & `odm_api-1.57.0/odm_api/api/validation_summary_as_curator_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -252,15 +252,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
```

### Comparing `odm-api-0.0.1/odm_api/api/variant_integration_as_curator_api.py` & `odm_api-1.57.0/odm_api/api/variant_integration_as_curator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import List, Optional
 from typing_extensions import Annotated
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -289,15 +289,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -570,15 +570,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -847,15 +847,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1124,15 +1124,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if source_id is not None:
             _path_params['sourceId'] = source_id
         if target_id is not None:
             _path_params['targetId'] = target_id
@@ -1453,15 +1453,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1781,15 +1781,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -2090,15 +2090,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/variant_integration_as_user_api.py` & `odm_api-1.57.0/odm_api/api/variant_integration_as_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import List, Optional
 from typing_extensions import Annotated
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 
 from odm_api.api_client import ApiClient, RequestSerialized
 from odm_api.api_response import ApiResponse
 from odm_api.rest import RESTResponseType
@@ -325,15 +325,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -653,15 +653,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -962,15 +962,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_limit is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/variant_spo_tas_curator_api.py` & `odm_api-1.57.0/odm_api/api/variant_spo_tas_curator_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.get_variant_as_curator200_response import GetVariantAsCurator200Response
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 from odm_api.models.runs_response import RunsResponse
 from odm_api.models.variant_response import VariantResponse
@@ -265,15 +265,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -546,15 +546,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -1019,15 +1019,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -1379,15 +1379,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1694,15 +1694,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -1998,15 +1998,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -2300,15 +2300,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -2570,15 +2570,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -2932,15 +2932,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -3259,15 +3259,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_offset is not None:
@@ -3551,15 +3551,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
```

### Comparing `odm-api-0.0.1/odm_api/api/variant_spo_tas_user_api.py` & `odm_api-1.57.0/odm_api/api/variant_spo_tas_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
 from pydantic import validate_call, Field, StrictFloat, StrictStr, StrictInt
 from typing import Any, Dict, List, Optional, Tuple, Union
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictBool, StrictInt, StrictStr, field_validator
-from typing import Optional
+from typing import Any, Dict, List, Optional
 from typing_extensions import Annotated
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.get_variant_as_curator200_response import GetVariantAsCurator200Response
 from odm_api.models.list_response import ListResponse
 from odm_api.models.metadata_with_id import MetadataWithId
 from odm_api.models.variant_response import VariantResponse
 
@@ -474,15 +474,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -834,15 +834,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1149,15 +1149,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         if version is not None:
             _path_params['version'] = version
@@ -1453,15 +1453,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -1755,15 +1755,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if response_format is not None:
@@ -2025,15 +2025,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -2387,15 +2387,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if response_format is not None:
             
             _query_params.append(('responseFormat', response_format))
@@ -2714,15 +2714,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if page_offset is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api/xrefset_queries_api.py` & `odm_api-1.57.0/odm_api/api/xrefset_queries_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -265,15 +265,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         # process the header parameters
         # process the form parameters
         # process the body parameter
@@ -549,15 +549,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -811,15 +811,15 @@
         _collection_formats: Dict[str, str] = {
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         # process the header parameters
@@ -1120,15 +1120,15 @@
             'targetId': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         # process the query parameters
         if source_id is not None:
             
             _query_params.append(('sourceId', source_id))
@@ -1459,15 +1459,15 @@
             'targetId': 'multi',
         }
 
         _path_params: Dict[str, str] = {}
         _query_params: List[Tuple[str, str]] = []
         _header_params: Dict[str, Optional[str]] = _headers or {}
         _form_params: List[Tuple[str, str]] = []
-        _files: Dict[str, str] = {}
+        _files: Dict[str, Union[str, bytes]] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
         if source_id is not None:
```

### Comparing `odm-api-0.0.1/odm_api/api_client.py` & `odm_api-1.57.0/odm_api/api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -18,15 +18,16 @@
 import json
 import mimetypes
 import os
 import re
 import tempfile
 
 from urllib.parse import quote
-from typing import Tuple, Optional, List, Dict
+from typing import Tuple, Optional, List, Dict, Union
+from pydantic import SecretStr
 
 from odm_api.configuration import Configuration
 from odm_api.api_response import ApiResponse, T as ApiResponseT
 import odm_api.models
 from odm_api import rest
 from odm_api.exceptions import (
     ApiValueError,
@@ -83,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.57.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
@@ -203,15 +204,16 @@
         if post_params or files:
             post_params = post_params if post_params else []
             post_params = self.sanitize_for_serialization(post_params)
             post_params = self.parameters_to_tuples(
                 post_params,
                 collection_formats
             )
-            post_params.extend(self.files_parameters(files))
+            if files:
+                post_params.extend(self.files_parameters(files))
 
         # auth setting
         self.update_params_for_auth(
             header_params,
             query_params,
             auth_settings,
             resource_path,
@@ -308,15 +310,18 @@
             elif response_type is not None:
                 match = None
                 content_type = response_data.getheader('content-type')
                 if content_type is not None:
                     match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
                 encoding = match.group(1) if match else "utf-8"
                 response_text = response_data.data.decode(encoding)
-                return_data = self.deserialize(response_text, response_type)
+                if response_type in ["bytearray", "str"]:
+                    return_data = self.__deserialize_primitive(response_text, response_type)
+                else:
+                    return_data = self.deserialize(response_text, response_type)
         finally:
             if not 200 <= response_data.status <= 299:
                 raise ApiException.from_response(
                     http_resp=response_data,
                     body=response_text,
                     data=return_data,
                 )
@@ -328,26 +333,31 @@
             raw_data = response_data.data
         )
 
     def sanitize_for_serialization(self, obj):
         """Builds a JSON POST object.
 
         If obj is None, return None.
+        If obj is SecretStr, return obj.get_secret_value()
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
             convert to string in iso8601 format.
         If obj is list, sanitize each element in the list.
         If obj is dict, return the dict.
         If obj is OpenAPI model, return the properties dict.
 
         :param obj: The data to serialize.
         :return: The serialized form of data.
         """
         if obj is None:
             return None
+        elif isinstance(obj, Enum):
+            return obj.value
+        elif isinstance(obj, SecretStr):
+            return obj.get_secret_value()
         elif isinstance(obj, self.PRIMITIVE_TYPES):
             return obj
         elif isinstance(obj, list):
             return [
                 self.sanitize_for_serialization(sub_obj) for sub_obj in obj
             ]
         elif isinstance(obj, tuple):
@@ -361,15 +371,18 @@
             obj_dict = obj
         else:
             # Convert model obj to dict except
             # attributes `openapi_types`, `attribute_map`
             # and attributes which value is not None.
             # Convert attribute name to json key in
             # model definition for request.
-            obj_dict = obj.to_dict()
+            if hasattr(obj, 'to_dict') and callable(getattr(obj, 'to_dict')):
+                obj_dict = obj.to_dict()
+            else:
+                obj_dict = obj.__dict__
 
         return {
             key: self.sanitize_for_serialization(val)
             for key, val in obj_dict.items()
         }
 
     def deserialize(self, response_text, response_type):
@@ -500,39 +513,38 @@
                         (k, delimiter.join(quote(str(value)) for value in v))
                     )
             else:
                 new_params.append((k, quote(str(v))))
 
         return "&".join(["=".join(map(str, item)) for item in new_params])
 
-    def files_parameters(self, files=None):
+    def files_parameters(self, files: Dict[str, Union[str, bytes]]):
         """Builds form parameters.
 
         :param files: File parameters.
         :return: Form parameters with files.
         """
         params = []
-
-        if files:
-            for k, v in files.items():
-                if not v:
-                    continue
-                file_names = v if type(v) is list else [v]
-                for n in file_names:
-                    with open(n, 'rb') as f:
-                        filename = os.path.basename(f.name)
-                        filedata = f.read()
-                        mimetype = (
-                            mimetypes.guess_type(filename)[0]
-                            or 'application/octet-stream'
-                        )
-                        params.append(
-                            tuple([k, tuple([filename, filedata, mimetype])])
-                        )
-
+        for k, v in files.items():
+            if isinstance(v, str):
+                with open(v, 'rb') as f:
+                    filename = os.path.basename(f.name)
+                    filedata = f.read()
+            elif isinstance(v, bytes):
+                filename = k
+                filedata = v
+            else:
+                raise ValueError("Unsupported file value")
+            mimetype = (
+                mimetypes.guess_type(filename)[0]
+                or 'application/octet-stream'
+            )
+            params.append(
+                tuple([k, tuple([filename, filedata, mimetype])])
+            )
         return params
 
     def select_header_accept(self, accepts: List[str]) -> Optional[str]:
         """Returns `Accept` based on an array of accepts provided.
 
         :param accepts: List of headers.
         :return: Accept (e.g. application/json).
```

### Comparing `odm-api-0.0.1/odm_api/api_response.py` & `odm_api-1.57.0/odm_api/api_response.py`

 * *Files identical despite different names*

### Comparing `odm-api-0.0.1/odm_api/configuration.py` & `odm_api-1.57.0/odm_api/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -404,15 +404,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: default-released\n"\
-               "SDK Package Version: 0.0.1".\
+               "SDK Package Version: 1.57.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `odm-api-0.0.1/odm_api/exceptions.py` & `odm_api-1.57.0/odm_api/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/odm_api/models/__init__.py` & `odm_api-1.57.0/odm_api/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 # flake8: noqa
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -20,18 +20,18 @@
 from odm_api.models.attribute_validation_summary import AttributeValidationSummary
 from odm_api.models.attribute_validation_summary_attribute_invalid_values_inner import AttributeValidationSummaryAttributeInvalidValuesInner
 from odm_api.models.base_error_response import BaseErrorResponse
 from odm_api.models.base_error_response_error import BaseErrorResponseError
 from odm_api.models.batch_of_ids import BatchOfIds
 from odm_api.models.commit_info import CommitInfo
 from odm_api.models.create_group201_response import CreateGroup201Response
+from odm_api.models.create_group201_response_all_of_meta import CreateGroup201ResponseAllOfMeta
 from odm_api.models.create_group_request import CreateGroupRequest
 from odm_api.models.create_group_request_members_inner import CreateGroupRequestMembersInner
 from odm_api.models.create_user201_response import CreateUser201Response
-from odm_api.models.create_user201_response_all_of_meta import CreateUser201ResponseAllOfMeta
 from odm_api.models.create_user_request import CreateUserRequest
 from odm_api.models.create_user_request_emails_inner import CreateUserRequestEmailsInner
 from odm_api.models.data_item import DataItem
 from odm_api.models.data_presentation import DataPresentation
 from odm_api.models.data_presentation_relationships import DataPresentationRelationships
 from odm_api.models.detached_collection import DetachedCollection
 from odm_api.models.detached_collection_data_inner import DetachedCollectionDataInner
@@ -51,32 +51,34 @@
 from odm_api.models.find_objects_response_filter_option_groups_inner_options_inner import FindObjectsResponseFilterOptionGroupsInnerOptionsInner
 from odm_api.models.find_objects_response_objects_page import FindObjectsResponseObjectsPage
 from odm_api.models.find_objects_response_objects_page_content_inner import FindObjectsResponseObjectsPageContentInner
 from odm_api.models.find_objects_response_objects_page_content_inner_summary_inner import FindObjectsResponseObjectsPageContentInnerSummaryInner
 from odm_api.models.flow_cytometry_item import FlowCytometryItem
 from odm_api.models.flow_cytometry_response import FlowCytometryResponse
 from odm_api.models.flow_cytometry_signal_source import FlowCytometrySignalSource
-from odm_api.models.get_expression_as_user200_response import GetExpressionAsUser200Response
-from odm_api.models.get_expression_as_user200_response_feature import GetExpressionAsUser200ResponseFeature
-from odm_api.models.get_expression_as_user200_response_value import GetExpressionAsUser200ResponseValue
+from odm_api.models.get_expression_as_curator200_response import GetExpressionAsCurator200Response
+from odm_api.models.get_expression_as_curator200_response_feature import GetExpressionAsCurator200ResponseFeature
 from odm_api.models.get_flow_cytometry_as_curator200_response import GetFlowCytometryAsCurator200Response
 from odm_api.models.get_variant_as_curator200_response import GetVariantAsCurator200Response
 from odm_api.models.group import Group
 from odm_api.models.group_patch import GroupPatch
+from odm_api.models.group_patch_operations_inner import GroupPatchOperationsInner
 from odm_api.models.group_response import GroupResponse
+from odm_api.models.group_response_all_of_members import GroupResponseAllOfMembers
 from odm_api.models.group_validation_summary import GroupValidationSummary
 from odm_api.models.group_validation_summary_attributes_inner import GroupValidationSummaryAttributesInner
 from odm_api.models.i_metadata import IMetadata
 from odm_api.models.import_expression_signal_run_request import ImportExpressionSignalRunRequest
 from odm_api.models.import_metadata_request import ImportMetadataRequest
 from odm_api.models.import_signal_run_request import ImportSignalRunRequest
 from odm_api.models.info import Info
 from odm_api.models.job_runtime_error import JobRuntimeError
 from odm_api.models.job_runtime_error_stack_inner import JobRuntimeErrorStackInner
 from odm_api.models.json_metadata import JsonMetadata
+from odm_api.models.json_metadata_attributes import JsonMetadataAttributes
 from odm_api.models.link import Link
 from odm_api.models.list_response import ListResponse
 from odm_api.models.list_response_meta import ListResponseMeta
 from odm_api.models.list_response_meta_pagination import ListResponseMetaPagination
 from odm_api.models.managed_object import ManagedObject
 from odm_api.models.member import Member
 from odm_api.models.meta import Meta
@@ -109,15 +111,14 @@
 from odm_api.models.study_generic_source import StudyGenericSource
 from odm_api.models.study_search_info import StudySearchInfo
 from odm_api.models.study_validation_summary import StudyValidationSummary
 from odm_api.models.study_validation_summary_samples_inner import StudyValidationSummarySamplesInner
 from odm_api.models.task_info import TaskInfo
 from odm_api.models.user import User
 from odm_api.models.user_patch import UserPatch
-from odm_api.models.user_patch_operations_inner import UserPatchOperationsInner
 from odm_api.models.user_response import UserResponse
 from odm_api.models.validation_error import ValidationError
 from odm_api.models.variant_item import VariantItem
 from odm_api.models.variant_response import VariantResponse
 from odm_api.models.variant_signal_source import VariantSignalSource
 from odm_api.models.xref_set_create_request import XrefSetCreateRequest
 from odm_api.models.xref_set_create_response import XrefSetCreateResponse
```

### Comparing `odm-api-0.0.1/odm_api/models/applied_filter.py` & `odm_api-1.57.0/odm_api/models/exception_type_and_message.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,58 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AppliedFilter(BaseModel):
+class ExceptionTypeAndMessage(BaseModel):
     """
-    AppliedFilter
+    ExceptionTypeAndMessage
     """ # noqa: E501
     type: Optional[StrictStr] = None
-    filter_option_id: Optional[StrictStr] = Field(default=None, alias="filterOptionId")
-    match: Optional[StrictStr] = None
-    mode: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["type", "filterOptionId", "match", "mode"]
-
-    @field_validator('type')
-    def type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['FULL_TEXT', 'SELECT']):
-            raise ValueError("must be one of enum values ('FULL_TEXT', 'SELECT')")
-        return value
-
-    @field_validator('mode')
-    def mode_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['STRICT', 'USE_NARROWER_TERMS']):
-            raise ValueError("must be one of enum values ('STRICT', 'USE_NARROWER_TERMS')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    message: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["type", "message"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AppliedFilter from a JSON string"""
+        """Create an instance of ExceptionTypeAndMessage from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -91,23 +69,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AppliedFilter from a dict"""
+        """Create an instance of ExceptionTypeAndMessage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "type": obj.get("type"),
-            "filterOptionId": obj.get("filterOptionId"),
-            "match": obj.get("match"),
-            "mode": obj.get("mode")
+            "message": obj.get("message")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/attribute_invalid_value.py` & `odm_api-1.57.0/odm_api/models/email.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,69 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt
+from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.attribute_invalid_value_errors_inner import AttributeInvalidValueErrorsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AttributeInvalidValue(BaseModel):
+class Email(BaseModel):
     """
-    AttributeInvalidValue
+    Email
     """ # noqa: E501
-    value: Optional[Dict[str, Any]] = None
-    count: Optional[StrictInt] = None
-    errors: Optional[List[AttributeInvalidValueErrorsInner]] = None
-    __properties: ClassVar[List[str]] = ["value", "count", "errors"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    type: Optional[StrictStr] = None
+    value: Optional[StrictStr] = None
+    primary: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["type", "value", "primary"]
+
+    @field_validator('type')
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in set(['work']):
+            raise ValueError("must be one of enum values ('work')")
+        return value
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AttributeInvalidValue from a JSON string"""
+        """Create an instance of Email from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,33 +76,26 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in errors (list)
-        _items = []
-        if self.errors:
-            for _item in self.errors:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['errors'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AttributeInvalidValue from a dict"""
+        """Create an instance of Email from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "type": obj.get("type"),
             "value": obj.get("value"),
-            "count": obj.get("count"),
-            "errors": [AttributeInvalidValueErrorsInner.from_dict(_item) for _item in obj["errors"]] if obj.get("errors") is not None else None
+            "primary": obj.get("primary")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/attribute_invalid_value_errors_inner.py` & `odm_api-1.57.0/odm_api/models/commit_info.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,99 +1,95 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AttributeInvalidValueErrorsInner(BaseModel):
+class CommitInfo(BaseModel):
     """
-    AttributeInvalidValueErrorsInner
+    CommitInfo
     """ # noqa: E501
-    error_type: Optional[StrictStr] = Field(default=None, alias="errorType")
-    error_message: Optional[StrictStr] = Field(default=None, alias="errorMessage")
-    __properties: ClassVar[List[str]] = ["errorType", "errorMessage"]
-
-    @field_validator('error_type')
-    def error_type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['VALUE_NOT_SET', 'VOCABULARY_NOT_FOUND', 'TYPE_NOT_MATCH', 'MISSING_ATTRIBUTE', 'SYNONYM_ATTRIBUTE']):
-            raise ValueError("must be one of enum values ('VALUE_NOT_SET', 'VOCABULARY_NOT_FOUND', 'TYPE_NOT_MATCH', 'MISSING_ATTRIBUTE', 'SYNONYM_ATTRIBUTE')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    author: Optional[StrictStr] = None
+    message: Optional[StrictStr] = None
+    timestamp: Optional[StrictInt] = None
+    version: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["author", "message", "timestamp", "version"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AttributeInvalidValueErrorsInner from a JSON string"""
+        """Create an instance of CommitInfo from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "version",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AttributeInvalidValueErrorsInner from a dict"""
+        """Create an instance of CommitInfo from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "errorType": obj.get("errorType"),
-            "errorMessage": obj.get("errorMessage")
+            "author": obj.get("author"),
+            "message": obj.get("message"),
+            "timestamp": obj.get("timestamp"),
+            "version": obj.get("version")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/attribute_validation_summary.py` & `odm_api-1.57.0/test/test_attribute_validation_summary_attribute_invalid_values_inner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,97 +1,55 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-from __future__ import annotations
-import pprint
-import re  # noqa: F401
-import json
+import unittest
 
-from pydantic import BaseModel, Field, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
 from odm_api.models.attribute_validation_summary_attribute_invalid_values_inner import AttributeValidationSummaryAttributeInvalidValuesInner
-from typing import Optional, Set
-from typing_extensions import Self
 
-class AttributeValidationSummary(BaseModel):
-    """
-    AttributeValidationSummary
-    """ # noqa: E501
-    attribute_name: Optional[StrictStr] = Field(default=None, alias="attributeName")
-    attribute_invalid_values: Optional[List[AttributeValidationSummaryAttributeInvalidValuesInner]] = Field(default=None, alias="attributeInvalidValues")
-    __properties: ClassVar[List[str]] = ["attributeName", "attributeInvalidValues"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
-
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.model_dump(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AttributeValidationSummary from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Return the dictionary representation of the model using alias.
-
-        This has the following differences from calling pydantic's
-        `self.model_dump(by_alias=True)`:
-
-        * `None` is only added to the output dict for nullable fields that
-          were set at model initialization. Other fields with value `None`
-          are ignored.
-        """
-        excluded_fields: Set[str] = set([
-        ])
+class TestAttributeValidationSummaryAttributeInvalidValuesInner(unittest.TestCase):
+    """AttributeValidationSummaryAttributeInvalidValuesInner unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
 
-        _dict = self.model_dump(
-            by_alias=True,
-            exclude=excluded_fields,
-            exclude_none=True,
+    def make_instance(self, include_optional) -> AttributeValidationSummaryAttributeInvalidValuesInner:
+        """Test AttributeValidationSummaryAttributeInvalidValuesInner
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `AttributeValidationSummaryAttributeInvalidValuesInner`
+        """
+        model = AttributeValidationSummaryAttributeInvalidValuesInner()
+        if include_optional:
+            return AttributeValidationSummaryAttributeInvalidValuesInner(
+                value = None,
+                count = 56,
+                errors = [
+                    {errorType=VALUE_NOT_SET, errorMessage=errorMessage}
+                    ]
+            )
+        else:
+            return AttributeValidationSummaryAttributeInvalidValuesInner(
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in attribute_invalid_values (list)
-        _items = []
-        if self.attribute_invalid_values:
-            for _item in self.attribute_invalid_values:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['attributeInvalidValues'] = _items
-        return _dict
-
-    @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AttributeValidationSummary from a dict"""
-        if obj is None:
-            return None
-
-        if not isinstance(obj, dict):
-            return cls.model_validate(obj)
-
-        _obj = cls.model_validate({
-            "attributeName": obj.get("attributeName"),
-            "attributeInvalidValues": [AttributeValidationSummaryAttributeInvalidValuesInner.from_dict(_item) for _item in obj["attributeInvalidValues"]] if obj.get("attributeInvalidValues") is not None else None
-        })
-        return _obj
+        """
 
+    def testAttributeValidationSummaryAttributeInvalidValuesInner(self):
+        """Test AttributeValidationSummaryAttributeInvalidValuesInner"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `odm-api-0.0.1/odm_api/models/attribute_validation_summary_attribute_invalid_values_inner.py` & `odm_api-1.57.0/odm_api/models/group_validation_summary_attributes_inner.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.attribute_invalid_value_errors_inner import AttributeInvalidValueErrorsInner
+from odm_api.models.attribute_validation_summary_attribute_invalid_values_inner import AttributeValidationSummaryAttributeInvalidValuesInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class AttributeValidationSummaryAttributeInvalidValuesInner(BaseModel):
+class GroupValidationSummaryAttributesInner(BaseModel):
     """
-    AttributeValidationSummaryAttributeInvalidValuesInner
+    GroupValidationSummaryAttributesInner
     """ # noqa: E501
-    value: Optional[Dict[str, Any]] = None
-    count: Optional[StrictInt] = None
-    errors: Optional[List[AttributeInvalidValueErrorsInner]] = None
-    __properties: ClassVar[List[str]] = ["value", "count", "errors"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    attribute_name: Optional[StrictStr] = Field(default=None, alias="attributeName")
+    attribute_invalid_values: Optional[List[AttributeValidationSummaryAttributeInvalidValuesInner]] = Field(default=None, alias="attributeInvalidValues")
+    __properties: ClassVar[List[str]] = ["attributeName", "attributeInvalidValues"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of AttributeValidationSummaryAttributeInvalidValuesInner from a JSON string"""
+        """Create an instance of GroupValidationSummaryAttributesInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,33 +66,32 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in errors (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in attribute_invalid_values (list)
         _items = []
-        if self.errors:
-            for _item in self.errors:
+        if self.attribute_invalid_values:
+            for _item in self.attribute_invalid_values:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['errors'] = _items
+            _dict['attributeInvalidValues'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of AttributeValidationSummaryAttributeInvalidValuesInner from a dict"""
+        """Create an instance of GroupValidationSummaryAttributesInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "value": obj.get("value"),
-            "count": obj.get("count"),
-            "errors": [AttributeInvalidValueErrorsInner.from_dict(_item) for _item in obj["errors"]] if obj.get("errors") is not None else None
+            "attributeName": obj.get("attributeName"),
+            "attributeInvalidValues": [AttributeValidationSummaryAttributeInvalidValuesInner.from_dict(_item) for _item in obj["attributeInvalidValues"]] if obj.get("attributeInvalidValues") is not None else None
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/base_error_response.py` & `odm_api-1.57.0/odm_api/models/metainfo_key_for_summary.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel
-from typing import Any, ClassVar, Dict, List
-from odm_api.models.base_error_response_error import BaseErrorResponseError
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class BaseErrorResponse(BaseModel):
+class MetainfoKeyForSummary(BaseModel):
     """
-    BaseErrorResponse
+    MetainfoKeyForSummary
     """ # noqa: E501
-    error: BaseErrorResponseError
-    __properties: ClassVar[List[str]] = ["error"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    key: Optional[StrictStr] = None
+    values: Optional[List[StrictStr]] = None
+    __properties: ClassVar[List[str]] = ["key", "values"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of BaseErrorResponse from a JSON string"""
+        """Create an instance of MetainfoKeyForSummary from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,27 +65,25 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of error
-        if self.error:
-            _dict['error'] = self.error.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of BaseErrorResponse from a dict"""
+        """Create an instance of MetainfoKeyForSummary from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "error": BaseErrorResponseError.from_dict(obj["error"]) if obj.get("error") is not None else None
+            "key": obj.get("key"),
+            "values": obj.get("values")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/base_error_response_error.py` & `odm_api-1.57.0/odm_api/models/job_runtime_error_stack_inner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class BaseErrorResponseError(BaseModel):
+class JobRuntimeErrorStackInner(BaseModel):
     """
-    BaseErrorResponseError
+    JobRuntimeErrorStackInner
     """ # noqa: E501
-    message: StrictStr = Field(description="Detailed error message")
-    __properties: ClassVar[List[str]] = ["message"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    type: Optional[StrictStr] = None
+    message: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["type", "message"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of BaseErrorResponseError from a JSON string"""
+        """Create an instance of JobRuntimeErrorStackInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,20 +69,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of BaseErrorResponseError from a dict"""
+        """Create an instance of JobRuntimeErrorStackInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "type": obj.get("type"),
             "message": obj.get("message")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/batch_of_ids.py` & `odm_api-1.57.0/odm_api/models/metadata_with_id.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,93 +1,91 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class BatchOfIds(BaseModel):
+class MetadataWithId(BaseModel):
     """
-    Request model for getting links by many IDs.
+    MetadataWithId
     """ # noqa: E501
-    first_type: StrictStr = Field(description="Type of the objects.", alias="firstType")
-    first_ids: List[StrictStr] = Field(description="Array of the object IDs with the same type.", alias="firstIds")
-    offset: Optional[StrictInt] = Field(default=None, description="Param says to skip that many links before beginning to return links. Default: 0.")
-    limit: Optional[StrictInt] = Field(default=None, description="Param says to limit the count of returned links. Default: 1000.")
-    __properties: ClassVar[List[str]] = ["firstType", "firstIds", "offset", "limit"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    item_id: Optional[StrictStr] = Field(default=None, alias="itemId")
+    metadata: Optional[Dict[str, Any]] = None
+    __properties: ClassVar[List[str]] = ["itemId", "metadata"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of BatchOfIds from a JSON string"""
+        """Create an instance of MetadataWithId from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "item_id",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of BatchOfIds from a dict"""
+        """Create an instance of MetadataWithId from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "firstType": obj.get("firstType"),
-            "firstIds": obj.get("firstIds"),
-            "offset": obj.get("offset"),
-            "limit": obj.get("limit")
+            "itemId": obj.get("itemId"),
+            "metadata": obj.get("metadata")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/commit_info.py` & `odm_api-1.57.0/odm_api/models/data_item.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,89 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CommitInfo(BaseModel):
+class DataItem(BaseModel):
     """
-    CommitInfo
+    DataItem
     """ # noqa: E501
-    author: Optional[StrictStr] = None
-    message: Optional[StrictStr] = None
-    timestamp: Optional[StrictInt] = None
-    version: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["author", "message", "timestamp", "version"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    item_id: Optional[StrictStr] = Field(default=None, alias="itemId")
+    metadata: Optional[Dict[str, Any]] = None
+    __properties: ClassVar[List[str]] = ["itemId", "metadata"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CommitInfo from a JSON string"""
+        """Create an instance of DataItem from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "version",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CommitInfo from a dict"""
+        """Create an instance of DataItem from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "author": obj.get("author"),
-            "message": obj.get("message"),
-            "timestamp": obj.get("timestamp"),
-            "version": obj.get("version")
+            "itemId": obj.get("itemId"),
+            "metadata": obj.get("metadata")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/create_group201_response.py` & `odm_api-1.57.0/odm_api/models/start_import_flow_cytometry_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,71 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.create_group_request_members_inner import CreateGroupRequestMembersInner
-from odm_api.models.create_user201_response_all_of_meta import CreateUser201ResponseAllOfMeta
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateGroup201Response(BaseModel):
+class StartImportFlowCytometryRequest(BaseModel):
     """
-    CreateGroup201Response
+    import signal data request
     """ # noqa: E501
-    external_id: Optional[StrictStr] = Field(default=None, description="External unique resource id", alias="externalId")
-    id: Optional[StrictStr] = Field(default=None, description="Unique resource id")
-    schemas: Optional[List[StrictStr]] = None
-    members: Optional[List[CreateGroupRequestMembersInner]] = None
-    display_name: StrictStr = Field(alias="displayName")
-    meta: Optional[CreateUser201ResponseAllOfMeta] = None
-    __properties: ClassVar[List[str]] = ["externalId", "id", "schemas", "members", "displayName", "meta"]
+    source: Optional[StrictStr] = None
+    metadata_link: Optional[StrictStr] = Field(default=None, alias="metadataLink")
+    data_link: StrictStr = Field(alias="dataLink")
+    template_id: Optional[StrictStr] = Field(default=None, alias="templateId")
+    previous_version: Optional[StrictStr] = Field(default=None, alias="previousVersion")
+    __properties: ClassVar[List[str]] = ["source", "metadataLink", "dataLink", "templateId", "previousVersion"]
 
-    @field_validator('schemas')
-    def schemas_validate_enum(cls, value):
+    @field_validator('source')
+    def source_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        for i in value:
-            if i not in set(['urn:ietf:params:scim:schemas:core:2.0:Group']):
-                raise ValueError("each list item must be one of ('urn:ietf:params:scim:schemas:core:2.0:Group')")
+        if value not in set(['ARVADOS', 'S3', 'HTTP']):
+            raise ValueError("must be one of enum values ('ARVADOS', 'S3', 'HTTP')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateGroup201Response from a JSON string"""
+        """Create an instance of StartImportFlowCytometryRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,39 +78,28 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in members (list)
-        _items = []
-        if self.members:
-            for _item in self.members:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['members'] = _items
-        # override the default output from pydantic by calling `to_dict()` of meta
-        if self.meta:
-            _dict['meta'] = self.meta.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateGroup201Response from a dict"""
+        """Create an instance of StartImportFlowCytometryRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "externalId": obj.get("externalId"),
-            "id": obj.get("id"),
-            "schemas": obj.get("schemas"),
-            "members": [CreateGroupRequestMembersInner.from_dict(_item) for _item in obj["members"]] if obj.get("members") is not None else None,
-            "displayName": obj.get("displayName"),
-            "meta": CreateUser201ResponseAllOfMeta.from_dict(obj["meta"]) if obj.get("meta") is not None else None
+            "source": obj.get("source"),
+            "metadataLink": obj.get("metadataLink"),
+            "dataLink": obj.get("dataLink"),
+            "templateId": obj.get("templateId"),
+            "previousVersion": obj.get("previousVersion")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/create_group_request.py` & `odm_api-1.57.0/odm_api/models/link.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,60 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.create_group_request_members_inner import CreateGroupRequestMembersInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateGroupRequest(BaseModel):
+class Link(BaseModel):
     """
-    CreateGroupRequest
+    Link between two objects. Each of them represented as a unique pair of ID (accession) and unique type.
     """ # noqa: E501
-    external_id: Optional[StrictStr] = Field(default=None, description="External unique resource id", alias="externalId")
-    id: Optional[StrictStr] = Field(default=None, description="Unique resource id")
-    schemas: Optional[List[StrictStr]] = None
-    members: Optional[List[CreateGroupRequestMembersInner]] = None
-    display_name: StrictStr = Field(alias="displayName")
-    __properties: ClassVar[List[str]] = ["externalId", "id", "schemas", "members", "displayName"]
-
-    @field_validator('schemas')
-    def schemas_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        for i in value:
-            if i not in set(['urn:ietf:params:scim:schemas:core:2.0:Group']):
-                raise ValueError("each list item must be one of ('urn:ietf:params:scim:schemas:core:2.0:Group')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    first_id: Optional[StrictStr] = Field(default=None, description="Object ID (accession) (e.g. accession of study)", alias="firstId")
+    first_type: Optional[StrictStr] = Field(default=None, description="Type of the object (e.g. study)", alias="firstType")
+    second_id: Optional[StrictStr] = Field(default=None, description="Object ID (accession) (e.g. accession of study)", alias="secondId")
+    second_type: Optional[StrictStr] = Field(default=None, description="Type of the object (e.g. study)", alias="secondType")
+    __properties: ClassVar[List[str]] = ["firstId", "firstType", "secondId", "secondType"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateGroupRequest from a JSON string"""
+        """Create an instance of Link from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -80,35 +67,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in members (list)
-        _items = []
-        if self.members:
-            for _item in self.members:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['members'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateGroupRequest from a dict"""
+        """Create an instance of Link from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "externalId": obj.get("externalId"),
-            "id": obj.get("id"),
-            "schemas": obj.get("schemas"),
-            "members": [CreateGroupRequestMembersInner.from_dict(_item) for _item in obj["members"]] if obj.get("members") is not None else None,
-            "displayName": obj.get("displayName")
+            "firstId": obj.get("firstId"),
+            "firstType": obj.get("firstType"),
+            "secondId": obj.get("secondId"),
+            "secondType": obj.get("secondType")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/create_group_request_members_inner.py` & `odm_api-1.57.0/odm_api/models/pagination_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateGroupRequestMembersInner(BaseModel):
+class PaginationInfo(BaseModel):
     """
-    CreateGroupRequestMembersInner
+    PaginationInfo
     """ # noqa: E501
-    value: StrictStr
-    display: Optional[StrictStr] = None
-    ref: StrictStr = Field(description="The URI of the member resource", alias="$ref")
-    __properties: ClassVar[List[str]] = ["value", "display", "$ref"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    count: Optional[StrictInt] = None
+    total: Optional[StrictInt] = None
+    offset: Optional[StrictInt] = None
+    limit: Optional[StrictInt] = None
+    __properties: ClassVar[List[str]] = ["count", "total", "offset", "limit"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateGroupRequestMembersInner from a JSON string"""
+        """Create an instance of PaginationInfo from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -70,22 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateGroupRequestMembersInner from a dict"""
+        """Create an instance of PaginationInfo from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "value": obj.get("value"),
-            "display": obj.get("display"),
-            "$ref": obj.get("$ref")
+            "count": obj.get("count"),
+            "total": obj.get("total"),
+            "offset": obj.get("offset"),
+            "limit": obj.get("limit")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/create_user201_response.py` & `odm_api-1.57.0/odm_api/models/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,75 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.create_user201_response_all_of_meta import CreateUser201ResponseAllOfMeta
 from odm_api.models.create_user_request_emails_inner import CreateUserRequestEmailsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateUser201Response(BaseModel):
+class User(BaseModel):
     """
-    CreateUser201Response
+    User
     """ # noqa: E501
     active: StrictBool = Field(description="User status")
     emails: List[CreateUserRequestEmailsInner]
     external_id: Optional[StrictStr] = Field(default=None, description="External unique resource id", alias="externalId")
     id: Optional[StrictStr] = Field(default=None, description="Unique resource id")
     schemas: Optional[List[StrictStr]] = None
     user_name: Optional[StrictStr] = Field(default=None, alias="userName")
     display_name: StrictStr = Field(alias="displayName")
-    meta: Optional[CreateUser201ResponseAllOfMeta] = None
-    __properties: ClassVar[List[str]] = ["active", "emails", "externalId", "id", "schemas", "userName", "displayName", "meta"]
+    __properties: ClassVar[List[str]] = ["active", "emails", "externalId", "id", "schemas", "userName", "displayName"]
 
     @field_validator('schemas')
     def schemas_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
         for i in value:
             if i not in set(['urn:ietf:params:scim:schemas:core:2.0:User']):
                 raise ValueError("each list item must be one of ('urn:ietf:params:scim:schemas:core:2.0:User')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateUser201Response from a JSON string"""
+        """Create an instance of User from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -91,34 +89,30 @@
         # override the default output from pydantic by calling `to_dict()` of each item in emails (list)
         _items = []
         if self.emails:
             for _item in self.emails:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['emails'] = _items
-        # override the default output from pydantic by calling `to_dict()` of meta
-        if self.meta:
-            _dict['meta'] = self.meta.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateUser201Response from a dict"""
+        """Create an instance of User from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "active": obj.get("active"),
             "emails": [CreateUserRequestEmailsInner.from_dict(_item) for _item in obj["emails"]] if obj.get("emails") is not None else None,
             "externalId": obj.get("externalId"),
             "id": obj.get("id"),
             "schemas": obj.get("schemas"),
             "userName": obj.get("userName"),
-            "displayName": obj.get("displayName"),
-            "meta": CreateUser201ResponseAllOfMeta.from_dict(obj["meta"]) if obj.get("meta") is not None else None
+            "displayName": obj.get("displayName")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/create_user201_response_all_of_meta.py` & `odm_api-1.57.0/odm_api/models/create_user_request_emails_inner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,69 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateUser201ResponseAllOfMeta(BaseModel):
+class CreateUserRequestEmailsInner(BaseModel):
     """
-    resource metadata
+    CreateUserRequestEmailsInner
     """ # noqa: E501
-    created: Optional[datetime] = None
-    last_modified: Optional[datetime] = Field(default=None, alias="lastModified")
-    resource_type: Optional[StrictStr] = Field(default=None, alias="resourceType")
-    __properties: ClassVar[List[str]] = ["created", "lastModified", "resourceType"]
+    type: Optional[StrictStr] = None
+    value: Optional[StrictStr] = None
+    primary: Optional[StrictBool] = None
+    __properties: ClassVar[List[str]] = ["type", "value", "primary"]
 
-    @field_validator('resource_type')
-    def resource_type_validate_enum(cls, value):
+    @field_validator('type')
+    def type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['User', 'Group']):
-            raise ValueError("must be one of enum values ('User', 'Group')")
+        if value not in set(['work']):
+            raise ValueError("must be one of enum values ('work')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateUser201ResponseAllOfMeta from a JSON string"""
+        """Create an instance of CreateUserRequestEmailsInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -81,22 +80,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateUser201ResponseAllOfMeta from a dict"""
+        """Create an instance of CreateUserRequestEmailsInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "created": obj.get("created"),
-            "lastModified": obj.get("lastModified"),
-            "resourceType": obj.get("resourceType")
+            "type": obj.get("type"),
+            "value": obj.get("value"),
+            "primary": obj.get("primary")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/create_user_request.py` & `odm_api-1.57.0/odm_api/models/flow_cytometry_signal_source.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,118 +1,95 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.create_user_request_emails_inner import CreateUserRequestEmailsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateUserRequest(BaseModel):
+class FlowCytometrySignalSource(BaseModel):
     """
-    CreateUserRequest
+    FlowCytometrySignalSource
     """ # noqa: E501
-    active: StrictBool = Field(description="User status")
-    emails: List[CreateUserRequestEmailsInner]
-    external_id: Optional[StrictStr] = Field(default=None, description="External unique resource id", alias="externalId")
-    id: Optional[StrictStr] = Field(default=None, description="Unique resource id")
-    schemas: Optional[List[StrictStr]] = None
-    user_name: Optional[StrictStr] = Field(default=None, alias="userName")
-    display_name: StrictStr = Field(alias="displayName")
-    __properties: ClassVar[List[str]] = ["active", "emails", "externalId", "id", "schemas", "userName", "displayName"]
-
-    @field_validator('schemas')
-    def schemas_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        for i in value:
-            if i not in set(['urn:ietf:params:scim:schemas:core:2.0:User']):
-                raise ValueError("each list item must be one of ('urn:ietf:params:scim:schemas:core:2.0:User')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    template_id: Optional[StrictStr] = Field(default=None, description="ID of template file.", alias="templateId")
+    link: StrictStr = Field(description="URL of the signal file.")
+    metadata_link: Optional[StrictStr] = Field(default=None, description="URL of the signal file metadata.", alias="metadataLink")
+    previous_version: Optional[StrictStr] = Field(default=None, description="Accession of matrix group or matrix group version chain.", alias="previousVersion")
+    __properties: ClassVar[List[str]] = ["templateId", "link", "metadataLink", "previousVersion"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateUserRequest from a JSON string"""
+        """Create an instance of FlowCytometrySignalSource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "template_id",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in emails (list)
-        _items = []
-        if self.emails:
-            for _item in self.emails:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['emails'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateUserRequest from a dict"""
+        """Create an instance of FlowCytometrySignalSource from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "active": obj.get("active"),
-            "emails": [CreateUserRequestEmailsInner.from_dict(_item) for _item in obj["emails"]] if obj.get("emails") is not None else None,
-            "externalId": obj.get("externalId"),
-            "id": obj.get("id"),
-            "schemas": obj.get("schemas"),
-            "userName": obj.get("userName"),
-            "displayName": obj.get("displayName")
+            "templateId": obj.get("templateId"),
+            "link": obj.get("link"),
+            "metadataLink": obj.get("metadataLink"),
+            "previousVersion": obj.get("previousVersion")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/create_user_request_emails_inner.py` & `odm_api-1.57.0/odm_api/models/filter_option.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,60 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictBool, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreateUserRequestEmailsInner(BaseModel):
+class FilterOption(BaseModel):
     """
-    CreateUserRequestEmailsInner
+    FilterOption
     """ # noqa: E501
-    type: Optional[StrictStr] = None
-    value: Optional[StrictStr] = None
-    primary: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["type", "value", "primary"]
-
-    @field_validator('type')
-    def type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['work']):
-            raise ValueError("must be one of enum values ('work')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    id: Optional[StrictStr] = None
+    filter_id: Optional[StrictStr] = Field(default=None, alias="filterId")
+    name: Optional[StrictStr] = None
+    count: Optional[StrictInt] = None
+    __properties: ClassVar[List[str]] = ["id", "filterId", "name", "count"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreateUserRequestEmailsInner from a JSON string"""
+        """Create an instance of FilterOption from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -80,22 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreateUserRequestEmailsInner from a dict"""
+        """Create an instance of FilterOption from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "type": obj.get("type"),
-            "value": obj.get("value"),
-            "primary": obj.get("primary")
+            "id": obj.get("id"),
+            "filterId": obj.get("filterId"),
+            "name": obj.get("name"),
+            "count": obj.get("count")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/data_item.py` & `odm_api-1.57.0/odm_api/models/omics_response_metadata_with_id.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from odm_api.models.metadata_with_id import MetadataWithId
 from typing import Optional, Set
 from typing_extensions import Self
 
-class DataItem(BaseModel):
+class OmicsResponseMetadataWithId(BaseModel):
     """
-    DataItem
+    OmicsResponseMetadataWithId
     """ # noqa: E501
-    item_id: Optional[StrictStr] = Field(default=None, alias="itemId")
-    metadata: Optional[Dict[str, Any]] = None
-    __properties: ClassVar[List[str]] = ["itemId", "metadata"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    data: Optional[List[MetadataWithId]] = None
+    results_exhausted: Optional[StrictBool] = Field(default=None, alias="resultsExhausted")
+    log: Optional[List[StrictStr]] = None
+    cursor: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["data", "resultsExhausted", "log", "cursor"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of DataItem from a JSON string"""
+        """Create an instance of OmicsResponseMetadataWithId from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,25 +68,34 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
+        _items = []
+        if self.data:
+            for _item in self.data:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['data'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of DataItem from a dict"""
+        """Create an instance of OmicsResponseMetadataWithId from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "itemId": obj.get("itemId"),
-            "metadata": obj.get("metadata")
+            "data": [MetadataWithId.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None,
+            "resultsExhausted": obj.get("resultsExhausted"),
+            "log": obj.get("log"),
+            "cursor": obj.get("cursor")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/data_presentation.py` & `odm_api-1.57.0/odm_api/models/data_presentation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from odm_api.models.data_presentation_relationships import DataPresentationRelationships
 from typing import Optional, Set
 from typing_extensions import Self
 
 class DataPresentation(BaseModel):
     """
     DataPresentation
     """ # noqa: E501
     item_id: Optional[StrictStr] = Field(default=None, alias="itemId")
     metadata: Optional[Dict[str, Any]] = None
     relationships: Optional[DataPresentationRelationships] = None
     __properties: ClassVar[List[str]] = ["itemId", "metadata", "relationships"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `odm-api-0.0.1/odm_api/models/data_presentation_relationships.py` & `odm_api-1.57.0/odm_api/models/list_response_meta_pagination.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,93 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class DataPresentationRelationships(BaseModel):
+class ListResponseMetaPagination(BaseModel):
     """
-    DataPresentationRelationships
+    ListResponseMetaPagination
     """ # noqa: E501
-    sample: Optional[StrictStr] = None
-    cell: Optional[StrictStr] = None
-    library: Optional[StrictStr] = None
-    preparation: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["sample", "cell", "library", "preparation"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    count: Optional[StrictInt] = None
+    total: Optional[StrictInt] = None
+    offset: Optional[StrictInt] = None
+    limit: Optional[StrictInt] = None
+    __properties: ClassVar[List[str]] = ["count", "total", "offset", "limit"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of DataPresentationRelationships from a JSON string"""
+        """Create an instance of ListResponseMetaPagination from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "sample",
-            "cell",
-            "library",
-            "preparation",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of DataPresentationRelationships from a dict"""
+        """Create an instance of ListResponseMetaPagination from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "sample": obj.get("sample"),
-            "cell": obj.get("cell"),
-            "library": obj.get("library"),
-            "preparation": obj.get("preparation")
+            "count": obj.get("count"),
+            "total": obj.get("total"),
+            "offset": obj.get("offset"),
+            "limit": obj.get("limit")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/detached_collection.py` & `odm_api-1.57.0/odm_api/models/search_study_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.detached_collection_data_inner import DetachedCollectionDataInner
+from odm_api.models.search_study_request_filters_inner import SearchStudyRequestFiltersInner
+from odm_api.models.search_study_request_page import SearchStudyRequestPage
 from typing import Optional, Set
 from typing_extensions import Self
 
-class DetachedCollection(BaseModel):
+class SearchStudyRequest(BaseModel):
     """
-    DetachedCollection
+    SearchStudyRequest
     """ # noqa: E501
-    data: List[DetachedCollectionDataInner]
-    cursor: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["data", "cursor"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    filters: Optional[List[SearchStudyRequestFiltersInner]] = None
+    page: Optional[SearchStudyRequestPage] = None
+    __properties: ClassVar[List[str]] = ["filters", "page"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of DetachedCollection from a JSON string"""
+        """Create an instance of SearchStudyRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,32 +67,35 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in filters (list)
         _items = []
-        if self.data:
-            for _item in self.data:
+        if self.filters:
+            for _item in self.filters:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['data'] = _items
+            _dict['filters'] = _items
+        # override the default output from pydantic by calling `to_dict()` of page
+        if self.page:
+            _dict['page'] = self.page.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of DetachedCollection from a dict"""
+        """Create an instance of SearchStudyRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "data": [DetachedCollectionDataInner.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None,
-            "cursor": obj.get("cursor")
+            "filters": [SearchStudyRequestFiltersInner.from_dict(_item) for _item in obj["filters"]] if obj.get("filters") is not None else None,
+            "page": SearchStudyRequestPage.from_dict(obj["page"]) if obj.get("page") is not None else None
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/detached_collection_data_inner.py` & `odm_api-1.57.0/odm_api/models/group_patch_operations_inner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,66 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from pydantic import BaseModel, Field, StrictStr, field_validator
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class DetachedCollectionDataInner(BaseModel):
+class GroupPatchOperationsInner(BaseModel):
     """
-    DetachedCollectionDataInner
+    GroupPatchOperationsInner
     """ # noqa: E501
-    genestackaccession: StrictStr = Field(alias="genestack:accession")
-    detached_object_type: StrictStr = Field(alias="detachedObjectType")
-    owner_email: StrictStr = Field(alias="ownerEmail")
-    created_at: datetime = Field(alias="createdAt")
-    __properties: ClassVar[List[str]] = ["genestack:accession", "detachedObjectType", "ownerEmail", "createdAt"]
+    op: StrictStr
+    path: Optional[StrictStr] = None
+    value: Optional[Dict[str, Any]] = Field(default=None, description="Corresponding 'value' of that field specified by 'path'")
+    __properties: ClassVar[List[str]] = ["op", "path", "value"]
 
-    @field_validator('detached_object_type')
-    def detached_object_type_validate_enum(cls, value):
+    @field_validator('op')
+    def op_validate_enum(cls, value):
         """Validates the enum"""
-        if value not in set(['SAMPLE_GROUP', 'LIBRARY_GROUP', 'PREPARATION_GROUP', 'TABULAR_DATA', 'GENE_VARIANT', 'FLOW_CYTOMETRY']):
-            raise ValueError("must be one of enum values ('SAMPLE_GROUP', 'LIBRARY_GROUP', 'PREPARATION_GROUP', 'TABULAR_DATA', 'GENE_VARIANT', 'FLOW_CYTOMETRY')")
+        if value not in set(['add', 'replace', 'remove']):
+            raise ValueError("must be one of enum values ('add', 'replace', 'remove')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of DetachedCollectionDataInner from a JSON string"""
+        """Create an instance of GroupPatchOperationsInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,23 +77,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of DetachedCollectionDataInner from a dict"""
+        """Create an instance of GroupPatchOperationsInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "genestack:accession": obj.get("genestack:accession"),
-            "detachedObjectType": obj.get("detachedObjectType"),
-            "ownerEmail": obj.get("ownerEmail"),
-            "createdAt": obj.get("createdAt")
+            "op": obj.get("op"),
+            "path": obj.get("path"),
+            "value": obj.get("value")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/detached_object.py` & `odm_api-1.57.0/odm_api/models/xref_set_search_result_entry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from pydantic import BaseModel, Field, StrictStr, field_validator
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class DetachedObject(BaseModel):
+class XrefSetSearchResultEntry(BaseModel):
     """
-    DetachedObject
+    XrefSetSearchResultEntry
     """ # noqa: E501
-    genestackaccession: StrictStr = Field(alias="genestack:accession")
-    detached_object_type: StrictStr = Field(alias="detachedObjectType")
-    owner_email: StrictStr = Field(alias="ownerEmail")
-    created_at: datetime = Field(alias="createdAt")
-    __properties: ClassVar[List[str]] = ["genestack:accession", "detachedObjectType", "ownerEmail", "createdAt"]
-
-    @field_validator('detached_object_type')
-    def detached_object_type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value not in set(['SAMPLE_GROUP', 'LIBRARY_GROUP', 'PREPARATION_GROUP', 'TABULAR_DATA', 'GENE_VARIANT', 'FLOW_CYTOMETRY']):
-            raise ValueError("must be one of enum values ('SAMPLE_GROUP', 'LIBRARY_GROUP', 'PREPARATION_GROUP', 'TABULAR_DATA', 'GENE_VARIANT', 'FLOW_CYTOMETRY')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    xref_set_id: Optional[StrictStr] = Field(default=None, alias="xrefSetId")
+    source_id: Optional[StrictStr] = Field(default=None, alias="sourceId")
+    target_ids: Optional[List[StrictStr]] = Field(default=None, alias="targetIds")
+    __properties: ClassVar[List[str]] = ["xrefSetId", "sourceId", "targetIds"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of DetachedObject from a JSON string"""
+        """Create an instance of XrefSetSearchResultEntry from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,23 +70,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of DetachedObject from a dict"""
+        """Create an instance of XrefSetSearchResultEntry from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "genestack:accession": obj.get("genestack:accession"),
-            "detachedObjectType": obj.get("detachedObjectType"),
-            "ownerEmail": obj.get("ownerEmail"),
-            "createdAt": obj.get("createdAt")
+            "xrefSetId": obj.get("xrefSetId"),
+            "sourceId": obj.get("sourceId"),
+            "targetIds": obj.get("targetIds")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/email.py` & `odm_api-1.57.0/odm_api/models/import_signal_run_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictBool, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Email(BaseModel):
+class ImportSignalRunRequest(BaseModel):
     """
-    Email
+    import signal data request
     """ # noqa: E501
-    type: Optional[StrictStr] = None
-    value: Optional[StrictStr] = None
-    primary: Optional[StrictBool] = None
-    __properties: ClassVar[List[str]] = ["type", "value", "primary"]
+    source: Optional[StrictStr] = None
+    metadata_link: Optional[StrictStr] = Field(default=None, alias="metadataLink")
+    data_link: StrictStr = Field(alias="dataLink")
+    template_id: Optional[StrictStr] = Field(default=None, alias="templateId")
+    previous_version: Optional[StrictStr] = Field(default=None, alias="previousVersion")
+    __properties: ClassVar[List[str]] = ["source", "metadataLink", "dataLink", "templateId", "previousVersion"]
 
-    @field_validator('type')
-    def type_validate_enum(cls, value):
+    @field_validator('source')
+    def source_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['work']):
-            raise ValueError("must be one of enum values ('work')")
+        if value not in set(['ARVADOS', 'S3', 'HTTP']):
+            raise ValueError("must be one of enum values ('ARVADOS', 'S3', 'HTTP')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Email from a JSON string"""
+        """Create an instance of ImportSignalRunRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -80,22 +82,24 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Email from a dict"""
+        """Create an instance of ImportSignalRunRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "type": obj.get("type"),
-            "value": obj.get("value"),
-            "primary": obj.get("primary")
+            "source": obj.get("source"),
+            "metadataLink": obj.get("metadataLink"),
+            "dataLink": obj.get("dataLink"),
+            "templateId": obj.get("templateId"),
+            "previousVersion": obj.get("previousVersion")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/error_message.py` & `odm_api-1.57.0/odm_api/models/list_response_meta.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict
+from typing import Any, ClassVar, Dict, List, Optional
+from odm_api.models.list_response_meta_pagination import ListResponseMetaPagination
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ErrorMessage(BaseModel):
+class ListResponseMeta(BaseModel):
     """
-    ErrorMessage
+    ListResponseMeta
     """ # noqa: E501
-    message: StrictStr = Field(description="Detailed error message")
-    __properties: ClassVar[List[str]] = ["message"]
+    pagination: Optional[ListResponseMetaPagination] = None
+    __properties: ClassVar[List[str]] = ["pagination"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ErrorMessage from a JSON string"""
+        """Create an instance of ListResponseMeta from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -64,24 +65,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of pagination
+        if self.pagination:
+            _dict['pagination'] = self.pagination.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ErrorMessage from a dict"""
+        """Create an instance of ListResponseMeta from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "message": obj.get("message")
+            "pagination": ListResponseMetaPagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/exception_type_and_message.py` & `odm_api-1.57.0/odm_api/models/find_objects_response_filter_option_groups_inner_options_inner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ExceptionTypeAndMessage(BaseModel):
+class FindObjectsResponseFilterOptionGroupsInnerOptionsInner(BaseModel):
     """
-    ExceptionTypeAndMessage
+    FindObjectsResponseFilterOptionGroupsInnerOptionsInner
     """ # noqa: E501
-    type: Optional[StrictStr] = None
-    message: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["type", "message"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    id: Optional[StrictStr] = None
+    filter_id: Optional[StrictStr] = Field(default=None, alias="filterId")
+    name: Optional[StrictStr] = None
+    count: Optional[StrictInt] = None
+    __properties: ClassVar[List[str]] = ["id", "filterId", "name", "count"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ExceptionTypeAndMessage from a JSON string"""
+        """Create an instance of FindObjectsResponseFilterOptionGroupsInnerOptionsInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,21 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ExceptionTypeAndMessage from a dict"""
+        """Create an instance of FindObjectsResponseFilterOptionGroupsInnerOptionsInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "type": obj.get("type"),
-            "message": obj.get("message")
+            "id": obj.get("id"),
+            "filterId": obj.get("filterId"),
+            "name": obj.get("name"),
+            "count": obj.get("count")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/expression_item.py` & `odm_api-1.57.0/odm_api/models/flow_cytometry_item.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,101 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional, Union
-from odm_api.models.get_expression_as_user200_response_feature import GetExpressionAsUser200ResponseFeature
-from odm_api.models.get_expression_as_user200_response_value import GetExpressionAsUser200ResponseValue
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ExpressionItem(BaseModel):
+class FlowCytometryItem(BaseModel):
     """
-    ExpressionItem
+    FlowCytometryItem
     """ # noqa: E501
     item_id: Optional[StrictStr] = Field(default=None, alias="itemId")
     metadata: Optional[Dict[str, Any]] = None
     run_id: Optional[StrictStr] = Field(default=None, alias="runId")
     group_id: Optional[StrictStr] = Field(default=None, alias="groupId")
-    gene: Optional[StrictStr] = None
+    readout_type: Optional[StrictStr] = Field(default=None, alias="readoutType")
+    cell_population: Optional[StrictStr] = Field(default=None, alias="cellPopulation")
+    marker: Optional[StrictStr] = None
     expression: Optional[Union[StrictFloat, StrictInt]] = None
-    feature: Optional[GetExpressionAsUser200ResponseFeature] = None
-    value: Optional[GetExpressionAsUser200ResponseValue] = None
-    description: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["itemId", "metadata", "runId", "groupId", "gene", "expression", "feature", "value", "description"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    __properties: ClassVar[List[str]] = ["itemId", "metadata", "runId", "groupId", "readoutType", "cellPopulation", "marker", "expression"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ExpressionItem from a JSON string"""
+        """Create an instance of FlowCytometryItem from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "description",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of feature
-        if self.feature:
-            _dict['feature'] = self.feature.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of value
-        if self.value:
-            _dict['value'] = self.value.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ExpressionItem from a dict"""
+        """Create an instance of FlowCytometryItem from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "itemId": obj.get("itemId"),
             "metadata": obj.get("metadata"),
             "runId": obj.get("runId"),
             "groupId": obj.get("groupId"),
-            "gene": obj.get("gene"),
-            "expression": obj.get("expression"),
-            "feature": GetExpressionAsUser200ResponseFeature.from_dict(obj["feature"]) if obj.get("feature") is not None else None,
-            "value": GetExpressionAsUser200ResponseValue.from_dict(obj["value"]) if obj.get("value") is not None else None,
-            "description": obj.get("description")
+            "readoutType": obj.get("readoutType"),
+            "cellPopulation": obj.get("cellPopulation"),
+            "marker": obj.get("marker"),
+            "expression": obj.get("expression")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/expression_response.py` & `odm_api-1.57.0/odm_api/models/json_metadata.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.get_expression_as_user200_response import GetExpressionAsUser200Response
+from odm_api.models.json_metadata_attributes import JsonMetadataAttributes
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ExpressionResponse(BaseModel):
+class JsonMetadata(BaseModel):
     """
-    ExpressionResponse
+    JsonMetadata
     """ # noqa: E501
-    data: Optional[List[GetExpressionAsUser200Response]] = None
-    cursor: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["data", "cursor"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    attributes: Optional[JsonMetadataAttributes] = None
+    __properties: ClassVar[List[str]] = ["attributes"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ExpressionResponse from a JSON string"""
+        """Create an instance of JsonMetadata from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,32 +65,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
-        _items = []
-        if self.data:
-            for _item in self.data:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['data'] = _items
+        # override the default output from pydantic by calling `to_dict()` of attributes
+        if self.attributes:
+            _dict['attributes'] = self.attributes.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ExpressionResponse from a dict"""
+        """Create an instance of JsonMetadata from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "data": [GetExpressionAsUser200Response.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None,
-            "cursor": obj.get("cursor")
+            "attributes": JsonMetadataAttributes.from_dict(obj["attributes"]) if obj.get("attributes") is not None else None
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/expression_signal_source.py` & `odm_api-1.57.0/odm_api/models/expression_signal_source.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ExpressionSignalSource(BaseModel):
     """
     ExpressionSignalSource
@@ -31,19 +31,19 @@
     metadata_link: Optional[StrictStr] = Field(default=None, description="URL of the signal file metadata.", alias="metadataLink")
     previous_version: Optional[StrictStr] = Field(default=None, description="Accession of matrix group or matrix group version chain.", alias="previousVersion")
     number_of_feature_attributes: Optional[StrictInt] = Field(default=None, description="Integer value that specifies the number of columns related to the feature in the uploaded data frame, and indicates the starting position of the sample data. This attribute is not needed if the uploaded file is in GCT format.", alias="numberOfFeatureAttributes")
     data_class: Optional[StrictStr] = Field(default=None, description="A mandatory parameter with the following possible values: `Bulk transcriptomics`, `Single-cell transcriptomics`, `Differential abundance (FC, pval, etc.)`, `Pathway analysis`, `Proteomics`, `Single-cell proteomics`, `Metabolomics`, `Epigenomics`, `DNA methylation`, `Chemoinformatics`, `Imaging features`, `Gene panel data`, `Biomarker data`, `Physical measures`, `Blood counts`, `Other body fluid counts`, `Nanopore`, `Other`.  In case the parameter is not set the dataClass is automatically defined as `Other`.", alias="dataClass")
     measurement_separator: Optional[StrictStr] = Field(default=None, description="This parameter is necessary when your file contains multiple measurement columns for each sample, library, or preparation. It represents the character that distinguishes the sample/library/preparation name from the measurement name in column headers. Supported separators include `. , : ; _ - /  |`, with the allowance for multi-character separators.", alias="measurementSeparator")
     __properties: ClassVar[List[str]] = ["templateId", "link", "metadataLink", "previousVersion", "numberOfFeatureAttributes", "dataClass", "measurementSeparator"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `odm-api-0.0.1/odm_api/models/filter_groups_response.py` & `odm_api-1.57.0/odm_api/models/create_group201_response_all_of_meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,73 +1,70 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr, field_validator
+from datetime import datetime
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.create_group201_response import CreateGroup201Response
 from typing import Optional, Set
 from typing_extensions import Self
 
-class FilterGroupsResponse(BaseModel):
+class CreateGroup201ResponseAllOfMeta(BaseModel):
     """
-    FilterGroupsResponse
+    resource metadata
     """ # noqa: E501
-    resources: Optional[List[CreateGroup201Response]] = Field(default=None, description="List of groups", alias="Resources")
-    items_per_page: Optional[StrictInt] = Field(default=None, alias="itemsPerPage")
-    schemas: Optional[List[StrictStr]] = None
-    start_index: Optional[StrictInt] = Field(default=None, alias="startIndex")
-    total_results: Optional[StrictInt] = Field(default=None, alias="totalResults")
-    __properties: ClassVar[List[str]] = ["Resources", "itemsPerPage", "schemas", "startIndex", "totalResults"]
+    created: Optional[datetime] = None
+    last_modified: Optional[datetime] = Field(default=None, alias="lastModified")
+    resource_type: Optional[StrictStr] = Field(default=None, alias="resourceType")
+    __properties: ClassVar[List[str]] = ["created", "lastModified", "resourceType"]
 
-    @field_validator('schemas')
-    def schemas_validate_enum(cls, value):
+    @field_validator('resource_type')
+    def resource_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        for i in value:
-            if i not in set(['urn:ietf:params:scim:api:messages:2.0:ListResponse']):
-                raise ValueError("each list item must be one of ('urn:ietf:params:scim:api:messages:2.0:ListResponse')")
+        if value not in set(['User', 'Group']):
+            raise ValueError("must be one of enum values ('User', 'Group')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of FilterGroupsResponse from a JSON string"""
+        """Create an instance of CreateGroup201ResponseAllOfMeta from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -80,35 +77,26 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in resources (list)
-        _items = []
-        if self.resources:
-            for _item in self.resources:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['Resources'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of FilterGroupsResponse from a dict"""
+        """Create an instance of CreateGroup201ResponseAllOfMeta from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "Resources": [CreateGroup201Response.from_dict(_item) for _item in obj["Resources"]] if obj.get("Resources") is not None else None,
-            "itemsPerPage": obj.get("itemsPerPage"),
-            "schemas": obj.get("schemas"),
-            "startIndex": obj.get("startIndex"),
-            "totalResults": obj.get("totalResults")
+            "created": obj.get("created"),
+            "lastModified": obj.get("lastModified"),
+            "resourceType": obj.get("resourceType")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/filter_option.py` & `odm_api-1.57.0/test/test_study_search_info.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,61 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-from __future__ import annotations
-import pprint
-import re  # noqa: F401
-import json
-
-from pydantic import BaseModel, Field, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
-from typing import Optional, Set
-from typing_extensions import Self
-
-class FilterOption(BaseModel):
-    """
-    FilterOption
-    """ # noqa: E501
-    id: Optional[StrictStr] = None
-    filter_id: Optional[StrictStr] = Field(default=None, alias="filterId")
-    name: Optional[StrictStr] = None
-    count: Optional[StrictInt] = None
-    __properties: ClassVar[List[str]] = ["id", "filterId", "name", "count"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
-
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.model_dump(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of FilterOption from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Return the dictionary representation of the model using alias.
-
-        This has the following differences from calling pydantic's
-        `self.model_dump(by_alias=True)`:
-
-        * `None` is only added to the output dict for nullable fields that
-          were set at model initialization. Other fields with value `None`
-          are ignored.
-        """
-        excluded_fields: Set[str] = set([
-        ])
+import unittest
 
-        _dict = self.model_dump(
-            by_alias=True,
-            exclude=excluded_fields,
-            exclude_none=True,
-        )
-        return _dict
+from odm_api.models.study_search_info import StudySearchInfo
+
+class TestStudySearchInfo(unittest.TestCase):
+    """StudySearchInfo unit test stubs"""
+
+    def setUp(self):
+        pass
 
-    @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of FilterOption from a dict"""
-        if obj is None:
-            return None
-
-        if not isinstance(obj, dict):
-            return cls.model_validate(obj)
-
-        _obj = cls.model_validate({
-            "id": obj.get("id"),
-            "filterId": obj.get("filterId"),
-            "name": obj.get("name"),
-            "count": obj.get("count")
-        })
-        return _obj
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional) -> StudySearchInfo:
+        """Test StudySearchInfo
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `StudySearchInfo`
+        """
+        model = StudySearchInfo()
+        if include_optional:
+            return StudySearchInfo(
+                accession = '',
+                name = '',
+                owner = '',
+                file_creation = '',
+                size = 56,
+                has_facs = True,
+                has_genomic = True,
+                has_transcriptomics = True,
+                summary = [
+                    {values=[values, values], key=key}
+                    ]
+            )
+        else:
+            return StudySearchInfo(
+        )
+        """
 
+    def testStudySearchInfo(self):
+        """Test StudySearchInfo"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `odm-api-0.0.1/odm_api/models/filter_users_response.py` & `odm_api-1.57.0/odm_api/models/filter_users_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from odm_api.models.create_user201_response import CreateUser201Response
 from typing import Optional, Set
 from typing_extensions import Self
 
 class FilterUsersResponse(BaseModel):
     """
@@ -41,19 +41,19 @@
             return value
 
         for i in value:
             if i not in set(['urn:ietf:params:scim:api:messages:2.0:ListResponse']):
                 raise ValueError("each list item must be one of ('urn:ietf:params:scim:api:messages:2.0:ListResponse')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `odm-api-0.0.1/odm_api/models/find_objects_response.py` & `odm_api-1.57.0/odm_api/models/objects_page.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.find_objects_response_filter_option_groups_inner import FindObjectsResponseFilterOptionGroupsInner
-from odm_api.models.find_objects_response_objects_page import FindObjectsResponseObjectsPage
+from odm_api.models.find_objects_response_objects_page_content_inner import FindObjectsResponseObjectsPageContentInner
+from odm_api.models.search_study_request_page import SearchStudyRequestPage
 from typing import Optional, Set
 from typing_extensions import Self
 
-class FindObjectsResponse(BaseModel):
+class ObjectsPage(BaseModel):
     """
-    FindObjectsResponse
+    ObjectsPage
     """ # noqa: E501
-    objects_page: Optional[FindObjectsResponseObjectsPage] = Field(default=None, alias="objectsPage")
-    filter_option_groups: Optional[List[FindObjectsResponseFilterOptionGroupsInner]] = Field(default=None, alias="filterOptionGroups")
-    __properties: ClassVar[List[str]] = ["objectsPage", "filterOptionGroups"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    filtered_count: Optional[StrictInt] = Field(default=None, alias="filteredCount")
+    page_request: Optional[SearchStudyRequestPage] = Field(default=None, alias="pageRequest")
+    content: Optional[List[FindObjectsResponseObjectsPageContentInner]] = None
+    __properties: ClassVar[List[str]] = ["filteredCount", "pageRequest", "content"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of FindObjectsResponse from a JSON string"""
+        """Create an instance of ObjectsPage from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,35 +68,36 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of objects_page
-        if self.objects_page:
-            _dict['objectsPage'] = self.objects_page.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in filter_option_groups (list)
+        # override the default output from pydantic by calling `to_dict()` of page_request
+        if self.page_request:
+            _dict['pageRequest'] = self.page_request.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in content (list)
         _items = []
-        if self.filter_option_groups:
-            for _item in self.filter_option_groups:
+        if self.content:
+            for _item in self.content:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['filterOptionGroups'] = _items
+            _dict['content'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of FindObjectsResponse from a dict"""
+        """Create an instance of ObjectsPage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "objectsPage": FindObjectsResponseObjectsPage.from_dict(obj["objectsPage"]) if obj.get("objectsPage") is not None else None,
-            "filterOptionGroups": [FindObjectsResponseFilterOptionGroupsInner.from_dict(_item) for _item in obj["filterOptionGroups"]] if obj.get("filterOptionGroups") is not None else None
+            "filteredCount": obj.get("filteredCount"),
+            "pageRequest": SearchStudyRequestPage.from_dict(obj["pageRequest"]) if obj.get("pageRequest") is not None else None,
+            "content": [FindObjectsResponseObjectsPageContentInner.from_dict(_item) for _item in obj["content"]] if obj.get("content") is not None else None
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/find_objects_response_filter_option_groups_inner.py` & `odm_api-1.57.0/odm_api/models/filter_option_group.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from odm_api.models.find_objects_response_filter_option_groups_inner_options_inner import FindObjectsResponseFilterOptionGroupsInnerOptionsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class FindObjectsResponseFilterOptionGroupsInner(BaseModel):
+class FilterOptionGroup(BaseModel):
     """
-    FindObjectsResponseFilterOptionGroupsInner
+    FilterOptionGroup
     """ # noqa: E501
     filter_id: Optional[StrictStr] = Field(default=None, alias="filterId")
     has_more_options: Optional[StrictBool] = Field(default=None, alias="hasMoreOptions")
     options: Optional[List[FindObjectsResponseFilterOptionGroupsInnerOptionsInner]] = None
     __properties: ClassVar[List[str]] = ["filterId", "hasMoreOptions", "options"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of FindObjectsResponseFilterOptionGroupsInner from a JSON string"""
+        """Create an instance of FilterOptionGroup from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,15 +78,15 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['options'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of FindObjectsResponseFilterOptionGroupsInner from a dict"""
+        """Create an instance of FilterOptionGroup from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `odm-api-0.0.1/odm_api/models/find_objects_response_objects_page.py` & `odm_api-1.57.0/odm_api/models/find_objects_response_objects_page.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
 from odm_api.models.find_objects_response_objects_page_content_inner import FindObjectsResponseObjectsPageContentInner
 from odm_api.models.search_study_request_page import SearchStudyRequestPage
 from typing import Optional, Set
 from typing_extensions import Self
 
 class FindObjectsResponseObjectsPage(BaseModel):
@@ -29,19 +29,19 @@
     FindObjectsResponseObjectsPage
     """ # noqa: E501
     filtered_count: Optional[StrictInt] = Field(default=None, alias="filteredCount")
     page_request: Optional[SearchStudyRequestPage] = Field(default=None, alias="pageRequest")
     content: Optional[List[FindObjectsResponseObjectsPageContentInner]] = None
     __properties: ClassVar[List[str]] = ["filteredCount", "pageRequest", "content"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `odm-api-0.0.1/odm_api/models/find_objects_response_objects_page_content_inner.py` & `odm_api-1.57.0/odm_api/models/source_type_pair.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,111 +1,93 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.find_objects_response_objects_page_content_inner_summary_inner import FindObjectsResponseObjectsPageContentInnerSummaryInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class FindObjectsResponseObjectsPageContentInner(BaseModel):
+class SourceTypePair(BaseModel):
     """
-    FindObjectsResponseObjectsPageContentInner
+    SourceTypePair
     """ # noqa: E501
-    accession: Optional[StrictStr] = None
-    name: Optional[StrictStr] = None
-    owner: Optional[StrictStr] = None
-    file_creation: Optional[StrictStr] = Field(default=None, alias="fileCreation")
-    size: Optional[StrictInt] = None
-    has_facs: Optional[StrictBool] = Field(default=None, alias="hasFacs")
-    has_genomic: Optional[StrictBool] = Field(default=None, alias="hasGenomic")
-    has_transcriptomics: Optional[StrictBool] = Field(default=None, alias="hasTranscriptomics")
-    summary: Optional[List[FindObjectsResponseObjectsPageContentInnerSummaryInner]] = None
-    __properties: ClassVar[List[str]] = ["accession", "name", "owner", "fileCreation", "size", "hasFacs", "hasGenomic", "hasTranscriptomics", "summary"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    first_type: Optional[StrictStr] = Field(default=None, description="Type of the object (e.g. study)", alias="firstType")
+    second_type: Optional[StrictStr] = Field(default=None, description="Type of the object (e.g. study)", alias="secondType")
+    __properties: ClassVar[List[str]] = ["firstType", "secondType"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of FindObjectsResponseObjectsPageContentInner from a JSON string"""
+        """Create an instance of SourceTypePair from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "first_type",
+            "second_type",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in summary (list)
-        _items = []
-        if self.summary:
-            for _item in self.summary:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['summary'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of FindObjectsResponseObjectsPageContentInner from a dict"""
+        """Create an instance of SourceTypePair from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "accession": obj.get("accession"),
-            "name": obj.get("name"),
-            "owner": obj.get("owner"),
-            "fileCreation": obj.get("fileCreation"),
-            "size": obj.get("size"),
-            "hasFacs": obj.get("hasFacs"),
-            "hasGenomic": obj.get("hasGenomic"),
-            "hasTranscriptomics": obj.get("hasTranscriptomics"),
-            "summary": [FindObjectsResponseObjectsPageContentInnerSummaryInner.from_dict(_item) for _item in obj["summary"]] if obj.get("summary") is not None else None
+            "firstType": obj.get("firstType"),
+            "secondType": obj.get("secondType")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/find_objects_response_objects_page_content_inner_summary_inner.py` & `odm_api-1.57.0/odm_api/models/error_message.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class FindObjectsResponseObjectsPageContentInnerSummaryInner(BaseModel):
+class ErrorMessage(BaseModel):
     """
-    FindObjectsResponseObjectsPageContentInnerSummaryInner
+    ErrorMessage
     """ # noqa: E501
-    key: Optional[StrictStr] = None
-    values: Optional[List[StrictStr]] = None
-    __properties: ClassVar[List[str]] = ["key", "values"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    message: StrictStr = Field(description="Detailed error message")
+    __properties: ClassVar[List[str]] = ["message"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of FindObjectsResponseObjectsPageContentInnerSummaryInner from a JSON string"""
+        """Create an instance of ErrorMessage from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,21 +68,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of FindObjectsResponseObjectsPageContentInnerSummaryInner from a dict"""
+        """Create an instance of ErrorMessage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "key": obj.get("key"),
-            "values": obj.get("values")
+            "message": obj.get("message")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/flow_cytometry_item.py` & `odm_api-1.57.0/odm_api/models/page_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class FlowCytometryItem(BaseModel):
+class PageRequest(BaseModel):
     """
-    FlowCytometryItem
+    PageRequest
     """ # noqa: E501
-    item_id: Optional[StrictStr] = Field(default=None, alias="itemId")
-    metadata: Optional[Dict[str, Any]] = None
-    run_id: Optional[StrictStr] = Field(default=None, alias="runId")
-    group_id: Optional[StrictStr] = Field(default=None, alias="groupId")
-    readout_type: Optional[StrictStr] = Field(default=None, alias="readoutType")
-    cell_population: Optional[StrictStr] = Field(default=None, alias="cellPopulation")
-    marker: Optional[StrictStr] = None
-    expression: Optional[Union[StrictFloat, StrictInt]] = None
-    __properties: ClassVar[List[str]] = ["itemId", "metadata", "runId", "groupId", "readoutType", "cellPopulation", "marker", "expression"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    offset: Optional[StrictInt] = Field(default=None, description="Param says to skip that many links before beginning to return links. Default: 0.")
+    limit: Optional[StrictInt] = Field(default=None, description="Param says to limit the count of returned links. Default: 1000.")
+    __properties: ClassVar[List[str]] = ["offset", "limit"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of FlowCytometryItem from a JSON string"""
+        """Create an instance of PageRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -75,27 +69,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of FlowCytometryItem from a dict"""
+        """Create an instance of PageRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "itemId": obj.get("itemId"),
-            "metadata": obj.get("metadata"),
-            "runId": obj.get("runId"),
-            "groupId": obj.get("groupId"),
-            "readoutType": obj.get("readoutType"),
-            "cellPopulation": obj.get("cellPopulation"),
-            "marker": obj.get("marker"),
-            "expression": obj.get("expression")
+            "offset": obj.get("offset"),
+            "limit": obj.get("limit")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/flow_cytometry_response.py` & `odm_api-1.57.0/odm_api/models/flow_cytometry_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from odm_api.models.get_flow_cytometry_as_curator200_response import GetFlowCytometryAsCurator200Response
 from typing import Optional, Set
 from typing_extensions import Self
 
 class FlowCytometryResponse(BaseModel):
     """
     FlowCytometryResponse
     """ # noqa: E501
     data: Optional[List[GetFlowCytometryAsCurator200Response]] = None
     cursor: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["data", "cursor"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `odm-api-0.0.1/odm_api/models/flow_cytometry_signal_source.py` & `odm_api-1.57.0/odm_api/models/omics_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,93 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class FlowCytometrySignalSource(BaseModel):
+class OmicsResponse(BaseModel):
     """
-    FlowCytometrySignalSource
+    OmicsResponse
     """ # noqa: E501
-    template_id: Optional[StrictStr] = Field(default=None, description="ID of template file.", alias="templateId")
-    link: StrictStr = Field(description="URL of the signal file.")
-    metadata_link: Optional[StrictStr] = Field(default=None, description="URL of the signal file metadata.", alias="metadataLink")
-    previous_version: Optional[StrictStr] = Field(default=None, description="Accession of matrix group or matrix group version chain.", alias="previousVersion")
-    __properties: ClassVar[List[str]] = ["templateId", "link", "metadataLink", "previousVersion"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    data: Optional[List[Dict[str, Any]]] = None
+    results_exhausted: Optional[StrictBool] = Field(default=None, alias="resultsExhausted")
+    log: Optional[List[StrictStr]] = None
+    cursor: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["data", "resultsExhausted", "log", "cursor"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of FlowCytometrySignalSource from a JSON string"""
+        """Create an instance of OmicsResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "template_id",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of FlowCytometrySignalSource from a dict"""
+        """Create an instance of OmicsResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "templateId": obj.get("templateId"),
-            "link": obj.get("link"),
-            "metadataLink": obj.get("metadataLink"),
-            "previousVersion": obj.get("previousVersion")
+            "data": obj.get("data"),
+            "resultsExhausted": obj.get("resultsExhausted"),
+            "log": obj.get("log"),
+            "cursor": obj.get("cursor")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/get_expression_as_user200_response.py` & `odm_api-1.57.0/odm_api/models/applied_filter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,113 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
-from odm_api.models.get_expression_as_user200_response_feature import GetExpressionAsUser200ResponseFeature
-from odm_api.models.get_expression_as_user200_response_value import GetExpressionAsUser200ResponseValue
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GetExpressionAsUser200Response(BaseModel):
+class AppliedFilter(BaseModel):
     """
-    GetExpressionAsUser200Response
+    AppliedFilter
     """ # noqa: E501
-    item_id: Optional[StrictStr] = Field(default=None, alias="itemId")
-    metadata: Optional[Dict[str, Any]] = None
-    run_id: Optional[StrictStr] = Field(default=None, alias="runId")
-    group_id: Optional[StrictStr] = Field(default=None, alias="groupId")
-    gene: Optional[StrictStr] = None
-    expression: Optional[Union[StrictFloat, StrictInt]] = None
-    feature: Optional[GetExpressionAsUser200ResponseFeature] = None
-    value: Optional[GetExpressionAsUser200ResponseValue] = None
-    description: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["itemId", "metadata", "runId", "groupId", "gene", "expression", "feature", "value", "description"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    type: Optional[StrictStr] = None
+    filter_option_id: Optional[StrictStr] = Field(default=None, alias="filterOptionId")
+    match: Optional[StrictStr] = None
+    mode: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["type", "filterOptionId", "match", "mode"]
+
+    @field_validator('type')
+    def type_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in set(['FULL_TEXT', 'SELECT']):
+            raise ValueError("must be one of enum values ('FULL_TEXT', 'SELECT')")
+        return value
+
+    @field_validator('mode')
+    def mode_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in set(['STRICT', 'USE_NARROWER_TERMS']):
+            raise ValueError("must be one of enum values ('STRICT', 'USE_NARROWER_TERMS')")
+        return value
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GetExpressionAsUser200Response from a JSON string"""
+        """Create an instance of AppliedFilter from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "description",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of feature
-        if self.feature:
-            _dict['feature'] = self.feature.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of value
-        if self.value:
-            _dict['value'] = self.value.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GetExpressionAsUser200Response from a dict"""
+        """Create an instance of AppliedFilter from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "itemId": obj.get("itemId"),
-            "metadata": obj.get("metadata"),
-            "runId": obj.get("runId"),
-            "groupId": obj.get("groupId"),
-            "gene": obj.get("gene"),
-            "expression": obj.get("expression"),
-            "feature": GetExpressionAsUser200ResponseFeature.from_dict(obj["feature"]) if obj.get("feature") is not None else None,
-            "value": GetExpressionAsUser200ResponseValue.from_dict(obj["value"]) if obj.get("value") is not None else None,
-            "description": obj.get("description")
+            "type": obj.get("type"),
+            "filterOptionId": obj.get("filterOptionId"),
+            "match": obj.get("match"),
+            "mode": obj.get("mode")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/get_expression_as_user200_response_feature.py` & `odm_api-1.57.0/odm_api/models/json_metadata_attributes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
-from pydantic import BaseModel, Field, StrictStr, ValidationError, field_validator
-from typing import Any, Dict, Optional
-from typing import Union, Any, List, TYPE_CHECKING, Optional, Dict
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, ValidationError, field_validator
+from typing import Optional
+from typing import Union, Any, List, Set, TYPE_CHECKING, Optional, Dict
 from typing_extensions import Literal, Self
 from pydantic import Field
 
-GETEXPRESSIONASUSER200RESPONSEFEATURE_ANY_OF_SCHEMAS = ["object", "str"]
+JSONMETADATAATTRIBUTES_ANY_OF_SCHEMAS = ["str"]
 
-class GetExpressionAsUser200ResponseFeature(BaseModel):
+class JsonMetadataAttributes(BaseModel):
     """
-    GetExpressionAsUser200ResponseFeature
+    JsonMetadataAttributes
     """
 
-    # data type: object
-    anyof_schema_1_validator: Optional[Dict[str, Any]] = None
     # data type: str
-    anyof_schema_2_validator: Optional[StrictStr] = None
+    anyof_schema_1_validator: Optional[StrictStr] = None
     if TYPE_CHECKING:
-        actual_instance: Optional[Union[object, str]] = None
+        actual_instance: Optional[Union[str]] = None
     else:
         actual_instance: Any = None
-    any_of_schemas: List[str] = Field(default=Literal["object", "str"])
+    any_of_schemas: Set[str] = { "str" }
 
     model_config = {
         "validate_assignment": True,
         "protected_namespaces": (),
     }
 
     def __init__(self, *args, **kwargs) -> None:
@@ -53,79 +51,64 @@
                 raise ValueError("If a position argument is used, keyword arguments cannot be used.")
             super().__init__(actual_instance=args[0])
         else:
             super().__init__(**kwargs)
 
     @field_validator('actual_instance')
     def actual_instance_must_validate_anyof(cls, v):
-        instance = GetExpressionAsUser200ResponseFeature.model_construct()
+        instance = JsonMetadataAttributes.model_construct()
         error_messages = []
-        # validate data type: object
-        try:
-            instance.anyof_schema_1_validator = v
-            return v
-        except (ValidationError, ValueError) as e:
-            error_messages.append(str(e))
         # validate data type: str
         try:
-            instance.anyof_schema_2_validator = v
+            instance.anyof_schema_1_validator = v
             return v
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
         if error_messages:
             # no match
-            raise ValueError("No match found when setting the actual_instance in GetExpressionAsUser200ResponseFeature with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when setting the actual_instance in JsonMetadataAttributes with anyOf schemas: str. Details: " + ", ".join(error_messages))
         else:
             return v
 
     @classmethod
     def from_dict(cls, obj: Dict[str, Any]) -> Self:
         return cls.from_json(json.dumps(obj))
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
         """Returns the object represented by the json string"""
         instance = cls.model_construct()
         error_messages = []
-        # deserialize data into object
+        # deserialize data into str
         try:
             # validation
             instance.anyof_schema_1_validator = json.loads(json_str)
             # assign value to actual_instance
             instance.actual_instance = instance.anyof_schema_1_validator
             return instance
         except (ValidationError, ValueError) as e:
             error_messages.append(str(e))
-        # deserialize data into str
-        try:
-            # validation
-            instance.anyof_schema_2_validator = json.loads(json_str)
-            # assign value to actual_instance
-            instance.actual_instance = instance.anyof_schema_2_validator
-            return instance
-        except (ValidationError, ValueError) as e:
-            error_messages.append(str(e))
 
         if error_messages:
             # no match
-            raise ValueError("No match found when deserializing the JSON string into GetExpressionAsUser200ResponseFeature with anyOf schemas: object, str. Details: " + ", ".join(error_messages))
+            raise ValueError("No match found when deserializing the JSON string into JsonMetadataAttributes with anyOf schemas: str. Details: " + ", ".join(error_messages))
         else:
             return instance
 
     def to_json(self) -> str:
         """Returns the JSON representation of the actual instance"""
         if self.actual_instance is None:
             return "null"
 
         if hasattr(self.actual_instance, "to_json") and callable(self.actual_instance.to_json):
             return self.actual_instance.to_json()
         else:
             return json.dumps(self.actual_instance)
 
-    def to_dict(self) -> Optional[Union[Dict[str, Any], object, str]]:
+    def to_dict(self) -> Optional[Union[Dict[str, Any], str]]:
         """Returns the dict representation of the actual instance"""
         if self.actual_instance is None:
             return None
 
         if hasattr(self.actual_instance, "to_dict") and callable(self.actual_instance.to_dict):
             return self.actual_instance.to_dict()
         else:
```

### Comparing `odm-api-0.0.1/odm_api/models/get_flow_cytometry_as_curator200_response.py` & `odm_api-1.57.0/odm_api/models/xref_set_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,61 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GetFlowCytometryAsCurator200Response(BaseModel):
+class XrefSetMetadata(BaseModel):
     """
-    GetFlowCytometryAsCurator200Response
+    Xrefset metadata
     """ # noqa: E501
-    item_id: Optional[StrictStr] = Field(default=None, alias="itemId")
-    metadata: Optional[Dict[str, Any]] = None
-    run_id: Optional[StrictStr] = Field(default=None, alias="runId")
-    group_id: Optional[StrictStr] = Field(default=None, alias="groupId")
-    readout_type: Optional[StrictStr] = Field(default=None, alias="readoutType")
-    cell_population: Optional[StrictStr] = Field(default=None, alias="cellPopulation")
-    marker: Optional[StrictStr] = None
-    expression: Optional[Union[StrictFloat, StrictInt]] = None
-    __properties: ClassVar[List[str]] = ["itemId", "metadata", "runId", "groupId", "readoutType", "cellPopulation", "marker", "expression"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    xref_set_id: Optional[StrictStr] = Field(default=None, alias="xrefSetId")
+    created_by: Optional[StrictStr] = Field(default=None, alias="createdBy")
+    created_date: Optional[StrictInt] = Field(default=None, alias="createdDate")
+    last_updated: Optional[StrictInt] = Field(default=None, alias="lastUpdated")
+    data: Optional[Dict[str, Any]] = None
+    __properties: ClassVar[List[str]] = ["xrefSetId", "createdBy", "createdDate", "lastUpdated", "data"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GetFlowCytometryAsCurator200Response from a JSON string"""
+        """Create an instance of XrefSetMetadata from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -75,27 +72,24 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GetFlowCytometryAsCurator200Response from a dict"""
+        """Create an instance of XrefSetMetadata from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "itemId": obj.get("itemId"),
-            "metadata": obj.get("metadata"),
-            "runId": obj.get("runId"),
-            "groupId": obj.get("groupId"),
-            "readoutType": obj.get("readoutType"),
-            "cellPopulation": obj.get("cellPopulation"),
-            "marker": obj.get("marker"),
-            "expression": obj.get("expression")
+            "xrefSetId": obj.get("xrefSetId"),
+            "createdBy": obj.get("createdBy"),
+            "createdDate": obj.get("createdDate"),
+            "lastUpdated": obj.get("lastUpdated"),
+            "data": obj.get("data")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/get_variant_as_curator200_response.py` & `odm_api-1.57.0/odm_api/models/variant_item.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GetVariantAsCurator200Response(BaseModel):
+class VariantItem(BaseModel):
     """
-    GetVariantAsCurator200Response
+    VariantItem
     """ # noqa: E501
     item_id: Optional[StrictStr] = Field(default=None, alias="itemId")
     metadata: Optional[Dict[str, Any]] = None
     run_id: Optional[StrictStr] = Field(default=None, alias="runId")
     group_id: Optional[StrictStr] = Field(default=None, alias="groupId")
     contig: Optional[StrictStr] = None
     start: Optional[StrictInt] = None
     reference: Optional[StrictStr] = None
     alteration: Optional[List[StrictStr]] = None
     variation_id: Optional[List[StrictStr]] = Field(default=None, alias="variationId")
     info: Optional[Dict[str, Any]] = None
     genotype: Optional[Dict[str, Any]] = None
     __properties: ClassVar[List[str]] = ["itemId", "metadata", "runId", "groupId", "contig", "start", "reference", "alteration", "variationId", "info", "genotype"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GetVariantAsCurator200Response from a JSON string"""
+        """Create an instance of VariantItem from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -78,15 +78,15 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GetVariantAsCurator200Response from a dict"""
+        """Create an instance of VariantItem from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `odm-api-0.0.1/odm_api/models/group.py` & `odm_api-1.57.0/odm_api/models/meta.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,73 +1,70 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from datetime import datetime
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.create_group_request_members_inner import CreateGroupRequestMembersInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Group(BaseModel):
+class Meta(BaseModel):
     """
-    Group
+    resource metadata
     """ # noqa: E501
-    external_id: Optional[StrictStr] = Field(default=None, description="External unique resource id", alias="externalId")
-    id: Optional[StrictStr] = Field(default=None, description="Unique resource id")
-    schemas: Optional[List[StrictStr]] = None
-    members: Optional[List[CreateGroupRequestMembersInner]] = None
-    display_name: StrictStr = Field(alias="displayName")
-    __properties: ClassVar[List[str]] = ["externalId", "id", "schemas", "members", "displayName"]
+    created: Optional[datetime] = None
+    last_modified: Optional[datetime] = Field(default=None, alias="lastModified")
+    resource_type: Optional[StrictStr] = Field(default=None, alias="resourceType")
+    __properties: ClassVar[List[str]] = ["created", "lastModified", "resourceType"]
 
-    @field_validator('schemas')
-    def schemas_validate_enum(cls, value):
+    @field_validator('resource_type')
+    def resource_type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        for i in value:
-            if i not in set(['urn:ietf:params:scim:schemas:core:2.0:Group']):
-                raise ValueError("each list item must be one of ('urn:ietf:params:scim:schemas:core:2.0:Group')")
+        if value not in set(['User', 'Group']):
+            raise ValueError("must be one of enum values ('User', 'Group')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Group from a JSON string"""
+        """Create an instance of Meta from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -80,35 +77,26 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in members (list)
-        _items = []
-        if self.members:
-            for _item in self.members:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['members'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Group from a dict"""
+        """Create an instance of Meta from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "externalId": obj.get("externalId"),
-            "id": obj.get("id"),
-            "schemas": obj.get("schemas"),
-            "members": [CreateGroupRequestMembersInner.from_dict(_item) for _item in obj["members"]] if obj.get("members") is not None else None,
-            "displayName": obj.get("displayName")
+            "created": obj.get("created"),
+            "lastModified": obj.get("lastModified"),
+            "resourceType": obj.get("resourceType")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/group_patch.py` & `odm_api-1.57.0/odm_api/models/study_validation_summary.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,58 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
-from typing import Any, ClassVar, Dict, List
-from odm_api.models.user_patch_operations_inner import UserPatchOperationsInner
+from pydantic import BaseModel, ConfigDict
+from typing import Any, ClassVar, Dict, List, Optional
+from odm_api.models.study_validation_summary_samples_inner import StudyValidationSummarySamplesInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GroupPatch(BaseModel):
+class StudyValidationSummary(BaseModel):
     """
-    GroupPatch
+    StudyValidationSummary
     """ # noqa: E501
-    operations: List[UserPatchOperationsInner] = Field(description="Patch operations list", alias="Operations")
-    schemas: List[StrictStr]
-    __properties: ClassVar[List[str]] = ["Operations", "schemas"]
-
-    @field_validator('schemas')
-    def schemas_validate_enum(cls, value):
-        """Validates the enum"""
-        for i in value:
-            if i not in set(['urn:ietf:params:scim:api:messages:2.0:PatchOp']):
-                raise ValueError("each list item must be one of ('urn:ietf:params:scim:api:messages:2.0:PatchOp')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    samples: Optional[List[StudyValidationSummarySamplesInner]] = None
+    __properties: ClassVar[List[str]] = ["samples"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GroupPatch from a JSON string"""
+        """Create an instance of StudyValidationSummary from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,32 +65,31 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in operations (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in samples (list)
         _items = []
-        if self.operations:
-            for _item in self.operations:
+        if self.samples:
+            for _item in self.samples:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['Operations'] = _items
+            _dict['samples'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GroupPatch from a dict"""
+        """Create an instance of StudyValidationSummary from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "Operations": [UserPatchOperationsInner.from_dict(_item) for _item in obj["Operations"]] if obj.get("Operations") is not None else None,
-            "schemas": obj.get("schemas")
+            "samples": [StudyValidationSummarySamplesInner.from_dict(_item) for _item in obj["samples"]] if obj.get("samples") is not None else None
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/group_response.py` & `odm_api-1.57.0/odm_api/models/i_metadata.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,65 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.create_group_request_members_inner import CreateGroupRequestMembersInner
-from odm_api.models.create_user201_response_all_of_meta import CreateUser201ResponseAllOfMeta
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GroupResponse(BaseModel):
+class IMetadata(BaseModel):
     """
-    GroupResponse
+    IMetadata
     """ # noqa: E501
-    external_id: Optional[StrictStr] = Field(default=None, description="External unique resource id", alias="externalId")
-    id: Optional[StrictStr] = Field(default=None, description="Unique resource id")
-    schemas: Optional[List[StrictStr]] = None
-    members: Optional[List[CreateGroupRequestMembersInner]] = None
-    display_name: StrictStr = Field(alias="displayName")
-    meta: Optional[CreateUser201ResponseAllOfMeta] = None
-    __properties: ClassVar[List[str]] = ["externalId", "id", "schemas", "members", "displayName", "meta"]
-
-    @field_validator('schemas')
-    def schemas_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        for i in value:
-            if i not in set(['urn:ietf:params:scim:schemas:core:2.0:Group']):
-                raise ValueError("each list item must be one of ('urn:ietf:params:scim:schemas:core:2.0:Group')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    source: Optional[StrictStr] = None
+    name: Optional[StrictStr] = None
+    public: Optional[StrictBool] = None
+    id: Optional[StrictStr] = None
+    content: Optional[Dict[str, Any]] = None
+    data_type: Optional[StrictStr] = Field(default=None, alias="dataType")
+    content_map: Optional[Dict[str, Any]] = Field(default=None, alias="contentMap")
+    metadata_content: Optional[Dict[str, Any]] = Field(default=None, alias="metadataContent")
+    file_id_associated_with_template: Optional[StrictStr] = Field(default=None, alias="fileIdAssociatedWithTemplate")
+    __properties: ClassVar[List[str]] = ["source", "name", "public", "id", "content", "dataType", "contentMap", "metadataContent", "fileIdAssociatedWithTemplate"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GroupResponse from a JSON string"""
+        """Create an instance of IMetadata from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,39 +72,32 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in members (list)
-        _items = []
-        if self.members:
-            for _item in self.members:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['members'] = _items
-        # override the default output from pydantic by calling `to_dict()` of meta
-        if self.meta:
-            _dict['meta'] = self.meta.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GroupResponse from a dict"""
+        """Create an instance of IMetadata from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "externalId": obj.get("externalId"),
+            "source": obj.get("source"),
+            "name": obj.get("name"),
+            "public": obj.get("public"),
             "id": obj.get("id"),
-            "schemas": obj.get("schemas"),
-            "members": [CreateGroupRequestMembersInner.from_dict(_item) for _item in obj["members"]] if obj.get("members") is not None else None,
-            "displayName": obj.get("displayName"),
-            "meta": CreateUser201ResponseAllOfMeta.from_dict(obj["meta"]) if obj.get("meta") is not None else None
+            "content": obj.get("content"),
+            "dataType": obj.get("dataType"),
+            "contentMap": obj.get("contentMap"),
+            "metadataContent": obj.get("metadataContent"),
+            "fileIdAssociatedWithTemplate": obj.get("fileIdAssociatedWithTemplate")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/group_validation_summary.py` & `odm_api-1.57.0/odm_api/models/relationships.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,101 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.group_validation_summary_attributes_inner import GroupValidationSummaryAttributesInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class GroupValidationSummary(BaseModel):
+class Relationships(BaseModel):
     """
-    GroupValidationSummary
+    Relationships
     """ # noqa: E501
-    group_accession: Optional[StrictStr] = Field(default=None, alias="groupAccession")
-    attributes: Optional[List[GroupValidationSummaryAttributesInner]] = None
-    __properties: ClassVar[List[str]] = ["groupAccession", "attributes"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    sample: Optional[StrictStr] = None
+    cell: Optional[StrictStr] = None
+    library: Optional[StrictStr] = None
+    preparation: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["sample", "cell", "library", "preparation"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of GroupValidationSummary from a JSON string"""
+        """Create an instance of Relationships from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "sample",
+            "cell",
+            "library",
+            "preparation",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in attributes (list)
-        _items = []
-        if self.attributes:
-            for _item in self.attributes:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['attributes'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of GroupValidationSummary from a dict"""
+        """Create an instance of Relationships from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "groupAccession": obj.get("groupAccession"),
-            "attributes": [GroupValidationSummaryAttributesInner.from_dict(_item) for _item in obj["attributes"]] if obj.get("attributes") is not None else None
+            "sample": obj.get("sample"),
+            "cell": obj.get("cell"),
+            "library": obj.get("library"),
+            "preparation": obj.get("preparation")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/i_metadata.py` & `odm_api-1.57.0/odm_api/models/runs_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,60 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class IMetadata(BaseModel):
+class RunsResponse(BaseModel):
     """
-    IMetadata
+    RunsResponse
     """ # noqa: E501
-    source: Optional[StrictStr] = None
-    name: Optional[StrictStr] = None
-    public: Optional[StrictBool] = None
-    id: Optional[StrictStr] = None
-    content: Optional[Dict[str, Any]] = None
-    data_type: Optional[StrictStr] = Field(default=None, alias="dataType")
-    content_map: Optional[Dict[str, Dict[str, Any]]] = Field(default=None, alias="contentMap")
-    metadata_content: Optional[Dict[str, Dict[str, Any]]] = Field(default=None, alias="metadataContent")
-    file_id_associated_with_template: Optional[StrictStr] = Field(default=None, alias="fileIdAssociatedWithTemplate")
-    __properties: ClassVar[List[str]] = ["source", "name", "public", "id", "content", "dataType", "contentMap", "metadataContent", "fileIdAssociatedWithTemplate"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    runs: Optional[List[Dict[str, Any]]] = None
+    experiment: Optional[StrictStr] = None
+    warnings: Optional[List[StrictStr]] = None
+    version_chain_id: Optional[StrictStr] = Field(default=None, alias="versionChainId")
+    __properties: ClassVar[List[str]] = ["runs", "experiment", "warnings", "versionChainId"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of IMetadata from a JSON string"""
+        """Create an instance of RunsResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -76,26 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of IMetadata from a dict"""
+        """Create an instance of RunsResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "source": obj.get("source"),
-            "name": obj.get("name"),
-            "public": obj.get("public"),
-            "id": obj.get("id"),
-            "content": obj.get("content"),
-            "dataType": obj.get("dataType"),
-            "fileIdAssociatedWithTemplate": obj.get("fileIdAssociatedWithTemplate")
+            "runs": obj.get("runs"),
+            "experiment": obj.get("experiment"),
+            "warnings": obj.get("warnings"),
+            "versionChainId": obj.get("versionChainId")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/import_expression_signal_run_request.py` & `odm_api-1.57.0/odm_api/models/xref_set_create_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,74 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ImportExpressionSignalRunRequest(BaseModel):
+class XrefSetCreateRequest(BaseModel):
     """
-    ImportExpressionSignalRunRequest
+    Create XrefSet request body
     """ # noqa: E501
-    number_of_feature_attributes: Optional[Any] = Field(default=None, description="Integer value that specifies the number of columns related to the feature in the uploaded data frame, and indicates the starting position of the sample data. This attribute is not needed if the uploaded file is in GCT format.", alias="numberOfFeatureAttributes")
-    data_class: Optional[Any] = Field(default=None, description="A mandatory parameter with the following possible values: `Bulk transcriptomics`, `Single-cell transcriptomics`, `Differential abundance (FC, pval, etc.)`, `Pathway analysis`, `Proteomics`, `Single-cell proteomics`, `Metabolomics`, `Epigenomics`, `DNA methylation`, `Chemoinformatics`, `Imaging features`, `Gene panel data`, `Biomarker data`, `Physical measures`, `Blood counts`, `Other body fluid counts`, `Nanopore`, `Other`.  In case the parameter is not set the dataClass is automatically defined as `Other`.", alias="dataClass")
-    measurement_separator: Optional[Any] = Field(default=None, description="This parameter is necessary when your file contains multiple measurement columns for each sample, library, or preparation. It represents the character that distinguishes the sample/library/preparation name from the measurement name in column headers. Supported separators include `. , : ; _ - / \\ |`, with the allowance for multi-character separators.", alias="measurementSeparator")
-    source: Optional[StrictStr] = None
-    metadata_link: Optional[StrictStr] = Field(default=None, alias="metadataLink")
-    data_link: StrictStr = Field(alias="dataLink")
-    template_id: Optional[StrictStr] = Field(default=None, alias="templateId")
-    previous_version: Optional[StrictStr] = Field(default=None, alias="previousVersion")
-    __properties: ClassVar[List[str]] = ["source", "metadataLink", "dataLink", "templateId", "previousVersion"]
+    xref_set_type: StrictStr = Field(description="Type of data stored in XrefSet", alias="xrefSetType")
+    data_link: StrictStr = Field(description="Mapping file link", alias="dataLink")
+    data_source: StrictStr = Field(description="Target storage dataLink points to", alias="dataSource")
+    metadata: Optional[Dict[str, Any]] = Field(default=None, description="Additional user metadata")
+    __properties: ClassVar[List[str]] = ["xrefSetType", "dataLink", "dataSource", "metadata"]
 
-    @field_validator('source')
-    def source_validate_enum(cls, value):
+    @field_validator('xref_set_type')
+    def xref_set_type_validate_enum(cls, value):
         """Validates the enum"""
-        if value is None:
-            return value
+        if value not in set(['gene-transcript']):
+            raise ValueError("must be one of enum values ('gene-transcript')")
+        return value
 
-        if value not in set(['ARVADOS', 'S3', 'HTTP']):
-            raise ValueError("must be one of enum values ('ARVADOS', 'S3', 'HTTP')")
+    @field_validator('data_source')
+    def data_source_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['arvados', 's3', 'http']):
+            raise ValueError("must be one of enum values ('arvados', 's3', 'http')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ImportExpressionSignalRunRequest from a JSON string"""
+        """Create an instance of XrefSetCreateRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -85,24 +85,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ImportExpressionSignalRunRequest from a dict"""
+        """Create an instance of XrefSetCreateRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "source": obj.get("source"),
-            "metadataLink": obj.get("metadataLink"),
+            "xrefSetType": obj.get("xrefSetType"),
             "dataLink": obj.get("dataLink"),
-            "templateId": obj.get("templateId"),
-            "previousVersion": obj.get("previousVersion")
+            "dataSource": obj.get("dataSource"),
+            "metadata": obj.get("metadata")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/import_metadata_request.py` & `odm_api-1.57.0/odm_api/models/import_metadata_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
 class ImportMetadataRequest(BaseModel):
     """
     ImportMetadataRequest
@@ -37,19 +37,19 @@
         if value is None:
             return value
 
         if value not in set(['ARVADOS', 'S3', 'HTTP']):
             raise ValueError("must be one of enum values ('ARVADOS', 'S3', 'HTTP')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `odm-api-0.0.1/odm_api/models/import_signal_run_request.py` & `odm_api-1.57.0/odm_api/models/xref_set_search_result_result_inner.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ImportSignalRunRequest(BaseModel):
+class XrefSetSearchResultResultInner(BaseModel):
     """
-    import signal data request
+    XrefSetSearchResultResultInner
     """ # noqa: E501
-    source: Optional[StrictStr] = None
-    metadata_link: Optional[StrictStr] = Field(default=None, alias="metadataLink")
-    data_link: StrictStr = Field(alias="dataLink")
-    template_id: Optional[StrictStr] = Field(default=None, alias="templateId")
-    previous_version: Optional[StrictStr] = Field(default=None, alias="previousVersion")
-    __properties: ClassVar[List[str]] = ["source", "metadataLink", "dataLink", "templateId", "previousVersion"]
-
-    @field_validator('source')
-    def source_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['ARVADOS', 'S3', 'HTTP']):
-            raise ValueError("must be one of enum values ('ARVADOS', 'S3', 'HTTP')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    xref_set_id: Optional[StrictStr] = Field(default=None, alias="xrefSetId")
+    source_id: Optional[StrictStr] = Field(default=None, alias="sourceId")
+    target_ids: Optional[List[StrictStr]] = Field(default=None, alias="targetIds")
+    __properties: ClassVar[List[str]] = ["xrefSetId", "sourceId", "targetIds"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ImportSignalRunRequest from a JSON string"""
+        """Create an instance of XrefSetSearchResultResultInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,24 +70,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ImportSignalRunRequest from a dict"""
+        """Create an instance of XrefSetSearchResultResultInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "source": obj.get("source"),
-            "metadataLink": obj.get("metadataLink"),
-            "dataLink": obj.get("dataLink"),
-            "templateId": obj.get("templateId"),
-            "previousVersion": obj.get("previousVersion")
+            "xrefSetId": obj.get("xrefSetId"),
+            "sourceId": obj.get("sourceId"),
+            "targetIds": obj.get("targetIds")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/info.py` & `odm_api-1.57.0/odm_api/models/managed_object.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,61 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from pydantic import BaseModel, Field, StrictInt, StrictStr, field_validator
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Info(BaseModel):
+class ManagedObject(BaseModel):
     """
-    job execution information
+    ManagedObject
     """ # noqa: E501
-    job_exec_id: StrictInt = Field(description="job execution id", alias="jobExecId")
-    started_by: StrictStr = Field(description="user name who started the job", alias="startedBy")
-    job_name: StrictStr = Field(description="actual job name", alias="jobName")
-    status: StrictStr = Field(description="current job status")
-    create_time: datetime = Field(alias="createTime")
-    end_time: Optional[datetime] = Field(default=None, alias="endTime")
-    __properties: ClassVar[List[str]] = ["jobExecId", "startedBy", "jobName", "status", "createTime", "endTime"]
-
-    @field_validator('status')
-    def status_validate_enum(cls, value):
-        """Validates the enum"""
-        if value not in set(['COMPLETED', 'STARTING', 'RUNNING', 'STOPPING', 'STOPPED', 'FAILED', 'ABANDONED', 'UNKNOWN']):
-            raise ValueError("must be one of enum values ('COMPLETED', 'STARTING', 'RUNNING', 'STOPPING', 'STOPPED', 'FAILED', 'ABANDONED', 'UNKNOWN')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    genestackaccession: StrictStr = Field(alias="genestack:accession")
+    object_type: StrictStr = Field(alias="objectType")
+    owner_email: StrictStr = Field(alias="ownerEmail")
+    created_at: datetime = Field(alias="createdAt")
+    __properties: ClassVar[List[str]] = ["genestack:accession", "objectType", "ownerEmail", "createdAt"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Info from a JSON string"""
+        """Create an instance of ManagedObject from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -81,25 +72,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Info from a dict"""
+        """Create an instance of ManagedObject from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "jobExecId": obj.get("jobExecId"),
-            "startedBy": obj.get("startedBy"),
-            "jobName": obj.get("jobName"),
-            "status": obj.get("status"),
-            "createTime": obj.get("createTime"),
-            "endTime": obj.get("endTime")
+            "genestack:accession": obj.get("genestack:accession"),
+            "objectType": obj.get("objectType"),
+            "ownerEmail": obj.get("ownerEmail"),
+            "createdAt": obj.get("createdAt")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/list_response_meta.py` & `odm_api-1.57.0/odm_api/models/list_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.list_response_meta_pagination import ListResponseMetaPagination
+from odm_api.models.list_response_meta import ListResponseMeta
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ListResponseMeta(BaseModel):
+class ListResponse(BaseModel):
     """
-    ListResponseMeta
+    ListResponse
     """ # noqa: E501
-    pagination: Optional[ListResponseMetaPagination] = None
-    __properties: ClassVar[List[str]] = ["pagination"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    meta: Optional[ListResponseMeta] = None
+    data: Optional[List[Dict[str, Any]]] = None
+    __properties: ClassVar[List[str]] = ["meta", "data"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ListResponseMeta from a JSON string"""
+        """Create an instance of ListResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,27 +66,28 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of pagination
-        if self.pagination:
-            _dict['pagination'] = self.pagination.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of meta
+        if self.meta:
+            _dict['meta'] = self.meta.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ListResponseMeta from a dict"""
+        """Create an instance of ListResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "pagination": ListResponseMetaPagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None
+            "meta": ListResponseMeta.from_dict(obj["meta"]) if obj.get("meta") is not None else None,
+            "data": obj.get("data")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/list_response_meta_pagination.py` & `odm_api-1.57.0/test/test_find_objects_response_objects_page.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,55 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-from __future__ import annotations
-import pprint
-import re  # noqa: F401
-import json
-
-from pydantic import BaseModel, StrictInt
-from typing import Any, ClassVar, Dict, List, Optional
-from typing import Optional, Set
-from typing_extensions import Self
-
-class ListResponseMetaPagination(BaseModel):
-    """
-    ListResponseMetaPagination
-    """ # noqa: E501
-    count: Optional[StrictInt] = None
-    total: Optional[StrictInt] = None
-    offset: Optional[StrictInt] = None
-    limit: Optional[StrictInt] = None
-    __properties: ClassVar[List[str]] = ["count", "total", "offset", "limit"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
-
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.model_dump(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ListResponseMetaPagination from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Return the dictionary representation of the model using alias.
-
-        This has the following differences from calling pydantic's
-        `self.model_dump(by_alias=True)`:
-
-        * `None` is only added to the output dict for nullable fields that
-          were set at model initialization. Other fields with value `None`
-          are ignored.
-        """
-        excluded_fields: Set[str] = set([
-        ])
+import unittest
 
-        _dict = self.model_dump(
-            by_alias=True,
-            exclude=excluded_fields,
-            exclude_none=True,
-        )
-        return _dict
+from odm_api.models.find_objects_response_objects_page import FindObjectsResponseObjectsPage
+
+class TestFindObjectsResponseObjectsPage(unittest.TestCase):
+    """FindObjectsResponseObjectsPage unit test stubs"""
+
+    def setUp(self):
+        pass
 
-    @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ListResponseMetaPagination from a dict"""
-        if obj is None:
-            return None
-
-        if not isinstance(obj, dict):
-            return cls.model_validate(obj)
-
-        _obj = cls.model_validate({
-            "count": obj.get("count"),
-            "total": obj.get("total"),
-            "offset": obj.get("offset"),
-            "limit": obj.get("limit")
-        })
-        return _obj
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional) -> FindObjectsResponseObjectsPage:
+        """Test FindObjectsResponseObjectsPage
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `FindObjectsResponseObjectsPage`
+        """
+        model = FindObjectsResponseObjectsPage()
+        if include_optional:
+            return FindObjectsResponseObjectsPage(
+                filtered_count = 56,
+                page_request = {offset=6, limit=50},
+                content = [
+                    {owner=owner, summary=[{values=[values, values], key=key}, {values=[values, values], key=key}], hasFacs=true, hasTranscriptomics=true, size=1, fileCreation=fileCreation, name=name, accession=accession, hasGenomic=true}
+                    ]
+            )
+        else:
+            return FindObjectsResponseObjectsPage(
+        )
+        """
 
+    def testFindObjectsResponseObjectsPage(self):
+        """Test FindObjectsResponseObjectsPage"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `odm-api-0.0.1/odm_api/models/managed_object.py` & `odm_api-1.57.0/odm_api/models/study_generic_source.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,91 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from pydantic import BaseModel, Field, StrictStr
-from typing import Any, ClassVar, Dict, List
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ManagedObject(BaseModel):
+class StudyGenericSource(BaseModel):
     """
-    ManagedObject
+    StudyGenericSource
     """ # noqa: E501
-    genestackaccession: StrictStr = Field(alias="genestack:accession")
-    object_type: StrictStr = Field(alias="objectType")
-    owner_email: StrictStr = Field(alias="ownerEmail")
-    created_at: datetime = Field(alias="createdAt")
-    __properties: ClassVar[List[str]] = ["genestack:accession", "objectType", "ownerEmail", "createdAt"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    link: StrictStr = Field(description="URL for a file with Study metadata.")
+    template_id: Optional[StrictStr] = Field(default=None, description="ID of template file.", alias="templateId")
+    __properties: ClassVar[List[str]] = ["link", "templateId"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ManagedObject from a JSON string"""
+        """Create an instance of StudyGenericSource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "template_id",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ManagedObject from a dict"""
+        """Create an instance of StudyGenericSource from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "genestack:accession": obj.get("genestack:accession"),
-            "objectType": obj.get("objectType"),
-            "ownerEmail": obj.get("ownerEmail"),
-            "createdAt": obj.get("createdAt")
+            "link": obj.get("link"),
+            "templateId": obj.get("templateId")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/meta.py` & `odm_api-1.57.0/odm_api/models/search_study_request_page.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,58 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Meta(BaseModel):
+class SearchStudyRequestPage(BaseModel):
     """
-    resource metadata
+    SearchStudyRequestPage
     """ # noqa: E501
-    created: Optional[datetime] = None
-    last_modified: Optional[datetime] = Field(default=None, alias="lastModified")
-    resource_type: Optional[StrictStr] = Field(default=None, alias="resourceType")
-    __properties: ClassVar[List[str]] = ["created", "lastModified", "resourceType"]
-
-    @field_validator('resource_type')
-    def resource_type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['User', 'Group']):
-            raise ValueError("must be one of enum values ('User', 'Group')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    offset: Optional[StrictInt] = Field(default=None, description="Param says to skip that many links before beginning to return links. Default: 0.")
+    limit: Optional[StrictInt] = Field(default=None, description="Param says to limit the count of returned links. Default: 1000.")
+    __properties: ClassVar[List[str]] = ["offset", "limit"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Meta from a JSON string"""
+        """Create an instance of SearchStudyRequestPage from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -81,22 +69,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Meta from a dict"""
+        """Create an instance of SearchStudyRequestPage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "created": obj.get("created"),
-            "lastModified": obj.get("lastModified"),
-            "resourceType": obj.get("resourceType")
+            "offset": obj.get("offset"),
+            "limit": obj.get("limit")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/meta_response.py` & `odm_api-1.57.0/odm_api/models/variant_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.list_response_meta_pagination import ListResponseMetaPagination
+from odm_api.models.get_variant_as_curator200_response import GetVariantAsCurator200Response
 from typing import Optional, Set
 from typing_extensions import Self
 
-class MetaResponse(BaseModel):
+class VariantResponse(BaseModel):
     """
-    MetaResponse
+    VariantResponse
     """ # noqa: E501
-    pagination: Optional[ListResponseMetaPagination] = None
-    __properties: ClassVar[List[str]] = ["pagination"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    data: Optional[List[GetVariantAsCurator200Response]] = None
+    cursor: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["data", "cursor"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of MetaResponse from a JSON string"""
+        """Create an instance of VariantResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,27 +66,32 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of pagination
-        if self.pagination:
-            _dict['pagination'] = self.pagination.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
+        _items = []
+        if self.data:
+            for _item in self.data:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['data'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of MetaResponse from a dict"""
+        """Create an instance of VariantResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "pagination": ListResponseMetaPagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None
+            "data": [GetVariantAsCurator200Response.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None,
+            "cursor": obj.get("cursor")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/metadata_presentation.py` & `odm_api-1.57.0/odm_api/models/omics_response_data_presentation_data_inner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,97 +1,97 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from odm_api.models.data_presentation_relationships import DataPresentationRelationships
-from odm_api.models.metadata_presentation_metadata import MetadataPresentationMetadata
 from typing import Optional, Set
 from typing_extensions import Self
 
-class MetadataPresentation(BaseModel):
+class OmicsResponseDataPresentationDataInner(BaseModel):
     """
-    A description of object metadata.  This will contain: - `genestack:accession`: the object ID - `Study Title` (for studies) - `Sample ID` (for samples) - all other attributes defined in the linked template (if any)
+    OmicsResponseDataPresentationDataInner
     """ # noqa: E501
-    metadata: Optional[MetadataPresentationMetadata] = None
+    item_id: Optional[StrictStr] = Field(default=None, alias="itemId")
+    metadata: Optional[Dict[str, Any]] = None
     relationships: Optional[DataPresentationRelationships] = None
-    __properties: ClassVar[List[str]] = ["metadata", "relationships"]
+    __properties: ClassVar[List[str]] = ["itemId", "metadata", "relationships"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of MetadataPresentation from a JSON string"""
+        """Create an instance of OmicsResponseDataPresentationDataInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "item_id",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of metadata
-        if self.metadata:
-            _dict['metadata'] = self.metadata.to_dict()
         # override the default output from pydantic by calling `to_dict()` of relationships
         if self.relationships:
             _dict['relationships'] = self.relationships.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of MetadataPresentation from a dict"""
+        """Create an instance of OmicsResponseDataPresentationDataInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "metadata": MetadataPresentationMetadata.from_dict(obj["metadata"]) if obj.get("metadata") is not None else None,
+            "itemId": obj.get("itemId"),
+            "metadata": obj.get("metadata"),
             "relationships": DataPresentationRelationships.from_dict(obj["relationships"]) if obj.get("relationships") is not None else None
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/metadata_presentation_metadata.py` & `odm_api-1.57.0/odm_api/models/study_validation_summary_samples_inner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from odm_api.models.group_validation_summary_attributes_inner import GroupValidationSummaryAttributesInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class MetadataPresentationMetadata(BaseModel):
+class StudyValidationSummarySamplesInner(BaseModel):
     """
-    MetadataPresentationMetadata
+    StudyValidationSummarySamplesInner
     """ # noqa: E501
-    source: Optional[StrictStr] = None
-    name: Optional[StrictStr] = None
-    public: Optional[StrictBool] = None
-    id: Optional[StrictStr] = None
-    content: Optional[Dict[str, Any]] = None
-    data_type: Optional[StrictStr] = Field(default=None, alias="dataType")
-    content_map: Optional[Dict[str, Dict[str, Any]]] = Field(default=None, alias="contentMap")
-    metadata_content: Optional[Dict[str, Dict[str, Any]]] = Field(default=None, alias="metadataContent")
-    file_id_associated_with_template: Optional[StrictStr] = Field(default=None, alias="fileIdAssociatedWithTemplate")
-    __properties: ClassVar[List[str]] = ["source", "name", "public", "id", "content", "dataType", "contentMap", "metadataContent", "fileIdAssociatedWithTemplate"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    group_accession: Optional[StrictStr] = Field(default=None, alias="groupAccession")
+    attributes: Optional[List[GroupValidationSummaryAttributesInner]] = None
+    __properties: ClassVar[List[str]] = ["groupAccession", "attributes"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of MetadataPresentationMetadata from a JSON string"""
+        """Create an instance of StudyValidationSummarySamplesInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,30 +66,32 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in attributes (list)
+        _items = []
+        if self.attributes:
+            for _item in self.attributes:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['attributes'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of MetadataPresentationMetadata from a dict"""
+        """Create an instance of StudyValidationSummarySamplesInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "source": obj.get("source"),
-            "name": obj.get("name"),
-            "public": obj.get("public"),
-            "id": obj.get("id"),
-            "content": obj.get("content"),
-            "dataType": obj.get("dataType"),
-            "fileIdAssociatedWithTemplate": obj.get("fileIdAssociatedWithTemplate")
+            "groupAccession": obj.get("groupAccession"),
+            "attributes": [GroupValidationSummaryAttributesInner.from_dict(_item) for _item in obj["attributes"]] if obj.get("attributes") is not None else None
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/omics_response.py` & `odm_api-1.57.0/odm_api/models/omics_response_metadata_presentation.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,60 +1,61 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from odm_api.models.omics_response_metadata_presentation_data_inner import OmicsResponseMetadataPresentationDataInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OmicsResponse(BaseModel):
+class OmicsResponseMetadataPresentation(BaseModel):
     """
-    OmicsResponse
+    OmicsResponseMetadataPresentation
     """ # noqa: E501
-    data: Optional[List[Dict[str, Any]]] = None
+    data: Optional[List[OmicsResponseMetadataPresentationDataInner]] = None
     results_exhausted: Optional[StrictBool] = Field(default=None, alias="resultsExhausted")
     log: Optional[List[StrictStr]] = None
     cursor: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["data", "resultsExhausted", "log", "cursor"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of OmicsResponse from a JSON string"""
+        """Create an instance of OmicsResponseMetadataPresentation from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,27 +68,34 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
+        _items = []
+        if self.data:
+            for _item in self.data:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['data'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of OmicsResponse from a dict"""
+        """Create an instance of OmicsResponseMetadataPresentation from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "data": obj.get("data"),
+            "data": [OmicsResponseMetadataPresentationDataInner.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None,
             "resultsExhausted": obj.get("resultsExhausted"),
             "log": obj.get("log"),
             "cursor": obj.get("cursor")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/omics_response_data_presentation.py` & `odm_api-1.57.0/odm_api/models/meta_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,58 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.omics_response_data_presentation_data_inner import OmicsResponseDataPresentationDataInner
+from odm_api.models.list_response_meta_pagination import ListResponseMetaPagination
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OmicsResponseDataPresentation(BaseModel):
+class MetaResponse(BaseModel):
     """
-    OmicsResponseDataPresentation
+    MetaResponse
     """ # noqa: E501
-    data: Optional[List[OmicsResponseDataPresentationDataInner]] = None
-    results_exhausted: Optional[StrictBool] = Field(default=None, alias="resultsExhausted")
-    log: Optional[List[StrictStr]] = None
-    cursor: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["data", "resultsExhausted", "log", "cursor"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    pagination: Optional[ListResponseMetaPagination] = None
+    __properties: ClassVar[List[str]] = ["pagination"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of OmicsResponseDataPresentation from a JSON string"""
+        """Create an instance of MetaResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,34 +65,27 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
-        _items = []
-        if self.data:
-            for _item in self.data:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['data'] = _items
+        # override the default output from pydantic by calling `to_dict()` of pagination
+        if self.pagination:
+            _dict['pagination'] = self.pagination.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of OmicsResponseDataPresentation from a dict"""
+        """Create an instance of MetaResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "data": [OmicsResponseDataPresentationDataInner.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None,
-            "resultsExhausted": obj.get("resultsExhausted"),
-            "log": obj.get("log"),
-            "cursor": obj.get("cursor")
+            "pagination": ListResponseMetaPagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/omics_response_data_presentation_data_inner.py` & `odm_api-1.57.0/odm_api/models/patch_operation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,98 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.data_presentation_relationships import DataPresentationRelationships
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OmicsResponseDataPresentationDataInner(BaseModel):
+class PatchOperation(BaseModel):
     """
-    OmicsResponseDataPresentationDataInner
+    PatchOperation
     """ # noqa: E501
-    item_id: Optional[StrictStr] = Field(default=None, alias="itemId")
-    metadata: Optional[Dict[str, Any]] = None
-    relationships: Optional[DataPresentationRelationships] = None
-    __properties: ClassVar[List[str]] = ["itemId", "metadata", "relationships"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    op: StrictStr
+    path: Optional[StrictStr] = None
+    value: Optional[Dict[str, Any]] = Field(default=None, description="Corresponding 'value' of that field specified by 'path'")
+    __properties: ClassVar[List[str]] = ["op", "path", "value"]
+
+    @field_validator('op')
+    def op_validate_enum(cls, value):
+        """Validates the enum"""
+        if value not in set(['add', 'replace', 'remove']):
+            raise ValueError("must be one of enum values ('add', 'replace', 'remove')")
+        return value
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of OmicsResponseDataPresentationDataInner from a JSON string"""
+        """Create an instance of PatchOperation from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "item_id",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of relationships
-        if self.relationships:
-            _dict['relationships'] = self.relationships.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of OmicsResponseDataPresentationDataInner from a dict"""
+        """Create an instance of PatchOperation from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "itemId": obj.get("itemId"),
-            "metadata": obj.get("metadata"),
-            "relationships": DataPresentationRelationships.from_dict(obj["relationships"]) if obj.get("relationships") is not None else None
+            "op": obj.get("op"),
+            "path": obj.get("path"),
+            "value": obj.get("value")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/omics_response_metadata_presentation_data_inner.py` & `odm_api-1.57.0/odm_api/models/attribute_invalid_value.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.data_presentation_relationships import DataPresentationRelationships
-from odm_api.models.metadata_presentation_metadata import MetadataPresentationMetadata
+from odm_api.models.attribute_invalid_value_errors_inner import AttributeInvalidValueErrorsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OmicsResponseMetadataPresentationDataInner(BaseModel):
+class AttributeInvalidValue(BaseModel):
     """
-    A description of object metadata.  This will contain: - `genestack:accession`: the object ID - `Study Title` (for studies) - `Sample ID` (for samples) - all other attributes defined in the linked template (if any)
+    AttributeInvalidValue
     """ # noqa: E501
-    metadata: Optional[MetadataPresentationMetadata] = None
-    relationships: Optional[DataPresentationRelationships] = None
-    __properties: ClassVar[List[str]] = ["metadata", "relationships"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    value: Optional[Dict[str, Any]] = None
+    count: Optional[StrictInt] = None
+    errors: Optional[List[AttributeInvalidValueErrorsInner]] = None
+    __properties: ClassVar[List[str]] = ["value", "count", "errors"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of OmicsResponseMetadataPresentationDataInner from a JSON string"""
+        """Create an instance of AttributeInvalidValue from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,31 +67,33 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of metadata
-        if self.metadata:
-            _dict['metadata'] = self.metadata.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of relationships
-        if self.relationships:
-            _dict['relationships'] = self.relationships.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in errors (list)
+        _items = []
+        if self.errors:
+            for _item in self.errors:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['errors'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of OmicsResponseMetadataPresentationDataInner from a dict"""
+        """Create an instance of AttributeInvalidValue from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "metadata": MetadataPresentationMetadata.from_dict(obj["metadata"]) if obj.get("metadata") is not None else None,
-            "relationships": DataPresentationRelationships.from_dict(obj["relationships"]) if obj.get("relationships") is not None else None
+            "value": obj.get("value"),
+            "count": obj.get("count"),
+            "errors": [AttributeInvalidValueErrorsInner.from_dict(_item) for _item in obj["errors"]] if obj.get("errors") is not None else None
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/output.py` & `odm_api-1.57.0/odm_api/models/validation_error.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.output_errors_inner import OutputErrorsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Output(BaseModel):
+class ValidationError(BaseModel):
     """
-    job execution output
+    ValidationError
     """ # noqa: E501
-    status: StrictStr = Field(description="current job status")
-    result: Optional[Dict[str, Any]] = Field(default=None, description="job result object (available if job completed successfully)")
-    errors: Optional[List[OutputErrorsInner]] = Field(default=None, description="array of errors occurred during execution of the job (available if job failed)")
-    __properties: ClassVar[List[str]] = ["status", "result", "errors"]
+    error_type: Optional[StrictStr] = Field(default=None, alias="errorType")
+    error_message: Optional[StrictStr] = Field(default=None, alias="errorMessage")
+    __properties: ClassVar[List[str]] = ["errorType", "errorMessage"]
 
-    @field_validator('status')
-    def status_validate_enum(cls, value):
+    @field_validator('error_type')
+    def error_type_validate_enum(cls, value):
         """Validates the enum"""
-        if value not in set(['COMPLETED', 'STARTING', 'RUNNING', 'STOPPING', 'STOPPED', 'FAILED', 'ABANDONED', 'UNKNOWN']):
-            raise ValueError("must be one of enum values ('COMPLETED', 'STARTING', 'RUNNING', 'STOPPING', 'STOPPED', 'FAILED', 'ABANDONED', 'UNKNOWN')")
+        if value is None:
+            return value
+
+        if value not in set(['VALUE_NOT_SET', 'VOCABULARY_NOT_FOUND', 'TYPE_NOT_MATCH', 'MISSING_ATTRIBUTE', 'SYNONYM_ATTRIBUTE']):
+            raise ValueError("must be one of enum values ('VALUE_NOT_SET', 'VOCABULARY_NOT_FOUND', 'TYPE_NOT_MATCH', 'MISSING_ATTRIBUTE', 'SYNONYM_ATTRIBUTE')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Output from a JSON string"""
+        """Create an instance of ValidationError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,33 +75,25 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in errors (list)
-        _items = []
-        if self.errors:
-            for _item in self.errors:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['errors'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Output from a dict"""
+        """Create an instance of ValidationError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "status": obj.get("status"),
-            "result": obj.get("result"),
-            "errors": [OutputErrorsInner.from_dict(_item) for _item in obj["errors"]] if obj.get("errors") is not None else None
+            "errorType": obj.get("errorType"),
+            "errorMessage": obj.get("errorMessage")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/output_errors_inner.py` & `odm_api-1.57.0/odm_api/models/job_runtime_error.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from odm_api.models.job_runtime_error_stack_inner import JobRuntimeErrorStackInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class OutputErrorsInner(BaseModel):
+class JobRuntimeError(BaseModel):
     """
-    OutputErrorsInner
+    JobRuntimeError
     """ # noqa: E501
     stage: Optional[StrictStr] = None
     stack: Optional[List[JobRuntimeErrorStackInner]] = None
     __properties: ClassVar[List[str]] = ["stage", "stack"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of OutputErrorsInner from a JSON string"""
+        """Create an instance of JobRuntimeError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -77,15 +77,15 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['stack'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of OutputErrorsInner from a dict"""
+        """Create an instance of JobRuntimeError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `odm-api-0.0.1/odm_api/models/page_request.py` & `odm_api-1.57.0/odm_api/models/batch_of_ids.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PageRequest(BaseModel):
+class BatchOfIds(BaseModel):
     """
-    PageRequest
+    Request model for getting links by many IDs.
     """ # noqa: E501
+    first_type: StrictStr = Field(description="Type of the objects.", alias="firstType")
+    first_ids: List[StrictStr] = Field(description="Array of the object IDs with the same type.", alias="firstIds")
     offset: Optional[StrictInt] = Field(default=None, description="Param says to skip that many links before beginning to return links. Default: 0.")
     limit: Optional[StrictInt] = Field(default=None, description="Param says to limit the count of returned links. Default: 1000.")
-    __properties: ClassVar[List[str]] = ["offset", "limit"]
+    __properties: ClassVar[List[str]] = ["firstType", "firstIds", "offset", "limit"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PageRequest from a JSON string"""
+        """Create an instance of BatchOfIds from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,21 +71,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PageRequest from a dict"""
+        """Create an instance of BatchOfIds from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "firstType": obj.get("firstType"),
+            "firstIds": obj.get("firstIds"),
             "offset": obj.get("offset"),
             "limit": obj.get("limit")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/runs_response.py` & `odm_api-1.57.0/test/test_find_objects_response_objects_page_content_inner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,61 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-from __future__ import annotations
-import pprint
-import re  # noqa: F401
-import json
-
-from pydantic import BaseModel, Field, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
-from typing import Optional, Set
-from typing_extensions import Self
-
-class RunsResponse(BaseModel):
-    """
-    RunsResponse
-    """ # noqa: E501
-    runs: Optional[List[Dict[str, Any]]] = None
-    experiment: Optional[StrictStr] = None
-    warnings: Optional[List[StrictStr]] = None
-    version_chain_id: Optional[StrictStr] = Field(default=None, alias="versionChainId")
-    __properties: ClassVar[List[str]] = ["runs", "experiment", "warnings", "versionChainId"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
-
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.model_dump(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of RunsResponse from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Return the dictionary representation of the model using alias.
-
-        This has the following differences from calling pydantic's
-        `self.model_dump(by_alias=True)`:
-
-        * `None` is only added to the output dict for nullable fields that
-          were set at model initialization. Other fields with value `None`
-          are ignored.
-        """
-        excluded_fields: Set[str] = set([
-        ])
+import unittest
 
-        _dict = self.model_dump(
-            by_alias=True,
-            exclude=excluded_fields,
-            exclude_none=True,
-        )
-        return _dict
+from odm_api.models.find_objects_response_objects_page_content_inner import FindObjectsResponseObjectsPageContentInner
+
+class TestFindObjectsResponseObjectsPageContentInner(unittest.TestCase):
+    """FindObjectsResponseObjectsPageContentInner unit test stubs"""
+
+    def setUp(self):
+        pass
 
-    @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of RunsResponse from a dict"""
-        if obj is None:
-            return None
-
-        if not isinstance(obj, dict):
-            return cls.model_validate(obj)
-
-        _obj = cls.model_validate({
-            "runs": obj.get("runs"),
-            "experiment": obj.get("experiment"),
-            "warnings": obj.get("warnings"),
-            "versionChainId": obj.get("versionChainId")
-        })
-        return _obj
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional) -> FindObjectsResponseObjectsPageContentInner:
+        """Test FindObjectsResponseObjectsPageContentInner
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `FindObjectsResponseObjectsPageContentInner`
+        """
+        model = FindObjectsResponseObjectsPageContentInner()
+        if include_optional:
+            return FindObjectsResponseObjectsPageContentInner(
+                accession = '',
+                name = '',
+                owner = '',
+                file_creation = '',
+                size = 56,
+                has_facs = True,
+                has_genomic = True,
+                has_transcriptomics = True,
+                summary = [
+                    {values=[values, values], key=key}
+                    ]
+            )
+        else:
+            return FindObjectsResponseObjectsPageContentInner(
+        )
+        """
 
+    def testFindObjectsResponseObjectsPageContentInner(self):
+        """Test FindObjectsResponseObjectsPageContentInner"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `odm-api-0.0.1/odm_api/models/scim_error_response.py` & `odm_api-1.57.0/odm_api/models/search_study_request_filters_inner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,80 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SCIMErrorResponse(BaseModel):
+class SearchStudyRequestFiltersInner(BaseModel):
     """
-    SCIMErrorResponse
+    SearchStudyRequestFiltersInner
     """ # noqa: E501
-    detail: Optional[StrictStr] = Field(default=None, description="Detailed error message")
-    schemas: Optional[List[StrictStr]] = None
-    scim_type: Optional[StrictStr] = Field(default=None, description="Bad request type when status code is 400", alias="scimType")
-    status: StrictStr = Field(description="Same as HTTP status code, e.g. 400, 403, etc.")
-    __properties: ClassVar[List[str]] = ["detail", "schemas", "scimType", "status"]
+    type: Optional[StrictStr] = None
+    filter_option_id: Optional[StrictStr] = Field(default=None, alias="filterOptionId")
+    match: Optional[StrictStr] = None
+    mode: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["type", "filterOptionId", "match", "mode"]
 
-    @field_validator('schemas')
-    def schemas_validate_enum(cls, value):
+    @field_validator('type')
+    def type_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        for i in value:
-            if i not in set(['urn:ietf:params:scim:api:messages:2.0:Error']):
-                raise ValueError("each list item must be one of ('urn:ietf:params:scim:api:messages:2.0:Error')")
+        if value not in set(['FULL_TEXT', 'SELECT']):
+            raise ValueError("must be one of enum values ('FULL_TEXT', 'SELECT')")
         return value
 
-    @field_validator('scim_type')
-    def scim_type_validate_enum(cls, value):
+    @field_validator('mode')
+    def mode_validate_enum(cls, value):
         """Validates the enum"""
         if value is None:
             return value
 
-        if value not in set(['uniqueness', 'tooMany', 'mutability', 'sensitive', 'invalidSyntax', 'invalidFilter', 'invalidPath', 'invalidValue', 'invalidVers', 'noTarget']):
-            raise ValueError("must be one of enum values ('uniqueness', 'tooMany', 'mutability', 'sensitive', 'invalidSyntax', 'invalidFilter', 'invalidPath', 'invalidValue', 'invalidVers', 'noTarget')")
+        if value not in set(['STRICT', 'USE_NARROWER_TERMS']):
+            raise ValueError("must be one of enum values ('STRICT', 'USE_NARROWER_TERMS')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SCIMErrorResponse from a JSON string"""
+        """Create an instance of SearchStudyRequestFiltersInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -92,23 +91,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SCIMErrorResponse from a dict"""
+        """Create an instance of SearchStudyRequestFiltersInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "detail": obj.get("detail"),
-            "schemas": obj.get("schemas"),
-            "scimType": obj.get("scimType"),
-            "status": obj.get("status")
+            "type": obj.get("type"),
+            "filterOptionId": obj.get("filterOptionId"),
+            "match": obj.get("match"),
+            "mode": obj.get("mode")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/search_study_request_page.py` & `odm_api-1.57.0/odm_api/models/member.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class SearchStudyRequestPage(BaseModel):
+class Member(BaseModel):
     """
-    SearchStudyRequestPage
+    Member
     """ # noqa: E501
-    offset: Optional[StrictInt] = Field(default=None, description="Param says to skip that many links before beginning to return links. Default: 0.")
-    limit: Optional[StrictInt] = Field(default=None, description="Param says to limit the count of returned links. Default: 1000.")
-    __properties: ClassVar[List[str]] = ["offset", "limit"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    value: StrictStr
+    display: Optional[StrictStr] = None
+    ref: StrictStr = Field(description="The URI of the member resource", alias="$ref")
+    __properties: ClassVar[List[str]] = ["value", "display", "$ref"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of SearchStudyRequestPage from a JSON string"""
+        """Create an instance of Member from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,21 +70,22 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of SearchStudyRequestPage from a dict"""
+        """Create an instance of Member from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "offset": obj.get("offset"),
-            "limit": obj.get("limit")
+            "value": obj.get("value"),
+            "display": obj.get("display"),
+            "$ref": obj.get("$ref")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/start_import_flow_cytometry_request.py` & `odm_api-1.57.0/odm_api/models/sample_source.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,105 +1,91 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class StartImportFlowCytometryRequest(BaseModel):
+class SampleSource(BaseModel):
     """
-    import signal data request
+    SampleSource
     """ # noqa: E501
-    source: Optional[StrictStr] = None
-    metadata_link: Optional[StrictStr] = Field(default=None, alias="metadataLink")
-    data_link: StrictStr = Field(alias="dataLink")
-    template_id: Optional[StrictStr] = Field(default=None, alias="templateId")
-    previous_version: Optional[StrictStr] = Field(default=None, alias="previousVersion")
-    __properties: ClassVar[List[str]] = ["source", "metadataLink", "dataLink", "templateId", "previousVersion"]
-
-    @field_validator('source')
-    def source_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['ARVADOS', 'S3', 'HTTP']):
-            raise ValueError("must be one of enum values ('ARVADOS', 'S3', 'HTTP')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    template_id: Optional[StrictStr] = Field(default=None, description="ID of template file.", alias="templateId")
+    link: StrictStr = Field(description="URL of sample file.")
+    __properties: ClassVar[List[str]] = ["templateId", "link"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of StartImportFlowCytometryRequest from a JSON string"""
+        """Create an instance of SampleSource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "template_id",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of StartImportFlowCytometryRequest from a dict"""
+        """Create an instance of SampleSource from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "source": obj.get("source"),
-            "metadataLink": obj.get("metadataLink"),
-            "dataLink": obj.get("dataLink"),
             "templateId": obj.get("templateId"),
-            "previousVersion": obj.get("previousVersion")
+            "link": obj.get("link")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/study_generic_source.py` & `odm_api-1.57.0/odm_api/models/variant_signal_source.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class StudyGenericSource(BaseModel):
+class VariantSignalSource(BaseModel):
     """
-    StudyGenericSource
+    VariantSignalSource
     """ # noqa: E501
-    link: StrictStr = Field(description="URL for a file with Study metadata.")
     template_id: Optional[StrictStr] = Field(default=None, description="ID of template file.", alias="templateId")
-    __properties: ClassVar[List[str]] = ["link", "templateId"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    link: StrictStr = Field(description="URL of the signal file.")
+    metadata_link: Optional[StrictStr] = Field(default=None, description="URL of the signal file metadata.", alias="metadataLink")
+    previous_version: Optional[StrictStr] = Field(default=None, description="Accession of matrix group or matrix group version chain.", alias="previousVersion")
+    __properties: ClassVar[List[str]] = ["templateId", "link", "metadataLink", "previousVersion"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of StudyGenericSource from a JSON string"""
+        """Create an instance of VariantSignalSource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -71,21 +73,23 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of StudyGenericSource from a dict"""
+        """Create an instance of VariantSignalSource from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
+            "templateId": obj.get("templateId"),
             "link": obj.get("link"),
-            "templateId": obj.get("templateId")
+            "metadataLink": obj.get("metadataLink"),
+            "previousVersion": obj.get("previousVersion")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/study_search_info.py` & `odm_api-1.57.0/odm_api/models/find_objects_response_objects_page_content_inner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from odm_api.models.find_objects_response_objects_page_content_inner_summary_inner import FindObjectsResponseObjectsPageContentInnerSummaryInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class StudySearchInfo(BaseModel):
+class FindObjectsResponseObjectsPageContentInner(BaseModel):
     """
-    StudySearchInfo
+    FindObjectsResponseObjectsPageContentInner
     """ # noqa: E501
     accession: Optional[StrictStr] = None
     name: Optional[StrictStr] = None
     owner: Optional[StrictStr] = None
     file_creation: Optional[StrictStr] = Field(default=None, alias="fileCreation")
     size: Optional[StrictInt] = None
     has_facs: Optional[StrictBool] = Field(default=None, alias="hasFacs")
     has_genomic: Optional[StrictBool] = Field(default=None, alias="hasGenomic")
     has_transcriptomics: Optional[StrictBool] = Field(default=None, alias="hasTranscriptomics")
     summary: Optional[List[FindObjectsResponseObjectsPageContentInnerSummaryInner]] = None
     __properties: ClassVar[List[str]] = ["accession", "name", "owner", "fileCreation", "size", "hasFacs", "hasGenomic", "hasTranscriptomics", "summary"]
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of StudySearchInfo from a JSON string"""
+        """Create an instance of FindObjectsResponseObjectsPageContentInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -84,15 +84,15 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['summary'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of StudySearchInfo from a dict"""
+        """Create an instance of FindObjectsResponseObjectsPageContentInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `odm-api-0.0.1/odm_api/models/study_validation_summary_samples_inner.py` & `odm_api-1.57.0/test/test_study_validation_summary_samples_inner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,54 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-from __future__ import annotations
-import pprint
-import re  # noqa: F401
-import json
-
-from pydantic import BaseModel, Field, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.group_validation_summary_attributes_inner import GroupValidationSummaryAttributesInner
-from typing import Optional, Set
-from typing_extensions import Self
-
-class StudyValidationSummarySamplesInner(BaseModel):
-    """
-    StudyValidationSummarySamplesInner
-    """ # noqa: E501
-    group_accession: Optional[StrictStr] = Field(default=None, alias="groupAccession")
-    attributes: Optional[List[GroupValidationSummaryAttributesInner]] = None
-    __properties: ClassVar[List[str]] = ["groupAccession", "attributes"]
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
-
-
-    def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
-        return pprint.pformat(self.model_dump(by_alias=True))
-
-    def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
-        # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
-        return json.dumps(self.to_dict())
-
-    @classmethod
-    def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of StudyValidationSummarySamplesInner from a JSON string"""
-        return cls.from_dict(json.loads(json_str))
-
-    def to_dict(self) -> Dict[str, Any]:
-        """Return the dictionary representation of the model using alias.
-
-        This has the following differences from calling pydantic's
-        `self.model_dump(by_alias=True)`:
-
-        * `None` is only added to the output dict for nullable fields that
-          were set at model initialization. Other fields with value `None`
-          are ignored.
-        """
-        excluded_fields: Set[str] = set([
-        ])
+import unittest
+
+from odm_api.models.study_validation_summary_samples_inner import StudyValidationSummarySamplesInner
+
+class TestStudyValidationSummarySamplesInner(unittest.TestCase):
+    """StudyValidationSummarySamplesInner unit test stubs"""
+
+    def setUp(self):
+        pass
 
-        _dict = self.model_dump(
-            by_alias=True,
-            exclude=excluded_fields,
-            exclude_none=True,
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional) -> StudyValidationSummarySamplesInner:
+        """Test StudyValidationSummarySamplesInner
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `StudyValidationSummarySamplesInner`
+        """
+        model = StudyValidationSummarySamplesInner()
+        if include_optional:
+            return StudyValidationSummarySamplesInner(
+                group_accession = '',
+                attributes = [
+                    {attributeName=attributeName, attributeInvalidValues=[{count=0, value={}, errors=[{errorType=VALUE_NOT_SET, errorMessage=errorMessage}, {errorType=VALUE_NOT_SET, errorMessage=errorMessage}]}, {count=0, value={}, errors=[{errorType=VALUE_NOT_SET, errorMessage=errorMessage}, {errorType=VALUE_NOT_SET, errorMessage=errorMessage}]}]}
+                    ]
+            )
+        else:
+            return StudyValidationSummarySamplesInner(
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in attributes (list)
-        _items = []
-        if self.attributes:
-            for _item in self.attributes:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['attributes'] = _items
-        return _dict
-
-    @classmethod
-    def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of StudyValidationSummarySamplesInner from a dict"""
-        if obj is None:
-            return None
-
-        if not isinstance(obj, dict):
-            return cls.model_validate(obj)
-
-        _obj = cls.model_validate({
-            "groupAccession": obj.get("groupAccession"),
-            "attributes": [GroupValidationSummaryAttributesInner.from_dict(_item) for _item in obj["attributes"]] if obj.get("attributes") is not None else None
-        })
-        return _obj
+        """
 
+    def testStudyValidationSummarySamplesInner(self):
+        """Test StudyValidationSummarySamplesInner"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `odm-api-0.0.1/odm_api/models/user.py` & `odm_api-1.57.0/odm_api/models/create_user_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List, Optional
 from odm_api.models.create_user_request_emails_inner import CreateUserRequestEmailsInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class User(BaseModel):
+class CreateUserRequest(BaseModel):
     """
-    User
+    CreateUserRequest
     """ # noqa: E501
     active: StrictBool = Field(description="User status")
     emails: List[CreateUserRequestEmailsInner]
     external_id: Optional[StrictStr] = Field(default=None, description="External unique resource id", alias="externalId")
     id: Optional[StrictStr] = Field(default=None, description="Unique resource id")
     schemas: Optional[List[StrictStr]] = None
     user_name: Optional[StrictStr] = Field(default=None, alias="userName")
@@ -43,33 +43,33 @@
             return value
 
         for i in value:
             if i not in set(['urn:ietf:params:scim:schemas:core:2.0:User']):
                 raise ValueError("each list item must be one of ('urn:ietf:params:scim:schemas:core:2.0:User')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of User from a JSON string"""
+        """Create an instance of CreateUserRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -93,15 +93,15 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['emails'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of User from a dict"""
+        """Create an instance of CreateUserRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `odm-api-0.0.1/odm_api/models/user_patch.py` & `odm_api-1.57.0/odm_api/models/create_group_request_members_inner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
-from typing import Any, ClassVar, Dict, List
-from odm_api.models.user_patch_operations_inner import UserPatchOperationsInner
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserPatch(BaseModel):
+class CreateGroupRequestMembersInner(BaseModel):
     """
-    UserPatch
+    CreateGroupRequestMembersInner
     """ # noqa: E501
-    operations: List[UserPatchOperationsInner] = Field(description="Patch operations list", alias="Operations")
-    schemas: List[StrictStr]
-    __properties: ClassVar[List[str]] = ["Operations", "schemas"]
-
-    @field_validator('schemas')
-    def schemas_validate_enum(cls, value):
-        """Validates the enum"""
-        for i in value:
-            if i not in set(['urn:ietf:params:scim:api:messages:2.0:PatchOp']):
-                raise ValueError("each list item must be one of ('urn:ietf:params:scim:api:messages:2.0:PatchOp')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    value: StrictStr
+    display: Optional[StrictStr] = None
+    ref: StrictStr = Field(description="The URI of the member resource", alias="$ref")
+    __properties: ClassVar[List[str]] = ["value", "display", "$ref"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserPatch from a JSON string"""
+        """Create an instance of CreateGroupRequestMembersInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -74,32 +66,26 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in operations (list)
-        _items = []
-        if self.operations:
-            for _item in self.operations:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['Operations'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserPatch from a dict"""
+        """Create an instance of CreateGroupRequestMembersInner from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "Operations": [UserPatchOperationsInner.from_dict(_item) for _item in obj["Operations"]] if obj.get("Operations") is not None else None,
-            "schemas": obj.get("schemas")
+            "value": obj.get("value"),
+            "display": obj.get("display"),
+            "$ref": obj.get("$ref")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/user_response.py` & `odm_api-1.57.0/odm_api/models/study_search_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,66 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictBool, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictInt, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
-from odm_api.models.create_user201_response_all_of_meta import CreateUser201ResponseAllOfMeta
-from odm_api.models.create_user_request_emails_inner import CreateUserRequestEmailsInner
+from odm_api.models.find_objects_response_objects_page_content_inner_summary_inner import FindObjectsResponseObjectsPageContentInnerSummaryInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserResponse(BaseModel):
+class StudySearchInfo(BaseModel):
     """
-    UserResponse
+    StudySearchInfo
     """ # noqa: E501
-    active: StrictBool = Field(description="User status")
-    emails: List[CreateUserRequestEmailsInner]
-    external_id: Optional[StrictStr] = Field(default=None, description="External unique resource id", alias="externalId")
-    id: Optional[StrictStr] = Field(default=None, description="Unique resource id")
-    schemas: Optional[List[StrictStr]] = None
-    user_name: Optional[StrictStr] = Field(default=None, alias="userName")
-    display_name: StrictStr = Field(alias="displayName")
-    meta: Optional[CreateUser201ResponseAllOfMeta] = None
-    __properties: ClassVar[List[str]] = ["active", "emails", "externalId", "id", "schemas", "userName", "displayName", "meta"]
-
-    @field_validator('schemas')
-    def schemas_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        for i in value:
-            if i not in set(['urn:ietf:params:scim:schemas:core:2.0:User']):
-                raise ValueError("each list item must be one of ('urn:ietf:params:scim:schemas:core:2.0:User')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    accession: Optional[StrictStr] = None
+    name: Optional[StrictStr] = None
+    owner: Optional[StrictStr] = None
+    file_creation: Optional[StrictStr] = Field(default=None, alias="fileCreation")
+    size: Optional[StrictInt] = None
+    has_facs: Optional[StrictBool] = Field(default=None, alias="hasFacs")
+    has_genomic: Optional[StrictBool] = Field(default=None, alias="hasGenomic")
+    has_transcriptomics: Optional[StrictBool] = Field(default=None, alias="hasTranscriptomics")
+    summary: Optional[List[FindObjectsResponseObjectsPageContentInnerSummaryInner]] = None
+    __properties: ClassVar[List[str]] = ["accession", "name", "owner", "fileCreation", "size", "hasFacs", "hasGenomic", "hasTranscriptomics", "summary"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserResponse from a JSON string"""
+        """Create an instance of StudySearchInfo from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -84,41 +73,39 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in emails (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in summary (list)
         _items = []
-        if self.emails:
-            for _item in self.emails:
+        if self.summary:
+            for _item in self.summary:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['emails'] = _items
-        # override the default output from pydantic by calling `to_dict()` of meta
-        if self.meta:
-            _dict['meta'] = self.meta.to_dict()
+            _dict['summary'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserResponse from a dict"""
+        """Create an instance of StudySearchInfo from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "active": obj.get("active"),
-            "emails": [CreateUserRequestEmailsInner.from_dict(_item) for _item in obj["emails"]] if obj.get("emails") is not None else None,
-            "externalId": obj.get("externalId"),
-            "id": obj.get("id"),
-            "schemas": obj.get("schemas"),
-            "userName": obj.get("userName"),
-            "displayName": obj.get("displayName"),
-            "meta": CreateUser201ResponseAllOfMeta.from_dict(obj["meta"]) if obj.get("meta") is not None else None
+            "accession": obj.get("accession"),
+            "name": obj.get("name"),
+            "owner": obj.get("owner"),
+            "fileCreation": obj.get("fileCreation"),
+            "size": obj.get("size"),
+            "hasFacs": obj.get("hasFacs"),
+            "hasGenomic": obj.get("hasGenomic"),
+            "hasTranscriptomics": obj.get("hasTranscriptomics"),
+            "summary": [FindObjectsResponseObjectsPageContentInnerSummaryInner.from_dict(_item) for _item in obj["summary"]] if obj.get("summary") is not None else None
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/validation_error.py` & `odm_api-1.57.0/odm_api/models/base_error_response_error.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,57 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
-from typing import Any, ClassVar, Dict, List, Optional
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ValidationError(BaseModel):
+class BaseErrorResponseError(BaseModel):
     """
-    ValidationError
+    BaseErrorResponseError
     """ # noqa: E501
-    error_type: Optional[StrictStr] = Field(default=None, alias="errorType")
-    error_message: Optional[StrictStr] = Field(default=None, alias="errorMessage")
-    __properties: ClassVar[List[str]] = ["errorType", "errorMessage"]
-
-    @field_validator('error_type')
-    def error_type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value is None:
-            return value
-
-        if value not in set(['VALUE_NOT_SET', 'VOCABULARY_NOT_FOUND', 'TYPE_NOT_MATCH', 'MISSING_ATTRIBUTE', 'SYNONYM_ATTRIBUTE']):
-            raise ValueError("must be one of enum values ('VALUE_NOT_SET', 'VOCABULARY_NOT_FOUND', 'TYPE_NOT_MATCH', 'MISSING_ATTRIBUTE', 'SYNONYM_ATTRIBUTE')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    message: StrictStr = Field(description="Detailed error message")
+    __properties: ClassVar[List[str]] = ["message"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ValidationError from a JSON string"""
+        """Create an instance of BaseErrorResponseError from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,21 +68,20 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ValidationError from a dict"""
+        """Create an instance of BaseErrorResponseError from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "errorType": obj.get("errorType"),
-            "errorMessage": obj.get("errorMessage")
+            "message": obj.get("message")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/xref_set_create_request.py` & `odm_api-1.57.0/odm_api/models/detached_collection.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
+from odm_api.models.detached_collection_data_inner import DetachedCollectionDataInner
 from typing import Optional, Set
 from typing_extensions import Self
 
-class XrefSetCreateRequest(BaseModel):
+class DetachedCollection(BaseModel):
     """
-    Create XrefSet request body
+    DetachedCollection
     """ # noqa: E501
-    xref_set_type: StrictStr = Field(description="Type of data stored in XrefSet", alias="xrefSetType")
-    data_link: StrictStr = Field(description="Mapping file link", alias="dataLink")
-    data_source: StrictStr = Field(description="Target storage dataLink points to", alias="dataSource")
-    metadata: Optional[Dict[str, Any]] = Field(default=None, description="Additional user metadata")
-    __properties: ClassVar[List[str]] = ["xrefSetType", "dataLink", "dataSource", "metadata"]
-
-    @field_validator('xref_set_type')
-    def xref_set_type_validate_enum(cls, value):
-        """Validates the enum"""
-        if value not in set(['gene-transcript']):
-            raise ValueError("must be one of enum values ('gene-transcript')")
-        return value
-
-    @field_validator('data_source')
-    def data_source_validate_enum(cls, value):
-        """Validates the enum"""
-        if value not in set(['arvados', 's3', 'http']):
-            raise ValueError("must be one of enum values ('arvados', 's3', 'http')")
-        return value
-
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    data: List[DetachedCollectionDataInner]
+    cursor: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["data", "cursor"]
+
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of XrefSetCreateRequest from a JSON string"""
+        """Create an instance of DetachedCollection from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -81,27 +66,32 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of each item in data (list)
+        _items = []
+        if self.data:
+            for _item in self.data:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['data'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of XrefSetCreateRequest from a dict"""
+        """Create an instance of DetachedCollection from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "xrefSetType": obj.get("xrefSetType"),
-            "dataLink": obj.get("dataLink"),
-            "dataSource": obj.get("dataSource"),
-            "metadata": obj.get("metadata")
+            "data": [DetachedCollectionDataInner.from_dict(_item) for _item in obj["data"]] if obj.get("data") is not None else None,
+            "cursor": obj.get("cursor")
         })
         return _obj
```

### Comparing `odm-api-0.0.1/odm_api/models/xref_set_create_response.py` & `odm_api-1.57.0/odm_api/models/xref_set_create_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, Field, StrictInt, StrictStr, field_validator
+from pydantic import BaseModel, ConfigDict, Field, StrictInt, StrictStr, field_validator
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
 class XrefSetCreateResponse(BaseModel):
     """
     Create XrefSet response body
@@ -38,19 +38,19 @@
     @field_validator('xref_set_type')
     def xref_set_type_validate_enum(cls, value):
         """Validates the enum"""
         if value not in set(['gene-transcript']):
             raise ValueError("must be one of enum values ('gene-transcript')")
         return value
 
-    model_config = {
-        "populate_by_name": True,
-        "validate_assignment": True,
-        "protected_namespaces": (),
-    }
+    model_config = ConfigDict(
+        populate_by_name=True,
+        validate_assignment=True,
+        protected_namespaces=(),
+    )
 
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
```

### Comparing `odm-api-0.0.1/odm_api/rest.py` & `odm_api-1.57.0/odm_api/rest.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -198,14 +198,16 @@
                         preload_content=False
                     )
                 elif content_type == 'multipart/form-data':
                     # must del headers['Content-Type'], or the correct
                     # Content-Type which generated by urllib3 will be
                     # overwritten.
                     del headers['Content-Type']
+                    # Ensures that dict objects are serialized
+                    post_params = [(a, json.dumps(b)) if isinstance(b, dict) else (a,b) for a, b in post_params]
                     r = self.pool_manager.request(
                         method,
                         url,
                         fields=post_params,
                         encode_multipart=True,
                         timeout=timeout,
                         headers=headers,
```

### Comparing `odm-api-0.0.1/odm_api.egg-info/SOURCES.txt` & `odm_api-1.57.0/odm_api.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -63,18 +63,18 @@
 odm_api/models/attribute_validation_summary.py
 odm_api/models/attribute_validation_summary_attribute_invalid_values_inner.py
 odm_api/models/base_error_response.py
 odm_api/models/base_error_response_error.py
 odm_api/models/batch_of_ids.py
 odm_api/models/commit_info.py
 odm_api/models/create_group201_response.py
+odm_api/models/create_group201_response_all_of_meta.py
 odm_api/models/create_group_request.py
 odm_api/models/create_group_request_members_inner.py
 odm_api/models/create_user201_response.py
-odm_api/models/create_user201_response_all_of_meta.py
 odm_api/models/create_user_request.py
 odm_api/models/create_user_request_emails_inner.py
 odm_api/models/data_item.py
 odm_api/models/data_presentation.py
 odm_api/models/data_presentation_relationships.py
 odm_api/models/detached_collection.py
 odm_api/models/detached_collection_data_inner.py
@@ -94,32 +94,34 @@
 odm_api/models/find_objects_response_filter_option_groups_inner_options_inner.py
 odm_api/models/find_objects_response_objects_page.py
 odm_api/models/find_objects_response_objects_page_content_inner.py
 odm_api/models/find_objects_response_objects_page_content_inner_summary_inner.py
 odm_api/models/flow_cytometry_item.py
 odm_api/models/flow_cytometry_response.py
 odm_api/models/flow_cytometry_signal_source.py
-odm_api/models/get_expression_as_user200_response.py
-odm_api/models/get_expression_as_user200_response_feature.py
-odm_api/models/get_expression_as_user200_response_value.py
+odm_api/models/get_expression_as_curator200_response.py
+odm_api/models/get_expression_as_curator200_response_feature.py
 odm_api/models/get_flow_cytometry_as_curator200_response.py
 odm_api/models/get_variant_as_curator200_response.py
 odm_api/models/group.py
 odm_api/models/group_patch.py
+odm_api/models/group_patch_operations_inner.py
 odm_api/models/group_response.py
+odm_api/models/group_response_all_of_members.py
 odm_api/models/group_validation_summary.py
 odm_api/models/group_validation_summary_attributes_inner.py
 odm_api/models/i_metadata.py
 odm_api/models/import_expression_signal_run_request.py
 odm_api/models/import_metadata_request.py
 odm_api/models/import_signal_run_request.py
 odm_api/models/info.py
 odm_api/models/job_runtime_error.py
 odm_api/models/job_runtime_error_stack_inner.py
 odm_api/models/json_metadata.py
+odm_api/models/json_metadata_attributes.py
 odm_api/models/link.py
 odm_api/models/list_response.py
 odm_api/models/list_response_meta.py
 odm_api/models/list_response_meta_pagination.py
 odm_api/models/managed_object.py
 odm_api/models/member.py
 odm_api/models/meta.py
@@ -152,15 +154,14 @@
 odm_api/models/study_generic_source.py
 odm_api/models/study_search_info.py
 odm_api/models/study_validation_summary.py
 odm_api/models/study_validation_summary_samples_inner.py
 odm_api/models/task_info.py
 odm_api/models/user.py
 odm_api/models/user_patch.py
-odm_api/models/user_patch_operations_inner.py
 odm_api/models/user_response.py
 odm_api/models/validation_error.py
 odm_api/models/variant_item.py
 odm_api/models/variant_response.py
 odm_api/models/variant_signal_source.py
 odm_api/models/xref_set_create_request.py
 odm_api/models/xref_set_create_response.py
@@ -174,18 +175,18 @@
 test/test_attribute_validation_summary.py
 test/test_attribute_validation_summary_attribute_invalid_values_inner.py
 test/test_base_error_response.py
 test/test_base_error_response_error.py
 test/test_batch_of_ids.py
 test/test_commit_info.py
 test/test_create_group201_response.py
+test/test_create_group201_response_all_of_meta.py
 test/test_create_group_request.py
 test/test_create_group_request_members_inner.py
 test/test_create_user201_response.py
-test/test_create_user201_response_all_of_meta.py
 test/test_create_user_request.py
 test/test_create_user_request_emails_inner.py
 test/test_data_import_jobs_api.py
 test/test_data_item.py
 test/test_data_presentation.py
 test/test_data_presentation_relationships.py
 test/test_detached_collection.py
@@ -214,34 +215,36 @@
 test/test_flow_cytometry_integration_as_curator_api.py
 test/test_flow_cytometry_integration_as_user_api.py
 test/test_flow_cytometry_item.py
 test/test_flow_cytometry_response.py
 test/test_flow_cytometry_signal_source.py
 test/test_flow_cytometry_spo_tas_curator_api.py
 test/test_flow_cytometry_spo_tas_user_api.py
-test/test_get_expression_as_user200_response.py
-test/test_get_expression_as_user200_response_feature.py
-test/test_get_expression_as_user200_response_value.py
+test/test_get_expression_as_curator200_response.py
+test/test_get_expression_as_curator200_response_feature.py
 test/test_get_flow_cytometry_as_curator200_response.py
 test/test_get_variant_as_curator200_response.py
 test/test_group.py
 test/test_group_patch.py
+test/test_group_patch_operations_inner.py
 test/test_group_response.py
+test/test_group_response_all_of_members.py
 test/test_group_validation_summary.py
 test/test_group_validation_summary_attributes_inner.py
 test/test_groups_api.py
 test/test_i_metadata.py
 test/test_import_expression_signal_run_request.py
 test/test_import_metadata_request.py
 test/test_import_signal_run_request.py
 test/test_info.py
 test/test_job_operations_api.py
 test/test_job_runtime_error.py
 test/test_job_runtime_error_stack_inner.py
 test/test_json_metadata.py
+test/test_json_metadata_attributes.py
 test/test_library_integration_as_curator_api.py
 test/test_library_integration_as_user_api.py
 test/test_library_spo_tas_curator_api.py
 test/test_library_spo_tas_user_api.py
 test/test_link.py
 test/test_linkage_as_curator_api.py
 test/test_linkage_as_user_api.py
@@ -297,15 +300,14 @@
 test/test_study_spo_tas_user_api.py
 test/test_study_validation_summary.py
 test/test_study_validation_summary_samples_inner.py
 test/test_task_info.py
 test/test_tasks_api_api.py
 test/test_user.py
 test/test_user_patch.py
-test/test_user_patch_operations_inner.py
 test/test_user_response.py
 test/test_users_api.py
 test/test_validation_error.py
 test/test_validation_summary_as_curator_api.py
 test/test_variant_integration_as_curator_api.py
 test/test_variant_integration_as_user_api.py
 test/test_variant_item.py
```

### Comparing `odm-api-0.0.1/pyproject.toml` & `odm_api-1.57.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "odm_api"
-version = "0.0.1"
-description = "Tasks API"
+version = "1.57.0"
+description = "ODM API"
 authors = ["OpenAPI Generator Community <team@openapitools.org>"]
 license = "NoLicense"
 readme = "README.md"
-repository = "https://github.com/genestack/odm-openapi"
-keywords = ["OpenAPI", "OpenAPI-Generator", "Tasks API"]
+repository = "https://github.com/genestack/openapi"
+keywords = ["OpenAPI", "OpenAPI-Generator", "ODM API"]
 include = ["odm_api/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 urllib3 = ">= 1.25.3"
 python-dateutil = ">=2.8.2"
```

### Comparing `odm-api-0.0.1/test/test_applied_filter.py` & `odm_api-1.57.0/test/test_filter_option.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.applied_filter import AppliedFilter
+from odm_api.models.filter_option import FilterOption
 
-class TestAppliedFilter(unittest.TestCase):
-    """AppliedFilter unit test stubs"""
+class TestFilterOption(unittest.TestCase):
+    """FilterOption unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> AppliedFilter:
-        """Test AppliedFilter
+    def make_instance(self, include_optional) -> FilterOption:
+        """Test FilterOption
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `AppliedFilter`
+        # uncomment below to create an instance of `FilterOption`
         """
-        model = AppliedFilter()
+        model = FilterOption()
         if include_optional:
-            return AppliedFilter(
-                type = 'FULL_TEXT',
-                filter_option_id = '',
-                match = '',
-                mode = 'STRICT'
+            return FilterOption(
+                id = '',
+                filter_id = '',
+                name = '',
+                count = 56
             )
         else:
-            return AppliedFilter(
+            return FilterOption(
         )
         """
 
-    def testAppliedFilter(self):
-        """Test AppliedFilter"""
+    def testFilterOption(self):
+        """Test FilterOption"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_attribute_validation_summary.py` & `odm_api-1.57.0/test/test_attribute_validation_summary.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_create_group201_response.py` & `odm_api-1.57.0/test/test_create_group201_response_all_of_meta.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,53 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.create_group201_response import CreateGroup201Response
+from odm_api.models.create_group201_response_all_of_meta import CreateGroup201ResponseAllOfMeta
 
-class TestCreateGroup201Response(unittest.TestCase):
-    """CreateGroup201Response unit test stubs"""
+class TestCreateGroup201ResponseAllOfMeta(unittest.TestCase):
+    """CreateGroup201ResponseAllOfMeta unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateGroup201Response:
-        """Test CreateGroup201Response
+    def make_instance(self, include_optional) -> CreateGroup201ResponseAllOfMeta:
+        """Test CreateGroup201ResponseAllOfMeta
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateGroup201Response`
+        # uncomment below to create an instance of `CreateGroup201ResponseAllOfMeta`
         """
-        model = CreateGroup201Response()
+        model = CreateGroup201ResponseAllOfMeta()
         if include_optional:
-            return CreateGroup201Response(
-                external_id = '',
-                id = '',
-                schemas = [
-                    'urn:ietf:params:scim:schemas:core:2.0:Group'
-                    ],
-                members = [
-                    {display=display, value=value, $ref=https://openapi-generator.tech}
-                    ],
-                display_name = '',
-                meta = odm_api.models.create_user_201_response_all_of_meta.createUser_201_response_allOf_meta(
-                    created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    last_modified = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    resource_type = 'User', )
+            return CreateGroup201ResponseAllOfMeta(
+                created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                last_modified = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                resource_type = 'User'
             )
         else:
-            return CreateGroup201Response(
-                display_name = '',
+            return CreateGroup201ResponseAllOfMeta(
         )
         """
 
-    def testCreateGroup201Response(self):
-        """Test CreateGroup201Response"""
+    def testCreateGroup201ResponseAllOfMeta(self):
+        """Test CreateGroup201ResponseAllOfMeta"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_create_group_request.py` & `odm_api-1.57.0/test/test_filter_option_group.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,60 +1,55 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.create_group_request import CreateGroupRequest
+from odm_api.models.filter_option_group import FilterOptionGroup
 
-class TestCreateGroupRequest(unittest.TestCase):
-    """CreateGroupRequest unit test stubs"""
+class TestFilterOptionGroup(unittest.TestCase):
+    """FilterOptionGroup unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateGroupRequest:
-        """Test CreateGroupRequest
+    def make_instance(self, include_optional) -> FilterOptionGroup:
+        """Test FilterOptionGroup
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateGroupRequest`
+        # uncomment below to create an instance of `FilterOptionGroup`
         """
-        model = CreateGroupRequest()
+        model = FilterOptionGroup()
         if include_optional:
-            return CreateGroupRequest(
-                external_id = '',
-                id = '',
-                schemas = [
-                    'urn:ietf:params:scim:schemas:core:2.0:Group'
-                    ],
-                members = [
-                    {display=display, value=value, $ref=https://openapi-generator.tech}
-                    ],
-                display_name = ''
+            return FilterOptionGroup(
+                filter_id = '',
+                has_more_options = True,
+                options = [
+                    {filterId=filterId, name=name, count=5, id=id}
+                    ]
             )
         else:
-            return CreateGroupRequest(
-                display_name = '',
+            return FilterOptionGroup(
         )
         """
 
-    def testCreateGroupRequest(self):
-        """Test CreateGroupRequest"""
+    def testFilterOptionGroup(self):
+        """Test FilterOptionGroup"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_create_user201_response.py` & `odm_api-1.57.0/test/test_list_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,54 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.create_user201_response import CreateUser201Response
+from odm_api.models.list_response import ListResponse
 
-class TestCreateUser201Response(unittest.TestCase):
-    """CreateUser201Response unit test stubs"""
+class TestListResponse(unittest.TestCase):
+    """ListResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateUser201Response:
-        """Test CreateUser201Response
+    def make_instance(self, include_optional) -> ListResponse:
+        """Test ListResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateUser201Response`
+        # uncomment below to create an instance of `ListResponse`
         """
-        model = CreateUser201Response()
+        model = ListResponse()
         if include_optional:
-            return CreateUser201Response(
-                active = True,
-                emails = [
-                    {type=work, value=value, primary=true}
-                    ],
-                external_id = '',
-                id = '',
-                schemas = [
-                    'urn:ietf:params:scim:schemas:core:2.0:User'
-                    ],
-                user_name = '',
-                display_name = '',
-                meta = odm_api.models.create_user_201_response_all_of_meta.createUser_201_response_allOf_meta(
-                    created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    last_modified = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    resource_type = 'User', )
+            return ListResponse(
+                meta = {pagination={total=6, offset=1, count=0, limit=5}},
+                data = [
+                    None
+                    ]
             )
         else:
-            return CreateUser201Response(
-                active = True,
-                emails = [
-                    {type=work, value=value, primary=true}
-                    ],
-                display_name = '',
+            return ListResponse(
         )
         """
 
-    def testCreateUser201Response(self):
-        """Test CreateUser201Response"""
+    def testListResponse(self):
+        """Test ListResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_create_user_request.py` & `odm_api-1.57.0/test/test_create_group_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,60 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.create_user_request import CreateUserRequest
+from odm_api.models.create_group_request import CreateGroupRequest
 
-class TestCreateUserRequest(unittest.TestCase):
-    """CreateUserRequest unit test stubs"""
+class TestCreateGroupRequest(unittest.TestCase):
+    """CreateGroupRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> CreateUserRequest:
-        """Test CreateUserRequest
+    def make_instance(self, include_optional) -> CreateGroupRequest:
+        """Test CreateGroupRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `CreateUserRequest`
+        # uncomment below to create an instance of `CreateGroupRequest`
         """
-        model = CreateUserRequest()
+        model = CreateGroupRequest()
         if include_optional:
-            return CreateUserRequest(
-                active = True,
-                emails = [
-                    {type=work, value=value, primary=true}
-                    ],
+            return CreateGroupRequest(
                 external_id = '',
                 id = '',
                 schemas = [
-                    'urn:ietf:params:scim:schemas:core:2.0:User'
+                    'urn:ietf:params:scim:schemas:core:2.0:Group'
+                    ],
+                members = [
+                    {display=display, value=value}
                     ],
-                user_name = '',
                 display_name = ''
             )
         else:
-            return CreateUserRequest(
-                active = True,
-                emails = [
-                    {type=work, value=value, primary=true}
-                    ],
+            return CreateGroupRequest(
                 display_name = '',
         )
         """
 
-    def testCreateUserRequest(self):
-        """Test CreateUserRequest"""
+    def testCreateGroupRequest(self):
+        """Test CreateGroupRequest"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_data_presentation.py` & `odm_api-1.57.0/test/test_group_patch_operations_inner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,54 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.data_presentation import DataPresentation
+from odm_api.models.group_patch_operations_inner import GroupPatchOperationsInner
 
-class TestDataPresentation(unittest.TestCase):
-    """DataPresentation unit test stubs"""
+class TestGroupPatchOperationsInner(unittest.TestCase):
+    """GroupPatchOperationsInner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> DataPresentation:
-        """Test DataPresentation
+    def make_instance(self, include_optional) -> GroupPatchOperationsInner:
+        """Test GroupPatchOperationsInner
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `DataPresentation`
+        # uncomment below to create an instance of `GroupPatchOperationsInner`
         """
-        model = DataPresentation()
+        model = GroupPatchOperationsInner()
         if include_optional:
-            return DataPresentation(
-                item_id = '',
-                metadata = None,
-                relationships = odm_api.models.data_presentation_relationships.DataPresentation_relationships(
-                    sample = '', 
-                    cell = '', 
-                    library = '', 
-                    preparation = '', )
+            return GroupPatchOperationsInner(
+                op = 'add',
+                path = '',
+                value = None
             )
         else:
-            return DataPresentation(
+            return GroupPatchOperationsInner(
+                op = 'add',
         )
         """
 
-    def testDataPresentation(self):
-        """Test DataPresentation"""
+    def testGroupPatchOperationsInner(self):
+        """Test GroupPatchOperationsInner"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_data_presentation_relationships.py` & `odm_api-1.57.0/test/test_data_presentation_relationships.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_detached_collection.py` & `odm_api-1.57.0/test/test_detached_collection.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_detached_collection_data_inner.py` & `odm_api-1.57.0/test/test_detached_collection_data_inner.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_detached_object.py` & `odm_api-1.57.0/test/test_detached_object.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_email.py` & `odm_api-1.57.0/test/test_group_response_all_of_members.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.email import Email
+from odm_api.models.group_response_all_of_members import GroupResponseAllOfMembers
 
-class TestEmail(unittest.TestCase):
-    """Email unit test stubs"""
+class TestGroupResponseAllOfMembers(unittest.TestCase):
+    """GroupResponseAllOfMembers unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Email:
-        """Test Email
+    def make_instance(self, include_optional) -> GroupResponseAllOfMembers:
+        """Test GroupResponseAllOfMembers
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Email`
+        # uncomment below to create an instance of `GroupResponseAllOfMembers`
         """
-        model = Email()
+        model = GroupResponseAllOfMembers()
         if include_optional:
-            return Email(
-                type = 'work',
+            return GroupResponseAllOfMembers(
                 value = '',
-                primary = True
+                display = '',
+                ref = ''
             )
         else:
-            return Email(
+            return GroupResponseAllOfMembers(
+                value = '',
+                ref = '',
         )
         """
 
-    def testEmail(self):
-        """Test Email"""
+    def testGroupResponseAllOfMembers(self):
+        """Test GroupResponseAllOfMembers"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_exception_type_and_message.py` & `odm_api-1.57.0/test/test_exception_type_and_message.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_expression_integration_as_curator_api.py` & `odm_api-1.57.0/test/test_expression_integration_as_curator_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_expression_integration_as_user_api.py` & `odm_api-1.57.0/test/test_expression_spo_tas_user_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,87 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.api.expression_integration_as_user_api import ExpressionIntegrationAsUserApi
+from odm_api.api.expression_spo_tas_user_api import ExpressionSPoTAsUserApi
 
 
-class TestExpressionIntegrationAsUserApi(unittest.TestCase):
-    """ExpressionIntegrationAsUserApi unit test stubs"""
+class TestExpressionSPoTAsUserApi(unittest.TestCase):
+    """ExpressionSPoTAsUserApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = ExpressionIntegrationAsUserApi()
+        self.api = ExpressionSPoTAsUserApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_get_expression_by_library_as_user(self) -> None:
-        """Test case for get_expression_by_library_as_user
+    def test_get_expression_as_user(self) -> None:
+        """Test case for get_expression_as_user
 
-        Retrieve expression run-level data by querying related library ID (accession)
+        Retrieve a single expression object by ID (accession)
         """
         pass
 
-    def test_get_expression_by_preparation_as_user(self) -> None:
-        """Test case for get_expression_by_preparation_as_user
+    def test_get_expression_by_version_as_user(self) -> None:
+        """Test case for get_expression_by_version_as_user
 
-        Retrieve expression run-level data by querying related preparation ID (accession)
+        Retrieve a single expression object by ID (accession)
         """
         pass
 
-    def test_get_expression_by_sample_as_user(self) -> None:
-        """Test case for get_expression_by_sample_as_user
+    def test_get_expression_data_as_user(self) -> None:
+        """Test case for get_expression_data_as_user
 
-        Retrieve expression run-level data by querying related sample ID (accession)
+        Retrieve multiple expression data and metadata objects
         """
         pass
 
-    def test_get_expression_groups_by_study_as_user(self) -> None:
-        """Test case for get_expression_groups_by_study_as_user
+    def test_get_expression_group_as_user(self) -> None:
+        """Test case for get_expression_group_as_user
 
-        Retrieve group metadata by querying study ID (accession)
+        Retrieve a single group object by ID (accession)
         """
         pass
 
-    def test_get_expression_run_to_library_pairs_as_user(self) -> None:
-        """Test case for get_expression_run_to_library_pairs_as_user
+    def test_get_expression_group_by_run_as_user(self) -> None:
+        """Test case for get_expression_group_by_run_as_user
 
-        Retrieve run-library pairs by group id. Pagination is based on unique runs, not unique pairs.
+        Retrieve a single group object by run ID (accession)
         """
         pass
 
-    def test_get_expression_run_to_preparation_pairs_as_user(self) -> None:
-        """Test case for get_expression_run_to_preparation_pairs_as_user
+    def test_get_expression_versions_as_user(self) -> None:
+        """Test case for get_expression_versions_as_user
 
-        Retrieve run-preparation pairs by group id. Pagination is based on unique runs, not unique pairs.
+        Retrieve a list of object versions by ID
         """
         pass
 
-    def test_get_expression_run_to_sample_pairs_as_user(self) -> None:
-        """Test case for get_expression_run_to_sample_pairs_as_user
+    def test_search_expression_groups_as_user(self) -> None:
+        """Test case for search_expression_groups_as_user
 
-        Retrieve run-sample pairs by group id. Pagination is based on unique runs, not unique pairs.
+        Retrieve groups that match a query
+        """
+        pass
+
+    def test_search_expression_runs_as_user(self) -> None:
+        """Test case for search_expression_runs_as_user
+
+        Retrieve run objects related to the given group
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_expression_spo_tas_curator_api.py` & `odm_api-1.57.0/test/test_expression_integration_as_user_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,80 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.api.expression_spo_tas_curator_api import ExpressionSPoTAsCuratorApi
+from odm_api.api.expression_integration_as_user_api import ExpressionIntegrationAsUserApi
 
 
-class TestExpressionSPoTAsCuratorApi(unittest.TestCase):
-    """ExpressionSPoTAsCuratorApi unit test stubs"""
+class TestExpressionIntegrationAsUserApi(unittest.TestCase):
+    """ExpressionIntegrationAsUserApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = ExpressionSPoTAsCuratorApi()
+        self.api = ExpressionIntegrationAsUserApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_add_expression_as_curator(self) -> None:
-        """Test case for add_expression_as_curator
+    def test_get_expression_by_library_as_user(self) -> None:
+        """Test case for get_expression_by_library_as_user
 
-        Create multiple new objects from a multi-row data file with optional supplied metadata
+        Retrieve expression run-level data by querying related library ID (accession)
         """
         pass
 
-    def test_delete_expression_group_as_curator(self) -> None:
-        """Test case for delete_expression_group_as_curator
+    def test_get_expression_by_preparation_as_user(self) -> None:
+        """Test case for get_expression_by_preparation_as_user
 
-        Delete the object
+        Retrieve expression run-level data by querying related preparation ID (accession)
         """
         pass
 
-    def test_get_expression_as_curator(self) -> None:
-        """Test case for get_expression_as_curator
+    def test_get_expression_by_sample_as_user(self) -> None:
+        """Test case for get_expression_by_sample_as_user
 
-        Retrieve a single expression object by ID (accession)
+        Retrieve expression run-level data by querying related sample ID (accession)
         """
         pass
 
-    def test_get_expression_by_version_as_curator(self) -> None:
-        """Test case for get_expression_by_version_as_curator
+    def test_get_expression_groups_by_study_as_user(self) -> None:
+        """Test case for get_expression_groups_by_study_as_user
 
-        Retrieve a single expression object by ID (accession)
+        Retrieve group metadata by querying study ID (accession)
         """
         pass
 
-    def test_get_expression_data_as_curator(self) -> None:
-        """Test case for get_expression_data_as_curator
+    def test_get_expression_run_to_library_pairs_as_user(self) -> None:
+        """Test case for get_expression_run_to_library_pairs_as_user
 
-        Retrieve multiple expression data and metadata objects
+        Retrieve run-library pairs by group id. Pagination is based on unique runs, not unique pairs.
         """
         pass
 
-    def test_get_expression_group_as_curator(self) -> None:
-        """Test case for get_expression_group_as_curator
+    def test_get_expression_run_to_preparation_pairs_as_user(self) -> None:
+        """Test case for get_expression_run_to_preparation_pairs_as_user
 
-        Retrieve a single group object by ID (accession)
+        Retrieve run-preparation pairs by group id. Pagination is based on unique runs, not unique pairs.
         """
         pass
 
-    def test_get_expression_group_by_run_as_curator(self) -> None:
-        """Test case for get_expression_group_by_run_as_curator
+    def test_get_expression_run_to_sample_pairs_as_user(self) -> None:
+        """Test case for get_expression_run_to_sample_pairs_as_user
 
-        Retrieve a single group object by run ID (accession)
-        """
-        pass
-
-    def test_get_expression_versions_as_curator(self) -> None:
-        """Test case for get_expression_versions_as_curator
-
-        Retrieve a list of object versions by ID
-        """
-        pass
-
-    def test_search_expression_groups_as_curator(self) -> None:
-        """Test case for search_expression_groups_as_curator
-
-        Retrieve groups that match a query
-        """
-        pass
-
-    def test_search_expression_runs_as_curator(self) -> None:
-        """Test case for search_expression_runs_as_curator
-
-        Retrieve run objects related to the given group
-        """
-        pass
-
-    def test_update_expression_run_as_curator(self) -> None:
-        """Test case for update_expression_run_as_curator
-
-        Update object metadata
+        Retrieve run-sample pairs by group id. Pagination is based on unique runs, not unique pairs.
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_expression_spo_tas_user_api.py` & `odm_api-1.57.0/test/test_flow_cytometry_spo_tas_user_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,86 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.api.expression_spo_tas_user_api import ExpressionSPoTAsUserApi
+from odm_api.api.flow_cytometry_spo_tas_user_api import FlowCytometrySPoTAsUserApi
 
 
-class TestExpressionSPoTAsUserApi(unittest.TestCase):
-    """ExpressionSPoTAsUserApi unit test stubs"""
+class TestFlowCytometrySPoTAsUserApi(unittest.TestCase):
+    """FlowCytometrySPoTAsUserApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = ExpressionSPoTAsUserApi()
+        self.api = FlowCytometrySPoTAsUserApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_get_expression_as_user(self) -> None:
-        """Test case for get_expression_as_user
+    def test_get_flow_cytometry_as_user(self) -> None:
+        """Test case for get_flow_cytometry_as_user
 
-        Retrieve a single expression object by ID (accession)
+        Retrieve a single sample flow cytometry by ID (accession)
         """
         pass
 
-    def test_get_expression_by_version_as_user(self) -> None:
-        """Test case for get_expression_by_version_as_user
+    def test_get_flow_cytometry_by_version_as_user(self) -> None:
+        """Test case for get_flow_cytometry_by_version_as_user
 
-        Retrieve a single expression object by ID (accession)
+        Retrieve a single sample flow cytometry by ID (accession)
         """
         pass
 
-    def test_get_expression_data_as_user(self) -> None:
-        """Test case for get_expression_data_as_user
+    def test_get_flow_cytometry_data_as_user(self) -> None:
+        """Test case for get_flow_cytometry_data_as_user
 
-        Retrieve multiple expression data and metadata objects
+        Retrieve multiple flow cytometry data and metadata objects
         """
         pass
 
-    def test_get_expression_group_as_user(self) -> None:
-        """Test case for get_expression_group_as_user
+    def test_get_flow_cytometry_group_as_user(self) -> None:
+        """Test case for get_flow_cytometry_group_as_user
 
         Retrieve a single group object by ID (accession)
         """
         pass
 
-    def test_get_expression_group_by_run_as_user(self) -> None:
-        """Test case for get_expression_group_by_run_as_user
+    def test_get_flow_cytometry_group_by_run_as_user(self) -> None:
+        """Test case for get_flow_cytometry_group_by_run_as_user
 
         Retrieve a single group object by run ID (accession)
         """
         pass
 
-    def test_get_expression_versions_as_user(self) -> None:
-        """Test case for get_expression_versions_as_user
+    def test_get_flow_cytometry_versions_as_user(self) -> None:
+        """Test case for get_flow_cytometry_versions_as_user
 
         Retrieve a list of object versions by ID
         """
         pass
 
-    def test_search_expression_groups_as_user(self) -> None:
-        """Test case for search_expression_groups_as_user
+    def test_search_flow_cytometry_groups_as_user(self) -> None:
+        """Test case for search_flow_cytometry_groups_as_user
 
         Retrieve groups that match a query
         """
         pass
 
-    def test_search_expression_runs_as_user(self) -> None:
-        """Test case for search_expression_runs_as_user
+    def test_search_flow_cytometry_runs_as_user(self) -> None:
+        """Test case for search_flow_cytometry_runs_as_user
 
         Retrieve run objects related to the given group
         """
         pass
 
 
 if __name__ == '__main__':
```

### Comparing `odm-api-0.0.1/test/test_filter_option.py` & `odm_api-1.57.0/test/test_expression_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.filter_option import FilterOption
+from odm_api.models.expression_response import ExpressionResponse
 
-class TestFilterOption(unittest.TestCase):
-    """FilterOption unit test stubs"""
+class TestExpressionResponse(unittest.TestCase):
+    """ExpressionResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> FilterOption:
-        """Test FilterOption
+    def make_instance(self, include_optional) -> ExpressionResponse:
+        """Test ExpressionResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `FilterOption`
+        # uncomment below to create an instance of `ExpressionResponse`
         """
-        model = FilterOption()
+        model = ExpressionResponse()
         if include_optional:
-            return FilterOption(
-                id = '',
-                filter_id = '',
-                name = '',
-                count = 56
+            return ExpressionResponse(
+                data = [
+                    {itemId=itemId, metadata={}, expression=1.82, feature={genes=MYO9A,, groupingKey=VRSLGGISPSEDRR}, gene=gene, groupId=groupId, description=description, runId=runId, value={expression=1.82}}
+                    ],
+                cursor = ''
             )
         else:
-            return FilterOption(
+            return ExpressionResponse(
         )
         """
 
-    def testFilterOption(self):
-        """Test FilterOption"""
+    def testExpressionResponse(self):
+        """Test ExpressionResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_filter_option_group.py` & `odm_api-1.57.0/test/test_search_study_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,52 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.filter_option_group import FilterOptionGroup
+from odm_api.models.search_study_request import SearchStudyRequest
 
-class TestFilterOptionGroup(unittest.TestCase):
-    """FilterOptionGroup unit test stubs"""
+class TestSearchStudyRequest(unittest.TestCase):
+    """SearchStudyRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> FilterOptionGroup:
-        """Test FilterOptionGroup
+    def make_instance(self, include_optional) -> SearchStudyRequest:
+        """Test SearchStudyRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `FilterOptionGroup`
+        # uncomment below to create an instance of `SearchStudyRequest`
         """
-        model = FilterOptionGroup()
+        model = SearchStudyRequest()
         if include_optional:
-            return FilterOptionGroup(
-                filter_id = '',
-                has_more_options = True,
-                options = [
-                    {filterId=filterId, name=name, count=5, id=id}
-                    ]
+            return SearchStudyRequest(
+                filters = [{type=FULL_TEXT, match=text_to_search, mode=STRICT}, {type=SELECT, filterOptionId=TUVUQURBVEFfU3R1ZHlfU291cmNlOlRlc3QgR0VP}],
+                page = {offset=6, limit=50}
             )
         else:
-            return FilterOptionGroup(
+            return SearchStudyRequest(
         )
         """
 
-    def testFilterOptionGroup(self):
-        """Test FilterOptionGroup"""
+    def testSearchStudyRequest(self):
+        """Test SearchStudyRequest"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_filter_users_response.py` & `odm_api-1.57.0/test/test_xref_set_metadata.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.filter_users_response import FilterUsersResponse
+from odm_api.models.xref_set_metadata import XrefSetMetadata
 
-class TestFilterUsersResponse(unittest.TestCase):
-    """FilterUsersResponse unit test stubs"""
+class TestXrefSetMetadata(unittest.TestCase):
+    """XrefSetMetadata unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> FilterUsersResponse:
-        """Test FilterUsersResponse
+    def make_instance(self, include_optional) -> XrefSetMetadata:
+        """Test XrefSetMetadata
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `FilterUsersResponse`
+        # uncomment below to create an instance of `XrefSetMetadata`
         """
-        model = FilterUsersResponse()
+        model = XrefSetMetadata()
         if include_optional:
-            return FilterUsersResponse(
-                resources = [
-                    null
-                    ],
-                items_per_page = 56,
-                schemas = [
-                    'urn:ietf:params:scim:api:messages:2.0:ListResponse'
-                    ],
-                start_index = 56,
-                total_results = 56
+            return XrefSetMetadata(
+                xref_set_id = '"GSF000477"',
+                created_by = '"Genestack Superuser"',
+                created_date = 1594846270242,
+                last_updated = 1594846270242,
+                data = None
             )
         else:
-            return FilterUsersResponse(
+            return XrefSetMetadata(
         )
         """
 
-    def testFilterUsersResponse(self):
-        """Test FilterUsersResponse"""
+    def testXrefSetMetadata(self):
+        """Test XrefSetMetadata"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_find_objects_response.py` & `odm_api-1.57.0/test/test_find_objects_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_find_objects_response_filter_option_groups_inner_options_inner.py` & `odm_api-1.57.0/test/test_find_objects_response_filter_option_groups_inner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.find_objects_response_filter_option_groups_inner_options_inner import FindObjectsResponseFilterOptionGroupsInnerOptionsInner
+from odm_api.models.find_objects_response_filter_option_groups_inner import FindObjectsResponseFilterOptionGroupsInner
 
-class TestFindObjectsResponseFilterOptionGroupsInnerOptionsInner(unittest.TestCase):
-    """FindObjectsResponseFilterOptionGroupsInnerOptionsInner unit test stubs"""
+class TestFindObjectsResponseFilterOptionGroupsInner(unittest.TestCase):
+    """FindObjectsResponseFilterOptionGroupsInner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> FindObjectsResponseFilterOptionGroupsInnerOptionsInner:
-        """Test FindObjectsResponseFilterOptionGroupsInnerOptionsInner
+    def make_instance(self, include_optional) -> FindObjectsResponseFilterOptionGroupsInner:
+        """Test FindObjectsResponseFilterOptionGroupsInner
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `FindObjectsResponseFilterOptionGroupsInnerOptionsInner`
+        # uncomment below to create an instance of `FindObjectsResponseFilterOptionGroupsInner`
         """
-        model = FindObjectsResponseFilterOptionGroupsInnerOptionsInner()
+        model = FindObjectsResponseFilterOptionGroupsInner()
         if include_optional:
-            return FindObjectsResponseFilterOptionGroupsInnerOptionsInner(
-                id = '',
+            return FindObjectsResponseFilterOptionGroupsInner(
                 filter_id = '',
-                name = '',
-                count = 56
+                has_more_options = True,
+                options = [
+                    {filterId=filterId, name=name, count=5, id=id}
+                    ]
             )
         else:
-            return FindObjectsResponseFilterOptionGroupsInnerOptionsInner(
+            return FindObjectsResponseFilterOptionGroupsInner(
         )
         """
 
-    def testFindObjectsResponseFilterOptionGroupsInnerOptionsInner(self):
-        """Test FindObjectsResponseFilterOptionGroupsInnerOptionsInner"""
+    def testFindObjectsResponseFilterOptionGroupsInner(self):
+        """Test FindObjectsResponseFilterOptionGroupsInner"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_flow_cytometry_item.py` & `odm_api-1.57.0/test/test_flow_cytometry_item.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_get_expression_as_user200_response.py` & `odm_api-1.57.0/test/test_expression_item.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.get_expression_as_user200_response import GetExpressionAsUser200Response
+from odm_api.models.expression_item import ExpressionItem
 
-class TestGetExpressionAsUser200Response(unittest.TestCase):
-    """GetExpressionAsUser200Response unit test stubs"""
+class TestExpressionItem(unittest.TestCase):
+    """ExpressionItem unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> GetExpressionAsUser200Response:
-        """Test GetExpressionAsUser200Response
+    def make_instance(self, include_optional) -> ExpressionItem:
+        """Test ExpressionItem
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `GetExpressionAsUser200Response`
+        # uncomment below to create an instance of `ExpressionItem`
         """
-        model = GetExpressionAsUser200Response()
+        model = ExpressionItem()
         if include_optional:
-            return GetExpressionAsUser200Response(
+            return ExpressionItem(
                 item_id = '',
                 metadata = None,
                 run_id = '',
                 group_id = '',
                 gene = '',
                 expression = 1.82,
                 feature = {genes=MYO9A,, groupingKey=VRSLGGISPSEDRR},
                 value = {expression=1.82},
                 description = ''
             )
         else:
-            return GetExpressionAsUser200Response(
+            return ExpressionItem(
         )
         """
 
-    def testGetExpressionAsUser200Response(self):
-        """Test GetExpressionAsUser200Response"""
+    def testExpressionItem(self):
+        """Test ExpressionItem"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_group_response.py` & `odm_api-1.57.0/test/test_user_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,70 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.group_response import GroupResponse
+from odm_api.models.user_response import UserResponse
 
-class TestGroupResponse(unittest.TestCase):
-    """GroupResponse unit test stubs"""
+class TestUserResponse(unittest.TestCase):
+    """UserResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> GroupResponse:
-        """Test GroupResponse
+    def make_instance(self, include_optional) -> UserResponse:
+        """Test UserResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `GroupResponse`
+        # uncomment below to create an instance of `UserResponse`
         """
-        model = GroupResponse()
+        model = UserResponse()
         if include_optional:
-            return GroupResponse(
+            return UserResponse(
+                active = True,
+                emails = [
+                    {type=work, value=value, primary=true}
+                    ],
                 external_id = '',
                 id = '',
                 schemas = [
-                    'urn:ietf:params:scim:schemas:core:2.0:Group'
-                    ],
-                members = [
-                    {display=display, value=value, $ref=https://openapi-generator.tech}
+                    'urn:ietf:params:scim:schemas:core:2.0:User'
                     ],
+                user_name = '',
                 display_name = '',
-                meta = odm_api.models.create_user_201_response_all_of_meta.createUser_201_response_allOf_meta(
+                meta = odm_api.models.create_group_201_response_all_of_meta.createGroup_201_response_allOf_meta(
                     created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     last_modified = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     resource_type = 'User', )
             )
         else:
-            return GroupResponse(
+            return UserResponse(
+                active = True,
+                emails = [
+                    {type=work, value=value, primary=true}
+                    ],
                 display_name = '',
         )
         """
 
-    def testGroupResponse(self):
-        """Test GroupResponse"""
+    def testUserResponse(self):
+        """Test UserResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_group_validation_summary.py` & `odm_api-1.57.0/test/test_study_validation_summary.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.group_validation_summary import GroupValidationSummary
+from odm_api.models.study_validation_summary import StudyValidationSummary
 
-class TestGroupValidationSummary(unittest.TestCase):
-    """GroupValidationSummary unit test stubs"""
+class TestStudyValidationSummary(unittest.TestCase):
+    """StudyValidationSummary unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> GroupValidationSummary:
-        """Test GroupValidationSummary
+    def make_instance(self, include_optional) -> StudyValidationSummary:
+        """Test StudyValidationSummary
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `GroupValidationSummary`
+        # uncomment below to create an instance of `StudyValidationSummary`
         """
-        model = GroupValidationSummary()
+        model = StudyValidationSummary()
         if include_optional:
-            return GroupValidationSummary(
-                group_accession = '',
-                attributes = [
-                    {attributeName=attributeName, attributeInvalidValues=[{count=0, value={}, errors=[{errorType=VALUE_NOT_SET, errorMessage=errorMessage}, {errorType=VALUE_NOT_SET, errorMessage=errorMessage}]}, {count=0, value={}, errors=[{errorType=VALUE_NOT_SET, errorMessage=errorMessage}, {errorType=VALUE_NOT_SET, errorMessage=errorMessage}]}]}
+            return StudyValidationSummary(
+                samples = [
+                    {groupAccession=groupAccession, attributes=[{attributeName=attributeName, attributeInvalidValues=[{count=0, value={}, errors=[{errorType=VALUE_NOT_SET, errorMessage=errorMessage}, {errorType=VALUE_NOT_SET, errorMessage=errorMessage}]}, {count=0, value={}, errors=[{errorType=VALUE_NOT_SET, errorMessage=errorMessage}, {errorType=VALUE_NOT_SET, errorMessage=errorMessage}]}]}, {attributeName=attributeName, attributeInvalidValues=[{count=0, value={}, errors=[{errorType=VALUE_NOT_SET, errorMessage=errorMessage}, {errorType=VALUE_NOT_SET, errorMessage=errorMessage}]}, {count=0, value={}, errors=[{errorType=VALUE_NOT_SET, errorMessage=errorMessage}, {errorType=VALUE_NOT_SET, errorMessage=errorMessage}]}]}]}
                     ]
             )
         else:
-            return GroupValidationSummary(
+            return StudyValidationSummary(
         )
         """
 
-    def testGroupValidationSummary(self):
-        """Test GroupValidationSummary"""
+    def testStudyValidationSummary(self):
+        """Test StudyValidationSummary"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_i_metadata.py` & `odm_api-1.57.0/test/test_patch_operation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,54 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.i_metadata import IMetadata
+from odm_api.models.patch_operation import PatchOperation
 
-class TestIMetadata(unittest.TestCase):
-    """IMetadata unit test stubs"""
+class TestPatchOperation(unittest.TestCase):
+    """PatchOperation unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> IMetadata:
-        """Test IMetadata
+    def make_instance(self, include_optional) -> PatchOperation:
+        """Test PatchOperation
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `IMetadata`
+        # uncomment below to create an instance of `PatchOperation`
         """
-        model = IMetadata()
+        model = PatchOperation()
         if include_optional:
-            return IMetadata(
-                source = '',
-                name = '',
-                public = True,
-                id = '',
-                content = None,
-                data_type = '',
-                content_map = {
-                    'key' : None
-                    },
-                metadata_content = {
-                    'key' : None
-                    },
-                file_id_associated_with_template = ''
+            return PatchOperation(
+                op = 'add',
+                path = '',
+                value = None
             )
         else:
-            return IMetadata(
+            return PatchOperation(
+                op = 'add',
         )
         """
 
-    def testIMetadata(self):
-        """Test IMetadata"""
+    def testPatchOperation(self):
+        """Test PatchOperation"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_info.py` & `odm_api-1.57.0/test/test_meta.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,53 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.info import Info
+from odm_api.models.meta import Meta
 
-class TestInfo(unittest.TestCase):
-    """Info unit test stubs"""
+class TestMeta(unittest.TestCase):
+    """Meta unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Info:
-        """Test Info
+    def make_instance(self, include_optional) -> Meta:
+        """Test Meta
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Info`
+        # uncomment below to create an instance of `Meta`
         """
-        model = Info()
+        model = Meta()
         if include_optional:
-            return Info(
-                job_exec_id = 12345,
-                started_by = 'job@genestack.com',
-                job_name = 'Protein folding',
-                status = 'STARTED',
-                create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                end_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
+            return Meta(
+                created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                last_modified = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                resource_type = 'User'
             )
         else:
-            return Info(
-                job_exec_id = 12345,
-                started_by = 'job@genestack.com',
-                job_name = 'Protein folding',
-                status = 'STARTED',
-                create_time = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+            return Meta(
         )
         """
 
-    def testInfo(self):
-        """Test Info"""
+    def testMeta(self):
+        """Test Meta"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_library_spo_tas_curator_api.py` & `odm_api-1.57.0/test/test_library_spo_tas_curator_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_library_spo_tas_user_api.py` & `odm_api-1.57.0/test/test_variant_spo_tas_user_api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,87 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.api.library_spo_tas_user_api import LibrarySPoTAsUserApi
+from odm_api.api.variant_spo_tas_user_api import VariantSPoTAsUserApi
 
 
-class TestLibrarySPoTAsUserApi(unittest.TestCase):
-    """LibrarySPoTAsUserApi unit test stubs"""
+class TestVariantSPoTAsUserApi(unittest.TestCase):
+    """VariantSPoTAsUserApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = LibrarySPoTAsUserApi()
+        self.api = VariantSPoTAsUserApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_get_libraries_by_group_as_user(self) -> None:
-        """Test case for get_libraries_by_group_as_user
+    def test_get_all_variants_as_user(self) -> None:
+        """Test case for get_all_variants_as_user
 
-        Retrieve libraries related to the given group
+        Retrieve multiple variant data and metadata objects
         """
         pass
 
-    def test_get_library_as_user(self) -> None:
-        """Test case for get_library_as_user
+    def test_get_variant_as_user(self) -> None:
+        """Test case for get_variant_as_user
 
-        Retrieve a single library object by ID (accession)
+        Retrieve a single variant object by ID (accession)
         """
         pass
 
-    def test_get_library_by_version_as_user(self) -> None:
-        """Test case for get_library_by_version_as_user
+    def test_get_variant_by_version_as_user(self) -> None:
+        """Test case for get_variant_by_version_as_user
 
-        Retrieve a single library object by ID (accession)
+        Retrieve a single variant object by ID (accession)
         """
         pass
 
-    def test_get_library_versions_as_user(self) -> None:
-        """Test case for get_library_versions_as_user
+    def test_get_variant_group_as_user(self) -> None:
+        """Test case for get_variant_group_as_user
+
+        Retrieve a single group object by ID (accession)
+        """
+        pass
+
+    def test_get_variant_group_by_run_as_user(self) -> None:
+        """Test case for get_variant_group_by_run_as_user
+
+        Retrieve a single group object by run ID (accession)
+        """
+        pass
+
+    def test_get_variant_versions_as_user(self) -> None:
+        """Test case for get_variant_versions_as_user
 
         Retrieve a list of object versions by ID
         """
         pass
 
-    def test_search_libraries_as_user(self) -> None:
-        """Test case for search_libraries_as_user
+    def test_search_variant_groups_as_user(self) -> None:
+        """Test case for search_variant_groups_as_user
+
+        Retrieve groups that match a query
+        """
+        pass
+
+    def test_search_variant_runs_as_user(self) -> None:
+        """Test case for search_variant_runs_as_user
 
-        List or search for library metadata objects
+        Retrieve run objects related to the given group
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_list_response_meta.py` & `odm_api-1.57.0/test/test_list_response_meta_pagination.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.list_response_meta import ListResponseMeta
+from odm_api.models.list_response_meta_pagination import ListResponseMetaPagination
 
-class TestListResponseMeta(unittest.TestCase):
-    """ListResponseMeta unit test stubs"""
+class TestListResponseMetaPagination(unittest.TestCase):
+    """ListResponseMetaPagination unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> ListResponseMeta:
-        """Test ListResponseMeta
+    def make_instance(self, include_optional) -> ListResponseMetaPagination:
+        """Test ListResponseMetaPagination
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `ListResponseMeta`
+        # uncomment below to create an instance of `ListResponseMetaPagination`
         """
-        model = ListResponseMeta()
+        model = ListResponseMetaPagination()
         if include_optional:
-            return ListResponseMeta(
-                pagination = {total=6, offset=1, count=0, limit=5}
+            return ListResponseMetaPagination(
+                count = 56,
+                total = 56,
+                offset = 56,
+                limit = 56
             )
         else:
-            return ListResponseMeta(
+            return ListResponseMetaPagination(
         )
         """
 
-    def testListResponseMeta(self):
-        """Test ListResponseMeta"""
+    def testListResponseMetaPagination(self):
+        """Test ListResponseMetaPagination"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_meta.py` & `odm_api-1.57.0/test/test_metainfo_key_for_summary.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.meta import Meta
+from odm_api.models.metainfo_key_for_summary import MetainfoKeyForSummary
 
-class TestMeta(unittest.TestCase):
-    """Meta unit test stubs"""
+class TestMetainfoKeyForSummary(unittest.TestCase):
+    """MetainfoKeyForSummary unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> Meta:
-        """Test Meta
+    def make_instance(self, include_optional) -> MetainfoKeyForSummary:
+        """Test MetainfoKeyForSummary
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Meta`
+        # uncomment below to create an instance of `MetainfoKeyForSummary`
         """
-        model = Meta()
+        model = MetainfoKeyForSummary()
         if include_optional:
-            return Meta(
-                created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                last_modified = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                resource_type = 'User'
+            return MetainfoKeyForSummary(
+                key = '',
+                values = [
+                    ''
+                    ]
             )
         else:
-            return Meta(
+            return MetainfoKeyForSummary(
         )
         """
 
-    def testMeta(self):
-        """Test Meta"""
+    def testMetainfoKeyForSummary(self):
+        """Test MetainfoKeyForSummary"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_metadata_presentation.py` & `odm_api-1.57.0/test/test_metadata_presentation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
@@ -38,20 +38,16 @@
                 metadata = odm_api.models.metadata_presentation_metadata.MetadataPresentation_metadata(
                     source = '', 
                     name = '', 
                     public = True, 
                     id = '', 
                     content = odm_api.models.content.content(), 
                     data_type = '', 
-                    content_map = {
-                        'key' : None
-                        }, 
-                    metadata_content = {
-                        'key' : None
-                        }, 
+                    content_map = odm_api.models.content.content(), 
+                    metadata_content = odm_api.models.content.content(), 
                     file_id_associated_with_template = '', ),
                 relationships = odm_api.models.data_presentation_relationships.DataPresentation_relationships(
                     sample = '', 
                     cell = '', 
                     library = '', 
                     preparation = '', )
             )
```

### Comparing `odm-api-0.0.1/test/test_objects_page.py` & `odm_api-1.57.0/test/test_objects_page.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_omics_response.py` & `odm_api-1.57.0/test/test_variant_signal_source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.omics_response import OmicsResponse
+from odm_api.models.variant_signal_source import VariantSignalSource
 
-class TestOmicsResponse(unittest.TestCase):
-    """OmicsResponse unit test stubs"""
+class TestVariantSignalSource(unittest.TestCase):
+    """VariantSignalSource unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> OmicsResponse:
-        """Test OmicsResponse
+    def make_instance(self, include_optional) -> VariantSignalSource:
+        """Test VariantSignalSource
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `OmicsResponse`
+        # uncomment below to create an instance of `VariantSignalSource`
         """
-        model = OmicsResponse()
+        model = VariantSignalSource()
         if include_optional:
-            return OmicsResponse(
-                data = [
-                    None
-                    ],
-                results_exhausted = True,
-                log = [
-                    ''
-                    ],
-                cursor = ''
+            return VariantSignalSource(
+                template_id = 'GSF000001',
+                link = '',
+                metadata_link = '',
+                previous_version = ''
             )
         else:
-            return OmicsResponse(
+            return VariantSignalSource(
+                link = '',
         )
         """
 
-    def testOmicsResponse(self):
-        """Test OmicsResponse"""
+    def testVariantSignalSource(self):
+        """Test VariantSignalSource"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_output_errors_inner.py` & `odm_api-1.57.0/test/test_create_group_request_members_inner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.output_errors_inner import OutputErrorsInner
+from odm_api.models.create_group_request_members_inner import CreateGroupRequestMembersInner
 
-class TestOutputErrorsInner(unittest.TestCase):
-    """OutputErrorsInner unit test stubs"""
+class TestCreateGroupRequestMembersInner(unittest.TestCase):
+    """CreateGroupRequestMembersInner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> OutputErrorsInner:
-        """Test OutputErrorsInner
+    def make_instance(self, include_optional) -> CreateGroupRequestMembersInner:
+        """Test CreateGroupRequestMembersInner
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `OutputErrorsInner`
+        # uncomment below to create an instance of `CreateGroupRequestMembersInner`
         """
-        model = OutputErrorsInner()
+        model = CreateGroupRequestMembersInner()
         if include_optional:
-            return OutputErrorsInner(
-                stage = '',
-                stack = [
-                    {type=type, message=message}
-                    ]
+            return CreateGroupRequestMembersInner(
+                value = '',
+                display = '',
+                ref = ''
             )
         else:
-            return OutputErrorsInner(
+            return CreateGroupRequestMembersInner(
+                value = '',
+                ref = '',
         )
         """
 
-    def testOutputErrorsInner(self):
-        """Test OutputErrorsInner"""
+    def testCreateGroupRequestMembersInner(self):
+        """Test CreateGroupRequestMembersInner"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_preparation_integration_as_curator_api.py` & `odm_api-1.57.0/test/test_variant_integration_as_curator_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,87 +1,80 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.api.preparation_integration_as_curator_api import PreparationIntegrationAsCuratorApi
+from odm_api.api.variant_integration_as_curator_api import VariantIntegrationAsCuratorApi
 
 
-class TestPreparationIntegrationAsCuratorApi(unittest.TestCase):
-    """PreparationIntegrationAsCuratorApi unit test stubs"""
+class TestVariantIntegrationAsCuratorApi(unittest.TestCase):
+    """VariantIntegrationAsCuratorApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = PreparationIntegrationAsCuratorApi()
+        self.api = VariantIntegrationAsCuratorApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_create_preparation_group_sample_group_link_as_curator(self) -> None:
-        """Test case for create_preparation_group_sample_group_link_as_curator
+    def test_create_variant_group_sample_group_link_as_curator(self) -> None:
+        """Test case for create_variant_group_sample_group_link_as_curator
 
-        Create links between samples and preparations
+        Create a link between a group of variant objects and a group of sample objects
         """
         pass
 
-    def test_create_preparation_sample_link_as_curator(self) -> None:
-        """Test case for create_preparation_sample_link_as_curator
+    def test_create_variant_sample_link_as_curator(self) -> None:
+        """Test case for create_variant_sample_link_as_curator
 
-        Create a link between a preparation and a sample
+        Create a link between a variant object and a sample
         """
         pass
 
-    def test_delete_preparation_group_sample_group_link_as_curator(self) -> None:
-        """Test case for delete_preparation_group_sample_group_link_as_curator
+    def test_delete_variant_group_sample_group_link_as_curator(self) -> None:
+        """Test case for delete_variant_group_sample_group_link_as_curator
 
-        Delete links between samples and preparations related to the specified group
+        Delete link between a group of variant objects and a group of sample objects
         """
         pass
 
-    def test_delete_preparation_sample_link_as_curator(self) -> None:
-        """Test case for delete_preparation_sample_link_as_curator
+    def test_delete_variant_sample_link_as_curator(self) -> None:
+        """Test case for delete_variant_sample_link_as_curator
 
-        Delete a link between a preparation and a sample
+        Delete link between a variant object and a sample
         """
         pass
 
-    def test_get_preparation_by_sample_as_curator(self) -> None:
-        """Test case for get_preparation_by_sample_as_curator
+    def test_get_variant_by_sample_as_curator(self) -> None:
+        """Test case for get_variant_by_sample_as_curator
 
-        Retrieve preparation metadata by querying related sample ID (accession)
+        Retrieve variant run-level data by querying related sample ID (accession)
         """
         pass
 
-    def test_get_preparation_groups_by_study_as_curator(self) -> None:
-        """Test case for get_preparation_groups_by_study_as_curator
+    def test_get_variant_groups_by_study_as_curator(self) -> None:
+        """Test case for get_variant_groups_by_study_as_curator
 
         Retrieve group metadata by querying study ID (accession)
         """
         pass
 
-    def test_get_preparation_links_to_samples_as_curator(self) -> None:
-        """Test case for get_preparation_links_to_samples_as_curator
+    def test_get_variant_run_to_sample_pairs_as_curator(self) -> None:
+        """Test case for get_variant_run_to_sample_pairs_as_curator
 
-        Retrieve run-sample pairs by group id. Pagination is based on unique preparations, not unique pairs.
-        """
-        pass
-
-    def test_get_preparations_by_samples_as_curator(self) -> None:
-        """Test case for get_preparations_by_samples_as_curator
-
-        Retrieve preparation metadata by querying related samples
+        Retrieve run-sample pairs by group id. Pagination is based on unique runs, not unique pairs.
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_preparation_integration_as_user_api.py` & `odm_api-1.57.0/test/test_library_integration_as_user_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.api.preparation_integration_as_user_api import PreparationIntegrationAsUserApi
+from odm_api.api.library_integration_as_user_api import LibraryIntegrationAsUserApi
 
 
-class TestPreparationIntegrationAsUserApi(unittest.TestCase):
-    """PreparationIntegrationAsUserApi unit test stubs"""
+class TestLibraryIntegrationAsUserApi(unittest.TestCase):
+    """LibraryIntegrationAsUserApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = PreparationIntegrationAsUserApi()
+        self.api = LibraryIntegrationAsUserApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_get_preparation_by_sample_as_user(self) -> None:
-        """Test case for get_preparation_by_sample_as_user
+    def test_get_libraries_by_samples_as_user(self) -> None:
+        """Test case for get_libraries_by_samples_as_user
 
-        Retrieve preparation metadata by querying related sample ID (accession)
+        Retrieve library metadata by querying related samples
         """
         pass
 
-    def test_get_preparation_groups_by_study_as_user(self) -> None:
-        """Test case for get_preparation_groups_by_study_as_user
+    def test_get_library_by_sample_as_user(self) -> None:
+        """Test case for get_library_by_sample_as_user
 
-        Retrieve group metadata by querying study ID (accession)
+        Retrieve library metadata by querying related sample ID (accession)
         """
         pass
 
-    def test_get_preparation_links_to_samples_as_user(self) -> None:
-        """Test case for get_preparation_links_to_samples_as_user
+    def test_get_library_groups_by_study_as_user(self) -> None:
+        """Test case for get_library_groups_by_study_as_user
 
-        Retrieve run-sample pairs by group id. Pagination is based on unique preparations, not unique pairs.
+        Retrieve group metadata by querying study ID (accession)
         """
         pass
 
-    def test_get_preparations_by_samples_as_user(self) -> None:
-        """Test case for get_preparations_by_samples_as_user
+    def test_get_library_links_to_samples_as_user(self) -> None:
+        """Test case for get_library_links_to_samples_as_user
 
-        Retrieve preparation metadata by querying related samples
+        Retrieve library-samples pairs by group id. Pagination is based on unique libraries, not unique pairs.
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_preparation_spo_tas_curator_api.py` & `odm_api-1.57.0/test/test_linkage_as_curator_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,94 +1,73 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.api.preparation_spo_tas_curator_api import PreparationSPoTAsCuratorApi
+from odm_api.api.linkage_as_curator_api import LinkageAsCuratorApi
 
 
-class TestPreparationSPoTAsCuratorApi(unittest.TestCase):
-    """PreparationSPoTAsCuratorApi unit test stubs"""
+class TestLinkageAsCuratorApi(unittest.TestCase):
+    """LinkageAsCuratorApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = PreparationSPoTAsCuratorApi()
+        self.api = LinkageAsCuratorApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_add_preparations_as_curator(self) -> None:
-        """Test case for add_preparations_as_curator
+    def test_delete_link_as_curator(self) -> None:
+        """Test case for delete_link_as_curator
 
-        Add new preparation object
+        Deletes existing links matching the specified criteria.
         """
         pass
 
-    def test_delete_preparation_as_curator(self) -> None:
-        """Test case for delete_preparation_as_curator
+    def test_get_data_types_as_curator(self) -> None:
+        """Test case for get_data_types_as_curator
 
-        Delete a preparation object
+        Lists all available data types.
         """
         pass
 
-    def test_delete_preparation_group_as_curator(self) -> None:
-        """Test case for delete_preparation_group_as_curator
+    def test_get_data_types_links_as_curator(self) -> None:
+        """Test case for get_data_types_links_as_curator
 
-        Delete a preparation group with all related preparation objects
+        List all possible links between data types that match the specified criteria.
         """
         pass
 
-    def test_get_preparation_as_curator(self) -> None:
-        """Test case for get_preparation_as_curator
+    def test_get_links_by_ids_as_curator(self) -> None:
+        """Test case for get_links_by_ids_as_curator
 
-        Retrieve a single preparation object by ID (accession)
+        Finds existing links by passing many IDs.  Pagination goes through all links matched the criteria.
         """
         pass
 
-    def test_get_preparation_by_version_as_curator(self) -> None:
-        """Test case for get_preparation_by_version_as_curator
+    def test_get_links_by_params_as_curator(self) -> None:
+        """Test case for get_links_by_params_as_curator
 
-        Retrieve a single preparation object by ID (accession)
+        Finds existing links matching the specified criteria.
         """
         pass
 
-    def test_get_preparation_versions_as_curator(self) -> None:
-        """Test case for get_preparation_versions_as_curator
+    def test_save_links_as_curator(self) -> None:
+        """Test case for save_links_as_curator
 
-        Retrieve a list of object versions by ID
-        """
-        pass
-
-    def test_get_preparations_by_group_as_curator(self) -> None:
-        """Test case for get_preparations_by_group_as_curator
-
-        Retrieve preparations related to the given group
-        """
-        pass
-
-    def test_search_preparations_as_curator(self) -> None:
-        """Test case for search_preparations_as_curator
-
-        List or search for preparation metadata objects
-        """
-        pass
-
-    def test_update_preparation_as_curator(self) -> None:
-        """Test case for update_preparation_as_curator
-
-        Update a preparation object
+        Creates new links between objects.
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_preparation_spo_tas_user_api.py` & `odm_api-1.57.0/test/test_library_spo_tas_user_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.api.preparation_spo_tas_user_api import PreparationSPoTAsUserApi
+from odm_api.api.library_spo_tas_user_api import LibrarySPoTAsUserApi
 
 
-class TestPreparationSPoTAsUserApi(unittest.TestCase):
-    """PreparationSPoTAsUserApi unit test stubs"""
+class TestLibrarySPoTAsUserApi(unittest.TestCase):
+    """LibrarySPoTAsUserApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = PreparationSPoTAsUserApi()
+        self.api = LibrarySPoTAsUserApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_get_preparation_as_user(self) -> None:
-        """Test case for get_preparation_as_user
+    def test_get_libraries_by_group_as_user(self) -> None:
+        """Test case for get_libraries_by_group_as_user
 
-        Retrieve a single preparation object by ID (accession)
+        Retrieve libraries related to the given group
         """
         pass
 
-    def test_get_preparation_by_version_as_user(self) -> None:
-        """Test case for get_preparation_by_version_as_user
+    def test_get_library_as_user(self) -> None:
+        """Test case for get_library_as_user
 
-        Retrieve a single preparation object by ID (accession)
+        Retrieve a single library object by ID (accession)
         """
         pass
 
-    def test_get_preparation_versions_as_user(self) -> None:
-        """Test case for get_preparation_versions_as_user
+    def test_get_library_by_version_as_user(self) -> None:
+        """Test case for get_library_by_version_as_user
 
-        Retrieve a list of object versions by ID
+        Retrieve a single library object by ID (accession)
         """
         pass
 
-    def test_get_preparations_by_group_as_user(self) -> None:
-        """Test case for get_preparations_by_group_as_user
+    def test_get_library_versions_as_user(self) -> None:
+        """Test case for get_library_versions_as_user
 
-        Retrieve preparations related to the given group
+        Retrieve a list of object versions by ID
         """
         pass
 
-    def test_search_preparations_as_user(self) -> None:
-        """Test case for search_preparations_as_user
+    def test_search_libraries_as_user(self) -> None:
+        """Test case for search_libraries_as_user
 
-        List or search for preparation metadata objects
+        List or search for library metadata objects
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_runs_response.py` & `odm_api-1.57.0/test/test_variant_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,54 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.runs_response import RunsResponse
+from odm_api.models.variant_response import VariantResponse
 
-class TestRunsResponse(unittest.TestCase):
-    """RunsResponse unit test stubs"""
+class TestVariantResponse(unittest.TestCase):
+    """VariantResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> RunsResponse:
-        """Test RunsResponse
+    def make_instance(self, include_optional) -> VariantResponse:
+        """Test VariantResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `RunsResponse`
+        # uncomment below to create an instance of `VariantResponse`
         """
-        model = RunsResponse()
+        model = VariantResponse()
         if include_optional:
-            return RunsResponse(
-                runs = [
-                    None
+            return VariantResponse(
+                data = [
+                    {reference=reference, itemId=itemId, metadata={}, variationId=[variationId, variationId], groupId=groupId, start=0, alteration=[alteration, alteration], runId=runId, contig=contig, info={key=[info, info]}, genotype={key=genotype}}
                     ],
-                experiment = '',
-                warnings = [
-                    ''
-                    ],
-                version_chain_id = ''
+                cursor = ''
             )
         else:
-            return RunsResponse(
+            return VariantResponse(
         )
         """
 
-    def testRunsResponse(self):
-        """Test RunsResponse"""
+    def testVariantResponse(self):
+        """Test VariantResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_scim_error_response.py` & `odm_api-1.57.0/test/test_page_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,52 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.scim_error_response import SCIMErrorResponse
+from odm_api.models.page_request import PageRequest
 
-class TestSCIMErrorResponse(unittest.TestCase):
-    """SCIMErrorResponse unit test stubs"""
+class TestPageRequest(unittest.TestCase):
+    """PageRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> SCIMErrorResponse:
-        """Test SCIMErrorResponse
+    def make_instance(self, include_optional) -> PageRequest:
+        """Test PageRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SCIMErrorResponse`
+        # uncomment below to create an instance of `PageRequest`
         """
-        model = SCIMErrorResponse()
+        model = PageRequest()
         if include_optional:
-            return SCIMErrorResponse(
-                detail = '',
-                schemas = [
-                    'urn:ietf:params:scim:api:messages:2.0:Error'
-                    ],
-                scim_type = 'uniqueness',
-                status = ''
+            return PageRequest(
+                offset = 56,
+                limit = 50
             )
         else:
-            return SCIMErrorResponse(
-                status = '',
+            return PageRequest(
         )
         """
 
-    def testSCIMErrorResponse(self):
-        """Test SCIMErrorResponse"""
+    def testPageRequest(self):
+        """Test PageRequest"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_start_import_flow_cytometry_request.py` & `odm_api-1.57.0/test/test_start_import_flow_cytometry_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_study_search_info.py` & `odm_api-1.57.0/test/test_commit_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,54 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.study_search_info import StudySearchInfo
+from odm_api.models.commit_info import CommitInfo
 
-class TestStudySearchInfo(unittest.TestCase):
-    """StudySearchInfo unit test stubs"""
+class TestCommitInfo(unittest.TestCase):
+    """CommitInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> StudySearchInfo:
-        """Test StudySearchInfo
+    def make_instance(self, include_optional) -> CommitInfo:
+        """Test CommitInfo
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `StudySearchInfo`
+        # uncomment below to create an instance of `CommitInfo`
         """
-        model = StudySearchInfo()
+        model = CommitInfo()
         if include_optional:
-            return StudySearchInfo(
-                accession = '',
-                name = '',
-                owner = '',
-                file_creation = '',
-                size = 56,
-                has_facs = True,
-                has_genomic = True,
-                has_transcriptomics = True,
-                summary = [
-                    {values=[values, values], key=key}
-                    ]
+            return CommitInfo(
+                author = '',
+                message = '',
+                timestamp = 56,
+                version = ''
             )
         else:
-            return StudySearchInfo(
+            return CommitInfo(
         )
         """
 
-    def testStudySearchInfo(self):
-        """Test StudySearchInfo"""
+    def testCommitInfo(self):
+        """Test CommitInfo"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_user.py` & `odm_api-1.57.0/test/test_create_user_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.user import User
+from odm_api.models.create_user_request import CreateUserRequest
 
-class TestUser(unittest.TestCase):
-    """User unit test stubs"""
+class TestCreateUserRequest(unittest.TestCase):
+    """CreateUserRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> User:
-        """Test User
+    def make_instance(self, include_optional) -> CreateUserRequest:
+        """Test CreateUserRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `User`
+        # uncomment below to create an instance of `CreateUserRequest`
         """
-        model = User()
+        model = CreateUserRequest()
         if include_optional:
-            return User(
+            return CreateUserRequest(
                 active = True,
                 emails = [
                     {type=work, value=value, primary=true}
                     ],
                 external_id = '',
                 id = '',
                 schemas = [
                     'urn:ietf:params:scim:schemas:core:2.0:User'
                     ],
                 user_name = '',
                 display_name = ''
             )
         else:
-            return User(
+            return CreateUserRequest(
                 active = True,
                 emails = [
                     {type=work, value=value, primary=true}
                     ],
                 display_name = '',
         )
         """
 
-    def testUser(self):
-        """Test User"""
+    def testCreateUserRequest(self):
+        """Test CreateUserRequest"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_user_response.py` & `odm_api-1.57.0/test/test_filter_users_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.user_response import UserResponse
+from odm_api.models.filter_users_response import FilterUsersResponse
 
-class TestUserResponse(unittest.TestCase):
-    """UserResponse unit test stubs"""
+class TestFilterUsersResponse(unittest.TestCase):
+    """FilterUsersResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> UserResponse:
-        """Test UserResponse
+    def make_instance(self, include_optional) -> FilterUsersResponse:
+        """Test FilterUsersResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `UserResponse`
+        # uncomment below to create an instance of `FilterUsersResponse`
         """
-        model = UserResponse()
+        model = FilterUsersResponse()
         if include_optional:
-            return UserResponse(
-                active = True,
-                emails = [
-                    {type=work, value=value, primary=true}
+            return FilterUsersResponse(
+                resources = [
+                    null
                     ],
-                external_id = '',
-                id = '',
+                items_per_page = 56,
                 schemas = [
-                    'urn:ietf:params:scim:schemas:core:2.0:User'
+                    'urn:ietf:params:scim:api:messages:2.0:ListResponse'
                     ],
-                user_name = '',
-                display_name = '',
-                meta = odm_api.models.create_user_201_response_all_of_meta.createUser_201_response_allOf_meta(
-                    created = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    last_modified = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    resource_type = 'User', )
+                start_index = 56,
+                total_results = 56
             )
         else:
-            return UserResponse(
-                active = True,
-                emails = [
-                    {type=work, value=value, primary=true}
-                    ],
-                display_name = '',
+            return FilterUsersResponse(
         )
         """
 
-    def testUserResponse(self):
-        """Test UserResponse"""
+    def testFilterUsersResponse(self):
+        """Test FilterUsersResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_validation_error.py` & `odm_api-1.57.0/test/test_validation_error.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_variant_integration_as_user_api.py` & `odm_api-1.57.0/test/test_variant_integration_as_user_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_variant_spo_tas_user_api.py` & `odm_api-1.57.0/test/test_job_operations_api.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,87 +1,59 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.api.variant_spo_tas_user_api import VariantSPoTAsUserApi
+from odm_api.api.job_operations_api import JobOperationsApi
 
 
-class TestVariantSPoTAsUserApi(unittest.TestCase):
-    """VariantSPoTAsUserApi unit test stubs"""
+class TestJobOperationsApi(unittest.TestCase):
+    """JobOperationsApi unit test stubs"""
 
     def setUp(self) -> None:
-        self.api = VariantSPoTAsUserApi()
+        self.api = JobOperationsApi()
 
     def tearDown(self) -> None:
         pass
 
-    def test_get_all_variants_as_user(self) -> None:
-        """Test case for get_all_variants_as_user
+    def test_info(self) -> None:
+        """Test case for info
 
-        Retrieve multiple variant data and metadata objects
+        get information about one particular job execution
         """
         pass
 
-    def test_get_variant_as_user(self) -> None:
-        """Test case for get_variant_as_user
+    def test_output(self) -> None:
+        """Test case for output
 
-        Retrieve a single variant object by ID (accession)
+        retrieve job output (result)
         """
         pass
 
-    def test_get_variant_by_version_as_user(self) -> None:
-        """Test case for get_variant_by_version_as_user
+    def test_restart(self) -> None:
+        """Test case for restart
 
-        Retrieve a single variant object by ID (accession)
+        restart stopped (failed) job
         """
         pass
 
-    def test_get_variant_group_as_user(self) -> None:
-        """Test case for get_variant_group_as_user
+    def test_stop(self) -> None:
+        """Test case for stop
 
-        Retrieve a single group object by ID (accession)
-        """
-        pass
-
-    def test_get_variant_group_by_run_as_user(self) -> None:
-        """Test case for get_variant_group_by_run_as_user
-
-        Retrieve a single group object by run ID (accession)
-        """
-        pass
-
-    def test_get_variant_versions_as_user(self) -> None:
-        """Test case for get_variant_versions_as_user
-
-        Retrieve a list of object versions by ID
-        """
-        pass
-
-    def test_search_variant_groups_as_user(self) -> None:
-        """Test case for search_variant_groups_as_user
-
-        Retrieve groups that match a query
-        """
-        pass
-
-    def test_search_variant_runs_as_user(self) -> None:
-        """Test case for search_variant_runs_as_user
-
-        Retrieve run objects related to the given group
+        stop running job
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_xref_set_search_result.py` & `odm_api-1.57.0/test/test_xref_set_search_result.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `odm-api-0.0.1/test/test_xref_set_search_result_entry.py` & `odm_api-1.57.0/test/test_xref_set_search_result_result_inner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.xref_set_search_result_entry import XrefSetSearchResultEntry
+from odm_api.models.xref_set_search_result_result_inner import XrefSetSearchResultResultInner
 
-class TestXrefSetSearchResultEntry(unittest.TestCase):
-    """XrefSetSearchResultEntry unit test stubs"""
+class TestXrefSetSearchResultResultInner(unittest.TestCase):
+    """XrefSetSearchResultResultInner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> XrefSetSearchResultEntry:
-        """Test XrefSetSearchResultEntry
+    def make_instance(self, include_optional) -> XrefSetSearchResultResultInner:
+        """Test XrefSetSearchResultResultInner
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `XrefSetSearchResultEntry`
+        # uncomment below to create an instance of `XrefSetSearchResultResultInner`
         """
-        model = XrefSetSearchResultEntry()
+        model = XrefSetSearchResultResultInner()
         if include_optional:
-            return XrefSetSearchResultEntry(
+            return XrefSetSearchResultResultInner(
                 xref_set_id = '"GSF0000013"',
                 source_id = '"ENSG00000231103.2"',
                 target_ids = ["ENST00000617423.4", "ENST00000334232.8"]
             )
         else:
-            return XrefSetSearchResultEntry(
+            return XrefSetSearchResultResultInner(
         )
         """
 
-    def testXrefSetSearchResultEntry(self):
-        """Test XrefSetSearchResultEntry"""
+    def testXrefSetSearchResultResultInner(self):
+        """Test XrefSetSearchResultResultInner"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `odm-api-0.0.1/test/test_xref_set_search_result_result_inner.py` & `odm_api-1.57.0/test/test_output_errors_inner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 # coding: utf-8
 
 """
-    Tasks API
+    ODM API
 
-    These API endpoints serve to work with asynchronous tasks. 
+    This swagger page describes the variantUser API endpoints for ODM. These are typically used to find and retrieve variant data and metadata.  Before carrying out any API calls you will need an API token. API tokens can be obtained under your profile within the Genestack software. Further instructions can be found [here](https://odm-user-guide.readthedocs.io/en/latest/doc-odm-user-guide/getting-a-genestack-api-token.html).  To try out calls in this swagger page:  1.  Click the 'Authorize' button below to enter your API token 2.  Scroll to the 'Parameters' section for the method you wish to try out and click the 'Try it out' button 3.  Enter parameter values that you wish to try 4.  Scroll to the bottom of the Parameters section and click the 'Execute' bar that appears    The server response will be in the section that follows.
 
     The version of the OpenAPI document: default-released
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 import unittest
 
-from odm_api.models.xref_set_search_result_result_inner import XrefSetSearchResultResultInner
+from odm_api.models.output_errors_inner import OutputErrorsInner
 
-class TestXrefSetSearchResultResultInner(unittest.TestCase):
-    """XrefSetSearchResultResultInner unit test stubs"""
+class TestOutputErrorsInner(unittest.TestCase):
+    """OutputErrorsInner unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def make_instance(self, include_optional) -> XrefSetSearchResultResultInner:
-        """Test XrefSetSearchResultResultInner
+    def make_instance(self, include_optional) -> OutputErrorsInner:
+        """Test OutputErrorsInner
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `XrefSetSearchResultResultInner`
+        # uncomment below to create an instance of `OutputErrorsInner`
         """
-        model = XrefSetSearchResultResultInner()
+        model = OutputErrorsInner()
         if include_optional:
-            return XrefSetSearchResultResultInner(
-                xref_set_id = '"GSF0000013"',
-                source_id = '"ENSG00000231103.2"',
-                target_ids = ["ENST00000617423.4", "ENST00000334232.8"]
+            return OutputErrorsInner(
+                stage = '',
+                stack = [
+                    {type=type, message=message}
+                    ]
             )
         else:
-            return XrefSetSearchResultResultInner(
+            return OutputErrorsInner(
         )
         """
 
-    def testXrefSetSearchResultResultInner(self):
-        """Test XrefSetSearchResultResultInner"""
+    def testOutputErrorsInner(self):
+        """Test OutputErrorsInner"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

