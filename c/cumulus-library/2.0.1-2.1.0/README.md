# Comparing `tmp/cumulus_library-2.0.1.tar.gz` & `tmp/cumulus_library-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-2.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-2.0.1.tar` & `cumulus_library-2.1.0.tar`

### file list

```diff
@@ -1,100 +1,109 @@
-lrwxr-xr-x   0        0        0        0 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/.sqlfluff -> cumulus_library/.sqlfluff
--rw-r--r--   0        0        0      689 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/README.md
--rw-r--r--   0        0        0     6677 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0       46 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/__init__.py
--rw-r--r--   0        0        0     4837 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/base_table_builder.py
--rw-r--r--   0        0        0     2898 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/base_utils.py
--rwxr-xr-x   0        0        0    17396 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/cli.py
--rw-r--r--   0        0        0     7923 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/cli_parser.py
--rw-r--r--   0        0        0    15082 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/databases.py
--rw-r--r--   0        0        0      422 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/enums.py
--rw-r--r--   0        0        0      523 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/errors.py
--rw-r--r--   0        0        0      205 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/module_allowlist.json
--rw-r--r--   0        0        0     2311 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/parsers/fhir_valueset.py
--rw-r--r--   0        0        0     1716 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/protected_table_builder.py
--rw-r--r--   0        0        0        0 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4731 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     3364 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     6024 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0    10730 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/counts.py
--rw-r--r--   0        0        0    14371 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/psm.py
--rw-r--r--   0        0        0     5136 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/psm.sql
--rw-r--r--   0        0        0     7541 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/count.sql.jinja
--rw-r--r--   0        0        0     2311 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/counts_templates.py
--rw-r--r--   0        0        0     1606 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja
--rw-r--r--   0        0        0      363 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/psm_distinct_ids.sql.jinja
--rw-r--r--   0        0        0     3272 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/psm_templates.py
--rw-r--r--   0        0        0     2943 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_condition.py
--rw-r--r--   0        0        0     2710 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_documentreference.py
--rw-r--r--   0        0        0     4776 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_encounter.py
--rw-r--r--   0        0        0     4731 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_medication.py
--rw-r--r--   0        0        0     2241 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_medicationrequest.py
--rw-r--r--   0        0        0     2734 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_observation.py
--rw-r--r--   0        0        0     2039 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_patient.py
--rw-r--r--   0        0        0      867 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/builder_prereq_tables.py
--rw-r--r--   0        0        0     2555 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/completion_utils.jinja
--rw-r--r--   0        0        0     2548 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/condition.sql.jinja
--rw-r--r--   0        0        0      854 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/core_templates.py
--rw-r--r--   0        0        0     5042 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/core_utils.jinja
--rw-r--r--   0        0        0     2782 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/documentreference.sql.jinja
--rw-r--r--   0        0        0     4718 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/encounter.sql.jinja
--rw-r--r--   0        0        0      274 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/incomplete_encounter.sql.jinja
--rw-r--r--   0        0        0     5984 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/medication.sql.jinja
--rw-r--r--   0        0        0     2058 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja
--rw-r--r--   0        0        0     3331 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/observation.sql.jinja
--rw-r--r--   0        0        0     1854 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/patient.sql.jinja
--rw-r--r--   0        0        0     5350 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/count_core.py
--rw-r--r--   0        0        0      948 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/fhir_lookup_tables.sql
--rw-r--r--   0        0        0     4879 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/fhir_mapping_tables.sql
--rw-r--r--   0        0        0      971 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     1163 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/observation_type.sql
--rw-r--r--   0        0        0     7810 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_condition.sql
--rw-r--r--   0        0        0     5213 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_documentreference.sql
--rw-r--r--   0        0        0    20656 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_encounter.sql
--rw-r--r--   0        0        0     1243 2024-04-16 16:14:11.613901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_medication.sql
--rw-r--r--   0        0        0     3286 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_medicationrequest.sql
--rw-r--r--   0        0        0     6190 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_observation.sql
--rw-r--r--   0        0        0     8678 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_patient.sql
--rw-r--r--   0        0        0     8008 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql
--rw-r--r--   0        0        0    29070 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/count_core.sql
--rw-r--r--   0        0        0     1440 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     2058 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0       69 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/core/version.sql
--rw-r--r--   0        0        0     2580 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/discovery/code_definitions.py
--rw-r--r--   0        0        0     2553 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/discovery/code_detection.py
--rw-r--r--   0        0        0     1978 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja
--rw-r--r--   0        0        0     1618 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py
--rw-r--r--   0        0        0      160 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/discovery/manifest.toml
--rw-r--r--   0        0        0     4622 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/discovery/reference_sql/code_detection.sql
--rw-r--r--   0        0        0      863 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     2312 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1142 2024-04-16 16:14:11.617901 cumulus_library-2.0.1/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0 10584966 2024-04-16 16:14:11.645901 cumulus_library-2.0.1/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv
--rw-r--r--   0        0        0 35303095 2024-04-16 16:14:11.729900 cumulus_library-2.0.1/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv
--rw-r--r--   0        0        0  1708185 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv
--rw-r--r--   0        0        0      410 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      145 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0     3227 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    31623 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/study_parser.py
--rw-r--r--   0        0        0       79 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/alias_table.sql.jinja
--rw-r--r--   0        0        0    11473 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/base_templates.py
--rw-r--r--   0        0        0     2532 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
--rw-r--r--   0        0        0     1893 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/coding_denormalize.sql.jinja
--rw-r--r--   0        0        0      385 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/column_datatype.sql.jinja
--rw-r--r--   0        0        0      563 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/create_view_as.sql.jinja
--rw-r--r--   0        0        0      586 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0      506 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/ctas_empty.sql.jinja
--rw-r--r--   0        0        0       61 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0     2534 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/extension_denormalize.sql.jinja
--rw-r--r--   0        0        0      535 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0      439 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/is_table_not_empty.sql.jinja
--rw-r--r--   0        0        0       34 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/select_all.sql.jinja
--rw-r--r--   0        0        0      370 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/shared_macros/syntax.sql.jinja
--rw-r--r--   0        0        0      169 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0      163 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0    10628 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/template_sql/sql_utils.py
--rw-r--r--   0        0        0     3308 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/cumulus_library/upload.py
--rw-r--r--   0        0        0     2316 2024-04-16 16:14:11.737900 cumulus_library-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 cumulus_library-2.0.1/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      689 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/README.md
+-rw-r--r--   0        0        0     7061 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0       46 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/apis/__init__.py
+-rw-r--r--   0        0        0     6322 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/apis/umls.py
+-rw-r--r--   0        0        0     4837 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/base_table_builder.py
+-rw-r--r--   0        0        0     3892 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/base_utils.py
+-rwxr-xr-x   0        0        0    18237 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/cli.py
+-rw-r--r--   0        0        0     8187 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/cli_parser.py
+-rw-r--r--   0        0        0    20782 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/databases.py
+-rw-r--r--   0        0        0      249 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/db_config.py
+-rw-r--r--   0        0        0      422 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/enums.py
+-rw-r--r--   0        0        0      665 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/errors.py
+-rw-r--r--   0        0        0      205 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0     2311 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/parsers/fhir_valueset.py
+-rw-r--r--   0        0        0     1716 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/protected_table_builder.py
+-rw-r--r--   0        0        0        0 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4731 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3364 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     6024 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0    10732 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/counts.py
+-rw-r--r--   0        0        0    14453 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/psm.py
+-rw-r--r--   0        0        0     5136 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/psm.sql
+-rw-r--r--   0        0        0     7541 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/count.sql.jinja
+-rw-r--r--   0        0        0     2311 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/counts_templates.py
+-rw-r--r--   0        0        0     1606 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja
+-rw-r--r--   0        0        0      363 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/psm_distinct_ids.sql.jinja
+-rw-r--r--   0        0        0     3272 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/psm_templates.py
+-rw-r--r--   0        0        0     3603 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_condition.py
+-rw-r--r--   0        0        0     2789 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_documentreference.py
+-rw-r--r--   0        0        0     4676 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_encounter.py
+-rw-r--r--   0        0        0     2422 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_medication.py
+-rw-r--r--   0        0        0     1853 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_medicationrequest.py
+-rw-r--r--   0        0        0     3772 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_observation.py
+-rw-r--r--   0        0        0     3098 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_patient.py
+-rw-r--r--   0        0        0      867 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_prereq_tables.py
+-rw-r--r--   0        0        0     2555 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/completion_utils.jinja
+-rw-r--r--   0        0        0     2400 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/condition.sql.jinja
+-rw-r--r--   0        0        0      418 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/core_templates.py
+-rw-r--r--   0        0        0     4999 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/core_utils.jinja
+-rw-r--r--   0        0        0     2829 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/documentreference.sql.jinja
+-rw-r--r--   0        0        0     4804 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/encounter.sql.jinja
+-rw-r--r--   0        0        0      274 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/incomplete_encounter.sql.jinja
+-rw-r--r--   0        0        0     2841 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/medication.sql.jinja
+-rw-r--r--   0        0        0     2422 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja
+-rw-r--r--   0        0        0     3324 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/observation.sql.jinja
+-rw-r--r--   0        0        0     2081 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/observation_component_valuequantity.sql.jinja
+-rw-r--r--   0        0        0     1854 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/patient.sql.jinja
+-rw-r--r--   0        0        0     5350 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/count_core.py
+-rw-r--r--   0        0        0      948 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/fhir_lookup_tables.sql
+-rw-r--r--   0        0        0     4879 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/fhir_mapping_tables.sql
+-rw-r--r--   0        0        0      971 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1744 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/observation_type.sql
+-rw-r--r--   0        0        0    12183 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_condition.sql
+-rw-r--r--   0        0        0     5610 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_documentreference.sql
+-rw-r--r--   0        0        0    21826 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_encounter.sql
+-rw-r--r--   0        0        0     3949 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_medication.sql
+-rw-r--r--   0        0        0     3017 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_medicationrequest.sql
+-rw-r--r--   0        0        0    11183 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_observation.sql
+-rw-r--r--   0        0        0     7061 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_patient.sql
+-rw-r--r--   0        0        0     8008 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql
+-rw-r--r--   0        0        0    29070 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/count_core.sql
+-rw-r--r--   0        0        0     1440 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     2058 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0       69 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/version.sql
+-rw-r--r--   0        0        0     2743 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/discovery/code_definitions.py
+-rw-r--r--   0        0        0     2762 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/discovery/code_detection.py
+-rw-r--r--   0        0        0     1978 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja
+-rw-r--r--   0        0        0     1618 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py
+-rw-r--r--   0        0        0      160 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/discovery/manifest.toml
+-rw-r--r--   0        0        0     4622 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/discovery/reference_sql/code_detection.sql
+-rw-r--r--   0        0        0      863 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     2312 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1142 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0       14 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/vocab/.gitignore
+-rw-r--r--   0        0        0      253 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/vocab/README.MD
+-rw-r--r--   0        0        0 10584966 2024-05-09 13:20:56.661008 cumulus_library-2.1.0/cumulus_library/studies/vocab/icd/ICD10CM_2023AA.bsv
+-rw-r--r--   0        0        0 35303095 2024-05-09 13:20:56.745009 cumulus_library-2.1.0/cumulus_library/studies/vocab/icd/ICD10PCS_2023AA.bsv
+-rw-r--r--   0        0        0  1708185 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/studies/vocab/icd/ICD9CM_2023AA.bsv
+-rw-r--r--   0        0        0      410 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      269 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0      681 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/studies/vocab/reference_sql/vocab_icd_builder.sql
+-rw-r--r--   0        0        0     2366 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    32529 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0       79 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/alias_table.sql.jinja
+-rw-r--r--   0        0        0    13075 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/base_templates.py
+-rw-r--r--   0        0        0     4423 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
+-rw-r--r--   0        0        0     1893 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/coding_denormalize.sql.jinja
+-rw-r--r--   0        0        0      385 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/column_datatype.sql.jinja
+-rw-r--r--   0        0        0      563 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/create_view_as.sql.jinja
+-rw-r--r--   0        0        0      586 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0      544 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/ctas_empty.sql.jinja
+-rw-r--r--   0        0        0      954 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/ctas_from_parquet.sql.jinja
+-rw-r--r--   0        0        0       61 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     2528 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      535 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0      439 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/is_table_not_empty.sql.jinja
+-rw-r--r--   0        0        0       34 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/select_all.sql.jinja
+-rw-r--r--   0        0        0      370 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/shared_macros/syntax.sql.jinja
+-rw-r--r--   0        0        0     1108 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/shared_macros/unnest_utils.jinja
+-rw-r--r--   0        0        0      169 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0      163 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0    12401 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/sql_utils.py
+-rw-r--r--   0        0        0     3261 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/upload.py
+-rw-r--r--   0        0        0     2313 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 cumulus_library-2.1.0/PKG-INFO
```

### Comparing `cumulus_library-2.0.1/README.md` & `cumulus_library-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/.sqlfluff` & `cumulus_library-2.1.0/cumulus_library/.sqlfluff`

 * *Files 14% similar despite different names*

```diff
@@ -57,51 +57,50 @@
             "has_data": False
         }
     ]
 column_name = 'bar'
 column_names = ['foo', 'bar']
 conditions = ["1 > 0", "1 < 2"]
 column_hierarchy = [('a', list),('b',dict)]
-config = 
-    {
-        "medication_datasources" : {
-            "by_contained_ref" : True, 
-            "by_external_ref" : True
-        }, 
-        'has_userselected': False
-    }
 count_ref = count_ref
 count_table = count_table
 dataset = 
     [
         ["foo","foo"],
         ["bar","bar"]
     ]
+db_type = duckdb
 dependent_variable = is_flu
 ext_systems = ["omb", "text"]
+extra_alias_done = True
+extra_field = ("field", "alias")
+extra_fields = [("field", "alias")]
 field = 'column_name'
+field_alias = 'field'
 filter_table = filter_table
 filter_resource = True
 fhir_extension = condition
 fhir_resource = patient
 id = 'id'
 join_cols_by_table = 
     { 
         "join_table": { 
             "join_id": "enc_ref",
             "included_cols": [["a"], ["b", "c"]]
         }
     }
 join_id = subject_ref
+local_location = /var/study/data/
 neg_source_table = neg_source_table
 output_table_name = 'created_table'
 parent_field = 'parent'
 prefix = Test
 primary_ref = encounter_ref
 pos_source_table = pos_source_table
+remote_location = s3://bucket/study/data/
 schema_name = test_schema
 schema = 
     {
         'condition': {
             'category': {
                 'coding': True, 'code': True, 'display': True, 'system': True, 'userSelected': True, 'version': True, 'text': True
             },
@@ -153,27 +152,38 @@
         'medicationrequest': {
             'id': True, 
             'status': True, 
             'intent': True, 
             'authoredOn': True, 
             'category': {
                 'code': True, 'system': True, 'display': False
-            }, 
+            },
+            'dosageInstruction': {
+                'text': True,
+            },
+            'medicationReference': {
+                'reference': True
+            },
             'subject': {
                 'reference': True
             }, 
             'encounter': {
                 'reference': True
             }
         }, 
         'observation': {
             'id': True, 
             'category': {
                 'coding': True, 'code': True, 'display': True, 'system': True, 'text': True
             },
+            'component': {
+                'valueQuantity': {
+                    'code': True, 'comparator': True, 'system': True, 'unit': True, 'value': True
+                },
+            },
             'status': True,
             'code': {
                 'coding': True, 'code': True, 'display': True, 'system': True, 'text': True
             }, 
             'interpretation': {
                 'coding': True, 'code': True, 'display': True, 'system': True, 'text': True
             }, 
@@ -189,15 +199,15 @@
             }, 
             'subject': {
                 'reference': True
             }, 
             'encounter': {
                 'reference': True
             }
-        }, 
+        },
         'patient': {
             'id': True, 
             'gender': True, 
             'address': True, 
             'birthdate': True
         }
     }
```

### Comparing `cumulus_library-2.0.1/cumulus_library/base_table_builder.py` & `cumulus_library-2.1.0/cumulus_library/base_table_builder.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/cli.py` & `cumulus_library-2.1.0/cumulus_library/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import json
 import os
 import pathlib
 import sys
 import sysconfig
 
+import requests
 import rich
 
 from cumulus_library import (
     __version__,
     base_utils,
     cli_parser,
     databases,
@@ -98,103 +99,114 @@
                     stats_clean=stats_clean,
                 )
 
     def clean_and_build_study(
         self,
         target: pathlib.Path,
         *,
-        stats_build: bool,
+        config: base_utils.StudyConfig,
         continue_from: str | None = None,
     ) -> None:
         """Recreates study views/tables
 
         :param target: A path to the study directory
-        :param stats_build: if True, forces creation of new stats tables
+        :param config: A StudyConfig object containing optional params
         :keyword continue_from: Restart a run from a specific sql file (for dev only)
         """
         studyparser = study_parser.StudyManifestParser(target, self.data_path)
         try:
             if not continue_from:
                 studyparser.run_protected_table_builder(
-                    self.cursor, self.schema_name, verbose=self.verbose
+                    self.cursor, self.schema_name, verbose=self.verbose, config=config
                 )
                 self.update_transactions(studyparser.get_study_prefix(), "started")
                 cleaned_tables = studyparser.clean_study(
                     self.cursor,
                     self.schema_name,
                     verbose=self.verbose,
                     stats_clean=False,
                 )
                 # If the study hasn't been created before, force stats table generation
                 if len(cleaned_tables) == 0:
-                    stats_build = True
+                    config.stats_build = True
                 studyparser.run_table_builder(
                     self.cursor,
                     self.schema_name,
                     verbose=self.verbose,
                     parser=self.db.parser(),
+                    config=config,
                 )
             else:
                 self.update_transactions(studyparser.get_study_prefix(), "resumed")
 
-            studyparser.build_study(self.cursor, self.verbose, continue_from)
+            studyparser.build_study(
+                self.cursor,
+                verbose=self.verbose,
+                continue_from=continue_from,
+                config=config,
+            )
             studyparser.run_counts_builders(
-                self.cursor, self.schema_name, verbose=self.verbose
+                self.cursor, self.schema_name, verbose=self.verbose, config=config
             )
             studyparser.run_statistics_builders(
                 self.cursor,
                 self.schema_name,
                 verbose=self.verbose,
-                stats_build=stats_build,
+                config=config,
             )
             self.update_transactions(studyparser.get_study_prefix(), "finished")
 
         except errors.StudyManifestFilesystemError as e:
             # This should be thrown prior to any database connections, so
             # skipping logging
             raise e
         except Exception as e:
             self.update_transactions(studyparser.get_study_prefix(), "error")
             raise e
 
     def run_matching_table_builder(
-        self, target: pathlib.Path, table_builder_name: str
+        self,
+        target: pathlib.Path,
+        table_builder_name: str,
+        config: base_utils.StudyConfig,
     ) -> None:
         """Runs a single table builder
 
         :param target: A path to the study directory
         :param table_builder_name: a builder file referenced in the study's manifest
+        :param config: A StudyConfig object containing optional params
         """
         studyparser = study_parser.StudyManifestParser(target)
         studyparser.run_matching_table_builder(
             self.cursor,
             self.schema_name,
             table_builder_name,
             self.verbose,
             parser=self.db.parser(),
+            config=config,
         )
 
-    def clean_and_build_all(self, study_dict: dict, stats_build: bool) -> None:
-        """Builds views for all studies.
+    def clean_and_build_all(
+        self, study_dict: dict, config: base_utils.StudyConfig
+    ) -> None:
+        """Builds tables for all studies.
 
         NOTE: By design, this method will always exclude the `template` study dir,
         since 99% of the time you don't need a live copy in the database.
 
         :param study_dict: A dict of paths
-        :param stats_build: if True, regen stats tables
+        :param config: A StudyConfig object containing optional params
         """
         study_dict = dict(study_dict)
         study_dict.pop("template")
         for precursor_study in ["vocab", "core"]:
-            self.clean_and_build_study(
-                study_dict[precursor_study], stats_build=stats_build
-            )
+            self.clean_and_build_study(study_dict[precursor_study], config=config)
             study_dict.pop(precursor_study)
         for key in study_dict:
-            self.clean_and_build_study(study_dict[key], stats_build=stats_build)
+            self.clean_and_build_study(study_dict[key], config=config)
 
     ### Data exporters
     def export_study(
         self, target: pathlib.Path, data_path: pathlib.Path, archive: bool
     ) -> None:
         """Exports aggregates defined in a manifest
 
@@ -207,28 +219,34 @@
 
     def export_all(self, study_dict: dict, data_path: pathlib.Path, archive: bool):
         """Exports all defined count tables to disk"""
         for key in study_dict.keys():
             self.export_study(study_dict[key], data_path, archive)
 
     def generate_study_sql(
-        self, target: pathlib.Path, builder: str | None = None
+        self,
+        target: pathlib.Path,
+        *,
+        config: base_utils.StudyConfig,
+        builder: str | None = None,
     ) -> None:
         """Materializes study sql from templates
 
         :param target: A path to the study directory
+        :param config: A StudyConfig object containing optional params
         :param builder: Specify a single builder to generate sql from
         """
         studyparser = study_parser.StudyManifestParser(target)
         studyparser.run_generate_sql(
             cursor=self.cursor,
             schema=self.schema_name,
             builder=builder,
             verbose=self.verbose,
             parser=self.db.parser(),
+            config=config,
         )
 
     def generate_study_markdown(
         self,
         target: pathlib.Path,
     ) -> None:
         """Materializes study sql from templates
@@ -314,21 +332,30 @@
 def run_cli(args: dict):
     """Controls which library tasks are run based on CLI arguments"""
     console = rich.console.Console()
     if args["action"] == "create":
         create_template(args["create_dir"])
 
     elif args["action"] == "upload":
-        upload.upload_files(args)
+        try:
+            upload.upload_files(args)
+        except requests.RequestException as e:
+            print(str(e))
+            sys.exit()
 
     # all other actions require connecting to the database
     else:
-        db_backend = databases.create_db_backend(args)
+        config = base_utils.StudyConfig(
+            db=databases.create_db_backend(args),
+            force_upload=args.get("replace_existing", False),
+            stats_build=args.get("stats_build", False),
+            umls_key=args.get("umls"),
+        )
         try:
-            runner = StudyRunner(db_backend, data_path=args.get("data_path"))
+            runner = StudyRunner(config.db, data_path=args.get("data_path"))
             if args.get("verbose"):
                 runner.verbose = True
             console.print("[italic] Connecting to database...")
             runner.cursor.execute("SHOW DATABASES")
             study_dict = get_study_dict(args["study_dir"])
             if "prefix" not in args.keys():
                 if args["target"]:
@@ -345,26 +372,25 @@
                     args["target"],
                     study_dict,
                     stats_clean=args["stats_clean"],
                     prefix=args["prefix"],
                 )
             elif args["action"] == "build":
                 if "all" in args["target"]:
-                    runner.clean_and_build_all(study_dict, args["stats_build"])
+                    runner.clean_and_build_all(study_dict, config=config)
                 else:
                     for target in args["target"]:
                         if args["builder"]:
                             runner.run_matching_table_builder(
-                                study_dict[target], args["builder"]
+                                study_dict[target], config=config
                             )
                         else:
                             runner.clean_and_build_study(
                                 study_dict[target],
-                                stats_build=args["stats_build"],
-                                continue_from=args["continue_from"],
+                                config=config,
                             )
 
             elif args["action"] == "export":
                 if args["archive"]:
                     warning_text = (
                         "🚨[bold red] This will export all study tables [/bold red]🚨"
                         "\n\nDepending on your study definition, this data may contain "
@@ -385,21 +411,23 @@
                     for target in args["target"]:
                         runner.export_study(
                             study_dict[target], args["data_path"], args["archive"]
                         )
 
             elif args["action"] == "generate-sql":
                 for target in args["target"]:
-                    runner.generate_study_sql(study_dict[target], args["builder"])
+                    runner.generate_study_sql(
+                        study_dict[target], builder=args["builder"], config=config
+                    )
 
             elif args["action"] == "generate-md":
                 for target in args["target"]:
                     runner.generate_study_markdown(study_dict[target])
         finally:
-            db_backend.close()
+            config.db.close()
 
 
 def main(cli_args=None):
     """Reads CLI input/environment variables and invokes library calls"""
 
     parser = cli_parser.get_parser()
     args = vars(parser.parse_args(cli_args))
@@ -412,25 +440,26 @@
     if args.get("target"):
         for target in args["target"]:
             if target == "all":
                 args["target"] = ["all"]
                 break
 
     arg_env_pairs = (
+        ("data_path", "CUMULUS_LIBRARY_DATA_PATH"),
         ("db_type", "CUMULUS_LIBRARY_DB_TYPE"),
+        ("id", "CUMULUS_AGGREGATOR_ID"),
+        ("load_ndjson_dir", "CUMULUS_LIBRARY_LOAD_NDJSON_DIR"),
         ("profile", "CUMULUS_LIBRARY_PROFILE"),
-        ("schema_name", "CUMULUS_LIBRARY_DATABASE"),
-        ("workgroup", "CUMULUS_LIBRARY_WORKGROUP"),
         ("region", "CUMULUS_LIBRARY_REGION"),
+        ("schema_name", "CUMULUS_LIBRARY_DATABASE"),
         ("study_dir", "CUMULUS_LIBRARY_STUDY_DIR"),
-        ("data_path", "CUMULUS_LIBRARY_DATA_PATH"),
-        ("load_ndjson_dir", "CUMULUS_LIBRARY_LOAD_NDJSON_DIR"),
-        ("user", "CUMULUS_AGGREGATOR_USER"),
-        ("id", "CUMULUS_AGGREGATOR_ID"),
+        ("umls", "UMLS_API_KEY"),
         ("url", "CUMULUS_AGGREGATOR_URL"),
+        ("user", "CUMULUS_AGGREGATOR_USER"),
+        ("workgroup", "CUMULUS_LIBRARY_WORKGROUP"),
     )
     read_env_vars = []
     for pair in arg_env_pairs:
         if env_val := os.environ.get(pair[1]):
             if pair[0] == "study_dir":
                 args[pair[0]] = [env_val]
             else:
```

### Comparing `cumulus_library-2.0.1/cumulus_library/cli_parser.py` & `cumulus_library-2.1.0/cumulus_library/cli_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -179,14 +179,23 @@
         help=(
             "Force regenerating statistics data from latest dataset. "
             "Stats are created by default when study is initially run"
         ),
         dest="stats_build",
     )
     build.add_argument(
+        "--umls-key",
+        help="An API Key for the UMLS API",
+    )
+    build.add_argument(
+        "--force-upload",
+        action="store_true",
+        help="Forces file downloads/uploads to occur, even if they already exist",
+    )
+    build.add_argument(
         "--continue",
         dest="continue_from",
         help=argparse.SUPPRESS,
     )
 
     # Database export
```

### Comparing `cumulus_library-2.0.1/cumulus_library/databases.py` & `cumulus_library-2.1.0/cumulus_library/databases.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,26 +8,30 @@
 wrapper method in one of DatabaseCursor or DatabaseBackend.
 """
 
 import abc
 import datetime
 import json
 import os
+import pathlib
 import sys
 from pathlib import Path
-from typing import Protocol
+from typing import Any, Protocol
 
+import boto3
 import cumulus_fhir_support
 import duckdb
 import pandas
 import pyarrow
 import pyathena
 from pyathena.common import BaseCursor as AthenaCursor
 from pyathena.pandas.cursor import PandasCursor as AthenaPandasCursor
 
+from cumulus_library import db_config, errors
+
 
 class DatabaseCursor(Protocol):
     """Protocol for a PEP-249 compatible cursor"""
 
     def execute(self, sql: str) -> None:
         pass
 
@@ -40,79 +44,101 @@
     def fetchall(self) -> list[list] | None:
         pass
 
 
 class DatabaseParser(abc.ABC):
     """Parses information_schema results from a database"""
 
-    def _parse_found_schema(
-        self, expected: dict[dict[list]], schema: dict[list]
-    ) -> dict:
-        """Checks for presence of field for each column in a table
+    @abc.abstractmethod
+    def parse_found_schema(self, schema: dict[str, str]) -> dict:
+        """Parses a database-provided schema string.
 
-        :param expected: A nested dict describing the expected data format of
-        a table. Expected format is like this:
+        :param schema: the results of a query from the get_column_datatype method
+        of the template_sql.templates function. It looks like this (for athena at
+        least, but the values are opaque strings and database-provider-specific):
             {
-                "object_col":["member_a", "member_b"]
-                "primitive_col": []
+                'object_col': 'row(member_a varchar, member_b date)',
+                'primitive_col': 'varchar',
             }
-        :param schema: the results of a query from the get_column_datatype method
-        of the template_sql.templates function. It looks like this:
-            [
-                ('object_col', 'row(member_a VARCHAR, member_b DATE)'),
-                ('primitive_col', 'VARCHAR')
-            ]
-
-        The actual contents of schema are database dependent. This naive method
-        is a first pass, ignoring complexities of differing database variable
-        types, just iterating through looking for column names.
 
-        TODO: on a per database instance, consider a more nuanced approach if needed
-              (compared to just checking if the schema contains the field name)
+        :returns: a dictionary with an entry for every field present in the schema.
+        For the above example, this should return:
+            {
+                'object_col': {
+                    'member_a': {},
+                    'member_b': {},
+                },
+                'primitive_col': {},
+            }
         """
+
+    def _recursively_validate(
+        self, expected: dict[str, Any], schema: dict[str, Any]
+    ) -> dict[str, Any]:
+        schema = schema or {}
         output = {}
 
         for column, fields in expected.items():
-            column_lower = column.lower()
+            col_schema = schema.get(column.lower())
 
-            # is this an object column? (like: "subject": ["reference"])
-            if fields:
-                col_schema = schema.get(column_lower, "").lower()
-                output[column] = {
-                    # TODO: make this check more robust
-                    field: field.lower() in col_schema
-                    for field in fields
-                }
+            # Is `fields` an falsy? (like: "recordedDate": None or [] or {})
+            # This means we just want to check existance of `column`
+            # otherwise this is a primitive col
+            if not fields:
+                output[column] = col_schema is not None
+
+            # Is `fields` a list? (like: "subject": ["reference"])
+            # This means we should check existance of all mentioned children.
+            elif isinstance(fields, list):
+                for field in fields:
+                    subschema = self._recursively_validate({field: None}, col_schema)
+                    output.setdefault(column, {}).update(subschema)
+
+            # Is `fields` a dict?
+            # Like: "component": {"valueQuantity": ["unit", "value"]}
+            # This means we should descend one level
+            elif isinstance(fields, dict):
+                subschema = self._recursively_validate(fields, col_schema)
+                output[column] = subschema
 
-            # otherwise this is a primitive col (like: "recordedDate": None)
             else:
-                output[column] = column_lower in schema
+                raise ValueError("Bad expected schema provided")
 
         return output
 
-    @abc.abstractmethod
     def validate_table_schema(
-        self, expected: dict[str, list[str]], schema: list[tuple]
+        self, expected: dict[str, list], schema: list[tuple]
     ) -> dict:
         """Public interface for investigating if fields are in a table schema.
 
+        expected is a dictionary of string column names to *something*:
+        - falsy (like None or []): just check that the column exists
+        - list of strings: check all the column children exist
+        - dict of a new child 'expected' dictionary, with same above rules
+
         This method should lightly format results and pass them to
-        _parse_found_schema(), or a more bespoke table analysis function if needed.
+        parse_found_schema(), or a more bespoke table analysis function if needed.
         """
+        parsed_schema = self.parse_found_schema(dict(schema))
+        return self._recursively_validate(expected, parsed_schema)
 
 
 class DatabaseBackend(abc.ABC):
     """A generic database backend, supporting basic cursor operations"""
 
     def __init__(self, schema_name: str):
         """Create connection to a database backend
 
         :param schema_name: the database name ('schema' is Athena-speak for a database)
         """
         self.schema_name = schema_name
+        # db_type, while perhaps feeling redundant, is intended to be a value that is
+        # passed to jinja templates for creating valid sql for a particular database's
+        # technology
+        self.db_type = None
 
     @abc.abstractmethod
     def cursor(self) -> DatabaseCursor:
         """Returns a connection to the backing database"""
 
     @abc.abstractmethod
     def pandas_cursor(self) -> DatabaseCursor:
@@ -126,75 +152,187 @@
     def execute_as_pandas(self, sql: str) -> pandas.DataFrame:
         """Returns a pandas.DataFrame version of the results from the provided SQL"""
 
     @abc.abstractmethod
     def parser(self) -> DatabaseParser:
         """Returns parser object for interrogating DB schemas"""
 
+    def upload_file(
+        self,
+        *,
+        file: pathlib.Path,
+        study: str,
+        topic: str,
+        remote_filename: str | None = None,
+        force_upload=False,
+    ) -> str | None:
+        """Handler for remote database file upload.
+
+        By default, this should return None. Only override this for databases that
+        have an API for file upload (i.e. cloud databases)"""
+        return None
+
     @abc.abstractmethod
     def close(self) -> None:
         """Clean up any resources necessary"""
 
 
 class AthenaDatabaseBackend(DatabaseBackend):
     """Database backend that can talk to AWS Athena"""
 
-    def __init__(self, region: str, workgroup: str, profile: str, schema_name: str):
+    def __init__(self, region: str, work_group: str, profile: str, schema_name: str):
         super().__init__(schema_name)
 
+        self.db_type = "athena"
+        self.region = region
+        self.work_group = work_group
+        self.profile = profile
+        self.schema_name = schema_name
+        # the profile may not be required, provided the above three AWS env vars
+        # are set. If both are present, the env vars take precedence
         connect_kwargs = {}
+        if self.profile is not None:
+            connect_kwargs["profile_name"] = self.profile
+
         for aws_env_name in [
             "AWS_ACCESS_KEY_ID",
             "AWS_SECRET_ACCESS_KEY",
             "AWS_SESSION_TOKEN",
         ]:
             if aws_env_val := os.environ.get(aws_env_name):
                 connect_kwargs[aws_env_name.lower()] = aws_env_val
-        # the profile may not be required, provided the above three AWS env vars
-        # are set. If both are present, the env vars take precedence
-        if profile is not None:
-            connect_kwargs["profile_name"] = profile
-
         self.connection = pyathena.connect(
-            region_name=region,
-            work_group=workgroup,
+            region_name=self.region,
+            work_group=self.work_group,
             schema_name=self.schema_name,
             **connect_kwargs,
         )
-        self.pandas_cursor = self.connection.cursor(cursor=AthenaPandasCursor)
 
     def cursor(self) -> AthenaCursor:
         return self.connection.cursor()
 
     def pandas_cursor(self) -> AthenaPandasCursor:
-        return self.pandas_cursor
+        return self.connection.cursor(cursor=AthenaPandasCursor)
 
     def execute_as_pandas(self, sql: str) -> pandas.DataFrame:
-        return self.pandas_cursor.execute(sql).as_pandas()
+        return self.pandas_cursor().execute(sql).as_pandas()
 
     def parser(self) -> DatabaseParser:
         return AthenaParser()
 
+    def upload_file(
+        self,
+        *,
+        file: pathlib.Path,
+        study: str,
+        topic: str,
+        remote_filename: str | None = None,
+        force_upload=False,
+    ) -> str | None:
+        # We'll investigate the connection to get the relevant S3 upload path.
+        wg_conf = self.connection._client.get_work_group(WorkGroup=self.work_group)[
+            "WorkGroup"
+        ]["Configuration"]["ResultConfiguration"]
+        s3_path = wg_conf["OutputLocation"]
+        bucket = "/".join(s3_path.split("/")[2:3])
+        key_prefix = "/".join(s3_path.split("/")[3:])
+        encryption_type = wg_conf.get("EncryptionConfiguration", {}).get(
+            "EncryptionOption", {}
+        )
+        if encryption_type != "SSE_KMS":
+            raise errors.AWSError(
+                f"Bucket {bucket} has unexpected encryption type {encryption_type}."
+                "AWS KMS encryption is expected for Cumulus buckets"
+            )
+        kms_arn = wg_conf.get("EncryptionConfiguration", {}).get("KmsKey", None)
+        s3_key = (
+            f"{key_prefix}cumulus_user_uploads/{self.schema_name}/" f"{study}/{topic}"
+        )
+        if not remote_filename:
+            remote_filename = file
+
+        session = boto3.Session(profile_name=self.connection.profile_name)
+        s3_client = session.client("s3")
+        if not force_upload:
+            res = s3_client.list_objects_v2(
+                Bucket=bucket,
+                Prefix=f"{s3_key}/{remote_filename}",
+            )
+            if res["KeyCount"] > 0:
+                return f"s3://{bucket}/{s3_key}"
+        with open(file, "rb") as b_file:
+            s3_client.put_object(
+                Bucket=bucket,
+                Key=f"{s3_key}/{remote_filename}",
+                Body=b_file,
+                ServerSideEncryption="aws:kms",
+                SSEKMSKeyId=kms_arn,
+            )
+        return f"s3://{bucket}/{s3_key}"
+
     def close(self) -> None:
         return self.connection.close()
 
 
 class AthenaParser(DatabaseParser):
-    def validate_table_schema(
-        self, expected: dict[dict[list]], schema: list[list]
-    ) -> dict:
-        schema = dict(schema)
-        return self._parse_found_schema(expected, schema)
+    def _find_type_len(self, row: str) -> int:
+        """Finds the end of a type string like row(...) or array(row(...))"""
+        # Note that this assumes the string is well formatted.
+        depth = 0
+        for i in range(len(row)):
+            match row[i]:
+                case ",":
+                    if depth == 0:
+                        break
+                case "(":
+                    depth += 1
+                case ")":
+                    depth -= 1
+        return i
+
+    def _split_row(self, row: str) -> dict[str, str]:
+        # Must handle "name type, name row(...), name type, name row(...)"
+        result = {}
+        # Real athena doesn't add extra spaces, but our unit tests do for
+        # readability, so let's strip out whitespace as we parse.
+        while row := row.strip():
+            name, remainder = row.split(" ", 1)
+            type_len = self._find_type_len(remainder)
+            result[name] = remainder[0:type_len]
+            row = remainder[type_len + 2 :]  # skip comma and space
+        return result
+
+    def parse_found_schema(self, schema: dict[str, str]) -> dict:
+        # A sample response for table `observation`, column `component`:
+        #   array(row(code varchar, display varchar)),
+        #             text varchar, id varchar)
+        parsed = {}
+
+        for key, value in schema.items():
+            # Strip arrays out, they don't affect the shape of our schema.
+            while value.startswith("array("):
+                value = value.removeprefix("array(")
+                value = value.removesuffix(")")
+
+            if value.startswith("row("):
+                value = value.removeprefix("row(")
+                value = value.removesuffix(")")
+                parsed[key] = self.parse_found_schema(self._split_row(value))
+            else:
+                parsed[key] = {}
+
+        return parsed
 
 
 class DuckDatabaseBackend(DatabaseBackend):
     """Database backend that uses local files via duckdb"""
 
     def __init__(self, db_file: str):
         super().__init__("main")
+        self.db_type = "duckdb"
         self.connection = duckdb.connect(db_file)
         # Aliasing Athena's as_pandas to duckDB's df cast
         duckdb.DuckDBPyConnection.as_pandas = duckdb.DuckDBPyConnection.df
 
         # Paper over some syntax differences between Athena and DuckDB
         self.connection.create_function(
             # DuckDB's version is array_to_string -- seems there is no standard here.
@@ -319,24 +457,34 @@
     def close(self) -> None:
         self.connection.close()
 
 
 class DuckDbParser(DatabaseParser):
     """Table parser for DuckDB schemas"""
 
-    def validate_table_schema(
-        self, expected: dict[dict[list]], schema: list[tuple]
-    ) -> dict:
+    def parse_found_schema(self, schema: dict[str, str]) -> dict:
         """parses a information_schema.tables query response for valid columns"""
-        schema = dict(schema)
-        # since we're defaulting to athena naming conventions elsewhere,
-        # we'll lower case all the keys
-        schema = {k.lower(): v for k, v in schema.items()}
+        parsed = {}
+
+        for key, value in schema.items():
+            if isinstance(value, str):
+                # DuckDB provides a parser to go from string -> type objects
+                value = duckdb.typing.DuckDBPyType(value)
+
+            # Collapse lists to the contained value
+            if value.id == "list":
+                value = value.children[0][1]  # [('child', CONTAINED_TYPE)]
+
+            if value.id == "struct":
+                result = self.parse_found_schema(dict(value.children))
+            else:
+                result = {}
+            parsed[key.lower()] = result
 
-        return self._parse_found_schema(expected, schema)
+        return parsed
 
 
 def _read_rows_from_table_dir(path: str) -> list[dict]:
     # Grab filenames to load (ignoring .meta files and handling missing folders)
     folder = Path(path)
     filenames = []
     if folder.exists():
@@ -399,28 +547,28 @@
             # Auto-detecting the schema works for these simple tables
             all_tables[metadata_table] = pyarrow.Table.from_pylist(rows)
 
     return all_tables
 
 
 def create_db_backend(args: dict[str, str]) -> DatabaseBackend:
-    db_type = args["db_type"]
+    db_config.db_type = args["db_type"]
     database = args["schema_name"]
     load_ndjson_dir = args.get("load_ndjson_dir")
 
-    if db_type == "duckdb":
+    if db_config.db_type == "duckdb":
         backend = DuckDatabaseBackend(database)  # `database` is path name in this case
         if load_ndjson_dir:
             backend.insert_tables(read_ndjson_dir(load_ndjson_dir))
-    elif db_type == "athena":
+    elif db_config.db_type == "athena":
         backend = AthenaDatabaseBackend(
             args["region"],
             args["workgroup"],
             args["profile"],
             database,
         )
         if load_ndjson_dir:
             sys.exit("Loading an ndjson dir is not supported with --db-type=athena.")
     else:
-        raise ValueError(f"Unexpected --db-type value '{db_type}'")
+        raise ValueError(f"Unexpected --db-type value '{db_config.db_type}'")
 
     return backend
```

### Comparing `cumulus_library-2.0.1/cumulus_library/errors.py` & `cumulus_library-2.1.0/cumulus_library/errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,7 +17,15 @@
 
 class StudyManifestParsingError(Exception):
     """Errors related to manifest parsing in StudyManifestParser"""
 
 
 class StudyManifestQueryError(Exception):
     """Errors related to data queries from StudyManifestParser"""
+
+
+class AWSError(Exception):
+    """Errors from interacting with AWS"""
+
+
+class ApiError(Exception):
+    """Errors from external API calls"""
```

### Comparing `cumulus_library-2.0.1/cumulus_library/parsers/fhir_valueset.py` & `cumulus_library-2.1.0/cumulus_library/parsers/fhir_valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/protected_table_builder.py` & `cumulus_library-2.1.0/cumulus_library/protected_table_builder.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/schema/columns.py` & `cumulus_library-2.1.0/cumulus_library/schema/columns.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/schema/typesystem.py` & `cumulus_library-2.1.0/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/schema/valueset.py` & `cumulus_library-2.1.0/cumulus_library/schema/valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/statistics/counts.py` & `cumulus_library-2.1.0/cumulus_library/statistics/counts.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
     def write_counts(self, filepath: str):
         """Convenience method for writing counts queries to disk
 
         :param filepath: path to file to write queries out to.
         """
         self.prepare_queries(cursor=None, schema=None)
         self.comment_queries()
-        self.write_queries(filename=filepath)
+        self.write_queries(path=Path(filepath))
 
     def prepare_queries(self, cursor: object | None = None, schema: str | None = None):
         """Stub implementing abstract base class
 
         This should be overridden in any count generator. See studies/core/count_core.py
         for an example
         """
```

### Comparing `cumulus_library-2.0.1/cumulus_library/statistics/psm.py` & `cumulus_library-2.1.0/cumulus_library/statistics/psm.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 
 class PsmBuilder(base_table_builder.BaseTableBuilder):
     """TableBuilder for creating PSM tables"""
 
     display_text = "Building PSM tables..."
 
-    def __init__(self, toml_config_path: str, data_path: pathlib.Path):
+    def __init__(self, toml_config_path: str, data_path: pathlib.Path, **kwargs):
         """Loads PSM job details from a PSM configuration file"""
         super().__init__()
         # We're stashing the toml path for error reporting later
         self.toml_path = toml_config_path
         self.data_path = data_path
         try:
             with open(self.toml_path, encoding="UTF-8") as file:
@@ -342,20 +342,24 @@
             )
         except ValueError:
             sys.exit(
                 "Encountered a value error during KNN matching. Try increasing "
                 "your sample size."
             )
 
-    def prepare_queries(self, cursor: object, schema: str, table_suffix: str):
+    def prepare_queries(
+        self, cursor: object, schema: str, table_suffix: str, *args, **kwargs
+    ):
         self._create_covariate_table(cursor, schema, table_suffix)
 
     def post_execution(
         self,
         cursor: object,
         schema: str,
-        verbose: bool,
+        *args,
+        verbose: bool = False,
         drop_table: bool = False,
         table_suffix: str | None = None,
+        **kwargs,
     ):
         # super().execute_queries(cursor, schema, verbose, drop_table)
         self.generate_psm_analysis(cursor, schema, table_suffix)
```

### Comparing `cumulus_library-2.0.1/cumulus_library/statistics/psm.sql` & `cumulus_library-2.1.0/cumulus_library/statistics/psm.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/count.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/count.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/counts_templates.py` & `cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/counts_templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/statistics/statistics_templates/psm_templates.py` & `cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/psm_templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/builder_documentreference.py` & `cumulus_library-2.1.0/cumulus_library/studies/core/builder_documentreference.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from cumulus_library import base_table_builder, databases
 from cumulus_library.studies.core.core_templates import core_templates
 from cumulus_library.template_sql import sql_utils
 
 expected_table_cols = {
     "documentreference": {
         "id": [],
-        "type": [],
         "status": [],
+        "date": [],
         "docStatus": [],
-        "subject": ["reference"],
-        "context": ["encounter", "period", "start"],
-        "category": [],
+        "subject": sql_utils.REFERENCE,
+        "context": {"encounter": sql_utils.REFERENCE, "period": ["start"]},
     }
 }
 
 
 class CoreDocumentreferenceBuilder(base_table_builder.BaseTableBuilder):
     display_text = "Creating DocumentReference tables..."
 
@@ -25,14 +24,15 @@
         *args,
         parser: databases.DatabaseParser = None,
         **kwargs,
     ):
         self.queries = sql_utils.denormalize_complex_objects(
             schema,
             cursor,
+            parser,
             [
                 sql_utils.CodeableConceptConfig(
                     source_table="documentreference",
                     source_id="id",
                     column_hierarchy=[("type", dict)],
                     target_table="core__documentreference_dn_type",
                 ),
@@ -54,16 +54,17 @@
                     ],
                 ),
                 sql_utils.CodingConfig(
                     source_table="documentreference",
                     source_id="id",
                     column_hierarchy=[("content", list), ("format", dict)],
                     target_table="core__documentreference_dn_format",
+                    expected={"format": sql_utils.CODING},
                 ),
             ],
         )
-        validated_schema = core_templates.validate_schema(
+        validated_schema = sql_utils.validate_schema(
             cursor, schema, expected_table_cols, parser
         )
         self.queries.append(
             core_templates.get_core_template("documentreference", validated_schema)
         )
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/builder_encounter.py` & `cumulus_library-2.1.0/cumulus_library/studies/core/builder_encounter.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,32 +2,22 @@
 
 from cumulus_library import base_table_builder, databases
 from cumulus_library.studies.core.core_templates import core_templates
 from cumulus_library.template_sql import sql_utils
 
 expected_table_cols = {
     "encounter": {
+        "id": [],
         "status": [],
         "period": [
             "start",
             "end",
         ],
-        "class": [
-            "code",
-            "system",
-            "display",
-            "userSelected",
-            "version",
-        ],
-        "subject": [
-            "reference",
-            "display",
-            "type",
-        ],
-        "id": [],
+        "class": sql_utils.CODING,
+        "subject": sql_utils.REFERENCE,
     },
     "etl__completion": {
         "group_name": [],
     },
     "etl__completion_encounters": {
         "group_name": [],
     },
@@ -43,15 +33,15 @@
     def __post_init__(self):
         self.target_table = f"core__encounter_dn_{self.column_hierarchy[-1][0]}"
 
 
 class CoreEncounterBuilder(base_table_builder.BaseTableBuilder):
     display_text = "Creating Encounter tables..."
 
-    def denormalize_codes(self, schema, cursor):
+    def denormalize_codes(self, schema, cursor, parser):
         code_configs = [
             EncConfig(
                 column_hierarchy=[("type", list)],
                 filter_priority=True,
                 code_systems=[
                     "http://terminology.hl7.org/CodeSystem/encounter-type",
                     "http://terminology.hl7.org/CodeSystem/v2-0004",
@@ -106,33 +96,34 @@
                 ],
             ),
             EncConfig(
                 column_hierarchy=[
                     ("hospitalization", dict),
                     ("dischargedisposition", dict),
                 ],
-                filter_priority=False,
+                expected={"dischargedisposition": sql_utils.CODEABLE_CONCEPT},
             ),
         ]
         self.queries += sql_utils.denormalize_complex_objects(
-            schema, cursor, code_configs
+            schema, cursor, parser, code_configs
         )
 
     def prepare_queries(
         self,
         cursor: object,
         schema: str,
         *args,
         parser: databases.DatabaseParser = None,
         **kwargs,
     ):
         self.denormalize_codes(
             schema,
             cursor,
+            parser,
         )
-        validated_schema = core_templates.validate_schema(
+        validated_schema = sql_utils.validate_schema(
             cursor, schema, expected_table_cols, parser
         )
         self.queries += [
             core_templates.get_core_template("encounter", validated_schema),
             core_templates.get_core_template("incomplete_encounter", validated_schema),
         ]
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/builder_medicationrequest.py` & `cumulus_library-2.1.0/cumulus_library/studies/core/builder_medicationrequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 expected_table_cols = {
     "medicationrequest": {
         "id": [],
         "status": [],
         "intent": [],
         "authoredOn": [],
         "reportedBoolean": [],
-        "category": ["code", "system", "display"],
-        "medicationCodeableConcept": ["code", "system", "display"],
-        "subject": ["reference"],
-        "encounter": ["reference"],
+        "subject": sql_utils.REFERENCE,
+        "encounter": sql_utils.REFERENCE,
         "dosageInstruction": ["text"],
     }
 }
 
 
 class MedicationRequestBuilder(base_table_builder.BaseTableBuilder):
     display_text = "Creating MedicationRequest tables..."
@@ -42,23 +40,17 @@
         code_sources = [
             sql_utils.CodeableConceptConfig(
                 source_table="medicationrequest",
                 source_id="id",
                 column_hierarchy=[("category", list)],
                 target_table="core__medicationrequest_dn_category",
             ),
-            sql_utils.CodeableConceptConfig(
-                source_table="medicationrequest",
-                source_id="id",
-                column_hierarchy=[("medicationcodeableconcept", dict)],
-                target_table="core__medicationrequest_dn_medication",
-            ),
         ]
         self.queries += sql_utils.denormalize_complex_objects(
-            schema, cursor, code_sources
+            schema, cursor, parser, code_sources
         )
-        validated_schema = core_templates.validate_schema(
+        validated_schema = sql_utils.validate_schema(
             cursor, schema, expected_table_cols, parser
         )
         self.queries.append(
             core_templates.get_core_template("medicationrequest", validated_schema)
         )
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/builder_patient.py` & `cumulus_library-2.1.0/cumulus_library/studies/core/builder_patient.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,26 +5,66 @@
 from cumulus_library.studies.core.core_templates import core_templates
 from cumulus_library.template_sql import base_templates, sql_utils
 
 expected_table_cols = {
     "patient": {
         "id": [],
         "gender": [],
-        "address": [],
+        "address": {"postalCode": {}},
         "birthDate": [],
     }
 }
 
 
 class PatientBuilder(BaseTableBuilder):
     display_text = "Creating Patient tables..."
 
+    @staticmethod
+    def make_extension_query(
+        schema: str,
+        cursor: databases.DatabaseCursor,
+        parser: databases.DatabaseParser,
+        name: str,
+        url: str,
+    ) -> str:
+        has_extensions = sql_utils.is_field_present(
+            schema=schema,
+            cursor=cursor,
+            parser=parser,
+            source_table="patient",
+            source_col="extension",
+            expected={
+                "extension": {
+                    "url": {},
+                    "valueCoding": sql_utils.CODING,
+                },
+                "url": {},
+            },
+        )
+        if has_extensions:
+            config = sql_utils.ExtensionConfig(
+                source_table="patient",
+                source_id="id",
+                target_table=f"core__patient_ext_{name}",
+                target_col_prefix=name,
+                fhir_extension=url,
+                ext_systems=["ombCategory", "detailed"],
+                is_array=True,
+            )
+            return base_templates.get_extension_denormalize_query(config)
+        else:
+            return base_templates.get_ctas_empty_query(
+                schema_name=schema,
+                table_name=f"core__patient_ext_{name}",
+                table_cols=["id", "system", f"{name}_code", f"{name}_display"],
+            )
+
     def prepare_queries(
         self,
-        cursor: object,
+        cursor: databases.DatabaseCursor,
         schema: str,
         *args,
         parser: databases.DatabaseParser = None,
         **kwargs,
     ):
         """constructs queries related to patient extensions of interest
 
@@ -37,25 +77,20 @@
                 "fhirpath": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race",
             },
             {
                 "name": "ethnicity",
                 "fhirpath": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity",
             },
         ]
-
         for extension in extension_types:
-            config = sql_utils.ExtensionConfig(
-                source_table="patient",
-                source_id="id",
-                target_table=f"core__patient_ext_{extension['name']}",
-                target_col_prefix=extension["name"],
-                fhir_extension=extension["fhirpath"],
-                ext_systems=["ombCategory", "detailed", "text"],
-                is_array=True,
+            self.queries.append(
+                self.make_extension_query(
+                    schema, cursor, parser, extension["name"], extension["fhirpath"]
+                )
             )
-            self.queries.append(base_templates.get_extension_denormalize_query(config))
-        validated_schema = core_templates.validate_schema(
+
+        validated_schema = sql_utils.validate_schema(
             cursor, schema, expected_table_cols, parser
         )
         self.queries.append(
             core_templates.get_core_template("patient", validated_schema)
         )
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/builder_prereq_tables.py` & `cumulus_library-2.1.0/cumulus_library/studies/core/builder_prereq_tables.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/completion_utils.jinja` & `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/completion_utils.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/condition.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/condition.sql.jinja`

 * *Files 19% similar despite different names*

```diff
@@ -13,15 +13,14 @@
             ) 
         }},
         {{- 
             utils.nullable_cols(
                 'condition',
                 'c',
                 [
-                    'category',
                     ('subject', 'reference', 'subject_ref'),
                     ('encounter', 'reference', 'encounter_ref'),
                 ], 
                 schema
             ) 
         }},
         {{- 
@@ -50,38 +49,36 @@
                 [
                     ('recordedDate', 'week'),
                     ('recordedDate', 'month'),
                     ('recordedDate', 'year'),
                 ],
                 schema
             ) 
-        }},
-        c.verificationStatus,
-        c.clinicalStatus
+        }}
     FROM condition AS c
     LEFT JOIN core__condition_codable_concepts_all AS cca ON c.id = cca.id
 )
 
 SELECT
     tc.id,
-    t_category_coding.category_row.code AS category_code,
-    t_category_coding.category_row.display AS category_display,
+    cdc.code AS category_code,
+    cdc.code_system AS category_code_system,
+    cdc.display AS category_display,
     tc.code,
     tc.code_system,
     tc.display AS code_display,
     tc.subject_ref,
     tc.encounter_ref,
     concat('Condition/', tc.id) AS condition_ref,
     tc.recordedDate,
     tc.recordedDate_week,
     tc.recordedDate_month,
     tc.recordedDate_year,
-    t_clinicalStatus_coding.clinicalStatus_row.code AS clinicalStatus_code,
-    t_verificationStatus_coding.verificationStatus_row.code AS verificationStatus_code
-FROM temp_condition AS tc,
-    unnest(category) AS t_category (category_coding),
-    unnest(category_coding.coding) AS t_category_coding (category_row),
-    unnest(clinicalStatus.coding) AS t_clinicalStatus_coding (clinicalStatus_row),
-    unnest(verificationStatus.coding)
-        AS t_verificationStatus_coding (verificationStatus_row)
-
+    {#- We don't expose code_system for these next two since we filter
+        down to a single system in the denormalization table #}
+    cdcs.code AS clinicalStatus_code,
+    cdvs.code AS verificationStatus_code
+FROM temp_condition AS tc
+LEFT JOIN core__condition_dn_category AS cdc ON tc.id = cdc.id
+LEFT JOIN core__condition_dn_clinical_status AS cdcs ON tc.id = cdcs.id
+LEFT JOIN core__condition_dn_verification_status AS cdvs ON tc.id = cdvs.id
 WHERE tc.recordedDate BETWEEN date('2016-01-01') AND current_date;
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/core_utils.jinja` & `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/core_utils.jinja`

 * *Files 3% similar despite different names*

```diff
@@ -23,34 +23,34 @@
 
 -#}
 {% macro nullable_cols(table, alias, targets, schema) %}
         {%- for col in targets %}
         {#- depth one nested column-#}
         {%- if col is not string and col|length ==3%}
         {%- if schema[table][col[0]][col[1]] %}
-        {{ alias }}.{{ col[0] }}.{{ col[1] }} AS {{col[2].lower()}}
+        {{ alias }}.{{ col[0] }}.{{ col[1] }} AS {{ col[2] }}
         {%- else %}
-        cast(NULL as varchar) AS {{ col[2].lower() }}
+        cast(NULL as varchar) AS {{ col[2] }}
         {%- endif %}
         {#- depth two nested column -#}
         {%- elif col is not string and col|length ==4%}
-        {%- if schema[table][col[0]][col[2]] %}
-        {{ alias }}.{{ col[0] }}.{{ col[1] }}.{{ col[2] }} AS {{col[3].lower()}}
+        {%- if schema[table][col[0]][col[1]][col[2]] %}
+        {{ alias }}.{{ col[0] }}.{{ col[1] }}.{{ col[2] }} AS {{ col[3] }}
         {%- else %}
-        cast(NULL as varchar) AS {{ col[3].lower()}}
+        cast(NULL as varchar) AS {{ col[3] }}
         {%- endif %}
         {#- SQL primitive column column-#}
         {%- elif schema[table][col] %}
         {{ alias }}.{{ col }}
         {%- else %}
         {#- workaround for docref date-#}
         {%- if col == "date"%}
-        cast(NULL as timestamp) AS "{{ col.lower() }}"
+        cast(NULL as timestamp) AS "{{ col }}"
         {%- else %}
-        cast(NULL as varchar) AS {{ col.lower() }}
+        cast(NULL as varchar) AS {{ col }}
         {%- endif %}
         {%- endif %}        
         {{- syntax.comma_delineate(loop) }}
         {%- endfor %}
 {%- endmacro %}
 
 {#- creates a date from a from an ISO formatted date str 
@@ -62,28 +62,28 @@
 {% macro date_cols_from_str(table, alias, targets, schema) %}
         {%- for col in targets %}
         {#- depth one nested column-#}
         {%- if col is not string and col|length ==3%}
         {%- if schema[table][col[0]][col[1]] %}
         date(from_iso8601_timestamp({{ alias }}.{{ col[0] }}.{{ col[1] }})) AS {{ col[2] }}
         {%- else %}
-        cast(NULL AS date) AS {{ col[1].lower() }}
+        cast(NULL AS date) AS {{ col[1] }}
         {% endif %}
         {#- depth two nested column -#}
         {%- elif col is not string and col|length ==4%}
-        {%- if schema[table][col[0]][col[2]] %}
+        {%- if schema[table][col[0]][col[1]][col[2]] %}
         date(from_iso8601_timestamp({{ alias }}.{{ col[0] }}.{{ col[1] }}.{{ col[2] }})) AS {{col[3]}}
         {%- else %}
-        cast(NULL AS date) AS {{ col[3].lower() }}
+        cast(NULL AS date) AS {{ col[3] }}
         {%- endif %}
         {#- SQL primitive column column-#}
         {%- elif schema[table][col] %}
         date(from_iso8601_timestamp({{ alias }}.{{ col }})) AS {{ col }}
         {%- else %}
-        cast(NULL AS date) AS {{ col.lower() }}
+        cast(NULL AS date) AS {{ col }}
         {%- endif %}    
         {{- syntax.comma_delineate(loop) }}
         {%- endfor %}
 {%- endmacro %}
 
 {#- creates a truncated date from an iso formatted date of the specified period
 
@@ -99,15 +99,15 @@
         date_trunc('{{ col[3] }}', date(from_iso8601_timestamp({{ alias }}."{{ col[0] }}"."{{ col[1] }}")))
             AS {{ col[2] }}
         {%- else %}
         cast(NULL AS date) AS {{col[2]}}
         {% endif %}
         {#- depth two nested column -#}
         {%- elif col is not string and col|length ==5%}
-        {%- if schema[table][col[0]][col[2]] %}
+        {%- if schema[table][col[0]][col[1]][col[2]] %}
         date_trunc('{{ col[4] }}', date(from_iso8601_timestamp({{ alias }}."{{ col[0] }}"."{{ col[1] }}"."{{col[2]}}")))
             AS {{ col[3] }}
         {%- else %}
         cast(NULL AS date) AS {{col[3]}}
         {%- endif %}
         {#- SQL primitive column column-#}
         {%- elif schema[table][col[0]] %}
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/documentreference.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/documentreference.sql.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -12,25 +12,29 @@
             ) 
         }},
         {#- TODO: validate usage of author vs spec language of period -#}
         {{- utils.nullable_cols(
                 'documentreference',
                 'dr',
                 [
-                    'type',
                     'status',
-                    'date',
                     'docStatus',
-                    'context',                
+                    'context',
                     ('subject', 'reference', 'subject_ref'),
-                    ('context', 'period', 'start', 'author_date')
                 ], 
                 schema
             ) 
         }},
+        {{- utils.date_cols_from_str(
+                'documentreference',
+                'dr',
+                ['date'],
+                schema
+            )
+        }},
         {{- utils.truncate_date_cols(
                 'documentreference',
                 'dr',
                 [
                     ('context', 'period', 'start', 'author_day', 'day'),
                     ('context', 'period', 'start', 'author_week', 'week'),
                     ('context', 'period', 'start', 'author_month', 'month'),
@@ -50,15 +54,15 @@
     LEFT JOIN core__documentreference_dn_format AS cdrf ON dr.id = cdrf.id
 ),
 
 temp_encounters AS (
     SELECT
         tdr.id,
 
-{% if schema["documentreference"]["context"]["encounter"] %}
+{% if schema["documentreference"]["context"]["encounter"]["reference"] %}
         context_encounter.encounter.reference AS encounter_ref
     FROM temp_documentreference AS tdr,
          unnest(context.encounter) AS context_encounter (encounter) --noqa
 
 {% else %}
         cast('' AS varchar) AS encounter_ref
     FROM temp_documentreference AS tdr
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/encounter.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/encounter.sql.jinja`

 * *Files 3% similar despite different names*

```diff
@@ -22,17 +22,17 @@
             ) 
         }},
         {{- utils.nullable_cols(
                 'encounter',
                 'e',
                 [
                     'status',
-                    'class', 
+                    ('class', 'code', 'class_code'),
+                    ('class', 'system', 'class_code_system'),
                     ('subject', 'reference', 'subject_ref'),
-                    'period',
                 ], 
                 schema
             ) 
         }},
         {{- utils.date_cols_from_str(
                 'encounter',
                 'e',
@@ -42,15 +42,15 @@
                 schema
             ) 
         }},
         {{- utils.truncate_date_cols(
                 'encounter',
                 'e',
                 [
-                    ('period','end', 'period_end_day', 'day'),
+                    ('period', 'end', 'period_end_day', 'day'),
                     ('period', 'start', 'period_start_day', 'day'),
                     ('period', 'start', 'period_start_week', 'week'),
                     ('period', 'start', 'period_start_month', 'month'),
                     ('period', 'start', 'period_start_year', 'year'),
                 ],
                 schema
             ) 
@@ -64,15 +64,16 @@
     )
 ),
 
 temp_encounter AS (
     SELECT DISTINCT
         e.id,
         e.status,
-        e.class,
+        e.class_code,
+        e.class_code_system,
         e.subject_ref,
         e.period_start,
         e.period_start_day,
         e.period_end_day,
         e.period_start_week,
         e.period_start_month,
         e.period_start_year,
@@ -89,15 +90,15 @@
         edr.code_system AS reasonCode_code_system,
         edr.display AS reasonCode_display,
         edd.code AS dischargeDisposition_code,
         edd.code_system AS dischargeDisposition_code_system,
         edd.display AS dischargeDisposition_display
 
     FROM temp_encounter_nullable AS e
-    LEFT JOIN core__encounter_dn_priority AS edt ON e.id = edt.id
+    LEFT JOIN core__encounter_dn_type AS edt ON e.id = edt.id
     LEFT JOIN core__encounter_dn_servicetype AS eds ON e.id = eds.id
     LEFT JOIN core__encounter_dn_priority AS edp ON e.id = edp.id
     LEFT JOIN core__encounter_dn_reasoncode AS edr ON e.id = edr.id
     LEFT JOIN core__encounter_dn_dischargedisposition AS edd ON e.id = edd.id
 )
 
 SELECT DISTINCT
@@ -130,12 +131,12 @@
     e.period_start_week AS period_start_week,
     e.period_start_month AS period_start_month,
     e.period_start_year AS period_start_year,
     e.subject_ref,
     concat('Encounter/', e.id) AS encounter_ref
 FROM temp_encounter AS e
 LEFT JOIN core__fhir_mapping_expected_act_encounter_code_v3 AS eac
-    ON e.class.code = eac.found
+    ON e.class_code = eac.found
 LEFT JOIN core__fhir_act_encounter_code_v3 AS ac ON eac.expected = ac.code
 INNER JOIN core__patient AS p ON e.subject_ref = p.subject_ref
 WHERE
     e.period_start_day BETWEEN date('2016-06-01') AND current_date;
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 {% import 'core_utils.jinja' as utils %}
 
 CREATE TABLE core__medicationrequest AS
-WITH temp_mr AS (
+WITH
+
+tmp_dn_dosage_text AS (
+    SELECT
+        mr.id,
+        {{- utils.nullable_cols(
+            'medicationrequest',
+            'u',
+            [
+                ('dosageInstruction', 'text', 'dosageInstruction_text'),
+            ],
+            schema
+        ) }}
+    FROM medicationrequest AS mr,
+        UNNEST(mr.dosageInstruction) AS u (dosageInstruction)
+    WHERE u.dosageInstruction.text IS NOT NULL
+),
+
+temp_mr AS (
     SELECT 
         {{- utils.basic_cols(
                 'medicationrequest',
                 'mr',
                 [
                     'id', 
                     'status', 
@@ -30,30 +48,30 @@
             ) 
         }},
         {{- utils.nullable_cols(
                 'medicationrequest',
 
                 'mr',
                 [
-                    'display',
                     'reportedBoolean',
-                    'dosageInstruction',
                     ('subject', 'reference', 'subject_ref'),
                     ('encounter', 'reference', 'encounter_ref'),
                 ],
                 schema
         ) -}},
         mrc.code AS category_code,
         mrc.code_system AS category_code_system,
         mrm.code AS medication_code,
         mrm.code_system AS medication_code_system,
-        mrm.display AS medication_display
+        mrm.display AS medication_display,
+        mrdt.dosageInstruction_text
     FROM medicationrequest AS mr
     LEFT JOIN core__medicationrequest_dn_category AS mrc ON mr.id = mrc.id
-    LEFT JOIN core__medicationrequest_dn_medication AS mrm ON mr.id = mrm.id
+    LEFT JOIN core__medicationrequest_dn_inline_code AS mrm ON mr.id = mrm.id
+    LEFT JOIN tmp_dn_dosage_text AS mrdt ON mr.id = mrdt.id
     WHERE mrm.code_system = 'http://www.nlm.nih.gov/research/umls/rxnorm'
 )
 
 SELECT
     mr.id,
     mr.status,
     mr.intent,
@@ -61,12 +79,11 @@
     mr.category_code_system,
     mr.reportedBoolean,
     mr.medication_code_system,
     mr.medication_code,
     mr.medication_display,
     mr.authoredOn,
     mr.authoredOn_month,
-    dose_row.dose_col.text AS dosageInstruction_text,
+    mr.dosageInstruction_text,
     mr.subject_ref,
     mr.encounter_ref
-FROM temp_mr AS mr,
-    UNNEST(dosageInstruction) AS dose_row (dose_col)
+FROM temp_mr AS mr
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/observation.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/observation.sql.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
                 ]
             ) 
         }},
         {{- utils.nullable_cols(
                 'observation',
                 'o',
                 [
+                    ('encounter', 'reference', 'encounter_ref'),
+                    ('subject', 'reference', 'subject_ref'),
                     'valueString',
                     ('valueQuantity', 'value', 'valueQuantity_value'),
                     ('valueQuantity', 'comparator', 'valueQuantity_comparator'),
                     ('valueQuantity', 'unit', 'valueQuantity_unit'),
-                    ('valueQuantity', 'system', 'valueQuantity_system'),
+                    ('valueQuantity', 'system', 'valueQuantity_code_system'),
                     ('valueQuantity', 'code', 'valueQuantity_code'),
                 ],
                 schema
             ) 
         }},
         {{- utils.truncate_date_cols(
                 'observation',
@@ -46,19 +48,15 @@
         odi.code_system AS interpretation_code_system,
         odi.display AS interpretation_display,
         odvcc.code AS valueCodeableConcept_code,
         odvcc.code_system AS valueCodeableConcept_code_system,
         odvcc.display AS valueCodeableConcept_display,
         odda.code AS dataAbsentReason_code,
         odda.code_system AS dataAbsentReason_code_system,
-        odda.display AS dataAbsentReason_display,
-        o.referencerange,
-        o.valueQuantity,
-        o.subject.reference AS subject_ref,
-        o.encounter.reference AS encounter_ref
+        odda.display AS dataAbsentReason_display
     FROM observation AS o
     LEFT JOIN core__observation_dn_category AS odcat ON o.id = odcat.id
     LEFT JOIN core__observation_dn_code AS odc ON o.id = odc.id
     LEFT JOIN core__observation_dn_interpretation AS odi ON o.id = odi.id
     LEFT JOIN core__observation_dn_valuecodeableconcept AS odvcc ON o.id = odvcc.id
     LEFT JOIN core__observation_dn_dataabsentreason AS odda ON o.id = odda.id
 )
@@ -79,15 +77,15 @@
     effectiveDateTime_year,
     valueCodeableConcept_code,
     valueCodeableConcept_code_system,
     valueCodeableConcept_display,
     valueQuantity_value,
     valueQuantity_comparator,
     valueQuantity_unit,
-    valueQuantity_system,
+    valueQuantity_code_system,
     valueQuantity_code,
     valueString,
     dataAbsentReason_code,
     dataAbsentReason_code_system,
     dataAbsentReason_display,
     subject_ref,
     encounter_ref,
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/core_templates/patient.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/patient.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/count_core.py` & `cumulus_library-2.1.0/cumulus_library/studies/core/count_core.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/fhir_lookup_tables.sql` & `cumulus_library-2.1.0/cumulus_library/studies/core/fhir_lookup_tables.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/fhir_mapping_tables.sql` & `cumulus_library-2.1.0/cumulus_library/studies/core/fhir_mapping_tables.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/manifest.toml` & `cumulus_library-2.1.0/cumulus_library/studies/core/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_documentreference.sql` & `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_documentreference.sql`

 * *Files 9% similar despite different names*

```diff
@@ -8,93 +8,116 @@
 
 CREATE TABLE core__documentreference_dn_type AS (
     WITH
 
     system_type_0 AS (
         SELECT DISTINCT
             s.id AS id,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            0 AS row,
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
             documentreference AS s,
-            UNNEST(s.type.coding) AS u (codeable_concept)
+            UNNEST(s.type.coding) AS u (coding)
     ), --noqa: LT07
 
     union_table AS (
         SELECT
             id,
+            row,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_type_0
         
     )
     SELECT
         id,
         code,
         code_system,
-        display
+        display,
+        userSelected
     FROM union_table
 );
 
 
 -- ###########################################################
 
 CREATE TABLE core__documentreference_dn_category AS (
     WITH
 
+    flattened_rows AS (
+        SELECT DISTINCT
+            t.id AS id,
+            ROW_NUMBER() OVER (PARTITION BY id) AS row,
+            r."category"
+        FROM
+            documentreference AS t,
+            UNNEST(t."category") AS r ("category")
+    ),
+
     system_category_0 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '0' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            documentreference AS s,
-            UNNEST(s.category) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.category.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'http://hl7.org/fhir/us/core/ValueSet/us-core-documentreference-category'
+            u.coding.system LIKE 'http://hl7.org/fhir/us/core/ValueSet/us-core-documentreference-category'
     ), --noqa: LT07
 
     union_table AS (
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_category_0
         
     ),
 
     partitioned_table AS (
         SELECT
             id,
+            row,
             code,
             code_system,
             display,
+            userSelected,
             priority,
             ROW_NUMBER()
                 OVER (
                     PARTITION BY id
                     ORDER BY priority ASC
                 ) AS available_priority
         FROM union_table
-        GROUP BY id, priority, code_system, code, display
+        GROUP BY
+            id, row, priority, code_system, code, display, userSelected
         ORDER BY priority ASC
     )
 
     SELECT
         id,
+        row,
         code,
         code_system,
-        display
+        display,
+        userSelected
     FROM partitioned_table
     WHERE available_priority = 1
 );
 
 
 -- ###########################################################
 
@@ -134,21 +157,19 @@
 
 
 -- noqa: PRS
 CREATE TABLE core__documentreference AS
 WITH temp_documentreference AS (
     SELECT DISTINCT
         dr.id,
-        dr.type,
         dr.status,
-        cast(NULL as timestamp) AS "date",
         dr.docStatus,
         dr.context,
         dr.subject.reference AS subject_ref,
-        dr.context.period.start AS author_date,
+        date(from_iso8601_timestamp(dr.date)) AS date,
         date_trunc('day', date(from_iso8601_timestamp(dr."context"."period"."start")))
             AS author_day,
         date_trunc('week', date(from_iso8601_timestamp(dr."context"."period"."start")))
             AS author_week,
         date_trunc('month', date(from_iso8601_timestamp(dr."context"."period"."start")))
             AS author_month,
         date_trunc('year', date(from_iso8601_timestamp(dr."context"."period"."start")))
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_encounter.sql` & `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_encounter.sql`

 * *Files 14% similar despite different names*

```diff
@@ -5,476 +5,558 @@
 -- option to derive the best SQL for your dataset.
 
 -- ###########################################################
 
 CREATE TABLE core__encounter_dn_type AS (
     WITH
 
+    flattened_rows AS (
+        SELECT DISTINCT
+            t.id AS id,
+            ROW_NUMBER() OVER (PARTITION BY id) AS row,
+            r."type"
+        FROM
+            encounter AS t,
+            UNNEST(t."type") AS r ("type")
+    ),
+
     system_type_0 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '0' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.type) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'http://terminology.hl7.org/CodeSystem/encounter-type'
+            u.coding.system LIKE 'http://terminology.hl7.org/CodeSystem/encounter-type'
     ), --noqa: LT07
 
     system_type_1 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '1' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.type) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'http://terminology.hl7.org/CodeSystem/v2-0004'
+            u.coding.system LIKE 'http://terminology.hl7.org/CodeSystem/v2-0004'
     ), --noqa: LT07
 
     system_type_2 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '2' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.type) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'urn:oid:2.16.840.1.113883.4.642.3.248'
+            u.coding.system LIKE 'urn:oid:2.16.840.1.113883.4.642.3.248'
     ), --noqa: LT07
 
     system_type_3 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '3' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.type) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'http://snomed.info/sct'
+            u.coding.system LIKE 'http://snomed.info/sct'
     ), --noqa: LT07
 
     system_type_4 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '4' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.type) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'https://fhir.cerner.com/%/codeSet/71'
+            u.coding.system LIKE 'https://fhir.cerner.com/%/codeSet/71'
     ), --noqa: LT07
 
     system_type_5 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '5' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.type) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.10.698084.10110'
+            u.coding.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.10.698084.10110'
     ), --noqa: LT07
 
     system_type_6 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '6' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.type) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.10.698084.18875'
+            u.coding.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.10.698084.18875'
     ), --noqa: LT07
 
     system_type_7 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '7' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.type) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.10.698084.30'
+            u.coding.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.10.698084.30'
     ), --noqa: LT07
 
     system_type_8 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '8' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.type) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.2.808267'
+            u.coding.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.2.808267'
     ), --noqa: LT07
 
     union_table AS (
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_type_0
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_type_1
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_type_2
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_type_3
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_type_4
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_type_5
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_type_6
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_type_7
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_type_8
         
     ),
 
     partitioned_table AS (
         SELECT
             id,
+            row,
             code,
             code_system,
             display,
+            userSelected,
             priority,
             ROW_NUMBER()
                 OVER (
                     PARTITION BY id
                     ORDER BY priority ASC
                 ) AS available_priority
         FROM union_table
-        GROUP BY id, priority, code_system, code, display
+        GROUP BY
+            id, row, priority, code_system, code, display, userSelected
         ORDER BY priority ASC
     )
 
     SELECT
         id,
+        row,
         code,
         code_system,
-        display
+        display,
+        userSelected
     FROM partitioned_table
     WHERE available_priority = 1
 );
 
 
 -- ###########################################################
 
 CREATE TABLE IF NOT EXISTS "main"."core__encounter_dn_servicetype"
 AS (
     SELECT * FROM (
         VALUES
-        (cast(NULL AS varchar),cast(NULL AS varchar),cast(NULL AS varchar),cast(NULL AS varchar))
+        (cast(NULL AS varchar),cast(NULL AS bigint),cast(NULL AS varchar),cast(NULL AS varchar),cast(NULL AS varchar),cast(NULL AS boolean))
     )
-        AS t ("id","code","code_system","display")
+        AS t ("id","row","code","code_system","display","userSelected")
+    WHERE 1 = 0 -- ensure empty table
 );
 
 -- ###########################################################
 
 CREATE TABLE IF NOT EXISTS "main"."core__encounter_dn_priority"
 AS (
     SELECT * FROM (
         VALUES
-        (cast(NULL AS varchar),cast(NULL AS varchar),cast(NULL AS varchar),cast(NULL AS varchar))
+        (cast(NULL AS varchar),cast(NULL AS bigint),cast(NULL AS varchar),cast(NULL AS varchar),cast(NULL AS varchar),cast(NULL AS boolean))
     )
-        AS t ("id","code","code_system","display")
+        AS t ("id","row","code","code_system","display","userSelected")
+    WHERE 1 = 0 -- ensure empty table
 );
 
 -- ###########################################################
 
 CREATE TABLE core__encounter_dn_reasoncode AS (
     WITH
 
+    flattened_rows AS (
+        SELECT DISTINCT
+            t.id AS id,
+            ROW_NUMBER() OVER (PARTITION BY id) AS row,
+            r."reasoncode"
+        FROM
+            encounter AS t,
+            UNNEST(t."reasoncode") AS r ("reasoncode")
+    ),
+
     system_reasoncode_0 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '0' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.reasoncode) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.reasoncode.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'http://terminology.hl7.org/CodeSystem/v3-ActPriority'
+            u.coding.system LIKE 'http://terminology.hl7.org/CodeSystem/v3-ActPriority'
     ), --noqa: LT07
 
     system_reasoncode_1 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '1' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.reasoncode) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.reasoncode.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'http://snomed.info/sct'
+            u.coding.system LIKE 'http://snomed.info/sct'
     ), --noqa: LT07
 
     system_reasoncode_2 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '2' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.reasoncode) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.reasoncode.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'http://hl7.org/fhir/sid/icd-10-cm'
+            u.coding.system LIKE 'http://hl7.org/fhir/sid/icd-10-cm'
     ), --noqa: LT07
 
     system_reasoncode_3 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '3' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.reasoncode) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.reasoncode.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'http://hl7.org/fhir/sid/icd-9-cm'
+            u.coding.system LIKE 'http://hl7.org/fhir/sid/icd-9-cm'
     ), --noqa: LT07
 
     system_reasoncode_4 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '4' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.reasoncode) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.reasoncode.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'https://fhir.cerner.com/%/nomenclature'
+            u.coding.system LIKE 'https://fhir.cerner.com/%/nomenclature'
     ), --noqa: LT07
 
     system_reasoncode_5 AS (
         SELECT DISTINCT
             s.id AS id,
+            s.row,
             '5' AS priority,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
-            encounter AS s,
-            UNNEST(s.reasoncode) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
+            flattened_rows AS s,
+            UNNEST(s.reasoncode.coding) AS u (coding)
         WHERE
-            u.codeable_concept.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.2.728286'
+            u.coding.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.2.728286'
     ), --noqa: LT07
 
     union_table AS (
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_reasoncode_0
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_reasoncode_1
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_reasoncode_2
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_reasoncode_3
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_reasoncode_4
         UNION
         SELECT
             id,
+            row,
             priority,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_reasoncode_5
         
     ),
 
     partitioned_table AS (
         SELECT
             id,
+            row,
             code,
             code_system,
             display,
+            userSelected,
             priority,
             ROW_NUMBER()
                 OVER (
                     PARTITION BY id
                     ORDER BY priority ASC
                 ) AS available_priority
         FROM union_table
-        GROUP BY id, priority, code_system, code, display
+        GROUP BY
+            id, row, priority, code_system, code, display, userSelected
         ORDER BY priority ASC
     )
 
     SELECT
         id,
+        row,
         code,
         code_system,
-        display
+        display,
+        userSelected
     FROM partitioned_table
     WHERE available_priority = 1
 );
 
 
 -- ###########################################################
 
 CREATE TABLE core__encounter_dn_dischargedisposition AS (
     WITH
 
     system_dischargedisposition_0 AS (
         SELECT DISTINCT
             s.id AS id,
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            0 AS row,
+            u.coding.code,
+            u.coding.display,
+            u.coding.system AS code_system,
+            u.coding.userSelected
         FROM
             encounter AS s,
-            UNNEST(s.hospitalization.dischargedisposition.coding) AS u (codeable_concept)
+            UNNEST(s.hospitalization.dischargedisposition.coding) AS u (coding)
     ), --noqa: LT07
 
     union_table AS (
         SELECT
             id,
+            row,
             code_system,
             code,
-            display
+            display,
+            userSelected
         FROM system_dischargedisposition_0
         
     )
     SELECT
         id,
         code,
         code_system,
-        display
+        display,
+        userSelected
     FROM union_table
 );
 
 
 -- ###########################################################
 
 
@@ -524,17 +606,17 @@
     LEFT JOIN temp_completed_tables AS tct ON tct.encounter_id = ece.encounter_id
 ),
 
 temp_encounter_nullable AS (
     SELECT DISTINCT
         e.id,
         e.status,
-        e.class,
+        e.class.code AS class_code,
+        e.class.system AS class_code_system,
         e.subject.reference AS subject_ref,
-        e.period,
         date(from_iso8601_timestamp(e.period.start)) AS period_start,
         date_trunc('day', date(from_iso8601_timestamp(e."period"."end")))
             AS period_end_day,
         date_trunc('day', date(from_iso8601_timestamp(e."period"."start")))
             AS period_start_day,
         date_trunc('week', date(from_iso8601_timestamp(e."period"."start")))
             AS period_start_week,
@@ -551,15 +633,16 @@
     )
 ),
 
 temp_encounter AS (
     SELECT DISTINCT
         e.id,
         e.status,
-        e.class,
+        e.class_code,
+        e.class_code_system,
         e.subject_ref,
         e.period_start,
         e.period_start_day,
         e.period_end_day,
         e.period_start_week,
         e.period_start_month,
         e.period_start_year,
@@ -576,15 +659,15 @@
         edr.code_system AS reasonCode_code_system,
         edr.display AS reasonCode_display,
         edd.code AS dischargeDisposition_code,
         edd.code_system AS dischargeDisposition_code_system,
         edd.display AS dischargeDisposition_display
 
     FROM temp_encounter_nullable AS e
-    LEFT JOIN core__encounter_dn_priority AS edt ON e.id = edt.id
+    LEFT JOIN core__encounter_dn_type AS edt ON e.id = edt.id
     LEFT JOIN core__encounter_dn_servicetype AS eds ON e.id = eds.id
     LEFT JOIN core__encounter_dn_priority AS edp ON e.id = edp.id
     LEFT JOIN core__encounter_dn_reasoncode AS edr ON e.id = edr.id
     LEFT JOIN core__encounter_dn_dischargedisposition AS edd ON e.id = edd.id
 )
 
 SELECT DISTINCT
@@ -617,15 +700,15 @@
     e.period_start_week AS period_start_week,
     e.period_start_month AS period_start_month,
     e.period_start_year AS period_start_year,
     e.subject_ref,
     concat('Encounter/', e.id) AS encounter_ref
 FROM temp_encounter AS e
 LEFT JOIN core__fhir_mapping_expected_act_encounter_code_v3 AS eac
-    ON e.class.code = eac.found
+    ON e.class_code = eac.found
 LEFT JOIN core__fhir_act_encounter_code_v3 AS ac ON eac.expected = ac.code
 INNER JOIN core__patient AS p ON e.subject_ref = p.subject_ref
 WHERE
     e.period_start_day BETWEEN date('2016-06-01') AND current_date;
 
 -- ###########################################################
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_patient.sql` & `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_patient.sql`

 * *Files 24% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             s.id AS id,
             '0' AS priority,
             'ombCategory' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS race_code,
             ext_child.ext.valuecoding.display AS race_display
         FROM
             patient AS s,
-            UNNEST(extension) AS ext_parent (ext),
+            UNNEST(s.extension) AS ext_parent (ext),
             UNNEST(ext_parent.ext.extension) AS ext_child (ext)
         WHERE
             ext_parent.ext.url = 'http://hl7.org/fhir/us/core/StructureDefinition/us-core-race'
             AND ext_child.ext.url = 'ombCategory'
             AND ext_child.ext.valuecoding.display != ''
     ),
 
@@ -31,39 +31,22 @@
             s.id AS id,
             '1' AS priority,
             'detailed' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS race_code,
             ext_child.ext.valuecoding.display AS race_display
         FROM
             patient AS s,
-            UNNEST(extension) AS ext_parent (ext),
+            UNNEST(s.extension) AS ext_parent (ext),
             UNNEST(ext_parent.ext.extension) AS ext_child (ext)
         WHERE
             ext_parent.ext.url = 'http://hl7.org/fhir/us/core/StructureDefinition/us-core-race'
             AND ext_child.ext.url = 'detailed'
             AND ext_child.ext.valuecoding.display != ''
     ),
 
-    system_text AS (
-        SELECT DISTINCT
-            s.id AS id,
-            '2' AS priority,
-            'text' AS system, -- noqa: RF04
-            ext_child.ext.valuecoding.code AS race_code,
-            ext_child.ext.valuecoding.display AS race_display
-        FROM
-            patient AS s,
-            UNNEST(extension) AS ext_parent (ext),
-            UNNEST(ext_parent.ext.extension) AS ext_child (ext)
-        WHERE
-            ext_parent.ext.url = 'http://hl7.org/fhir/us/core/StructureDefinition/us-core-race'
-            AND ext_child.ext.url = 'text'
-            AND ext_child.ext.valuecoding.display != ''
-    ),
-
     union_table AS (
         SELECT
             id,
             priority,
             system,
             race_code,
             race_display
@@ -72,22 +55,14 @@
         SELECT
             id,
             priority,
             system,
             race_code,
             race_display
         FROM system_detailed
-        UNION
-        SELECT
-            id,
-            priority,
-            system,
-            race_code,
-            race_display
-        FROM system_text
         
         ORDER BY id, priority
     )
 
     SELECT
         id,
         system,
@@ -114,15 +89,15 @@
                             race_display
                         )
                     ), '; '
                 )
             ) AS race_display,
             ROW_NUMBER()
                 OVER (
-                    PARTITION BY id, system
+                    PARTITION BY id
                     ORDER BY priority ASC
                 ) AS available_priority
         FROM union_table
         GROUP BY id, system, priority
     )
     WHERE available_priority = 1
 );
@@ -137,15 +112,15 @@
             s.id AS id,
             '0' AS priority,
             'ombCategory' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS ethnicity_code,
             ext_child.ext.valuecoding.display AS ethnicity_display
         FROM
             patient AS s,
-            UNNEST(extension) AS ext_parent (ext),
+            UNNEST(s.extension) AS ext_parent (ext),
             UNNEST(ext_parent.ext.extension) AS ext_child (ext)
         WHERE
             ext_parent.ext.url = 'http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity'
             AND ext_child.ext.url = 'ombCategory'
             AND ext_child.ext.valuecoding.display != ''
     ),
 
@@ -154,39 +129,22 @@
             s.id AS id,
             '1' AS priority,
             'detailed' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS ethnicity_code,
             ext_child.ext.valuecoding.display AS ethnicity_display
         FROM
             patient AS s,
-            UNNEST(extension) AS ext_parent (ext),
+            UNNEST(s.extension) AS ext_parent (ext),
             UNNEST(ext_parent.ext.extension) AS ext_child (ext)
         WHERE
             ext_parent.ext.url = 'http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity'
             AND ext_child.ext.url = 'detailed'
             AND ext_child.ext.valuecoding.display != ''
     ),
 
-    system_text AS (
-        SELECT DISTINCT
-            s.id AS id,
-            '2' AS priority,
-            'text' AS system, -- noqa: RF04
-            ext_child.ext.valuecoding.code AS ethnicity_code,
-            ext_child.ext.valuecoding.display AS ethnicity_display
-        FROM
-            patient AS s,
-            UNNEST(extension) AS ext_parent (ext),
-            UNNEST(ext_parent.ext.extension) AS ext_child (ext)
-        WHERE
-            ext_parent.ext.url = 'http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity'
-            AND ext_child.ext.url = 'text'
-            AND ext_child.ext.valuecoding.display != ''
-    ),
-
     union_table AS (
         SELECT
             id,
             priority,
             system,
             ethnicity_code,
             ethnicity_display
@@ -195,22 +153,14 @@
         SELECT
             id,
             priority,
             system,
             ethnicity_code,
             ethnicity_display
         FROM system_detailed
-        UNION
-        SELECT
-            id,
-            priority,
-            system,
-            ethnicity_code,
-            ethnicity_display
-        FROM system_text
         
         ORDER BY id, priority
     )
 
     SELECT
         id,
         system,
@@ -237,15 +187,15 @@
                             ethnicity_display
                         )
                     ), '; '
                 )
             ) AS ethnicity_display,
             ROW_NUMBER()
                 OVER (
-                    PARTITION BY id, system
+                    PARTITION BY id
                     ORDER BY priority ASC
                 ) AS available_priority
         FROM union_table
         GROUP BY id, system, priority
     )
     WHERE available_priority = 1
 );
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql` & `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/reference_sql/count_core.sql` & `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/count_core.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/setup.sql` & `cumulus_library-2.1.0/cumulus_library/studies/core/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/core/study_period.sql` & `cumulus_library-2.1.0/cumulus_library/studies/core/study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/discovery/code_definitions.py` & `cumulus_library-2.1.0/cumulus_library/studies/discovery/code_definitions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # A collection of codes & codeableConcepts to extract available codes from.
 
+from cumulus_library.template_sql import sql_utils
 
 code_list = [
     # Condition
     {
         "table_name": "condition",
         "column_hierarchy": [("category", list), ("coding", list)],
     },
@@ -20,14 +21,15 @@
         "table_name": "documentreference",
         "column_hierarchy": [("category", list), ("coding", list)],
     },
     # Encounter
     {
         "table_name": "encounter",
         "column_hierarchy": [("class", dict)],
+        "expected": sql_utils.CODING,
     },
     {
         "table_name": "encounter",
         "column_hierarchy": [("type", list), ("coding", list)],
     },
     {
         "table_name": "encounter",
@@ -44,14 +46,15 @@
     {
         "table_name": "encounter",
         "column_hierarchy": [
             ("hospitalization", dict),
             ("dischargedisposition", dict),
             ("coding", list),
         ],
+        "expected": {"dischargedisposition": sql_utils.CODEABLE_CONCEPT},
     },
     # Medication
     {
         "table_name": "medication",
         "column_hierarchy": [("codecodeableconcept", dict), ("coding", list)],
     },
     {
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/discovery/code_detection.py` & `cumulus_library-2.1.0/cumulus_library/studies/discovery/code_detection.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 """ Module for generating encounter codeableConcept table"""
 
-from cumulus_library import base_table_builder, base_utils
+from cumulus_library import base_table_builder, base_utils, databases
 from cumulus_library.studies.discovery import code_definitions
 from cumulus_library.studies.discovery.discovery_templates import discovery_templates
 from cumulus_library.template_sql import sql_utils
 
 
 class CodeDetectionBuilder(base_table_builder.BaseTableBuilder):
     display_text = "Selecting unique code systems..."
 
-    def _check_coding_against_db(self, code_source, schema, cursor):
+    def _check_coding_against_db(self, code_source, schema, cursor, parser):
         """selects the appropriate DB query to run"""
 
         return sql_utils.is_field_populated(
             schema=schema,
             source_table=code_source["table_name"],
             hierarchy=code_source["column_hierarchy"],
-            expected=sql_utils.CODING,
+            expected=code_source.get("expected"),
             cursor=cursor,
+            parser=parser,
         )
 
-    def _check_codes_in_fields(self, code_sources: list[dict], schema, cursor) -> dict:
+    def _check_codes_in_fields(
+        self, code_sources: list[dict], schema, cursor, parser
+    ) -> dict:
         """checks if Coding/CodeableConcept fields are present and populated"""
 
         with base_utils.get_progress_bar() as progress:
             task = progress.add_task(
                 "Discovering available coding systems...",
                 total=len(code_sources),
             )
             for code_source in code_sources:
                 code_source["has_data"] = self._check_coding_against_db(
-                    code_source, schema, cursor
+                    code_source, schema, cursor, parser
                 )
                 progress.advance(task)
         return code_sources
 
-    def prepare_queries(self, cursor: object, schema: str, *args, **kwargs):
+    def prepare_queries(
+        self,
+        cursor: databases.DatabaseCursor,
+        schema: str,
+        parser: databases.DatabaseParser = None,
+        *args,
+        **kwargs,
+    ):
         """Constructs queries related to condition codeableConcept
 
         :param cursor: A database cursor object
         :param schema: the schema/db name, matching the cursor
 
         """
 
@@ -53,12 +63,12 @@
                 )
             code_source = {
                 "has_data": False,
             }
             for key in code_definition.keys():
                 code_source[key] = code_definition[key]
             code_sources.append(code_source)
-        code_sources = self._check_codes_in_fields(code_sources, schema, cursor)
+        code_sources = self._check_codes_in_fields(code_sources, schema, cursor, parser)
         query = discovery_templates.get_code_system_pairs(
             "discovery__code_sources", code_sources
         )
         self.queries.append(query)
```

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py` & `cumulus_library-2.1.0/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/discovery/reference_sql/code_detection.sql` & `cumulus_library-2.1.0/cumulus_library/studies/discovery/reference_sql/code_detection.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/template/counts.sql` & `cumulus_library-2.1.0/cumulus_library/studies/template/counts.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-2.1.0/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/template/manifest.toml` & `cumulus_library-2.1.0/cumulus_library/studies/template/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/template/setup.sql` & `cumulus_library-2.1.0/cumulus_library/studies/template/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/vocab/ICD10CM_2023AA.bsv` & `cumulus_library-2.1.0/cumulus_library/studies/vocab/icd/ICD10CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/vocab/ICD10PCS_2023AA.bsv` & `cumulus_library-2.1.0/cumulus_library/studies/vocab/icd/ICD10PCS_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/studies/vocab/ICD9CM_2023AA.bsv` & `cumulus_library-2.1.0/cumulus_library/studies/vocab/icd/ICD9CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/study_parser.py` & `cumulus_library-2.1.0/cumulus_library/study_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -325,14 +325,16 @@
                 cursor.execute(drop_view_table)
 
     def _load_and_execute_builder(
         self,
         filename: str,
         cursor: databases.DatabaseCursor,
         schema: str,
+        *,
+        config: base_utils.StudyConfig,
         verbose: bool = False,
         drop_table: bool = False,
         parser: databases.DatabaseParser = None,
         write_reference_sql: bool = False,
         doc_str: str | None = None,
     ) -> None:
         """Loads a table builder from a file.
@@ -378,120 +380,143 @@
 
         # We'll get the subclass, initialize it, run the executor code, and then
         # remove it so it doesn't interfere with the next python module to
         # execute, since the subclass would otherwise hang around.
         table_builder_class = table_builder_subclasses[0]
         table_builder = table_builder_class()
         if write_reference_sql:
-            table_builder.prepare_queries(cursor, schema, parser=parser)
+            table_builder.prepare_queries(cursor, schema, parser=parser, config=config)
             table_builder.comment_queries(doc_str=doc_str)
             new_filename = pathlib.Path(f"{filename}").stem + ".sql"
             table_builder.write_queries(
                 path=pathlib.Path(f"{self._study_path}/reference_sql/" + new_filename)
             )
         else:
             table_builder.execute_queries(
-                cursor, schema, verbose=verbose, drop_table=drop_table, parser=parser
+                cursor,
+                schema,
+                verbose=verbose,
+                drop_table=drop_table,
+                parser=parser,
+                config=config,
             )
 
         # After running the executor code, we'll remove
         # it so it doesn't interfere with the next python module to
         # execute, since the subclass would otherwise hang around.
         del sys.modules[table_builder_module.__name__]
         del table_builder_module
 
     def run_protected_table_builder(
-        self, cursor: databases.DatabaseCursor, schema: str, verbose: bool = False
+        self,
+        cursor: databases.DatabaseCursor,
+        schema: str,
+        *,
+        config: base_utils.StudyConfig,
+        verbose: bool = False,
     ) -> None:
         """Creates protected tables for persisting selected data across runs
 
         :param cursor: A DatabaseCursor object
         :param schema: The name of the schema to write tables to
         :param verbose: toggle from progress bar to query output
         """
         ptb = protected_table_builder.ProtectedTableBuilder()
         ptb.execute_queries(
             cursor,
             schema,
             verbose,
             study_name=self._study_config.get("study_prefix"),
             study_stats=self._study_config.get("statistics_config"),
+            config=config,
         )
 
     def run_table_builder(
         self,
         cursor: databases.DatabaseCursor,
         schema: str,
+        *,
+        config: base_utils.StudyConfig,
         verbose: bool = False,
         parser: databases.DatabaseParser = None,
     ) -> None:
         """Loads modules from a manifest and executes code via BaseTableBuilder
 
         :param cursor: A DatabaseCursor object
         :param schema: The name of the schema to write tables to
         :param verbose: toggle from progress bar to query output
         """
         for file in self.get_table_builder_file_list():
             self._load_and_execute_builder(
-                file, cursor, schema, verbose=verbose, parser=parser
+                file, cursor, schema, verbose=verbose, parser=parser, config=config
             )
 
     def run_counts_builders(
-        self, cursor: databases.DatabaseCursor, schema: str, verbose: bool = False
+        self,
+        cursor: databases.DatabaseCursor,
+        schema: str,
+        *,
+        config: base_utils.StudyConfig,
+        verbose: bool = False,
     ) -> None:
         """Loads counts modules from a manifest and executes code via BaseTableBuilder
 
         While a count is a form of statistics, it is treated separately from other
         statistics because it is, by design, always going to be static against a
         given dataset, where other statistical methods may use sampling techniques
         or adjustable input parameters that may need to be preserved for later review.
 
         :param cursor: A DatabaseCursor object
         :param schema: The name of the schema to write tables to
         :param verbose: toggle from progress bar to query output
         """
         for file in self.get_counts_builder_file_list():
-            self._load_and_execute_builder(file, cursor, schema, verbose=verbose)
+            self._load_and_execute_builder(
+                file, cursor, schema, verbose=verbose, config=config
+            )
 
     def run_statistics_builders(
         self,
         cursor: databases.DatabaseCursor,
         schema: str,
+        *,
+        config: base_utils.StudyConfig,
         verbose: bool = False,
-        stats_build: bool = False,
     ) -> None:
         """Loads statistics modules from toml definitions and executes
 
         :param cursor: A DatabaseCursor object
         :param schema: The name of the schema to write tables to
         :keyword verbose: toggle from progress bar to query output
         :keyword stats_build: If true, will run statistical sampling & table generation
         """
-        if not stats_build:
+        if not config.stats_build:
             return
         for file in self.get_statistics_file_list():
             # This open is a bit redundant with the open inside of the PSM builder,
             # but we're letting it slide so that builders function similarly
             # across the board
             safe_timestamp = base_utils.get_tablename_safe_iso_timestamp()
             toml_path = pathlib.Path(f"{self._study_path}/{file}")
             with open(toml_path, encoding="UTF-8") as file:
                 config = toml.load(file)
                 config_type = config["config_type"]
                 target_table = config["target_table"]
             if config_type == "psm":
                 builder = psm.PsmBuilder(
-                    toml_path, self.data_path / f"{self.get_study_prefix()}/psm"
+                    toml_path,
+                    self.data_path / f"{self.get_study_prefix()}/psm",
+                    config=config,
                 )
             else:
                 raise errors.StudyManifestParsingError(
                     f"{toml_path} references an invalid statistics type {config_type}."
                 )
             builder.execute_queries(
-                cursor, schema, verbose, table_suffix=safe_timestamp
+                cursor, schema, verbose, table_suffix=safe_timestamp, config=config
             )
 
             insert_query = base_templates.get_insert_into_query(
                 f"{self.get_study_prefix()}__{enums.ProtectedTables.STATISTICS.value}",
                 [
                     "study_name",
                     "library_version",
@@ -514,30 +539,40 @@
             cursor.execute(insert_query)
 
     def run_matching_table_builder(
         self,
         cursor: databases.DatabaseCursor,
         schema: str,
         builder: str,
+        *,
+        config: base_utils.StudyConfig,
         verbose: bool = False,
         parser: databases.DatabaseParser = None,
     ):
         """targets all table builders matching a target string for running"""
         all_generators = self.get_all_generators()
         for file in all_generators:
             if builder and file.find(builder) == -1:
                 continue
             self._load_and_execute_builder(
-                file, cursor, schema, verbose=verbose, drop_table=True, parser=parser
+                file,
+                cursor,
+                schema,
+                verbose=verbose,
+                drop_table=True,
+                parser=parser,
+                config=config,
             )
 
     def run_generate_sql(
         self,
         cursor: databases.DatabaseCursor,
         schema: str,
+        *,
+        config: base_utils.StudyConfig,
         builder: str | None = None,
         parser: databases.DatabaseParser = None,
         verbose: bool = False,
     ) -> None:
         """Generates reference SQL from builders listed in the manifest
 
         :param cursor: A DatabaseCursor object
@@ -560,14 +595,15 @@
                 file,
                 cursor,
                 schema,
                 parser=parser,
                 write_reference_sql=True,
                 doc_str=doc_str,
                 verbose=verbose,
+                config=config,
             )
 
     def run_generate_markdown(
         self,
         cursor: databases.DatabaseCursor,
         schema: str,
         parser: databases.DatabaseParser = None,
@@ -615,14 +651,16 @@
         writer.stream = file
         writer.write_table()
         file.write("\n\n")
 
     def build_study(
         self,
         cursor: databases.DatabaseCursor,
+        *,
+        config: base_utils.StudyConfig,
         verbose: bool = False,
         continue_from: str | None = None,
     ) -> list:
         """Creates tables in the schema by iterating through the sql_config.file_names
 
         :param cursor: A DatabaseCursor object
         :param schema: The name of the schema to write tables to
@@ -646,14 +684,15 @@
             )
             self._execute_build_queries(
                 cursor,
                 verbose,
                 queries,
                 progress,
                 task,
+                config,
             )
         return queries
 
     def _query_error(self, query_and_filename: list, exit_message: str) -> None:
         print(
             "An error occured executing the following query in ",
             f"{query_and_filename[1]}:",
@@ -667,14 +706,15 @@
     def _execute_build_queries(
         self,
         cursor: databases.DatabaseCursor,
         verbose: bool,
         queries: list,
         progress: Progress,
         task: TaskID,
+        config: base_utils.StudyConfig,
     ) -> None:
         """Handler for executing create table queries and displaying console output.
 
         :param cursor: A DatabaseCursor object
         :param verbose: toggle from progress bar to query output
         :param queries: a list of queries read from files in sql_config.file_names
         :param progress: a rich progress bar renderer
```

### Comparing `cumulus_library-2.0.1/cumulus_library/template_sql/base_templates.py` & `cumulus_library-2.1.0/cumulus_library/template_sql/base_templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import enum
 import pathlib
 
 import jinja2
 import pandas
 
+from cumulus_library import db_config
 from cumulus_library.template_sql import sql_utils
 
 
 class TableView(enum.Enum):
     """Convenience enum for building drop queries"""
 
     TABLE = "TABLE"
@@ -32,15 +33,15 @@
     with open(f"{path or base_path}/{filename_stem}.sql.jinja") as file:
         template = file.read()
         macro_paths = [base_path / "shared_macros"]
         if path:
             macro_paths.append(path)
         loader = jinja2.FileSystemLoader(macro_paths)
         env = jinja2.Environment(loader=loader).from_string(template)
-        return env.render(**kwargs)
+        return env.render(**kwargs, db_type=db_config.db_type)
 
 
 # All remaining functions are context-specific calls aimed at providing
 # guidance around table creation for commonly used SQL functions
 
 
 def get_alias_table_query(source_table: str, target_table: str):
@@ -75,17 +76,21 @@
         source_table=config.source_table,
         source_id=config.source_id,
         column_name=config.column_hierarchy[-1][0],
         parent_field=None
         if len(config.column_hierarchy) == 1
         else config.column_hierarchy[0][0],
         is_array=(config.column_hierarchy[0][1] == list),
+        child_is_array=False
+        if len(config.column_hierarchy) == 1
+        else config.column_hierarchy[1][1] == list,
         target_table=config.target_table,
         filter_priority=config.filter_priority,
         code_systems=config.code_systems,
+        extra_fields=config.extra_fields or [],
     )
 
 
 def get_coding_denormalize_query(
     config: sql_utils.CodingConfig,
 ) -> str:
     """extracts codings from a specified table.
@@ -147,14 +152,49 @@
         "create_view_as",
         view_name=view_name,
         dataset=dataset,
         view_cols=view_cols,
     )
 
 
+def get_ctas_from_parquet_query(
+    schema_name: str,
+    table_name: str,
+    local_location: str,
+    remote_location: str,
+    table_cols: list[str],
+    remote_table_cols_types: list[str],
+) -> str:
+    """Generates a create table as query using a directory of parquet files as a source
+
+    This function will generate an appropriate query for the underlying DB.
+    Not all params are used by each type of database.
+
+    :param schema_name: (athena) The schema to create the table in
+    :param table_name: (all) The name of the athena table to create
+    :param local_location: (duckdb) A directory containing parquet files to group
+        into a table
+    :param remote_location: (athena) An S3 URL to a directory containing parquert
+        fiels to group into a table
+    :param table_cols: (all) names of fields in your parquet to use as SQL columns
+    :param remote_table_cols_types: (athena) The types to assign to the columns
+        created in athena. Note that these should not be SQL types, but instead
+        should be parquet types.
+    """
+    return get_base_template(
+        "ctas_from_parquet",
+        schema_name=schema_name,
+        table_name=table_name,
+        local_location=local_location,
+        remote_location=remote_location,
+        table_cols=table_cols,
+        remote_table_cols_types=remote_table_cols_types,
+    )
+
+
 def get_ctas_query(
     schema_name: str, table_name: str, dataset: list[list[str]], table_cols: list[str]
 ) -> str:
     """Generates a create table as query for inserting static data into athena
 
     Note that unlike other queries, the nature of the CTAS implementation in athena
     requires a schema name. This schema name should match the schema of your cursor,
```

### Comparing `cumulus_library-2.0.1/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/template_sql/coding_denormalize.sql.jinja`

 * *Files 20% similar despite different names*

```diff
@@ -5,39 +5,23 @@
 
     system_{{ column_name }}_{{ loop.index0 }} AS (
         SELECT DISTINCT
             s.{{ source_id }} AS id,
             {%- if filter_priority %}
             '{{ loop.index0 }}' AS priority,
             {%- endif %}
-            u.codeable_concept.code,
-            u.codeable_concept.display,
-            u.codeable_concept.system AS code_system
+            u.parent_col.{{ column_name }}.code,
+            u.parent_col.{{ column_name }}.display,
+            u.parent_col.{{ column_name }}.system AS code_system
         FROM
-        {#- Temp workaround - to be reworked by generic DN -#}
-        {%- if parent_field != None %}
             {{ source_table }} AS s,
-        {%- if is_array %}
-            UNNEST(s.{{ parent_field }}) AS parent (parent_row),
-            UNNEST(parent.parent_row.{{ column_name }}.coding) AS u (codeable_concept)
-        {%- else %}
-            UNNEST(s.{{ parent_field }}.{{ column_name }}.coding) AS u (codeable_concept)
-        {%- endif %}
-        {%- else %}
-            {{ source_table }} AS s,
-        {%- if is_array %}
-            UNNEST(s.{{ column_name }}) AS cc (cc_row),
-            UNNEST(cc.cc_row.coding) AS u (codeable_concept)
-        {%- else %}
-            UNNEST(s.{{ column_name }}.coding) AS u (codeable_concept)
-        {%- endif %}
-        {%- endif %}
+            UNNEST(s.{{ parent_field }}) AS u (parent_col)
         {%- if filter_priority %}
         WHERE
-            u.codeable_concept.system LIKE '{{ system }}'
+            u.parent_col.{{ column_name }}.system LIKE '{{ system }}'
         {%- endif %}
     ), --noqa: LT07
     {%- endfor %}
 
     union_table AS (
         {%- for system in code_systems %}
         SELECT
```

### Comparing `cumulus_library-2.0.1/cumulus_library/template_sql/create_view_as.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/template_sql/create_view_as.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/template_sql/ctas.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/template_sql/ctas.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/template_sql/extension_denormalize.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/template_sql/extension_denormalize.sql.jinja`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
             s.{{ source_id }} AS id,
             '{{ loop.index0 }}' AS priority,
             '{{ system }}' AS system, -- noqa: RF04
             ext_child.ext.valuecoding.code AS {{ target_col_prefix }}_code,
             ext_child.ext.valuecoding.display AS {{ target_col_prefix }}_display
         FROM
             {{ source_table }} AS s,
-            UNNEST(extension) AS ext_parent (ext),
+            UNNEST(s.extension) AS ext_parent (ext),
             UNNEST(ext_parent.ext.extension) AS ext_child (ext)
         WHERE
             ext_parent.ext.url = '{{ fhir_extension }}'
             AND ext_child.ext.url = '{{ system }}'
             AND ext_child.ext.valuecoding.display != ''
     ),
     {%- endfor %}
@@ -68,15 +68,15 @@
             LOWER({{ target_col_prefix }}_code) AS {{ target_col_prefix }}_code,
             LOWER(
                 {{ target_col_prefix }}_display
             ) AS {{ target_col_prefix }}_display,
             {%- endif %}
             ROW_NUMBER()
                 OVER (
-                    PARTITION BY id, system
+                    PARTITION BY id
                     ORDER BY priority ASC
                 ) AS available_priority
         FROM union_table
         GROUP BY id, system, priority
     )
     WHERE available_priority = 1
 );
```

### Comparing `cumulus_library-2.0.1/cumulus_library/template_sql/insert_into.sql.jinja` & `cumulus_library-2.1.0/cumulus_library/template_sql/insert_into.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.0.1/cumulus_library/template_sql/sql_utils.py` & `cumulus_library-2.1.0/cumulus_library/template_sql/sql_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,19 +10,23 @@
 """
 import abc
 from dataclasses import dataclass, field
 
 from cumulus_library import base_utils, databases
 from cumulus_library.template_sql import base_templates
 
-# TODO: this should be reworked as part of an evenutal typesystem refactor/FHIRClient
-# cutover, possibly tied to a database parser update
-
-CODING = ["code", "system", "display"]
-CODEABLE_CONCEPT = ["coding", "code", "system", "display"]
+# *** Some convenience constants for providing to validate_schema() ***
+# * Only include necessary fields that we actually use.
+# * If any sub-field is not present, we may ignore the parent-field.
+# * Though, cumulus-fhir-support does guarantee a full Coding or Concept.
+CODING = ["code", "display", "system", "userSelected", "version"]
+# If you think you need CODEABLE_CONCEPT, you probably need a de-normalization table
+# instead, since CodeableConcepts can contain multiple entries.
+CODEABLE_CONCEPT = {"coding": CODING, "text": {}}
+REFERENCE = ["reference"]
 
 
 @dataclass(kw_only=True)
 class BaseConfig(abc.ABC):
     """Abstract ase class for handling table detection/denormalization"""
 
     source_table: str = None
@@ -41,28 +45,33 @@
     :keyword target_table: the name of the table to create
     :keyword source_id: the id field to use in the new table (default: 'id')
     :keyword filter_priority: If true, will use code systems to select a single code,
       in preference order, for use as a display value.
     :keyword code_systems: a list of strings matching the start of the systems field,
       in preference order, for selecting data for filtering. This should not be set
       if filter_priority is false.
+    :keyword expected: a schema fragment for what the shape of this field should be.
+      If any bit of this schema fragment is not present, there will be no results.
+    :keyword extra_fields: extra fields to include, as siblings of the concept.
+      It's a list of tuples (field, alias).
     """
 
     column_hierarchy: list[tuple]
     filter_priority: bool = False
     code_systems: list = None
-    expected: list = field(default_factory=lambda: CODEABLE_CONCEPT)
+    expected: list | dict = field(default_factory=lambda: CODEABLE_CONCEPT)
+    extra_fields: list[tuple] = None  # candidate for moving into base config
 
 
 @dataclass(kw_only=True)
 class CodingConfig(BaseConfig):
     column_hierarchy: list[tuple]
     filter_priority: bool = False
     code_systems: list = None
-    expected: list = field(default_factory=lambda: CODING)
+    expected: list | dict = field(default_factory=lambda: CODING)
 
 
 @dataclass(kw_only=True)
 class ExtensionConfig(BaseConfig):
     """convenience class for holding parameters for generating extension tables.
 
     :keyword source_table: the table to extract extensions from
@@ -79,14 +88,15 @@
     ext_systems: list[str]
     is_array: bool = False
 
 
 def _check_data_in_fields(
     schema: str,
     cursor: databases.DatabaseCursor,
+    parser: databases.DatabaseParser,
     code_sources: list[CodeableConceptConfig],
 ) -> dict:
     """checks if CodeableConcept fields actually have data available
 
     CodeableConcept fields are mostly optional in the FHIR spec, and may be arrays
     or single objects. Additionally, the null representation can be inconsistent,
     depending on how the data is provided from an EHR and how the ETL manages
@@ -111,48 +121,70 @@
             # detect valid data is in the DB
             total=len(code_sources),
         )
         for code_source in code_sources:
             code_source.has_data = is_field_populated(
                 schema=schema,
                 cursor=cursor,
+                parser=parser,
                 source_table=code_source.source_table,
                 hierarchy=code_source.column_hierarchy,
                 expected=code_source.expected,
             )
             progress.advance(task)
     return code_sources
 
 
 def denormalize_complex_objects(
     schema: str,
     cursor: databases.DatabaseCursor,
+    parser: databases.DatabaseParser,
     code_sources: list[BaseConfig],
 ):
     queries = []
-    code_sources = _check_data_in_fields(schema, cursor, code_sources)
+    code_sources = _check_data_in_fields(schema, cursor, parser, code_sources)
     for code_source in code_sources:
         # TODO: This method of pairing classed config objects to
         # specific queries should be considered temporary. This should be
         # replaced at some point by a more generic table schema traversal/
         # generic jinja template approach.
         match code_source:
             case CodeableConceptConfig():
                 if code_source.has_data:
                     queries.append(
                         base_templates.get_codeable_concept_denormalize_query(
                             code_source
                         )
                     )
                 else:
+                    table_cols = [
+                        "id",
+                        "row",
+                        "code",
+                        "code_system",
+                        "display",
+                        "userSelected",
+                    ]
+                    col_types = [
+                        "varchar",
+                        "bigint",
+                        "varchar",
+                        "varchar",
+                        "varchar",
+                        "boolean",
+                    ]
+                    if code_source.extra_fields:
+                        table_cols += [f[1] for f in code_source.extra_fields]
+                        col_types += ["varchar"] * len(code_source.extra_fields)
                     queries.append(
                         base_templates.get_ctas_empty_query(
                             schema_name=schema,
                             table_name=code_source.target_table,
-                            table_cols=["id", "code", "code_system", "display"],
+                            table_cols=table_cols,
+                            table_cols_types=col_types,
                         )
                     )
             case CodingConfig():
                 if code_source.has_data:
                     queries.append(
                         base_templates.get_coding_denormalize_query(code_source)
                     )
@@ -164,47 +196,63 @@
                             table_cols=["id", "code", "code_system", "display"],
                         )
                     )
 
     return queries
 
 
+def validate_schema(
+    cursor: databases.DatabaseCursor,
+    schema: str,
+    expected_table_cols: dict,
+    parser: databases.DatabaseParser,
+) -> dict:
+    validated_schema = {}
+    for table, cols in expected_table_cols.items():
+        query = base_templates.get_column_datatype_query(schema, table, cols.keys())
+        table_schema = cursor.execute(query).fetchall()
+        validated_schema[table] = parser.validate_table_schema(cols, table_schema)
+    return validated_schema
+
+
 def is_field_populated(
     *,
     schema: str,
     cursor: databases.DatabaseCursor,
+    parser: databases.DatabaseParser,
     source_table: str,
     hierarchy: list[tuple],
-    expected: list | None = None,
+    expected: list | dict | None = None,
 ) -> bool:
     """Traverses a complex field and determines if it exists and has data
 
+    Non-core studies that rely on the core tables shouldn't need this method.
+    This is just to examine the weird and wonderful world of the raw FHIR tables.
+
     :keyword schema: The schema/database name
     :keyword cursor: a PEP-249 compliant database cursor
     :keyword source_table: The table to query against
     :keyword hierarchy: a list of tuples defining the FHIR path to the element.
         Each tuple should be of the form ('element_name', dict | list), where
         a dict is a bare nested object and a list is an array object
     :keyword expected: a list of elements that should be present in the field.
         If none, we assume it is a CodeableConcept.
     :returns: a boolean indicating if valid data is present.
     """
-    if not _check_schema_if_exists(
+    if not is_field_present(
         schema=schema,
         cursor=cursor,
+        parser=parser,
         source_table=source_table,
         source_col=hierarchy[0][0],
         expected=expected,
-        nested_field=hierarchy[-1][0] if len(hierarchy) > 1 else None,
     ):
         return False
     unnests = []
     source_field = []
-    last_table_alias = None
-    last_row_alias = None
     for element in hierarchy:
         if element[1] == list:
             unnests.append(
                 {
                     "source_col": ".".join([*source_field, element[0]]),
                     "table_alias": f"{element[0]}_table",
                     "row_alias": f"{element[0]}_row",
@@ -225,52 +273,44 @@
     )
     res = cursor.execute(query).fetchall()
     if len(res) == 0:
         return False
     return True
 
 
-def _check_schema_if_exists(
+def is_field_present(
     *,
     schema: str,
     cursor: databases.DatabaseCursor,
+    parser: databases.DatabaseParser,
     source_table: str,
     source_col: str,
-    expected: str | None = None,
-    nested_field: str | None = None,
+    expected: list | dict | None = None,
 ) -> bool:
     """Validation check for a column existing, and having the expected schema
 
     :keyword schema: The schema/database name
     :keyword cursor: a PEP-249 compliant database cursor
+    :keyword parser: a database schema parser
     :keyword source_table: The table to query against
     :keyword source_col: The column to check the schema against
     :keyword expected: a list of elements that should be present in source_col.
         If none, we assume it is a CodeableConcept.
     :returns: a boolean indicating if the schema was found.
     """
-    try:
-        query = base_templates.get_is_table_not_empty_query(source_table, source_col)
-        cursor.execute(query)
-        if cursor.fetchone() is None:
-            return False
+    if expected is None:
+        expected = CODEABLE_CONCEPT
 
-        query = base_templates.get_column_datatype_query(
-            schema, source_table, [source_col]
-        )
-        cursor.execute(query)
-        schema_str = str(cursor.fetchone()[1])
-        if expected is None:
-            expected = CODEABLE_CONCEPT
-        # TODO: this naievely checks a column for:
-        #   - containing the target field
-        #   - containing the expected elements
-        # but it does not check the elements are actually associated with that field.
-        # This should be revisited once we've got better database parsing logic in place
-        if nested_field:
-            expected = [nested_field, *expected]
-        if any(x not in schema_str.lower() for x in expected):
-            return False
-        return True
+    table_cols = {source_table: {source_col: expected}}
+    schema = validate_schema(cursor, schema, table_cols, parser)
 
-    except Exception:
-        return False
+    def _get_all_values(d: dict) -> list:
+        all_values = []
+        for value in d.values():
+            if isinstance(value, dict):
+                all_values += _get_all_values(value)
+            else:
+                all_values.append(value)
+        return all_values
+
+    all_schema_values = _get_all_values(schema)
+    return all(all_schema_values)
```

### Comparing `cumulus_library-2.0.1/cumulus_library/upload.py` & `cumulus_library-2.1.0/cumulus_library/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,28 +38,27 @@
         print("headers", prefetch_res.request.headers)
         print("body", prefetch_res.request.body, "\n")
         print("response")
         print(prefetch_res.json(), "\n")
 
     if prefetch_res.status_code != 200:
         print("Invalid user/site id")
-        raise requests.RequestException(response=prefetch_res)
+        prefetch_res.raise_for_status()
     res_body = prefetch_res.json()
-
     with open(file_path, "rb") as data_file:
         files = {"file": (file_name, data_file)}
         upload_req = requests.Request(
             "POST", res_body["url"], data=res_body["fields"], files=files
         ).prepare()
         if not args["preview"]:
             s = requests.Session()
             upload_res = s.send(upload_req, timeout=60)
             if upload_res.status_code != 204:
                 print(f"Error uploading {study}/{file_name}")
-                raise requests.RequestException(response=upload_res)
+                upload_res.raise_for_status()
         else:
             print("upload_req")
             print("headers", upload_req.headers)
             print("body", upload_req.body, "\n")
     progress.update(file_upload_progress, advance=1)
```

### Comparing `cumulus_library-2.0.1/pyproject.toml` & `cumulus_library-2.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "cumulus-library"
 requires-python = ">= 3.10"
 dependencies = [
     "ctakesclient >= 1.3",
-    "cumulus-fhir-support >= 1",
+    "cumulus-fhir-support >= 1.1",
     "duckdb >= 0.9",
     "fhirclient >= 4.1",
     "Jinja2 > 3",
     "pandas <3, >=2.1.3",
     "psmpy <1, >=0.3.13",
     "pyarrow >= 11.0",
     "pyathena >= 2.23",
@@ -33,15 +33,15 @@
 dev = [
     "ruff == 0.2.1",
     "pre-commit",
 ]
 test = [
     "freezegun",
     "pytest",
-    "requests-mock",
+    "responses"
 ]
 
 [project.urls]
 Home = "https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/"
 Documentation = "https://docs.smarthealthit.org/cumulus/"
 Source = "https://github.com/smart-on-fhir/cumulus-library"
```

### Comparing `cumulus_library-2.0.1/PKG-INFO` & `cumulus_library-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 2.0.1
+Version: 2.1.0
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
 Requires-Python: >= 3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: ctakesclient >= 1.3
-Requires-Dist: cumulus-fhir-support >= 1
+Requires-Dist: cumulus-fhir-support >= 1.1
 Requires-Dist: duckdb >= 0.9
 Requires-Dist: fhirclient >= 4.1
 Requires-Dist: Jinja2 > 3
 Requires-Dist: pandas <3, >=2.1.3
 Requires-Dist: psmpy <1, >=0.3.13
 Requires-Dist: pyarrow >= 11.0
 Requires-Dist: pyathena >= 2.23
@@ -24,15 +24,15 @@
 Requires-Dist: sqlfluff  >= 3
 Requires-Dist: sqlparse >0.4
 Requires-Dist: toml >= 0.10
 Requires-Dist: ruff == 0.2.1 ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: freezegun ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
-Requires-Dist: requests-mock ; extra == "test"
+Requires-Dist: responses ; extra == "test"
 Project-URL: Documentation, https://docs.smarthealthit.org/cumulus/
 Project-URL: Home, https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/
 Project-URL: Source, https://github.com/smart-on-fhir/cumulus-library
 Provides-Extra: dev
 Provides-Extra: test
 
 # Cumulus Library - Core
```

