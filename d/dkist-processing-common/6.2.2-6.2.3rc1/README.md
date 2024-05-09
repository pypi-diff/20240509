# Comparing `tmp/dkist-processing-common-6.2.2.tar.gz` & `tmp/dkist-processing-common-6.2.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-6.2.2.tar", last modified: Wed May  8 01:30:03 2024, max compression
+gzip compressed data, was "dkist-processing-common-6.2.3rc1.tar", last modified: Thu May  9 16:15:12 2024, max compression
```

## Comparing `dkist-processing-common-6.2.2.tar` & `dkist-processing-common-6.2.3rc1.tar`

### file list

```diff
@@ -1,136 +1,139 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.391739 dkist-processing-common-6.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    25369 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4391 2024-05-08 01:30:03.391739 dkist-processing-common-6.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3730 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3271 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.379739 dkist-processing-common-6.2.2/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.379739 dkist-processing-common-6.2.2/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.383739 dkist-processing-common-6.2.2/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3244 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     3426 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)    10378 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     6226 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.383739 dkist-processing-common-6.2.2/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/codecs/asdf.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2331 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)     3090 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/codecs/quality.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.383739 dkist-processing-common-6.2.2/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.383739 dkist-processing-common-6.2.2/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5409 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4113 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3681 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     6532 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)    11949 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/models/task_name.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.387739 dkist-processing-common-6.2.2/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6461 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2595 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     3938 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     7839 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     3041 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/unique_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.387739 dkist-processing-common-6.2.2/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12507 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    13198 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     9891 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.387739 dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6598 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2077 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    14466 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3242 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.387739 dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8094 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47664 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7986 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8917 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     5215 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8266 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/trial_catalog.py
--rw-rw-rw-   0 root         (0) root         (0)     9483 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    19478 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.391739 dkist-processing-common-6.2.2/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27198 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4165 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    16866 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_assemble_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)    20569 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     5903 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)    10946 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     3151 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3120 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8346 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10629 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9156 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36296 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16481 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)    24306 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_stems.py
--rw-rw-rw-   0 root         (0) root         (0)     3778 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_submit_dataset_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_task_name.py
--rw-rw-rw-   0 root         (0) root         (0)     4027 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_task_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     5494 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6658 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6814 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_trial_catalog.py
--rw-rw-rw-   0 root         (0) root         (0)    20114 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10488 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    17411 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.379739 dkist-processing-common-6.2.2/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4391 2024-05-08 01:30:03.000000 dkist-processing-common-6.2.2/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5094 2024-05-08 01:30:03.000000 dkist-processing-common-6.2.2/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-08 01:30:03.000000 dkist-processing-common-6.2.2/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-08 01:30:03.000000 dkist-processing-common-6.2.2/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-08 01:30:03.000000 dkist-processing-common-6.2.2/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.391739 dkist-processing-common-6.2.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 01:30:03.391739 dkist-processing-common-6.2.2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1887 2024-05-08 01:30:03.391739 dkist-processing-common-6.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-08 01:29:56.000000 dkist-processing-common-6.2.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.470883 dkist-processing-common-6.2.3rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    25646 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4394 2024-05-09 16:15:12.470883 dkist-processing-common-6.2.3rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3730 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3271 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.454883 dkist-processing-common-6.2.3rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/changelog/189.misc.rst
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/changelog/190.bugfix.rst
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/changelog/191.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.454883 dkist-processing-common-6.2.3rc1/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.458883 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3244 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     3426 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)    10378 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6226 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.458883 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/asdf.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2331 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)     3090 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.458883 dkist-processing-common-6.2.3rc1/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.462883 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5409 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4113 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3681 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     6532 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    11949 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/task_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.462883 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6461 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     3938 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     7839 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     3041 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/unique_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.462883 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12776 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    13198 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     9891 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.466884 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6598 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2077 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    14466 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3242 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.466884 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8130 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47664 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3699 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7986 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8917 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     5215 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8266 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/trial_catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)     9483 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    19802 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.470883 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27198 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4165 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    16866 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_assemble_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    20569 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5903 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)    10946 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3120 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8346 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10629 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9156 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36887 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16481 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)    24306 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_stems.py
+-rw-rw-rw-   0 root         (0) root         (0)     3778 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_submit_dataset_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_task_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     4027 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_task_parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     5494 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6658 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6814 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_trial_catalog.py
+-rw-rw-rw-   0 root         (0) root         (0)    20114 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10488 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    17411 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.454883 dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4394 2024-05-09 16:15:12.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5168 2024-05-09 16:15:12.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-09 16:15:12.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-09 16:15:12.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-09 16:15:12.000000 dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.470883 dkist-processing-common-6.2.3rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 16:15:12.470883 dkist-processing-common-6.2.3rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1887 2024-05-09 16:15:12.470883 dkist-processing-common-6.2.3rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-09 16:15:06.000000 dkist-processing-common-6.2.3rc1/setup.py
```

### Comparing `dkist-processing-common-6.2.2/.gitignore` & `dkist-processing-common-6.2.3rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/.pre-commit-config.yaml` & `dkist-processing-common-6.2.3rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/CHANGELOG.rst` & `dkist-processing-common-6.2.3rc1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 Features
 --------
 
 - Add the ability to create a quality report from a trial workflow. (`#185 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/185>`__)
 
 
+Bugfixes
+--------
+
+- `QualityL0Metrics.calculate_l0_metrics` now correctly identifies the TASK type. Previously it could have erroneously used the WORKFLOWTASK tag to find the IP TASK TYPE. (`#185 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/185>`__)
+
+
 v6.2.1 (2024-05-01)
 ===================
 
 Misc
 ----
 
 - Change filenames of browse movie and quality report to free up namespace for other future files. (`#124 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/124>`__)
```

### Comparing `dkist-processing-common-6.2.2/PKG-INFO` & `dkist-processing-common-6.2.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 6.2.2
+Version: 6.2.3rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-6.2.2/README.rst` & `dkist-processing-common-6.2.3rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/bitbucket-pipelines.yml` & `dkist-processing-common-6.2.3rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/check_changelog_updated.sh` & `dkist-processing-common-6.2.3rc1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/_util/config.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/_util/constants.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/_util/tags.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/codecs/asdf.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/asdf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/codecs/json.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/codecs/quality.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/codecs/str.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/manual.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/models/constants.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/models/graphql.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/models/message.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/models/parameters.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/models/quality.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/models/tags.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/models/task_name.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/task_name.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/task.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/time.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/parsers/wavelength.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/__init__.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/assemble_movie.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
                 Useful for writing a line of text in `write_overlay`. ``line = 0`` is the bottom of the frame.
 
     """
 
     MOVIE_FRAME_SHAPE = (2048, 1536)  # Is this a/THE standard size?
     IMAGES_PER_SEC = 3
     MINIMUM_DURATION = 10  # seconds
+    MAXIMUM_DURATION = 60  # seconds
     FPS = 15
     FONT_FILE = pkg_resources.resource_filename("dkist_processing_common", "fonts/Lato-Regular.ttf")
     TEXT_MARGIN_PX = 5
     MPL_COLOR_MAP = "viridis"
 
     @property
     def fits_parsing_class(self):
@@ -122,14 +123,18 @@
         self.font_36 = ImageFont.truetype(self.FONT_FILE, size=36)
 
         # If movie length would be less than minimum_duration, extend its length to minimum_duration
         if (self.num_images / self.IMAGES_PER_SEC) < self.MINIMUM_DURATION:
             self.IMAGES_PER_SEC = self.num_images / self.MINIMUM_DURATION
             self.FPS = round(self.num_images / self.MINIMUM_DURATION) or 1
 
+        # IF movie length would be more than maximum duration, stride the frames
+        if (self.num_images / self.IMAGES_PER_SEC) > self.MAXIMUM_DURATION:
+            self.IMAGES_PER_SEC = self.num_images / self.MAXIMUM_DURATION
+
         self.duration = self.num_images / self.IMAGES_PER_SEC
 
         ## This is here to fix a floating point bug in moviepy
         #
         # The following line is what moviepy uses to iterate over the number of frames. It can be larger than we want
         # (duration * fps) due to floating point errors
         iter_nframes = np.arange(0, self.duration, 1.0 / self.FPS).size
```

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/base.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,20 +129,20 @@
 
             square_2 = data[-corner_square_length:, 0:corner_square_height]  # top right
 
             square_3 = data[0:corner_square_length, -corner_square_height:]  # bottom left
 
             square_4 = data[-corner_square_length:, -corner_square_height:]  # bottom right
 
-            return np.average(
+            return np.nanmean(
                 [
-                    np.std(square_1),
-                    np.std(square_2),
-                    np.std(square_3),
-                    np.std(square_4),
+                    np.nanstd(square_1),
+                    np.nanstd(square_2),
+                    np.nanstd(square_3),
+                    np.nanstd(square_4),
                 ]
             )
 
         if len(data.shape) == 3:  # 3D data
             corner_cube_length = int(data.shape[0] * 0.2)  # 1/5th of x dimension of array
             corner_cube_height = int(data.shape[1] * 0.2)  # 1/5th of y dimension of array
             corner_cube_width = int(data.shape[2] * 0.2)  # 1/5th of z dimension of array
@@ -175,19 +175,19 @@
                 -corner_cube_length:, -corner_cube_height:, 0:corner_cube_width
             ]  # bottom right front
 
             cube_8 = data[
                 -corner_cube_length:, -corner_cube_height:, -corner_cube_width:
             ]  # bottom right back
 
-            return np.average(
+            return np.nanmean(
                 [
-                    np.std(cube_1),
-                    np.std(cube_2),
-                    np.std(cube_3),
-                    np.std(cube_4),
-                    np.std(cube_5),
-                    np.std(cube_6),
-                    np.std(cube_7),
-                    np.std(cube_8),
+                    np.nanstd(cube_1),
+                    np.nanstd(cube_2),
+                    np.nanstd(cube_3),
+                    np.nanstd(cube_4),
+                    np.nanstd(cube_5),
+                    np.nanstd(cube_6),
+                    np.nanstd(cube_7),
+                    np.nanstd(cube_8),
                 ]
             )
```

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/trial_catalog.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/trial_catalog.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tasks/write_l1.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,20 +64,25 @@
                 l1_header = self.convert_l0_to_l1(
                     header=calibrated_fits_object.header,
                     data=calibrated_fits_object.data,
                     hdu_size=calibrated_fits_object.size,
                     stokes_param=stokes_param,
                 )
 
+                data_array = calibrated_fits_object.data
+                # Cast array to float32 if float64
+                if np.issubdtype(data_array.dtype, np.float64):
+                    # Cast to float32 with the conservative casting option
+                    # just incase something weird has happened.
+                    data_array = data_array.astype(np.float32, casting="same_kind")
+
                 # Get the tile size to use for compression. None means use astropy defaults
-                tile_size = self._get_tile_size(calibrated_fits_object.data)
+                tile_size = self._get_tile_size(data_array)
                 # Write frame to disk - compressed
-                hdu = fits.CompImageHDU(
-                    header=l1_header, data=calibrated_fits_object.data, tile_shape=tile_size
-                )
+                hdu = fits.CompImageHDU(header=l1_header, data=data_array, tile_shape=tile_size)
                 formatted_header = reformat_spec214_header(hdu.header)
                 hdu = fits.CompImageHDU(
                     header=formatted_header, data=hdu.data, tile_shape=tile_size
                 )
                 all_tags = self.tags(calibrated_fits_object.name)
                 all_tags.remove(Tag.calibrated())
                 relative_path = self.l1_filename(header=l1_header, stokes=stokes_param)
```

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_assemble_quality.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_assemble_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -970,7 +970,27 @@
         cls=QualityValueEncoder,
     )
     metric = quality_task.quality_build_polcal_efficiency(label=label)
 
     assert metric["name"] == f"PolCal Modulation Efficiency - {label}"
     efficiency_data = metric["efficiency_data"]
     assert efficiency_data["efficiency_list"] == [[1.0, 2.0], [2.0, 3.0]]
+
+
+@pytest.mark.parametrize(
+    "array_shape", [pytest.param((100, 100), id="2D"), pytest.param((100, 100, 100), id="3D")]
+)
+def test_avg_noise_nan_values(quality_task, array_shape):
+    """
+    Given: A data array that contains NaN values
+    When: Computing the noise with `avg_noise`
+    Then: A non-NaN value is returned
+    """
+    rng = np.random.default_rng()
+    data = rng.random(array_shape)
+
+    # Make 1/3 of the px NaNs
+    nan_idx = np.where((data > 0.333) & (data < 0.666))
+    data[nan_idx] = np.nan
+    result = quality_task.avg_noise(data)
+
+    assert not np.isnan(result)
```

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_stems.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_stems.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_submit_dataset_metadata.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_submit_dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_task_name.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_task_name.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_task_parsing.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_task_parsing.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_trial_catalog.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_trial_catalog.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-6.2.3rc1/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 6.2.2
+Version: 6.2.3rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
+changelog/189.misc.rst
+changelog/190.bugfix.rst
+changelog/191.feature.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
 dkist_processing_common.egg-info/requires.txt
 dkist_processing_common.egg-info/top_level.txt
```

### Comparing `dkist-processing-common-6.2.2/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-6.2.3rc1/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/docs/Makefile` & `dkist-processing-common-6.2.3rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/docs/conf.py` & `dkist-processing-common-6.2.3rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/docs/make.bat` & `dkist-processing-common-6.2.3rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/licenses/LICENSE.rst` & `dkist-processing-common-6.2.3rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/pyproject.toml` & `dkist-processing-common-6.2.3rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-6.2.2/setup.cfg` & `dkist-processing-common-6.2.3rc1/setup.cfg`

 * *Files identical despite different names*

