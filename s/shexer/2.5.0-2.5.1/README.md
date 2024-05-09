# Comparing `tmp/shexer-2.5.0.tar.gz` & `tmp/shexer-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shexer-2.5.0.tar", last modified: Wed May  8 19:54:21 2024, max compression
+gzip compressed data, was "shexer-2.5.1.tar", last modified: Thu May  9 16:14:03 2024, max compression
```

## Comparing `shexer-2.5.0.tar` & `shexer-2.5.1.tar`

### file list

```diff
@@ -1,252 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.653262 shexer-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 19:54:17.000000 shexer-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28687 2024-05-08 19:54:21.653262 shexer-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27686 2024-05-08 19:54:17.000000 shexer-2.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 19:54:21.653262 shexer-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-08 19:54:17.000000 shexer-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.633262 shexer-2.5.0/shexer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.633262 shexer-2.5.0/shexer/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.633262 shexer-2.5.0/shexer/core/instances/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/abstract_instance_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.633262 shexer-2.5.0/shexer/core/instances/annotators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/annotators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/annotators/annotator_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/annotators/annotator_tracking_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/annotators/base_annotator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.637262 shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/instances_cap_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/instance_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.637262 shexer-2.5.0/shexer/core/instances/mappings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/mappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/mappings/shape_map_instance_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.637262 shexer-2.5.0/shexer/core/instances/mix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/mix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/mix/mixed_instance_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/instances/pconsts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.637262 shexer-2.5.0/shexer/core/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/profiling/class_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/profiling/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.637262 shexer-2.5.0/shexer/core/profiling/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/profiling/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/profiling/strategy/direct_features_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9630 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/profiling/strategy/include_reverse_features_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.637262 shexer-2.5.0/shexer/core/shexing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/shexing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/shexing/class_shexer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.637262 shexer-2.5.0/shexer/core/shexing/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/shexing/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16801 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/shexing/strategy/abstract_shexing_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/shexing/strategy/direct_shexing_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.637262 shexer-2.5.0/shexer/core/shexing/strategy/minimal_iri_strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.637262 shexer-2.5.0/shexer/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.637262 shexer-2.5.0/shexer/io/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/graph/yielder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/base_triples_yielder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16607 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/big_ttl_triples_yielder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/graph/yielder/filter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/multi_nt_triples_yielder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/multi_zip_triples_yielder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/multifile_base_triples_yielder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/nt_triples_yielder.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/rdflib_triple_yielder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/graph/yielder/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/json/json_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/line_reader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/line_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/line_reader/file_line_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/line_reader/gz_line_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/line_reader/raw_string_line_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/line_reader/zip_file_line_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/profile/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/profile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/profile/formater/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/profile/formater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/profile/formater/abstract_profile_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/shacl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shacl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/shacl/formater/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shacl/formater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shacl/formater/shacl_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/shape_map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shape_map/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/shape_map/label/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shape_map/label/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shape_map/label/shape_map_label_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/shape_map/node_selector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shape_map/node_selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shape_map/node_selector/node_selector_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shape_map/shape_map_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/shex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/shex/formater/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/shex_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.641262 shexer-2.5.0/shexer/io/shex/formater/statement_serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/statement_serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.645262 shexer-2.5.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.645262 shexer-2.5.0/shexer/io/sparql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/sparql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/sparql/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.645262 shexer-2.5.0/shexer/io/uml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/uml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/uml/uml_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/io/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.645262 shexer-2.5.0/shexer/model/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/IRI.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/Literal.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/Macro.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/bnode.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/const_elem_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/fixed_prop_choice_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.645262 shexer-2.5.0/shexer/model/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/graph/abstract_sgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/graph/endpoint_sgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/graph/rdflib_sgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/hierarchy_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/property.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/shape.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/shape_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/model/statement.py
--rw-r--r--   0 runner    (1001) docker     (127)    26225 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/shaper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.645262 shexer-2.5.0/shexer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.649262 shexer-2.5.0/shexer/utils/factories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/factories/class_profiler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/factories/class_shexer_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/factories/h_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    12134 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/factories/instance_tracker_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/factories/iri_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/factories/remote_graph_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/factories/shape_map_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/factories/shape_map_parser_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/factories/shape_serializer_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    20793 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/factories/triple_yielders_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/obj_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.649262 shexer-2.5.0/shexer/utils/structures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/structures/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/target_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.649262 shexer-2.5.0/shexer/utils/translators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/translators/list_of_classes_to_shape_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/triple_yielders.py
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-05-08 19:54:17.000000 shexer-2.5.0/shexer/utils/uri.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.653262 shexer-2.5.0/shexer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28687 2024-05-08 19:54:21.000000 shexer-2.5.0/shexer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-05-08 19:54:21.000000 shexer-2.5.0/shexer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 19:54:21.000000 shexer-2.5.0/shexer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 19:54:21.000000 shexer-2.5.0/shexer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 19:54:21.000000 shexer-2.5.0/shexer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.653262 shexer-2.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-08 19:54:17.000000 shexer-2.5.0/test/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-05-08 19:54:17.000000 shexer-2.5.0/test/t_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_all_classes_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_allow_opt_cardinality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_allow_redundant_or.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.653262 shexer-2.5.0/test/test_bugs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_bugs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_bugs/test_no_sharp_in_auto_shape_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11004 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_compression_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_decimals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_depth_for_building_subgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_detect_minimal_iri.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_disable_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_disable_endpoint_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_disable_exact_cardinality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_disable_or_statements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_discard_and_compliant.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_examples_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_file_target_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_graph_file_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_graph_list_of_file_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_infer_numeric_types_for_untyped_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_input_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_instances_cap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_instances_file_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_instances_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_instantiation_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_inverse_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_keep_less_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_list_of_url_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_namespaces_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_namespaces_to_ignore.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_raw_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_raw_shape_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_rdflib_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_remove_empty_sahpes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.653262 shexer-2.5.0/test/test_shacl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_shacl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_shacl/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_shacl/test_class_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_shacl/test_detect_minimal_iri.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_shacl/test_https.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_shacl/test_literal_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_shape_map_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_shape_map_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_shape_qualifiers_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_shapes_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_target_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_uml_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_url_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_url_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 19:54:17.000000 shexer-2.5.0/test/test_wikidata_annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:21.653262 shexer-2.5.0/ws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 19:54:17.000000 shexer-2.5.0/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19366 2024-05-08 19:54:17.000000 shexer-2.5.0/ws/shexer_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 19:54:17.000000 shexer-2.5.0/ws/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.667791 shexer-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-09 16:13:55.000000 shexer-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28705 2024-05-09 16:14:03.667791 shexer-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27704 2024-05-09 16:13:55.000000 shexer-2.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-09 16:14:03.667791 shexer-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-09 16:13:55.000000 shexer-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.643790 shexer-2.5.1/shexer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.643790 shexer-2.5.1/shexer/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.643790 shexer-2.5.1/shexer/core/instances/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/abstract_instance_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.643790 shexer-2.5.1/shexer/core/instances/annotators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/annotators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/annotators/annotator_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/annotators/annotator_tracking_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/annotators/base_annotator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.647791 shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/instances_cap_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/instance_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.647791 shexer-2.5.1/shexer/core/instances/mappings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/mappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/mappings/shape_map_instance_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.647791 shexer-2.5.1/shexer/core/instances/mix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/mix/mixed_instance_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/instances/pconsts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.647791 shexer-2.5.1/shexer/core/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12655 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/profiling/class_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/profiling/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.647791 shexer-2.5.1/shexer/core/profiling/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/profiling/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/profiling/strategy/direct_features_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9630 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/profiling/strategy/include_reverse_features_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.647791 shexer-2.5.1/shexer/core/shexing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/shexing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/shexing/class_shexer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.647791 shexer-2.5.1/shexer/core/shexing/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/shexing/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16801 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/shexing/strategy/abstract_shexing_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/shexing/strategy/direct_shexing_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.647791 shexer-2.5.1/shexer/core/shexing/strategy/minimal_iri_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/shexing/strategy/minimal_iri_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/shexing/strategy/minimal_iri_strategy/abstract_min_iri_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/core/shexing/strategy/minimal_iri_strategy/ignore_min_iri_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.647791 shexer-2.5.1/shexer/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.647791 shexer-2.5.1/shexer/io/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/graph/yielder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/base_triples_yielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16607 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/big_ttl_triples_yielder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/graph/yielder/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/multi_nt_triples_yielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/multi_zip_triples_yielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/multifile_base_triples_yielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/nt_triples_yielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/rdflib_triple_yielder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/graph/yielder/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/graph/yielder/tsv_nt_triples_yielder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/json/json_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/line_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/line_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/line_reader/file_line_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/line_reader/gz_line_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/line_reader/raw_string_line_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/line_reader/xz_line_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/line_reader/zip_file_line_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/profile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/profile/formater/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/profile/formater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/profile/formater/abstract_profile_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/shacl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shacl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/shacl/formater/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shacl/formater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shacl/formater/shacl_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/shape_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shape_map/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/shape_map/label/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shape_map/label/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shape_map/label/shape_map_label_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/shape_map/node_selector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shape_map/node_selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shape_map/node_selector/node_selector_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shape_map/shape_map_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/shex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/shex/formater/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/shex_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.651790 shexer-2.5.1/shexer/io/shex/formater/statement_serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/statement_serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.655790 shexer-2.5.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/abs_freq_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/base_frequency_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.655790 shexer-2.5.1/shexer/io/sparql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/sparql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/sparql/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.655790 shexer-2.5.1/shexer/io/uml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/uml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/uml/uml_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/io/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.655790 shexer-2.5.1/shexer/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/IRI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/Literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/Macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/bnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/const_elem_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/fixed_prop_choice_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.655790 shexer-2.5.1/shexer/model/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6049 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/graph/abstract_sgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/graph/endpoint_sgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/graph/rdflib_sgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/hierarchy_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/shape_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/model/statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26237 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/shaper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.655790 shexer-2.5.1/shexer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.659790 shexer-2.5.1/shexer/utils/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/factories/class_profiler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/factories/class_shexer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/factories/h_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12134 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/factories/instance_tracker_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/factories/iri_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/factories/remote_graph_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/factories/shape_map_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/factories/shape_map_parser_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/factories/shape_serializer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20793 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/factories/triple_yielders_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/obj_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/shapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.659790 shexer-2.5.1/shexer/utils/structures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/structures/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/target_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.659790 shexer-2.5.1/shexer/utils/translators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/translators/list_of_classes_to_shape_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/triple_yielders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-05-09 16:13:55.000000 shexer-2.5.1/shexer/utils/uri.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.663791 shexer-2.5.1/shexer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28705 2024-05-09 16:14:03.000000 shexer-2.5.1/shexer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-09 16:14:03.000000 shexer-2.5.1/shexer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 16:14:03.000000 shexer-2.5.1/shexer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-09 16:14:03.000000 shexer-2.5.1/shexer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-09 16:14:03.000000 shexer-2.5.1/shexer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.663791 shexer-2.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-09 16:13:55.000000 shexer-2.5.1/test/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-05-09 16:13:55.000000 shexer-2.5.1/test/t_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_all_classes_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_allow_opt_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_allow_redundant_or.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.663791 shexer-2.5.1/test/test_bugs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_bugs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_bugs/test_no_sharp_in_auto_shape_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14823 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_compression_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_decimals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_depth_for_building_subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_detect_minimal_iri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_disable_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_disable_endpoint_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_disable_exact_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_disable_or_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_discard_and_compliant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_examples_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_file_target_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_graph_file_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_graph_list_of_file_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_infer_numeric_types_for_untyped_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8509 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_input_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_instances_cap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_instances_file_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_instances_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_instantiation_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_inverse_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_keep_less_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_list_of_url_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_namespaces_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_namespaces_to_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_raw_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_raw_shape_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_rdflib_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_remove_empty_sahpes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.663791 shexer-2.5.1/test/test_shacl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_shacl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_shacl/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_shacl/test_class_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_shacl/test_detect_minimal_iri.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_shacl/test_https.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_shacl/test_literal_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_shape_map_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_shape_map_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_shape_qualifiers_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_shapes_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_target_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_uml_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_url_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_url_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-09 16:13:55.000000 shexer-2.5.1/test/test_wikidata_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 16:14:03.663791 shexer-2.5.1/ws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 16:13:55.000000 shexer-2.5.1/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19366 2024-05-09 16:13:55.000000 shexer-2.5.1/ws/shexer_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 16:13:55.000000 shexer-2.5.1/ws/wsgi.py
```

### Comparing `shexer-2.5.0/LICENSE` & `shexer-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/PKG-INFO` & `shexer-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.5.0
+Version: 2.5.1
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.5.0.tar.gz
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.5.1.tar.gz
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -214,15 +214,15 @@
 * instances_cap (default -1): when this param is set to a positive value, sheXer will only use a maximun of instance_cap instances to get extract each shape. This may cause some lost of information, but if the sample of instances used is representative enough, your results won't be that different but you'll save main memory and execution time. 
 * depth_for_building_subgraph (default 1): use this param just in case you are working against a SPARQL endpoint. This integer indicates the max distance from any seed node to consider in order to track a subgraph from the endpoint. Please, remind that a high depth can cause a massive number of queries and have a high performance cost. 
 * track_classes_for_entities_at_last_depth_level (default True): use this param just in case you are working against a SPARQL endpoint. If it set to True, it makes a step further to the distance to the seed nodes indicated in the param depth. However, it will just look for triples related to typing, not the whole neighborhood of the nodes in the last level of depth.
 * limit_remote_instances *DEPRECATED* (default -1). Use this param if you are working against an endpoint using the param target_classes. If it is set to a positive number, sheXer will just get limit_remote_instances instances for each class from the endpoint (by adding LIMIT at the end of the sparql query). This is useful when working with big sources with tons on instances, causing too many or too heavy SPARQL queries to retrieve  all the content. NOTE: This parameter only affects computation consuming SPARQL endpoints. On the other hand, the parameter instances_cap works for any case, including SPARQL endpoints. Due to retrocompatibility reasons, limit_remote_instances still works, but it will be removed in future sheXer releases.
 * disable_endpoint_cache (default False). By default, if sheXer is told to consume triples from an endpoint, it will make some SPARQL queries and store the results in a local graph. If this parameter is set to True, sheXer won't save that content locally. This will help to reduce main memory usage, but will decrease the performance, as sheXer will need to make more SPARQL queries to the endpoint.
 * namespaces_dict (default None): dictionary in which the keys are namespaces and the values are their expected prefixes in the outputs. 
 * input_format (default "NT"): the format of the graph which is going to be computed. The default value is const.NT. IMPORTANT: currently, sheXer does not guess input format, so ensure you specify the format here in case you are not providing n-triples content. In case you provide a combined input (several files, several URLs...) they all should have the same format. If you work against an endpoit, then this param do not have any effect.
-* compression_mode (default None). Only when you are working with local files, if they are compressed, you do not need to uncompress to parse them. Currently supported formats are ZIP and GZ. Set compression_format to "zip" or "gz" to work with such files. Each gz file will be assumed to contain a single graph file. Each zip file will be assumed to be a directory containing one or more graph files. In case the zip contains several files, they will be all parsed and merged (they should have the same format, indicated with input_format). In every case, sheXer won't write any uncompressed content to your disk.
+* compression_mode (default None). Only when you are working with local files, if they are compressed, you do not need to uncompress to parse them. Currently supported formats are ZIP, GZ, and XZ. Set compression_format to "zip", "gz", or "xz" to work with such files. Each gz or xz file will be assumed to contain a single graph file. Each zip file will be assumed to be a directory containing one or more graph files. In case the zip contains several files, they will be all parsed and merged (they should have the same format, indicated with input_format). In every case, sheXer won't write any uncompressed content to your disk.
 
 #### Params to tune the shexing process
 
 All this parameters have a default value so you do not need to use any of them. But you can modify the schema extraction in many different ways.
 
 * instantiation_property (default rdf:type): full URI (no prefixes) of the property linking instances and classes (ex: P31 in Wikidata's ontology)
 * namespaces_to_ignore (default None): list of namespaces of properties used in the target graph which are going to be ignored. For example, if you set namespaces_to_ignore to \[http://example.org/\], every triple whose predicate belongs to that namespace will not be computed. It just excludes properties whose name is a direct child of the namespace. For example, triples with <http:/example.org/foo> will be ignored, but triples with <http://example.org/anotherLevel/foo> will be computed.
```

### Comparing `shexer-2.5.0/README.md` & `shexer-2.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 * instances_cap (default -1): when this param is set to a positive value, sheXer will only use a maximun of instance_cap instances to get extract each shape. This may cause some lost of information, but if the sample of instances used is representative enough, your results won't be that different but you'll save main memory and execution time. 
 * depth_for_building_subgraph (default 1): use this param just in case you are working against a SPARQL endpoint. This integer indicates the max distance from any seed node to consider in order to track a subgraph from the endpoint. Please, remind that a high depth can cause a massive number of queries and have a high performance cost. 
 * track_classes_for_entities_at_last_depth_level (default True): use this param just in case you are working against a SPARQL endpoint. If it set to True, it makes a step further to the distance to the seed nodes indicated in the param depth. However, it will just look for triples related to typing, not the whole neighborhood of the nodes in the last level of depth.
 * limit_remote_instances *DEPRECATED* (default -1). Use this param if you are working against an endpoint using the param target_classes. If it is set to a positive number, sheXer will just get limit_remote_instances instances for each class from the endpoint (by adding LIMIT at the end of the sparql query). This is useful when working with big sources with tons on instances, causing too many or too heavy SPARQL queries to retrieve  all the content. NOTE: This parameter only affects computation consuming SPARQL endpoints. On the other hand, the parameter instances_cap works for any case, including SPARQL endpoints. Due to retrocompatibility reasons, limit_remote_instances still works, but it will be removed in future sheXer releases.
 * disable_endpoint_cache (default False). By default, if sheXer is told to consume triples from an endpoint, it will make some SPARQL queries and store the results in a local graph. If this parameter is set to True, sheXer won't save that content locally. This will help to reduce main memory usage, but will decrease the performance, as sheXer will need to make more SPARQL queries to the endpoint.
 * namespaces_dict (default None): dictionary in which the keys are namespaces and the values are their expected prefixes in the outputs. 
 * input_format (default "NT"): the format of the graph which is going to be computed. The default value is const.NT. IMPORTANT: currently, sheXer does not guess input format, so ensure you specify the format here in case you are not providing n-triples content. In case you provide a combined input (several files, several URLs...) they all should have the same format. If you work against an endpoit, then this param do not have any effect.
-* compression_mode (default None). Only when you are working with local files, if they are compressed, you do not need to uncompress to parse them. Currently supported formats are ZIP and GZ. Set compression_format to "zip" or "gz" to work with such files. Each gz file will be assumed to contain a single graph file. Each zip file will be assumed to be a directory containing one or more graph files. In case the zip contains several files, they will be all parsed and merged (they should have the same format, indicated with input_format). In every case, sheXer won't write any uncompressed content to your disk.
+* compression_mode (default None). Only when you are working with local files, if they are compressed, you do not need to uncompress to parse them. Currently supported formats are ZIP, GZ, and XZ. Set compression_format to "zip", "gz", or "xz" to work with such files. Each gz or xz file will be assumed to contain a single graph file. Each zip file will be assumed to be a directory containing one or more graph files. In case the zip contains several files, they will be all parsed and merged (they should have the same format, indicated with input_format). In every case, sheXer won't write any uncompressed content to your disk.
 
 #### Params to tune the shexing process
 
 All this parameters have a default value so you do not need to use any of them. But you can modify the schema extraction in many different ways.
 
 * instantiation_property (default rdf:type): full URI (no prefixes) of the property linking instances and classes (ex: P31 in Wikidata's ontology)
 * namespaces_to_ignore (default None): list of namespaces of properties used in the target graph which are going to be ignored. For example, if you set namespaces_to_ignore to \[http://example.org/\], every triple whose predicate belongs to that namespace will not be computed. It just excludes properties whose name is a direct child of the namespace. For example, triples with <http:/example.org/foo> will be ignored, but triples with <http://example.org/anotherLevel/foo> will be computed.
```

### Comparing `shexer-2.5.0/setup.py` & `shexer-2.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 def read(file_path):
 	with open(file_path, "r") as in_stream:
 		return in_stream.read()
 
 setup(
   name = 'shexer',
   packages = find_packages(exclude=["*.local_code.*"]), # this must be the same as the name above
-  version = '2.5.0',
+  version = '2.5.1',
   description = 'Automatic schema extraction for RDF graphs',
   author = 'Daniel Fernandez-Alvarez',
   author_email = 'danifdezalvarez@gmail.com',
   url = 'https://github.com/DaniFdezAlvarez/shexer',
-  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.5.0.tar.gz',
+  download_url = 'https://github.com/DaniFdezAlvarez/shexer/archive/2.5.1.tar.gz',
   keywords = ['testing', 'shexer', 'shexerp3', "rdf", "shex", "shacl", "schema"],
   long_description = read('README.md'),
   long_description_content_type='text/markdown',
   classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `shexer-2.5.0/shexer/consts.py` & `shexer-2.5.1/shexer/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 #NAMESPACES
 SHAPES_DEFAULT_NAMESPACE = "http://weso.es/shapes/"
 
 #COMPRESSION FORMATS
 ZIP = "zip"
 GZ = "gz"
+XZ = "xz"
 
 # FREQUENCY MODES
 
 RATIO_INSTANCES = "ratio"
 ABSOLUTE_INSTANCES = "abs"
 MIXED_INSTANCES = "mixed"
```

### Comparing `shexer-2.5.0/shexer/core/instances/abstract_instance_tracker.py` & `shexer-2.5.1/shexer/core/instances/abstract_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/instances/annotators/annotator_tracking_instances.py` & `shexer-2.5.1/shexer/core/instances/annotators/annotator_tracking_instances.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/instances/annotators/base_annotator.py` & `shexer-2.5.1/shexer/core/instances/annotators/base_annotator.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py` & `shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py` & `shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/base_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py` & `shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/compound_strategy_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py` & `shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/instance_cap_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py` & `shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py` & `shexer-2.5.1/shexer/core/instances/annotators/strategy_mode/target_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/instances/instance_tracker.py` & `shexer-2.5.1/shexer/core/instances/instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/instances/mappings/shape_map_instance_tracker.py` & `shexer-2.5.1/shexer/core/instances/mappings/shape_map_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/instances/mix/mixed_instance_tracker.py` & `shexer-2.5.1/shexer/core/instances/mix/mixed_instance_tracker.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/profiling/class_profiler.py` & `shexer-2.5.1/shexer/core/profiling/class_profiler.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py` & `shexer-2.5.1/shexer/core/profiling/strategy/abstract_feature_direction_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/profiling/strategy/direct_features_strategy.py` & `shexer-2.5.1/shexer/core/profiling/strategy/direct_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/profiling/strategy/include_reverse_features_strategy.py` & `shexer-2.5.1/shexer/core/profiling/strategy/include_reverse_features_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/shexing/class_shexer.py` & `shexer-2.5.1/shexer/core/shexing/class_shexer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/shexing/strategy/abstract_shexing_strategy.py` & `shexer-2.5.1/shexer/core/shexing/strategy/abstract_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py` & `shexer-2.5.1/shexer/core/shexing/strategy/direct_and_inverse_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/shexing/strategy/direct_shexing_strategy.py` & `shexer-2.5.1/shexer/core/shexing/strategy/direct_shexing_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py` & `shexer-2.5.1/shexer/core/shexing/strategy/minimal_iri_strategy/annotate_min_iri_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/base_triples_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/base_triples_yielder.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 from shexer.io.line_reader.file_line_reader import FileLineReader
 from shexer.io.line_reader.raw_string_line_reader import RawStringLineReader
 from shexer.io.line_reader.gz_line_reader import GzFileLineReader
 from shexer.io.line_reader.zip_file_line_reader import ZipFileLineReader
+from shexer.io.line_reader.xz_line_reader import XzFileLineReader
 from shexer.utils.obj_references import check_just_one_not_none
-from shexer.consts import ZIP, GZ
+from shexer.consts import ZIP, GZ, XZ
 
 class BaseTriplesYielder(object):
 
     def __init__(self):
         pass
 
     def _decide_line_reader(self, raw_graph, source_file,
@@ -21,12 +22,14 @@
         elif compression_mode is None:
             return FileLineReader(source_file=source_file)
         elif compression_mode == GZ:
             return GzFileLineReader(gz_file=source_file)
         elif compression_mode == ZIP:
             return ZipFileLineReader(zip_archive=zip_base_archive,
                                      zip_target=source_file)
+        elif compression_mode == XZ:
+            return XzFileLineReader(xz_file=source_file)
         else:
             raise ValueError("Unsupported compression mode: {}".format(compression_mode))
 
     def yield_triples(self):
         raise NotImplementedError("Implement this method in derived classes")
```

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/big_ttl_triples_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/big_ttl_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/filter/filter_namespaces_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/multi_big_ttl_files_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/multi_nt_triples_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/multi_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/multi_rdflib_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/multi_tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/multi_zip_triples_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/multi_zip_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/multifile_base_triples_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/multifile_base_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/nt_triples_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/rdflib_triple_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/rdflib_triple_yielder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from rdflib.graph import Graph, URIRef, Literal, BNode
 from shexer.io.graph.yielder.base_triples_yielder import BaseTriplesYielder
-from shexer.consts import N3, TURTLE, RDF_XML, NT, JSON_LD, ZIP, GZ
+from shexer.consts import N3, TURTLE, RDF_XML, NT, JSON_LD, ZIP, GZ, XZ
 
 from shexer.model.Literal import Literal as model_Literal
 from shexer.model.IRI import IRI as model_IRI
 from shexer.model.bnode import BNode as model_BNode
 from shexer.model.property import Property as model_Property
 
 from shexer.utils.uri import decide_literal_type
-from shexer.utils.compression import get_content_gz_file, get_content_zip_internal_file
+from shexer.utils.compression import get_content_gz_file, get_content_zip_internal_file, get_content_xz_file
 
 _SUPPORTED_FORMATS = [N3, TURTLE, RDF_XML, NT, JSON_LD]
 
 _XML_WRONG_URI = "http://www.w3.org/XML/1998/namespace"
 
 
 class RdflibTripleYielder(BaseTriplesYielder):
@@ -151,14 +151,16 @@
     def _parse_compressed_files(self, rdflib_graph):
         if self._compression_mode == GZ:
             rdflib_graph.parse(data=get_content_gz_file(self._source), format=self._input_format)
         elif self._compression_mode == ZIP:
             rdflib_graph.parse(data=get_content_zip_internal_file(base_archive=self._zip_archive_file,
                                                                   target_file=self._source),
                                format=self._input_format)
+        elif self._compression_mode == XZ:
+            rdflib_graph.parse(data=get_content_xz_file(self._source), format=self._input_format)
         else:
             raise ValueError("Unknown compression format")
 
     @staticmethod
     def _check_input_format(input_format):
         if input_format not in _SUPPORTED_FORMATS:
             raise ValueError("Unsupported input format: " + input_format)
```

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/graph/yielder/tsv_nt_triples_yielder.py` & `shexer-2.5.1/shexer/io/graph/yielder/tsv_nt_triples_yielder.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/shacl/formater/shacl_serializer.py` & `shexer-2.5.1/shexer/io/shacl/formater/shacl_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/shape_map/label/shape_map_label_parser.py` & `shexer-2.5.1/shexer/io/shape_map/label/shape_map_label_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/shape_map/node_selector/node_selector_parser.py` & `shexer-2.5.1/shexer/io/shape_map/node_selector/node_selector_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/shape_map/shape_map_parser.py` & `shexer-2.5.1/shexer/io/shape_map/shape_map_parser.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/shex/formater/shex_serializer.py` & `shexer-2.5.1/shexer/io/shex/formater/shex_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py` & `shexer-2.5.1/shexer/io/shex/formater/statement_serializers/base_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py` & `shexer-2.5.1/shexer/io/shex/formater/statement_serializers/fixed_prop_choice_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py` & `shexer-2.5.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/mixed_frequency_strategy.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py` & `shexer-2.5.1/shexer/io/shex/formater/statement_serializers/frequency_strategy/ratio_freq_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py` & `shexer-2.5.1/shexer/io/shex/formater/statement_serializers/inverse_statement_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py` & `shexer-2.5.1/shexer/io/shex/formater/statement_serializers/st_serializers_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/sparql/query.py` & `shexer-2.5.1/shexer/io/sparql/query.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/io/uml/uml_serializer.py` & `shexer-2.5.1/shexer/io/uml/uml_serializer.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/model/IRI.py` & `shexer-2.5.1/shexer/model/IRI.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/model/Macro.py` & `shexer-2.5.1/shexer/model/Macro.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/model/fixed_prop_choice_statement.py` & `shexer-2.5.1/shexer/model/fixed_prop_choice_statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/model/graph/abstract_sgraph.py` & `shexer-2.5.1/shexer/model/graph/abstract_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/model/graph/endpoint_sgraph.py` & `shexer-2.5.1/shexer/model/graph/endpoint_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/model/graph/rdflib_sgraph.py` & `shexer-2.5.1/shexer/model/graph/rdflib_sgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/model/hierarchy_tree.py` & `shexer-2.5.1/shexer/model/hierarchy_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/model/node_selector.py` & `shexer-2.5.1/shexer/model/node_selector.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/model/shape.py` & `shexer-2.5.1/shexer/model/shape.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/model/shape_map.py` & `shexer-2.5.1/shexer/model/shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/model/statement.py` & `shexer-2.5.1/shexer/model/statement.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/shaper.py` & `shexer-2.5.1/shexer/shaper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from shexer.utils.obj_references import check_just_one_not_none
 
 from shexer.consts import SHEXC, SHACL_TURTLE, NT, TSV_SPO, N3, TURTLE, TURTLE_ITER, \
-    RDF_XML, FIXED_SHAPE_MAP, JSON_LD, RDF_TYPE, SHAPES_DEFAULT_NAMESPACE, ZIP, GZ, \
+    RDF_XML, FIXED_SHAPE_MAP, JSON_LD, RDF_TYPE, SHAPES_DEFAULT_NAMESPACE, ZIP, GZ, XZ, \
     ALL_EXAMPLES, CONSTRAINT_EXAMPLES, SHAPE_EXAMPLES
 from shexer.utils.factories.class_profiler_factory import get_class_profiler
 from shexer.utils.factories.instance_tracker_factory import get_instance_tracker
 from shexer.utils.factories.class_shexer_factory import get_class_shexer
 from shexer.utils.factories.remote_graph_factory import get_remote_graph_if_needed
 from shexer.utils.factories.shape_map_factory import get_shape_map_if_needed
 from shexer.io.profile.formater.abstract_profile_serializer import AbstractProfileSerializer
@@ -426,19 +426,19 @@
     @staticmethod
     def _check_input_format(input_format):
         if input_format not in [NT, TSV_SPO, N3, TURTLE, RDF_XML, JSON_LD, TURTLE_ITER]:
             raise ValueError("Currently unsupported input format: " + input_format)
 
     @staticmethod
     def _check_compression_mode(compression_mode, url_endpoint, url_graph_input, list_of_url_input):
-        if compression_mode not in [ZIP, GZ, None]:
+        if compression_mode not in [ZIP, GZ, XZ, None]:
             raise ValueError("Unknownk compression mode: {}. "
                              "The currently supported compression formats are {}.".format(
                 compression_mode,
-                ", ".join([ZIP, GZ])))
+                ", ".join([ZIP, GZ, XZ])))
         if compression_mode is not None and (url_endpoint is not None or url_graph_input is not None or list_of_url_input is not None):
             raise ValueError("You've chosed some compression mode ({}) to work with remote sources."
                              "Currently, sheXer can only parse compressed local files".format(compression_mode))
 
 
     @staticmethod
     def _check_target_classes(target_classes, file_target_classes, all_classes_mode, shape_map_file, shape_map_raw):
```

### Comparing `shexer-2.5.0/shexer/utils/compression.py` & `shexer-2.5.1/shexer/utils/compression.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,19 @@
-import gzip
+from gzip import open as gzopen
 from zipfile import ZipFile
+from xz import open as xzopen
+
+
+def get_content_xz_file(xz_path):
+    with xzopen(xz_path, "r") as in_stream:
+        return in_stream.read()
+
 
 def get_content_gz_file(gz_path):
-    with gzip.open(gz_path, "r") as in_stream:
+    with gzopen(gz_path, "r") as in_stream:
         return in_stream.read()
 
 
 def yield_contents_zip_dir(zip_path):
     with ZipFile(zip_path, 'r') as zip:
         for a_file_path in zip.filelist:
             with zip.open(a_file_path) as in_file:
```

### Comparing `shexer-2.5.0/shexer/utils/factories/class_profiler_factory.py` & `shexer-2.5.1/shexer/utils/factories/class_profiler_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/factories/class_shexer_factory.py` & `shexer-2.5.1/shexer/utils/factories/class_shexer_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/factories/h_tree.py` & `shexer-2.5.1/shexer/utils/factories/h_tree.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/factories/instance_tracker_factory.py` & `shexer-2.5.1/shexer/utils/factories/instance_tracker_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/factories/shape_map_factory.py` & `shexer-2.5.1/shexer/utils/factories/shape_map_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/factories/shape_map_parser_factory.py` & `shexer-2.5.1/shexer/utils/factories/shape_map_parser_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/factories/shape_serializer_factory.py` & `shexer-2.5.1/shexer/utils/factories/shape_serializer_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/factories/triple_yielders_factory.py` & `shexer-2.5.1/shexer/utils/factories/triple_yielders_factory.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/namespaces.py` & `shexer-2.5.1/shexer/utils/namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/obj_references.py` & `shexer-2.5.1/shexer/utils/obj_references.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/shapes.py` & `shexer-2.5.1/shexer/utils/shapes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/structures/dicts.py` & `shexer-2.5.1/shexer/utils/structures/dicts.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/target_elements.py` & `shexer-2.5.1/shexer/utils/target_elements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/translators/list_of_classes_to_shape_map.py` & `shexer-2.5.1/shexer/utils/translators/list_of_classes_to_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/triple_yielders.py` & `shexer-2.5.1/shexer/utils/triple_yielders.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer/utils/uri.py` & `shexer-2.5.1/shexer/utils/uri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/shexer.egg-info/PKG-INFO` & `shexer-2.5.1/shexer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: shexer
-Version: 2.5.0
+Version: 2.5.1
 Summary: Automatic schema extraction for RDF graphs
 Home-page: https://github.com/DaniFdezAlvarez/shexer
-Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.5.0.tar.gz
+Download-URL: https://github.com/DaniFdezAlvarez/shexer/archive/2.5.1.tar.gz
 Author: Daniel Fernandez-Alvarez
 Author-email: danifdezalvarez@gmail.com
 Keywords: testing,shexer,shexerp3,rdf,shex,shacl,schema
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -214,15 +214,15 @@
 * instances_cap (default -1): when this param is set to a positive value, sheXer will only use a maximun of instance_cap instances to get extract each shape. This may cause some lost of information, but if the sample of instances used is representative enough, your results won't be that different but you'll save main memory and execution time. 
 * depth_for_building_subgraph (default 1): use this param just in case you are working against a SPARQL endpoint. This integer indicates the max distance from any seed node to consider in order to track a subgraph from the endpoint. Please, remind that a high depth can cause a massive number of queries and have a high performance cost. 
 * track_classes_for_entities_at_last_depth_level (default True): use this param just in case you are working against a SPARQL endpoint. If it set to True, it makes a step further to the distance to the seed nodes indicated in the param depth. However, it will just look for triples related to typing, not the whole neighborhood of the nodes in the last level of depth.
 * limit_remote_instances *DEPRECATED* (default -1). Use this param if you are working against an endpoint using the param target_classes. If it is set to a positive number, sheXer will just get limit_remote_instances instances for each class from the endpoint (by adding LIMIT at the end of the sparql query). This is useful when working with big sources with tons on instances, causing too many or too heavy SPARQL queries to retrieve  all the content. NOTE: This parameter only affects computation consuming SPARQL endpoints. On the other hand, the parameter instances_cap works for any case, including SPARQL endpoints. Due to retrocompatibility reasons, limit_remote_instances still works, but it will be removed in future sheXer releases.
 * disable_endpoint_cache (default False). By default, if sheXer is told to consume triples from an endpoint, it will make some SPARQL queries and store the results in a local graph. If this parameter is set to True, sheXer won't save that content locally. This will help to reduce main memory usage, but will decrease the performance, as sheXer will need to make more SPARQL queries to the endpoint.
 * namespaces_dict (default None): dictionary in which the keys are namespaces and the values are their expected prefixes in the outputs. 
 * input_format (default "NT"): the format of the graph which is going to be computed. The default value is const.NT. IMPORTANT: currently, sheXer does not guess input format, so ensure you specify the format here in case you are not providing n-triples content. In case you provide a combined input (several files, several URLs...) they all should have the same format. If you work against an endpoit, then this param do not have any effect.
-* compression_mode (default None). Only when you are working with local files, if they are compressed, you do not need to uncompress to parse them. Currently supported formats are ZIP and GZ. Set compression_format to "zip" or "gz" to work with such files. Each gz file will be assumed to contain a single graph file. Each zip file will be assumed to be a directory containing one or more graph files. In case the zip contains several files, they will be all parsed and merged (they should have the same format, indicated with input_format). In every case, sheXer won't write any uncompressed content to your disk.
+* compression_mode (default None). Only when you are working with local files, if they are compressed, you do not need to uncompress to parse them. Currently supported formats are ZIP, GZ, and XZ. Set compression_format to "zip", "gz", or "xz" to work with such files. Each gz or xz file will be assumed to contain a single graph file. Each zip file will be assumed to be a directory containing one or more graph files. In case the zip contains several files, they will be all parsed and merged (they should have the same format, indicated with input_format). In every case, sheXer won't write any uncompressed content to your disk.
 
 #### Params to tune the shexing process
 
 All this parameters have a default value so you do not need to use any of them. But you can modify the schema extraction in many different ways.
 
 * instantiation_property (default rdf:type): full URI (no prefixes) of the property linking instances and classes (ex: P31 in Wikidata's ontology)
 * namespaces_to_ignore (default None): list of namespaces of properties used in the target graph which are going to be ignored. For example, if you set namespaces_to_ignore to \[http://example.org/\], every triple whose predicate belongs to that namespace will not be computed. It just excludes properties whose name is a direct child of the namespace. For example, triples with <http:/example.org/foo> will be ignored, but triples with <http://example.org/anotherLevel/foo> will be computed.
```

### Comparing `shexer-2.5.0/shexer.egg-info/SOURCES.txt` & `shexer-2.5.1/shexer.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 shexer/io/graph/yielder/remote/sgraph_from_selectors_triple_yielder.py
 shexer/io/json/__init__.py
 shexer/io/json/json_loader.py
 shexer/io/line_reader/__init__.py
 shexer/io/line_reader/file_line_reader.py
 shexer/io/line_reader/gz_line_reader.py
 shexer/io/line_reader/raw_string_line_reader.py
+shexer/io/line_reader/xz_line_reader.py
 shexer/io/line_reader/zip_file_line_reader.py
 shexer/io/profile/__init__.py
 shexer/io/profile/formater/__init__.py
 shexer/io/profile/formater/abstract_profile_serializer.py
 shexer/io/shacl/__init__.py
 shexer/io/shacl/formater/__init__.py
 shexer/io/shacl/formater/shacl_serializer.py
```

### Comparing `shexer-2.5.0/test/const.py` & `shexer-2.5.1/test/const.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/t_utils.py` & `shexer-2.5.1/test/t_utils.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_all_classes_mode.py` & `shexer-2.5.1/test/test_all_classes_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_allow_opt_cardinality.py` & `shexer-2.5.1/test/test_allow_opt_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_allow_redundant_or.py` & `shexer-2.5.1/test/test_allow_redundant_or.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_bugs/test_no_sharp_in_auto_shape_names.py` & `shexer-2.5.1/test/test_bugs/test_no_sharp_in_auto_shape_names.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py` & `shexer-2.5.1/test/test_bugs/test_no_sharp_nor_slash_due_to_prefixing.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_compression_mode.py` & `shexer-2.5.1/test/test_compression_mode.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 from shexer.shaper import Shaper
 from test.const import G1, BASE_FILES, default_namespaces, G1_ALL_CLASSES_NO_COMMENTS
 from test.t_utils import file_vs_str_tunned_comparison
 import os.path as pth
 
-from shexer.consts import TURTLE_ITER, GZ, ZIP, N3, TURTLE, RDF_XML, TSV_SPO, NT, JSON_LD
+from shexer.consts import TURTLE_ITER, GZ, ZIP, XZ, N3, TURTLE, RDF_XML, TSV_SPO, NT, JSON_LD
 
 
 
 _BASE_DIR = BASE_FILES + "compression" + pth.sep
 
 
 class TestCompressionMode(unittest.TestCase):
@@ -195,14 +195,108 @@
             disable_comments=True,
             compression_mode=ZIP
         )
         str_result = shaper.shex_graph(string_output=True)
         self.assertTrue(file_vs_str_tunned_comparison(file_path=G1_ALL_CLASSES_NO_COMMENTS,
                                                       str_target=str_result))
 
+
+    ########################  xz
+
+    def test_ttl_iter_xz(self):
+        shaper = Shaper(
+            graph_file_input=_BASE_DIR + "t_graph_1.ttl.xz",
+            namespaces_dict=default_namespaces(),
+            all_classes_mode=True,
+            input_format=TURTLE_ITER,
+            disable_comments=True,
+            compression_mode=XZ
+        )
+        str_result = shaper.shex_graph(string_output=True)
+        self.assertTrue(file_vs_str_tunned_comparison(file_path=G1_ALL_CLASSES_NO_COMMENTS,
+                                                      str_target=str_result))
+
+    def test_n3_xz(self):
+        shaper = Shaper(
+            graph_file_input=_BASE_DIR + "t_graph_1.n3.xz",
+            namespaces_dict=default_namespaces(),
+            all_classes_mode=True,
+            input_format=N3,
+            disable_comments=True,
+            compression_mode=XZ
+        )
+        str_result = shaper.shex_graph(string_output=True)
+        self.assertTrue(file_vs_str_tunned_comparison(file_path=G1_ALL_CLASSES_NO_COMMENTS,
+                                                      str_target=str_result))
+
+    def test_json_xz(self):
+        shaper = Shaper(
+            graph_file_input=_BASE_DIR + "t_graph_1.json.xz",
+            namespaces_dict=default_namespaces(),
+            all_classes_mode=True,
+            input_format=JSON_LD,
+            disable_comments=True,
+            compression_mode=XZ
+        )
+        str_result = shaper.shex_graph(string_output=True)
+        self.assertTrue(file_vs_str_tunned_comparison(file_path=G1_ALL_CLASSES_NO_COMMENTS,
+                                                      str_target=str_result))
+
+    def test_ttl_rdflib_xz(self):
+        shaper = Shaper(
+            graph_file_input=_BASE_DIR + "t_graph_1.ttl.xz",
+            namespaces_dict=default_namespaces(),
+            all_classes_mode=True,
+            input_format=TURTLE,
+            disable_comments=True,
+            compression_mode=XZ
+        )
+        str_result = shaper.shex_graph(string_output=True)
+        self.assertTrue(file_vs_str_tunned_comparison(file_path=G1_ALL_CLASSES_NO_COMMENTS,
+                                                      str_target=str_result))
+
+    def test_xml_xz(self):
+        shaper = Shaper(
+            graph_file_input=_BASE_DIR + "t_graph_1.xml.xz",
+            namespaces_dict=default_namespaces(),
+            all_classes_mode=True,
+            input_format=RDF_XML,
+            disable_comments=True,
+            compression_mode=XZ
+        )
+        str_result = shaper.shex_graph(string_output=True)
+        self.assertTrue(file_vs_str_tunned_comparison(file_path=G1_ALL_CLASSES_NO_COMMENTS,
+                                                      str_target=str_result))
+
+    def test_tsv_spo_xz(self):
+        shaper = Shaper(
+            graph_file_input=_BASE_DIR + "t_graph_1.tsv.xz",
+            namespaces_dict=default_namespaces(),
+            all_classes_mode=True,
+            input_format=TSV_SPO,
+            disable_comments=True,
+            compression_mode=XZ
+        )
+        str_result = shaper.shex_graph(string_output=True)
+        self.assertTrue(file_vs_str_tunned_comparison(file_path=G1_ALL_CLASSES_NO_COMMENTS,
+                                                      str_target=str_result))
+
+    def test_nt_xz(self):
+        shaper = Shaper(
+            graph_file_input=_BASE_DIR + "t_graph_1.nt.xz",
+            namespaces_dict=default_namespaces(),
+            all_classes_mode=True,
+            input_format=NT,
+            disable_comments=True,
+            compression_mode=XZ
+        )
+        str_result = shaper.shex_graph(string_output=True)
+        self.assertTrue(file_vs_str_tunned_comparison(file_path=G1_ALL_CLASSES_NO_COMMENTS,
+                                                      str_target=str_result))
+
     ########################  Wrong params
 
     def test_unknown_mode(self):
         try:
             shaper = Shaper(
                 graph_file_input=_BASE_DIR + "t_graph_1.json.zip",
                 namespaces_dict=default_namespaces(),
```

### Comparing `shexer-2.5.0/test/test_decimals.py` & `shexer-2.5.1/test/test_decimals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_depth_for_building_subgraph.py` & `shexer-2.5.1/test/test_depth_for_building_subgraph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_detect_minimal_iri.py` & `shexer-2.5.1/test/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_disable_comments.py` & `shexer-2.5.1/test/test_disable_comments.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_disable_endpoint_cache.py` & `shexer-2.5.1/test/test_disable_endpoint_cache.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_disable_exact_cardinality.py` & `shexer-2.5.1/test/test_disable_exact_cardinality.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_disable_or_statements.py` & `shexer-2.5.1/test/test_disable_or_statements.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_discard_and_compliant.py` & `shexer-2.5.1/test/test_discard_and_compliant.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_examples_mode.py` & `shexer-2.5.1/test/test_examples_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_file_target_classes.py` & `shexer-2.5.1/test/test_file_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_graph_file_input.py` & `shexer-2.5.1/test/test_graph_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_graph_list_of_file_inputs.py` & `shexer-2.5.1/test/test_graph_list_of_file_inputs.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_infer_numeric_types_for_untyped_literals.py` & `shexer-2.5.1/test/test_infer_numeric_types_for_untyped_literals.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_input_format.py` & `shexer-2.5.1/test/test_input_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_instances_cap.py` & `shexer-2.5.1/test/test_instances_cap.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_instances_file_input.py` & `shexer-2.5.1/test/test_instances_file_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_instances_report.py` & `shexer-2.5.1/test/test_instances_report.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_instantiation_property.py` & `shexer-2.5.1/test/test_instantiation_property.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_inverse_paths.py` & `shexer-2.5.1/test/test_inverse_paths.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_keep_less_specific.py` & `shexer-2.5.1/test/test_keep_less_specific.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_list_of_url_input.py` & `shexer-2.5.1/test/test_list_of_url_input.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_namespaces_dict.py` & `shexer-2.5.1/test/test_namespaces_dict.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_namespaces_to_ignore.py` & `shexer-2.5.1/test/test_namespaces_to_ignore.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_raw_graph.py` & `shexer-2.5.1/test/test_raw_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_raw_shape_map.py` & `shexer-2.5.1/test/test_raw_shape_map.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_rdflib_graph.py` & `shexer-2.5.1/test/test_rdflib_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_remove_empty_sahpes.py` & `shexer-2.5.1/test/test_remove_empty_sahpes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_shacl/test_annotation.py` & `shexer-2.5.1/test/test_shacl/test_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_shacl/test_class_selection.py` & `shexer-2.5.1/test/test_shacl/test_class_selection.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_shacl/test_detect_minimal_iri.py` & `shexer-2.5.1/test/test_shacl/test_detect_minimal_iri.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_shacl/test_https.py` & `shexer-2.5.1/test/test_shacl/test_https.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_shacl/test_literal_types.py` & `shexer-2.5.1/test/test_shacl/test_literal_types.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_shape_map_file.py` & `shexer-2.5.1/test/test_shape_map_file.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_shape_map_format.py` & `shexer-2.5.1/test/test_shape_map_format.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_shape_qualifiers_mode.py` & `shexer-2.5.1/test/test_shape_qualifiers_mode.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_shapes_namespaces.py` & `shexer-2.5.1/test/test_shapes_namespaces.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_sort.py` & `shexer-2.5.1/test/test_sort.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_target_classes.py` & `shexer-2.5.1/test/test_target_classes.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_threshold.py` & `shexer-2.5.1/test/test_threshold.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_uml_gen.py` & `shexer-2.5.1/test/test_uml_gen.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_url_endpoint.py` & `shexer-2.5.1/test/test_url_endpoint.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_url_graph.py` & `shexer-2.5.1/test/test_url_graph.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/test/test_wikidata_annotation.py` & `shexer-2.5.1/test/test_wikidata_annotation.py`

 * *Files identical despite different names*

### Comparing `shexer-2.5.0/ws/shexer_rest.py` & `shexer-2.5.1/ws/shexer_rest.py`

 * *Files identical despite different names*

