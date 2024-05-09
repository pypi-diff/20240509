# Comparing `tmp/odm-sdk-0.0.1.tar.gz` & `tmp/odm_sdk-1.57.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odm-sdk-0.0.1.tar", last modified: Thu Feb 22 14:36:11 2024, max compression
+gzip compressed data, was "odm_sdk-1.57.0.tar", last modified: Thu May  9 11:04:17 2024, max compression
```

## Comparing `odm-sdk-0.0.1.tar` & `odm_sdk-1.57.0.tar`

### file list

```diff
@@ -1,102 +1,97 @@
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.137929 odm-sdk-0.0.1/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1089 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/LICENSE.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      199 2024-02-12 09:45:53.000000 odm-sdk-0.0.1/MANIFEST.in
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1256 2024-02-22 14:36:11.137685 odm-sdk-0.0.1/PKG-INFO
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      667 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/README.md
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.126419 odm-sdk-0.0.1/odm_sdk/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1084 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/odm_sdk/__init__.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2159 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/bio_meta_keys.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    10516 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/odm_sdk/chunked_upload.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    10682 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/cla.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    13028 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/odm_sdk/connection.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3418 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/data_flow_editor.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    30993 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/data_importer.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     5918 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/datasets_util.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3766 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/odm_sdk/exceptions.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     7208 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/expression_navigator.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     5579 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/file_filters.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1323 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/file_initializer.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      239 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/file_permissions.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1757 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/file_types.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    23275 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/odm_sdk/files_util.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1957 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/genome_query.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      493 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/groups_util.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    13264 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/odm_sdk/metainfo.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     7634 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/metainfo_scalar_values.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     5961 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/samples.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.129935 odm-sdk-0.0.1/odm_sdk/scripts/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)        0 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/__init__.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1270 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/delete_study_or_template.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.130363 odm-sdk-0.0.1/odm_sdk/scripts/dictionaries/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      242 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/dictionaries/__init__.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4868 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/dictionaries/load_init_share_dictionaries.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    74461 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/import_ODM_data.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.131523 odm-sdk-0.0.1/odm_sdk/scripts/internal/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      242 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/internal/__init__.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.131688 odm-sdk-0.0.1/odm_sdk/scripts/internal/data/
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)       82 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/internal/data/disease_extension.csv
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    12766 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/internal/generate_dictionaries.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2954 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/internal/upload_dictionaries_with_specific_metainfo.py
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)     1827 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/internal/upload_gene_dictionary.py
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)     1390 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/internal/wait_for_host.py
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)     1547 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/internal/wait_until_ready.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.132084 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)        0 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/__init__.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1127 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/get_template.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.132948 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)       64 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/__init__.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1124 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/dictionary_search.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1448 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/format.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1177 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/json_validation.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.133332 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/schemas/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1032 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/schemas/config_schema.json
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2276 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/schemas/template_schema.json
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)     5831 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/template_importer.py
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)     1106 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/update_template.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2829 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/odm_sdk/scripts/shell.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.134076 odm-sdk-0.0.1/odm_sdk/scripts/study_management/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     4463 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/study_management/GEO_prepare.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)       61 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/study_management/__init__.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     5129 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/study_management/create_curation_file.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2981 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/study_management/share_study_with_group.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     3493 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/upload_reference_genome.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    12441 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/odm_sdk/scripts/user_setup.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.135002 odm-sdk-0.0.1/odm_sdk/scripts/users/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)        0 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/users/__init__.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     5083 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/users/add_permissions_to_users.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      836 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/users/add_token_to_user.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     6115 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/users/add_users_to_groups.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2641 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/users/create_groups.py
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)     3278 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/users/create_users.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1346 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/scripts/utils.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.135615 odm-sdk-0.0.1/odm_sdk/settings/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)       84 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/odm_sdk/settings/__init__.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     9673 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/odm_sdk/settings/config.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     5199 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/odm_sdk/settings/user.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    10225 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/share_util.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)    13828 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/odm_sdk/shell.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2293 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/task_log_viewer.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.136007 odm-sdk-0.0.1/odm_sdk/tests/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)        0 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/tests/__init__.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     7907 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/tests/test_import.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      668 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/unaligned_reads.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     6771 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/odm_sdk/utils.py
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      142 2024-02-22 14:33:50.000000 odm-sdk-0.0.1/odm_sdk/version.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.137272 odm-sdk-0.0.1/odm_sdk.egg-info/
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     1256 2024-02-22 14:36:11.000000 odm-sdk-0.0.1/odm_sdk.egg-info/PKG-INFO
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)     2920 2024-02-22 14:36:11.000000 odm-sdk-0.0.1/odm_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)        1 2024-02-22 14:36:11.000000 odm-sdk-0.0.1/odm_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      818 2024-02-22 14:36:11.000000 odm-sdk-0.0.1/odm_sdk.egg-info/entry_points.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)      105 2024-02-22 14:36:11.000000 odm-sdk-0.0.1/odm_sdk.egg-info/requires.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)        8 2024-02-22 14:36:11.000000 odm-sdk-0.0.1/odm_sdk.egg-info/top_level.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)       93 2024-02-21 12:56:19.000000 odm-sdk-0.0.1/requirements-internal.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)       36 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/requirements-test.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)       89 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/requirements.txt
--rw-r--r--   0 olegkunitsyn   (501) staff       (20)       38 2024-02-22 14:36:11.137974 odm-sdk-0.0.1/setup.cfg
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)     2871 2024-02-21 14:39:15.000000 odm-sdk-0.0.1/setup.py
-drwxr-xr-x   0 olegkunitsyn   (501) staff       (20)        0 2024-02-22 14:36:11.137057 odm-sdk-0.0.1/test/
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)     3124 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/test/test_arguments.py
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)     2608 2024-02-20 09:46:59.000000 odm-sdk-0.0.1/test/test_connection.py
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)     3903 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/test/test_differential_expression.py
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)     2313 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/test/test_file_filters.py
--rwxr-xr-x   0 olegkunitsyn   (501) staff       (20)     3212 2024-02-09 18:34:01.000000 odm-sdk-0.0.1/test/test_metainfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.392775 odm_sdk-1.57.0/
+-rw-r--r--   0 root         (0) root         (0)     1089 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      199 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-05-09 11:04:17.392775 odm_sdk-1.57.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      667 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.384775 odm_sdk-1.57.0/odm_sdk/
+-rw-r--r--   0 root         (0) root         (0)     1084 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/bio_meta_keys.py
+-rw-r--r--   0 root         (0) root         (0)    10516 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/chunked_upload.py
+-rw-r--r--   0 root         (0) root         (0)    10682 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/cla.py
+-rw-r--r--   0 root         (0) root         (0)    13965 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/connection.py
+-rw-r--r--   0 root         (0) root         (0)     3418 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/data_flow_editor.py
+-rw-r--r--   0 root         (0) root         (0)    30993 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/data_importer.py
+-rw-r--r--   0 root         (0) root         (0)     5918 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/datasets_util.py
+-rw-r--r--   0 root         (0) root         (0)     3766 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7208 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/expression_navigator.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/file_filters.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/file_initializer.py
+-rw-r--r--   0 root         (0) root         (0)      239 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/file_permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/file_types.py
+-rw-r--r--   0 root         (0) root         (0)    23275 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/files_util.py
+-rw-r--r--   0 root         (0) root         (0)     1957 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/genome_query.py
+-rw-r--r--   0 root         (0) root         (0)      493 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/groups_util.py
+-rw-r--r--   0 root         (0) root         (0)    13264 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/metainfo.py
+-rw-r--r--   0 root         (0) root         (0)     7634 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/metainfo_scalar_values.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/samples.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.384775 odm_sdk-1.57.0/odm_sdk/scripts/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/delete_study_or_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.388775 odm_sdk-1.57.0/odm_sdk/scripts/dictionaries/
+-rw-r--r--   0 root         (0) root         (0)      242 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/dictionaries/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4868 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/dictionaries/load_init_share_dictionaries.py
+-rw-r--r--   0 root         (0) root         (0)    74461 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/import_ODM_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.388775 odm_sdk-1.57.0/odm_sdk/scripts/internal/
+-rw-r--r--   0 root         (0) root         (0)     1157 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/internal/README.md
+-rw-r--r--   0 root         (0) root         (0)      242 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.388775 odm_sdk-1.57.0/odm_sdk/scripts/internal/data/
+-rwxr-xr-x   0 root         (0) root         (0)       82 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/internal/data/disease_extension.csv
+-rw-r--r--   0 root         (0) root         (0)    18277 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/internal/generate_gene_dictionaries.py
+-rw-r--r--   0 root         (0) root         (0)    12766 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/internal/generate_unit_dictionaries.py
+-rw-r--r--   0 root         (0) root         (0)     4244 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/internal/upload_dictionaries_with_specific_metainfo.py
+-rwxr-xr-x   0 root         (0) root         (0)     1390 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/internal/wait_for_host.py
+-rwxr-xr-x   0 root         (0) root         (0)     1547 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/internal/wait_until_ready.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.388775 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/get_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.388775 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/
+-rw-r--r--   0 root         (0) root         (0)       64 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/dictionary_search.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/format.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/json_validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.388775 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/schemas/
+-rw-r--r--   0 root         (0) root         (0)     1032 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/schemas/config_schema.json
+-rw-r--r--   0 root         (0) root         (0)     2276 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/schemas/template_schema.json
+-rwxr-xr-x   0 root         (0) root         (0)     5831 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/template_importer.py
+-rwxr-xr-x   0 root         (0) root         (0)     1106 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/update_template.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/shell.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.392775 odm_sdk-1.57.0/odm_sdk/scripts/study_management/
+-rw-r--r--   0 root         (0) root         (0)     4463 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/study_management/GEO_prepare.py
+-rw-r--r--   0 root         (0) root         (0)       61 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/study_management/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/study_management/create_curation_file.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/study_management/share_study_with_group.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/upload_reference_genome.py
+-rw-r--r--   0 root         (0) root         (0)    13209 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/user_setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.392775 odm_sdk-1.57.0/odm_sdk/scripts/users/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/users/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5083 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/users/add_permissions_to_users.py
+-rw-r--r--   0 root         (0) root         (0)      836 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/users/add_token_to_user.py
+-rw-r--r--   0 root         (0) root         (0)     6115 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/users/add_users_to_groups.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/users/create_groups.py
+-rwxr-xr-x   0 root         (0) root         (0)     3278 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/users/create_users.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/scripts/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.392775 odm_sdk-1.57.0/odm_sdk/settings/
+-rw-r--r--   0 root         (0) root         (0)       84 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/settings/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9673 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/settings/config.py
+-rw-r--r--   0 root         (0) root         (0)     7398 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/settings/user.py
+-rw-r--r--   0 root         (0) root         (0)    10225 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/share_util.py
+-rw-r--r--   0 root         (0) root         (0)    13828 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/shell.py
+-rw-r--r--   0 root         (0) root         (0)     2293 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/task_log_viewer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.392775 odm_sdk-1.57.0/odm_sdk/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7907 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/tests/test_import.py
+-rw-r--r--   0 root         (0) root         (0)      668 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/unaligned_reads.py
+-rw-r--r--   0 root         (0) root         (0)     7258 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/odm_sdk/utils.py
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-09 11:04:17.000000 odm_sdk-1.57.0/odm_sdk/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 11:04:17.392775 odm_sdk-1.57.0/odm_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-05-09 11:04:17.000000 odm_sdk-1.57.0/odm_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2832 2024-05-09 11:04:17.000000 odm_sdk-1.57.0/odm_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 11:04:17.000000 odm_sdk-1.57.0/odm_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      818 2024-05-09 11:04:17.000000 odm_sdk-1.57.0/odm_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-09 11:04:17.000000 odm_sdk-1.57.0/odm_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 11:04:17.000000 odm_sdk-1.57.0/odm_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-09 11:03:38.000000 odm_sdk-1.57.0/requirements-internal.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/requirements-test.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 11:04:17.392775 odm_sdk-1.57.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2861 2020-04-16 12:00:00.000000 odm_sdk-1.57.0/setup.py
```

### Comparing `odm-sdk-0.0.1/LICENSE.txt` & `odm_sdk-1.57.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/PKG-INFO` & `odm_sdk-1.57.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: odm-sdk
-Version: 0.0.1
+Version: 1.57.0
 Summary: SDK for interacting with the Open Data Manager
-Home-page: https://github.com/genestack/python-client
+Home-page: https://github.com/genestack/sdk
 Author: Genestack Limited
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://genestack-client.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/genestack/python-client/
 Project-URL: Tracker, https://github.com/genestack/python-client/issues
 Keywords: genestack,odm,import,share,create,delete,curate,genomics,api
@@ -18,13 +18,13 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: keyring==24.3.0
+Requires-Dist: keyring==25.2.0
 Requires-Dist: requests==2.31.0
-Requires-Dist: pyOpenSSL==24.0.0
-Requires-Dist: jsonschema==4.21.1
+Requires-Dist: pyOpenSSL==24.1.0
+Requires-Dist: jsonschema==4.22.0
 Requires-Dist: pyrsistent==0.20.0
-Requires-Dist: odm-api==1.56.1
+Requires-Dist: odm-api==1.57.0
```

### Comparing `odm-sdk-0.0.1/README.md` & `odm_sdk-1.57.0/README.md`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/__init__.py` & `odm_sdk-1.57.0/odm_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/bio_meta_keys.py` & `odm_sdk-1.57.0/odm_sdk/bio_meta_keys.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/chunked_upload.py` & `odm_sdk-1.57.0/odm_sdk/chunked_upload.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/cla.py` & `odm_sdk-1.57.0/odm_sdk/cla.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/connection.py` & `odm_sdk-1.57.0/odm_sdk/connection.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,14 +127,33 @@
         """
         logged = self.application('genestack/signin').invoke('authenticateByApiToken', token)
         Connection._handle_inactive_user_auth(logged)
         if not logged['authenticated']:
             hostname = urlsplit(self.server_url).hostname
             raise GenestackAuthenticationException('Fail to login by token to %s' % hostname)
 
+    def login_by_access_token(self, access_token):
+        """
+        Attempt a login on the connection with the specified access token.
+        Raises an exception if the login fails.
+
+        :param access_token: OAuth access token
+        :type access_token: str
+        :rtype: None
+        :raises: :py:class:`~odm_sdk.GenestackAuthenticationException` if login failed
+        """
+        access_token = os.getenv(access_token, access_token)
+        self.session.headers.update({'Authorization': f'Bearer {access_token}'})
+        logged = self.application('genestack/signin').invoke('authenticateOAuthAccessToken', access_token)
+        Connection._handle_inactive_user_auth(logged)
+        if not logged['authenticated']:
+            self.session.headers.pop('Authorization')
+            hostname = urlsplit(self.server_url).hostname
+            raise GenestackAuthenticationException('Fail to login by token to %s' % hostname)
+
     def logout(self):
         """
         Logout from server.
 
         :rtype: None
         """
         self.application('genestack/signin').invoke('signOut')
```

### Comparing `odm-sdk-0.0.1/odm_sdk/data_flow_editor.py` & `odm_sdk-1.57.0/odm_sdk/data_flow_editor.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/data_importer.py` & `odm_sdk-1.57.0/odm_sdk/data_importer.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/datasets_util.py` & `odm_sdk-1.57.0/odm_sdk/datasets_util.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/exceptions.py` & `odm_sdk-1.57.0/odm_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/expression_navigator.py` & `odm_sdk-1.57.0/odm_sdk/expression_navigator.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/file_filters.py` & `odm_sdk-1.57.0/odm_sdk/file_filters.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/file_initializer.py` & `odm_sdk-1.57.0/odm_sdk/file_initializer.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/file_types.py` & `odm_sdk-1.57.0/odm_sdk/file_types.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/files_util.py` & `odm_sdk-1.57.0/odm_sdk/files_util.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/genome_query.py` & `odm_sdk-1.57.0/odm_sdk/genome_query.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/metainfo.py` & `odm_sdk-1.57.0/odm_sdk/metainfo.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/metainfo_scalar_values.py` & `odm_sdk-1.57.0/odm_sdk/metainfo_scalar_values.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/samples.py` & `odm_sdk-1.57.0/odm_sdk/samples.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/delete_study_or_template.py` & `odm_sdk-1.57.0/odm_sdk/scripts/delete_study_or_template.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/dictionaries/load_init_share_dictionaries.py` & `odm_sdk-1.57.0/odm_sdk/scripts/dictionaries/load_init_share_dictionaries.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/import_ODM_data.py` & `odm_sdk-1.57.0/odm_sdk/scripts/import_ODM_data.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/internal/generate_dictionaries.py` & `odm_sdk-1.57.0/odm_sdk/scripts/internal/generate_unit_dictionaries.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/internal/upload_dictionaries_with_specific_metainfo.py` & `odm_sdk-1.57.0/odm_sdk/scripts/internal/upload_dictionaries_with_specific_metainfo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,11 @@
-import os
 from odm_sdk import get_connection, Metainfo
 from odm_sdk.scripts.dictionaries.load_init_share_dictionaries import (load_dictionary, sharing,
                                                                                    initialization)
 
-
-def get_path(path):
-    return os.path.join(os.path.dirname(__file__), 'data', path)
-
-
 def upload_disease():
 
     # Upload Disease Ontology
     disease_ontology = {
         'name': 'Disease Ontology',
         'url': 'https://odm-init.s3.amazonaws.com/dictionaries/with_specific_metainfo/doid.owl',
         'description': 'An ontology for describing the classification of human diseases organized by etiology. '
@@ -50,18 +44,53 @@
     metainfo = Metainfo()
     metainfo.add_string(Metainfo.DATA_TYPE, 'Gene Ontology')
     gene_ontology_accession = load_dictionary(connection, gene_ontology, metainfo=metainfo)
     sharing(connection, [gene_ontology_accession])
     initialization(connection, [gene_ontology_accession])
 
 
+def upload_gene_dictionaries():
+    organisms_to_load = [
+        'Bos taurus',
+        'Danio rerio',
+        'Homo sapiens',
+        'Macaca fascicularis',
+        'Mus musculus',
+        'Oryctolagus cuniculus',
+        'Rattus norvegicus',
+        'Sus scrofa'
+    ]
+    connection = get_connection()
+    dictionary_accessions = []
+
+    for organism in organisms_to_load:
+        gene_dict = {
+            "name": organism + " genes",
+            "url": "https://odm-init.s3.ap-south-1.amazonaws.com/dictionaries/gene-dictionaries/" +
+                   organism.replace(" ", "+") + ".csv",
+            "description": "Dictionary contains the following information about gene: Ensembl gene name and id, "
+                           "Ensembl transcript name and id, Ensembl protein id, Reactome pathway name and id, "
+                           "Entrez gene id, Uniprot symbol, HGNC gene id and description, GO term label and id."
+        }
+
+        metainfo = Metainfo()
+        metainfo.add_string('genestack.dictionary:termType', 'gene')
+        metainfo.add_string('Release', '99')
+        metainfo.add_string('genestack.bio:organism', organism)
+        gene_ontology_accession = load_dictionary(connection, gene_dict, metainfo=metainfo)
+        dictionary_accessions.append(gene_ontology_accession)
+
+    sharing(connection, dictionary_accessions)
+
+
 def main():
     """
     Currently we don't support metainfo parsing via auxiliary scripts from json in proper way.
     In the future we have to add this possibility and rework script to using only CLI call.
     """
     upload_disease()
     upload_gene_ontology()
+    upload_gene_dictionaries()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/internal/wait_for_host.py` & `odm_sdk-1.57.0/odm_sdk/scripts/internal/wait_for_host.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/internal/wait_until_ready.py` & `odm_sdk-1.57.0/odm_sdk/scripts/internal/wait_until_ready.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/get_template.py` & `odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/get_template.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/dictionary_search.py` & `odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/dictionary_search.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/format.py` & `odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/format.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/json_validation.py` & `odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/json_validation.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/schemas/config_schema.json` & `odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/schemas/config_schema.json`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/schemas/template_schema.json` & `odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/schemas/template_schema.json`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/importers/template_importer.py` & `odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/importers/template_importer.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/metainfo_templates/update_template.py` & `odm_sdk-1.57.0/odm_sdk/scripts/metainfo_templates/update_template.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/shell.py` & `odm_sdk-1.57.0/odm_sdk/scripts/shell.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/study_management/GEO_prepare.py` & `odm_sdk-1.57.0/odm_sdk/scripts/study_management/GEO_prepare.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/study_management/create_curation_file.py` & `odm_sdk-1.57.0/odm_sdk/scripts/study_management/create_curation_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,27 +51,24 @@
 
 DEFAULT_VERSION_MESSAGE = "Edited using curation script"
 
 
 class CurationApplication(Application):
     APPLICATION_ID = "genestack/curation"
 
-    def create_files(self, target_studies_accessions, template_accession=None, overwrite=False,
+    def create_files(self, target_studies_accessions, overwrite=False,
                      dry_run=False, rules=None, new_version_message=None, publish_new_version=True):
-        return self.invoke('createCurationFiles', target_studies_accessions, template_accession,
+        return self.invoke('createCurationFiles', target_studies_accessions,
                            overwrite, dry_run, rules, new_version_message, publish_new_version)
 
 
 def main():
     parser = make_connection_parser()
     parser.add_argument('accessions', metavar='<accessions>', nargs='*',
                         help='Accession(s) of the study (or studies) to curate')
-    parser.add_argument('--template', metavar='<template>', default=None,
-                        help="Accession of the template to curate studies. If not specified "
-                             "use organization's default template")
     parser.add_argument('--dry-run', action='store_true', help='Do not write any metainfo')
     parser.add_argument('--overwrite', action='store_true', help='Overwrite existing curated keys')
     parser.add_argument('--rules', metavar='<rules_file>',
                         help='A JSON-formatted curation rules file')
     # make `publish_new_version = True` a default, allow overriding
     version_args = parser.add_mutually_exclusive_group()
     version_args.add_argument('--do-not-publish', action='store_false', dest='publish_new_version',
@@ -108,15 +105,14 @@
     except ValidationError as e:
         print("Invalid JSON curation file: " + e.message)
         sys.exit(1)
 
     print("Creating and initializing automated curation file...")
 
     accessions = curation_app.create_files(arguments.accessions,
-                                           arguments.template,
                                            arguments.overwrite,
                                            arguments.dry_run,
                                            rules,
                                            arguments.new_version_message,
                                            arguments.publish_new_version
                                            )
```

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/study_management/share_study_with_group.py` & `odm_sdk-1.57.0/odm_sdk/scripts/study_management/share_study_with_group.py`

 * *Files 13% similar despite different names*

```diff
@@ -46,35 +46,38 @@
     # The class constructor is a subject to change, its parameters might be changed in the future.
     def __init__(
             self,
             host,
             study_accession,
             group_name,
             token=None,
+            access_token=None,
             user=None,
             pwd=None,
             show_logs=False,
             debug=False
     ):
         self.host = host.rstrip('/')
         self.token = token
+        self.access_token = access_token
         self.user = user
         self.pwd = pwd
         self.study_accession = study_accession
         self.group_name = group_name
         self.show_logs = show_logs
         self.debug = debug
 
     @classmethod
     def from_parsed_params(cls, args):
         return cls(
             host=args.host,
             study_accession=args.study_accession,
             group_name=args.group_name,
             token=args.token,
+            access_token=args.access_token,
             user=args.user,
             pwd=args.pwd,
             show_logs=args.show_logs,
             debug=args.debug
         )
```

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/upload_reference_genome.py` & `odm_sdk-1.57.0/odm_sdk/scripts/upload_reference_genome.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/user_setup.py` & `odm_sdk-1.57.0/odm_sdk/scripts/user_setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,19 +51,22 @@
     :type host:  basestring
     :param alias: user alias
     :type alias: basestring
     :return: user
     :rtype: User
     """
     by_token = 'by token'
-    items = [by_token, 'by email and password']
-    use_token = interactive_select(items, 'Select authentication') == by_token
+    by_access_token = 'by access token'
+    items = [by_token, by_access_token, 'by email and password']
+    choice = interactive_select(items, 'Select authentication')
 
-    if use_token:
+    if choice == by_token:
         return create_user_from_token(host, alias=alias)
+    elif choice == by_access_token:
+        return create_user_from_access_token(host, alias=alias)
     else:
         return create_user_from_input_email_and_password(host, alias=alias)
 
 
 def create_user_from_input_email_and_password(host, alias=None):
     """
     Ask email and password, check that it is possible to login with this credentials
@@ -115,15 +118,33 @@
     with_alias = '' if not alias else ' for "%s"' % alias
     msg = msg % with_alias
     while True:
         token = getpass(msg)
         if not token:
             print('Token cannot be empty')
             continue
-        user = User(email=None, host=host, password=None, alias=alias, token=token)
+        user = User(host=host, alias=alias, token=token)
+        try:
+            user.get_connection()
+            break
+        except GenestackAuthenticationException:
+            print('Could not login with given token, please try again')
+    return user
+
+
+def create_user_from_access_token(host, alias=None):
+    print(f'Host: {host}')
+    with_alias = f' for "{alias}"' if alias else ''
+    msg = f'Please specify access token or environment variable with its value{with_alias}: '
+    while True:
+        access_token = input(msg)
+        if not access_token:
+            print('Token cannot be empty')
+            continue
+        user = User(host=host, alias=alias, access_token=access_token)
         try:
             user.get_connection()
             break
         except GenestackAuthenticationException:
             print('Could not login with given token, please try again')
     return user
```

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/users/add_permissions_to_users.py` & `odm_sdk-1.57.0/odm_sdk/scripts/users/add_permissions_to_users.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/users/add_token_to_user.py` & `odm_sdk-1.57.0/odm_sdk/scripts/users/add_token_to_user.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/users/add_users_to_groups.py` & `odm_sdk-1.57.0/odm_sdk/scripts/users/add_users_to_groups.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/users/create_groups.py` & `odm_sdk-1.57.0/odm_sdk/scripts/users/create_groups.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/users/create_users.py` & `odm_sdk-1.57.0/odm_sdk/scripts/users/create_users.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/scripts/utils.py` & `odm_sdk-1.57.0/odm_sdk/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/settings/config.py` & `odm_sdk-1.57.0/odm_sdk/settings/config.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/settings/user.py` & `odm_sdk-1.57.0/odm_sdk/settings/user.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,24 +22,56 @@
         return '%s/frontend/endpoint' % url_stub
 
     raise GenestackAuthenticationException(
         "Could not connect to host '{}', check if it is defined correctly"
         "".format(host))
 
 
+def _read_non_canonical(msg):
+    """
+    An enhanced input method designed to read user inputs that may exceed the standard terminal input buffer size,
+    typically limited to 1024 characters. It is required for interactively reading lengthy inputs such as raw access
+    tokens directly from the user.
+    The function attempts to switch the terminal to non-canonical mode, this mode is only supported on Unix-like
+    systems where the termios module is available.
+    :param msg: The prompt message displayed to the user.
+    :return: The user input, stripped of leading and trailing whitespace.
+    """
+    try:
+        import termios, tty, atexit, sys
+        termios.tcgetattr, termios.tcsetattr
+    except (ImportError, AttributeError):
+        # fallback to standard input on systems that don't support termios
+        return input(msg).strip()
+    fd = sys.stdin.fileno()
+    original_attrs = termios.tcgetattr(fd)
+    # ensure that terminal settings are restored to their original state on program exit
+    atexit.register(lambda: termios.tcsetattr(fd, termios.TCSADRAIN, original_attrs))
+
+    # temporarily switch to non-canonical mode modifying local modes
+    new_attrs = termios.tcgetattr(fd)
+    new_attrs[3] = new_attrs[3] & ~termios.ICANON
+    termios.tcsetattr(fd, termios.TCSADRAIN, new_attrs)
+    try:
+        return input(msg).strip()
+    finally:
+        # restore the original settings
+        termios.tcsetattr(fd, termios.TCSADRAIN, original_attrs)
+
+
 class User(object):
     """
     Class encapsulating all user info required for authentication.
 
     That includes:
      - user alias
      - server URL (or is it hostname?)
      - token *or* email/password pair
     """
-    def __init__(self, email, alias=None, host=None, password=None, token=None):
+    def __init__(self, email=None, alias=None, host=None, password=None, token=None, access_token=None):
         """
         All fields are optional.
         If ``alias`` is None it will be the same as ``email``.
 
         If you login interactively, no ``email`` or ``password`` is required.
         The alias is used to find the matching user in :py:func:`~odm_sdk.get_user`
 
@@ -53,14 +85,15 @@
         :type password: str
         """
         self.host = host
         self.email = email
         self.password = password  # TODO make property
         self.alias = alias or email
         self.token = token
+        self.access_token = access_token
 
     def get_connection(self, interactive=True, debug=False, show_logs=False):
         """
         Return a logged-in connection for current user.
         If ``interactive`` is ``True`` and the password or email are unknown,
         they will be asked in interactive mode.
 
@@ -72,14 +105,16 @@
         :type show_logs: bool
         :return: logged connection
         :rtype: odm_sdk.Connection
         """
         connection = Connection(_get_server_url(self.host), debug=debug, show_logs=show_logs)
         if self.token:
             connection.login_by_token(self.token)
+        elif self.access_token:
+            connection.login_by_access_token(self.access_token)
         elif self.email and self.password:
             connection.login(self.email, self.password)
         elif interactive:
             self.__interactive_login(connection)
         #else:
         #    raise GenestackException('Not enough user data to login')
         return connection
@@ -92,18 +127,19 @@
         if not isatty():
             raise GenestackException("Interactive login is not possible")
 
         email = self.email
         message = 'Connecting to %s' % self.host
 
         login_by_token = 'by token'
+        login_by_access_token = 'by access token'
         login_by_email = 'by email and password'
         login_anonymously = 'anonymously'
 
-        choice = interactive_select([login_by_token, login_by_email, login_anonymously],
+        choice = interactive_select([login_by_token, login_by_access_token, login_by_email, login_anonymously],
                                     'How do you want to login')
 
         if choice == login_anonymously:
             return
 
         while True:
             if message:
@@ -118,14 +154,22 @@
                     connection.login(email, password)
                     self.email = email
                     self.password = password
                     return
                 except GenestackAuthenticationException:
                     message = ('Your username and password have been rejected by %s, '
                                'please try again' % self.host)
+            elif choice == login_by_access_token:
+                access_token = _read_non_canonical('access token or environment variable with its value: ')
+                try:
+                    connection.login_by_access_token(access_token)
+                    self.access_token = access_token
+                    return
+                except GenestackAuthenticationException:
+                    message = 'Your access token has been rejected by %s, please try again' % self.host
             else:
                 token = getpass('token: ')
                 try:
                     connection.login_by_token(token)
                     self.token = token
                     return
                 except GenestackAuthenticationException:
```

### Comparing `odm-sdk-0.0.1/odm_sdk/share_util.py` & `odm_sdk-1.57.0/odm_sdk/share_util.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/shell.py` & `odm_sdk-1.57.0/odm_sdk/shell.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/task_log_viewer.py` & `odm_sdk-1.57.0/odm_sdk/task_log_viewer.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/tests/test_import.py` & `odm_sdk-1.57.0/odm_sdk/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/unaligned_reads.py` & `odm_sdk-1.57.0/odm_sdk/unaligned_reads.py`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/odm_sdk/utils.py` & `odm_sdk-1.57.0/odm_sdk/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,47 +32,52 @@
     except AttributeError:
         return False
 
 
 class GenestackArgumentParser(argparse.ArgumentParser):
     def parse_known_args(self, args=None, namespace=None):
         args, argv = super(GenestackArgumentParser, self).parse_known_args(args, namespace)
-        if args.token and args.user:
-            self.error('Token and user should not be specified together')
+        if sum([bool(args.token), bool(args.user), bool(args.access_token)]) > 1:
+            self.error('Exactly one of token, access_token or user should be specified')
         if args.pwd and not args.user:
             self.error('Password should not be specified without user')
         return args, argv
 
 
-def make_connection_parser(user=None, password=None, host=None, token=None):
+def make_connection_parser(user=None, password=None, host=None, token=None, access_token=None):
     """
     Creates an argument parser with the provided connection parameters.
     If one of ``email``, ``password`` or ``user`` is specified, they are used. Otherwise, the default
     identity from the local config file will be used.
 
     :param user: user alias or email
     :type user: str
     :param password: user password
     :type password: str
     :param host: host
     :type host: str
     :param token: API token string
     :type token: str
+    :param access_token: access token string
+    :type access_token: str
     :return: parser
     :rtype: argparse.ArgumentParser
     """
     parser = GenestackArgumentParser()
     group = parser.add_argument_group('connection')
     group.add_argument('-H', '--host', default=host, help='server host', metavar='<host>')
     group.add_argument('-u', '--user', dest='user', metavar='<user>', default=user,
                        help='user alias from settings or email')
     group.add_argument('-p', '--password', dest='pwd', default=password, metavar='<password>',
                        help='user password')
     group.add_argument('--token', dest='token', default=token, metavar='<api-token>',
                        help='API token to be used instead of the login and password')
+    group.add_argument('--access-token', dest='access_token', default=access_token, metavar='<access-token>',
+                       help='Access token or environment variable with its value to be used instead '
+                            'of the login and password')
     group.add_argument('--debug', dest='debug', action='store_true',
                        help='include server stacktrace into error messages (implies --show-logs)')
     group.add_argument('--show-logs', dest='show_logs', action='store_true',
                        help='print application logs received from server to stdout')
     return parser
 
 
@@ -90,16 +95,17 @@
     from .settings import config, User
 
     if args is None:
         args = make_connection_parser().parse_args()
 
     alias = args.user
     if args.token:
-        return User(email=None, host=args.host, password=None, token=args.token)
-
+        return User(host=args.host, token=args.token)
+    if args.access_token:
+        return User(host=args.host, access_token=args.access_token)
     if not args.host and not args.pwd:
         if not alias and config.default_user:
             return config.default_user
         if alias in config.users:
             return config.users[alias]
     return User(email=alias, host=args.host, password=args.pwd, token=args.token)
```

### Comparing `odm-sdk-0.0.1/odm_sdk.egg-info/PKG-INFO` & `odm_sdk-1.57.0/odm_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: odm-sdk
-Version: 0.0.1
+Version: 1.57.0
 Summary: SDK for interacting with the Open Data Manager
-Home-page: https://github.com/genestack/python-client
+Home-page: https://github.com/genestack/sdk
 Author: Genestack Limited
 Author-email: 
 License: MIT
 Project-URL: Documentation, https://genestack-client.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/genestack/python-client/
 Project-URL: Tracker, https://github.com/genestack/python-client/issues
 Keywords: genestack,odm,import,share,create,delete,curate,genomics,api
@@ -18,13 +18,13 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: keyring==24.3.0
+Requires-Dist: keyring==25.2.0
 Requires-Dist: requests==2.31.0
-Requires-Dist: pyOpenSSL==24.0.0
-Requires-Dist: jsonschema==4.21.1
+Requires-Dist: pyOpenSSL==24.1.0
+Requires-Dist: jsonschema==4.22.0
 Requires-Dist: pyrsistent==0.20.0
-Requires-Dist: odm-api==1.56.1
+Requires-Dist: odm-api==1.57.0
```

### Comparing `odm-sdk-0.0.1/odm_sdk.egg-info/SOURCES.txt` & `odm_sdk-1.57.0/odm_sdk.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -42,18 +42,19 @@
 odm_sdk/scripts/import_ODM_data.py
 odm_sdk/scripts/shell.py
 odm_sdk/scripts/upload_reference_genome.py
 odm_sdk/scripts/user_setup.py
 odm_sdk/scripts/utils.py
 odm_sdk/scripts/dictionaries/__init__.py
 odm_sdk/scripts/dictionaries/load_init_share_dictionaries.py
+odm_sdk/scripts/internal/README.md
 odm_sdk/scripts/internal/__init__.py
-odm_sdk/scripts/internal/generate_dictionaries.py
+odm_sdk/scripts/internal/generate_gene_dictionaries.py
+odm_sdk/scripts/internal/generate_unit_dictionaries.py
 odm_sdk/scripts/internal/upload_dictionaries_with_specific_metainfo.py
-odm_sdk/scripts/internal/upload_gene_dictionary.py
 odm_sdk/scripts/internal/wait_for_host.py
 odm_sdk/scripts/internal/wait_until_ready.py
 odm_sdk/scripts/internal/data/disease_extension.csv
 odm_sdk/scripts/metainfo_templates/__init__.py
 odm_sdk/scripts/metainfo_templates/get_template.py
 odm_sdk/scripts/metainfo_templates/update_template.py
 odm_sdk/scripts/metainfo_templates/importers/__init__.py
@@ -73,13 +74,8 @@
 odm_sdk/scripts/users/add_users_to_groups.py
 odm_sdk/scripts/users/create_groups.py
 odm_sdk/scripts/users/create_users.py
 odm_sdk/settings/__init__.py
 odm_sdk/settings/config.py
 odm_sdk/settings/user.py
 odm_sdk/tests/__init__.py
-odm_sdk/tests/test_import.py
-test/test_arguments.py
-test/test_connection.py
-test/test_differential_expression.py
-test/test_file_filters.py
-test/test_metainfo.py
+odm_sdk/tests/test_import.py
```

### Comparing `odm-sdk-0.0.1/odm_sdk.egg-info/entry_points.txt` & `odm_sdk-1.57.0/odm_sdk.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `odm-sdk-0.0.1/setup.py` & `odm_sdk-1.57.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 exec(open('odm_sdk/version.py').read())
 
 setup(
     name='odm-sdk',
     install_requires=required + required_internal,
     version=__version__,
     packages=find_packages(),
-    url='https://github.com/genestack/python-client',
+    url='https://github.com/genestack/sdk',
     license='MIT',
     author='Genestack Limited',
     author_email='',
     description='SDK for interacting with the Open Data Manager',
     long_description=__doc__,
     long_description_content_type="text/markdown",
     keywords=['genestack', 'odm', 'import', 'share', 'create',
```

