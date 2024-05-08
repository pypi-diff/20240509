# Comparing `tmp/gemmapy-0.0.2.tar.gz` & `tmp/gemmapy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/vavilov/work/pySDK/package/dist/tmpubbi1x3i/gemmapy-0.0.2.tar", last modified: Mon Nov 14 20:30:35 2022, max compression
+gzip compressed data, was "gemmapy-1.0.0.tar", last modified: Wed May  8 23:49:00 2024, max compression
```

## Comparing `gemmapy-0.0.2.tar` & `gemmapy-1.0.0.tar`

### file list

```diff
@@ -1,116 +1,157 @@
-drwxrwxr-x   0 vavilov   (1001) vavilov   (1001)        0 2022-11-14 20:30:35.000000 gemmapy-0.0.2/
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    11357 2022-08-19 18:47:04.000000 gemmapy-0.0.2/LICENSE.md
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     1457 2022-11-14 20:30:35.000000 gemmapy-0.0.2/PKG-INFO
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     1305 2022-10-14 22:09:44.000000 gemmapy-0.0.2/README.rst
-drwxrwxr-x   0 vavilov   (1001) vavilov   (1001)        0 2022-11-14 20:30:35.000000 gemmapy-0.0.2/gemmapy/
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)       61 2022-08-03 00:06:55.000000 gemmapy-0.0.2/gemmapy/__init__.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    21216 2022-11-14 20:27:46.000000 gemmapy-0.0.2/gemmapy/gemmapy_api.py
-drwxrwxr-x   0 vavilov   (1001) vavilov   (1001)        0 2022-11-14 20:30:35.000000 gemmapy-0.0.2/gemmapy/sdk/
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    12754 2022-10-17 22:43:27.000000 gemmapy-0.0.2/gemmapy/sdk/__init__.py
-drwxrwxr-x   0 vavilov   (1001) vavilov   (1001)        0 2022-11-14 20:30:35.000000 gemmapy-0.0.2/gemmapy/sdk/api/
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)      138 2022-09-08 19:22:46.000000 gemmapy-0.0.2/gemmapy/sdk/api/__init__.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)   176316 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/api/default_api.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    29812 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/api_client.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    13121 2022-10-17 22:43:27.000000 gemmapy-0.0.2/gemmapy/sdk/configuration.py
-drwxrwxr-x   0 vavilov   (1001) vavilov   (1001)        0 2022-11-14 20:30:35.000000 gemmapy-0.0.2/gemmapy/sdk/models/
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    12557 2022-10-17 22:43:27.000000 gemmapy-0.0.2/gemmapy/sdk/models/__init__.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    10120 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/annotation_search_result_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    12808 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/annotation_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     8981 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/api_info_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    24713 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/array_design_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    12505 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/audit_event_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    16174 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/bio_assay_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    12646 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/bio_material_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    10669 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/characteristic_basic_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    11357 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/characteristic_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7068 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/composite_sequence_arg.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     9978 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/composite_sequence_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    12492 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/contrast_result_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7052 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/database_entry_arg.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     9348 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/database_entry_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7016 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/dataset.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7020 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/dataset1.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7020 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/dataset2.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7020 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/dataset3.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7020 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/dataset4.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7020 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/dataset5.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7020 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/dataset6.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7020 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/dataset7.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7020 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/dataset8.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7028 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/dataset_arg.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    19692 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/diff_ex_result_set_summary_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    10881 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/differential_expression_analysis_result_set_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    13623 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/differential_expression_analysis_result_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    17081 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/differential_expression_analysis_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     9073 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/experiment_expression_levels_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    12895 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/experimental_factor_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    30068 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/expression_experiment_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     8945 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/external_database_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    13805 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/factor_value_basic_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    14980 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/factor_value_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    29597 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/geeq_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7004 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/gene.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7008 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/gene1.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7008 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/gene2.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7008 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/gene3.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7008 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/gene4.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7016 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/gene_arg.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     9718 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/gene_element_expressions_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    11834 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/gene_ontology_term_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    12816 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/gene_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7659 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/identifiable_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    10339 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/measurement_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    11177 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/paginated_response_data_object_array_design_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    11339 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/paginated_response_data_object_composite_sequence_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    11933 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/paginated_response_data_object_differential_expression_analysis_result_set_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    11420 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/paginated_response_data_object_expression_experiment_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    10988 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/paginated_response_data_object_gene_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    12091 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/physical_location_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7020 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/platform.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7024 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/platform1.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7024 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/platform2.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7024 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/platform3.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7024 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/platform4.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7024 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/platform5.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7032 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/platform_arg.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7008 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/probe.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7848 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_api_info_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     8200 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_differential_expression_analysis_result_set_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     8063 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_list_annotation_search_result_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7942 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_list_array_design_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7909 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_list_bio_assay_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     8151 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_list_differential_expression_analysis_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     8107 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_list_experiment_expression_levels_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7997 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_list_gene_ontology_term_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7865 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_list_gene_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7997 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_list_physical_location_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7876 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_list_taxon_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7923 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_set_annotation_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7870 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_data_object_simple_svd_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     8485 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/response_error_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7052 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/search_result_type.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    10104 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/search_result_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     8779 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/search_results_response_data_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    10802 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/search_settings_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     9375 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/simple_svd_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     8403 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/sort_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7008 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/taxon.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7012 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/taxon1.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7012 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/taxon2.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7012 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/taxon3.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7012 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/taxon4.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7012 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/taxon5.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7012 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/taxon6.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     7020 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/taxon_arg.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    10723 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/taxon_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     9126 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/vector_element_value_object.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     9042 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/models/well_composed_error_body.py
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)    17616 2022-10-14 21:35:00.000000 gemmapy-0.0.2/gemmapy/sdk/rest.py
-drwxrwxr-x   0 vavilov   (1001) vavilov   (1001)        0 2022-11-14 20:30:35.000000 gemmapy-0.0.2/gemmapy.egg-info/
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     1457 2022-11-14 20:30:35.000000 gemmapy-0.0.2/gemmapy.egg-info/PKG-INFO
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)     4954 2022-11-14 20:30:35.000000 gemmapy-0.0.2/gemmapy.egg-info/SOURCES.txt
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)        1 2022-11-14 20:30:35.000000 gemmapy-0.0.2/gemmapy.egg-info/dependency_links.txt
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)      107 2022-11-14 20:30:35.000000 gemmapy-0.0.2/gemmapy.egg-info/requires.txt
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)        8 2022-11-14 20:30:35.000000 gemmapy-0.0.2/gemmapy.egg-info/top_level.txt
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)       81 2022-06-02 19:33:40.000000 gemmapy-0.0.2/pyproject.toml
--rw-rw-r--   0 vavilov   (1001) vavilov   (1001)      372 2022-11-14 20:30:35.000000 gemmapy-0.0.2/setup.cfg
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-08 23:49:00.396396 gemmapy-1.0.0/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    11357 2024-05-04 04:09:08.000000 gemmapy-1.0.0/LICENSE.md
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     1730 2024-05-08 23:49:00.396396 gemmapy-1.0.0/PKG-INFO
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     1306 2024-05-07 21:06:20.000000 gemmapy-1.0.0/README.rst
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-08 23:49:00.344395 gemmapy-1.0.0/gemmapy/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)       61 2024-05-04 04:09:08.000000 gemmapy-1.0.0/gemmapy/__init__.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    21504 2024-05-08 23:46:56.000000 gemmapy-1.0.0/gemmapy/_processors.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6768 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/_subprocessors.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)      936 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/_validators.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    89458 2024-05-08 00:42:56.000000 gemmapy-1.0.0/gemmapy/gemmapy_api.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-08 23:49:00.348395 gemmapy-1.0.0/gemmapy/sdk/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    12986 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/__init__.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-08 23:49:00.348395 gemmapy-1.0.0/gemmapy/sdk/api/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)      138 2024-05-04 04:09:08.000000 gemmapy-1.0.0/gemmapy/sdk/api/__init__.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)   214827 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/api/default_api.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    25975 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/api_client.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9213 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/configuration.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-08 23:49:00.392396 gemmapy-1.0.0/gemmapy/sdk/models/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    12789 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/__init__.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6156 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/annotation_search_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8608 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/annotation_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9891 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/annotation_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5987 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/api_info_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    24020 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/array_design_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    24987 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/array_design_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8819 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/audit_event_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7478 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/bibliographic_phenotypes_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    16799 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/bibliographic_reference_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    14982 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/bio_assay_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9742 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/bio_material_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10036 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/bio_sequence_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5992 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/category_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7293 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/characteristic_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6624 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/citation_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3104 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/composite_sequence_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6014 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/composite_sequence_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8528 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/contrast_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/database_entry_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5384 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/database_entry_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3052 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/dataset.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/dataset1.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/dataset10.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/dataset2.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/dataset3.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/dataset4.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/dataset5.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/dataset6.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/dataset7.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/dataset8.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/dataset9.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3064 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/dataset_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    15728 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/diff_ex_result_set_summary_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7917 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/differential_expression_analysis_result_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9659 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/differential_expression_analysis_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    14048 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/differential_expression_analysis_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5109 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/experiment_expression_levels_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9358 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/experimental_factor_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    15105 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/expression_experiment_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    28654 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    31623 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/expression_experiment_with_search_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9207 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/external_database_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10910 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/factor_value_basic_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    16266 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/factor_value_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3104 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/filter_arg_array_design.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3168 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/filter_arg_expression_analysis_result_set.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3140 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/filter_arg_expression_experiment.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9152 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/filtered_and_paginated_response_data_object_array_design_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9362 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/filtered_and_paginated_response_data_object_composite_sequence_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10132 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/filtered_and_paginated_response_data_object_differential_expression_analysis_result_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9467 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/filtered_and_paginated_response_data_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8907 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/filtered_and_paginated_response_data_object_gene_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    25633 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/geeq_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3040 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/gene.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/gene1.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/gene2.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/gene3.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/gene4.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3052 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/gene_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5754 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/gene_element_expressions_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7870 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/gene_ontology_term_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6956 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/gene_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     9642 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/gene_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8358 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/limited_response_data_object_annotation_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8389 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/limited_response_data_object_array_design_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/measurement_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3208 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/one_of_search_result_value_object_object_result_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5194 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/ontology_term_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8221 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/paginated_response_data_object_composite_sequence_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8314 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/paginated_response_data_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8127 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/physical_location_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/platform.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/platform1.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/platform2.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/platform3.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/platform4.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3060 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/platform5.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3068 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/platform_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/probe.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/quantitation_type.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3100 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/quantitation_type_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    17466 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/quantitation_type_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10652 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/queried_and_filtered_and_paginated_response_data_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    11276 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/queried_and_filtered_and_paginated_response_data_object_expression_experiment_with_search_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7723 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/queried_and_filtered_response_data_object_category_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7642 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/queried_and_filtered_response_data_object_taxon_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/query_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3884 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_api_info_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4236 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_differential_expression_analysis_result_set_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4099 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_list_annotation_search_result_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3978 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_list_array_design_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3945 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_list_bio_assay_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4187 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_list_differential_expression_analysis_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4143 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_list_experiment_expression_levels_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4033 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_list_gene_ontology_term_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3901 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_list_gene_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4033 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_list_physical_location_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3912 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_list_taxon_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3727 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_long.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3959 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_set_annotation_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4025 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_set_quantitation_type_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3906 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_data_object_simple_svd_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4521 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/response_error_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3088 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/search_result_type.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7682 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/search_result_value_object_expression_experiment_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7127 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/search_result_value_object_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4833 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/search_results_response_data_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6838 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/search_settings_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5411 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/simple_svd_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3096 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/sort_arg_array_design.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3160 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/sort_arg_expression_analysis_result_set.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3132 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/sort_arg_expression_experiment.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3072 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/sort_arg_taxon.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     4439 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/sort_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    10286 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/statement_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3044 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/taxon.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/taxon1.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/taxon2.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/taxon3.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/taxon4.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/taxon5.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3048 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/taxon6.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3056 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/taxon_arg.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     6759 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/taxon_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     8441 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/taxon_with_usage_statistics_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5162 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/vector_element_value_object.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     5078 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/models/well_composed_error_body.py
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)    13649 2024-05-07 20:41:44.000000 gemmapy-1.0.0/gemmapy/sdk/rest.py
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-08 23:49:00.396396 gemmapy-1.0.0/gemmapy.egg-info/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     1730 2024-05-08 23:49:00.000000 gemmapy-1.0.0/gemmapy.egg-info/PKG-INFO
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     7474 2024-05-08 23:49:00.000000 gemmapy-1.0.0/gemmapy.egg-info/SOURCES.txt
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)        1 2024-05-08 23:49:00.000000 gemmapy-1.0.0/gemmapy.egg-info/dependency_links.txt
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)      114 2024-05-08 23:49:00.000000 gemmapy-1.0.0/gemmapy.egg-info/requires.txt
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)        8 2024-05-08 23:49:00.000000 gemmapy-1.0.0/gemmapy.egg-info/top_level.txt
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)       81 2024-05-04 04:09:08.000000 gemmapy-1.0.0/pyproject.toml
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)      404 2024-05-08 23:49:00.396396 gemmapy-1.0.0/setup.cfg
+drwxr-xr-x   0 omancarci (30067) pavlab   (30005)        0 2024-05-08 23:49:00.392396 gemmapy-1.0.0/tests/
+-rw-r--r--   0 omancarci (30067) pavlab   (30005)     3766 2024-05-08 05:16:40.000000 gemmapy-1.0.0/tests/test_basic.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gemmapy-0.0.2/LICENSE.md` & `gemmapy-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gemmapy-0.0.2/PKG-INFO` & `gemmapy-1.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: gemmapy
-Version: 0.0.2
-Summary: a Python Wrapper for the Gemma API
-Keywords: gemma,bioinformatics
-License-File: LICENSE.md
-
 gemmapy: a Python Wrapper for the Gemma API
 ===========================================
 
 This is a Python wrapper for `Gemma <https://gemma.msl.ubc.ca/>`_'s
 RESTful `API <https://gemma.msl.ubc.ca/resources/restapidocs/>`_. Gemma is a web
 site, database and a set of tools for the meta-analysis, re-use and
 sharing of genomics data, currently primarily targeted at the analysis
@@ -16,15 +9,15 @@
 public studies, referencing thousands of published papers.
 
 
 Installation instructions
 -------------------------
 .. This is a content of docs/install.rst. Update it whenever install.rst changes.
    
-The package requires Python3.6+. 
+The package requires Python3.10+. 
 
 #. Install it from a local copy
 
    .. code-block:: bash
 
       git clone git@github.com:PavlidisLab/gemmapy.git
       cd gemmapy
```

### Comparing `gemmapy-0.0.2/README.rst` & `gemmapy-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: gemmapy
+Version: 1.0.0
+Summary: a Python Wrapper for the Gemma API
+Keywords: gemma,bioinformatics
+Requires-Python: >3.10
+License-File: LICENSE.md
+Requires-Dist: certifi>=14.05.14
+Requires-Dist: six>=1.10
+Requires-Dist: python_dateutil>=2.5.3
+Requires-Dist: setuptools>=21.0.0
+Requires-Dist: urllib3>=1.15.1
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: anndata
+Requires-Dist: typing
+
 gemmapy: a Python Wrapper for the Gemma API
 ===========================================
 
 This is a Python wrapper for `Gemma <https://gemma.msl.ubc.ca/>`_'s
 RESTful `API <https://gemma.msl.ubc.ca/resources/restapidocs/>`_. Gemma is a web
 site, database and a set of tools for the meta-analysis, re-use and
 sharing of genomics data, currently primarily targeted at the analysis
@@ -9,15 +26,15 @@
 public studies, referencing thousands of published papers.
 
 
 Installation instructions
 -------------------------
 .. This is a content of docs/install.rst. Update it whenever install.rst changes.
    
-The package requires Python3.6+. 
+The package requires Python3.10+. 
 
 #. Install it from a local copy
 
    .. code-block:: bash
 
       git clone git@github.com:PavlidisLab/gemmapy.git
       cd gemmapy
```

### Comparing `gemmapy-0.0.2/gemmapy/sdk/api/default_api.py` & `gemmapy-1.0.0/gemmapy/sdk/api/default_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gemma RESTful API
 
-    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  Fix return type for `getResultSets` which was incorrectly referring to a renamed VO.  Remove the `security` requirements by default from the specification, which forced the Python package to supply empty credentials. There is currently no privileged endpoints, although some can return additional results.  ## Updates  ### Update 2.5.1  Restore `objectClass` visibility in `AnnotationValueObject`.  Fix incorrect response types for annotations search endpoints returning datasets.  ### Update 2.5.0  Major cleanups were performed in this release in order to stabilize the specification. Numerous properties from Gemma Web that were never intended to be exposed in Gemma REST have been hidden. It's a bit too much to describe in here, but you can navigate to the schemas section below to get a good glance at the models.  Favour `numberOfSomething` instead of `somethingCount` which is clearer. The older names are kept for backward-compatibility, but should be considered deprecated.  Gene aliases and multifunctionality rank are now filled in `GeneValueObject`.  Uniformly use `TaxonValueObject` to represent taxon. This is breaking change for the `ExpressionExperimentValueObject` and `ArrayDesignValueObject` as their `taxon` property will be an `object` instead of a `string`. Properties such as `taxonId` are now deprecated and `taxon.id` should be used instead.  Entities that have IDs now all inherit from `IdentifiableValueObject`. This implies that you can assume the presence of an `id` in a search result `resultObject` attribute for example.  New `/search` endpoint! for an unified search experience. Annotation-based search endpoints under `/annotations` are now deprecated.  New API docs! While not as nice looking, the previous theme will be gradually ported to Swagger UI as we focused on functionality over prettiness for this release.  ### Update 2.4.0 through 2.4.1  Release notes for the 2.4 series were not written down, so I'll try to do my best to recall features that were introduced at that time.  An [OpenAPI](https://www.openapis.org/) specification was introduced and available under `/rest/v2/openapi.json`, although not fully stabilized.  Add a `/resultSets` endpoint to navigate result sets directly, by ID or by dataset.  Add a `/resultSets/{resultSetId}` endpoint to retrieve a specific result set by its ID. This endpoint can be negotiated with an `Accept: text/tab-separated-values` header to obtain a TSV representation.  Add a `/datasets/{dataset}/analyses/differential/resultSets` endpoint that essentially redirect to a specific `/resultSet` endpoint by dataset ID.  Add an endpoint to retrieve preferred raw expression vectors.  ### Update 2.3.4  November 6th, 2018  November 6th [2.3.4] Bug fixes in the dataset search endpoint.  November 5th [2.3.3] Added filtering parameters to dataset search.  October 25th [2.3.2] Changed behavior of the dataset search endpoint to more closely match the Gemma web interface.  October 2nd [2.3.1] Added group information to the User value object.  September 27th [2.3.0] Breaking change in Taxa: Abbreviation property has been removed and is therefore no longer an accepted identifier.  ### Update 2.2.6  June 7th, 2018  Code maintenance, bug fixes. Geeq scores stable and made public.  June 7th [2.2.6] Added: User authentication endpoint.  May 2nd [2.2.5] Fixed: Cleaned up and optimized platforms/elements endpoint, removed redundant information (recursive properties nesting).  April 12th [2.2.3] Fixed: Array arguments not handling non-string properties properly, e.g. `ncbiIds` of genes.  April 9th [2.2.1] Fixed: Filter argument not working when the filtered field was a primitive type. This most significantly allows filtering by geeq boolean and double properties.  ### Update 2.2.0  February 8th, 2018  Breaking change in the 'Dataset differential analysis' endpoint: - No longer using `qValueThreshold` parameter. - Response format changed, now using `DifferentialExpressionAnalysisValueObject` instead of `DifferentialExpressionValueObject` - [Experimental] Added Geeq (Gene Expression Experiment Quality) scores to the dataset value objects   # noqa: E501
+    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  You can [consult the CHANGELOG.md file](https://gemma.msl.ubc.ca/resources/restapidocs/CHANGELOG.md) to view  release notes and recent changes to the Gemma RESTful API.   # noqa: E501
 
-    OpenAPI spec version: 2.5.1
+    OpenAPI spec version: 2.7.4
     Contact: pavlab-support@msl.ubc.ca
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -31,42 +31,42 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def get_api_info(self, **kwargs):  # noqa: E501
         """Retrieve an object with basic API information  # noqa: E501
 
+        The payload contains a list of featured external databases that Gemma uses under the `externalDatabases` field. Those are mainly genomic references and sources of gene annotations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_api_info(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :return: ResponseDataObjectApiInfoValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_api_info_with_http_info(**kwargs)  # noqa: E501
         else:
             (data) = self.get_api_info_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def get_api_info_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve an object with basic API information  # noqa: E501
 
+        The payload contains a list of featured external databases that Gemma uses under the `externalDatabases` field. Those are mainly genomic references and sources of gene annotations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_api_info_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :return: ResponseDataObjectApiInfoValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = []  # noqa: E501
         all_params.append('async_req')
@@ -120,19 +120,18 @@
             collection_formats=collection_formats)
 
     def get_dataset_annotations(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the annotations of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_annotations(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Dataset dataset: (required)
         :return: ResponseDataObjectSetAnnotationValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -142,19 +141,18 @@
             return data
 
     def get_dataset_annotations_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the annotations of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_annotations_with_http_info(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Dataset dataset: (required)
         :return: ResponseDataObjectSetAnnotationValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['dataset']  # noqa: E501
@@ -215,19 +213,18 @@
             collection_formats=collection_formats)
 
     def get_dataset_design(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the design of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_design(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Dataset1 dataset: (required)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -237,19 +234,18 @@
             return data
 
     def get_dataset_design_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the design of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_design_with_http_info(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Dataset1 dataset: (required)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['dataset']  # noqa: E501
@@ -310,19 +306,18 @@
             collection_formats=collection_formats)
 
     def get_dataset_differential_expression(self, datasets, **kwargs):  # noqa: E501
         """Retrieve the expression levels of a set of datasets subject to a threshold on their differential expressions  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_differential_expression(datasets, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] datasets: (required)
         :param int diff_ex_set:
         :param float threshold:
         :param int limit:
         :param bool keep_non_specific:
         :param str consolidate:
         :return: ResponseDataObjectListExperimentExpressionLevelsValueObject
@@ -337,19 +332,18 @@
             return data
 
     def get_dataset_differential_expression_with_http_info(self, datasets, **kwargs):  # noqa: E501
         """Retrieve the expression levels of a set of datasets subject to a threshold on their differential expressions  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_differential_expression_with_http_info(datasets, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] datasets: (required)
         :param int diff_ex_set:
         :param float threshold:
         :param int limit:
         :param bool keep_non_specific:
         :param str consolidate:
         :return: ResponseDataObjectListExperimentExpressionLevelsValueObject
@@ -426,19 +420,18 @@
             collection_formats=collection_formats)
 
     def get_dataset_differential_expression_analyses(self, dataset, **kwargs):  # noqa: E501
         """Retrieve annotations and surface level stats for a dataset's differential analyses  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_differential_expression_analyses(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Dataset2 dataset: (required)
         :param int offset:
         :param int limit:
         :return: ResponseDataObjectListDifferentialExpressionAnalysisValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -450,19 +443,18 @@
             return data
 
     def get_dataset_differential_expression_analyses_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve annotations and surface level stats for a dataset's differential analyses  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_differential_expression_analyses_with_http_info(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Dataset2 dataset: (required)
         :param int offset:
         :param int limit:
         :return: ResponseDataObjectListDifferentialExpressionAnalysisValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -529,19 +521,18 @@
             collection_formats=collection_formats)
 
     def get_dataset_differential_expression_analyses_result_sets(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the result sets of all differential analyses of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_differential_expression_analyses_result_sets(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Dataset3 dataset: (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -551,19 +542,18 @@
             return data
 
     def get_dataset_differential_expression_analyses_result_sets_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the result sets of all differential analyses of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_differential_expression_analyses_result_sets_with_http_info(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Dataset3 dataset: (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['dataset']  # noqa: E501
@@ -598,15 +588,15 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['*/*'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
             '/datasets/{dataset}/analyses/differential/resultSets', 'GET',
             path_params,
@@ -620,49 +610,49 @@
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_dataset_expression(self, dataset, **kwargs):  # noqa: E501
-        """Retrieve the expression data of a dataset  # noqa: E501
+        """Retrieve processed expression data of a dataset  # noqa: E501
 
+        This endpoint is deprecated and getDatasetProcessedExpression() should be used instead.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_expression(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Dataset4 dataset: (required)
         :param bool filter:
-        :return: str
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_dataset_expression_with_http_info(dataset, **kwargs)  # noqa: E501
         else:
             (data) = self.get_dataset_expression_with_http_info(dataset, **kwargs)  # noqa: E501
             return data
 
     def get_dataset_expression_with_http_info(self, dataset, **kwargs):  # noqa: E501
-        """Retrieve the expression data of a dataset  # noqa: E501
+        """Retrieve processed expression data of a dataset  # noqa: E501
 
+        This endpoint is deprecated and getDatasetProcessedExpression() should be used instead.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_expression_with_http_info(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Dataset4 dataset: (required)
         :param bool filter:
-        :return: str
+        :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['dataset', 'filter']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -710,32 +700,31 @@
             '/datasets/{dataset}/data', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='str',  # noqa: E501
+            response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_dataset_expression_for_genes(self, datasets, genes, **kwargs):  # noqa: E501
         """Retrieve the expression data matrix of a set of datasets and genes  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_expression_for_genes(datasets, genes, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] datasets: (required)
         :param list[object] genes: (required)
         :param bool keep_non_specific:
         :param str consolidate:
         :return: ResponseDataObjectListExperimentExpressionLevelsValueObject
                  If the method is called asynchronously,
                  returns the request thread.
@@ -748,19 +737,18 @@
             return data
 
     def get_dataset_expression_for_genes_with_http_info(self, datasets, genes, **kwargs):  # noqa: E501
         """Retrieve the expression data matrix of a set of datasets and genes  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_expression_for_genes_with_http_info(datasets, genes, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] datasets: (required)
         :param list[object] genes: (required)
         :param bool keep_non_specific:
         :param str consolidate:
         :return: ResponseDataObjectListExperimentExpressionLevelsValueObject
                  If the method is called asynchronously,
                  returns the request thread.
@@ -836,19 +824,18 @@
             collection_formats=collection_formats)
 
     def get_dataset_expression_pca(self, datasets, **kwargs):  # noqa: E501
         """Retrieve the principal components (PCA) of a set of datasets  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_expression_pca(datasets, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] datasets: (required)
         :param int component:
         :param int limit:
         :param bool keep_non_specific:
         :param str consolidate:
         :return: ResponseDataObjectListExperimentExpressionLevelsValueObject
                  If the method is called asynchronously,
@@ -862,19 +849,18 @@
             return data
 
     def get_dataset_expression_pca_with_http_info(self, datasets, **kwargs):  # noqa: E501
         """Retrieve the principal components (PCA) of a set of datasets  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_expression_pca_with_http_info(datasets, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] datasets: (required)
         :param int component:
         :param int limit:
         :param bool keep_non_specific:
         :param str consolidate:
         :return: ResponseDataObjectListExperimentExpressionLevelsValueObject
                  If the method is called asynchronously,
@@ -948,19 +934,18 @@
             collection_formats=collection_formats)
 
     def get_dataset_platforms(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the platforms of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_platforms(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Dataset5 dataset: (required)
         :return: ResponseDataObjectListArrayDesignValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -970,19 +955,18 @@
             return data
 
     def get_dataset_platforms_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the platforms of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_platforms_with_http_info(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Dataset5 dataset: (required)
         :return: ResponseDataObjectListArrayDesignValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['dataset']  # noqa: E501
@@ -1038,25 +1022,211 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_dataset_processed_expression(self, dataset, **kwargs):  # noqa: E501
+        """Retrieve processed expression data of a dataset  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_dataset_processed_expression(dataset, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param Dataset6 dataset: (required)
+        :return: str
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_dataset_processed_expression_with_http_info(dataset, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_dataset_processed_expression_with_http_info(dataset, **kwargs)  # noqa: E501
+            return data
+
+    def get_dataset_processed_expression_with_http_info(self, dataset, **kwargs):  # noqa: E501
+        """Retrieve processed expression data of a dataset  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_dataset_processed_expression_with_http_info(dataset, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param Dataset6 dataset: (required)
+        :return: str
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['dataset']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_dataset_processed_expression" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'dataset' is set
+        if ('dataset' not in params or
+                params['dataset'] is None):
+            raise ValueError("Missing the required parameter `dataset` when calling `get_dataset_processed_expression`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'dataset' in params:
+            path_params['dataset'] = params['dataset']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['text/tab-separated-values; charset=UTF-8', 'application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/datasets/{dataset}/data/processed', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='str',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_dataset_quantitation_types(self, dataset, **kwargs):  # noqa: E501
+        """Retrieve quantitation types of a dataset  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_dataset_quantitation_types(dataset, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param Dataset7 dataset: (required)
+        :return: ResponseDataObjectSetQuantitationTypeValueObject
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_dataset_quantitation_types_with_http_info(dataset, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_dataset_quantitation_types_with_http_info(dataset, **kwargs)  # noqa: E501
+            return data
+
+    def get_dataset_quantitation_types_with_http_info(self, dataset, **kwargs):  # noqa: E501
+        """Retrieve quantitation types of a dataset  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_dataset_quantitation_types_with_http_info(dataset, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param Dataset7 dataset: (required)
+        :return: ResponseDataObjectSetQuantitationTypeValueObject
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['dataset']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_dataset_quantitation_types" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'dataset' is set
+        if ('dataset' not in params or
+                params['dataset'] is None):
+            raise ValueError("Missing the required parameter `dataset` when calling `get_dataset_quantitation_types`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'dataset' in params:
+            path_params['dataset'] = params['dataset']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/datasets/{dataset}/quantitationTypes', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ResponseDataObjectSetQuantitationTypeValueObject',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_dataset_raw_expression(self, dataset, **kwargs):  # noqa: E501
         """Retrieve raw expression data of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_raw_expression(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param Dataset6 dataset: (required)
+        :param async_req bool
+        :param Dataset8 dataset: (required)
+        :param QuantitationType quantitation_type:
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_dataset_raw_expression_with_http_info(dataset, **kwargs)  # noqa: E501
@@ -1065,26 +1235,26 @@
             return data
 
     def get_dataset_raw_expression_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve raw expression data of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_raw_expression_with_http_info(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param Dataset6 dataset: (required)
+        :param async_req bool
+        :param Dataset8 dataset: (required)
+        :param QuantitationType quantitation_type:
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['dataset']  # noqa: E501
+        all_params = ['dataset', 'quantitation_type']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -1103,14 +1273,16 @@
         collection_formats = {}
 
         path_params = {}
         if 'dataset' in params:
             path_params['dataset'] = params['dataset']  # noqa: E501
 
         query_params = []
+        if 'quantitation_type' in params:
+            query_params.append(('quantitationType', params['quantitation_type']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -1138,20 +1310,19 @@
             collection_formats=collection_formats)
 
     def get_dataset_samples(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the samples of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_samples(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param Dataset7 dataset: (required)
+        :param async_req bool
+        :param Dataset9 dataset: (required)
         :return: ResponseDataObjectListBioAssayValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_dataset_samples_with_http_info(dataset, **kwargs)  # noqa: E501
@@ -1160,20 +1331,19 @@
             return data
 
     def get_dataset_samples_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the samples of a dataset  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_samples_with_http_info(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param Dataset7 dataset: (required)
+        :param async_req bool
+        :param Dataset9 dataset: (required)
         :return: ResponseDataObjectListBioAssayValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['dataset']  # noqa: E501
         all_params.append('async_req')
@@ -1233,20 +1403,19 @@
             collection_formats=collection_formats)
 
     def get_dataset_svd(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the singular value decomposition (SVD) of a dataset expression data  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_svd(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param Dataset8 dataset: (required)
+        :param async_req bool
+        :param Dataset10 dataset: (required)
         :return: ResponseDataObjectSimpleSVDValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_dataset_svd_with_http_info(dataset, **kwargs)  # noqa: E501
@@ -1255,20 +1424,19 @@
             return data
 
     def get_dataset_svd_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve the singular value decomposition (SVD) of a dataset expression data  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_dataset_svd_with_http_info(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param Dataset8 dataset: (required)
+        :param async_req bool
+        :param Dataset10 dataset: (required)
         :return: ResponseDataObjectSimpleSVDValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['dataset']  # noqa: E501
         all_params.append('async_req')
@@ -1328,24 +1496,24 @@
             collection_formats=collection_formats)
 
     def get_datasets(self, **kwargs):  # noqa: E501
         """Retrieve all datasets  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_datasets(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param str filter:
+        :param async_req bool
+        :param QueryArg query:
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgExpressionExperiment sort:
+        :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentWithSearchResultValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_datasets_with_http_info(**kwargs)  # noqa: E501
         else:
@@ -1353,29 +1521,29 @@
             return data
 
     def get_datasets_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve all datasets  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_datasets_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param str filter:
+        :param async_req bool
+        :param QueryArg query:
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgExpressionExperiment sort:
+        :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentWithSearchResultValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['filter', 'offset', 'limit', 'sort']  # noqa: E501
+        all_params = ['query', 'filter', 'offset', 'limit', 'sort']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -1388,14 +1556,16 @@
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'query' in params:
+            query_params.append(('query', params['query']))  # noqa: E501
         if 'filter' in params:
             query_params.append(('filter', params['filter']))  # noqa: E501
         if 'offset' in params:
             query_params.append(('offset', params['offset']))  # noqa: E501
         if 'limit' in params:
             query_params.append(('limit', params['limit']))  # noqa: E501
         if 'sort' in params:
@@ -1418,38 +1588,149 @@
             '/datasets', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
+            response_type='QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentWithSearchResultValueObject',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_datasets_annotations_usage_statistics(self, **kwargs):  # noqa: E501
+        """Retrieve usage statistics of annotations among datasets matching the provided query and filter  # noqa: E501
+
+        Usage statistics are aggregated across experiment tags, samples and factor values mentioned in the experimental design.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_datasets_annotations_usage_statistics(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param QueryArg query:
+        :param FilterArgExpressionExperiment filter:
+        :param list[str] exclude: List of fields to exclude from the payload. Only `parentTerms` can be excluded.
+        :param int limit: Maximum number of annotations to returned; capped at 5000.
+        :param int min_frequency: Minimum number of associated datasets to report an annotation. If used, the limit will default to 5000.
+        :param str category: A category URI to restrict reported annotations. If unspecified, annotations from all categories are reported. If empty, uncategorized terms are reported.
+        :return: LimitedResponseDataObjectAnnotationWithUsageStatisticsValueObject
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_datasets_annotations_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.get_datasets_annotations_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def get_datasets_annotations_usage_statistics_with_http_info(self, **kwargs):  # noqa: E501
+        """Retrieve usage statistics of annotations among datasets matching the provided query and filter  # noqa: E501
+
+        Usage statistics are aggregated across experiment tags, samples and factor values mentioned in the experimental design.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_datasets_annotations_usage_statistics_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param QueryArg query:
+        :param FilterArgExpressionExperiment filter:
+        :param list[str] exclude: List of fields to exclude from the payload. Only `parentTerms` can be excluded.
+        :param int limit: Maximum number of annotations to returned; capped at 5000.
+        :param int min_frequency: Minimum number of associated datasets to report an annotation. If used, the limit will default to 5000.
+        :param str category: A category URI to restrict reported annotations. If unspecified, annotations from all categories are reported. If empty, uncategorized terms are reported.
+        :return: LimitedResponseDataObjectAnnotationWithUsageStatisticsValueObject
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['query', 'filter', 'exclude', 'limit', 'min_frequency', 'category']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_datasets_annotations_usage_statistics" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'query' in params:
+            query_params.append(('query', params['query']))  # noqa: E501
+        if 'filter' in params:
+            query_params.append(('filter', params['filter']))  # noqa: E501
+        if 'exclude' in params:
+            query_params.append(('exclude', params['exclude']))  # noqa: E501
+            collection_formats['exclude'] = 'multi'  # noqa: E501
+        if 'limit' in params:
+            query_params.append(('limit', params['limit']))  # noqa: E501
+        if 'min_frequency' in params:
+            query_params.append(('minFrequency', params['min_frequency']))  # noqa: E501
+        if 'category' in params:
+            query_params.append(('category', params['category']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/datasets/annotations', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='LimitedResponseDataObjectAnnotationWithUsageStatisticsValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_datasets_by_ids(self, dataset, **kwargs):  # noqa: E501
         """Retrieve datasets by their identifiers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_datasets_by_ids(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] dataset: (required)
-        :param str filter:
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgExpressionExperiment sort:
+        :return: FilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_datasets_by_ids_with_http_info(dataset, **kwargs)  # noqa: E501
         else:
@@ -1457,25 +1738,24 @@
             return data
 
     def get_datasets_by_ids_with_http_info(self, dataset, **kwargs):  # noqa: E501
         """Retrieve datasets by their identifiers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_datasets_by_ids_with_http_info(dataset, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] dataset: (required)
-        :param str filter:
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgExpressionExperiment sort:
+        :return: FilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['dataset', 'filter', 'offset', 'limit', 'sort']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -1530,32 +1810,322 @@
             '/datasets/{dataset}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
+            response_type='FilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_datasets_categories_usage_statistics(self, **kwargs):  # noqa: E501
+        """Retrieve usage statistics of categories among datasets matching the provided query and filter  # noqa: E501
+
+        Usage statistics are aggregated across experiment tags, samples and factor values mentioned in the experimental design.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_datasets_categories_usage_statistics(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param QueryArg query:
+        :param FilterArgExpressionExperiment filter:
+        :param int limit:
+        :return: QueriedAndFilteredResponseDataObjectCategoryWithUsageStatisticsValueObject
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_datasets_categories_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.get_datasets_categories_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def get_datasets_categories_usage_statistics_with_http_info(self, **kwargs):  # noqa: E501
+        """Retrieve usage statistics of categories among datasets matching the provided query and filter  # noqa: E501
+
+        Usage statistics are aggregated across experiment tags, samples and factor values mentioned in the experimental design.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_datasets_categories_usage_statistics_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param QueryArg query:
+        :param FilterArgExpressionExperiment filter:
+        :param int limit:
+        :return: QueriedAndFilteredResponseDataObjectCategoryWithUsageStatisticsValueObject
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['query', 'filter', 'limit']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_datasets_categories_usage_statistics" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'query' in params:
+            query_params.append(('query', params['query']))  # noqa: E501
+        if 'filter' in params:
+            query_params.append(('filter', params['filter']))  # noqa: E501
+        if 'limit' in params:
+            query_params.append(('limit', params['limit']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/datasets/categories', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='QueriedAndFilteredResponseDataObjectCategoryWithUsageStatisticsValueObject',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_datasets_platforms_usage_statistics(self, **kwargs):  # noqa: E501
+        """Retrieve usage statistics of platforms among datasets matching the provided query and filter  # noqa: E501
+
+        Usage statistics are aggregated across experiment tags, samples and factor values mentioned in the experimental design.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_datasets_platforms_usage_statistics(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param QueryArg query:
+        :param FilterArgExpressionExperiment filter:
+        :param int limit:
+        :return: LimitedResponseDataObjectArrayDesignWithUsageStatisticsValueObject
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_datasets_platforms_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.get_datasets_platforms_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def get_datasets_platforms_usage_statistics_with_http_info(self, **kwargs):  # noqa: E501
+        """Retrieve usage statistics of platforms among datasets matching the provided query and filter  # noqa: E501
+
+        Usage statistics are aggregated across experiment tags, samples and factor values mentioned in the experimental design.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_datasets_platforms_usage_statistics_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param QueryArg query:
+        :param FilterArgExpressionExperiment filter:
+        :param int limit:
+        :return: LimitedResponseDataObjectArrayDesignWithUsageStatisticsValueObject
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['query', 'filter', 'limit']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_datasets_platforms_usage_statistics" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'query' in params:
+            query_params.append(('query', params['query']))  # noqa: E501
+        if 'filter' in params:
+            query_params.append(('filter', params['filter']))  # noqa: E501
+        if 'limit' in params:
+            query_params.append(('limit', params['limit']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/datasets/platforms', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='LimitedResponseDataObjectArrayDesignWithUsageStatisticsValueObject',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_datasets_taxa_usage_statistics(self, **kwargs):  # noqa: E501
+        """Retrieve taxa usage statistics for datasets matching the provided query and filter  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_datasets_taxa_usage_statistics(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param QueryArg query:
+        :param FilterArgExpressionExperiment filter:
+        :return: QueriedAndFilteredResponseDataObjectTaxonWithUsageStatisticsValueObject
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_datasets_taxa_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.get_datasets_taxa_usage_statistics_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def get_datasets_taxa_usage_statistics_with_http_info(self, **kwargs):  # noqa: E501
+        """Retrieve taxa usage statistics for datasets matching the provided query and filter  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_datasets_taxa_usage_statistics_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param QueryArg query:
+        :param FilterArgExpressionExperiment filter:
+        :return: QueriedAndFilteredResponseDataObjectTaxonWithUsageStatisticsValueObject
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['query', 'filter']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_datasets_taxa_usage_statistics" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'query' in params:
+            query_params.append(('query', params['query']))  # noqa: E501
+        if 'filter' in params:
+            query_params.append(('filter', params['filter']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/datasets/taxa', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='QueriedAndFilteredResponseDataObjectTaxonWithUsageStatisticsValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_gene_go_terms(self, gene, **kwargs):  # noqa: E501
         """Retrieve the GO terms associated to a gene  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_gene_go_terms(gene, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Gene gene: (required)
         :return: ResponseDataObjectListGeneOntologyTermValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -1565,19 +2135,18 @@
             return data
 
     def get_gene_go_terms_with_http_info(self, gene, **kwargs):  # noqa: E501
         """Retrieve the GO terms associated to a gene  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_gene_go_terms_with_http_info(gene, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Gene gene: (required)
         :return: ResponseDataObjectListGeneOntologyTermValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['gene']  # noqa: E501
@@ -1638,19 +2207,18 @@
             collection_formats=collection_formats)
 
     def get_gene_locations(self, gene, **kwargs):  # noqa: E501
         """Retrieve the physical locations of a given gene  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_gene_locations(gene, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Gene1 gene: (required)
         :return: ResponseDataObjectListPhysicalLocationValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -1660,19 +2228,18 @@
             return data
 
     def get_gene_locations_with_http_info(self, gene, **kwargs):  # noqa: E501
         """Retrieve the physical locations of a given gene  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_gene_locations_with_http_info(gene, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Gene1 gene: (required)
         :return: ResponseDataObjectListPhysicalLocationValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['gene']  # noqa: E501
@@ -1733,19 +2300,18 @@
             collection_formats=collection_formats)
 
     def get_gene_locations_in_taxon(self, taxon, gene, **kwargs):  # noqa: E501
         """Retrieve physical locations for a given gene and taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_gene_locations_in_taxon(taxon, gene, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Taxon3 taxon: (required)
         :param Gene3 gene: (required)
         :return: ResponseDataObjectListPhysicalLocationValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
@@ -1756,19 +2322,18 @@
             return data
 
     def get_gene_locations_in_taxon_with_http_info(self, taxon, gene, **kwargs):  # noqa: E501
         """Retrieve physical locations for a given gene and taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_gene_locations_in_taxon_with_http_info(taxon, gene, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Taxon3 taxon: (required)
         :param Gene3 gene: (required)
         :return: ResponseDataObjectListPhysicalLocationValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
@@ -1836,23 +2401,22 @@
             collection_formats=collection_formats)
 
     def get_gene_probes(self, gene, **kwargs):  # noqa: E501
         """Retrieve the probes associated to a genes across all platforms  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_gene_probes(gene, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Gene2 gene: (required)
         :param int offset:
         :param int limit:
-        :return: PaginatedResponseDataObjectCompositeSequenceValueObject
+        :return: FilteredAndPaginatedResponseDataObjectCompositeSequenceValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_gene_probes_with_http_info(gene, **kwargs)  # noqa: E501
         else:
@@ -1860,23 +2424,22 @@
             return data
 
     def get_gene_probes_with_http_info(self, gene, **kwargs):  # noqa: E501
         """Retrieve the probes associated to a genes across all platforms  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_gene_probes_with_http_info(gene, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Gene2 gene: (required)
         :param int offset:
         :param int limit:
-        :return: PaginatedResponseDataObjectCompositeSequenceValueObject
+        :return: FilteredAndPaginatedResponseDataObjectCompositeSequenceValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['gene', 'offset', 'limit']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -1926,32 +2489,31 @@
             '/genes/{gene}/probes', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectCompositeSequenceValueObject',  # noqa: E501
+            response_type='FilteredAndPaginatedResponseDataObjectCompositeSequenceValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_genes(self, genes, **kwargs):  # noqa: E501
         """Retrieve genes matching gene identifiers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_genes(genes, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] genes: (required)
         :return: ResponseDataObjectListGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -1961,19 +2523,18 @@
             return data
 
     def get_genes_with_http_info(self, genes, **kwargs):  # noqa: E501
         """Retrieve genes matching gene identifiers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_genes_with_http_info(genes, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] genes: (required)
         :return: ResponseDataObjectListGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['genes']  # noqa: E501
@@ -2030,24 +2591,294 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_number_of_datasets(self, **kwargs):  # noqa: E501
+        """Count datasets matching the provided query and filter  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_number_of_datasets(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param QueryArg query:
+        :param FilterArgExpressionExperiment filter:
+        :return: ResponseDataObjectLong
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_number_of_datasets_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.get_number_of_datasets_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def get_number_of_datasets_with_http_info(self, **kwargs):  # noqa: E501
+        """Count datasets matching the provided query and filter  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_number_of_datasets_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param QueryArg query:
+        :param FilterArgExpressionExperiment filter:
+        :return: ResponseDataObjectLong
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['query', 'filter']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_number_of_datasets" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'query' in params:
+            query_params.append(('query', params['query']))  # noqa: E501
+        if 'filter' in params:
+            query_params.append(('filter', params['filter']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/datasets/count', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ResponseDataObjectLong',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_number_of_platforms(self, **kwargs):  # noqa: E501
+        """Count platforms matching the provided filter  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_number_of_platforms(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param FilterArgArrayDesign filter:
+        :return: ResponseDataObjectLong
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_number_of_platforms_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.get_number_of_platforms_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def get_number_of_platforms_with_http_info(self, **kwargs):  # noqa: E501
+        """Count platforms matching the provided filter  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_number_of_platforms_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param FilterArgArrayDesign filter:
+        :return: ResponseDataObjectLong
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['filter']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_number_of_platforms" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'filter' in params:
+            query_params.append(('filter', params['filter']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/platforms/count', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ResponseDataObjectLong',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_number_of_result_sets(self, **kwargs):  # noqa: E501
+        """Count result sets matching the provided filter  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_number_of_result_sets(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param FilterArgExpressionAnalysisResultSet filter:
+        :return: ResponseDataObjectLong
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.get_number_of_result_sets_with_http_info(**kwargs)  # noqa: E501
+        else:
+            (data) = self.get_number_of_result_sets_with_http_info(**kwargs)  # noqa: E501
+            return data
+
+    def get_number_of_result_sets_with_http_info(self, **kwargs):  # noqa: E501
+        """Count result sets matching the provided filter  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.get_number_of_result_sets_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param FilterArgExpressionAnalysisResultSet filter:
+        :return: ResponseDataObjectLong
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['filter']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_number_of_result_sets" % key
+                )
+            params[key] = val
+        del params['kwargs']
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+        if 'filter' in params:
+            query_params.append(('filter', params['filter']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/resultSets/count', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='ResponseDataObjectLong',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_platform_annotations(self, platform, **kwargs):  # noqa: E501
         """Retrieve the annotations of a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platform_annotations(platform, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Platform platform: (required)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -2057,19 +2888,18 @@
             return data
 
     def get_platform_annotations_with_http_info(self, platform, **kwargs):  # noqa: E501
         """Retrieve the annotations of a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platform_annotations_with_http_info(platform, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Platform platform: (required)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['platform']  # noqa: E501
@@ -2130,19 +2960,18 @@
             collection_formats=collection_formats)
 
     def get_platform_datasets(self, platform, **kwargs):  # noqa: E501
         """Retrieve all experiments using a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platform_datasets(platform, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Platform1 platform: (required)
         :param int offset:
         :param int limit:
         :return: PaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -2154,19 +2983,18 @@
             return data
 
     def get_platform_datasets_with_http_info(self, platform, **kwargs):  # noqa: E501
         """Retrieve all experiments using a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platform_datasets_with_http_info(platform, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Platform1 platform: (required)
         :param int offset:
         :param int limit:
         :return: PaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -2229,53 +3057,51 @@
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_platform_element(self, platform, probes, **kwargs):  # noqa: E501
-        """Retrieve the selected composite sequences for a given platform  # noqa: E501
+        """Retrieve the selected probes for a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platform_element(platform, probes, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Platform2 platform: (required)
         :param list[object] probes: (required)
         :param int offset:
         :param int limit:
-        :return: PaginatedResponseDataObjectCompositeSequenceValueObject
+        :return: FilteredAndPaginatedResponseDataObjectCompositeSequenceValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_platform_element_with_http_info(platform, probes, **kwargs)  # noqa: E501
         else:
             (data) = self.get_platform_element_with_http_info(platform, probes, **kwargs)  # noqa: E501
             return data
 
     def get_platform_element_with_http_info(self, platform, probes, **kwargs):  # noqa: E501
-        """Retrieve the selected composite sequences for a given platform  # noqa: E501
+        """Retrieve the selected probes for a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platform_element_with_http_info(platform, probes, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Platform2 platform: (required)
         :param list[object] probes: (required)
         :param int offset:
         :param int limit:
-        :return: PaginatedResponseDataObjectCompositeSequenceValueObject
+        :return: FilteredAndPaginatedResponseDataObjectCompositeSequenceValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['platform', 'probes', 'offset', 'limit']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -2332,37 +3158,36 @@
             '/platforms/{platform}/elements/{probes}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectCompositeSequenceValueObject',  # noqa: E501
+            response_type='FilteredAndPaginatedResponseDataObjectCompositeSequenceValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_platform_element_genes(self, platform, probe, **kwargs):  # noqa: E501
         """Retrieve the genes associated to a probe in a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platform_element_genes(platform, probe, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Platform3 platform: (required)
         :param Probe probe: (required)
         :param int offset:
         :param int limit:
-        :return: PaginatedResponseDataObjectGeneValueObject
+        :return: FilteredAndPaginatedResponseDataObjectGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_platform_element_genes_with_http_info(platform, probe, **kwargs)  # noqa: E501
         else:
@@ -2370,24 +3195,23 @@
             return data
 
     def get_platform_element_genes_with_http_info(self, platform, probe, **kwargs):  # noqa: E501
         """Retrieve the genes associated to a probe in a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platform_element_genes_with_http_info(platform, probe, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Platform3 platform: (required)
         :param Probe probe: (required)
         :param int offset:
         :param int limit:
-        :return: PaginatedResponseDataObjectGeneValueObject
+        :return: FilteredAndPaginatedResponseDataObjectGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['platform', 'probe', 'offset', 'limit']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -2443,32 +3267,31 @@
             '/platforms/{platform}/elements/{probe}/genes', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectGeneValueObject',  # noqa: E501
+            response_type='FilteredAndPaginatedResponseDataObjectGeneValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_platform_elements(self, platform, **kwargs):  # noqa: E501
-        """Retrieve the composite sequences for a given platform  # noqa: E501
+        """Retrieve the probes for a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platform_elements(platform, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Platform4 platform: (required)
         :param int offset:
         :param int limit:
         :return: PaginatedResponseDataObjectCompositeSequenceValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -2476,23 +3299,22 @@
         if kwargs.get('async_req'):
             return self.get_platform_elements_with_http_info(platform, **kwargs)  # noqa: E501
         else:
             (data) = self.get_platform_elements_with_http_info(platform, **kwargs)  # noqa: E501
             return data
 
     def get_platform_elements_with_http_info(self, platform, **kwargs):  # noqa: E501
-        """Retrieve the composite sequences for a given platform  # noqa: E501
+        """Retrieve the probes for a given platform  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platform_elements_with_http_info(platform, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Platform4 platform: (required)
         :param int offset:
         :param int limit:
         :return: PaginatedResponseDataObjectCompositeSequenceValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -2559,24 +3381,23 @@
             collection_formats=collection_formats)
 
     def get_platforms(self, **kwargs):  # noqa: E501
         """Retrieve all platforms  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platforms(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param str filter:
+        :param async_req bool
+        :param FilterArgArrayDesign filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectArrayDesignValueObject
+        :param SortArgArrayDesign sort:
+        :return: FilteredAndPaginatedResponseDataObjectArrayDesignValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_platforms_with_http_info(**kwargs)  # noqa: E501
         else:
@@ -2584,24 +3405,23 @@
             return data
 
     def get_platforms_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve all platforms  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platforms_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param str filter:
+        :param async_req bool
+        :param FilterArgArrayDesign filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectArrayDesignValueObject
+        :param SortArgArrayDesign sort:
+        :return: FilteredAndPaginatedResponseDataObjectArrayDesignValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['filter', 'offset', 'limit', 'sort']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -2649,38 +3469,37 @@
             '/platforms', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectArrayDesignValueObject',  # noqa: E501
+            response_type='FilteredAndPaginatedResponseDataObjectArrayDesignValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_platforms_by_ids(self, platform, **kwargs):  # noqa: E501
         """Retrieve all platforms matching a set of platform identifiers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platforms_by_ids(platform, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] platform: (required)
-        :param str filter:
+        :param FilterArgArrayDesign filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectArrayDesignValueObject
+        :param SortArgArrayDesign sort:
+        :return: FilteredAndPaginatedResponseDataObjectArrayDesignValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_platforms_by_ids_with_http_info(platform, **kwargs)  # noqa: E501
         else:
@@ -2688,25 +3507,24 @@
             return data
 
     def get_platforms_by_ids_with_http_info(self, platform, **kwargs):  # noqa: E501
         """Retrieve all platforms matching a set of platform identifiers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_platforms_by_ids_with_http_info(platform, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] platform: (required)
-        :param str filter:
+        :param FilterArgArrayDesign filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectArrayDesignValueObject
+        :param SortArgArrayDesign sort:
+        :return: FilteredAndPaginatedResponseDataObjectArrayDesignValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['platform', 'filter', 'offset', 'limit', 'sort']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -2761,32 +3579,31 @@
             '/platforms/{platform}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectArrayDesignValueObject',  # noqa: E501
+            response_type='FilteredAndPaginatedResponseDataObjectArrayDesignValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_result_set(self, result_set, **kwargs):  # noqa: E501
         """Retrieve a single analysis result set by its identifier  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_result_set(result_set, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param int result_set: (required)
         :return: ResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -2796,19 +3613,18 @@
             return data
 
     def get_result_set_with_http_info(self, result_set, **kwargs):  # noqa: E501
         """Retrieve a single analysis result set by its identifier  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_result_set_with_http_info(result_set, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param int result_set: (required)
         :return: ResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['result_set']  # noqa: E501
@@ -2869,19 +3685,18 @@
             collection_formats=collection_formats)
 
     def get_result_set_as_tsv(self, result_set_, **kwargs):  # noqa: E501
         """Retrieve a single analysis result set by its identifier as a tab-separated values  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_result_set_as_tsv(result_set_, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param int result_set_: (required)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -2891,19 +3706,18 @@
             return data
 
     def get_result_set_as_tsv_with_http_info(self, result_set_, **kwargs):  # noqa: E501
         """Retrieve a single analysis result set by its identifier as a tab-separated values  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_result_set_as_tsv_with_http_info(result_set_, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param int result_set_: (required)
         :return: str
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['result_set_']  # noqa: E501
@@ -2938,15 +3752,15 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/tab-separated-values; charset=UTF-8'])  # noqa: E501
+            ['text/tab-separated-values; charset=UTF-8', 'application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['basicAuth', 'cookieAuth']  # noqa: E501
 
         return self.api_client.call_api(
             '/resultSets/{resultSet_}', 'GET',
             path_params,
@@ -2964,26 +3778,25 @@
             collection_formats=collection_formats)
 
     def get_result_sets(self, **kwargs):  # noqa: E501
         """Retrieve all result sets matching the provided criteria  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_result_sets(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] datasets:
         :param list[object] database_entries:
-        :param str filter:
+        :param FilterArgExpressionAnalysisResultSet filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject
+        :param SortArgExpressionAnalysisResultSet sort:
+        :return: FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_result_sets_with_http_info(**kwargs)  # noqa: E501
         else:
@@ -2991,26 +3804,25 @@
             return data
 
     def get_result_sets_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve all result sets matching the provided criteria  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_result_sets_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] datasets:
         :param list[object] database_entries:
-        :param str filter:
+        :param FilterArgExpressionAnalysisResultSet filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject
+        :param SortArgExpressionAnalysisResultSet sort:
+        :return: FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['datasets', 'database_entries', 'filter', 'offset', 'limit', 'sort']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -3064,32 +3876,31 @@
             '/resultSets', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject',  # noqa: E501
+            response_type='FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_taxa(self, **kwargs):  # noqa: E501
         """Retrieve all available taxa  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_taxa(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :return: ResponseDataObjectListTaxonValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_taxa_with_http_info(**kwargs)  # noqa: E501
@@ -3098,19 +3909,18 @@
             return data
 
     def get_taxa_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve all available taxa  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_taxa_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :return: ResponseDataObjectListTaxonValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = []  # noqa: E501
         all_params.append('async_req')
@@ -3164,19 +3974,18 @@
             collection_formats=collection_formats)
 
     def get_taxa_by_ids(self, taxa, **kwargs):  # noqa: E501
         """Retrieve taxa by their identifiers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_taxa_by_ids(taxa, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] taxa: (required)
         :return: ResponseDataObjectListTaxonValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
@@ -3186,19 +3995,18 @@
             return data
 
     def get_taxa_by_ids_with_http_info(self, taxa, **kwargs):  # noqa: E501
         """Retrieve taxa by their identifiers  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_taxa_by_ids_with_http_info(taxa, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param list[object] taxa: (required)
         :return: ResponseDataObjectListTaxonValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['taxa']  # noqa: E501
@@ -3260,25 +4068,24 @@
             collection_formats=collection_formats)
 
     def get_taxon_datasets(self, taxon, **kwargs):  # noqa: E501
         """Retrieve the datasets for a given taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_taxon_datasets(taxon, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Taxon4 taxon: (required)
-        :param str filter:
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgTaxon sort:
+        :return: FilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_taxon_datasets_with_http_info(taxon, **kwargs)  # noqa: E501
         else:
@@ -3286,25 +4093,24 @@
             return data
 
     def get_taxon_datasets_with_http_info(self, taxon, **kwargs):  # noqa: E501
         """Retrieve the datasets for a given taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_taxon_datasets_with_http_info(taxon, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Taxon4 taxon: (required)
-        :param str filter:
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgTaxon sort:
+        :return: FilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['taxon', 'filter', 'offset', 'limit', 'sort']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -3358,32 +4164,31 @@
             '/taxa/{taxon}/datasets', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
+            response_type='FilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_taxon_genes(self, taxon, gene, **kwargs):  # noqa: E501
         """Retrieve all genes in a given taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_taxon_genes(taxon, gene, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Taxon5 taxon: (required)
         :param Gene4 gene: (required)
         :return: ResponseDataObjectListGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
@@ -3394,19 +4199,18 @@
             return data
 
     def get_taxon_genes_with_http_info(self, taxon, gene, **kwargs):  # noqa: E501
         """Retrieve all genes in a given taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.get_taxon_genes_with_http_info(taxon, gene, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Taxon5 taxon: (required)
         :param Gene4 gene: (required)
         :return: ResponseDataObjectListGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
@@ -3469,61 +4273,59 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def get_taxon_genes_overlapping_chromosome(self, taxon, chromosome, **kwargs):  # noqa: E501
+    def get_taxon_genes_overlapping_chromosome(self, taxon, chromosome, start, size, **kwargs):  # noqa: E501
         """Retrieve genes overlapping a given region in a taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_taxon_genes_overlapping_chromosome(taxon, chromosome, async_req=True)
+        >>> thread = api.get_taxon_genes_overlapping_chromosome(taxon, chromosome, start, size, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Taxon6 taxon: (required)
         :param str chromosome: (required)
+        :param int start: (required)
+        :param int size: (required)
         :param str strand:
-        :param int start:
-        :param int size:
         :return: ResponseDataObjectListGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.get_taxon_genes_overlapping_chromosome_with_http_info(taxon, chromosome, **kwargs)  # noqa: E501
+            return self.get_taxon_genes_overlapping_chromosome_with_http_info(taxon, chromosome, start, size, **kwargs)  # noqa: E501
         else:
-            (data) = self.get_taxon_genes_overlapping_chromosome_with_http_info(taxon, chromosome, **kwargs)  # noqa: E501
+            (data) = self.get_taxon_genes_overlapping_chromosome_with_http_info(taxon, chromosome, start, size, **kwargs)  # noqa: E501
             return data
 
-    def get_taxon_genes_overlapping_chromosome_with_http_info(self, taxon, chromosome, **kwargs):  # noqa: E501
+    def get_taxon_genes_overlapping_chromosome_with_http_info(self, taxon, chromosome, start, size, **kwargs):  # noqa: E501
         """Retrieve genes overlapping a given region in a taxon  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_taxon_genes_overlapping_chromosome_with_http_info(taxon, chromosome, async_req=True)
+        >>> thread = api.get_taxon_genes_overlapping_chromosome_with_http_info(taxon, chromosome, start, size, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Taxon6 taxon: (required)
         :param str chromosome: (required)
+        :param int start: (required)
+        :param int size: (required)
         :param str strand:
-        :param int start:
-        :param int size:
         :return: ResponseDataObjectListGeneValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['taxon', 'chromosome', 'strand', 'start', 'size']  # noqa: E501
+        all_params = ['taxon', 'chromosome', 'start', 'size', 'strand']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -3538,14 +4340,22 @@
         if ('taxon' not in params or
                 params['taxon'] is None):
             raise ValueError("Missing the required parameter `taxon` when calling `get_taxon_genes_overlapping_chromosome`")  # noqa: E501
         # verify the required parameter 'chromosome' is set
         if ('chromosome' not in params or
                 params['chromosome'] is None):
             raise ValueError("Missing the required parameter `chromosome` when calling `get_taxon_genes_overlapping_chromosome`")  # noqa: E501
+        # verify the required parameter 'start' is set
+        if ('start' not in params or
+                params['start'] is None):
+            raise ValueError("Missing the required parameter `start` when calling `get_taxon_genes_overlapping_chromosome`")  # noqa: E501
+        # verify the required parameter 'size' is set
+        if ('size' not in params or
+                params['size'] is None):
+            raise ValueError("Missing the required parameter `size` when calling `get_taxon_genes_overlapping_chromosome`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         if 'taxon' in params:
             path_params['taxon'] = params['taxon']  # noqa: E501
         if 'chromosome' in params:
@@ -3585,60 +4395,60 @@
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def search(self, **kwargs):  # noqa: E501
-        """Search everything in Gemma.  # noqa: E501
+        """Search everything in Gemma  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param str query:
+        :param async_req bool
+        :param QueryArg query:
         :param Taxon2 taxon:
         :param Platform5 platform:
         :param list[str] result_types:
-        :param int limit:
+        :param int limit: Maximum number of search results to return; capped at 2000 unless `resultObject` is excluded.
+        :param list[str] exclude: List of fields to exclude from the payload. Only `resultObject` is supported.
         :return: SearchResultsResponseDataObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.search_with_http_info(**kwargs)  # noqa: E501
         else:
             (data) = self.search_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def search_with_http_info(self, **kwargs):  # noqa: E501
-        """Search everything in Gemma.  # noqa: E501
+        """Search everything in Gemma  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param str query:
+        :param async_req bool
+        :param QueryArg query:
         :param Taxon2 taxon:
         :param Platform5 platform:
         :param list[str] result_types:
-        :param int limit:
+        :param int limit: Maximum number of search results to return; capped at 2000 unless `resultObject` is excluded.
+        :param list[str] exclude: List of fields to exclude from the payload. Only `resultObject` is supported.
         :return: SearchResultsResponseDataObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['query', 'taxon', 'platform', 'result_types', 'limit']  # noqa: E501
+        all_params = ['query', 'taxon', 'platform', 'result_types', 'limit', 'exclude']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -3662,14 +4472,17 @@
         if 'platform' in params:
             query_params.append(('platform', params['platform']))  # noqa: E501
         if 'result_types' in params:
             query_params.append(('resultTypes', params['result_types']))  # noqa: E501
             collection_formats['resultTypes'] = 'multi'  # noqa: E501
         if 'limit' in params:
             query_params.append(('limit', params['limit']))  # noqa: E501
+        if 'exclude' in params:
+            query_params.append(('exclude', params['exclude']))  # noqa: E501
+            collection_formats['exclude'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -3697,20 +4510,19 @@
             collection_formats=collection_formats)
 
     def search_annotations(self, **kwargs):  # noqa: E501
         """Search for annotation tags  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_annotations(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param list[str] query:
+        :param async_req bool
+        :param list[str] query: A comma-delimited list of keywords to find annotations.
         :return: ResponseDataObjectListAnnotationSearchResultValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.search_annotations_with_http_info(**kwargs)  # noqa: E501
@@ -3719,20 +4531,19 @@
             return data
 
     def search_annotations_with_http_info(self, **kwargs):  # noqa: E501
         """Search for annotation tags  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_annotations_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param list[str] query:
+        :param async_req bool
+        :param list[str] query: A comma-delimited list of keywords to find annotations.
         :return: ResponseDataObjectListAnnotationSearchResultValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['query']  # noqa: E501
         all_params.append('async_req')
@@ -3785,46 +4596,46 @@
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def search_annotations_by_path_query(self, query, **kwargs):  # noqa: E501
-        """Search for annotation tags.  # noqa: E501
+        """Search for annotation tags  # noqa: E501
 
+        This is deprecated in favour of passing `query` as a query parameter.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_annotations_by_path_query(query, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param list[str] query: (required)
+        :param async_req bool
+        :param list[str] query: A comma-delimited list of keywords to find annotations. (required)
         :return: ResponseDataObjectListAnnotationSearchResultValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.search_annotations_by_path_query_with_http_info(query, **kwargs)  # noqa: E501
         else:
             (data) = self.search_annotations_by_path_query_with_http_info(query, **kwargs)  # noqa: E501
             return data
 
     def search_annotations_by_path_query_with_http_info(self, query, **kwargs):  # noqa: E501
-        """Search for annotation tags.  # noqa: E501
+        """Search for annotation tags  # noqa: E501
 
+        This is deprecated in favour of passing `query` as a query parameter.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_annotations_by_path_query_with_http_info(query, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param list[str] query: (required)
+        :param async_req bool
+        :param list[str] query: A comma-delimited list of keywords to find annotations. (required)
         :return: ResponseDataObjectListAnnotationSearchResultValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['query']  # noqa: E501
         all_params.append('async_req')
@@ -3883,53 +4694,53 @@
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def search_datasets(self, **kwargs):  # noqa: E501
         """Retrieve datasets associated to an annotation tags search  # noqa: E501
 
+        This is deprecated in favour of the [/datasets](#/default/getDatasets) endpoint. Use the `AND` operator to intersect the results of multiple queries.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_datasets(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param list[str] query:
-        :param str filter:
+        :param async_req bool
+        :param list[str] query: A comma-delimited list of keywords to find annotations. Matching datasets for each query are intersected.
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgExpressionExperiment sort:
+        :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.search_datasets_with_http_info(**kwargs)  # noqa: E501
         else:
             (data) = self.search_datasets_with_http_info(**kwargs)  # noqa: E501
             return data
 
     def search_datasets_with_http_info(self, **kwargs):  # noqa: E501
         """Retrieve datasets associated to an annotation tags search  # noqa: E501
 
+        This is deprecated in favour of the [/datasets](#/default/getDatasets) endpoint. Use the `AND` operator to intersect the results of multiple queries.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_datasets_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param list[str] query:
-        :param str filter:
+        :param async_req bool
+        :param list[str] query: A comma-delimited list of keywords to find annotations. Matching datasets for each query are intersected.
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgExpressionExperiment sort:
+        :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['query', 'filter', 'offset', 'limit', 'sort']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -3980,64 +4791,64 @@
             '/annotations/search/datasets', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
+            response_type='QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def search_datasets_by_query_in_path(self, query, **kwargs):  # noqa: E501
         """Retrieve datasets associated to an annotation tags search  # noqa: E501
 
+        This is deprecated in favour of passing `query` as a query parameter.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_datasets_by_query_in_path(query, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param list[str] query: (required)
-        :param str filter:
+        :param async_req bool
+        :param list[str] query: A comma-delimited list of keywords to find annotations. Matching datasets for each query are intersected. (required)
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgExpressionExperiment sort:
+        :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.search_datasets_by_query_in_path_with_http_info(query, **kwargs)  # noqa: E501
         else:
             (data) = self.search_datasets_by_query_in_path_with_http_info(query, **kwargs)  # noqa: E501
             return data
 
     def search_datasets_by_query_in_path_with_http_info(self, query, **kwargs):  # noqa: E501
         """Retrieve datasets associated to an annotation tags search  # noqa: E501
 
+        This is deprecated in favour of passing `query` as a query parameter.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_datasets_by_query_in_path_with_http_info(query, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
-        :param list[str] query: (required)
-        :param str filter:
+        :param async_req bool
+        :param list[str] query: A comma-delimited list of keywords to find annotations. Matching datasets for each query are intersected. (required)
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgExpressionExperiment sort:
+        :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['query', 'filter', 'offset', 'limit', 'sort']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -4092,66 +4903,66 @@
             '/annotations/search/{query}/datasets', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
+            response_type='QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def search_taxon_datasets(self, taxon, **kwargs):  # noqa: E501
         """Retrieve datasets within a given taxa associated to an annotation tags search  # noqa: E501
 
+        This is deprecated in favour of the [/datasets](#/default/getDatasets) endpoint with a `query` parameter and a `filter` parameter with `taxon.id = {taxon} or taxon.commonName = {taxon} or taxon.scientificName = {taxon}` to restrict the taxon instead.  Use the `AND` operator to intersect the results of multiple queries.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_taxon_datasets(taxon, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Taxon taxon: (required)
-        :param list[str] query:
-        :param str filter:
+        :param list[str] query: A comma-delimited list of keywords to find annotations. Matching datasets for each query are intersected.
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgExpressionExperiment sort:
+        :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.search_taxon_datasets_with_http_info(taxon, **kwargs)  # noqa: E501
         else:
             (data) = self.search_taxon_datasets_with_http_info(taxon, **kwargs)  # noqa: E501
             return data
 
     def search_taxon_datasets_with_http_info(self, taxon, **kwargs):  # noqa: E501
         """Retrieve datasets within a given taxa associated to an annotation tags search  # noqa: E501
 
+        This is deprecated in favour of the [/datasets](#/default/getDatasets) endpoint with a `query` parameter and a `filter` parameter with `taxon.id = {taxon} or taxon.commonName = {taxon} or taxon.scientificName = {taxon}` to restrict the taxon instead.  Use the `AND` operator to intersect the results of multiple queries.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_taxon_datasets_with_http_info(taxon, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Taxon taxon: (required)
-        :param list[str] query:
-        :param str filter:
+        :param list[str] query: A comma-delimited list of keywords to find annotations. Matching datasets for each query are intersected.
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgExpressionExperiment sort:
+        :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['taxon', 'query', 'filter', 'offset', 'limit', 'sort']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -4208,66 +5019,66 @@
             '/annotations/{taxon}/search/datasets', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
+            response_type='QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def search_taxon_datasets_by_query_in_path(self, taxon, query, **kwargs):  # noqa: E501
         """Retrieve datasets within a given taxa associated to an annotation tags search  # noqa: E501
 
+        This is deprecated in favour of passing `query` as a query parameter.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_taxon_datasets_by_query_in_path(taxon, query, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Taxon1 taxon: (required)
-        :param list[str] query: (required)
-        :param str filter:
+        :param list[str] query: A comma-delimited list of keywords to find annotations. Matching datasets for each query are intersected. (required)
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgExpressionExperiment sort:
+        :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.search_taxon_datasets_by_query_in_path_with_http_info(taxon, query, **kwargs)  # noqa: E501
         else:
             (data) = self.search_taxon_datasets_by_query_in_path_with_http_info(taxon, query, **kwargs)  # noqa: E501
             return data
 
     def search_taxon_datasets_by_query_in_path_with_http_info(self, taxon, query, **kwargs):  # noqa: E501
         """Retrieve datasets within a given taxa associated to an annotation tags search  # noqa: E501
 
+        This is deprecated in favour of passing `query` as a query parameter.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-
         >>> thread = api.search_taxon_datasets_by_query_in_path_with_http_info(taxon, query, async_req=True)
         >>> result = thread.get()
 
-        :param bool async_req:
+        :param async_req bool
         :param Taxon1 taxon: (required)
-        :param list[str] query: (required)
-        :param str filter:
+        :param list[str] query: A comma-delimited list of keywords to find annotations. Matching datasets for each query are intersected. (required)
+        :param FilterArgExpressionExperiment filter:
         :param int offset:
         :param int limit:
-        :param str sort:
-        :return: PaginatedResponseDataObjectExpressionExperimentValueObject
+        :param SortArgExpressionExperiment sort:
+        :return: QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['taxon', 'query', 'filter', 'offset', 'limit', 'sort']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -4328,14 +5139,14 @@
             '/annotations/{taxon}/search/{query}/datasets', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='PaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
+            response_type='QueriedAndFilteredAndPaginatedResponseDataObjectExpressionExperimentValueObject',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `gemmapy-0.0.2/gemmapy/sdk/api_client.py` & `gemmapy-1.0.0/gemmapy/sdk/api_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # coding: utf-8
 """
     Gemma RESTful API
 
-    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  Fix return type for `getResultSets` which was incorrectly referring to a renamed VO.  Remove the `security` requirements by default from the specification, which forced the Python package to supply empty credentials. There is currently no privileged endpoints, although some can return additional results.  ## Updates  ### Update 2.5.1  Restore `objectClass` visibility in `AnnotationValueObject`.  Fix incorrect response types for annotations search endpoints returning datasets.  ### Update 2.5.0  Major cleanups were performed in this release in order to stabilize the specification. Numerous properties from Gemma Web that were never intended to be exposed in Gemma REST have been hidden. It's a bit too much to describe in here, but you can navigate to the schemas section below to get a good glance at the models.  Favour `numberOfSomething` instead of `somethingCount` which is clearer. The older names are kept for backward-compatibility, but should be considered deprecated.  Gene aliases and multifunctionality rank are now filled in `GeneValueObject`.  Uniformly use `TaxonValueObject` to represent taxon. This is breaking change for the `ExpressionExperimentValueObject` and `ArrayDesignValueObject` as their `taxon` property will be an `object` instead of a `string`. Properties such as `taxonId` are now deprecated and `taxon.id` should be used instead.  Entities that have IDs now all inherit from `IdentifiableValueObject`. This implies that you can assume the presence of an `id` in a search result `resultObject` attribute for example.  New `/search` endpoint! for an unified search experience. Annotation-based search endpoints under `/annotations` are now deprecated.  New API docs! While not as nice looking, the previous theme will be gradually ported to Swagger UI as we focused on functionality over prettiness for this release.  ### Update 2.4.0 through 2.4.1  Release notes for the 2.4 series were not written down, so I'll try to do my best to recall features that were introduced at that time.  An [OpenAPI](https://www.openapis.org/) specification was introduced and available under `/rest/v2/openapi.json`, although not fully stabilized.  Add a `/resultSets` endpoint to navigate result sets directly, by ID or by dataset.  Add a `/resultSets/{resultSetId}` endpoint to retrieve a specific result set by its ID. This endpoint can be negotiated with an `Accept: text/tab-separated-values` header to obtain a TSV representation.  Add a `/datasets/{dataset}/analyses/differential/resultSets` endpoint that essentially redirect to a specific `/resultSet` endpoint by dataset ID.  Add an endpoint to retrieve preferred raw expression vectors.  ### Update 2.3.4  November 6th, 2018  November 6th [2.3.4] Bug fixes in the dataset search endpoint.  November 5th [2.3.3] Added filtering parameters to dataset search.  October 25th [2.3.2] Changed behavior of the dataset search endpoint to more closely match the Gemma web interface.  October 2nd [2.3.1] Added group information to the User value object.  September 27th [2.3.0] Breaking change in Taxa: Abbreviation property has been removed and is therefore no longer an accepted identifier.  ### Update 2.2.6  June 7th, 2018  Code maintenance, bug fixes. Geeq scores stable and made public.  June 7th [2.2.6] Added: User authentication endpoint.  May 2nd [2.2.5] Fixed: Cleaned up and optimized platforms/elements endpoint, removed redundant information (recursive properties nesting).  April 12th [2.2.3] Fixed: Array arguments not handling non-string properties properly, e.g. `ncbiIds` of genes.  April 9th [2.2.1] Fixed: Filter argument not working when the filtered field was a primitive type. This most significantly allows filtering by geeq boolean and double properties.  ### Update 2.2.0  February 8th, 2018  Breaking change in the 'Dataset differential analysis' endpoint: - No longer using `qValueThreshold` parameter. - Response format changed, now using `DifferentialExpressionAnalysisValueObject` instead of `DifferentialExpressionValueObject` - [Experimental] Added Geeq (Gene Expression Experiment Quality) scores to the dataset value objects   # noqa: E501
+    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  You can [consult the CHANGELOG.md file](https://gemma.msl.ubc.ca/resources/restapidocs/CHANGELOG.md) to view  release notes and recent changes to the Gemma RESTful API.   # noqa: E501
 
-    OpenAPI spec version: 2.5.1
+    OpenAPI spec version: 2.7.4
     Contact: pavlab-support@msl.ubc.ca
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import datetime
 import json
 import mimetypes
 from multiprocessing.pool import ThreadPool
 import os
 import re
 import tempfile
+import numpy as np
 
 # python 2 and python 3 compatibility library
 import six
 from six.moves.urllib.parse import quote
 
 from gemmapy.sdk.configuration import Configuration
 import gemmapy.sdk.models
@@ -68,15 +69,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.0.0/python'
+        self.user_agent = 'gemmapy/0.0.2'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
@@ -181,14 +182,16 @@
         :param obj: The data to serialize.
         :return: The serialized form of data.
         """
         if obj is None:
             return None
         elif isinstance(obj, self.PRIMITIVE_TYPES):
             return obj
+        elif isinstance(obj,np.int64) or isinstance(obj,np.int32) or isinstance(obj,np.int16):
+            return int(obj)
         elif isinstance(obj, list):
             return [self.sanitize_for_serialization(sub_obj)
                     for sub_obj in obj]
         elif isinstance(obj, tuple):
             return tuple(self.sanitize_for_serialization(sub_obj)
                          for sub_obj in obj)
         elif isinstance(obj, (datetime.datetime, datetime.date)):
```

### Comparing `gemmapy-0.0.2/gemmapy/sdk/models/array_design_value_object.py` & `gemmapy-1.0.0/gemmapy/sdk/models/array_design_value_object.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gemma RESTful API
 
-    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  Fix return type for `getResultSets` which was incorrectly referring to a renamed VO.  Remove the `security` requirements by default from the specification, which forced the Python package to supply empty credentials. There is currently no privileged endpoints, although some can return additional results.  ## Updates  ### Update 2.5.1  Restore `objectClass` visibility in `AnnotationValueObject`.  Fix incorrect response types for annotations search endpoints returning datasets.  ### Update 2.5.0  Major cleanups were performed in this release in order to stabilize the specification. Numerous properties from Gemma Web that were never intended to be exposed in Gemma REST have been hidden. It's a bit too much to describe in here, but you can navigate to the schemas section below to get a good glance at the models.  Favour `numberOfSomething` instead of `somethingCount` which is clearer. The older names are kept for backward-compatibility, but should be considered deprecated.  Gene aliases and multifunctionality rank are now filled in `GeneValueObject`.  Uniformly use `TaxonValueObject` to represent taxon. This is breaking change for the `ExpressionExperimentValueObject` and `ArrayDesignValueObject` as their `taxon` property will be an `object` instead of a `string`. Properties such as `taxonId` are now deprecated and `taxon.id` should be used instead.  Entities that have IDs now all inherit from `IdentifiableValueObject`. This implies that you can assume the presence of an `id` in a search result `resultObject` attribute for example.  New `/search` endpoint! for an unified search experience. Annotation-based search endpoints under `/annotations` are now deprecated.  New API docs! While not as nice looking, the previous theme will be gradually ported to Swagger UI as we focused on functionality over prettiness for this release.  ### Update 2.4.0 through 2.4.1  Release notes for the 2.4 series were not written down, so I'll try to do my best to recall features that were introduced at that time.  An [OpenAPI](https://www.openapis.org/) specification was introduced and available under `/rest/v2/openapi.json`, although not fully stabilized.  Add a `/resultSets` endpoint to navigate result sets directly, by ID or by dataset.  Add a `/resultSets/{resultSetId}` endpoint to retrieve a specific result set by its ID. This endpoint can be negotiated with an `Accept: text/tab-separated-values` header to obtain a TSV representation.  Add a `/datasets/{dataset}/analyses/differential/resultSets` endpoint that essentially redirect to a specific `/resultSet` endpoint by dataset ID.  Add an endpoint to retrieve preferred raw expression vectors.  ### Update 2.3.4  November 6th, 2018  November 6th [2.3.4] Bug fixes in the dataset search endpoint.  November 5th [2.3.3] Added filtering parameters to dataset search.  October 25th [2.3.2] Changed behavior of the dataset search endpoint to more closely match the Gemma web interface.  October 2nd [2.3.1] Added group information to the User value object.  September 27th [2.3.0] Breaking change in Taxa: Abbreviation property has been removed and is therefore no longer an accepted identifier.  ### Update 2.2.6  June 7th, 2018  Code maintenance, bug fixes. Geeq scores stable and made public.  June 7th [2.2.6] Added: User authentication endpoint.  May 2nd [2.2.5] Fixed: Cleaned up and optimized platforms/elements endpoint, removed redundant information (recursive properties nesting).  April 12th [2.2.3] Fixed: Array arguments not handling non-string properties properly, e.g. `ncbiIds` of genes.  April 9th [2.2.1] Fixed: Filter argument not working when the filtered field was a primitive type. This most significantly allows filtering by geeq boolean and double properties.  ### Update 2.2.0  February 8th, 2018  Breaking change in the 'Dataset differential analysis' endpoint: - No longer using `qValueThreshold` parameter. - Response format changed, now using `DifferentialExpressionAnalysisValueObject` instead of `DifferentialExpressionValueObject` - [Experimental] Added Geeq (Gene Expression Experiment Quality) scores to the dataset value objects   # noqa: E501
+    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  You can [consult the CHANGELOG.md file](https://gemma.msl.ubc.ca/resources/restapidocs/CHANGELOG.md) to view  release notes and recent changes to the Gemma RESTful API.   # noqa: E501
 
-    OpenAPI spec version: 2.5.1
+    OpenAPI spec version: 2.7.4
     Contact: pavlab-support@msl.ubc.ca
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -40,16 +40,19 @@
         'description': 'str',
         'expression_experiment_count': 'int',
         'is_merged': 'bool',
         'is_mergee': 'bool',
         'name': 'str',
         'short_name': 'str',
         'technology_type': 'str',
-        'number_of_expression_experiments': 'int',
+        'release_version': 'str',
+        'release_url': 'str',
+        'external_references': 'list[DatabaseEntryValueObject]',
         'taxon_id': 'int',
+        'number_of_expression_experiments': 'int',
         'trouble_details': 'str',
         'number_of_switched_expression_experiments': 'int',
         'taxon': 'TaxonValueObject'
     }
 
     attribute_map = {
         'id': 'id',
@@ -64,22 +67,25 @@
         'description': 'description',
         'expression_experiment_count': 'expressionExperimentCount',
         'is_merged': 'isMerged',
         'is_mergee': 'isMergee',
         'name': 'name',
         'short_name': 'shortName',
         'technology_type': 'technologyType',
-        'number_of_expression_experiments': 'numberOfExpressionExperiments',
+        'release_version': 'releaseVersion',
+        'release_url': 'releaseUrl',
+        'external_references': 'externalReferences',
         'taxon_id': 'taxonID',
+        'number_of_expression_experiments': 'numberOfExpressionExperiments',
         'trouble_details': 'troubleDetails',
         'number_of_switched_expression_experiments': 'numberOfSwitchedExpressionExperiments',
         'taxon': 'taxon'
     }
 
-    def __init__(self, id=None, last_updated=None, troubled=None, last_troubled_event=None, needs_attention=None, last_needs_attention_event=None, curation_note=None, last_note_update_event=None, color=None, description=None, expression_experiment_count=None, is_merged=None, is_mergee=None, name=None, short_name=None, technology_type=None, number_of_expression_experiments=None, taxon_id=None, trouble_details=None, number_of_switched_expression_experiments=None, taxon=None):  # noqa: E501
+    def __init__(self, id=None, last_updated=None, troubled=None, last_troubled_event=None, needs_attention=None, last_needs_attention_event=None, curation_note=None, last_note_update_event=None, color=None, description=None, expression_experiment_count=None, is_merged=None, is_mergee=None, name=None, short_name=None, technology_type=None, release_version=None, release_url=None, external_references=None, taxon_id=None, number_of_expression_experiments=None, trouble_details=None, number_of_switched_expression_experiments=None, taxon=None):  # noqa: E501
         """ArrayDesignValueObject - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._last_updated = None
         self._troubled = None
         self._last_troubled_event = None
         self._needs_attention = None
         self._last_needs_attention_event = None
@@ -89,16 +95,19 @@
         self._description = None
         self._expression_experiment_count = None
         self._is_merged = None
         self._is_mergee = None
         self._name = None
         self._short_name = None
         self._technology_type = None
-        self._number_of_expression_experiments = None
+        self._release_version = None
+        self._release_url = None
+        self._external_references = None
         self._taxon_id = None
+        self._number_of_expression_experiments = None
         self._trouble_details = None
         self._number_of_switched_expression_experiments = None
         self._taxon = None
         self.discriminator = None
         if id is not None:
             self.id = id
         if last_updated is not None:
@@ -127,18 +136,24 @@
             self.is_mergee = is_mergee
         if name is not None:
             self.name = name
         if short_name is not None:
             self.short_name = short_name
         if technology_type is not None:
             self.technology_type = technology_type
-        if number_of_expression_experiments is not None:
-            self.number_of_expression_experiments = number_of_expression_experiments
+        if release_version is not None:
+            self.release_version = release_version
+        if release_url is not None:
+            self.release_url = release_url
+        if external_references is not None:
+            self.external_references = external_references
         if taxon_id is not None:
             self.taxon_id = taxon_id
+        if number_of_expression_experiments is not None:
+            self.number_of_expression_experiments = number_of_expression_experiments
         if trouble_details is not None:
             self.trouble_details = trouble_details
         if number_of_switched_expression_experiments is not None:
             self.number_of_switched_expression_experiments = number_of_switched_expression_experiments
         if taxon is not None:
             self.taxon = taxon
 
@@ -324,14 +339,20 @@
     def color(self, color):
         """Sets the color of this ArrayDesignValueObject.
 
 
         :param color: The color of this ArrayDesignValueObject.  # noqa: E501
         :type: str
         """
+        allowed_values = ["TWOCOLOR", "DUALMODE", "ONECOLOR", "SEQUENCING", "GENELIST", "OTHER"]  # noqa: E501
+        if color not in allowed_values:
+            raise ValueError(
+                "Invalid value for `color` ({0}), must be one of {1}"  # noqa: E501
+                .format(color, allowed_values)
+            )
 
         self._color = color
 
     @property
     def description(self):
         """Gets the description of this ArrayDesignValueObject.  # noqa: E501
 
@@ -471,37 +492,85 @@
     def technology_type(self, technology_type):
         """Sets the technology_type of this ArrayDesignValueObject.
 
 
         :param technology_type: The technology_type of this ArrayDesignValueObject.  # noqa: E501
         :type: str
         """
+        allowed_values = ["TWOCOLOR", "DUALMODE", "ONECOLOR", "SEQUENCING", "GENELIST", "OTHER"]  # noqa: E501
+        if technology_type not in allowed_values:
+            raise ValueError(
+                "Invalid value for `technology_type` ({0}), must be one of {1}"  # noqa: E501
+                .format(technology_type, allowed_values)
+            )
 
         self._technology_type = technology_type
 
     @property
-    def number_of_expression_experiments(self):
-        """Gets the number_of_expression_experiments of this ArrayDesignValueObject.  # noqa: E501
+    def release_version(self):
+        """Gets the release_version of this ArrayDesignValueObject.  # noqa: E501
 
 
-        :return: The number_of_expression_experiments of this ArrayDesignValueObject.  # noqa: E501
-        :rtype: int
+        :return: The release_version of this ArrayDesignValueObject.  # noqa: E501
+        :rtype: str
         """
-        return self._number_of_expression_experiments
+        return self._release_version
 
-    @number_of_expression_experiments.setter
-    def number_of_expression_experiments(self, number_of_expression_experiments):
-        """Sets the number_of_expression_experiments of this ArrayDesignValueObject.
+    @release_version.setter
+    def release_version(self, release_version):
+        """Sets the release_version of this ArrayDesignValueObject.
 
 
-        :param number_of_expression_experiments: The number_of_expression_experiments of this ArrayDesignValueObject.  # noqa: E501
-        :type: int
+        :param release_version: The release_version of this ArrayDesignValueObject.  # noqa: E501
+        :type: str
         """
 
-        self._number_of_expression_experiments = number_of_expression_experiments
+        self._release_version = release_version
+
+    @property
+    def release_url(self):
+        """Gets the release_url of this ArrayDesignValueObject.  # noqa: E501
+
+
+        :return: The release_url of this ArrayDesignValueObject.  # noqa: E501
+        :rtype: str
+        """
+        return self._release_url
+
+    @release_url.setter
+    def release_url(self, release_url):
+        """Sets the release_url of this ArrayDesignValueObject.
+
+
+        :param release_url: The release_url of this ArrayDesignValueObject.  # noqa: E501
+        :type: str
+        """
+
+        self._release_url = release_url
+
+    @property
+    def external_references(self):
+        """Gets the external_references of this ArrayDesignValueObject.  # noqa: E501
+
+
+        :return: The external_references of this ArrayDesignValueObject.  # noqa: E501
+        :rtype: list[DatabaseEntryValueObject]
+        """
+        return self._external_references
+
+    @external_references.setter
+    def external_references(self, external_references):
+        """Sets the external_references of this ArrayDesignValueObject.
+
+
+        :param external_references: The external_references of this ArrayDesignValueObject.  # noqa: E501
+        :type: list[DatabaseEntryValueObject]
+        """
+
+        self._external_references = external_references
 
     @property
     def taxon_id(self):
         """Gets the taxon_id of this ArrayDesignValueObject.  # noqa: E501
 
 
         :return: The taxon_id of this ArrayDesignValueObject.  # noqa: E501
@@ -517,14 +586,35 @@
         :param taxon_id: The taxon_id of this ArrayDesignValueObject.  # noqa: E501
         :type: int
         """
 
         self._taxon_id = taxon_id
 
     @property
+    def number_of_expression_experiments(self):
+        """Gets the number_of_expression_experiments of this ArrayDesignValueObject.  # noqa: E501
+
+
+        :return: The number_of_expression_experiments of this ArrayDesignValueObject.  # noqa: E501
+        :rtype: int
+        """
+        return self._number_of_expression_experiments
+
+    @number_of_expression_experiments.setter
+    def number_of_expression_experiments(self, number_of_expression_experiments):
+        """Sets the number_of_expression_experiments of this ArrayDesignValueObject.
+
+
+        :param number_of_expression_experiments: The number_of_expression_experiments of this ArrayDesignValueObject.  # noqa: E501
+        :type: int
+        """
+
+        self._number_of_expression_experiments = number_of_expression_experiments
+
+    @property
     def trouble_details(self):
         """Gets the trouble_details of this ArrayDesignValueObject.  # noqa: E501
 
 
         :return: The trouble_details of this ArrayDesignValueObject.  # noqa: E501
         :rtype: str
         """
```

### Comparing `gemmapy-0.0.2/gemmapy/sdk/models/bio_assay_value_object.py` & `gemmapy-1.0.0/gemmapy/sdk/models/bio_assay_value_object.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gemma RESTful API
 
-    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  Fix return type for `getResultSets` which was incorrectly referring to a renamed VO.  Remove the `security` requirements by default from the specification, which forced the Python package to supply empty credentials. There is currently no privileged endpoints, although some can return additional results.  ## Updates  ### Update 2.5.1  Restore `objectClass` visibility in `AnnotationValueObject`.  Fix incorrect response types for annotations search endpoints returning datasets.  ### Update 2.5.0  Major cleanups were performed in this release in order to stabilize the specification. Numerous properties from Gemma Web that were never intended to be exposed in Gemma REST have been hidden. It's a bit too much to describe in here, but you can navigate to the schemas section below to get a good glance at the models.  Favour `numberOfSomething` instead of `somethingCount` which is clearer. The older names are kept for backward-compatibility, but should be considered deprecated.  Gene aliases and multifunctionality rank are now filled in `GeneValueObject`.  Uniformly use `TaxonValueObject` to represent taxon. This is breaking change for the `ExpressionExperimentValueObject` and `ArrayDesignValueObject` as their `taxon` property will be an `object` instead of a `string`. Properties such as `taxonId` are now deprecated and `taxon.id` should be used instead.  Entities that have IDs now all inherit from `IdentifiableValueObject`. This implies that you can assume the presence of an `id` in a search result `resultObject` attribute for example.  New `/search` endpoint! for an unified search experience. Annotation-based search endpoints under `/annotations` are now deprecated.  New API docs! While not as nice looking, the previous theme will be gradually ported to Swagger UI as we focused on functionality over prettiness for this release.  ### Update 2.4.0 through 2.4.1  Release notes for the 2.4 series were not written down, so I'll try to do my best to recall features that were introduced at that time.  An [OpenAPI](https://www.openapis.org/) specification was introduced and available under `/rest/v2/openapi.json`, although not fully stabilized.  Add a `/resultSets` endpoint to navigate result sets directly, by ID or by dataset.  Add a `/resultSets/{resultSetId}` endpoint to retrieve a specific result set by its ID. This endpoint can be negotiated with an `Accept: text/tab-separated-values` header to obtain a TSV representation.  Add a `/datasets/{dataset}/analyses/differential/resultSets` endpoint that essentially redirect to a specific `/resultSet` endpoint by dataset ID.  Add an endpoint to retrieve preferred raw expression vectors.  ### Update 2.3.4  November 6th, 2018  November 6th [2.3.4] Bug fixes in the dataset search endpoint.  November 5th [2.3.3] Added filtering parameters to dataset search.  October 25th [2.3.2] Changed behavior of the dataset search endpoint to more closely match the Gemma web interface.  October 2nd [2.3.1] Added group information to the User value object.  September 27th [2.3.0] Breaking change in Taxa: Abbreviation property has been removed and is therefore no longer an accepted identifier.  ### Update 2.2.6  June 7th, 2018  Code maintenance, bug fixes. Geeq scores stable and made public.  June 7th [2.2.6] Added: User authentication endpoint.  May 2nd [2.2.5] Fixed: Cleaned up and optimized platforms/elements endpoint, removed redundant information (recursive properties nesting).  April 12th [2.2.3] Fixed: Array arguments not handling non-string properties properly, e.g. `ncbiIds` of genes.  April 9th [2.2.1] Fixed: Filter argument not working when the filtered field was a primitive type. This most significantly allows filtering by geeq boolean and double properties.  ### Update 2.2.0  February 8th, 2018  Breaking change in the 'Dataset differential analysis' endpoint: - No longer using `qValueThreshold` parameter. - Response format changed, now using `DifferentialExpressionAnalysisValueObject` instead of `DifferentialExpressionValueObject` - [Experimental] Added Geeq (Gene Expression Experiment Quality) scores to the dataset value objects   # noqa: E501
+    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  You can [consult the CHANGELOG.md file](https://gemma.msl.ubc.ca/resources/restapidocs/CHANGELOG.md) to view  release notes and recent changes to the Gemma RESTful API.   # noqa: E501
 
-    OpenAPI spec version: 2.5.1
+    OpenAPI spec version: 2.7.4
     Contact: pavlab-support@msl.ubc.ca
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -35,14 +35,17 @@
         'metadata': 'str',
         'name': 'str',
         'original_platform': 'ArrayDesignValueObject',
         'outlier': 'bool',
         'predicted_outlier': 'bool',
         'processing_date': 'datetime',
         'sample': 'BioMaterialValueObject',
+        'sequence_paired_reads': 'bool',
+        'sequence_read_count': 'int',
+        'sequence_read_length': 'int',
         'user_flagged_outlier': 'bool'
     }
 
     attribute_map = {
         'id': 'id',
         'accession': 'accession',
         'array_design': 'arrayDesign',
@@ -50,30 +53,36 @@
         'metadata': 'metadata',
         'name': 'name',
         'original_platform': 'originalPlatform',
         'outlier': 'outlier',
         'predicted_outlier': 'predictedOutlier',
         'processing_date': 'processingDate',
         'sample': 'sample',
+        'sequence_paired_reads': 'sequencePairedReads',
+        'sequence_read_count': 'sequenceReadCount',
+        'sequence_read_length': 'sequenceReadLength',
         'user_flagged_outlier': 'userFlaggedOutlier'
     }
 
-    def __init__(self, id=None, accession=None, array_design=None, description=None, metadata=None, name=None, original_platform=None, outlier=None, predicted_outlier=None, processing_date=None, sample=None, user_flagged_outlier=None):  # noqa: E501
+    def __init__(self, id=None, accession=None, array_design=None, description=None, metadata=None, name=None, original_platform=None, outlier=None, predicted_outlier=None, processing_date=None, sample=None, sequence_paired_reads=None, sequence_read_count=None, sequence_read_length=None, user_flagged_outlier=None):  # noqa: E501
         """BioAssayValueObject - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._accession = None
         self._array_design = None
         self._description = None
         self._metadata = None
         self._name = None
         self._original_platform = None
         self._outlier = None
         self._predicted_outlier = None
         self._processing_date = None
         self._sample = None
+        self._sequence_paired_reads = None
+        self._sequence_read_count = None
+        self._sequence_read_length = None
         self._user_flagged_outlier = None
         self.discriminator = None
         if id is not None:
             self.id = id
         if accession is not None:
             self.accession = accession
         if array_design is not None:
@@ -90,14 +99,20 @@
             self.outlier = outlier
         if predicted_outlier is not None:
             self.predicted_outlier = predicted_outlier
         if processing_date is not None:
             self.processing_date = processing_date
         if sample is not None:
             self.sample = sample
+        if sequence_paired_reads is not None:
+            self.sequence_paired_reads = sequence_paired_reads
+        if sequence_read_count is not None:
+            self.sequence_read_count = sequence_read_count
+        if sequence_read_length is not None:
+            self.sequence_read_length = sequence_read_length
         if user_flagged_outlier is not None:
             self.user_flagged_outlier = user_flagged_outlier
 
     @property
     def id(self):
         """Gets the id of this BioAssayValueObject.  # noqa: E501
 
@@ -325,14 +340,77 @@
         :param sample: The sample of this BioAssayValueObject.  # noqa: E501
         :type: BioMaterialValueObject
         """
 
         self._sample = sample
 
     @property
+    def sequence_paired_reads(self):
+        """Gets the sequence_paired_reads of this BioAssayValueObject.  # noqa: E501
+
+
+        :return: The sequence_paired_reads of this BioAssayValueObject.  # noqa: E501
+        :rtype: bool
+        """
+        return self._sequence_paired_reads
+
+    @sequence_paired_reads.setter
+    def sequence_paired_reads(self, sequence_paired_reads):
+        """Sets the sequence_paired_reads of this BioAssayValueObject.
+
+
+        :param sequence_paired_reads: The sequence_paired_reads of this BioAssayValueObject.  # noqa: E501
+        :type: bool
+        """
+
+        self._sequence_paired_reads = sequence_paired_reads
+
+    @property
+    def sequence_read_count(self):
+        """Gets the sequence_read_count of this BioAssayValueObject.  # noqa: E501
+
+
+        :return: The sequence_read_count of this BioAssayValueObject.  # noqa: E501
+        :rtype: int
+        """
+        return self._sequence_read_count
+
+    @sequence_read_count.setter
+    def sequence_read_count(self, sequence_read_count):
+        """Sets the sequence_read_count of this BioAssayValueObject.
+
+
+        :param sequence_read_count: The sequence_read_count of this BioAssayValueObject.  # noqa: E501
+        :type: int
+        """
+
+        self._sequence_read_count = sequence_read_count
+
+    @property
+    def sequence_read_length(self):
+        """Gets the sequence_read_length of this BioAssayValueObject.  # noqa: E501
+
+
+        :return: The sequence_read_length of this BioAssayValueObject.  # noqa: E501
+        :rtype: int
+        """
+        return self._sequence_read_length
+
+    @sequence_read_length.setter
+    def sequence_read_length(self, sequence_read_length):
+        """Sets the sequence_read_length of this BioAssayValueObject.
+
+
+        :param sequence_read_length: The sequence_read_length of this BioAssayValueObject.  # noqa: E501
+        :type: int
+        """
+
+        self._sequence_read_length = sequence_read_length
+
+    @property
     def user_flagged_outlier(self):
         """Gets the user_flagged_outlier of this BioAssayValueObject.  # noqa: E501
 
 
         :return: The user_flagged_outlier of this BioAssayValueObject.  # noqa: E501
         :rtype: bool
         """
```

### Comparing `gemmapy-0.0.2/gemmapy/sdk/models/expression_experiment_value_object.py` & `gemmapy-1.0.0/gemmapy/sdk/models/expression_experiment_value_object.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gemma RESTful API
 
-    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  Fix return type for `getResultSets` which was incorrectly referring to a renamed VO.  Remove the `security` requirements by default from the specification, which forced the Python package to supply empty credentials. There is currently no privileged endpoints, although some can return additional results.  ## Updates  ### Update 2.5.1  Restore `objectClass` visibility in `AnnotationValueObject`.  Fix incorrect response types for annotations search endpoints returning datasets.  ### Update 2.5.0  Major cleanups were performed in this release in order to stabilize the specification. Numerous properties from Gemma Web that were never intended to be exposed in Gemma REST have been hidden. It's a bit too much to describe in here, but you can navigate to the schemas section below to get a good glance at the models.  Favour `numberOfSomething` instead of `somethingCount` which is clearer. The older names are kept for backward-compatibility, but should be considered deprecated.  Gene aliases and multifunctionality rank are now filled in `GeneValueObject`.  Uniformly use `TaxonValueObject` to represent taxon. This is breaking change for the `ExpressionExperimentValueObject` and `ArrayDesignValueObject` as their `taxon` property will be an `object` instead of a `string`. Properties such as `taxonId` are now deprecated and `taxon.id` should be used instead.  Entities that have IDs now all inherit from `IdentifiableValueObject`. This implies that you can assume the presence of an `id` in a search result `resultObject` attribute for example.  New `/search` endpoint! for an unified search experience. Annotation-based search endpoints under `/annotations` are now deprecated.  New API docs! While not as nice looking, the previous theme will be gradually ported to Swagger UI as we focused on functionality over prettiness for this release.  ### Update 2.4.0 through 2.4.1  Release notes for the 2.4 series were not written down, so I'll try to do my best to recall features that were introduced at that time.  An [OpenAPI](https://www.openapis.org/) specification was introduced and available under `/rest/v2/openapi.json`, although not fully stabilized.  Add a `/resultSets` endpoint to navigate result sets directly, by ID or by dataset.  Add a `/resultSets/{resultSetId}` endpoint to retrieve a specific result set by its ID. This endpoint can be negotiated with an `Accept: text/tab-separated-values` header to obtain a TSV representation.  Add a `/datasets/{dataset}/analyses/differential/resultSets` endpoint that essentially redirect to a specific `/resultSet` endpoint by dataset ID.  Add an endpoint to retrieve preferred raw expression vectors.  ### Update 2.3.4  November 6th, 2018  November 6th [2.3.4] Bug fixes in the dataset search endpoint.  November 5th [2.3.3] Added filtering parameters to dataset search.  October 25th [2.3.2] Changed behavior of the dataset search endpoint to more closely match the Gemma web interface.  October 2nd [2.3.1] Added group information to the User value object.  September 27th [2.3.0] Breaking change in Taxa: Abbreviation property has been removed and is therefore no longer an accepted identifier.  ### Update 2.2.6  June 7th, 2018  Code maintenance, bug fixes. Geeq scores stable and made public.  June 7th [2.2.6] Added: User authentication endpoint.  May 2nd [2.2.5] Fixed: Cleaned up and optimized platforms/elements endpoint, removed redundant information (recursive properties nesting).  April 12th [2.2.3] Fixed: Array arguments not handling non-string properties properly, e.g. `ncbiIds` of genes.  April 9th [2.2.1] Fixed: Filter argument not working when the filtered field was a primitive type. This most significantly allows filtering by geeq boolean and double properties.  ### Update 2.2.0  February 8th, 2018  Breaking change in the 'Dataset differential analysis' endpoint: - No longer using `qValueThreshold` parameter. - Response format changed, now using `DifferentialExpressionAnalysisValueObject` instead of `DifferentialExpressionValueObject` - [Experimental] Added Geeq (Gene Expression Experiment Quality) scores to the dataset value objects   # noqa: E501
+    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  You can [consult the CHANGELOG.md file](https://gemma.msl.ubc.ca/resources/restapidocs/CHANGELOG.md) to view  release notes and recent changes to the Gemma RESTful API.   # noqa: E501
 
-    OpenAPI spec version: 2.5.1
+    OpenAPI spec version: 2.7.4
     Contact: pavlab-support@msl.ubc.ca
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -38,15 +38,17 @@
         'last_note_update_event': 'AuditEventValueObject',
         'number_of_bio_assays': 'int',
         'description': 'str',
         'name': 'str',
         'accession': 'str',
         'batch_confound': 'str',
         'batch_effect': 'str',
+        'batch_effect_statistics': 'str',
         'external_database': 'str',
+        'external_database_uri': 'str',
         'external_uri': 'str',
         'geeq': 'GeeqValueObject',
         'metadata': 'str',
         'short_name': 'str',
         'source': 'str',
         'technology_type': 'str',
         'taxon_id': 'int',
@@ -68,30 +70,32 @@
         'last_note_update_event': 'lastNoteUpdateEvent',
         'number_of_bio_assays': 'numberOfBioAssays',
         'description': 'description',
         'name': 'name',
         'accession': 'accession',
         'batch_confound': 'batchConfound',
         'batch_effect': 'batchEffect',
+        'batch_effect_statistics': 'batchEffectStatistics',
         'external_database': 'externalDatabase',
+        'external_database_uri': 'externalDatabaseUri',
         'external_uri': 'externalUri',
         'geeq': 'geeq',
         'metadata': 'metadata',
         'short_name': 'shortName',
         'source': 'source',
         'technology_type': 'technologyType',
         'taxon_id': 'taxonId',
         'bio_assay_count': 'bioAssayCount',
         'trouble_details': 'troubleDetails',
         'number_of_array_designs': 'numberOfArrayDesigns',
         'number_of_processed_expression_vectors': 'numberOfProcessedExpressionVectors',
         'taxon': 'taxon'
     }
 
-    def __init__(self, id=None, last_updated=None, troubled=None, last_troubled_event=None, needs_attention=None, last_needs_attention_event=None, curation_note=None, last_note_update_event=None, number_of_bio_assays=None, description=None, name=None, accession=None, batch_confound=None, batch_effect=None, external_database=None, external_uri=None, geeq=None, metadata=None, short_name=None, source=None, technology_type=None, taxon_id=None, bio_assay_count=None, trouble_details=None, number_of_array_designs=None, number_of_processed_expression_vectors=None, taxon=None):  # noqa: E501
+    def __init__(self, id=None, last_updated=None, troubled=None, last_troubled_event=None, needs_attention=None, last_needs_attention_event=None, curation_note=None, last_note_update_event=None, number_of_bio_assays=None, description=None, name=None, accession=None, batch_confound=None, batch_effect=None, batch_effect_statistics=None, external_database=None, external_database_uri=None, external_uri=None, geeq=None, metadata=None, short_name=None, source=None, technology_type=None, taxon_id=None, bio_assay_count=None, trouble_details=None, number_of_array_designs=None, number_of_processed_expression_vectors=None, taxon=None):  # noqa: E501
         """ExpressionExperimentValueObject - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._last_updated = None
         self._troubled = None
         self._last_troubled_event = None
         self._needs_attention = None
         self._last_needs_attention_event = None
@@ -99,15 +103,17 @@
         self._last_note_update_event = None
         self._number_of_bio_assays = None
         self._description = None
         self._name = None
         self._accession = None
         self._batch_confound = None
         self._batch_effect = None
+        self._batch_effect_statistics = None
         self._external_database = None
+        self._external_database_uri = None
         self._external_uri = None
         self._geeq = None
         self._metadata = None
         self._short_name = None
         self._source = None
         self._technology_type = None
         self._taxon_id = None
@@ -141,16 +147,20 @@
             self.name = name
         if accession is not None:
             self.accession = accession
         if batch_confound is not None:
             self.batch_confound = batch_confound
         if batch_effect is not None:
             self.batch_effect = batch_effect
+        if batch_effect_statistics is not None:
+            self.batch_effect_statistics = batch_effect_statistics
         if external_database is not None:
             self.external_database = external_database
+        if external_database_uri is not None:
+            self.external_database_uri = external_database_uri
         if external_uri is not None:
             self.external_uri = external_uri
         if geeq is not None:
             self.geeq = geeq
         if metadata is not None:
             self.metadata = metadata
         if short_name is not None:
@@ -459,18 +469,45 @@
     def batch_effect(self, batch_effect):
         """Sets the batch_effect of this ExpressionExperimentValueObject.
 
 
         :param batch_effect: The batch_effect of this ExpressionExperimentValueObject.  # noqa: E501
         :type: str
         """
+        allowed_values = ["NO_BATCH_INFO", "SINGLETON_BATCHES_FAILURE", "UNINFORMATIVE_HEADERS_FAILURE", "PROBLEMATIC_BATCH_INFO_FAILURE", "BATCH_EFFECT_FAILURE", "BATCH_CORRECTED_SUCCESS", "SINGLE_BATCH_SUCCESS", "BATCH_EFFECT_UNDETERMINED_FAILURE", "NO_BATCH_EFFECT_SUCCESS"]  # noqa: E501
+        if batch_effect not in allowed_values:
+            raise ValueError(
+                "Invalid value for `batch_effect` ({0}), must be one of {1}"  # noqa: E501
+                .format(batch_effect, allowed_values)
+            )
 
         self._batch_effect = batch_effect
 
     @property
+    def batch_effect_statistics(self):
+        """Gets the batch_effect_statistics of this ExpressionExperimentValueObject.  # noqa: E501
+
+
+        :return: The batch_effect_statistics of this ExpressionExperimentValueObject.  # noqa: E501
+        :rtype: str
+        """
+        return self._batch_effect_statistics
+
+    @batch_effect_statistics.setter
+    def batch_effect_statistics(self, batch_effect_statistics):
+        """Sets the batch_effect_statistics of this ExpressionExperimentValueObject.
+
+
+        :param batch_effect_statistics: The batch_effect_statistics of this ExpressionExperimentValueObject.  # noqa: E501
+        :type: str
+        """
+
+        self._batch_effect_statistics = batch_effect_statistics
+
+    @property
     def external_database(self):
         """Gets the external_database of this ExpressionExperimentValueObject.  # noqa: E501
 
 
         :return: The external_database of this ExpressionExperimentValueObject.  # noqa: E501
         :rtype: str
         """
@@ -484,14 +521,35 @@
         :param external_database: The external_database of this ExpressionExperimentValueObject.  # noqa: E501
         :type: str
         """
 
         self._external_database = external_database
 
     @property
+    def external_database_uri(self):
+        """Gets the external_database_uri of this ExpressionExperimentValueObject.  # noqa: E501
+
+
+        :return: The external_database_uri of this ExpressionExperimentValueObject.  # noqa: E501
+        :rtype: str
+        """
+        return self._external_database_uri
+
+    @external_database_uri.setter
+    def external_database_uri(self, external_database_uri):
+        """Sets the external_database_uri of this ExpressionExperimentValueObject.
+
+
+        :param external_database_uri: The external_database_uri of this ExpressionExperimentValueObject.  # noqa: E501
+        :type: str
+        """
+
+        self._external_database_uri = external_database_uri
+
+    @property
     def external_uri(self):
         """Gets the external_uri of this ExpressionExperimentValueObject.  # noqa: E501
 
 
         :return: The external_uri of this ExpressionExperimentValueObject.  # noqa: E501
         :rtype: str
         """
```

### Comparing `gemmapy-0.0.2/gemmapy/sdk/models/factor_value_value_object.py` & `gemmapy-1.0.0/gemmapy/sdk/models/factor_value_value_object.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gemma RESTful API
 
-    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  Fix return type for `getResultSets` which was incorrectly referring to a renamed VO.  Remove the `security` requirements by default from the specification, which forced the Python package to supply empty credentials. There is currently no privileged endpoints, although some can return additional results.  ## Updates  ### Update 2.5.1  Restore `objectClass` visibility in `AnnotationValueObject`.  Fix incorrect response types for annotations search endpoints returning datasets.  ### Update 2.5.0  Major cleanups were performed in this release in order to stabilize the specification. Numerous properties from Gemma Web that were never intended to be exposed in Gemma REST have been hidden. It's a bit too much to describe in here, but you can navigate to the schemas section below to get a good glance at the models.  Favour `numberOfSomething` instead of `somethingCount` which is clearer. The older names are kept for backward-compatibility, but should be considered deprecated.  Gene aliases and multifunctionality rank are now filled in `GeneValueObject`.  Uniformly use `TaxonValueObject` to represent taxon. This is breaking change for the `ExpressionExperimentValueObject` and `ArrayDesignValueObject` as their `taxon` property will be an `object` instead of a `string`. Properties such as `taxonId` are now deprecated and `taxon.id` should be used instead.  Entities that have IDs now all inherit from `IdentifiableValueObject`. This implies that you can assume the presence of an `id` in a search result `resultObject` attribute for example.  New `/search` endpoint! for an unified search experience. Annotation-based search endpoints under `/annotations` are now deprecated.  New API docs! While not as nice looking, the previous theme will be gradually ported to Swagger UI as we focused on functionality over prettiness for this release.  ### Update 2.4.0 through 2.4.1  Release notes for the 2.4 series were not written down, so I'll try to do my best to recall features that were introduced at that time.  An [OpenAPI](https://www.openapis.org/) specification was introduced and available under `/rest/v2/openapi.json`, although not fully stabilized.  Add a `/resultSets` endpoint to navigate result sets directly, by ID or by dataset.  Add a `/resultSets/{resultSetId}` endpoint to retrieve a specific result set by its ID. This endpoint can be negotiated with an `Accept: text/tab-separated-values` header to obtain a TSV representation.  Add a `/datasets/{dataset}/analyses/differential/resultSets` endpoint that essentially redirect to a specific `/resultSet` endpoint by dataset ID.  Add an endpoint to retrieve preferred raw expression vectors.  ### Update 2.3.4  November 6th, 2018  November 6th [2.3.4] Bug fixes in the dataset search endpoint.  November 5th [2.3.3] Added filtering parameters to dataset search.  October 25th [2.3.2] Changed behavior of the dataset search endpoint to more closely match the Gemma web interface.  October 2nd [2.3.1] Added group information to the User value object.  September 27th [2.3.0] Breaking change in Taxa: Abbreviation property has been removed and is therefore no longer an accepted identifier.  ### Update 2.2.6  June 7th, 2018  Code maintenance, bug fixes. Geeq scores stable and made public.  June 7th [2.2.6] Added: User authentication endpoint.  May 2nd [2.2.5] Fixed: Cleaned up and optimized platforms/elements endpoint, removed redundant information (recursive properties nesting).  April 12th [2.2.3] Fixed: Array arguments not handling non-string properties properly, e.g. `ncbiIds` of genes.  April 9th [2.2.1] Fixed: Filter argument not working when the filtered field was a primitive type. This most significantly allows filtering by geeq boolean and double properties.  ### Update 2.2.0  February 8th, 2018  Breaking change in the 'Dataset differential analysis' endpoint: - No longer using `qValueThreshold` parameter. - Response format changed, now using `DifferentialExpressionAnalysisValueObject` instead of `DifferentialExpressionValueObject` - [Experimental] Added Geeq (Gene Expression Experiment Quality) scores to the dataset value objects   # noqa: E501
+    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  You can [consult the CHANGELOG.md file](https://gemma.msl.ubc.ca/resources/restapidocs/CHANGELOG.md) to view  release notes and recent changes to the Gemma RESTful API.   # noqa: E501
 
-    OpenAPI spec version: 2.5.1
+    OpenAPI spec version: 2.7.4
     Contact: pavlab-support@msl.ubc.ca
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -25,74 +25,94 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'id': 'int',
+        'ontology_id': 'str',
+        'experimental_factor_id': 'int',
+        'experimental_factor_category': 'CharacteristicValueObject',
+        'characteristics': 'list[CharacteristicValueObject]',
+        'statements': 'list[StatementValueObject]',
+        'summary': 'str',
+        'factor_id': 'int',
+        'char_id': 'int',
         'category': 'str',
         'category_uri': 'str',
         'description': 'str',
-        'value': 'str',
-        'value_uri': 'str',
-        'char_id': 'int',
-        'factor_id': 'int',
         'factor_value': 'str',
-        'is_baseline': 'bool',
+        'measurement': 'MeasurementValueObject',
         'is_measurement': 'bool'
     }
 
     attribute_map = {
         'id': 'id',
+        'ontology_id': 'ontologyId',
+        'experimental_factor_id': 'experimentalFactorId',
+        'experimental_factor_category': 'experimentalFactorCategory',
+        'characteristics': 'characteristics',
+        'statements': 'statements',
+        'summary': 'summary',
+        'factor_id': 'factorId',
+        'char_id': 'charId',
         'category': 'category',
         'category_uri': 'categoryUri',
         'description': 'description',
-        'value': 'value',
-        'value_uri': 'valueUri',
-        'char_id': 'charId',
-        'factor_id': 'factorId',
         'factor_value': 'factorValue',
-        'is_baseline': 'isBaseline',
+        'measurement': 'measurement',
         'is_measurement': 'isMeasurement'
     }
 
-    def __init__(self, id=None, category=None, category_uri=None, description=None, value=None, value_uri=None, char_id=None, factor_id=None, factor_value=None, is_baseline=None, is_measurement=None):  # noqa: E501
+    def __init__(self, id=None, ontology_id=None, experimental_factor_id=None, experimental_factor_category=None, characteristics=None, statements=None, summary=None, factor_id=None, char_id=None, category=None, category_uri=None, description=None, factor_value=None, measurement=None, is_measurement=None):  # noqa: E501
         """FactorValueValueObject - a model defined in Swagger"""  # noqa: E501
         self._id = None
+        self._ontology_id = None
+        self._experimental_factor_id = None
+        self._experimental_factor_category = None
+        self._characteristics = None
+        self._statements = None
+        self._summary = None
+        self._factor_id = None
+        self._char_id = None
         self._category = None
         self._category_uri = None
         self._description = None
-        self._value = None
-        self._value_uri = None
-        self._char_id = None
-        self._factor_id = None
         self._factor_value = None
-        self._is_baseline = None
+        self._measurement = None
         self._is_measurement = None
         self.discriminator = None
         if id is not None:
             self.id = id
+        if ontology_id is not None:
+            self.ontology_id = ontology_id
+        if experimental_factor_id is not None:
+            self.experimental_factor_id = experimental_factor_id
+        if experimental_factor_category is not None:
+            self.experimental_factor_category = experimental_factor_category
+        if characteristics is not None:
+            self.characteristics = characteristics
+        if statements is not None:
+            self.statements = statements
+        if summary is not None:
+            self.summary = summary
+        if factor_id is not None:
+            self.factor_id = factor_id
+        if char_id is not None:
+            self.char_id = char_id
         if category is not None:
             self.category = category
         if category_uri is not None:
             self.category_uri = category_uri
         if description is not None:
             self.description = description
-        if value is not None:
-            self.value = value
-        if value_uri is not None:
-            self.value_uri = value_uri
-        if char_id is not None:
-            self.char_id = char_id
-        if factor_id is not None:
-            self.factor_id = factor_id
         if factor_value is not None:
             self.factor_value = factor_value
-        if is_baseline is not None:
-            self.is_baseline = is_baseline
+        if measurement is not None:
+            self.measurement = measurement
         if is_measurement is not None:
             self.is_measurement = is_measurement
 
     @property
     def id(self):
         """Gets the id of this FactorValueValueObject.  # noqa: E501
 
@@ -110,216 +130,314 @@
         :param id: The id of this FactorValueValueObject.  # noqa: E501
         :type: int
         """
 
         self._id = id
 
     @property
-    def category(self):
-        """Gets the category of this FactorValueValueObject.  # noqa: E501
+    def ontology_id(self):
+        """Gets the ontology_id of this FactorValueValueObject.  # noqa: E501
 
 
-        :return: The category of this FactorValueValueObject.  # noqa: E501
+        :return: The ontology_id of this FactorValueValueObject.  # noqa: E501
         :rtype: str
         """
-        return self._category
+        return self._ontology_id
 
-    @category.setter
-    def category(self, category):
-        """Sets the category of this FactorValueValueObject.
+    @ontology_id.setter
+    def ontology_id(self, ontology_id):
+        """Sets the ontology_id of this FactorValueValueObject.
 
 
-        :param category: The category of this FactorValueValueObject.  # noqa: E501
+        :param ontology_id: The ontology_id of this FactorValueValueObject.  # noqa: E501
         :type: str
         """
 
-        self._category = category
+        self._ontology_id = ontology_id
 
     @property
-    def category_uri(self):
-        """Gets the category_uri of this FactorValueValueObject.  # noqa: E501
+    def experimental_factor_id(self):
+        """Gets the experimental_factor_id of this FactorValueValueObject.  # noqa: E501
 
 
-        :return: The category_uri of this FactorValueValueObject.  # noqa: E501
-        :rtype: str
+        :return: The experimental_factor_id of this FactorValueValueObject.  # noqa: E501
+        :rtype: int
         """
-        return self._category_uri
+        return self._experimental_factor_id
 
-    @category_uri.setter
-    def category_uri(self, category_uri):
-        """Sets the category_uri of this FactorValueValueObject.
+    @experimental_factor_id.setter
+    def experimental_factor_id(self, experimental_factor_id):
+        """Sets the experimental_factor_id of this FactorValueValueObject.
 
 
-        :param category_uri: The category_uri of this FactorValueValueObject.  # noqa: E501
-        :type: str
+        :param experimental_factor_id: The experimental_factor_id of this FactorValueValueObject.  # noqa: E501
+        :type: int
         """
 
-        self._category_uri = category_uri
+        self._experimental_factor_id = experimental_factor_id
 
     @property
-    def description(self):
-        """Gets the description of this FactorValueValueObject.  # noqa: E501
+    def experimental_factor_category(self):
+        """Gets the experimental_factor_category of this FactorValueValueObject.  # noqa: E501
 
 
-        :return: The description of this FactorValueValueObject.  # noqa: E501
-        :rtype: str
+        :return: The experimental_factor_category of this FactorValueValueObject.  # noqa: E501
+        :rtype: CharacteristicValueObject
         """
-        return self._description
+        return self._experimental_factor_category
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this FactorValueValueObject.
+    @experimental_factor_category.setter
+    def experimental_factor_category(self, experimental_factor_category):
+        """Sets the experimental_factor_category of this FactorValueValueObject.
 
 
-        :param description: The description of this FactorValueValueObject.  # noqa: E501
-        :type: str
+        :param experimental_factor_category: The experimental_factor_category of this FactorValueValueObject.  # noqa: E501
+        :type: CharacteristicValueObject
         """
 
-        self._description = description
+        self._experimental_factor_category = experimental_factor_category
 
     @property
-    def value(self):
-        """Gets the value of this FactorValueValueObject.  # noqa: E501
+    def characteristics(self):
+        """Gets the characteristics of this FactorValueValueObject.  # noqa: E501
 
 
-        :return: The value of this FactorValueValueObject.  # noqa: E501
-        :rtype: str
+        :return: The characteristics of this FactorValueValueObject.  # noqa: E501
+        :rtype: list[CharacteristicValueObject]
         """
-        return self._value
+        return self._characteristics
 
-    @value.setter
-    def value(self, value):
-        """Sets the value of this FactorValueValueObject.
+    @characteristics.setter
+    def characteristics(self, characteristics):
+        """Sets the characteristics of this FactorValueValueObject.
 
 
-        :param value: The value of this FactorValueValueObject.  # noqa: E501
-        :type: str
+        :param characteristics: The characteristics of this FactorValueValueObject.  # noqa: E501
+        :type: list[CharacteristicValueObject]
+        """
+
+        self._characteristics = characteristics
+
+    @property
+    def statements(self):
+        """Gets the statements of this FactorValueValueObject.  # noqa: E501
+
+
+        :return: The statements of this FactorValueValueObject.  # noqa: E501
+        :rtype: list[StatementValueObject]
+        """
+        return self._statements
+
+    @statements.setter
+    def statements(self, statements):
+        """Sets the statements of this FactorValueValueObject.
+
+
+        :param statements: The statements of this FactorValueValueObject.  # noqa: E501
+        :type: list[StatementValueObject]
         """
 
-        self._value = value
+        self._statements = statements
 
     @property
-    def value_uri(self):
-        """Gets the value_uri of this FactorValueValueObject.  # noqa: E501
+    def summary(self):
+        """Gets the summary of this FactorValueValueObject.  # noqa: E501
 
 
-        :return: The value_uri of this FactorValueValueObject.  # noqa: E501
+        :return: The summary of this FactorValueValueObject.  # noqa: E501
         :rtype: str
         """
-        return self._value_uri
+        return self._summary
 
-    @value_uri.setter
-    def value_uri(self, value_uri):
-        """Sets the value_uri of this FactorValueValueObject.
+    @summary.setter
+    def summary(self, summary):
+        """Sets the summary of this FactorValueValueObject.
 
 
-        :param value_uri: The value_uri of this FactorValueValueObject.  # noqa: E501
+        :param summary: The summary of this FactorValueValueObject.  # noqa: E501
         :type: str
         """
 
-        self._value_uri = value_uri
+        self._summary = summary
+
+    @property
+    def factor_id(self):
+        """Gets the factor_id of this FactorValueValueObject.  # noqa: E501
+
+        Use `experimentalFactorId` instead.  # noqa: E501
+
+        :return: The factor_id of this FactorValueValueObject.  # noqa: E501
+        :rtype: int
+        """
+        return self._factor_id
+
+    @factor_id.setter
+    def factor_id(self, factor_id):
+        """Sets the factor_id of this FactorValueValueObject.
+
+        Use `experimentalFactorId` instead.  # noqa: E501
+
+        :param factor_id: The factor_id of this FactorValueValueObject.  # noqa: E501
+        :type: int
+        """
+
+        self._factor_id = factor_id
 
     @property
     def char_id(self):
         """Gets the char_id of this FactorValueValueObject.  # noqa: E501
 
+        Use `measurement.id` or `characteristics.id` instead.  # noqa: E501
 
         :return: The char_id of this FactorValueValueObject.  # noqa: E501
         :rtype: int
         """
         return self._char_id
 
     @char_id.setter
     def char_id(self, char_id):
         """Sets the char_id of this FactorValueValueObject.
 
+        Use `measurement.id` or `characteristics.id` instead.  # noqa: E501
 
         :param char_id: The char_id of this FactorValueValueObject.  # noqa: E501
         :type: int
         """
 
         self._char_id = char_id
 
     @property
-    def factor_id(self):
-        """Gets the factor_id of this FactorValueValueObject.  # noqa: E501
+    def category(self):
+        """Gets the category of this FactorValueValueObject.  # noqa: E501
 
+        Use experimentalFactorCategory.category instead.  # noqa: E501
 
-        :return: The factor_id of this FactorValueValueObject.  # noqa: E501
-        :rtype: int
+        :return: The category of this FactorValueValueObject.  # noqa: E501
+        :rtype: str
         """
-        return self._factor_id
+        return self._category
 
-    @factor_id.setter
-    def factor_id(self, factor_id):
-        """Sets the factor_id of this FactorValueValueObject.
+    @category.setter
+    def category(self, category):
+        """Sets the category of this FactorValueValueObject.
 
+        Use experimentalFactorCategory.category instead.  # noqa: E501
 
-        :param factor_id: The factor_id of this FactorValueValueObject.  # noqa: E501
-        :type: int
+        :param category: The category of this FactorValueValueObject.  # noqa: E501
+        :type: str
         """
 
-        self._factor_id = factor_id
+        self._category = category
+
+    @property
+    def category_uri(self):
+        """Gets the category_uri of this FactorValueValueObject.  # noqa: E501
+
+        Use experimentalFactorCategory.categoryUri instead.  # noqa: E501
+
+        :return: The category_uri of this FactorValueValueObject.  # noqa: E501
+        :rtype: str
+        """
+        return self._category_uri
+
+    @category_uri.setter
+    def category_uri(self, category_uri):
+        """Sets the category_uri of this FactorValueValueObject.
+
+        Use experimentalFactorCategory.categoryUri instead.  # noqa: E501
+
+        :param category_uri: The category_uri of this FactorValueValueObject.  # noqa: E501
+        :type: str
+        """
+
+        self._category_uri = category_uri
+
+    @property
+    def description(self):
+        """Gets the description of this FactorValueValueObject.  # noqa: E501
+
+        This property is never filled nor used; use `summary` if you need a human-readable representation of this factor value.  # noqa: E501
+
+        :return: The description of this FactorValueValueObject.  # noqa: E501
+        :rtype: str
+        """
+        return self._description
+
+    @description.setter
+    def description(self, description):
+        """Sets the description of this FactorValueValueObject.
+
+        This property is never filled nor used; use `summary` if you need a human-readable representation of this factor value.  # noqa: E501
+
+        :param description: The description of this FactorValueValueObject.  # noqa: E501
+        :type: str
+        """
+
+        self._description = description
 
     @property
     def factor_value(self):
         """Gets the factor_value of this FactorValueValueObject.  # noqa: E501
 
+        Use `summary` if you need a human-readable representation of this factor value or lookup the `characteristics` bag.  # noqa: E501
 
         :return: The factor_value of this FactorValueValueObject.  # noqa: E501
         :rtype: str
         """
         return self._factor_value
 
     @factor_value.setter
     def factor_value(self, factor_value):
         """Sets the factor_value of this FactorValueValueObject.
 
+        Use `summary` if you need a human-readable representation of this factor value or lookup the `characteristics` bag.  # noqa: E501
 
         :param factor_value: The factor_value of this FactorValueValueObject.  # noqa: E501
         :type: str
         """
 
         self._factor_value = factor_value
 
     @property
-    def is_baseline(self):
-        """Gets the is_baseline of this FactorValueValueObject.  # noqa: E501
+    def measurement(self):
+        """Gets the measurement of this FactorValueValueObject.  # noqa: E501
 
 
-        :return: The is_baseline of this FactorValueValueObject.  # noqa: E501
-        :rtype: bool
+        :return: The measurement of this FactorValueValueObject.  # noqa: E501
+        :rtype: MeasurementValueObject
         """
-        return self._is_baseline
+        return self._measurement
 
-    @is_baseline.setter
-    def is_baseline(self, is_baseline):
-        """Sets the is_baseline of this FactorValueValueObject.
+    @measurement.setter
+    def measurement(self, measurement):
+        """Sets the measurement of this FactorValueValueObject.
 
 
-        :param is_baseline: The is_baseline of this FactorValueValueObject.  # noqa: E501
-        :type: bool
+        :param measurement: The measurement of this FactorValueValueObject.  # noqa: E501
+        :type: MeasurementValueObject
         """
 
-        self._is_baseline = is_baseline
+        self._measurement = measurement
 
     @property
     def is_measurement(self):
         """Gets the is_measurement of this FactorValueValueObject.  # noqa: E501
 
+        Check if a `measurement` key exists instead.  # noqa: E501
 
         :return: The is_measurement of this FactorValueValueObject.  # noqa: E501
         :rtype: bool
         """
         return self._is_measurement
 
     @is_measurement.setter
     def is_measurement(self, is_measurement):
         """Sets the is_measurement of this FactorValueValueObject.
 
+        Check if a `measurement` key exists instead.  # noqa: E501
 
         :param is_measurement: The is_measurement of this FactorValueValueObject.  # noqa: E501
         :type: bool
         """
 
         self._is_measurement = is_measurement
```

### Comparing `gemmapy-0.0.2/gemmapy/sdk/models/geeq_value_object.py` & `gemmapy-1.0.0/gemmapy/sdk/models/geeq_value_object.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gemma RESTful API
 
-    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  Fix return type for `getResultSets` which was incorrectly referring to a renamed VO.  Remove the `security` requirements by default from the specification, which forced the Python package to supply empty credentials. There is currently no privileged endpoints, although some can return additional results.  ## Updates  ### Update 2.5.1  Restore `objectClass` visibility in `AnnotationValueObject`.  Fix incorrect response types for annotations search endpoints returning datasets.  ### Update 2.5.0  Major cleanups were performed in this release in order to stabilize the specification. Numerous properties from Gemma Web that were never intended to be exposed in Gemma REST have been hidden. It's a bit too much to describe in here, but you can navigate to the schemas section below to get a good glance at the models.  Favour `numberOfSomething` instead of `somethingCount` which is clearer. The older names are kept for backward-compatibility, but should be considered deprecated.  Gene aliases and multifunctionality rank are now filled in `GeneValueObject`.  Uniformly use `TaxonValueObject` to represent taxon. This is breaking change for the `ExpressionExperimentValueObject` and `ArrayDesignValueObject` as their `taxon` property will be an `object` instead of a `string`. Properties such as `taxonId` are now deprecated and `taxon.id` should be used instead.  Entities that have IDs now all inherit from `IdentifiableValueObject`. This implies that you can assume the presence of an `id` in a search result `resultObject` attribute for example.  New `/search` endpoint! for an unified search experience. Annotation-based search endpoints under `/annotations` are now deprecated.  New API docs! While not as nice looking, the previous theme will be gradually ported to Swagger UI as we focused on functionality over prettiness for this release.  ### Update 2.4.0 through 2.4.1  Release notes for the 2.4 series were not written down, so I'll try to do my best to recall features that were introduced at that time.  An [OpenAPI](https://www.openapis.org/) specification was introduced and available under `/rest/v2/openapi.json`, although not fully stabilized.  Add a `/resultSets` endpoint to navigate result sets directly, by ID or by dataset.  Add a `/resultSets/{resultSetId}` endpoint to retrieve a specific result set by its ID. This endpoint can be negotiated with an `Accept: text/tab-separated-values` header to obtain a TSV representation.  Add a `/datasets/{dataset}/analyses/differential/resultSets` endpoint that essentially redirect to a specific `/resultSet` endpoint by dataset ID.  Add an endpoint to retrieve preferred raw expression vectors.  ### Update 2.3.4  November 6th, 2018  November 6th [2.3.4] Bug fixes in the dataset search endpoint.  November 5th [2.3.3] Added filtering parameters to dataset search.  October 25th [2.3.2] Changed behavior of the dataset search endpoint to more closely match the Gemma web interface.  October 2nd [2.3.1] Added group information to the User value object.  September 27th [2.3.0] Breaking change in Taxa: Abbreviation property has been removed and is therefore no longer an accepted identifier.  ### Update 2.2.6  June 7th, 2018  Code maintenance, bug fixes. Geeq scores stable and made public.  June 7th [2.2.6] Added: User authentication endpoint.  May 2nd [2.2.5] Fixed: Cleaned up and optimized platforms/elements endpoint, removed redundant information (recursive properties nesting).  April 12th [2.2.3] Fixed: Array arguments not handling non-string properties properly, e.g. `ncbiIds` of genes.  April 9th [2.2.1] Fixed: Filter argument not working when the filtered field was a primitive type. This most significantly allows filtering by geeq boolean and double properties.  ### Update 2.2.0  February 8th, 2018  Breaking change in the 'Dataset differential analysis' endpoint: - No longer using `qValueThreshold` parameter. - Response format changed, now using `DifferentialExpressionAnalysisValueObject` instead of `DifferentialExpressionValueObject` - [Experimental] Added Geeq (Gene Expression Experiment Quality) scores to the dataset value objects   # noqa: E501
+    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  You can [consult the CHANGELOG.md file](https://gemma.msl.ubc.ca/resources/restapidocs/CHANGELOG.md) to view  release notes and recent changes to the Gemma RESTful API.   # noqa: E501
 
-    OpenAPI spec version: 2.5.1
+    OpenAPI spec version: 2.7.4
     Contact: pavlab-support@msl.ubc.ca
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `gemmapy-0.0.2/gemmapy/sdk/models/paginated_response_data_object_composite_sequence_value_object.py` & `gemmapy-1.0.0/gemmapy/sdk/models/paginated_response_data_object_composite_sequence_value_object.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Gemma RESTful API
 
-    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  Fix return type for `getResultSets` which was incorrectly referring to a renamed VO.  Remove the `security` requirements by default from the specification, which forced the Python package to supply empty credentials. There is currently no privileged endpoints, although some can return additional results.  ## Updates  ### Update 2.5.1  Restore `objectClass` visibility in `AnnotationValueObject`.  Fix incorrect response types for annotations search endpoints returning datasets.  ### Update 2.5.0  Major cleanups were performed in this release in order to stabilize the specification. Numerous properties from Gemma Web that were never intended to be exposed in Gemma REST have been hidden. It's a bit too much to describe in here, but you can navigate to the schemas section below to get a good glance at the models.  Favour `numberOfSomething` instead of `somethingCount` which is clearer. The older names are kept for backward-compatibility, but should be considered deprecated.  Gene aliases and multifunctionality rank are now filled in `GeneValueObject`.  Uniformly use `TaxonValueObject` to represent taxon. This is breaking change for the `ExpressionExperimentValueObject` and `ArrayDesignValueObject` as their `taxon` property will be an `object` instead of a `string`. Properties such as `taxonId` are now deprecated and `taxon.id` should be used instead.  Entities that have IDs now all inherit from `IdentifiableValueObject`. This implies that you can assume the presence of an `id` in a search result `resultObject` attribute for example.  New `/search` endpoint! for an unified search experience. Annotation-based search endpoints under `/annotations` are now deprecated.  New API docs! While not as nice looking, the previous theme will be gradually ported to Swagger UI as we focused on functionality over prettiness for this release.  ### Update 2.4.0 through 2.4.1  Release notes for the 2.4 series were not written down, so I'll try to do my best to recall features that were introduced at that time.  An [OpenAPI](https://www.openapis.org/) specification was introduced and available under `/rest/v2/openapi.json`, although not fully stabilized.  Add a `/resultSets` endpoint to navigate result sets directly, by ID or by dataset.  Add a `/resultSets/{resultSetId}` endpoint to retrieve a specific result set by its ID. This endpoint can be negotiated with an `Accept: text/tab-separated-values` header to obtain a TSV representation.  Add a `/datasets/{dataset}/analyses/differential/resultSets` endpoint that essentially redirect to a specific `/resultSet` endpoint by dataset ID.  Add an endpoint to retrieve preferred raw expression vectors.  ### Update 2.3.4  November 6th, 2018  November 6th [2.3.4] Bug fixes in the dataset search endpoint.  November 5th [2.3.3] Added filtering parameters to dataset search.  October 25th [2.3.2] Changed behavior of the dataset search endpoint to more closely match the Gemma web interface.  October 2nd [2.3.1] Added group information to the User value object.  September 27th [2.3.0] Breaking change in Taxa: Abbreviation property has been removed and is therefore no longer an accepted identifier.  ### Update 2.2.6  June 7th, 2018  Code maintenance, bug fixes. Geeq scores stable and made public.  June 7th [2.2.6] Added: User authentication endpoint.  May 2nd [2.2.5] Fixed: Cleaned up and optimized platforms/elements endpoint, removed redundant information (recursive properties nesting).  April 12th [2.2.3] Fixed: Array arguments not handling non-string properties properly, e.g. `ncbiIds` of genes.  April 9th [2.2.1] Fixed: Filter argument not working when the filtered field was a primitive type. This most significantly allows filtering by geeq boolean and double properties.  ### Update 2.2.0  February 8th, 2018  Breaking change in the 'Dataset differential analysis' endpoint: - No longer using `qValueThreshold` parameter. - Response format changed, now using `DifferentialExpressionAnalysisValueObject` instead of `DifferentialExpressionValueObject` - [Experimental] Added Geeq (Gene Expression Experiment Quality) scores to the dataset value objects   # noqa: E501
+    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  You can [consult the CHANGELOG.md file](https://gemma.msl.ubc.ca/resources/restapidocs/CHANGELOG.md) to view  release notes and recent changes to the Gemma RESTful API.   # noqa: E501
 
-    OpenAPI spec version: 2.5.1
+    OpenAPI spec version: 2.7.4
     Contact: pavlab-support@msl.ubc.ca
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -25,44 +25,49 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'data': 'list[CompositeSequenceValueObject]',
+        'group_by': 'list[str]',
+        'sort': 'SortValueObject',
         'offset': 'int',
         'limit': 'int',
-        'sort': 'SortValueObject',
         'total_elements': 'int'
     }
 
     attribute_map = {
         'data': 'data',
+        'group_by': 'groupBy',
+        'sort': 'sort',
         'offset': 'offset',
         'limit': 'limit',
-        'sort': 'sort',
         'total_elements': 'totalElements'
     }
 
-    def __init__(self, data=None, offset=None, limit=None, sort=None, total_elements=None):  # noqa: E501
+    def __init__(self, data=None, group_by=None, sort=None, offset=None, limit=None, total_elements=None):  # noqa: E501
         """PaginatedResponseDataObjectCompositeSequenceValueObject - a model defined in Swagger"""  # noqa: E501
         self._data = None
+        self._group_by = None
+        self._sort = None
         self._offset = None
         self._limit = None
-        self._sort = None
         self._total_elements = None
         self.discriminator = None
         if data is not None:
             self.data = data
+        if group_by is not None:
+            self.group_by = group_by
+        if sort is not None:
+            self.sort = sort
         if offset is not None:
             self.offset = offset
         if limit is not None:
             self.limit = limit
-        if sort is not None:
-            self.sort = sort
         if total_elements is not None:
             self.total_elements = total_elements
 
     @property
     def data(self):
         """Gets the data of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
 
@@ -80,14 +85,56 @@
         :param data: The data of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
         :type: list[CompositeSequenceValueObject]
         """
 
         self._data = data
 
     @property
+    def group_by(self):
+        """Gets the group_by of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
+
+
+        :return: The group_by of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._group_by
+
+    @group_by.setter
+    def group_by(self, group_by):
+        """Sets the group_by of this PaginatedResponseDataObjectCompositeSequenceValueObject.
+
+
+        :param group_by: The group_by of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
+        :type: list[str]
+        """
+
+        self._group_by = group_by
+
+    @property
+    def sort(self):
+        """Gets the sort of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
+
+
+        :return: The sort of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
+        :rtype: SortValueObject
+        """
+        return self._sort
+
+    @sort.setter
+    def sort(self, sort):
+        """Sets the sort of this PaginatedResponseDataObjectCompositeSequenceValueObject.
+
+
+        :param sort: The sort of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
+        :type: SortValueObject
+        """
+
+        self._sort = sort
+
+    @property
     def offset(self):
         """Gets the offset of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
 
 
         :return: The offset of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
         :rtype: int
         """
@@ -122,35 +169,14 @@
         :param limit: The limit of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
         :type: int
         """
 
         self._limit = limit
 
     @property
-    def sort(self):
-        """Gets the sort of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
-
-
-        :return: The sort of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
-        :rtype: SortValueObject
-        """
-        return self._sort
-
-    @sort.setter
-    def sort(self, sort):
-        """Sets the sort of this PaginatedResponseDataObjectCompositeSequenceValueObject.
-
-
-        :param sort: The sort of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
-        :type: SortValueObject
-        """
-
-        self._sort = sort
-
-    @property
     def total_elements(self):
         """Gets the total_elements of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
 
 
         :return: The total_elements of this PaginatedResponseDataObjectCompositeSequenceValueObject.  # noqa: E501
         :rtype: int
         """
```

### Comparing `gemmapy-0.0.2/gemmapy/sdk/models/paginated_response_data_object_differential_expression_analysis_result_set_value_object.py` & `gemmapy-1.0.0/gemmapy/sdk/models/filtered_and_paginated_response_data_object_differential_expression_analysis_result_set_value_object.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,171 +1,223 @@
 # coding: utf-8
 
 """
     Gemma RESTful API
 
-    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  Fix return type for `getResultSets` which was incorrectly referring to a renamed VO.  Remove the `security` requirements by default from the specification, which forced the Python package to supply empty credentials. There is currently no privileged endpoints, although some can return additional results.  ## Updates  ### Update 2.5.1  Restore `objectClass` visibility in `AnnotationValueObject`.  Fix incorrect response types for annotations search endpoints returning datasets.  ### Update 2.5.0  Major cleanups were performed in this release in order to stabilize the specification. Numerous properties from Gemma Web that were never intended to be exposed in Gemma REST have been hidden. It's a bit too much to describe in here, but you can navigate to the schemas section below to get a good glance at the models.  Favour `numberOfSomething` instead of `somethingCount` which is clearer. The older names are kept for backward-compatibility, but should be considered deprecated.  Gene aliases and multifunctionality rank are now filled in `GeneValueObject`.  Uniformly use `TaxonValueObject` to represent taxon. This is breaking change for the `ExpressionExperimentValueObject` and `ArrayDesignValueObject` as their `taxon` property will be an `object` instead of a `string`. Properties such as `taxonId` are now deprecated and `taxon.id` should be used instead.  Entities that have IDs now all inherit from `IdentifiableValueObject`. This implies that you can assume the presence of an `id` in a search result `resultObject` attribute for example.  New `/search` endpoint! for an unified search experience. Annotation-based search endpoints under `/annotations` are now deprecated.  New API docs! While not as nice looking, the previous theme will be gradually ported to Swagger UI as we focused on functionality over prettiness for this release.  ### Update 2.4.0 through 2.4.1  Release notes for the 2.4 series were not written down, so I'll try to do my best to recall features that were introduced at that time.  An [OpenAPI](https://www.openapis.org/) specification was introduced and available under `/rest/v2/openapi.json`, although not fully stabilized.  Add a `/resultSets` endpoint to navigate result sets directly, by ID or by dataset.  Add a `/resultSets/{resultSetId}` endpoint to retrieve a specific result set by its ID. This endpoint can be negotiated with an `Accept: text/tab-separated-values` header to obtain a TSV representation.  Add a `/datasets/{dataset}/analyses/differential/resultSets` endpoint that essentially redirect to a specific `/resultSet` endpoint by dataset ID.  Add an endpoint to retrieve preferred raw expression vectors.  ### Update 2.3.4  November 6th, 2018  November 6th [2.3.4] Bug fixes in the dataset search endpoint.  November 5th [2.3.3] Added filtering parameters to dataset search.  October 25th [2.3.2] Changed behavior of the dataset search endpoint to more closely match the Gemma web interface.  October 2nd [2.3.1] Added group information to the User value object.  September 27th [2.3.0] Breaking change in Taxa: Abbreviation property has been removed and is therefore no longer an accepted identifier.  ### Update 2.2.6  June 7th, 2018  Code maintenance, bug fixes. Geeq scores stable and made public.  June 7th [2.2.6] Added: User authentication endpoint.  May 2nd [2.2.5] Fixed: Cleaned up and optimized platforms/elements endpoint, removed redundant information (recursive properties nesting).  April 12th [2.2.3] Fixed: Array arguments not handling non-string properties properly, e.g. `ncbiIds` of genes.  April 9th [2.2.1] Fixed: Filter argument not working when the filtered field was a primitive type. This most significantly allows filtering by geeq boolean and double properties.  ### Update 2.2.0  February 8th, 2018  Breaking change in the 'Dataset differential analysis' endpoint: - No longer using `qValueThreshold` parameter. - Response format changed, now using `DifferentialExpressionAnalysisValueObject` instead of `DifferentialExpressionValueObject` - [Experimental] Added Geeq (Gene Expression Experiment Quality) scores to the dataset value objects   # noqa: E501
+    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  You can [consult the CHANGELOG.md file](https://gemma.msl.ubc.ca/resources/restapidocs/CHANGELOG.md) to view  release notes and recent changes to the Gemma RESTful API.   # noqa: E501
 
-    OpenAPI spec version: 2.5.1
+    OpenAPI spec version: 2.7.4
     Contact: pavlab-support@msl.ubc.ca
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject(object):
+class FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'data': 'list[DifferentialExpressionAnalysisResultSetValueObject]',
+        'filter': 'str',
+        'group_by': 'list[str]',
+        'sort': 'SortValueObject',
         'offset': 'int',
         'limit': 'int',
-        'sort': 'SortValueObject',
         'total_elements': 'int'
     }
 
     attribute_map = {
         'data': 'data',
+        'filter': 'filter',
+        'group_by': 'groupBy',
+        'sort': 'sort',
         'offset': 'offset',
         'limit': 'limit',
-        'sort': 'sort',
         'total_elements': 'totalElements'
     }
 
-    def __init__(self, data=None, offset=None, limit=None, sort=None, total_elements=None):  # noqa: E501
-        """PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, data=None, filter=None, group_by=None, sort=None, offset=None, limit=None, total_elements=None):  # noqa: E501
+        """FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject - a model defined in Swagger"""  # noqa: E501
         self._data = None
+        self._filter = None
+        self._group_by = None
+        self._sort = None
         self._offset = None
         self._limit = None
-        self._sort = None
         self._total_elements = None
         self.discriminator = None
         if data is not None:
             self.data = data
+        if filter is not None:
+            self.filter = filter
+        if group_by is not None:
+            self.group_by = group_by
+        if sort is not None:
+            self.sort = sort
         if offset is not None:
             self.offset = offset
         if limit is not None:
             self.limit = limit
-        if sort is not None:
-            self.sort = sort
         if total_elements is not None:
             self.total_elements = total_elements
 
     @property
     def data(self):
-        """Gets the data of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        """Gets the data of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
 
 
-        :return: The data of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :return: The data of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
         :rtype: list[DifferentialExpressionAnalysisResultSetValueObject]
         """
         return self._data
 
     @data.setter
     def data(self, data):
-        """Sets the data of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.
+        """Sets the data of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.
 
 
-        :param data: The data of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :param data: The data of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
         :type: list[DifferentialExpressionAnalysisResultSetValueObject]
         """
 
         self._data = data
 
     @property
-    def offset(self):
-        """Gets the offset of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+    def filter(self):
+        """Gets the filter of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
 
 
-        :return: The offset of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
-        :rtype: int
+        :return: The filter of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :rtype: str
         """
-        return self._offset
+        return self._filter
 
-    @offset.setter
-    def offset(self, offset):
-        """Sets the offset of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.
+    @filter.setter
+    def filter(self, filter):
+        """Sets the filter of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.
 
 
-        :param offset: The offset of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
-        :type: int
+        :param filter: The filter of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :type: str
         """
 
-        self._offset = offset
+        self._filter = filter
 
     @property
-    def limit(self):
-        """Gets the limit of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+    def group_by(self):
+        """Gets the group_by of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
 
 
-        :return: The limit of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
-        :rtype: int
+        :return: The group_by of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._limit
+        return self._group_by
 
-    @limit.setter
-    def limit(self, limit):
-        """Sets the limit of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.
+    @group_by.setter
+    def group_by(self, group_by):
+        """Sets the group_by of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.
 
 
-        :param limit: The limit of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
-        :type: int
+        :param group_by: The group_by of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :type: list[str]
         """
 
-        self._limit = limit
+        self._group_by = group_by
 
     @property
     def sort(self):
-        """Gets the sort of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        """Gets the sort of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
 
 
-        :return: The sort of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :return: The sort of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
         :rtype: SortValueObject
         """
         return self._sort
 
     @sort.setter
     def sort(self, sort):
-        """Sets the sort of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.
+        """Sets the sort of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.
 
 
-        :param sort: The sort of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :param sort: The sort of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
         :type: SortValueObject
         """
 
         self._sort = sort
 
     @property
+    def offset(self):
+        """Gets the offset of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+
+
+        :return: The offset of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :rtype: int
+        """
+        return self._offset
+
+    @offset.setter
+    def offset(self, offset):
+        """Sets the offset of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.
+
+
+        :param offset: The offset of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :type: int
+        """
+
+        self._offset = offset
+
+    @property
+    def limit(self):
+        """Gets the limit of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+
+
+        :return: The limit of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :rtype: int
+        """
+        return self._limit
+
+    @limit.setter
+    def limit(self, limit):
+        """Sets the limit of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.
+
+
+        :param limit: The limit of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :type: int
+        """
+
+        self._limit = limit
+
+    @property
     def total_elements(self):
-        """Gets the total_elements of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        """Gets the total_elements of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
 
 
-        :return: The total_elements of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :return: The total_elements of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
         :rtype: int
         """
         return self._total_elements
 
     @total_elements.setter
     def total_elements(self, total_elements):
-        """Sets the total_elements of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.
+        """Sets the total_elements of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.
 
 
-        :param total_elements: The total_elements of this PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
+        :param total_elements: The total_elements of this FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject.  # noqa: E501
         :type: int
         """
 
         self._total_elements = total_elements
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -184,15 +236,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject, dict):
+        if issubclass(FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -200,15 +252,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject):
+        if not isinstance(other, FilteredAndPaginatedResponseDataObjectDifferentialExpressionAnalysisResultSetValueObject):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `gemmapy-0.0.2/gemmapy/sdk/models/search_result_value_object.py` & `gemmapy-1.0.0/gemmapy/sdk/models/differential_expression_analysis_result_value_object.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,149 +1,253 @@
 # coding: utf-8
 
 """
     Gemma RESTful API
 
-    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  Fix return type for `getResultSets` which was incorrectly referring to a renamed VO.  Remove the `security` requirements by default from the specification, which forced the Python package to supply empty credentials. There is currently no privileged endpoints, although some can return additional results.  ## Updates  ### Update 2.5.1  Restore `objectClass` visibility in `AnnotationValueObject`.  Fix incorrect response types for annotations search endpoints returning datasets.  ### Update 2.5.0  Major cleanups were performed in this release in order to stabilize the specification. Numerous properties from Gemma Web that were never intended to be exposed in Gemma REST have been hidden. It's a bit too much to describe in here, but you can navigate to the schemas section below to get a good glance at the models.  Favour `numberOfSomething` instead of `somethingCount` which is clearer. The older names are kept for backward-compatibility, but should be considered deprecated.  Gene aliases and multifunctionality rank are now filled in `GeneValueObject`.  Uniformly use `TaxonValueObject` to represent taxon. This is breaking change for the `ExpressionExperimentValueObject` and `ArrayDesignValueObject` as their `taxon` property will be an `object` instead of a `string`. Properties such as `taxonId` are now deprecated and `taxon.id` should be used instead.  Entities that have IDs now all inherit from `IdentifiableValueObject`. This implies that you can assume the presence of an `id` in a search result `resultObject` attribute for example.  New `/search` endpoint! for an unified search experience. Annotation-based search endpoints under `/annotations` are now deprecated.  New API docs! While not as nice looking, the previous theme will be gradually ported to Swagger UI as we focused on functionality over prettiness for this release.  ### Update 2.4.0 through 2.4.1  Release notes for the 2.4 series were not written down, so I'll try to do my best to recall features that were introduced at that time.  An [OpenAPI](https://www.openapis.org/) specification was introduced and available under `/rest/v2/openapi.json`, although not fully stabilized.  Add a `/resultSets` endpoint to navigate result sets directly, by ID or by dataset.  Add a `/resultSets/{resultSetId}` endpoint to retrieve a specific result set by its ID. This endpoint can be negotiated with an `Accept: text/tab-separated-values` header to obtain a TSV representation.  Add a `/datasets/{dataset}/analyses/differential/resultSets` endpoint that essentially redirect to a specific `/resultSet` endpoint by dataset ID.  Add an endpoint to retrieve preferred raw expression vectors.  ### Update 2.3.4  November 6th, 2018  November 6th [2.3.4] Bug fixes in the dataset search endpoint.  November 5th [2.3.3] Added filtering parameters to dataset search.  October 25th [2.3.2] Changed behavior of the dataset search endpoint to more closely match the Gemma web interface.  October 2nd [2.3.1] Added group information to the User value object.  September 27th [2.3.0] Breaking change in Taxa: Abbreviation property has been removed and is therefore no longer an accepted identifier.  ### Update 2.2.6  June 7th, 2018  Code maintenance, bug fixes. Geeq scores stable and made public.  June 7th [2.2.6] Added: User authentication endpoint.  May 2nd [2.2.5] Fixed: Cleaned up and optimized platforms/elements endpoint, removed redundant information (recursive properties nesting).  April 12th [2.2.3] Fixed: Array arguments not handling non-string properties properly, e.g. `ncbiIds` of genes.  April 9th [2.2.1] Fixed: Filter argument not working when the filtered field was a primitive type. This most significantly allows filtering by geeq boolean and double properties.  ### Update 2.2.0  February 8th, 2018  Breaking change in the 'Dataset differential analysis' endpoint: - No longer using `qValueThreshold` parameter. - Response format changed, now using `DifferentialExpressionAnalysisValueObject` instead of `DifferentialExpressionValueObject` - [Experimental] Added Geeq (Gene Expression Experiment Quality) scores to the dataset value objects   # noqa: E501
+    This website documents the usage of the [Gemma RESTful API](https://gemma.msl.ubc.ca/rest/v2/). Here you can find example script usage of the API, as well as graphical interface for each endpoint, with description of its parameters and the endpoint URL.  Use of this webpage and the Gemma Web services, including the REST API, is subject to [these terms and conditions](https://pavlidislab.github.io/Gemma/terms.html). Please read these in full before continuing to use this webpage or any other part of the Gemma system.  You can [consult the CHANGELOG.md file](https://gemma.msl.ubc.ca/resources/restapidocs/CHANGELOG.md) to view  release notes and recent changes to the Gemma RESTful API.   # noqa: E501
 
-    OpenAPI spec version: 2.5.1
+    OpenAPI spec version: 2.7.4
     Contact: pavlab-support@msl.ubc.ca
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SearchResultValueObject(object):
+class DifferentialExpressionAnalysisResultValueObject(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'result_id': 'int',
-        'result_type': 'SearchResultType',
-        'score': 'float',
-        'result_object': 'IdentifiableValueObject'
+        'id': 'int',
+        'probe_id': 'int',
+        'probe_name': 'str',
+        'genes': 'list[GeneValueObject]',
+        'corrected_pvalue': 'float',
+        'rank': 'float',
+        'contrasts': 'list[ContrastResultValueObject]',
+        'pvalue': 'float'
     }
 
     attribute_map = {
-        'result_id': 'resultId',
-        'result_type': 'resultType',
-        'score': 'score',
-        'result_object': 'resultObject'
+        'id': 'id',
+        'probe_id': 'probeId',
+        'probe_name': 'probeName',
+        'genes': 'genes',
+        'corrected_pvalue': 'correctedPvalue',
+        'rank': 'rank',
+        'contrasts': 'contrasts',
+        'pvalue': 'pvalue'
     }
 
-    def __init__(self, result_id=None, result_type=None, score=None, result_object=None):  # noqa: E501
-        """SearchResultValueObject - a model defined in Swagger"""  # noqa: E501
-        self._result_id = None
-        self._result_type = None
-        self._score = None
-        self._result_object = None
+    def __init__(self, id=None, probe_id=None, probe_name=None, genes=None, corrected_pvalue=None, rank=None, contrasts=None, pvalue=None):  # noqa: E501
+        """DifferentialExpressionAnalysisResultValueObject - a model defined in Swagger"""  # noqa: E501
+        self._id = None
+        self._probe_id = None
+        self._probe_name = None
+        self._genes = None
+        self._corrected_pvalue = None
+        self._rank = None
+        self._contrasts = None
+        self._pvalue = None
         self.discriminator = None
-        if result_id is not None:
-            self.result_id = result_id
-        if result_type is not None:
-            self.result_type = result_type
-        if score is not None:
-            self.score = score
-        if result_object is not None:
-            self.result_object = result_object
+        if id is not None:
+            self.id = id
+        if probe_id is not None:
+            self.probe_id = probe_id
+        if probe_name is not None:
+            self.probe_name = probe_name
+        if genes is not None:
+            self.genes = genes
+        if corrected_pvalue is not None:
+            self.corrected_pvalue = corrected_pvalue
+        if rank is not None:
+            self.rank = rank
+        if contrasts is not None:
+            self.contrasts = contrasts
+        if pvalue is not None:
+            self.pvalue = pvalue
 
     @property
-    def result_id(self):
-        """Gets the result_id of this SearchResultValueObject.  # noqa: E501
+    def id(self):
+        """Gets the id of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
 
 
-        :return: The result_id of this SearchResultValueObject.  # noqa: E501
+        :return: The id of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
         :rtype: int
         """
-        return self._result_id
+        return self._id
 
-    @result_id.setter
-    def result_id(self, result_id):
-        """Sets the result_id of this SearchResultValueObject.
+    @id.setter
+    def id(self, id):
+        """Sets the id of this DifferentialExpressionAnalysisResultValueObject.
 
 
-        :param result_id: The result_id of this SearchResultValueObject.  # noqa: E501
+        :param id: The id of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
         :type: int
         """
 
-        self._result_id = result_id
+        self._id = id
 
     @property
-    def result_type(self):
-        """Gets the result_type of this SearchResultValueObject.  # noqa: E501
+    def probe_id(self):
+        """Gets the probe_id of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
 
 
-        :return: The result_type of this SearchResultValueObject.  # noqa: E501
-        :rtype: SearchResultType
+        :return: The probe_id of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+        :rtype: int
+        """
+        return self._probe_id
+
+    @probe_id.setter
+    def probe_id(self, probe_id):
+        """Sets the probe_id of this DifferentialExpressionAnalysisResultValueObject.
+
+
+        :param probe_id: The probe_id of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+        :type: int
+        """
+
+        self._probe_id = probe_id
+
+    @property
+    def probe_name(self):
+        """Gets the probe_name of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+
+
+        :return: The probe_name of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+        :rtype: str
+        """
+        return self._probe_name
+
+    @probe_name.setter
+    def probe_name(self, probe_name):
+        """Sets the probe_name of this DifferentialExpressionAnalysisResultValueObject.
+
+
+        :param probe_name: The probe_name of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+        :type: str
+        """
+
+        self._probe_name = probe_name
+
+    @property
+    def genes(self):
+        """Gets the genes of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+
+
+        :return: The genes of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+        :rtype: list[GeneValueObject]
+        """
+        return self._genes
+
+    @genes.setter
+    def genes(self, genes):
+        """Sets the genes of this DifferentialExpressionAnalysisResultValueObject.
+
+
+        :param genes: The genes of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+        :type: list[GeneValueObject]
+        """
+
+        self._genes = genes
+
+    @property
+    def corrected_pvalue(self):
+        """Gets the corrected_pvalue of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+
+
+        :return: The corrected_pvalue of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+        :rtype: float
         """
-        return self._result_type
+        return self._corrected_pvalue
 
-    @result_type.setter
-    def result_type(self, result_type):
-        """Sets the result_type of this SearchResultValueObject.
+    @corrected_pvalue.setter
+    def corrected_pvalue(self, corrected_pvalue):
+        """Sets the corrected_pvalue of this DifferentialExpressionAnalysisResultValueObject.
 
 
-        :param result_type: The result_type of this SearchResultValueObject.  # noqa: E501
-        :type: SearchResultType
+        :param corrected_pvalue: The corrected_pvalue of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+        :type: float
         """
 
-        self._result_type = result_type
+        self._corrected_pvalue = corrected_pvalue
 
     @property
-    def score(self):
-        """Gets the score of this SearchResultValueObject.  # noqa: E501
+    def rank(self):
+        """Gets the rank of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
 
 
-        :return: The score of this SearchResultValueObject.  # noqa: E501
+        :return: The rank of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
         :rtype: float
         """
-        return self._score
+        return self._rank
 
-    @score.setter
-    def score(self, score):
-        """Sets the score of this SearchResultValueObject.
+    @rank.setter
+    def rank(self, rank):
+        """Sets the rank of this DifferentialExpressionAnalysisResultValueObject.
 
 
-        :param score: The score of this SearchResultValueObject.  # noqa: E501
+        :param rank: The rank of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
         :type: float
         """
 
-        self._score = score
+        self._rank = rank
 
     @property
-    def result_object(self):
-        """Gets the result_object of this SearchResultValueObject.  # noqa: E501
+    def contrasts(self):
+        """Gets the contrasts of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
 
 
-        :return: The result_object of this SearchResultValueObject.  # noqa: E501
-        :rtype: IdentifiableValueObject
+        :return: The contrasts of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+        :rtype: list[ContrastResultValueObject]
         """
-        return self._result_object
+        return self._contrasts
 
-    @result_object.setter
-    def result_object(self, result_object):
-        """Sets the result_object of this SearchResultValueObject.
+    @contrasts.setter
+    def contrasts(self, contrasts):
+        """Sets the contrasts of this DifferentialExpressionAnalysisResultValueObject.
 
 
-        :param result_object: The result_object of this SearchResultValueObject.  # noqa: E501
-        :type: IdentifiableValueObject
+        :param contrasts: The contrasts of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+        :type: list[ContrastResultValueObject]
+        """
+
+        self._contrasts = contrasts
+
+    @property
+    def pvalue(self):
+        """Gets the pvalue of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+
+
+        :return: The pvalue of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+        :rtype: float
+        """
+        return self._pvalue
+
+    @pvalue.setter
+    def pvalue(self, pvalue):
+        """Sets the pvalue of this DifferentialExpressionAnalysisResultValueObject.
+
+
+        :param pvalue: The pvalue of this DifferentialExpressionAnalysisResultValueObject.  # noqa: E501
+        :type: float
         """
 
-        self._result_object = result_object
+        self._pvalue = pvalue
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -158,15 +262,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SearchResultValueObject, dict):
+        if issubclass(DifferentialExpressionAnalysisResultValueObject, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -174,15 +278,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SearchResultValueObject):
+        if not isinstance(other, DifferentialExpressionAnalysisResultValueObject):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `gemmapy-0.0.2/gemmapy.egg-info/PKG-INFO` & `gemmapy-1.0.0/gemmapy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 Metadata-Version: 2.1
 Name: gemmapy
-Version: 0.0.2
+Version: 1.0.0
 Summary: a Python Wrapper for the Gemma API
 Keywords: gemma,bioinformatics
+Requires-Python: >3.10
 License-File: LICENSE.md
+Requires-Dist: certifi>=14.05.14
+Requires-Dist: six>=1.10
+Requires-Dist: python_dateutil>=2.5.3
+Requires-Dist: setuptools>=21.0.0
+Requires-Dist: urllib3>=1.15.1
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: anndata
+Requires-Dist: typing
 
 gemmapy: a Python Wrapper for the Gemma API
 ===========================================
 
 This is a Python wrapper for `Gemma <https://gemma.msl.ubc.ca/>`_'s
 RESTful `API <https://gemma.msl.ubc.ca/resources/restapidocs/>`_. Gemma is a web
 site, database and a set of tools for the meta-analysis, re-use and
@@ -16,15 +26,15 @@
 public studies, referencing thousands of published papers.
 
 
 Installation instructions
 -------------------------
 .. This is a content of docs/install.rst. Update it whenever install.rst changes.
    
-The package requires Python3.6+. 
+The package requires Python3.10+. 
 
 #. Install it from a local copy
 
    .. code-block:: bash
 
       git clone git@github.com:PavlidisLab/gemmapy.git
       cd gemmapy
```

